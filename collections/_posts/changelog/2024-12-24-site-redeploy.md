---
layout: changelog
category: changelog
title: Site Redeploy
date: 2024-12-24
---

Just before the end of the year, I've got the new site repo discussed [last time](/2024/12/17/oh-hey-were-back/) deployed through Netlify + Hover. I didn't remember all the details, but thankfully I'd written them up [previously](/2023/01/23/site-live/) and the [Terabyte Tiger](https://terabytetiger.com/lessons/website-deployment-with-hover-and-netlify) guide remains valid.

Setting up a new site in Netlify is very easy: simply connect to your repo through one of the supported git hosts (GitHub, GitLab, Bitbucket, or Azure DevOps), then set your build parameters, and off you go. I'm using Jekyll to build my static site, so to build all I need is build command <code>jekyll build</code>, and then set my publish directory to <code>/site</code>, and Netlify does the rest.

Then, to direct my DNS to the Netlify URL, I log in to my control panel at Hover, navigate to my DNS settings, and add three records: an A record with <code>*</code> for hostname,[^1] directed to Netlify's provided IP address; another A record with <code>@</code> for hostname,[^2] also directed to Netlify's provided IP address; and finally, a CNAME record with <code>www</code> for hostname,[^3] and the target set to my Netlify site's URL. With these three records set, my site is now accessible at either <https://steinea.ca> or <https://www.steinea.ca>, and is provisioned with a TLS certificate by Netlify.

While Sourcehut Pages did handle provisioning a TLS certificate, I unfortunately could not figure out how to get a CNAME working for the site. Documentation and forum discussions were very limited, and the only seemingly conclusive answer was that I would need to serve a second repository with a config file pointing to the <code>www</code> subdomain, which I did not want to do. Netlify handles this much more smoothly, and opens up some cool functionality with environment variables and edge functions.

Some major commits since the last changelog:
* [026ab65](https://github.com/steinea/steinea/commit/026ab6513137c647a74ca2a987e963afc7344740) Added COMMIT_REF environment variables
* [e1d267e](https://github.com/steinea/steinea/commit/e1d267e823a3c8e0bf2ea07b97baa557128f4de4) Added the jekyll-environment-variables gem so this would work
* [a5c1c31](https://github.com/steinea/steinea/commit/a5c1c312fcf5c14af1072a6a1dab0f0ab0ab443b) Added a /slashes page
* [a241013](https://github.com/steinea/steinea/commit/a241013559dd76eec3571a9b051a6a14e0568c87) Added a /verify slash page
* [9a7f50c](https://github.com/steinea/steinea/commit/9a7f50cc1a37eb82b8feaf62153d36a611fbe459) Added my PGP public key
* [0588c48](https://github.com/steinea/steinea/commit/0588c48be658431a0cc5a3049b694b7188d008f3) Added CC BY-NC-SA 4.0 license
* [8266b1e](https://github.com/steinea/steinea/commit/8266b1e2e2b20f6727de0b5bfa374d7b21ccbeaa) Added robots.txt to combat GenAI crawlers
* [dd277a0](https://github.com/steinea/steinea/commit/dd277a0dbb0035de24b16066c753c6e031055bcb) Switched to Latin Modern font (the Pandoc default font)
* *Many Commits* Added all site content (posts, pages, wiki, etc.)

<br>

#### Notes

[^1]: The <code>*</code> record "answers DNS requests for any subdomain you haven't already defined." See <https://kb.porkbun.com/article/94-what-is-a-wildcard-dns-record>.
[^2]: The <code>@</code> record "represents the origin or root of the domain itself." See <https://betterstack.com/community/questions/what-is-the-meaning-of-at-sign-in-a-dns-zone-file/>.
[^3]: With a CNAME record, <code>www</code> is mapped as "an alias name to a true or canonical domain name," in this case my apex domain, <code>steinea.ca</code>. See <https://support.google.com/a/answer/112037?hl=en#zippy=%2Cset-up-cname-records-now>.

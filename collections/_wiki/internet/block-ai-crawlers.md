---
layout: wiki
category: wiki
subcategory: internet
title: Block AI Crawlers
publication: Twitter & GitHub
link: https://x.com/Jay_X_Peet/status/1831437003319386351
date: 2024-09-04
---

"For others wondering how to go about blocking the crawlers:

First step is to have a robots.txt file such as the one used at <https://gameuidatabase.com/robots.txt>. If OpenAI care enough the crawler should read that and then ignore your website but they could one day decide not to...

If you have access to your server config we can explicitly deny the IPs that they say are in use. (Nginx example: <https://gist.github.com/JayPeet/e190fd5a272549ce0a2ff44168aa5a4e>)/ They might change IPs in the future so I will probably end up having to write some kind of API to maintain the deny list for me

There might be a community already tracking this stuff, if anyone knows of that I would love to hear about it.

The changes helped a lot with the website, its getting hammered a lot less (And can continue to be used by real humans who care about creativity and development)"

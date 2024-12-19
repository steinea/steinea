---
layout: wiki
category: wiki
subcategory: internet
title: Mastodon for Static Blog Comments
publication: Carl Schwan
link: https://carlschwan.eu/2020/12/29/adding-comments-to-your-static-blog-with-mastodon/
date: 2024-05-02
---

"One of the biggest disadvantages of static site generators is that they are static and can’t include comments.

There are multiples solutions to solve this problem. You could add a third party blog engine like Disqus, but this has the drawback of including a third-party tool with a bad privacy record in your website. Another solution would be to host an open-source alternative but this comes at the cost of a higher maintenance burden. Having to host a database was something we wanted to avoid with a static site generator.

In my opinion, a better solution is to leverage the Mastodon and Fediverse platform. Mastodon is a decentralized social network and it allows people to communicate with each other without being on the same server. It is inspired by Twitter, but instead of tweeting, you write toot.

When publishing an article, you now only need to also write a simple toot linking to your article. Then Mastodon has a simple API to fetch the answer to your toot. This is the code I made for my Hugo powered blog, but it is easily adaptable for other static site generators. It will create a button to load comments instead of loading them for every visitor so that it decreases the load on your mastodon server."

Follow the link above for code...

---
layout: wiki
category: wiki
subcategory: internet
title: Engineering for Slow Internet
publication: brr
link: https://brr.fyi/posts/engineering-for-slow-internet
date: 2024-09-27
---

"For a 14-month period, while working in Antarctica, I had access to the Internet only through an extremely limited series of satellite links provided by the United States Antarctic Program.

...

It’s a non-trivial feat of engineering to get any Internet at the South Pole! If you’re bored, check out the [South Pole Satellite Communications](https://www.usap.gov/technology/sctnsouthpolesats.cfm) page on the public USAP.gov website, for an overview of the limited selection of satellites available for Polar use.

...

Until very recently, at McMurdo, nearly a thousand people, plus numerous scientific projects and operational workloads, all relied on a series of links that provided max, aggregate speeds of a few dozen megabits per second to the entire station. For comparison, that’s less bandwidth shared by everyone combined than what everyone individually can get on a typical 4g cellular network in an American suburb.

...

As of October 2023, South Pole had the limitations described above, plus there was only connectivity for a few hours a day, when the satellites rose above the horizon and the station was authorized to use them. The satellite schedule generally shifts forward (earlier) by about 4 minutes per day, due to the difference between Sidereal time and Solar (Civil) time.

...

These small intermittent links to the outside world are shared by everyone at Pole, for operational, science, and community / morale usage.

Complicating matters further is the unavoidable physics of this connectivity. These satellites are in a high orbit, thousands of miles up. This means high latency. If you’ve used a consumer satellite product such as HughesNet or ViaSat, you’ll understand.

...

These constraints drastically impact the modern web experience! Some of it is unavoidable. The link characteristics described above are truly bleak. But – a lot of the end-user impact is caused by web and app engineering which fails to take slow/intermittent links into consideration."

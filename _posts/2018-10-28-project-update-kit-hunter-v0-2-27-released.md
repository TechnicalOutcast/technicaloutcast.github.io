---
layout: default
title: Project Update - Kit Hunter v0.2.27 Released
categories: blog
permalink: /blog/:year/:month/:day/:title/
date: 2018-10-28
description: Earlier this summer I wrote about Kit Hunter. Today I updated the core code because I needed to add a brief note explaining the delay as the tags file itself is read.
image: /images/kit_hunter_example.jpg
---

## Kit Hunter Updated to v0.2.27

Earlier this summer I wrote about Kit Hunter, [my Python project for systems administrators][1] that locates phishing kits on web servers. For the most part, most of the updates have centered on the tags file instead of the kit itself. Today I updated the core code because I needed to add a brief note explaining the delay as the tags file itself is read.

Normally, the script takes seconds to load and generate a report, but because the tags file has grown so much, I felt that adding some sort of notice was warranted. Since I changed the core code itself, the version number was updated to reflect it, even if it was a minor change.

## More Changes In The Works

As for the tag file, it’s now at 200 lines, and will detect a majority of the kits currently being traded by scammers online. Today I added about 60 kits worth of new information, and I still have dozens of kits to research. If you’re [following the project on GitHub][2], make sure you grab a new copy or update your forks.

[1]:/data/2018/08/03/learning-python-the-hard-way-kit-hunter-project/

[2]:https://github.com/SteveD3/kit_hunter
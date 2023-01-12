---
layout: default
title: Learning Python the Hard Way - Kit Hunter Project
image: /images/kit_hunter_example.jpg
categories: blog
tags: blog projects python phishing
date: 2018-08-03
permalink: /blog/:year/:month/:day/:title/
description: So I wanted to learn Python, and I figured the best way to do so would be a project of some kind. Since Phishing research is a hobby and interest of mine, that’s where I started.
---

## I’ve started to code in Python

So I wanted to learn Python, and I figured the best way to do so would be a project of some kind. Since phishing research is a hobby and interest of mine, that’s where I started. My first adventure into Python turned out to be a looped search tool, which eventually became Kit Hunter.

## It’s designed for administrators

Kit Hunter is made for server administrators, as they can place the script outside of the document root (e.g. public_html) and locate phishing kits that have been uploaded to the server. As I mention on GitHub:

>Kit Hunter is a basic scanning tool that will search directories and locate phishing kits based on established markers. As detection happens, a report is generated for administrators.
The report is basic:
* The opening line points the administrator to the directory where detection took place.
* After that, the log reports the exact file name that caused the detection.
* Line three shows the tag responsible for the warning in the first place.
* Finally, the log displays the complete line of code where the tag is visible.

For my old day job at CSO Online, [I wrote about Kit Hunter][1] and created a video showing it off. The video is below. If you want to check out the script, feel free to do so [over at GitHub][2].

<iframe width="560" height="315" src="https://www.youtube.com/embed/Fqkvu1cg6oo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[1]:https://www.csoonline.com/article/3290945/salted-hash-introducing-kit-hunter-a-phishing-kit-detection-script.html

[2]:https://github.com/SteveD3/kit_hunter

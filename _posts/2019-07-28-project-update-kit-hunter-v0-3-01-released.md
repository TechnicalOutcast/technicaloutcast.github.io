---
layout: default
title: Project Update - Kit Hunter v0.3.01 Released
image: /images/kit_hunter_example.jpg
categories: blog
tags: blog projects python phishing
date: 2019-07-28
permalink: /blog/:year/:month/:day/:title/
description: I sorted 66 phishing kits today and added new tags to help identify them. These updates will also likely discover other kits that are likely to be developed from the base code.
---

## Kit Hunter Updated to v0.3.01
It's been a while since I've written about Kit Hunter, the project I [first started last summer][1] in order to learn more about Python.

Life has been a bit hectic, so I haven't updated it as much as I want, but I sorted 66 phishing kits today and added new tags to help identify them. These updates will also likely discover other kits that are likely to be developed from the base code.

## Future Plans
I still have hundreds of other kits to sort, but the updates today focused on core phishing kit operations. Most of the unsorted kits will be detected anyway, as I'm focusing on elements that verify bin numbers, victim geographic details, logging, and security checks.

## Development Advantages
The interesting thing about phishing kits, and part of what makes Kit Hunter work so well, is that most kit developers recycle code and functions.

They do this, not because they're lazy (though they are), but because the base functions work, and it doesn't make sense to _**"fix"**_ something that isn't broke.

However, anyone who has ever worked in security knows that holding to such a mindset comes with plenty of risks. In this case the risk and failure is that phishing kits developed with recycled (or hijacked) code are easy to detect and remove.

Feel free to [download Kit Hunter][2] and run it on your web servers. It's a good baseline tool to have handy when hunting for shady things in your environment.

[1]:/data/2018/08/03/learning-python-the-hard-way-kit-hunter-project/

[2]:https://github.com/SteveD3/kit_hunter

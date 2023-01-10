---
layout: default
title: Welcome!
description: Technical Outcast is a new project from Steve Ragan. In addition to security, Technical Outcast will focus on other areas of technology, including privacy, policy, code, and more.
image: /images/header-image.jpg
---

<img src="/images/header-image.jpg">

# Welcome!

Technical Outcast is a new project from Steve Ragan.

This website was launched in the summer of 2018 with a goal of delivering news, analysis, and opinions related to the security sector. In addition, Technical Outcast will focus on other areas of technology, including privacy, policy, code, and more.

One of the main themes on Technical Outcast will be security education, geared towards those who live outside of the echo chamber. Please feel free to have a look around and reach out if you have questions or ideas.
<hr>
<table>
  {% for post in site.posts limit:4 %}
  <tr>
    <td>{{ post.date | date_to_string }}</td>
    <td><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></td>
  </tr>
  {% endfor %}
</table>

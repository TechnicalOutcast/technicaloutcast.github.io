---
layout: default
title: HackBot&#58; An AI-driven security chatbot
image: /images/hackbot.jpg
categories: blog
tags: blog random artificial-intelligence Meta-LLama2 vulnerabilities code-analysis
date: 2023-08-22
permalink: /blog/:year/:month/:day/:title/
description: HackBot is an AI-driven chatbot designed to provide helpful and accurate answers to various cybersecurity-related queries, while also doing code and vulnerability analysis.
---

So I came across something pretty neat in my blog feed the other day. A project on GitHub by [morpheuslord](https://twitter.com/morpheuslord2), aims to answer basic security questions, while providing some static code analysis, and vulnerability analysis.

I love little projects like this. Given that I've been doing a lot of research into artificial intelligence lately, a Meta-LLama2 driven script certainly caught my attention.

From the project page:

>Welcome to HackBot, an AI-powered cybersecurity chatbot designed to provide helpful and accurate answers to your cybersecurity-related queries and also do code analysis and scan analysis. Whether you are a security researcher, an ethical hacker, or just curious about cybersecurity, HackBot is here to assist you in finding the information you need.
><br><br>
>HackBot utilizes the powerful language model Meta-LLama2 through the "LlamaCpp" library. This allows HackBot to respond to your questions in a coherent and relevant manner.

Some of the features listed include:
* HackBot can answer various cybersecurity-related queries, helping you with penetration testing, security analysis, and more.<br><br>
* Static Code Analysis: Utilizes the provided scan data or log file for conducting static code analysis. It thoroughly examines the source code without executing it, identifying potential vulnerabilities, coding errors, and security issues.<br><br>
* Vulnerability Analysis: Performs a comprehensive vulnerability analysis using the provided scan data or log file. It identifies and assesses security weaknesses, misconfigurations, and potential exploits present in the target system or network.

The project is only a few weeks old, and there is a note for those with a "know-how of training text generation models" to help contribute. It's certainly worth watching and trying out.

You can install HackBot by following the directions over on GitHub:
[https://github.com/morpheuslord/HackBot](https://github.com/morpheuslord/HackBot)

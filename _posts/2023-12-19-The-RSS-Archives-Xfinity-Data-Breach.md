---
layout: default
title: The RSS Archives&#58; 36 million impacted by Xfinity Data breach&#44; passwords reset
image: /images/news_recaps.jpg
categories: blog
tags: blog RSS OpenAI data-breach passwords vulnerabilities Comcast-Xfinity Citrix
date: 2023-12-19
permalink: /blog/:year/:month/:day/:title/
description: Another Citrix-related incident. Passwords have been forced to reset after 36M people were determined to be affected by the Xfinity data breach.
---

Quick update this morning. I was forced to change my Xfinity account, an action related to the fallout over the data breach Comcast disclosed on Monday impacting nearly 36M people.

### 36M people impacted by Xfinity data breach

#### Source: [Business Wire](https://www.businesswire.com/news/home/20231218979935/en/Notice-To-Customers-of-Data-Security-Incident/), [Comcast](https://assets.xfinity.com/assets/dotcom/learn/Notice%20To%20Customers%20of%20Data%20Security%20Incident.pdf?INTCMP=dsi-12152023), [Maine Attorney General](https://apps.web.maine.gov/online/aeviewer/ME/40/49e711c6-e27c-4340-867c-9a529ab3ca2c.shtml)

Xfinity has issued a notice regarding a data breach that occurred between October 16 and 19, 2023. The incident affects 35,879,455 customers. The breach was linked to a vulnerability in Citrix software ([CVE-2023-4966](https://www.netscaler.com/blog/news/cve-2023-4966-critical-security-update-now-available-for-netscaler-adc-and-netscaler-gateway/)), which Xfinity uses along with thousands of other companies. Despite prompt action to patch and mitigate this vulnerability, unauthorized access to Xfinity's internal systems was detected during a routine cybersecurity exercise on October 25, 2023. On November 16, 2023, Xfinity determined that information was likely acquired by the attackers, and the scope of the compromised data was confirmed on December 6, 2023.

The compromised data potentially includes usernames, hashed passwords, names, contact information, parts of social security numbers, dates of birth, and security questions and answers. Xfinity has required password resets for affected accounts and recommends customers enable two-factor or multi-factor authentication. A dedicated call center has been established for customer inquiries (888-799-2560), operating Monday through Friday
from 9:00 AM to 9:00 PM EST.

The incident is still under investigation.

CISA has released two advisories related to the Citrix issue Comcast references.<br>
* [Alert Code: AA23-325A](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-325ahttps://www.cisa.gov/news-events/cybersecurity-advisories/aa23-325a) - On how Lockbit 3.0 is leveraging the vulnerability.
* [General Guidance](https://www.cisa.gov/guidance-addressing-citrix-netscaler-adc-and-gateway-vulnerability-cve-2023-4966-citrix-bleed) on the Citrix Bleed vulnerability.

>**Observations:**<br>
>This isn't the first time passwords have had to be reset due to a data breach. As one of the world's largest ISPs, Comcast (Xfinity) is no stranger to the painful process of defending their systems and customer accounts. This incident highlights the struggle security practitioners face each day. Comcast did the right thing, they patched as soon as possible, but it still wasn't enough.
><br><br>
>After patching, it's clear from the company statement that their security team continued to check to see if there was any impact related to the Citrix vulnerability. Now, how they determined this, and what actions were taken during their assessments is unknown. Clearly they were checking access logs in some way and they were able to connect the dots. It would be nice to see an overview of their assessment, but that is unlikely to happen.
><br><br>
>On another note, my forced password reset this morning reminded me of a news item I wrote years ago. Back then, 200,000 people had to go through the process after their accounts were exposed within a [list of passwords being sold on the darknet](https://www.csoonline.com/article/553519/comcast-resets-nearly-200000-passwords-after-customer-list-goes-on-sale.html). Also, last year there were the [credential stuffing attacks that targeted Xfinity users](https://www.bleepingcomputer.com/news/security/comcast-xfinity-accounts-hacked-in-widespread-2fa-bypass-attacks/), so there is a clear concern this could happen again.
><br><br>
>The likely compromise of password reset questions and answers is concerning. People likely reuse those prompts on other websites, and now those accounts are vulnerable to attack as well. Security questions and answers are reused, not because people are lazy, but because they're forced to reuse them.
><br><br>
>In many cases, identity protection systems put the user and their accounts in an unwinnable game of guess the answer, where the answer can be a bit of personal trivia, or an easily guessed phrase or word. They're limited to a set of questions, and the fear they'll forget those answers and lose recovery options is what keeps them using the same questions and answers over and over again.
><br><br>
>There are a few clever ways to mitigate the security question problem (using sentences that are unrelated to the question, storing complex strings for the answer in a password manager, etc.), but most people won't use them (again, they're afraid to take this path), leaving MFA as the main defense. But when one-time-passwords (OTPs, the code sent via text message to the users) are the only option available, and OTPs can be bypassed, the cat and mouse game keeps going. It's frustrating.
{: .box-news }

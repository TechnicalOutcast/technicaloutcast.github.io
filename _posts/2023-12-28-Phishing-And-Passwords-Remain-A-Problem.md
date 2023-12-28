---
layout: default
title: Phishing and Passwords Remain Top Concern for IT Pros
image: /images/stock/login_screen.jpg
categories: news
tags: news phishing passwords credential-stuffing scams fraud RSS
date: 2023-12-28
permalink: /news/:year/:month/:day/:title/
description: Passwords remain a problem for IT professionals, who are greatly concerned about phishing and its impact within the enterprise.
---

I've been reading the _"2023 State of Authentication Survey"_ by [Axiad][1], which highlights an ongoing struggle within organizations to transition away from password-based security systems.

This is an area I'm obsessed with honestly, because most of my career has been focused on passwords, phishing, and social engineering; by either using them in attacks, or advising organizations on how to defend against said attacks from implementation, to detection and response.  

The report is based on a survey of 200 IT professionals. While that's a small number, the concerns, issues, and problems highlighted by the survey's responses demonstrate a grim reality that IT and Security staffers are faced with the world over on a daily basis.

The gist of the report is this:

Despite the known risks of passwords, which are implicated in over 80% of data breaches (source: FIDO Alliance), the majority of organizations continue to rely on them as their primary authentication method. Phishing is considered the most significant threat to the organization, with 39% of respondents listing it as a top concern and 49% believing it to be the most likely attack to occur. But, there is a bit of a disconnect, because while 89% of the respondents are confident can face phishing attacks head on, only 22% use phishing-resistant multi-factor authentication (MFA) or passwordless tech.

The report emphasizes the critical need for organizations to move towards more secure authentication methods, such as passwordless and phishing-resistant MFA. It underscores the role of industry guidance (e.g., CISA and NIST) in influencing this shift, with organizations gradually recognizing the importance of evolving their cybersecurity strategies in response to increasing phishing attacks and other credential-based threats.

### Why Passwords Remain
Drilling down into the report, one of the focal points centers on why passwords are still the main driver for access and protection within the organization. According to the respondents, the reasoning is mixed.

* Fear of change (64%)
* The perceived need to replace existing technology (54%)
* Time constraints (51%)
* Staffing limitations (25%).

All of this is understandable. Each point is honestly a valid reason as to why passwords are still being used despite their shortcomings. No two organizations are alike. Their needs and goals will shift with time, and their ability to adapt every aspect of their technology stack - including passwords - can be somewhat limited. But there has to be some movement somewhere, because stagnant security is why we're seeing so many ransomware incidents. Access brokers target weak authentication and access control points, often by using an organization's own passwords against them.

It isn't like awareness around technology to defend against password breaches doesn't exist. It's there, but planning and deployment takes time. 72% of the respondents said they plan to implement some sort of passwordless or phishing-resistant technology within their organization in the near future.

### Fixing the Blame
According to Axiad, responsibility for password breaches is divided among IT staff (35%), end users (32%), and security teams (25%). It is interesting to note that 8% of the respondents said that leadership is responsible, and it isn't clear why.

If leadership is responsible because they approve budgets, then there is a deeper issue at play. If the leadership is singled out because they are the managers of the authentication systems, then I'd argue that they're rolled under IT or Security. Ultimately, the responsibility falls to IT and Security, as victim blaming and end user blaming doesn't solve anything.

At the same time, blaming IT and Security for password problems is really an oversimplification. Sure, sometimes someone will screw up and do something that leads to an incident, but other times incidents happen because these teams are forced to work with inefficient technology, processes, or regulations that expose them to password-based attacks. The risk of such was just accepted as part of the business.

### Overconfidence
88% of the survey respondents said their company was prepared for a password-based attack (phishing or otherwise), and yet, 52% said they had experienced such an attack in the recent past. At least, that is the context presented in the report itself. Presuming the mentioned successful attacks happened within the past year, which I admit is a bit of a leap, there is a clear case to be made for overconfidence.

Access and authentication technologies, which guard applications, services, and systems, are not something that can be switched on, configured, and then left alone. They need to be monitored, tuned, and adjusted on a regular basis in order to address business growth, shifting priorities, and changes to threat and risk models.

The gaps in this process is where criminals thrive. Phishing attacks against users target the active base, while credential stuffing looks to target both the active base and the inactive base, where the inactive base could consist of aged accounts, former staff, or forgotten / non-inventoried systems. Criminals will use this access as a launchpad for further harm, and the main defense starts with a seriously detailed and finely tuned identity access management and control system.

### A Bigger Problem
But the problem is, these sort of systems take time to implement. Depending on the size of the organization, from beginning to end the implementation can be costly. This cost isn't just the vendor charge either, it's the hourly labor cost of dealing with password-related incidents and helpdesk tickets too. This is why starting with a strong authentication posture is so important.

Yet, you can't just _start_ with strong authentication in many cases, because most organizations inherited their password problems. They were founded at a time when passwords were the main defense against unauthorized use and access, and there wasn't much anyone could do about attacks against them. So as changes are designed and pushed out, the costs associated with password defense starts to mount.

Users just want to get their work done, so overly complex password requirements and processes slow them down. When that happens, users will turn to solutions that fall within the rules, but result in weak and risky defense postures. Examples of this can be pattern-based passwords that are easily cracked or guessed, recycled passwords, or a mix of both.   

So there is a trade to be made. __Ease of use__ vs. __Management and control__. Often you'll see organizations do staged rollouts of passwordless and phishing-resistant tech, where the most critical systems and services are brought online first, followed by systems and services that see moderate, but consistent use.

### Passwords Are a Problem
At the end of the day, passwords are a problem. They can't be trusted to protect an organization on their own. While the Axiad survey has a small pool of respondents, the overall picture painted is all too common these days. Between the pressures of doing more with less faced by IT and Security teams, and end users who just want to get their work finished, criminals have carved out a nice little niche on the attack surface that they can exploit over and over again.

Passwordless and phishing-resistant tech is the strongest defense at play, but it isn't a silver bullet. Such solutions need to be backed by proactive monitoring and tuning, and implemented in such a way that scaling isn't a problem.

[1]: https://www.axiad.com/blog/pdfviewer/axiad-state-of-authentication-survey-q4-2023-infographic/

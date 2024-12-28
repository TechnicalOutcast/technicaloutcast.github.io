---
layout: default
title: RSS Recap January 2024 Volume 1
image: /images/news_recaps5.jpg
categories: news
tags: news RSS OpenAI data-breach healthcare government passwords ransomware
date: 2024-01-09
permalink: /blog/:year/:month/:day/:title/
description: This is the first edition of my news recap series.
---

I've been doing some reading, and figured I'd share what I've found interesting in a quick recap. This is a continuation of the RSS Archives series. With a recap of the things I've found while reading my various RSS feeds.

<hr>
**Key cybersecurity skills gap statistics you should be aware of**

#### Source: [Help Net Security](https://www.helpnetsecurity.com/2024/01/02/cybersecurity-skills-gap-statistics/)

As cyber threats intensify, the demand for skilled cybersecurity professionals is at an all-time high, highlighting a critical skills gap. This gap poses significant vulnerabilities in business and institutional defense mechanisms, with shortages in key areas like penetration testing and threat analysis. Factors contributing to this gap are multifaceted, including workforce diversity and ongoing skill development.

Other notable findings include an anticipated improvement in the cloud skills gap, reevaluation of degree requirements for entry-level jobs, and a growing focus on soft skills in cybersecurity roles. The article also notes challenges such as a rise in cybersecurity staff burnout, layoffs exacerbating skills gaps, and unrealistic job expectations.

Additionally, there's an increasing demand for STEM training and internal tech skill development within organizations, despite cost-cutting measures. A worrying trend is the lack of cybersecurity experts and incident response plans in mid-sized businesses. Lastly, the article highlights the extended time it now takes for companies to fill critical cybersecurity positions.

<hr>
**Aliquippa water authority in Pennsylvania hit by Iranian cyberattack**

#### Source: [Fortune](https://fortune.com/2024/01/02/aliquippa-water-authority-pennsylvania-iranian-cyberattack/)

The Municipal Water Authority of Aliquippa, Pennsylvania, a small authority, was unexpectedly targeted by Iranian-backed hackers. These hackers attacked several U.S. water utilities, exploiting an Israeli-made equipment vulnerability.

>“If you told me to list 10 things that would go wrong with our water authority, this would not be on the list,” said Matthew Mottes, the chairman of the authority that handles water and wastewater for about 22,000 people in the woodsy exurbs around a one-time steel town outside Pittsburgh.

This incident has raised serious concerns about water utility cybersecurity in the U.S., highlighting the potential for hackers to disrupt or contaminate water supplies. Challenges in addressing cybersecurity in this sector include financial constraints, lack of expertise, and resistance to perceived privatization.

Some states have enacted legislation to enhance cybersecurity, but efforts are hindered by limited funding and opposition to regulations. The EPA's attempted regulation faced legal challenges and was withdrawn, while public water authorities are seeking legislative solutions. Meanwhile, cybersecurity companies like Dragos Inc. are offering support to under-resourced utilities.

<hr>
**LastPass Hikes Password Requirements to 12 Characters**

#### Source: [Security Boulevard](https://securityboulevard.com/2024/01/embattled-lastpass-enforcing-12-character-passwords-for-all/), [BleepingComputer](https://www.bleepingcomputer.com/news/security/lastpass-now-requires-12-character-master-passwords-for-better-security/)

LastPass, grappling with the fallout from significant data breaches in 2022, has escalated its security protocols for users' master passwords. Amidst criticisms from the cybersecurity community and a need for greater transparency, LastPass now mandates a minimum of 12 characters for all master passwords. This change, while not novel (having been the default since 2018) could previously be bypassed by users. As of April 2023, new users and those resetting passwords were required to adhere to this standard, and now, the enforcement extends to all existing accounts.

Additionally, LastPass will start cross-referencing new or reset passwords against a breached credentials database. This move is to prevent users from unknowingly selecting compromised passwords. Users with matches to known breached credentials will receive alerts to change their passwords. T

These measures follow two severe breaches in August and November 2022, where threat actors accessed source code, technical information, and LastPass internal system secrets, leading to substantial data theft, including customer vault data. In October 2023, hackers exploited this stolen information to extract $4.4 million in cryptocurrency from victims.

>**Side Note:**<br>
> I [wrote about the LastPass incidents last year](https://technicaloutcast.com/news/2023/01/14/lastpass-data-breach-timeline-need-to-know/), right around this time to be exact. It directly impacted my family, so I took a keen interest in it. I was already watching the news unfold due to my job, but this hit close to home. What I said then, holds true now.
><br><br>
>"The LastPass incident isn’t just about a data breach. The data the criminals compromised can also lead to phishing attacks that leverage the LastPass incident as a lure. Clearly this can cause additional knock-on problems for the victims in this case."
{: .box-news }

<hr>
**Weak Password and Infostealer Blamed for Orange Spain Outage**

#### Source: [The Register](https://www.theregister.com/2024/01/04/orange_spain_outage_breach/)

Orange Spain, the country's second-largest network provider, recently faced a massive network outage. The culprit? A combination of infostealer malware and a weak password. The RIPE account of Orange Spain, a vital component in managing of IP addresses and routing, was compromised  by an individual known as "Snow," who demonstrated the attack's execution through shared screenshots. 'Snow' exploited this access to disrupt nearly half of the network's traffic.

Analysis of these images by Hudson Rock researchers revealed that the RIPE account was accessed using credentials harvested by infostealer malware, which had infected an employee's account at Orange Spain. The password used, "ripeadmin," was criticized for being strikingly weak and guessable, highlighting a significant oversight in password management.

This incident underscores the devastating impact a single infostealer infection can have on a company. Security expert Kevin Beaumont pointed out that RIPE, unlike its North American counterpart ARIN, doesn't mandate the use of multi-factor authentication (MFA) or have a robust password policy, making it a veritable 'powder keg' of security vulnerabilities. The breach led to the hijacking of the provider's border gateway protocol (BGP) traffic by the attacker, causing a severe service outage. This was achieved by altering the autonomous system number and route origin authorizations associated with Orange Spain's IP address.

While Orange Spain confirmed the breach and the subsequent restoration of services, they assured that no customer or client data was compromised during the incident. However, the severity of the breach and the simplicity of the attack method have raised concerns in the cybersecurity community. Beaumont noted the prevalence of RIPE account credentials on infostealer marketplaces, suggesting that similar attacks might become more common.

<hr>
**Breach at Defunct Boston Ambulance Service Impacts 900,000+**

#### Source: [SecurityWeek](https://www.securityweek.com/over-900k-impacted-by-data-breach-at-defunct-boston-ambulance-service/)

Over 900,000 individuals' personal data was compromised in a breach at Fallon Ambulance Service, a now-defunct subsidiary of Transformative Healthcare. This breach, detected on April 23, 2023, occurred after the ambulance service ceased operations but retained archived data. The compromised data included sensitive personal and medical information.

Transformative, offering free identity protection services, reported that the Alphv/BlackCat ransomware group claimed responsibility for this breach, part of their wider attacks on over 1,000 entities before law enforcement targeted their operations.

<hr>
**Nigerian Hacker Arrested for Stealing $7.5M from Charities**

#### Source: [BleepingComputer](https://www.bleepingcomputer.com/news/security/nigerian-hacker-arrested-for-stealing-75m-from-charities/)

Olusegun Samson Adejorin was apprehended in Ghana for orchestrating business email compromise attacks against U.S. charities, leading to a loss of over $7.5 million. This complex fraud, executed between June and August 2020, involved impersonating charity employees and manipulating email communications to divert large fund transfers.

Adejorin faces up to 20 years for wire fraud, five years for unauthorized computer access, and two years for identity theft, with potential additional penalties. This case is just another example of the significant financial damage caused by BEC attacks and underscores the need for robust email security defenses.

---
layout: default
title: loanDepot Breach Disclosure Outlines Successful Phishing Attack
image: /images/post-images/loanDepot/loanDepot.jpg
categories: news
tags: news RSS OpenAI data-breach identity phishing passwords
date: 2024-01-23
permalink: /blog/:year/:month/:day/:title/
description: A breach notification from loanDepot in 2023 outlines a textbook example of a phishing attack, and the threat actor's TTPs.
---

I'm reading my RSS feeds this morning and see several news items discussing the loanDepot ransomware attack disclosure.
[**Source:** [Bleeping Computer](https://www.bleepingcomputer.com/news/security/us-mortgage-lender-loandepot-confirms-ransomware-attack/), [8-K filing](https://www.sec.gov/Archives/edgar/data/1831631/000183163124000004/ldi-20240104.htm)]

News of the ransomware incident started to break on January 6, 2024, after disruptions were observed by mortgage customers on the company's website. The breach was quietly investigated by law enforcement and the company's information security team. loanDepot has not yet provided specific details about the kinds of information accessed or the extent of the data encrypted.

However, while that certainly sucks, because ransomware is just a blight on the world and I feel for the IT teams at loanDepot, the news reminded me of a different disclosure made last summer.

This isn't the first time loanDepot has had problems. Last summer, loanDepot disclosed a textbook example of a phishing attack from start to finish, which was indicative of previous attacks targeting Exchange, Office365, and Google Workspace users.
<hr>

#### Phishing is a Numbers Game
In May of 2023, loanDepot disclosed that it was successfully phished. The phishing attack started with 215 emails to employees, and leveraged the Zix platform for encryption, which helped the attackers bypass loanDepot's email security controls. Of the 215 employees targeted, four (4) were successfully phished and provided their Office365 credentials to the threat actors.

Zix is a secure messaging service, often used to share sensitive documents. In 2021, researchers discovered Zix being [used as a phishing lure](https://blog.knowbe4.com/phishing-campaign-impersonates-zix-messages) to target accounts on multiple platforms including Office365, Google Workspace, and Exchange.
{: .box-warning }

While the threat actors likely wanted more than four victims, the attack was still a good return on the investment made. Email lists are abundant, cheap, and easily customized. Attacks using a template, such as Zix, are easily automated and can be ran 24/7. Spoofing headers so that the emails appear to come from Zix, or using compromised Zix accounts to implement an attack is also a viable, yet low-cost option available to criminals. So with little effort, the threat actors responsible for the 2022 incident managed to score valid accounts within a major financial firm.
{: .box-news }

#### Pivoting and Bypassing MFA
The phishing attack happened on August 2, 2022. The threat actors wasted no time, because on August 3, they attempted to access the accounts provisioned to the four employees who fell for the scheme.

Multi-factor authentication (MFA) initially prevented this access, but the threat actors shifted to a legacy authentication protocol. The legacy method used was not disclosed by loanDepot, but based on the changes made after the incident, it is possible the threat actors used push-notification fatigue. No matter what, it was by shifting to the legacy protocol that the threat actors were able to bypass loanDepot's MFA controls and obtain access.

For those not familiar, push-notification fatigue is when a threat actor will blast the victim with so many notification approval requests they will eventually - either out of frustration or on accident - just accept the request in order to make the flood of notices stop.
{: .box-warning }

MFA bypasses are common in phishing attacks, because MFA has become a common standard to protect identities. However, not all MFA is equal. Criminals have started to target push notifications, weak or fragmented implementations, SMS-driven one-time passwords (OTPs), etc., in order to lower the effectiveness of MFA.
{: .box-news }

#### Bypassing Access Controls
Internal controls at loanDepot block network access from non-US IP address. However, the threat actors simply pivoted to using US-based VPN, which rendered those IP blocks useless. Once they successfully bypassed all controls, access to the four phished loanDepot accounts was granted.

The criminals chose a common and easy path. Matching their location to that which the victim is likely to expect and allow, is a core element of the post-compromise process during an attack like this. You see VPN services being sold or traded in criminal markets all the time.
{: .box-news }

As an example, many banking scams require a threat actor to use localized VPN or proxy services in order to be successful. So in addition to a set of fullz, most bank fraud packages include VPN access tied to the location of those represented within the records, or remote systems within the geographic area.
{: .box-news }

Fullz are the records and information needed to spoof or access a banking customer, or establish a false identity in order to fraudulently open an account.
{: .box-warning }

#### Some Positive News
The incident was detected and resolved within three hours, thanks largely to loanDepot employees who reported suspicious emails as phishing to the IT department. This is good news, but phishing is a numbers game. While some employees reported the attempts, not everyone did. In the end, all the threat actors needed were the four victims they came out with.

Humans are the best form of early-warning system. While their detections might not be perfect, and false positives are common, they can still find and report things that email security settings and filters might miss. The fact that the staff at loanDepot were trained to spot potential problems, and comfortable reporting their suspicions immediately (even if they could be wrong) is wonderful news.
{: .box-news }

#### Impact and Scale
An investigation into the incident revealed that the threat actors could have accessed all of the information the four successfully phished accounts had permissions to. After a manual review of 42,440 documents, it was discovered that 1,364 people were impacted.

The records compromised by the threat actors across the four accounts included images, handwritten documents, and more, exposing names, Social Security Numbers, and other sensitive details. Essentially, consider all of the documentation that goes into a mortgage, and it would be a safe bet that some (if not all) of data that was compromised at the time.

The company says their "nationwide team of 6,000-plus members" assist "more than 27,000 customers" monthly. By that count, the August 2022 incident (disclosed in May, 2023, eight months later) impacted just about 5% of their customer base.

The disclosure delay was due to the time it took to process the manual review.

That all of this came from just four accounts is frightening. What would have happened if the threat actors managed to get all 215?
{: .box-news }

#### Recovery
loanDepot forced password and active session resets for all employees as part of their recovery, which is said to have terminated the threat actor's access to the network.

In addition, loanDepot said they've taken further protection steps including disabling legacy authentication protocols and moving from an approve-or-deny method of MFA, to code-matching MFA. They company also increased the cadence of its phishing awareness training from quarterly to monthly.

This move from approve-or-deny to code-matching is why I think the threat actors used notification fatigue.
{: .box-news }

image: [NYSE](https://twitter.com/NYSE/status/1363933517474721797/photo/1)

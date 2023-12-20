---
layout: default
title: The RSS Archives&#58; Hacktivists Hit Iran Petrol Stations
image: /images/news_recaps.jpg
categories: blog
tags: blog RSS OpenAI data-breach passwords ransomware government
date: 2023-12-20
permalink: /blog/:year/:month/:day/:title/
description: Critical infrastructure attacks hit Iran, Mr.Cooper data breach likely the worst one of 2023.
---

Here's a quick look at the headlines I'm reading this morning. Naturally, [the Comcast breach](https://technicaloutcast.com/blog/2023/12/19/The-RSS-Archives-Xfinity-Data-Breach) is the main focus of coverage in my news feeds today, followed by thge Mr. Cooper data breach (covered below). But there are some other stories worth noting.

<hr>
### Iran Petrol Stations Hit by Cyberattack, Oil Minister Says

#### Source: [Reuters](https://www.reuters.com/world/middle-east/iran-petrol-stations-hit-by-cyberattack-oil-minister-says-2023-12-18/)

On December 18, 2023, approximately 70% of Iran's fuel stations experienced disruptions due to a cyberattack. Iranian Oil Minister Javad Owji confirmed that the IT systems of the nation's petrol stations were targeted. The attack led to long queues at gas stations across the country. The incident has been attributed to a software problem within the fuel system, as acknowledged by Reza Navar, spokesperson for Iran's gas stations association. While experts are working on fixing the issue, the possibility of a cyberattack has not been entirely ruled out.

Iranian authorities have [pointed to an Israeli-linked group](https://t.me/GonjeshkeDarandeOfficial/3) (Telegram), Predatory Sparrow (a.k.a. Gonjeshke Darande), as being responsible for the disruptions. Reports suggest that the cyberattack was politically motivated, potentially implicating international elements in the incident. On Twitter, Gonjeshke Darande reposted their claims from Telegram, and added "A month ago we warned you that we’re back and that we will impose cost for your provocations. This is just a taste of what we have in store."

![Gonjeshke Darande post on Twitter claiming responsibility for the attack.](https://technicaloutcast.com/images/post-images/RSS/GonjeshkeDarande.jpg)

>**Observations:**<br>
>Attacks against critical infrastructure are a serious threat, no matter who owns and operates these assets. Hacktivist groups have always focused their efforts on disruption of some sort, and in some cases have used these disruptive acts as a means to enage in other cyber objectives such as data exfiltration or the installation of malware, which can be used to stage additional attacks. Because of the nature of OT, IoT, SCADA, and ICS equipment, as well as the contracts that come with such investments, it isn't always possible to just patch or update. In fact, most of these assets are often required to be placed in a visible part of the network, making constant defense a critical, but often near-impossible task.
><br><br>
>Protecting critical infrastructure is a prime example of a goal where no single vendor has all the answers. It isn't something you can just throw money at, or purchase a product license for. While there are vendor elements at play, there also has to be a focus on supply chain management and protection, local and national government support, legal alignment (laws and regulation), and strong partnerships between the public and private sectors. Cyber attacks have no border, and the world is just now starting to come to grips with the need to protect something that really wasn't designed to integrate  with the networks of today, nor was it designed to withstand attacks that are now commonplace.
{: .box-news }

<hr>
### Financial Sector Experiences More Cyberattacks Than Other Verticals

#### Source: [Netwrix](https://www.netwrix.com/the-financial-sector-experiences-more-cyberattacks-than-other-verticals-and-those-incidents-result-in-costlier-outcomes.html)

A recent report from Netwrix highlighted that 77% of financial organizations detected a cyberattack on their infrastructure in the past 12 months, a significantly higher rate compared to 68% among other sectors. Phishing and ransomware were identified as the most common types of attacks across all sectors. Based on the findings, 39% of financial organizations reported targeted attacks on their cloud infrastructure and 26% experienced attacks on their on-premises systems. These figures surpass the overall industry rates of 30% for cloud and 19% for on-premises attacks.

Moreover, the financial sector also incurs higher costs due to cyberattacks compared to other industries. About 24% of financial organizations estimated their damages from such incidents to be at least $50,000, compared to only 16% among other industries. To mitigate these risks, 73% of financial sector respondents either have a cyber insurance policy or plan to acquire one within the next year. This is in contrast to just 59% in other industries. However, due to the high-risk nature of the financial sector, insurance companies often impose more stringent security requirements. For instance, 49% of financial organizations needed to enhance identity and access management, and 48% had to comply with privileged access management standards, compared to 38% and 36%, respectively, in other sectors.

>**Observations:**<br>
> What's the old saying? Criminals target banks because that's where the money is? It isn't just money these days though, information is a currency all on its own. The data used to generate this report comes from 1,610 IT professionals from 106 countries, so while the base isn't too big, it's large enough to give a decent picture. It shouldn't shock anyone to learn that the financial sector is the most targeted, nor that phishing and ransomware are the most common threats.
><br><br>
>The interesting thing  in this report for me was the requirements that insurance companies are pushing. Stronger identity and access controls are vital protection elements, and the idea that identity (people, applications, services) needs to be completely managed and controlled is one of those things that everyone knows is true, but it's easier said than done. But the notion that insurance vendors are forcing the issue is a net positive in my opinion. On the money side of things, I think the $50,000 benchmark is a bit low, given the resources and impact a ransomware attack can have on a mid-level enterprise.
{: .box-news }

<hr>
### 14M Impacted by Mr. Cooper Hack

#### Source: [TechCrunch](https://techcrunch.com/2023/12/18/mr-cooper-hackers-stole-personal-data-on-14-million-customers/)

Hackers breached the systems of Mr. Cooper, a major mortgage and loan company, and stole sensitive personal information of over 14.6 million customers. The stolen data includes customer names, addresses, dates of birth, phone numbers, Social Security numbers, and bank account numbers. While Mr. Cooper previously indicated that customer banking information, stored by a third-party company, was believed to be unaffected, the scale of the breach suggests otherwise.

This incident has impacted "substantially all" of Mr. Cooper's current and former customers, exceeding the four million existing customers mentioned on the company's website. The breach also includes data from customers whose mortgages were previously acquired or serviced by the company when it was known as Nationstar Mortgage, before its rebranding. Customers from a sister brand of Mr. Cooper might also be affected.

On October 31, the day of the breach, Mr. Cooper initially reported its systems were offline due to an outage, which was later confirmed to be related to a cybersecurity incident. Customers experienced difficulties in accessing their accounts and making mortgage payments. The company has not disclosed the specific type of cyberattack it suffered and has declined to comment on whether it received any demands from the hackers.
>**Observations:**<br>
> This is bad. The amount of information available on each compromised mortgage record is staggering. Criminals can use this data for all sorts of fraud and attacks. Even worse, they can use it to augment existing victim records and update things with newer information. For those not aware, criminals do compile complete profiles on potential victims and sell or trade this information. The profiles are used for credit fraud, ID fraud, and more. While the numbers might not be as high as Comcast, I'd argue this is the worst data breach of 2023.
{: .box-news }

<hr>
### Targeted F5 Vulnerability 'Update' Delivers Wiper to Israeli Victims

#### Sources:
- [Dark Reading](https://www.darkreading.com/cyberattacks-data-breaches/targeted-f5-vulnerability-update-delivers-wiper-israeli-victims)
- [We Live Security](https://www.welivesecurity.com/2022/12/07/fantasy-new-agrius-wiper-supply-chain-attack/)
- [The Hacker News](https://thehackernews.com/2023/10/pro-hamas-hacktivists-targeting-israeli.html)

Israel's National Cyber Directorate (NCD) has issued an urgent warning regarding a targeted email campaign. This campaign, impersonating F5 Networks, is distributing a dangerous wiper malware. The deception involves emails sent from "cert @ f5.support" containing a file named "update.zip," which, when executed, deletes the contents of any F5 servers it is run on.

The situation is part of a broader pattern of cyberattacks targeting Israeli entities. For instance, the Fantasy wiper, deployed through a supply-chain attack, impacted victims in South Africa, Israel, and Hong Kong within a 2.5-hour timeframe. Additionally, a pro-Hamas hacktivist group has been observed using a new Linux-based wiper malware, dubbed BiBi-Linux Wiper, specifically targeting Israeli entities amid the ongoing Israeli-Hamas conflict. This malware, described as an x64 ELF executable without obfuscation or protective measures, can potentially destroy entire targeted folders.

Furthermore, the Iranian-linked Agonizing Serpens APT group has been involved in a recent destructive wiper attack as part of a broader offensive targeting Israeli organizations, particularly those in the education and technology sectors.

>**Observations:**<br>
> Given how important F5 is, and the size of its userbase, supply chain attacks like this are crushing. Wiper malware is a pain to deal with, and can be hard to recover from if there are issues with backups and recovery planning.
{: .box-news }
<hr>
### Play Ransomware CISA Advisory

#### Source: [CISA](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-352a)

A recent CISA advisory on Play Ransomware outlines the TTPs and IOCs used by the Play ransomware group.

Since June 2022, Play Ransomware, also known as Playcrypt, has targeted a wide range of businesses and critical infrastructure in North America, South America, and Europe. As of October 2023, approximately 300 entities have been reportedly exploited by this group, with incidents in Australia noted since April 2023. Play ransomware operates with a closed group model and employs the use of a double-extortion model, demanding ransom payments in cryptocurrency. If victims refuse to pay, the group threatens to publish the exfiltrated data on their leak site. The ransom notes provided to victims do not include initial demands or payment instructions; instead, victims are instructed to contact the threat actors via email.

The advisory includes several recommendations for mitigating the impact of ransomware incidents, including the importance of patching known vulnerabilities, especially in internet-facing systems. Other recommendations include implementing multifactor authentication, maintaining offline backups, and having a recovery plan, network segmentation to prevent the spread of ransomware and restrict adversary lateral movement, monitoring network traffic and implementing real-time detection. Organizations are also advised to audit user accounts with administrative privileges and configure access controls according to the principle of least privilege.

Initial access by the Play ransomware group is achieved through exploiting valid accounts and public-facing applications, including known vulnerabilities in FortiOS and Microsoft Exchange. They have also been observed using external-facing services like Remote Desktop Protocol (RDP) and Virtual Private Networks (VPN) for initial access.
>**Observations:**<br>
> A solid overview of data, tips, and IOC resources for an active ransomware group.
{: .box-news }

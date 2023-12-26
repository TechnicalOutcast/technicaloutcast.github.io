---
layout: default
title: MongoDB Investigating Security Incident
image: /images/news_recaps.jpg
categories: blog
tags: blog RSS OpenAI data-breach ransomware identity
date: 2023-12-17
permalink: /blog/:year/:month/:day/:title/
description: Today's news centers on the MongoDB incident and a ransomware attack at a law firm.
---

Todays' news items are a mix of trust and identity, as well as a nifty tool for researchers. Clearly the main item is the MongoDB incident, but all of the items seem to fall under a common theme. Looks like we'll be ending the year on a bit of a down note in the defensive security sector.

<hr>
### Otis data breach cries out for basic security fixes

#### Source: [The Boston Globe](https://www.bostonglobe.com/2023/12/17/opinion/jack-teixeira-discord-classified-leak-ukraine-war-otis-massachusetts-air-national-guard/)

The Otis Air National Guard Base security breach, involving Jack Teixeira, highlights a systemic failure in military security clearances and supervision. Teixeira, 21, gained access to sensitive information despite prior troubling reports in his past. He allegedly leaked hundreds of classified documents via Discord and other social channels, including assessments of the Ukraine war and information about U.S. allies. The breach exposed issues in the "need to know" principle, supervision lapses, and the inadequacy of background checks, including the neglect of applicants' online activities within the 102d Intelligence Wing. The Air Force disciplined 15 members over the incident, including unit commander Colonel Sean Riley (who was later relieved of command). An [IG report (PDF)](https://s3.documentcloud.org/documents/24223085/af_teixiera_leak_investigation.pdf) on the incident emphasizes the need for stricter enforcement of security protocols and improved vigilance in monitoring and reporting potential security breaches.

>**Observations:**<br>
>Access and availability are important within an enterprise, but even then you have to trust your people. The IG report outlines numerous areas were existing checks and controls were available, but were not adhered to. Most firms operating within the DIB need to implement tighter controls on services and identities, which in some cases provide automatic notifications when access is out-of-bounds or abnormal.
><br><br>
>In this case, given that if there were no intelligence missions scheduled for the evening, the three person crew like the one A1C Teixeira was on, had a primary role was to ensure the HVAC system was operating properly and answer the phones. There were no controls in place to monitor print jobs, and no business rules for print products. This essentially granted crews unlimited access to JWICS sites and high-volume print jobs with no oversight.
{: .box-news }

<hr>
### MongoDB Investigating Security Incident

#### Source:  [MongoDB](https://www.mongodb.com/alerts)

MongoDB is investigating a security breach involving unauthorized access to their corporate systems. The incident, detected on December 13th, 2023, led to the exposure of customer account metadata and contact information. While there's no evidence that data stored in MongoDB Atlas was compromised, customers are advised to stay alert for social engineering and phishing attempts. Recommendations include activating phishing-resistant multi-factor authentication (MFA) and regularly changing MongoDB Atlas passwords. MongoDB will provide updates on the incident as the investigation progresses.

>**Observations:**<br> The key warning, given that metadata and contact information was accessed, centers on social engineering and phishing attacks. The data exposed is exactly the kind of data needed by a threat actor to develop an attack campaign, and locate possible subjects or targets. Base mitigations such as strong identity protections (people, apps, services) are certainly a fist line of defense, but other considerations such as deployment posture (access, availability, segmentation), and patch levels for services and applications should come into play as well. Phishing-resistant MFA is a bit open to interpretation, but should focus on passwordless auth methods rather than plain OTPs, especially those that are delivered via SMS.
{: .box-news }

<hr>
### Delta Dental of California Data Breach

#### Source: [BleepingComputer](https://www.bleepingcomputer.com/news/security/delta-dental-of-california-data-breach-exposed-info-of-7-million-people/)

Delta Dental of California experienced a massive data breach affecting nearly 7 million patients. The breach occurred through the MOVEit Transfer software, which was compromised due to a zero-day SQL injection flaw exploited by the Clop ransomware gang. This vulnerability allowed unauthorized access and data theft between May 27 and May 30, 2023. The exposed data includes names, financial account numbers, and credit/debit card details. Delta Dental has offered free credit monitoring and identity theft protection services to impacted patients and advises customers to be cautious of unsolicited communications. This incident ranks as the third-largest MOVEit data breach, following Maximus and Welltok. See Also: [Maine Attorney General notice](https://apps.web.maine.gov/online/aeviewer/ME/40/0f821b31-9e4f-4b15-872c-69fef62a93fa.shtml) and the [official notification letter from Delta Dental of California](https://www1.deltadentalins.com/content/dam/ddins/en/pdf/banners/notice-of-moveit-data-security-incident-en.pdf)

>**Observations:**<br> On a personal note, the timeline in this incident is all sorts of crazy. The incident was discovered on June 1, 2023, confirmed on July 6, 2023, and the threat actors were active from May 27-30, 2023. However, the investigation didn't complete until November 27, 2023. Patches were posted by MOVEit on May 31,2023, so this means that Delta Dental of California was one of the first organizations hit more than likely. Each organization is different, and there are regulatory and legal issues involved in some cases that delay investigations and notifications, but for the life of me, I can't understand why this incident took so long to confirm and complete.
><br><br>
>As for technical elements, keeping up with patches and implementing and deploying said patches is a full time job. It isn't easy, but clearly it is a critical operation for organizations of any size. The nightmare for many are the unknown problems that simply do not have a patch available, which is why incident response planning and strategies are so important. Detect quicker, and focus on increased visibility across the network. Lean on prevention as a core defensive element.
{: .box-news }

<hr>
### CMS becomes the latest law firm to fall victim to LockBit cyber-attack

#### Source: [Legal IT Insider](https://legaltechnology.com/2023/12/15/cms-becomes-the-latest-law-firm-to-fall-victim-to-lockbit-cyber-attack/)

CMS, an international law firm, has been targeted by a LockBit cyber-attack, specifically affecting CMS Spain. The ransomware organization claimed to have stolen 500GB of data, including "all confidential information in the USA," with a ransom payment deadline originally set for December 15, 2023. CMS Spain confirmed the attack impacted a small number of storage servers, but other CMS member firms were not affected. CMS has engaged external forensic specialists and its own cyber security response team to focus on isolation and control over incident, with a key focus on determining the extent of incident and what data has been affected. The incident was reported to the Spanish Data Protection Agency and the Public Prosecutor’s Office for Computer Crime.

>**Observations:**<br> In November, [CISA released an advisory](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-325a) focused on LockBit 3.0 and its exploitation of Citrix Bleed vulnerability (CVE-2023-4966), affecting Citrix NetScaler web application delivery control (ADC) and NetScaler Gateway appliances. LockBit 3.0 has targeted various critical infrastructure sectors, leveraging Citrix Bleed to bypass password requirements and multifactor authentication, enabling session hijacking and data access.
><br><br>
>Targeting legal firms makes sense from a threat actor's perspective, not only because they are a target of opportunity, but because the information held on those systems can lead to additional targets and potential ransom payouts. Obviously, platform and software patching is critical in cases like this, but when attacks happen at a rapid clip, it can be hard to keep on top of things - if not impossible - in those early days. The fallback then, given that patching alone is never enough, is for organizations to focus on increased visibility across their infrastructure, and harden identity and access controls, which can help limit some of the fallout of an active incident. It isn't perfect, but the little mitigations add up over time.
{: .box-news }

<hr>
### NetworkSherlock: Powerful and Flexible Port Scanning Tool with Shodan

#### Source: [KitPloit](https://www.kitploit.com/2023/12/networksherlock-powerful-and-flexible.html)

NetworkSherlock is a sophisticated port scanning tool tailored for network security professionals and penetration testers. NetworkSherlock can efficiently scan IP ranges, CIDR blocks, and multiple targets. It also comes with detailed banner grabbing capabilities across various protocols and integration with Shodan.

>**Observations:**<br> A handy tool for researchers and bounty hunters. This looked cool, so I wanted to share.
{: .box-news }

<hr>

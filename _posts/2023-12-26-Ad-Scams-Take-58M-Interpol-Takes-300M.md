---
layout: default
title: Ad Scams Take $58M&#59; Interpol seizes $300M
image: /images/news_recaps4.jpg
categories: blog
tags: blog RSS OpenAI data-breach government fraud
date: 2023-12-26
permalink: /blog/:year/:month/:day/:title/
description: A Mint Mobile data breach. Criminals use malicious ads to drain wallets, and Interpol conducts successful raids.
---

Now that Christmas is behind me (I got my nails painted by my granddaughter, and my kids had a Nerf war), I wanted to relax with some reading.

Mint Mobile has disclosed a data breach, and I am floored by the Interpol raid results. Also of interest is the research that led to having fake VPNs pulled from Google Play. Finally, crypto-focused malware drained millions from their victim's wallets.

<hr>
### $300 Million Seized and 3,500 Arrested During Interpol Operation

#### Sources:
1. [Databreaches.net](https://www.databreaches.net/usd-300-million-seized-and-3500-suspects-arrested-in-international-financial-crime-operation/)
2. [The Hacker News](https://thehackernews.com/2023/12/3500-arrested-in-global-operation-haechi.html)
3. [The Register](https://www.theregister.com/2023/12/20/interpol_op_cuffs_3500_cyber/)
4. [Gizmodo](https://gizmodo.com/interpol-arrests-3500-suspects-in-sweeping-cybercrime-1850315280)

Operation HAECHI IV, a six-month-long international police operation led by INTERPOL, has successfully resulted in the arrests of nearly 3,500 individuals and the seizure of assets worth $300 million. This operation, which spanned from July to December 2023, involved 34 countries and focused on combating a range of cyber-enabled financial crimes.

The types of scams targeted by this operation included voice phishing, romance scams, online sextortion, investment fraud, money laundering related to illegal online gambling, business email compromise fraud, and e-commerce fraud. The operation was designed to disrupt and dismantle the networks behind these scams and to seize the proceeds of their criminal activities.

Investigators used INTERPOL’s Global Rapid Intervention of Payments (I-GRIP) system, a stop-payment mechanism, to detect online fraud and freeze associated bank and virtual asset service provider (VASP) accounts. This collaborative approach was crucial in blocking criminal proceeds and bringing the perpetrators to justice.

One notable success of the operation was the arrest in Manila of a high-profile online gambling criminal after a two-year manhunt by Korea’s National Police Agency. In total, the operation led to the blocking of 82,112 suspicious bank accounts, with the seized assets including $199 million in hard currency and $101 million in virtual assets.

Stephen Kavanagh, INTERPOL’s Executive Director of Police Services, highlighted the significance of the operation. He pointed out that the seizure of $300 million represents a serious threat to global security and undermines the economic stability of nations. He emphasized that such a vast accumulation of unlawful wealth is derived from the savings and hard-earned cash of victims.

Additionally, the operation blocked over 80,000 suspicious bank accounts and alerted government officials to new types of scams using AI and fake NFTs.

>**Observations:**<br>
> Damn! This is a massive win for law enforcement.
{: .box-news }

<hr>
### The Cashback Extension Killer

#### Source: [ReasonLabs](https://reasonlabs.com/research/the-cashback-extension-killer)

ReasonLabs researchers have uncovered a widespread malware campaign involving malicious web extensions disguised as VPNs, distributed through torrent files, mimicking popular video games like Grand Theft Auto and Assassins Creed. These extensions, including 'netPlus' with over 1 million users and others with nearly 500K combined installations, were forcibly installed on users' browsers through sophisticated means, bypassing traditional installation approvals.

The extensions, primarily targeting Russian-speaking users, were not only fake VPNs but also executed a cashback activity hack, deactivating other cashback extensions in the infected browsers. Their operation involved over 20,000 lines of complex JavaScript code, and they presented a real VPN interface with limited functionalities to maintain the illusion. These extensions communicated with certain domains, suggesting a focus on Russian-speaking countries.

>**Observations:**<br>
> Google has pulled the fake VPNs, but this is just another example of targeted malicious apps, which on the surface look harmless and often pass random code checks from static scanners.
{: .box-news }

<hr>
### Mint Mobile Discloses New Data Breach Exposing Customer Data

#### Source: [BleepingComputer](https://www.bleepingcomputer.com/news/security/mint-mobile-discloses-new-data-breach-exposing-customer-data/)

Mint Mobile recently disclosed a data breach that compromised customer personal information, which could potentially be used for SIM swap attacks. Mint Mobile, a mobile virtual network operator owned by T-Mobile, provides budget, pre-paid mobile plans. The breach exposed customers' names, phone numbers, email addresses, SIM serial numbers, IMEI numbers, and service plan details. However, credit card numbers and passwords were not compromised due to not being stored by Mint and the use of strong cryptographic technology for password protection.

>**Observations:**<br>
> SIM swapping is still a big deal on networks that rely on such technologies. The identity element here is the exposure of a compromised device, which can lead to all sorts of problems. SMS-based authentication needs to be eliminated long-term.
{: .box-news }

<hr>
### From Google to X Ads: Tracing the Crypto Wallet Drainer's $58 Million Trail

#### Source: [Scam Sniffer](https://drops.scamsniffer.io/post/from-google-to-x-ads-tracing-the-crypto-wallet-drainers-58-million-trail/)

A recent investigation by Scam Sniffer reveals a complex web of phishing scams involving 'wallet drainers,' which have caused significant financial damage. These scams have utilized various methods, including phishing ads, supply chain attacks, and social media phishing, to exploit users and steal assets. Wallet drainer attacks are exactly what they sound like, an attack against crypto wallets, and the users holding them. A particular wallet drainer, first identified in phishing campaigns using Google Search ads, was later found in phishing attempts on X (Twitter). In total, approximately 10,072 phishing websites were linked to this wallet drainer, which amassed nearly USD $58.98 million from about 63,210 victims over the past nine months.

These malicious ads were found to employ methods to bypass ad audits, often targeting specific regions, making the detection process challenging. Additionally, redirect deception techniques were used to make ads appear credible, often misrepresenting them as official domains. Over nine months, phishing sites related to this wallet drainer were monitored, with notable peaks in activity in May, June, and November.
>**Observations:**<br>
> Advertising is one of the tools of the trade for scammers and dedicated criminals, as they can target pools of victims for in a common market, area, or vertical for little to no cost. Moreover, some advert campaigns automatically include social elements, which will only increase their reach.
><br><br>
>Anyone with a crypto holding, no matter what it is, should be really careful in safeguarding access, and use all available account protections from the crypto service (MFA apps), and treat the passwords used for these  accounts like a state secret. At no point should crypto passwords be the same as any other account held, nor should they be remotely related. Password managers will also help, as they can generate long, random password strings, and will only auto-fill on the legitimate website, which would defeat most crypto phishing attempts.
{: .box-news }

---
layout: default
title: RSS Recap January 2024 Volume 3
image: /images/news_recaps7.jpg
categories: news
tags: news RSS OpenAI government education healthcare data-breach vulnerabilities
date: 2024-01-24
permalink: /blog/:year/:month/:day/:title/
description: This is the third edition of my news recap series.
---

Today it's volume 3. I figured I'd share what I've found interesting while scanning my RSS feeds in a quick recap. This is a continuation of the RSS Archives series.

<hr>

**Title:** Data Breach at Carnegie Mellon University

**Source:** [California Attorney General](https://oag.ca.gov/system/files/EXPERIAN_K6458_Carnegie%20Mellon%20University_L02_SAS_2_Redacted.pdf), [TribLIVE](https://triblive.com/business/technology/carnegie-mellon-university-hit-by-cyberattack-informs-7300-people-possibly-affected/), [Yahoo News](https://news.yahoo.com/carnegie-mellon-university-hit-cyberattack-231114996.html)

Carnegie Mellon University (CMU) recently disclosed a data breach impacting approximately 7,300 individuals. Detected on August 25, 2023, the breach involved unauthorized access to a CMU computer system, possibly resulting in the copying of files containing personal data from students, employees, applicants, and contractors; such as names, social security numbers, and dates of birth.

The incident was confirmed completed on December 4, 2023, after an extensive investigation and review process involving law enforcement. CMU has taken steps to prevent future incidents and is offering affected individuals 24 months of credit monitoring and identity theft protection.
<hr>

**Title:** Court Fines Developer After Security Disclosure

**Source:** [Bleeping Computer](https://www.bleepingcomputer.com/news/security/court-charges-dev-with-hacking-after-cybersecurity-issue-disclosure/)

A German court has fined a programmer €3,000 ($3,265) for hacking, following their investigation into an IT problem. The programmer, working as a freelance IT service provider, discovered and disclosed a significant data privacy issue in merchandise management software.

The issue involved a MySQL connection to a server owned by Modern Solution GmbH, a management software vendor, containing sensitive data of nearly 700,000 customers. Despite the programmer's efforts to responsibly report the vulnerability, they were charged under Germany's 'Hacker Paragraph' in the Criminal Code. The programmer plans to appeal the decision.

Granted, the blogger and the programmer went public before Modern Solution GmbH could respond, but the fact that the company sought to prosecute the person disclosing a security issue is my problem. This is why researchers hesitate, and it is just crazy that we still have laws on the books that allow companies to do this.
{: .box-news }
<hr>

**Title:** Law Firm That Handles Data Breaches Hit by Data Breach

**Source:** [TechCrunch](https://techcrunch.com/2024/01/04/orrick-law-firm-data-breach/), [SecurityWeek](https://www.securityweek.com/law-firm-orrick-reveals-extensive-data-breach-over-half-a-million-affected)

Orrick, Herrington & Sutcliffe, a San Francisco-based international law firm known for handling data breaches and security incidents, experienced a cyberattack themselves in March 2023.

The breach resulted in the theft of sensitive health information and personal data of more than 637,000 individuals, and exposed various types of personal information, including consumer names, dates of birth, addresses, government-issued identification numbers, medical treatment and diagnosis information, insurance claims, and financial details.

Among the affected were clients of Orrick, including EyeMed Vision Care, Delta Dental of California, MultiPlan, Beacon Health Options (now Carelon), and the U.S. Small Business Administration. Orrick deployed additional security measures and tools to enhance its network's security following the incident. In December 2023, Orrick reached a tentative settlement in four class action lawsuits related to the data breach.
<hr>

**Title:** Hair Club for Men Suffers Data Breach

**Sources:** [Maine Attorney General](https://apps.web.maine.gov/online/aeviewer/ME/40/d570ad19-5ac8-4b21-8b2c-1330a5e7c386.shtml)

Hair Club for Men, Ltd., Inc., experienced a data breach on October 18, 2023, which was disclosed on January 12, 2024. Hair Club for Men, famous for its specialized focus on hair loss treatments and solutions, offers an extensive array of services tailored to both men and women.

The breach involved unauthorized access to personal identifiable information and sensitive health information of over 4,000 current and former employees. Compromised data includes names, Social Security numbers, driver’s license information, direct deposit account information, and medical information related to work injuries. The company is offering one year of free credit monitoring and identity theft protection services to affected individuals.
<hr>

**Title:** Burnout: Inferno Drainer’s Multimillion-Dollar Scam Scheme Detailed

**Source:** [Group-IB Blog](https://www.group-ib.com/blog/inferno-drainer/)

Inferno Drainer, a prominent multichain crypto drainer, operated from November 2022 to November 2023 under a scam-as-a-service model. The scheme involved sophisticated phishing websites tricking victims into connecting their cryptocurrency wallets to the attacker's infrastructure, resulting in significant financial loss.

Group-IB identified over 16,000 domains linked to Inferno Drainer’s phishing operations, with more than 100 crypto brands impersonated. The drainer contained scripts that spoofed popular Web3 protocols, facilitating unauthorized transactions. Despite its shutdown, the impact of Inferno Drainer highlights the ongoing risks in the crypto world, with the potential for similar scams to emerge.
<hr>

**Title:** Ransomware Actors Abusing TeamViewer for Initial Access

**Sources:** [Bleeping Computer](https://www.bleepingcomputer.com/news/security/teamviewer-abused-to-breach-networks-in-new-ransomware-attacks/), [Huntress](https://www.huntress.com/blog/ransomware-deployment-attempts-via-teamviewer)

Ransomware actors are increasingly exploiting TeamViewer, a widely-used remote access tool, to gain initial access to organizational networks and deploy encryptors, notably those derived from the leaked LockBit ransomware builder. This method of attack echoes a similar incidents from back in 2016, where TeamViewer was leveraged in other ransomware attacks. The primary vulnerability exploited by attackers is not a software flaw but compromised user credentials, but credential stuffing.

Recent reports from Huntress reveal that criminals continue to use this tactic, successfully infiltrating devices through TeamViewer to initiate ransomware attacks. Log file analyses indicate a common attacker in multiple incidents. The attackers targeted endpoints with varying levels of usage and monitoring, deploying ransomware through a DOS batch file named PP.bat.

TeamViewer has responded to these security incidents, emphasizing the importance of robust security practices like using complex passwords, two-factor authentication, and regular software updates. They have also [released best practices for secure unattended access](https://community.teamviewer.com/English/kb/articles/108681-best-practices-for-secure-unattended-access) to aid users in boosting their security measures.
<hr>

**Title:** VF Corp's Data Breach Impacts 35.5 Million

**Sources:** [Reuters](https://www.reuters.com/business/retail-consumer/vf-corps-cyber-incident-causes-data-breach-355-million-consumers-2024-01-18/), [SecurityWeek](https://www.securityweek.com/vf-corp-says-data-breach-resulting-from-ransomware-attack-impacts-35-million/), [TechCrunch](https://techcrunch.com/2024/01/18/vf-corporation-vans-supreme-owner-data-breach-millions/)

VF Corporation, the parent company of well-known apparel brands such as Vans, Supreme, and The North Face, disclosed a massive data breach as a result of a cyberattack in December. This incident led to the theft of personal data of approximately 35.5 million customers. The Denver, Colorado-based company reported the breach to regulators, stating that the attackers disrupted operations by encrypting some IT systems, implying a ransomware attack. The ALPHV (BlackCat) ransomware group later claimed responsibility for the breach.

VF Corp. acknowledged the disruption to its operations, including impacts on its ability to fulfill orders. The company has since made substantial progress in restoring the impacted IT systems and data, but continues to deal with minor operational impacts.

---
layout: default
title: The LastPass Data Breach Overview
image: /images/lastpass_app.jpg
categories: news
tags: news passwords data-breach lastpass
date: 2023-01-14
permalink: /news/:year/:month/:day/:title/
description: Since I blogged about moving my parents away from LastPass, I wanted to create a sort of an index related to the data breach, and a timeline explaining everything you need to know about it.
---
Since I [blogged about moving my parents away from LastPass][1], I wanted to create a sort of an index related to the data breach, and a timeline explaining everything you need to know about it.

### August 2022 - Initial Breach Notification

[LastPass informs the public][3] that a developer account was compromised and the threat actors responsible leveraged this access to steal source code and other proprietary LastPass technical information.

### September 2022 - Update #1

LastPass updates their public notice regarding the August incident. In addition to confirming the timing of the incident to four days in August 2022, LastPass includes the following details in their update:

>Our investigation determined that the threat actor gained access to the Development environment using a developer’s compromised endpoint. While the method used for the initial endpoint compromise is inconclusive, the threat actor utilized their persistent access to impersonate the developer once the developer had successfully authenticated using multi-factor authentication.

While not confirmed, it is possible the threat actor used an MFA fatigue attack[^1], or tricked the developer into sharing their MFA code, enabling  the threat actor to log-in.

The update also included this line, which is what has come  back to haunt LastPass:

>Although the threat actor was able to access the Development environment, our system design and controls prevented the threat actor from accessing any customer data or encrypted password vaults.

### November 2022 - Update #2

LastPass updates their public notice again, this time disclosing that the threat actors responsible for the August incident also targeted GoTo (the company behind LogMeIn and GoToMyPC), and accessed customer information.

>We recently detected unusual activity within a third-party cloud storage service, which is currently shared by both LastPass and its affiliate, GoTo. We immediately launched an investigation, engaged Mandiant, a leading security firm, and alerted law enforcement.
><br><br>
>We have determined that an unauthorized party, using information obtained in the August 2022 incident, was able to gain access to certain elements of our customers’ information.

At this point, it is known that the LastPass attackers had compromised an employee, and used that compromised account to access source code, and other customer information. The third-party cloud storage provider is [Amazon's AWS][2]. For those in the security community, the case  here is lateral movement, and many were speculating that the customer password vaults were compromised too. But LastPass had already stated that wasn't the case. Turns out, it was.

### December 2022 - Vaults Confirmed Compromised

In yet another update to their public notice, LastPass finally confirmed the worst fears for many in the security space. In their December update, LassPass confirmed that multiple employees were targeted, and threat actors did indeed access customer password vaults.

>To date, we have determined that once the cloud storage access key and dual storage container decryption keys were obtained, the threat actor copied information from backup that contained basic customer account information and related metadata including company names, end-user names, billing addresses, email addresses, telephone numbers, and the IP addresses from which customers were accessing the LastPass service.
><br><br>
>The threat actor was also able to copy a backup of customer vault data from the encrypted storage container which is stored in a proprietary binary format that contains both unencrypted data, such as website URLs, as well as fully-encrypted sensitive fields such as website usernames and passwords, secure notes, and form-filled data.

There were a number of things in the December statement that stood out. An article by [Zack Whittaker][5] at TechCrunch [offered breakdown of the announcement][4], and explained both what was said - and what wasn't said - by LastPass. [Wladimir Palant also published an overview][6] of the December update, and said the statement was "full of omissions, half-truths and outright lies."

Palant wrote:

>LastPass is trying to present the August 2022 incident and the data leak now as two separate events. But using information gained in the initial access in order to access more assets is actually a typical technique used by threat actors. It is called lateral movement.
><br><br>
>So the more correct interpretation of events is: we do not have a new breach now, LastPass rather failed to contain the August 2022 breach. And because of that failure people’s data is now gone.
><br><br>
>Note how LastPass admits not encrypting website URLs but doesn’t group it under “sensitive fields.” But website URLs are very much sensitive data. Threat actors would love to know what you have access to. Then they could produce well-targeted phishing emails just for the people who are worth their effort.

As to LastPass' statement that it would be "extremely difficult to attempt to brute force guess master passwords for those customers who follow our password best practices" Palant suggested the company was preparing the ground to blame customers if their accounts got hacked.

>This prepares the ground for blaming the customers. LastPass should be aware that passwords will be decrypted for at least some of their customers. And they have a convenient explanation already: these customers clearly didn’t follow their best practices.

Palant also [blogged about the iterations used by LastPass][7], which explains why they matter, and what's wrong with them. Including the fact that password cracking is a very real possibility.

Pointing out that a dedicated attacker could make 10 billion guesses for less than $100 USD, LastPass competitor, 1Password, [said in their blog][8] that "unless your password was created by a good password generator, it is crackable."

>The LastPass account password “best practices” advice linked to in their announcement says nothing about using a password generator, so it would be incorrect to assume that users are generating their LastPass passwords using a strong password generator.

Palant summed up the situation rather well, change your passwords.

>If you are someone who might be targeted by state-level actors: danger is imminent, and you should change all your passwords ASAP. If you are a regular “nobody”: access to your accounts is probably not worth the effort. Should you hold the keys to your company’s assets however (network infrastructure, HR systems, hot legal information), it should be a good idea to replace these keys now.

### Additional Reading

Brian X. Chen at The New York Times has a good piece on the incident titled: [A Breach at LastPass Has Password Lessons for Us All][9]

LastPass is facing a class action lawsuit, filed in the US District Court of Massachusetts, [filed by a man who lost $53,000 in Bitcoin][10]. This individual's LastPass account followed all of the company's recommended best practices, but that didn't stop criminals from wiping out his assets.

To put it plainly, the claim made by the lawyers representing the man states that "LastPass 'Best Practices' Were Woefully Insufficient to Protect its Users’  Private Information from Compromise and Misuse" Remember, LastPass claimed it would be extremely difficult to brute force master passwords if customers followed best practices.

The legal team preparing the lawsuit address this, even going so far as to cite Wladimir Palant.

>[LastPass] never provided direct notice to Plaintiff or Class members of  any such “best practices,” nor did it ever attempt to enforce these practices; not to mention,  Defendant’s “stronger-than-typical” implementation of 100,100 iterations of the PBKDF2  algorithm is actually well below the standard 310,000 iterations recommendation by the Open  Web Application Security Project (“OWASP”).6

Lily Hay Newman at Wired published ["Yes, It’s Time to Ditch LastPass"][11] noting in the subhead that the LastPass incident was so concerning " users need to take immediate steps to protect themselves."

______

[1]: https://technicaloutcast.com/blog/2022/12/30/moving-my-parents-away-from-lastpass/
[2]: https://archive.ph/wip/FOKDb
[3]: https://blog.lastpass.com/2022/12/notice-of-recent-security-incident/
[4]: https://techcrunch.com/2022/12/14/parsing-lastpass-august-data-breach-notice/
[5]: https://twitter.com/zackwhittaker
[6]: https://palant.info/2022/12/26/whats-in-a-pr-statement-lastpass-breach-explained/
[7]: https://palant.info/2022/12/28/lastpass-breach-the-significance-of-these-password-iterations/
[8]: https://blog.1password.com/not-in-a-million-years/
[9]: https://www.nytimes.com/2023/01/05/technology/personaltech/lastpass-breach-password-safety.html
[10]: https://storage.courtlistener.com/recap/gov.uscourts.mad.252095/gov.uscourts.mad.252095.1.0_2.pdf
[11]: https://www.wired.com/story/lastpass-breach-vaults-password-managers/

[^1]: An MFA fatigue attack is where a criminal will trigger MFA push notifications over and over again until the victim gets sick of seeing them, presuming the notification flood is a technical glitch, and just accepts the request.

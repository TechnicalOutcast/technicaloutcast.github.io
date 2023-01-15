---
layout: default
title: Inspector General&#58; 21&#37; of DOI Passwords Easily Compromised in Test
image: /images/login_screen.jpg
categories: news
tags: news passwords government
date: 2023-01-18
permalink: /news/:year/:month/:day/:title/
description:  An Office of Inspector General report says that 21% of the US Department of the Interior passwords were easily cracked during a recent test. The report found rampant password reuse, weak password schemes, and a lack of MFA.
---

An [Office of Inspector General (OIG) report says][1] that 21% of the US Department of the Interior (DOI) passwords were easily cracked during a recent test. The report found rampant password reuse, weak password schemes, and a lack of MFA.

### Password Problems at the DOI

The title of the report says it all:

>P@s$w0rds at the U.S. Department of the Interior: Easily Cracked Passwords, Lack of Multifactor Authentication, and Other Failures Put Critical DOI Systems at Risk

According to the report, the OIG spent about $15,000 USD to build the cracking rig used in the test.

The wordlists were comprised of [the RockYou2021 list][2], which is a collection of words and known passwords that have been previously compromised and released to the public. In addition to RockYou2021, the report also references wordlists made up of  dictionaries  from multiple languages, U.S. Government terminology, and pop culture references. The OIG also used cracked DOI passwords to generate new wordlists.

In all, the OIG was able to crack 21% of the DOI passwords, and 16% of those were cracked within the first  90 minutes of testing.

There were 14 agencies tested, including the Bureau of Indian Affairs (BIA); the Bureau of Land Management (BLM); the Bureau of Reclamation (BOR); the Bureau of Trust Funds Administration (BTFA); the Interior Business Center (IBC); the Minerals Management Service (MMS); the Bureau of Ocean Energy Management (BOEM); the Bureau of Safety and Environmental Enforcement (BSEE); the Office of Natural Resources Revenue (ONRR); the National Park Service (NPS); the Office of Inspector General (OIG); the Office of Surface Mining Reclamation and Enforcement (OSMRE); the U.S. Fish and Wildlife Service (FWS); and the U.S. Geological Survey (USGS).

The OIG report really centers on the need for MFA adoption, and urges DOI to speed up their efforts, citing the cracked passwords as a key risk.

>In particular, in the first 90 minutes of testing, our hash-cracking system obtained clear text passwords for 13,924 (16 percent) of 85,944 Department Active Directory (AD) user accounts. Overall, we cracked 18,174 (21 percent) of the Department’s AD user accounts. We also cracked 288 passwords for accounts with elevated privileges and 362 passwords belonging to senior Government employees (GS–15 or higher, including senior executives)—among them, passwords belonging to 3 high-level OCIO management accounts and a total of 54 senior executives Departmentwide.
><br><br>
>We also learned that the Department’s password complexity requirements implicitly allowed unrelated staff to use the same inherently weak passwords and that the Department did not timely disable inactive accounts or enforce password age limits. It is likely that if a well-resourced attacker were to capture Department AD password hashes, the attacker would have achieved a success rate similar to ours in cracking the hashes.

![Table 1 from the OIG report showing the number and type of passwords cracked.](https://technicaloutcast.com/images/post-images/OIG-Report/table1.jpg)

The summarized OIG findings are below:

The Department did not consistently implement multifactor authentication, including for 89 percent of its High Value Assets (assets that could have serious impacts to the Department’s ability to conduct business if compromised), which left these systems vulnerable to password compromising attacks.
{: .box-error }

The Department’s password complexity requirements were outdated and ineffective, allowing users to select easy-to-crack passwords (e.g., Changeme$12345, Polar_bear65, Nationalparks2014!). We found, for example, that 4.75 percent of all active user account passwords were based on the word “password.” In the first 90 minutes of testing, we cracked the passwords for 16 percent of the Department’s user accounts.
{: .box-error }

The Department’s password complexity requirements implicitly allowed unrelated staff to use the same inherently weak passwords—meaning there was not a rule in place to prevent this practice. For example, the most commonly reused password (Password-1234) was used on 478 unique active accounts. In fact, 5 of the 10 most reused passwords at the Department included a variation of “password” combined with “1234”; this combination currently meets the Department’s requirements even though it is not difficult to crack.
{: .box-error }

The Department did not timely disable inactive (unused) accounts or enforce password age limits, which left more than 6,000 additional active accounts vulnerable to attack.
{: .box-error }



-[30]-

[1]: https://www.doioig.gov/sites/default/files/2021-migration/Final%20Inspection%20Report_DOI%20Password_Public.pdf
[2]: https://github.com/ohmybahgosh/RockYou2021.txt

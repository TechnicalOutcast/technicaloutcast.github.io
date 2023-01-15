---
layout: default
title: A Review of the Top 200 Most Common Passwords
image: /images/login_screen.jpg
categories: news
tags: news blog passwords
date: 2023-01-17
permalink: /news/:year/:month/:day/:title/
description:  NordPass recently published their report focusing on the Top 200 most common passwords, broken down  by region and topic, and the results are about what you'd expect.
---
### Recycled, reused, easily guessed passwords
NordPass [recently published their report focusing on the Top 200 most common passwords][1], broken down  by region and topic, and the results are about what you'd expect.

Truth be told, I didn't know lists like this were still a thing. Years ago, back when I had an active byline, I'd get pitched on stuff like this. While there was a general interest, most IT and InfoSec readers just didn't care, as it was the same story year-to-year. It was good filler content though, something to get a few clicks on a slow day.

However, as time went on, these collections and the news surrounding them started to reveal patterns. It's always the same usual suspects in the top 10, with a few exceptions once in a while, and nearly every password in the list comes off as a collection of throwaway passwords that were harvested up by malware and general cracking lists.

So let's see what this year has to offer. Here is a breakdown of the top 20 most common passwords globally.

### Top 20 Most Common Passwords 2022

 | Rank   | Password   | Count      | Rank   | Password    | Count    |
 | ------ | ---------- | ---------- | ------ | ----------- | -------- |
 | **1**  | password   | 4,929,113  | **11** | 1234567     | 110,279  |
 | **2**  | 123456     | 1,523,537  | **12** | 1234        | 106,929  |
 | **3**  | 123456789  | 413,056    | **13** | 1234567890  | 105,189  |
 | **4**  | guest      | 376,417    | **14** | 000000      | 102,636  |
 | **5**  | qwerty     | 309,679    | **15** | 555555      | 98,353   |
 | **6**  | 12345678   | 284,946    | **16** | 666666      | 91,274   |
 | **7**  | 111111     | 229,047    | **17** | 123321      | 83,241   |
 | **8**  | 12345      | 188,602    | **18** | 654321      | 81,231   |
 | **9**  | col123456  | 140,505    | **19** | 7777777     | 74,233   |
 | **10** | 123123     | 127,762    | **20** | 123         | 60,795   |
{: .box-success }

### The pattern remains
What I see here are throwaway passwords and mobile passwords. Things that people used because they are quick and easy to type. Does that invalidate the list? Absolutely not. In fact, it proves a point that humans will want convenience over complexity. Last June, Digital Shadows published [research stating that some 24 billion][2] username and password combinations were available online. That's a 65% increase over the totals from 2020.

#### A word about the process
Criminals often get their password collections from phishing and infostealer installs. The harvested passwords are then placed into collections that are sold and traded, before being merged into sub-collections based on account, regional breakdowns, access type, etc. Over the years when I was doing research at Akamai, I would monitor and track the credential harvesting and account takeover trade, so the data presented by Digital Shadows isn't unbelievable at all. If anything, it might be conservative.

### It's a decent report, but it's lacking
NordPass says that the passwords in their list come from a primary collection that is 3TB in size, sourced from researchers working security incidents. That doesn't really explain the source of the passwords. It's a trivial personal gripe of mine when the context isn't fully explained.

I'm still not a fan of these lists. While the NordPass research covered the Top 200 globally, they also do a breakdown of the passwords by country, gender, and even type (fashion brands, cards, food, movies, swear words, video games, and artists). But there was plenty missing. How about a breakdown of passwords by length, complexity, and root-word?

An argument could be made for the educational element of such a list, but I think the education aspect is better served by showing wins and not failures. So instead of here are 200 bad passwords you are all using, I'd focus on password managers, and why they're superior.

Let me give an example using the RockYou password list and [analysis from Pipal][3].

This is a breakdown of the 10 most common base words in the RockYou list, meaning the words used to generate a password (e.g. july13). Following that is a  breakdown of the 10 most common password lengths in the RockYou list.

 | **Top 10 Base Words** | **Password Length**   |
 | --------------------- | -------------------   |
 | love = 9829 (0.07%)   | 8 = 2965991 (20.68%)  |
 | angel = 4845 (0.03%)  | 7 = 2506256 (17.47%)  |
 | june = 4347 (0.03%)   | 9 = 2190993 (15.27%)  |
 | baby = 4160 (0.03%)   | 10 = 2013686 (14.04%) |
 | july = 4103 (0.03%)   | 6 = 1947848 (13.58%)  |
 | alex = 3816 (0.03%)   | 11 = 865969 (6.04%)   |
 | pink = 3331 (0.02%)   | 12 = 555331 (3.87%)   |
 | april = 3227 (0.02%)  | 13 = 364169 (2.54%)   |
 | sexy = 3039 (0.02%)   | 5 = 259169 (1.81%)    |
 | chris = 3017 (0.02%)  | 14 = 248513 (1.73%)   |

If you notice, most of the passwords in the RockYou list are between 6-8 characters in length, which was rather common for the time. In fact, 15% of the RockYou list has 1-6 characters as a password, which is the smallest subset. The majority of passwords had 1-8 characters (53%), followed by passwords with more than eight characters (46%).

So what does the RockYou list tell us? The stats show that most people were using easily remembered passwords, and following the general advice at the time, which was 5-8 character passwords with letters and numbers. A small percentage, the clear minority, went above and beyond with their passwords. That advice is terrible now, and most password cracking programs would make short work of the RockYou list today.

### Password managers are essential
But the RockYou list does give us an example of why password managers are so important. Humans can't do complex, especially once you mix in special characters, upper and lowercase letters, and numbers. A human would likely stick to a pattern - (```ZxcZaq123!```) - or a easily remembered series of words with a repeatable pattern - (```!!Alph@Br@v0G@mm@D3lt@!!```) - that will only slow a password cracking rig for a few seconds before the passwords  are cracked.

This is why password managers are superior. They can create truly random, lengthy passwords that a human never has to remember. Just remember to make the master password a good one, perhaps a sentence would do the trick. Otherwise, you'll face [the same risks that LastPass users are facing][4].

[1]: https://nordpass.com/most-common-passwords-list/
[2]: https://www.digitalshadows.com/press-releases/24-billion-usernames-and-passwords-available-on-the-dark-web-an-increase-of-65-in-just-two-years/
[3]: https://digi.ninja/projects/pipal.php
[4]: https://technicaloutcast.com/news/2023/01/14/lastpass-data-breach-timeline-need-to-know/

-[30]-

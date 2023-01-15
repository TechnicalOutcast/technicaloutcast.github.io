---
layout: default
title: Norton LifeLock Password Manager Accounts Compromised
image: /images/LifeLock_Logo.jpg
categories: news
tags: news passwords data-breach credential-stuffing
date: 2023-01-16
permalink: /news/:year/:month/:day/:title/
description: Breach notification letters from Norton LifeLock warn that customers using their password manager services have been compromised. The situation is exactly what those affected by the LastPass data breach are worried about.
---
## Norton LifeLock Breach Notification

Breach notification letters from Norton LifeLock warn that customers using their password manager services have been compromised. However, unlike the LastPass data breach, this security incident is due to credential stuffing attacks.

In a letter dated January 9, 2023, Norton LifeLock says that accounts on ```login.norton.com``` were targeted by credential stuffing attacks, which began on December 1, 2022.

The [breach notification letter][1] reads in part:

>... we strongly believe that an unauthorized third party knows and has utilized your username and password for your account. This username and password combination may potentially also be known to other.
><br><br>
>In accessing your account with your username and password, the unauthorized third party may have viewed your first name, last name, phone number, and mailing address. Our records indicate that you utilize our Norton Password Manager feature and, we cannot rule out that the unauthorized third party also obtained details stored  there especially if your Password Manager key is identical or very similar to your Norton account password.

Norton LifeLock says they reset the passwords of those affected in order to prevent additional access attempts, and urged those impacted to change their password and leverage two-factor authentication in the future. In addition, the company is also offering credit monitoring services.

## Credential Stuffing

The Norton LifeLock incident is a classic case of credential stuffing, and a really common attack online. It's also a prime example of what many security experts are [expecting to happen with customers of LastPass][2].

#### How it Works
Starting with a list of usernames and passwords, the attacker runs the list and keeps track of the successes. From there, the successfully attacked accounts are either accessed, and the contents of the account logged and leveraged in further crimes, or the list could be traded or sold to other criminals.

#### Criminal Economics
There is a whole economy around credentials, and compromised access is a major source of income when the account in question is a high-value target.

Ransomware affiliates for example, will have hundreds, sometimes thousands of dollars for access to a victim,  and the more credentials there are, the more they are likely to pay for them.

On the lower scale of things, password lists used in credential stuffing are also used for password cracking. If a person was part of a data breach, and their password was ```Michael22```, a criminal isn't going to hesitate to attempt variations of that password and keep a running log of what works and what doesn't.

If they manage to get a whole profile on a given victim, including several compromised accounts, they can flip it for a decent profit, or additional access to other accounts and services.

## Password Managers Work

Password managers work, but the protection offered is only as strong as the master password needed to unlock the vault. If the password manager is protected by an easily guessable, or previously compromised password, then the protections offered by the application are rendered useless.

Password recycling, or password reuse as it is sometimes called, is the exact problem that password managers were built to eliminate. But they're not a silver bullet, and as the LifeLock incident demonstrates, all the encrypted data in the world isn't going to survive someone using ```iLovePuppies24!```.

## Password Advice

Use a password manager. That is really the only advice a reporter, technical writer, or security researcher can offer these days. Humans simply cannot create complex passwords. So any advice on that front might do more harm than good.

What you can do however, other than use the password manager, is create a strong master password to unlock the application itself.

Make the master password a strong one, not just with complexity, but with length too. But how can you do that? You just read that humans cannot create complex passwords.

Make your master password a sentence. A sentence with all the proper formatting and structure needed. Make it personal to you, and something that no one could guess, even if they know one or two elements in it.

#### A 10 word, 48 character example:

```
My '79 Malibu had an 8-Track player. I liked it.
```
{: .box-error }

Some people know about my first car, few know about the radio, next to none know that I really used it and liked it.

Obviously, since you're reading it here, I don't use this as a password for anything. But you see the structure right? The formatting? The fact that it has spaces, numbers, symbols, upper and lowercase letters?

My parents use sentences to unlock their password manager, and those sentences are inside jokes between the two of them.

The trick is to make it something you can remember, and something that no one would guess, even if they know you.

### Don't Want a Sentence?

If you don't want to use a sentence as your master password, then I suggest using a password that is long ([such as six Diceware words][3]) backed by a YubiKey. Visit [this link][4] to learn how to use a YubiKey to protect your password manager, and get instructions for many of the popular password management tools on the market.

No matter what, you should use a password manager. Maybe you should avoid LastPass though.

But seriously, use a password manager.

-[30]-

[1]: https://ago.vermont.gov/blog/2023/01/09/nortonlifelock-gen-digital-data-breach-notice-to-consumers/
[2]: https://technicaloutcast.com/news/2023/01/16/lastpass-data-breach-timeline-need-to-know/
[3]: https://diceware.dmuth.org/
[4]: https://www.yubico.com/works-with-yubikey/catalog/?usecase=25&sort=popular
[5]: https://technicaloutcast.com/news/2023/01/16/lastpass-data-breach-timeline-need-to-know/

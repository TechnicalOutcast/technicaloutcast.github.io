---
layout: default
title: Fraudulent Card Transactions - A Black Friday Story
categories: blog
permalink: /blog/:year/:month/:day/:title/
date: 2018-12-04
description: Dealing with card fraud is a frustrating and time consuming process. While you as the consumer are not liable for fraudulent charges, you do have to jump though some hoops to recover your funds. Most banks don’t hold you liable for anything related to debit card fraud. Check with your financial institution for more details.
image: /images/CARD_IMG_20181125_142544102.jpg
---

It’s Saturday, the day after Black Friday. I’m checking email to see if I’ve missed anything. It’s the normal collection of bulk email, mostly previews of Cyber Monday deals, but something unusual catches my attention. One of the emails was a charge notification from PayPal. At 2:14 PM EST, someone used by PayPal Business Debit Mastercard to make a purchase for $73.14.

The last time I used this particular card, it was an online purchase at DoorDash (food delivery). Yet, I know for certain the food wasn’t that expensive. So I log into PayPal and check to see if the transaction alert was legitimate. The emailed charge was the first thing visible, posted to my account as a pending transaction.

**Side Note:** I avoided clicking any of the links in the notification email thinking it was a clever forgery. So I went to PayPal directly by typing the web address myself. This is a good habit to have when it comes to investigating potential credit card fraud like this. Don’t. Trust. Emailed. Links.

Seeing the pending transaction caused my heart to sink. It isn’t the first time my credit cards have been compromised, but that doesn’t mean it gets any easier. To make matters worse, a second charge notification alert arrived ten minutes later for $201.45. It too was listed as pending on my PayPal account.

Both charges were for: `"EB *BROWARD COUNTY FAI,SAN FRANCISCO,CA"`

A quick Google search tells me that EB * is the marker for Eventbrite and the tickets are for the Broward County Fair, an event in Florida. However, the merchant account isn’t AUTHORIZE.NET, [it looks as if the card was processed though Eventbrite directly][1].

Obviously, I’m not in Florida. I checked, and sure enough [the Broward County Fair][2] is using Eventbrite for their ticket sales.

## Fraudulent PayPal Business Debit Mastercard Charges

Like it or not, I have to deal with this.

Step one was to report the PayPal Business Debit Mastercard as stolen and have it canceled. After that, I called PayPal directly and disputed the charges.

PayPal Email Regarding the Cases:

>We’ll email you on each of the cases within 10 days with more information and next steps, if required. Additionally, we are sending you a new debit card and will notify you by email when it has been mailed.

I’m not certain how the card was compromised.

[Magecart has been a growing concern for online merchants][3], and I have used this card recently at DoorDash (an unlikely, but possible Magecart target) and Kohl’s (a prime Magecart target). It’s also possible the card was compromised via skimmer.

While I try to avoid it, I do use my PayPal Business Debit Mastercard for purchases at the register. But rarely do I swipe it, usually I have to insert the card’s chip into the terminal and enter a PIN. For the curious, the security chips in all the new credit and debit cards (EMV chips) do little to stop fraud when it comes to skimmers and hijacking online transactions.

I could get into a whole post on these chips and the problematic push to get retailers to support them fully, but the key thing to know here is that you have two types of transactions: CP (Card Present, you’re in the checkout line at the register) and CNP (Card Not Present, you’re shopping online).

A traditional skimmer will focus on CP transactions, and criminals use malware and website compromises to target CNP transactions.

Skimmers copy your card data when you swipe your card at the point-of-sale (POS) terminal. If you have a chip in your card, but you swipe it, a skimmer can copy that data. I’m sure plenty of you reading this have heard ‘the chip reader isn’t working so just swipe it‘ at one point or another. It isn’t as common these days, but shortly after the EMV cards started to roll out, plenty of merchants conducted business without chip support.

Online, criminals (like those associated with Magecart) compromise the website in order to copy your card details as you enter them into the form or submit them during the checkout process. Once the criminals have your card details they can clone them for use. This is an oversimplification, but that’s the basics as far as card fraud goes. The end result of this type of crime – for me at least – is a person in Florida purchasing tickets to the county fair with my card.

Like I said, for each instance where I used my card at a POS recently, I didn’t swipe it. I had to insert it into the chip reader and use a PIN. However, there is a process called ‘shimming’ (like skimming) and this can compromise chip cards when they are inserted into the POS.

[Shims sit between the chip and the chip reader][4], and allow a criminal to read and record the data on the chip as it is being read by the POS. However, this isn’t a flawless method of attack, as it only works if the bank responsible for the card made a mistake when it comes to implementing checks against the dynamic CVV (iCVV) created by the chip, which is different form the three digit number on the back of the card.

[As one advisory put it:][5]

>The only way for this attack to be successful is if an issuer [i.e. bank responsible for the card] neglects to check the CVV when authorizing a transaction. One of the additional security components is the integrated circuit card verification value (iCVV), which differs from the main card verification value (CVV) held on the magnetic stripe.
>This protects against the copying of magnetic stripe data from the chip to create counterfeit magnetic stripe cards. But this latest scam (card shimming) suggests thieves may be targeting issuers where they believe the CVV will not be checked.

If the CVV checks are not done correctly, it’s possible for a criminal to copy the data and generate a cloned card. At the moment, my gut says my card was compromised during a CNP transaction, not at a POS. However, I have no proof to say one way or another. If Kohl’s or DoorDash issue a breach notification, I’ll know for sure. It’s also possible neither of them are the source, and my card was compromised long before it was actually used by a criminal.

## Payment Card Fraud is Stressful

After I reported the card stolen and disputed the charges, PayPal opened an investigation into the matter. But before PayPal can do anything, the charges have to clear and hit my checking account.

I’m fortunate. Even if nothing goes my way and I’m out $274.59, it isn’t going to result in me losing my home or having utilities shut off. But I’m in a good situation. What about everyone else?

The idea that I have to let these charges hit my bank account first is frustrating, and I can imagine for some PayPal customers, such a requirement would be devastating. Honestly, about 18 years ago such a situation would have crushed me, $300 was a quarter of what I earned in a month.

For their part, once the charges hit and the investigation on their end officially starts, PayPal will issue a provisional credit equal to the amount disputed and I can also file additional requests if the disputed purchases result in NSF (Insufficient Funds) charges at my bank.

This is helpful, but in the short term, I’m more concerned about those who simply can’t ignore almost $300 in losses. If there are NSF charges, it could take days before PayPal credits you for them, and those charges add up by the day at most banks, so by the time you’ve gotten one credit, you’ll need to file for two or three more. This is in addition to the wait required before the initial provisional credits are delivered. This is financial stress at its worst.

Now, don’t get me wrong, I’m thankful for PayPal’s assistance here, but the process needs some work in my opinion. A 48-hour wait to get the provisional funds from PayPal, followed by the delay to shift them to a checking account, is beyond frustrating.

## Eventbrite

When I first noticed the fraudulent charges, as mentioned, I immediately called PayPal to report the problem. However, I also wanted to reach out to Eventbrite. Only, I couldn’t.

There was no number listed on the charge; it showed up eventually, but not until after the purchase had posted and the funds cleared my bank. For the record, the number to dispute questionable Eventbrite charges is 801-413-7200.

As I said, I searched Eventbrite’s website, but I couldn’t locate a number or email address to report fraudulent purchases. If it’s on the website, I certainly couldn’t find it with any sort of ease. But I’m fortunate to have dozens of knowledgeable security experts following me on Twitter. I posted about my problems and asked for suggestions. Almost immediately, several people directed me to the security@eventbrite address. I had seen this address while searching for a fraud contact, but it was listed as the address for research and disclosure issues, not card fraud. Still, it was worth a shot.

I emailed the address at about 1:30 PM EST on 11/24, and at 11:00 PM the same day (9.5 hours later?!) someone responded. However, the response simply told me my message was received and those manning the security@eventbrite address “have alerted the appropriate teams internally to investigate.” Remember, all of this happened on a Saturday. I didn’t hear back from anyone via email until the following Tuesday at 5:41 PM EST. By then, the fraudulent card charges had posted and the funds cleared my bank.

Now, during the process of waiting to speak to someone from Eventbrite, one of their security team reached out to me on Twitter to follow-up. This was on Monday, and when I responded that I hadn’t yet heard form anyone after that initial email on Saturday, this individual promised to follow-up on my situation personally.

After three additional emails, one on Tuesday and two on Wednesday, Eventbrite determined the charges were fraudulent and promised a refund “within 5-7 banking days.” Within 48-hours the fraudulent charges were reversed and credited back to me. But, is that a typical case? If a company executive hadn’t looked into my situation (which I’m thankful for by the way), would I have had to wait the full week? I don’t know. I hope not, but I honestly don’t know.

## Mounting Frustration

So because I had a platform and contacts, and because I was able to report the fraud quickly, I got my money back quicker than expected. This is great news for me, but I wasn’t really impacted by the financial losses. Sure, losing nearly $300 sucked, but my bills were paid and there was food in the kitchen. My problem, my beef with this whole process, is the fact I’m one of the lucky ones.

What about everyone else? Why does this process have to be so difficult and take so long? We can transfer millions between banks in seconds, but it takes a day, or several days, to credit fraudulent purchases? Maybe it’s just my frustration speaking here. I know there are processes, checks, approvals, etc. which are required before refunds and fraudulent charges are finalized or reversed; it’s to protect the business as well as the consumer. I also know that “5-7 banking days” is a boilerplate timeline too. Sometimes refunds are quicker, sometime they’re not.

But maybe – just maybe – there is a way to improve on things.

Again, 18 years ago, having to wait 5-7 days – after losing this money to begin with – would have meant choosing between eating or putting gas in the car, or pay paying bills before they were disconnected. Not to mention the impact of stress-related sleeplessness, headaches, and fear a situation like this would have caused me back then.

## Aftermath

As things would have it, PayPal issued their provisional credit the same day the charges were reversed. As I mentioned earlier, while PayPal works their process for the fraudulent charge report, or case as they call it, they grant me funds equal to the amount of the disputed purchases. Since Eventbrite reversed the charges, PayPal will take those funds back. If, like me, the customer moved those temporary credits to their bank account, PayPal will pull the funds form that source. It won’t be an instant process for PayPal, they’ll give some warning before they do.

So I’m in the clear. While I need to wait for PayPal to reverse their provisional credit, the fraudulent purchases have been refunded and I’ve received my new PayPal Business Debit Mastercard. I’ll be a little more cautious when using it online going forward.

## Some Advice
Dealing with card fraud is a frustrating and a time consuming process. While you as the consumer are not liable for fraudulent charges, you do have to jump though some hoops to recover your funds. For many of us, these delays only compound an already stressful situation. But remember, a delay in reporting could mean delays in recovery and increased liability. So the moment you notice something’s off, call the bank or card issuer (in my case it was PayPal) and dispute the charges while reporting the card as stolen.

Some will argue that you shouldn’t used debit cards at all, and this is somewhat true. But not really. These days banks limit your liability to $0 when you report a lost or stolen card, or report a fraudulent transaction the moment you notice something wrong. The Fair Credit Billing Act (FCBA) and the Electronic Fund Transfer Act (EFTA) protect you, [but you have to report losses quickly][6]. Under the FCBA, you’re liable for $50 if you report a loss or theft within two business days after learning about it. More than two business days, but less than 60 days after your statement is sent, the FCBA says liability is $500.

Again, most banks don’t hold you liable for anything related to debit card fraud. Check with your financial institution for more details. For a quick reference, the banks below publish their debit card liability claims.

[PNC Bank][7] – Zero Liability Fraud Protection, but does not apply to ATM transactions, or PIN transactions not processed by Visa.

[Chase Bank][8] – Zero Liability Protection, but does not apply to use of an account by an authorized user without the approval of the primary cardmember.

[Fifth Third Bank][9] – Zero Liability, but requires the customer to assist in the investigation if they believe their debit card is lost or stolen.

[Huntington Bank][10] – Zero Liability, but requires the customer to assist in the investigation and report fraud promptly.

[Wells Fargo][11] – Zero Liability, but you have to report the unauthorized transaction within 60 days of the statement showing the fraud being delivered.

[Bank of America][12] – Zero Liability, but you have to report the fraud immediately.

[Citi][13] – Zero Liability, but incidents need to be reported immediately. Option not available on all cards.

After things have settled, keep an eye on statements and your credit report. If you notice anything questionable, make sure you report it immediately. For more information, checkout the [FTC’s guidance on dealing with identity theft][14].

[1]:https://www.eventbrite.com/support/articles/en_US/Q_A/what-is-this-charge-from-eventbrite?lg=en_US

[2]:https://www.eventbrite.com/e/broward-county-fair-tickets-50196772899

[3]:https://www.flashpoint-intel.com/blog/inside-magecart-exposes-operation-behind-webs-biggest-ecommerce-scourge/

[4]:http://coquitlam.bc.rcmp-grc.gc.ca/ViewPage.action?siteNodeId=2115&languageId=1&contentId=49796

[5]:https://www.ncr.com/company/blogs/financial/are-emv-cards-vulnerable-at-the-atm

[6]:https://www.consumer.ftc.gov/articles/0213-lost-or-stolen-credit-atm-and-debit-cards

[7]:https://www.pnc.com/en/personal-banking/banking/debit-and-prepaid-cards/pnc-bank-visa-debit-card.html

[8]:https://www.chase.com/digital/fraud-security

[9]:https://www.53.com/content/fifth-third/en/personal-banking/bank/debit-cards.html#s

[10]:https://www.huntington.com/Personal/checking/platinum-debit-card

[11]:https://www08.wellsfargomedia.com/assets/pdf/personal/debit-card/terms-and-conditions.pdf

[12]:https://www.bankofamerica.com/deposits/checking/debit-card/

[13]:https://www.cardbenefits.citi.com/Products/0-Liability-on-Unauthorized-Charges

[14]:https://www.consumer.ftc.gov/topics/identity-theft

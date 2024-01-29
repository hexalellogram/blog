---
layout: post
title:  "Adventures in Transaction Tracking and Budgeting"
date:   2024-01-28 19:38:0 -0800
---

The latest rabbit hole that I've gotten into is transaction tracking - as in, tracking your bank accounts and the balances that each has. It's useful for keeping an eye on checking accounts, credit cards, and whatnot. Ancillary to this is budgeting - setting out money for different categories for a defined period of time, usually a month. The thing is, I don't budget in the normal sense. Actually, I kind of don't budget at all - my primary philosophy is that money in should be greater than money out. If money out is greater, then find somewhere to cut back so that money out goes below money in. It's a bit of a privileged position to be in, but I find that all the logical games around "budgeting" to be a bit of a distraction from the real question - are you saving up for things, are you investing, are you making more than you're spending?

But Bryce, you just said you don't want to deal with the whole business of budgeting? How the heck did you fall down the rabbit hole of tracking every single transaction? And where is the inevitable giant Excel spreadsheet? Answers to all of these questions come in due time, but first it's important to note that I believe in a few key general philosophies around money:

1. Money in > money out. I already explained this one above.
2. Trust is overrated. Don't trust what the bank says. While banks are reliable systems as a whole, I believe it's important to have an independent ledger that tracks what you spend and where. The most common issue I've found is restaurants - they probably misread my infamously horrendous chicken scratch on the receipt, and adjusted my bill by a different amount than I expected. That's happened at least twice.
3. Automation is, also, overrated. While some just want their finances to get out of the way, I believe that being firmly involved in the minutae gives me a better perspective on what I'm actually spending my money on.
4. Optimization is important, but not everything. While I talk about transaction tracking and budgeting, my overall approach to finance also encompasses things like cash back/rewards on credit cards. At the same time, I don't believe in going to the furthest with these - there are people that get insane value out of their rewards points because they got a great deal on a business class flight from Los Angeles to Tokyo. As a short guy who fits perfectly fine into most economy airline seats, who most often flies Southwest Airlines not because it's comfortable, but because they have cheap flights into airports that I want to fly to, I would never pay cash for a business class seat, so paying points for one doesn't have much attraction to me. On the other hand, I still do care about cash back, so I do have a fair amount of credit cards to make the most of that, so having something that can accommodate multiple accounts easily is a must for me.

Now let's talk apps, and why I eventually settled on one called Lunch Money.

## The State of the World

Going into this, it's not like I was never tracking my transactions before. My parents drilled it into me that I should be tracking my spending in a checkbook, at least for the checks I wrote. And because I can never stick to something unless it involves an electronic gadget *somehow*, my inevitable solution was to use an app. Originally I used an app I found on the App Store, [Debit & Credit](https://debitandcredit.app/). It's, all things said and done, a very nice app. Native macOS and iOS apps, a solid and responsive UI - this app served me well for a few years, but as the years have gone by a few things have started to stick out.

![Screenshot of Debit & Credit app](/imgs/2024-01-28-transaction-tracking-budgeting/debit-and-credit.png)

Debit & Credit does things a bit differently than most transaction tracking apps. It explicitly disavows syncing with a bank, because according to the developer being hands on with your finances is superior from a privacy perspective. While I have no qualms with aggregators like Plaid, which most apps use to connect with banks and automatically import transactions, having to do everything manually is not a dealbreaker for me. So I can live with it.

Something else that Debit & Credit does differently is having description, payee, and long-form notes all be separate. To the uninitiated, these all sound similar, and others might have a different idea of what these mean. In my view, a description is something short that describes what the purchase was for - think "Lunch 2/8/2023". Payee is the merchant or person that I paid (or that paid me), e.g. "Chipotle". Finally, long-form notes would contain other information relevant to the transaction, perhaps the fact that I used a $10 gift card with this transaction, which explains why the transaction is less than my normal lunch at Chipotle would be. Make sense? This will be important later.

Notably, Debit & Credit has autocomplete for the description and payee fields, so frequently-used descriptions can be autofilled easily. While this sounds like a good thing (especially for payees), my descriptions tend to be unique to the date (think "Lunch 2/8/2023" vs. "Lunch"). The app started complaining that having too many unique descriptions could begin to degrade app performance, so that's when I started looking for alternatives.

## You Need A Budget

![Screenshot of YNAB](/imgs/2024-01-28-transaction-tracking-budgeting/ynab.png)

No, that's not a statement. That's a reference to the wildly popular app [You Need A Budget](https://www.ynab.com/), henceforth referred to as YNAB. My friend [Matei](https://matei.gard.us/) told me to try it out - he said it worked well for him. And bonus ducks - YNAB offers a yearlong free trial for students. So I tried it out. There were some things about YNAB that I liked, but a lot that I didn't. My primary gripe is (probably) unsurprising - YNAB places a high emphasis on budgeting, something that I don't do at all. So trying to use YNAB as a pure transaction tracking app was not a great experience - I was constantly interrupted and pestered to assign money to specific categories so that I had a valid budget.

The one thing that I liked about YNAB was that they used the same set of categories for income and expenses - in contrast to Debit & Credit which has distinct sets of categories for Income and Expenses. This made things like categorizing reimbursements from friends a lot easier - if they paid me back for a dinner, then I'd just categorize that in the same category as the original restaurant expense.

When my trial was up earlier this January, I decided not to renew. Why? Overall, YNAB did not offer enough over Debit & Credit to justify the increased yearly price ($100/year), compared to what I was paying for Debit & Credit. Yet I still wasn't fully satisfied with Debit & Credit either, because the more I think about it, the more features I want in an app like this. Features that Debit & Credit lacked. So I set out in search of a new app.

## Features, Features

Over the past few years, I've figured out what I want to see in an app like this:

* Transaction tagging - this would be useful to be able to categorize things in arbitrary ways that aren't necessarily supported by the app. One big example for me is tracking transactions made on of my rewards credit cards, the Chase Freedom Flex. This card offers boosted rewards on the first $1,500 of purchases made in specific categories each quarter, so I'd want to tag categories that earned bonus rewards so that I don't exceed the $1,500 cap. Debit & Credit only supported one tag per transaction - I want to be able to add multiple tags per transaction.
* Mobile and desktop apps - I want to be able to track things on the go, because I believe that immediate data entry is the best way to not fall behind. Apps that restrict themselves to desktop only are well-intentioned in that they give you the space to think and analyze about your financial picture effectively, and you can see more data at a glance, but making it difficult to enter information on mobile makes it more difficult to live with on a day to day basis.
* Being able to mark transactions as cleared and/or reconciled - this is important to keep banks accountable, to make sure that their records match with yours. While some apps support reconciliation on a statement-by-statement basis, I prefer to reconcile transactions as the banks clear them, as frequently as every day depending on how many transactions I have. Attending to this frequently means it's never that much of a chore.
* Support for recurring transactions - being able to see the history of things like my payments for Spotify Premium is nice, without having to use search.
* Speaking of which, a powerful search interface - after using Notion, I've come to appreciate how Notion approaches filtering and search, with an easy-to-use yet powerful set of filtering options using the various categories and columns.

In my journey, I've tried way too many financial apps at this point, and there are also a few cardinal sins that I consider a dealbreaker:

* Combining the payee and description - if your app only allows me to say that I spent $14.55 at Chipotle, but not note down *what that transaction was for*, that's just silly. Was it for lunch or dinner? I guess without this, we'll never know. It sounds like such a basic thing to be missing, but you'd be surprised at how many apps lack this. If nothing else, it was an easy way to eliminate an app without testing it further. [Copilot](https://copilot.money/) is one of the biggest violators here - it's extremely hyped in personal finance communities, and for good reason - it's got an extremely slick UI. But for it to be missing a feature as basic as this is, quite frankly, baffling to me. It must be a deliberate choice by the developers, one that I fundamentally disagree with, so it means I won't be using their app.
* Not allowing the user to edit data imported from the bank - many of the apps I tried were focused on allowing the user to connect their bank accounts, and transaction data would be automatically imported from the bank, so you can see all of your accounts in one place. A nice idea, but if you don't allow the user to edit the information from the bank, that's particularly problematic. This manifested itself most often in withdrawals from Venmo. I withdraw from Venmo every time someone sends me money on Venmo, because I don't like keeping money there - money received from friends is, to my knowledge, not FDIC insured. Moreover, this prevents situations like withdrawing large amounts of money from Venmo that cannot be itemized in a transaction tracker - who knows what that $500 was for? If it's just a generic Venmo withdrawal, that information doesn't help anyone.
* Forcing me to sync through Plaid or another aggregator - while I can tolerate this as an optional feature, making it required is annoying. Even worse is if they combine this bullet and the previous. I prefer to add things myself and because I typically do it immediately, I can typically beat Plaid sync in speed.
* Not being able to add transactions on mobile - I'm going to specifically call out [Pocketsmith](https://www.pocketsmith.com/) for this. Why? No one asked. That's particularly painful because adding transactions is the primary thing I do on mobile anyways.

## Excel is Depression/Notion to the Rescue (Or Not)

So, given all those weird requirements, why didn't I just make the mother of all Excel spreadsheets for my finances? Two reasons:

1. Editing an Excel spreadsheet on the go is like asking for pain. The Excel mobile app exists, but how good of a user experience it is is another question entirely.
2. Implementing multi-select tags in Excel would require VBA (Visual Basic for Applications), which isn't supported by Excel on iOS anyways.

I also thought about trying to put all this data into Notion. Notion is great for creating custom databases, which sounded like a great fit for this project. However, I also decided against Notion, because editing a Notion database on mobile was only marginally better than an Excel spreadsheet, at best. Moreover, getting good metrics out of Notion was difficult - it's not a spreadsheet, and for good reason. Charts and graphs would be extremely difficult to generate.

Now that we've got that discussion out of the way, let's talk about the app I eventually settled on - Lunch Money.

## Lunch Money

![Screenshot of Lunch Money](/imgs/2024-01-28-transaction-tracking-budgeting/lunch-money.png)

[Lunch Money](https://lunchmoney.app/) is a web app created by an independent solopreneur (Jen) that I stumbled upon while browsing through a list of apps similar to Intuit Mint on Reddit (Mint is another one entry in this category, but it's being shut down. Plus on an ethical level, I refuse to use Intuit products due to their sketchy history of lobbying to prevent the IRS from creating a taxpayer friendly tax filing system). There are a few things that set Lunch Money apart from the pack:

* Transaction tags - as I described above, tags are a super important part of my workflow.
* Linking transactions together for group payments - say I spent $36.77 at Chipotle for dinner for myself and a friend, and then they Venmoed me back $18.37 for their portion of the meal. Transaction grouping allows me to link those two transactions together, so when viewing all transactions, the app shows that I only spent $18.40 at Chipotle for my portion. Yet while viewing transactions by account, the transactions that make up the group are shown instead. This is super handy for when I front money for a whole group - restaurant bills, rent in my college apartment where I paid all the rent and everyone else paid me back, etc. This was the single most important feature that convinced me to try out Lunch Money - more on that below.
* A super powerful recurring transactions engine built on matching rules - sometimes transactions are not the same from month to month. For example, my electric bill varies based on usage. Lunch Money allows for this variance, and even allows me to manually match transactions to their recurring instance, so that the recurring transaction is counted as paid for the month no matter what.
* An open developer API! I haven't actually done anything with the API yet, but it's exciting to have the opportunity open, plus it opens the door for community integrations as well.
* The ability to bulk edit multiple transactions in one go, for example to apply the same tag to all of them.
* It was easy enough to ignore the budgeting section of the app.
* A "choose your own pricing" model - annual pricing starts at $40, and it goes up from there if you would like to support the developer more. The recommended sustainable pricing is $100, which matches what YNAB was charging.

That transaction grouping feature in particular was the single most important feature that convinced me to try out Lunch Money. When I went through the past 5 years of transactions, I found a disturbing number of transactions where I had forgotten to ask for money from people, or I had forgotten to pay someone for a refund. I thought my mental system was pretty good, and I guess considering the sheer transaction volume, it was solid, but it definitely wasn't as bulletproof as I thought it was. Being able to group transactions should make this whole process much more reliable.

However, Lunch Money isn't perfect (nor would I expect it to be given that it's developed and maintained by a solo entrepreneur):

* There are a few visual bugs that I've reported. For example, changing the date of a transaction causes the new date shown to be one day behind. This doesn't actually affect the data stored - a reload is enough to get things in order - but it's a weird visual glitch nonetheless.
* There is no first party mobile app. jen [justifies this](https://lunchmoney.app/features/web-first) by arguing that a mobile app would be a much greater development workload, plus it's better to see things on a desktop where there's more space. However, I feel that there's room for both, and besides, given that there's an API, that means that the community can step up to the plate! Examples include [Snack Change](https://apps.apple.com/us/app/snack-change/id1557614640) which is an official iOS companion app, but it doesn't support the full Lunch Money feature set and I find it a bit barebones.
    * The Lunch Money website is *somewhat responsive* on mobile, but it's not perfect - information density is a bit low, but it gets the job done at least for adding transactions. More complex operations like grouping transactions, setting up recurring transactions, etc. are a lot more difficult on mobile.
* There is no dedicated pending/cleared transaction state. Unlike Debit & Credit, where I could specifically mark a transaction as pending or cleared, Lunch Money doesn't seem to have an analog for this situation for manually-updated accounts. It supports pending transactions for accounts that sync with banks through Plaid, but transaction information (including amount) cannot be edited until the transaction is reported as no longer pending by the bank. And banks are *slow*. This is particularly problematic for restaurants where the initial authorization typically won't include the tip.
    * Building on this, there's also no way to see account balance split out by cleared and pending balance. Lunch Money only shows the pending balance (i.e. what the balance would be if all transactions were cleared). This makes reconciliation with the bank *much* harder, especially if the bank doesn't include pending transactions in the total, such as my Chase credit cards.
* Viewing transactions by account is possible through Lunch Money's powerful filters, but not necessarily the easiest thing to do, because it requires configuring that filter every time. By comparison, Debit & Credit allowed me to filter by transaction through its sidebar.
* Keyboard shortcut support is meager at best and nonexistent in most places. It's not a dealbreaker, but it does slow me down a bit when I can't press Enter to close a modal.
* The entire app is built around splitting hings up between different months: the transactions view, recurring transactions, etc. While it's possible to view transactions for all time, it's not the default. I find this month-to-month distinction largely arbitrary for all accounts that aren't my main checking account.

The good news is that Lunch Money has an open feedback tracker! I've upvoted solutions to several of these and hopefully these can be addressed soon.

## Conclusion

In the meantime I'll be continuing my free trial of Lunch Money (and probably subscribing afterwards), because Lunch Money solves a lot of problems that I've had with Debit & Credit. I may operate these two apps in parallel for a while (I ran Debit & Credit and YNAB in parallel for a whole year, and my current Debit & Credit subscription doesn't expire till November). We'll see how things fare then.

Thanks for coming along with me on this unhinged rollercoaster ride through the state of today's financial apps.

---
layout: article
title:  "Common Problems and their Fixes: Java Edition"
name: "java"
desc: "Common Problems and their Fixes in Minecraft: Java Edition"
---
# Common Problems and their Fixes: Java Edition
This article is a guide to common problems that users may encounter in Java Edition, and how to fix them. Remember, if you're not sure about an issue, it's better to admit that you don't know than to give bad advice and potentially make the problem worse. Some fixes include Absol factoids, which you can use if you're helping in Minecraft Community Support or any other Discord server that has Absol in it.

 ## Cannot log in on one device, launcher stuck in offline mode or getting "The Authentication Servers are down for Maintenance" or "Not Authenticated with minecraft.net when trying to join servers
This error is usually caused by piracy tools, such as MCLeaks, Alterning, EasyMC etc, which work by redirecting queries going to Mojang's authentication servers to ones run by them, tricking the launcher into thinking the game has been paid for. To fix it, the user must repair their hosts file by following the instructions located [here](_help/hosts-file) (Absol factoid: `fix/hosts`)

## Not Receiving Password Reset Emails
Send them https://help.minecraft.net/hc/en-us/articles/360046038092-Password-Reset-not-Working-. If nothing in it works they need to email Mojang Support at https://help.minecraft.net/hc/requests/new (Absol factoid: `!?f account/send-email`).

## Trying to recover account
Ask them to contact Mojang at https://help.minecraft.net/hc/requests/new. If you are helping in Minecraft Community Support you can direct them to the #account-support channel instead. (Absol factoids: `as` for explaining that community volunteers cannot provide account support and `account/send-email` for emailing Mojang)

## Game freezes on loading screen
Caused by malware called PremiereOpinion, run [Malwarebytes Adwcleaner](https://www.malwarebytes.com/adwcleaner/) (Absol Factoid: `av/adwcleaner`)



## Multiplayer and Realms buttons greyed out on 1.16.4+ or "Failed to log in:null" on older versions
This is caused if the user uses a Microsoft account to log in and is not considered an adult by the MS Account system. A parent or guardian will need to add the user to a [Microsoft Family](http://account.microsoft.com/family/addmember) and enable "You can join multiplayer games" under their profile in [Xbox Settings](https://account.xbox.com/settings). They will need to restart Minecraft for the changes to take effect (Absol Factoid: `account/microsoft/multiplayer`)


## Can only play demo
Make sure they are logging in with the **Microsoft Login** button if they bought after December 1st, 2020, and **Mojang Login** if they bought before. If they are logging in with Microsoft and bought after, ask for a screenshot of the launcher and https://minecraft.net/en-us/profile (contains no personal information if logging in with Microsoft) and compare the listed Xbox gamertags to make sure they match and make sure a Minecraft username is shown on the webpage as they have not bought the game otherwise. If they have not bought the game, establish if an email from Mojang containing a Transaction ID was received. If it was not, see https://help.minecraft.net/hc/en-us/articles/360042693692-Minecraft-Java-Edition-I-Was-Charged-but-Did-Not-Receive-the-Game- (Absol Factoid: `account/payment/pending`)

If all else fails, contact Mojang Support at https://help.minecraft.net/hc/requests/new  (Absol Factoid: `!?f account/send-email`)

## Exit Code 0
Establish whether the game is freezing on the loading screen, if so see above. [to be filled]

## Mojang Support wait time
It is unwise to give any estimates on wait time for Mojang Support emails as they is experiencing a backlog of tickets, and giving expectations that may not be met just results in furstrated users. Explain this to the user and also note that sending multiple emails will increase your wait time. You can also send them https://help.minecraft.net/hc/en-us/articles/360042503912-We-re-experiencing-very-heavy-contact-volume-right-now (Absol Factoids: `info/wait-time` for those asking for estimates and `account/send-email/wait-time` for those who are annoyed at the wait times.)

## Account Migration issues
If it is unclear, establish whether the user is trying to migrate from a Legacy account to a Mojang account or a Mojang account to a Microsoft account. If they are trying to migrate a Legacy account, inform them that Legacy -> Mojang migration is currently unavailable but they can still log into the launcher. If they are trying to migrate to a Microsoft account, explain that account migration has not yet started, and link them to the account migration FAQ page at https://help.minecraft.net/hc/en-us/articles/360050865492 (Absol Factoid: `account/microsoft`)

## Trouble buying Minecraft
Establish what country the user is trying to purchase from. If they are in the [US](https://www.amazon.com/Minecraft-PC-Mac-Code/dp/B010KYDNDG), [UK](https://www.amazon.co.uk/Minecraft-PC-Mac-Code/dp/B010KYDNDG/), [France](https://www.amazon.fr/Minecraft-PC-Mac-Code/dp/B010KYDNDG/) or [Germany](https://www.amazon.de/Minecraft-PC-Mac-Code/dp/B010KYDNDG/) they can buy a gift code off Amazon (Absol factoid: `account/buy/amazon`). Otherwise, the most reliable way is to use PayPal or PayPal Guest, which does not require an account. You can access PayPal Guest by selecting the PayPal option at checkout, clicking the PayPal button and selecting Guest Checkout.

If PayPal is not available in the user's country, they must try with different cards and devices. Note that you can't buy Minecraft with prepaid cards, and credit cards seem to be preferred over debit. 

If the user's card was charged but they have not received the game, check whether they received an email from Mojang containing a Transaction ID. If they did not, see [I Was Charged but Did Not Receive the Game](https://help.minecraft.net/hc/en-us/articles/360042693692-Minecraft-Java-Edition-I-Was-Charged-but-Did-Not-Receive-the-Game-) (Absol Factoid: `account/payment/pending`). If they did, see "Can Only Play Demo" above.

If all else fails, it can't hurt to contact Mojang Support if they haven't already.


## If you have no ideas
Run HiJackThis and Adwcleaner to check for incompatible software. For networking issues, have them try on a mobile hotspot and change their DNS (https://1.1.1.1/dns/). Google and https://bugs.mojang.com are also good places to search for issues.

Please also read through the Absol factoid database at https://cp.minecrafthopper.net/factoid?db=minecraft to familiarise yourself with the most important ones.
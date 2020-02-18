# Open Source software and hardware. Your rights and obilgations

### Replies: 149 Views: 3959

## \#1 Posted by: trampa Posted at: 2017-12-07T13:16:51.598Z Reads: 309

```
Hi, 

for given reason I opened this thread about selling hardware containing GPL-licensed firmware and offering downloads for software, licensed under the GNU GENERAL PUBLIC LICENSE (GPL).

Open Source software is a great thing. Unlike hardware, code is usually not visible to the public or the competition. If someone writes code and puts it in the public domain, everyone can make use of the code and learn from the code base, reuse it and mix it. But, depending on the copyright license, there are also obligations to fulfil. The licenses differ, but the core around they are built, is always the copyright law. 

I hope, that reading through this thread will help to understand the matter and avoid violations, which will terminate the GPL-license automatically, putting the violator into a bad legal situation. As soon as you trade or convey a covered work, the terms of the GPL have to be respected. 
The good news: It is not very hard to fulfil the obligations.
The bad news: If you violate the contract you are infringing someone's copyright. 

I hope that this thread will also help customers to understand what their rights are. If you buy hardware containing GPLed, open source software/firmware, you should be able to get access to the source code and you should be able to compile it for your needs. If you are not informed about the fact that your device contains open source software or your vendor fails to inform you how and/or where you can get access to the source code, it is obvious that the GPL has been violated. If you don't get a copy of the GPL-license contract together with your purchase, your vendor probably violated the GPL-license contract. 

Best practice is to actually read the GPL license contract, which can be found here:

https://www.gnu.org/licenses/gpl-3.0.en.html

These are, among others, your obligations and rights:

- If you sell hardware containing GPLed software (e.g. firmware) you convey a work, covered by the GPL license contract. In consequence you need to inform the customer that your device contains Open Source Software and send a copy of the GPL license to each customer you supply. Linking to the the GPL-licens is not a valid form of giving access to the license! At least you should send out an e-mail to each customer, containing the full text of the GPL. You could also print the GPL-license and drop it in the box. 
- If you sell hardware containing GPLed software, all customers have to be informed where the exact source code can be found, or that you will supply a copy on request (written offer). Easiest way to deal with that: Make sure it is easily accessible online, so you can point your customers in this direction. The link should be easy to find on your website, associated to the product. Github is a good option and many sources are available there already. Make sure to store a copy of the code on your hard drive! In case the online availability is not given anymore, you can then upload it again, or send your customers a copy via mail or on a disc. Your customers have a right to access to the source code – if you don't have it, you can't supply it. If they don't know of their rights, you failed to inform them! 
- If you offer downloads for executable GPLed Software, the software itself and the way you distribute it need to be in harmony with the GPL. The GPL-license has to be accessible from the user interface of the software. If it is a derived work (not the original source), your customers need to know that it is a derived work of the original source. Your customers need to know it is GPL-licensed and they need to be able to get access to the exact source code through your service. They need to be able to access the source code, compile the software and run it. If that is not the case something is obviously missing. 
- If you offer a link to an executable GPLed software, make sure that the software you link to is in harmony with the GPL-license. Otherwise you offer a link to a software, which is distributed without permission and license contract from the copyright holder(s). Depending on the applicable law, you may be held accountable for stuff you link! Usually it is best practice to link to the original source of the software, since this is probably the most credible software version, will have all the updates and and you will support the software developers, linking back to them.

I hope this helps to understand the matter a bit better. 

Frank
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-12-07T13:47:40.681Z Reads: 262

```
Bit simpler explanation about GPL https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)
```

---
## \#3 Posted by: trampa Posted at: 2017-12-07T13:50:07.327Z Reads: 258

```
Thx for the link!

Frank
```

---
## \#4 Posted by: Kug3lis Posted at: 2017-12-07T13:51:03.443Z Reads: 250

```
No problem, it's typical stuff then you are contributor to open source projects ;)
```

---
## \#5 Posted by: chaka Posted at: 2017-12-07T14:44:11.910Z Reads: 241

```
How does this relate to the ti instaspin software?
```

---
## \#6 Posted by: Kug3lis Posted at: 2017-12-07T14:50:05.337Z Reads: 241

```
What does TI InstaPin suppose to do with VESC?
```

---
## \#7 Posted by: chaka Posted at: 2017-12-07T14:50:37.056Z Reads: 238

```
It was the starting point in the vesc development.
```

---
## \#8 Posted by: Kug3lis Posted at: 2017-12-07T14:51:59.808Z Reads: 228

```
But it's only for TI microprocessors
```

---
## \#9 Posted by: chaka Posted at: 2017-12-07T14:56:35.697Z Reads: 225

```
I'm just saying, if you write a book and the first few pages were from Hemingway you would want to give attribution right?
```

---
## \#10 Posted by: Kug3lis Posted at: 2017-12-07T14:57:35.637Z Reads: 221

```
If we go this far we should also include GCC, LibC and, ChibiOS and other libraries is used in the code :)
```

---
## \#11 Posted by: chaka Posted at: 2017-12-07T15:00:31.763Z Reads: 216

```
If you study the instaspin software you will see how big of a role it plays in un-sensored motor control and the development of the VESC software. Just trying to find out where the line blurs between proprietary software and open source when we give credit.
```

---
## \#12 Posted by: trampa Posted at: 2017-12-07T15:11:01.833Z Reads: 213

```
This thread is more general. I just want to create awareness. 
This is not predominately VESC-related. It refers to any GPLed stuff sold or distributed.
Once software gets more complex, more parties hold a copyright to parts of the code used.
As soon as you violate the GPL, you infringe the copyrights of all code contributors.
Any of them can terminate their license if the violations are known and not cured within 30 days.
Any of them can go to court. In consequence it is best to work it in harmony with the GPL.

Frank
```

---
## \#13 Posted by: chaka Posted at: 2017-12-07T15:11:07.072Z Reads: 207

```
After reading TI's terms, it seems we are fine as long as we use the code with TI processors.
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-12-07T20:44:54.101Z Reads: 209

```
[quote="trampa, post:1, topic:40375"]
Linking to the the GPL-licens is not a valid form of giving access to the license! At least you should send out an e-mail to each customer, containing the full text of the GPL. You could also print the GPL-license and drop it in the box.
[/quote]

No. You want to print shit and mail it to my customers? fine. You want to write a plugin for shopify for me that automatically sends emails? ok. Short of that, No. They get a link and a good explanation. 

[quote="trampa, post:1, topic:40375"]
f you sell hardware containing GPLed software, all customers have to be informed where the exact source code can be found, or that you will supply a copy on request (written offer). Easiest way to deal with that: Make sure it is easily accessible online, so you can point your customers in this direction. The link should be easy to find on your website, associated to the product. Github is a good option and many sources are available there already. Make sure to store a copy of the code on your hard drive! In case the online availability is not given anymore, you can then upload it again, or send your customers a copy via mail or on a disc. Your customers have a right to access to the source code – if you don't have it, you can't supply it. If they don't know of their rights, you failed to inform them!
[/quote]

No. I'll be more than happy to link to GitHub where Vedder has his project stored already. I'm not creating ANOTHER duplicate file, duplicate repository, or duplicate anything that has to be updated, essentiually forking the fucking thing again. Linking directly the Vedder's own repository IS the best and should be the only acceptable solution.

[quote="trampa, post:1, topic:40375"]
If you offer downloads for executable GPLed Software, the software itself and the way you distribute it need to be in harmony with the GPL. The GPL-license has to be accessible from the user interface of the software. If it is a derived work (not the original source), your customers need to know that it is a derived work of the original source. Your customers need to know it is GPL-licensed and they need to be able to get access to the exact source code through your service. They need to be able to access the source code, compile the software and run it. If that is not the case something is obviously missing.
[/quote]

I'm not decompiling the FocBox variant of the BLDC-Tool to make sure Jason left the fucking comments in there. Fuck that. The source for BLDC Tool is available, i can link to that as well as link to the repository for the firmwares. But what i'm going to offer on my site for the FocBox as a download to work with the FocBox will be the software that came with the FocBox. I'm not going to confuse noobs looking for shit they actually need by shoving a bunch of shit they don't understand in their faces. 

[quote="trampa, post:1, topic:40375"]
If you offer a link to an executable GPLed software, make sure that the software you link to is in harmony with the GPL-license. Otherwise you offer a link to a software, which is distributed without permission and license contract from the copyright holder(s). Depending on the applicable law, you may be held accountable for stuff you link! Usually it is best practice to link to the original source of the software, since this is probably the most credible software version, will have all the updates and and you will support the software developers, linking back to them.
[/quote]

This is the same shit just reworded with thinly veiled threats. The answer is the same. They get focbox software and a link to the original source with plenty of feel goodery and an opportunity to donate and support Ben. Period. 


You keep talking about copyright. Look up First Sale Doctrine. I am a customer of Enertion. That means i can fucking sell this shit without regard to any of the shit Enertion is beholden to. I'm not a distributer. Enertion doesn't ship things to me because they own me or because i'm a subsidiary. They ship things to me because they SOLD shit to me. I can then SELL that shit, as a SECOND SALE, to whoever the fuck i want however i want.
```

---
## \#15 Posted by: mmaner Posted at: 2017-12-07T20:55:49.763Z Reads: 190

```
@longhairedboy @psychotiller  All of that is irrelevant when it comes to you guys.  As vendors you cannot be held liable for licensing issues that are directed at manufacturers, programmers, etc.  This is just more heavy handed bullshit from on high that only has weight if you let it.

I would look at it like this...

If you sold carburetors, you can sell Holley 650 Double Pumper 4 barrel carbs all day long and it doesn't matter if Holley is paying for manufacturing/resale rights from GMC because it uses a ton of the features that originated on the Quadrajet.  It would matter to Holley, but not to you as a reseller.
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-12-07T21:00:44.883Z Reads: 189

```
[quote="mmaner, post:15, topic:40375"]
All of that is irrelevant when it comes to you guys.  As vendors you cannot be held liable for licensing issues that are directed at manufacturers, programmers, etc.  This is just more heavy handed bullshit from on high that only has weight if you let it.
[/quote]

THAT'S WAHT I KEEP TRYING TO TELL THEM. I'm SO DONE. 

I will extend what i believe is the best support I can do right now, because I want to. I want to provide information and i want to support Ben. 

I will not fucking go this far its retarded.
```

---
## \#17 Posted by: psychotiller Posted at: 2017-12-07T23:40:11.714Z Reads: 183

```
Yeah. But no.
```

---
## \#18 Posted by: Deckoz Posted at: 2017-12-07T23:55:41.856Z Reads: 186

```
The DRV is made by TI....


Trampa:
As to selling hardware with gpl'd code... Lol can pretty much do what you want, as your distributing the hardware. The code runs it and your not distributing the 'code' per say. As to get the code you'd have to JTAG and pull the hex file. To even acquire the code..

Go tell every company that sold a computer with a gpl'd bootloader they had to supply the code for binaries already on hardware. Lol

This is a joke and your obviously not familiar with the world of development.
```

---
## \#19 Posted by: Kug3lis Posted at: 2017-12-08T00:00:11.980Z Reads: 185

```
DRV is only Gate controller with some sensing and protections... InstaSpin is algorithm to control BLDC which works "only" on TI microprocessors...
```

---
## \#20 Posted by: Deckoz Posted at: 2017-12-08T00:03:29.101Z Reads: 186

```
Yea but what gate drivers do you think instaspin was made for?
```

---
## \#21 Posted by: Kug3lis Posted at: 2017-12-08T00:06:15.785Z Reads: 181

```
Gate driver is the only element which bootstrap voltage required to turn the gate of the MOSFET, it does no more than if the pin is high turn on if low turn off. Don't mix stuff.
```

---
## \#22 Posted by: Kug3lis Posted at: 2017-12-08T00:06:51.782Z Reads: 179

```
InstaSpin is an algorithm for controlling signal modulation, you don't need DRV for it.
```

---
## \#23 Posted by: longhairedboy Posted at: 2017-12-08T00:13:27.615Z Reads: 181

```
<img src="/uploads/db1493/original/3X/e/a/ea4471a8aa112f46464460174e7a033269666609.png" width="428" height="500">
```

---
## \#24 Posted by: lock Posted at: 2017-12-08T00:47:04.260Z Reads: 177

```
It's really the intent of the license you should aim to follow. While it seems correct; that Trampa writeup is horrible.

Say some smart guy at Enertion came up with a way in software to stop DRVs from blowing, then tried to keep that fix exclusive to focboxes. That would suck as it'd have significant community benefit, it's also what the GPL aims to prevent by requiring you to hand over the modified source under the same license. Really if you have a device or application that includes GPLed code, you should have reasonably easy access to the source.

There's a stack of examples out there. Here's how [BMW complied in one case](https://www.theregister.co.uk/2016/03/30/bmw_complies_with_gpl/).
> BMW has sent Terence Eden a DVD containing GPL-licenced code used in its electric i3 model .
```

---
## \#25 Posted by: trampa Posted at: 2017-12-08T08:14:41.947Z Reads: 174

```
Hi, I don' get the point why everyone freaks out over a 10cm high hurdle that needs to be taken.
Just wanted to help and create awareness. It is not a big deal to fulfil the GPL license.
There is probably a good reason why the GPL wants you to act accordingly.
otherwise the code will drift from OS to quasi-proprietary. 
The source code needs to resemble the **exact** software found on the device.

If you sell hardware with OS- Firmware you convey it. Section 6 GPL.

https://opensource.stackexchange.com/questions/4718/hardware-with-gpl-firmware

_I would like to know if selling a hardware product which runs a firmware is considered as conveying that firmware._

_**Yes.** The binaries are inside the device and are therefore redistributed with the device aka. conveyed._

Simple example: You buy a device in order to re-distribute it. You have access to the firmware sources on the device, since the GPL requires that the wholeseler you buy from has the obligation to provide you with the source code, the information that the device contains GPLed code and the GPL itself.
Since you have the code, you can make it public (best practice) or send out a written offer to supply it on demand.
Since you convey the work, you need to make sure that the customer is informed about the fact that the device runs on, or includes OS software and you need to make sure that the customer can have access to the sources and get the GPL delivered with the product. 

The obligations get passed on from manufacturers to wholesalers and distributors. Each of them have the same obligations. 

It is very easy to fulfil these requirements. Basically an email to the customer can sort out that matter.
You get something for free, as long as you fulfil the license. That is not to much of a demand.
Some additional information on the website will also help.

Frank
```

---
## \#26 Posted by: onloop Posted at: 2017-12-08T10:52:03.127Z Reads: 160

```

## esk8ers don't care about this stuff Frank! they certainly don't want to get emails about license's etc. 

**People just want affordable reliable & programmable motor controllers & most importantly they just want to skate.**

I suggest you rethink your approach to this subject, you are taking it too far with your legal rhetoric & price gouging tactics & in the end, you will eventually be shunned by the majority of people in this community because of these actions. You may go down in history as the guy who actually _killed_ the VESC project. - not the guy who made it better/great!. 

It is questionable whether your actions are of any benefit to VESC/BV, they seem to be of no meaningful benefit to the community or to the advancement of the technology itself & If I were BV I would fire you & distance myself from you and get back to serving the community. - Ben never wanted this mess.

Also, a friendly reminder, this market is very fickle, the second a better motor controller becomes available VESC is dead. There is actually no brand loyalty to the name VESC - actually, you could argue VESC isn't a brand - it was originally a **"community-based-technological-movement"** driven by passionate people who just wanted better electric skateboards. What we all created together as a community was very impressive.

**Don't get me wrong - BV definitely deserves praise and probably money too, but he only got this community so far then stopped to focus on VESC6!**

 * if not for @jacobbloy for taking the risk, doing the 1st ever group buy, making windows & mac compatible software & getting beta units into the hands of esk8rs
 * if not for @chaka  who was able to identify many hardware weakness & make the VESC more robust & reliable.
 * if not for @Blasto for adding, even more, hardware improvements, doing ongoing testing & developing & making form factor changes to improve thermal properties 
 * if not for @Ackmaniac for spending hours & hours trying to tweak software & develop apps to get better results & functionality 
 * if not for the thousands of beta tester that used the VESC and reported back to vendors about problems...

If these people didn't have the passion & want to make the vesc better for everyone the VESC would have died in 2015




----------


----------



Let me leave you with some advice, I always ask myself this question in business, how can my actions benefit all parties involved? WIN-WIN-WIN

Frank, sometimes I think all you are trying to do is WIN for yourself, you forgot that everyone else in the game needs to win as well & that is why you will actually end up being the loser.
```

---
## \#27 Posted by: Surfer Posted at: 2017-12-08T11:26:56.175Z Reads: 159

```
https://www.electric-skateboard.builders/t/news-to-the-name-vesc/23017/58?u=surfer

From may!!
```

---
## \#28 Posted by: trampa Posted at: 2017-12-08T11:59:25.211Z Reads: 167

```
Hi Jason, is it really so hard to send your customers a mail, telling them that the device runs OS software, attached the license. Is it so hard to point the users to the source code? If you are (as a user) not interested in that kind of stuff you don't read it, simple as that. The license is the license and there are good reasons why it is written the way it is written.
The brains behind it are probably quite clever. 

You are saying: The users don't care, so lets not care about the license. It just annoys them, since they are skate brains.
I am saying: The user needs to be able to make that decision himself. You don't harm anyone sending out an e-mail and offering the sources. You harm someone if you fail to do so.

The matter doesn't need to be debated any further. The GPL is applied to the code and it is binding. Your personal attitude towards it, or the uses attitude towards it has **zero** effect on the license. There is simply no choice on the table, since it is a binding license agreement. You accept it the moment you convey a GPLed work. If you violate it you are doing copyright infringement. If you do that twice, any involved copyright holder can terminate your license once and for forever. Section 8 GPL. 

There are multiple parties involved holding a copyright. If you are talking WIN-WIN-WIN, then you should respect other peoples rights! Otherwise you put yourself into a WIN situation while messing around with someone else's copyright.
This is the exact reason why the GPL has been written up and is used so widely. The obligations make sure that the code stays OS and visible. It is a license with a viral character to assure that things stay open, visible and workable. 

I can't understand why people freak out over the content of the GPL license. It is quite a clever piece of paper.
I din't write it BTW Jason, although you want to give the impression that I am responsible that the code is licensed under the GPL. Sorry, not my fault.
I Just wanted to create some awareness and summarize some basic information.
The license works in favour of the **USER**, and those who want to work with the code. In consequence I would not complain to much about it. Because of this license you can use the code for your boards.
The only reason to complain about it is, if you want to use the code proprietary.
Since no one wants to do that I guess, there is no reason to complain.

**It is so easy to comply with the GPL, that it is hardly worth talking about it.**
**It is so easy to comply with the GPL, that is hardly worth violating it.**

Frank
```

---
## \#29 Posted by: jacobbloy Posted at: 2017-12-08T12:16:12.754Z Reads: 163

```
I just want to say that @onloop is 100% right in this. Benjamin 100% deserves credit! I’ll be the first to say this! He deserves to have large financial backing to fortune develop. The biggest thing is so many others in the community also contributed to the vesc being a success. 
In 2015 we did the first production of just 50pcs and struggles to sell them all. We did it at no profit to support the community because it was about time for some thing better to come out. Benjamin was getting flooded with questions asking for help to program and assemble vesc (by some who should never or had never used a soldering iron) we pushed and pushed and I worked to get drivers working for other operating systems and did how to videos to take the strain away from Benjamin. 

I had a lot of conversations with him about the product and how I could help. I put so many hours/money into rewriting BLDC tool to seporate the logic from the ui to allow the development of the android and iOS apps (the point of vesc tool being developed) all to complement the community and the vesc.

A large % of the world can’t code and can’t or won’t use Linux. It was a learning curve for so many. The day that BLDC tool windows and OS X was supported the vesc blew up and so many who couldn’t see them selfs using such a great peace of hardware because of restriction could finally use it and they wanted it so diy stores took advantage of it. Because sadly at this poin Benjamin didn’t want to do any production and after his run of 100 pcs he saw the effort that went into it and didn’t see the benefit in doing this.

we saw another massive increase in vesc through the free publicity that it was getting on this forum, from 100’s to 1000’s of users talking about it praising or complaining about faults. This led to 10,000’s owning vesc.

The vesc and the reason for licensing was made huge because of this community and you took it away.

I 100% think that each vesc sold should have a contribution to Benjamin and the only way to track this might be through licensing and vesc tool. But if the community the chance to have what they helped to develop as a brand and let them keep using the vesc 4.12 and profit of the vesc 6 with its amazing benifits in the automotive or other big industries. The diy community is small and wont give Benjamin $60,000 a year to develop while the price of a vesc 6 is $350 each. But they did when it was being sold $150 each.

There buying diy because it’s better for cheaper. Not better with high price tags and licensing.

I know your talking about the GPL licensing and not the trade mark but as I said the diy community arnt who you need to be informing about this.
```

---
## \#30 Posted by: jacobbloy Posted at: 2017-12-08T12:37:13.833Z Reads: 153

```
I personally haven’t touched any thing to do with with the vesc in so many months maybe I shouldn’t comment.
```

---
## \#31 Posted by: longhairedboy Posted at: 2017-12-08T12:39:56.670Z Reads: 154

```
Also Ben's getting money from me in January anyway. A backpayment, if you will, for the e-switches. Because I do actually have the eswitches made at a factory and the hardware for that is open source. There is no software involved, and i did make a minor upgrade to it, but it is his hardware and in spite of only moving maybe 80 of them and paying to have them made and burning up half of them trying to figure out why they sucked and talking to people and testing and burning and testing and falling on my face a few times, I'm going to send him a percentage of the sales. 

Not because i feel morally obligated or am being forced to comply. But because i WANT TO support him. The same way I WANT to support this entire community and ALL of the hard work they've done. The same way they have supported me. 

Ben wouldn't be the INFAMOUS BENJAMIN VEDDER (reverb on 11) if it wasn't for this community, I wouldn't be in business if it wasn't for this community, @onloop would be at home on the shopping channel while his wife does brain surgery and @chaka would be making cabinets for people who don't know what the fuck they want in their kitchen. Chris chaput might even have hair. Utter pandemonium, dogs and cats living together, total protonic reversal. 

everyone here is responsible for everyone else being here. We all support each other anyway, take your lawyers and fuck off.
```

---
## \#32 Posted by: onloop Posted at: 2017-12-08T12:56:56.862Z Reads: 157

```
[quote="trampa, post:28, topic:40375"]
If you violate it you are doing copyright infringement. If you do that twice, any involved copyright holder can terminate your license once and for forever. Section 8 GPL.
[/quote]

So now Benjamin Vedder is going to be using his precious time policing _(instead of developing)_, vendors from all over the world who are selling a vesc based product, to check they are sending an email _(that nobody will read)_ explaining the license, so that he can be sure they are in compliance with the license? 

& Further to this, when they are ALL found to be breaching this rule, he is going to terminate them, essentially destroying the entire market and driving demand to the Chinese suppliers who don't give a shit about the project or Vedder?

Surely his time & yours would be better spent trying to make the VESC6 a viable product in the market? 

I fully understand that everything you are preaching is written law, But this is so backward... Do you realize If you didn't trademark the name VESC - than it would have been self-explanatory to all people globally buying VESC that is was indeed a VEDDER.E.S.C - Vendors always wanted Vedder to get the recognition, that's why vendors never invented new names. But ironically you forced them to not use the name VESC.

It so stupid i feel i need to summarise, You forced vendors to stop using the name VESC _(which seriously diluted the brand)_ & now you are forcing the same vendors to tell everyone, in a special email, that it is actually a VESC! _(Because you clearly want that publicity again)_ - & if they don't you will terminate them 

It seems you made a strategic error, i would fire you if you were my business consultant.
```

---
## \#33 Posted by: longhairedboy Posted at: 2017-12-08T13:26:18.197Z Reads: 152

```
Maybe instead of buying a VESC6 we should all just send Ben $10 and buy a fucking FocBox.
```

---
## \#34 Posted by: trampa Posted at: 2017-12-08T13:28:22.754Z Reads: 155

```
You clearly don't understand the matter and mix things up that have nothing to do with another Jason.

**This thread is about the GPL and creating some awareness.** It is not even specifically related to a certain OS project. 

A software under the GPL license may contain **multiple** copyrights from **various authors**. A few have been named here already. The GPL license has been applied by all of them for given reasons.  
Any of them have the same rights when it comes to copyright infringements. In consequence it is good to know that and educate yourself about the matter when you trade or convey GPLed stuff. You can still make the decision to simply not care about the fact, close your eyes and hope that no one will care about what you do. This is totally up to you.
However, it is simply stupid to act like that, since it is totally unnecessary to do so. 
Still don't get the point why it is so hard to inform your customers and give them access to the sources.
It is no big deal. 

**In that mail or manual etc. you simply need to tell people that the thing contains OS-Code, this is the license and this is how you can get access to the sources**. 

Seams to be a very complicated matter... 

Frank
```

---
## \#35 Posted by: onloop Posted at: 2017-12-08T13:32:28.601Z Reads: 151

```
[quote="trampa, post:34, topic:40375"]
Still don't get the point why it is so hard to inform your customers and give them access to the sources.
[/quote]

it's there, it's accessible, always has been, always will be....   

<img src="/uploads/db1493/original/3X/8/d/8dd53b1f10c126eec4ae60d6175a61a56c75f907.png" width="285" height="214">
```

---
## \#36 Posted by: trampa Posted at: 2017-12-08T13:41:00.456Z Reads: 148

```
That is a link to Benjamins website. What has that to do with the matter?
```

---
## \#37 Posted by: mmaner Posted at: 2017-12-08T14:05:28.169Z Reads: 150

```
This is as big a bunch of bullshit as I've ever seen...

[quote="trampa, post:34, topic:40375"]
This thread is about the GPL and creating some awareness. It is not even specifically related to a certain OS project.
[/quote]

...yet, we have threats...

[quote="trampa, post:12, topic:40375"]
As soon as you violate the GPL, you infringe the copyrights of all code contributors.
Any of them can terminate their license if the violations are known and not cured within 30 days.
[/quote]

@trampa you cant talk out of both sides of your mouth and expect people to have any respect for what you say.  This began with you attempting to stop people from using the name VESC.  Well, you did that.  Now your seeing that FocBox is the name getting talked about so you wanna get VESC back in the mix.  Too bad.  THis whole enterprise since you took over has been a mistake and no good for anyone, especially Ben.

@onloop just do you brother, Trampa hasn't done anything to benefit anyone, you have.  I'm not trying to put a halo on you, just saying that your products have made electric skateboards much more viable and available to the masses.  The only reason I'm even in this conversation is because I hate to see people with money create a 'legal' situation where they can bully others into increasing their profit margins.  

An open request to Ben Vedder:
Dude, you gotta get out here and say something.  Frank is ruining your name and is essentially guaranteeing you  a substantial loss in profits.  If you would just make a statement to say what YOU want this whole issue could be resolved once and for all.
```

---
## \#38 Posted by: PXSS Posted at: 2017-12-08T14:05:32.983Z Reads: 146

```
[quote="longhairedboy, post:31, topic:40375"]
but it is his hardware
[/quote]

It is not!!!! Vedder copied the design over from Fetcher on Endless Sphere. Put your pennies away
```

---
## \#39 Posted by: longhairedboy Posted at: 2017-12-08T14:36:08.526Z Reads: 143

```
Oh. Well then. 

More skittles for me!
```

---
## \#40 Posted by: mmaner Posted at: 2017-12-08T14:49:09.876Z Reads: 147

```
[quote="PXSS, post:38, topic:40375"]
It is not!!!! Vedder copied the design over from Fetcher on Endless Sphere
[/quote]

That's a hell of a game changer...
```

---
## \#41 Posted by: trampa Posted at: 2017-12-08T14:57:39.715Z Reads: 147

```
Sorry guys, why do you think that the TM and the GPL-obligations have anything to do with another?
Why do you think that you need to use the VESC-Brand to comply with the GPL?

For software you need to state that it is OS, a copyright notice, offer the sources, the GPL-license and that is about it. 
Sure, the copyright will show Benjamin Vedders name, which obviously differs from VESC.
If you offer modified software/firmware you need to state that it is a modified version of the original software by e.g. Benjamin Vedder.
You can ad an "About" button in the menu bar and drop the licensing and copyright notice there. 
Open Firefox >> Help >> About and you will see.

Frank

@PXSS what design are you talking about? Software or Hardware. We are talking software and GPL.
```

---
## \#42 Posted by: Kug3lis Posted at: 2017-12-08T14:59:56.345Z Reads: 149

```
That's why I "love" companies selling OS and then trying to get involved in fair trades... :D
```

---
## \#43 Posted by: rene Posted at: 2017-12-08T15:02:42.204Z Reads: 148

```
Sorry guys - stop shooting the messenger!

I am only six weeks to this awesome community of esk8ing
- but I am in software for decades ('84 as I turned 12 years old)

There is GPL in all that VESC / VESC-Tool / BLDC-Tool / Firmwares etc.
Thats why "it" has to include GPL information.

Thread will not come from Vedder or Trampa - 
it will come from FSF (FreeSoftwareFoundation) [https://www.fsf.org](https://www.fsf.org).
Its big, well founded and it has the right to sue.

@onloop - is right (nobody does care about GPL)
@trampa - is right (GPL Information has to be included )

We are all giants on the shoulders of others.

Cheers from Hamburg / Germany,

René

PS: 
Owner of four Focboxes, two "vesc" made in DK, just soldering his first batterypack.
Beeing thankfull to this forum-community and its founder. 
Bought the $20 Version of the VESC-Tool to support B. Vedder.
```

---
## \#44 Posted by: Kug3lis Posted at: 2017-12-08T15:03:30.558Z Reads: 148

```
What about ChibiOS GPL license why you don't include it too?
```

---
## \#45 Posted by: Kug3lis Posted at: 2017-12-08T15:10:00.856Z Reads: 149

```
I don't see anywhere mentioned that it uses ChibiOS not in your store, not on the vesc-project website... So please stop talking about GPL then you guys yourself violate it ;)
```

---
## \#46 Posted by: gogomrrobot Posted at: 2017-12-08T15:26:43.343Z Reads: 147

```
[quote="Kug3lis, post:45, topic:40375, full:true"]
I don't see anywhere mentioned that it uses ChibiOS not in your store, not on the vesc-project website... So please stop talking about GPL then you guys yourself violate it ;)
[/quote]

I figure this is all politics and theatre...but I agree with @onloop 

@onloop could just block all Trampa threads on here in a minute. Delete and even mention of their website name if so desired. I don't see it happening.

@trampa could give us a $99 USD one day special on VESC6 as makeup for doing nothing for us on Black Friday or Cyber Monday.  They could lower the price of the VESC6 permanently to $150... win the hearts and minds and wallets of our community.  Now he will come in here and drone and drone about paying BV and employees and god save the queen.  Slow moving avoidable but inevitable & guaranteed trainwreck in progress
```

---
## \#47 Posted by: mmaner Posted at: 2017-12-08T15:41:36.224Z Reads: 148

```
[quote="gogomrrobot, post:46, topic:40375"]
Slow moving avoidable but inevitable & guaranteed trainwreck in progress
[/quote]

This is very concisely stated, good on you.

I'm gonna just put this out.  If there is someone who can prove without doubt that the original VESC design was not BV's in a well documented and cited thesis I've got $100 I will PayPal you as soon as I have it in my email.  

Furthermore, if there is someone who wants to completely rewrite the code so that none of BV/Trampa code is used making the software/firmware completely independant of the Trampa trademark (@Ackmaniac I'm looking at you), completely open source, not for re-sale available to the world at large I've got $1000 to give you.  I realize that is just a drop in the bucket, considering the time it will take.  I also think there's at least 5 other people/vendors in this thread that will match that donation, not too mention all the $5 donation that will flood in.

I feel for Ben, I really do...but...I think he shit all of his respectability down the toilet when he turned his legal and marketing mouthpiece out.  I'm done, putting my money where my mouth is.
```

---
## \#48 Posted by: trampa Posted at: 2017-12-08T15:49:10.694Z Reads: 151

```
Well, if that is the case, than it will be fixed ASAP. If you read the GPL V3, it gives violators the chance to cure any issues after notification from the copyright owner within 30 days. As soon as you realize that there is an issue you should fix it immediately. I'm open to criticism and if someone points out an issue, it can be fixed. That is how things should work. 

If you will go through this thread, then you will see, that I tried to keep it non specific to a certain project.
There are quite a few OS-projects around in the world of e-skating, e-biking etc. Just wanted to create awareness.

The reason why I chose to come up with it was helping vendors understand the matter and create awareness.
If you are aware of something, you can act accordingly. If you are not aware of something you are likely to fail in being compliant. 

Is it a bad thing to be pointed to relevant information for your business?  Probably not. 

I didn't come up with donations developer support and the like... I try to stay on topic.

Frank
```

---
## \#49 Posted by: Kug3lis Posted at: 2017-12-08T15:54:33.071Z Reads: 152

```
I have been OS developer for over a decade now... My one of the biggest libraries are released under MIT and has over 50 billion installs and I have received 0 donations for my time spent on it and I don't go to the forums and cry that oh well I did some work please pay me. You released your code as an open source project don't expect money from it otherwise use a different license. I hate to see people who say oh it's OS but please don't forget to donate to it.
```

---
## \#50 Posted by: trampa Posted at: 2017-12-08T15:58:59.154Z Reads: 152

```
I didn't come up that @Kug3lis. No outcry for donations. 

Frank
```

---
## \#51 Posted by: Kug3lis Posted at: 2017-12-08T16:01:12.322Z Reads: 149

```
[quote="trampa, post:75, topic:26862, full:true"]
If you buy them with a board, 187 GBP is the price. US customers usually pay 240 GBP for a single unit. I hope @stewii has priced some $$ in for Benjamin. 95% of the hardware vendors forget to do so. Cheap Cheap Cheap and let's forget about software development.... Without the software those units would not spin a motor a quarter turn.

Frank
[/quote]

10char....
```

---
## \#52 Posted by: Kug3lis Posted at: 2017-12-08T16:03:24.551Z Reads: 148

```
So according to you why don't pay a cut for ChibiOS, Qt, GCC, and other libraries for the time spent on developing because without them there would not be spinning motor?
```

---
## \#53 Posted by: trampa Posted at: 2017-12-08T16:03:27.107Z Reads: 148

```
But that has nothing to do with this thread. That is a separate matter.
```

---
## \#54 Posted by: Kug3lis Posted at: 2017-12-08T16:04:05.760Z Reads: 150

```
That's not separate matter. It's talk about OS code and hardware and paying for it because you sell it.
```

---
## \#55 Posted by: Kug3lis Posted at: 2017-12-08T16:11:35.972Z Reads: 149

```
So please stop all this non-sense, @trampa you yourself not include all required licenses and etc so just forget about it.
```

---
## \#56 Posted by: mmaner Posted at: 2017-12-08T16:24:51.419Z Reads: 148

```
You are a Rock Star @Kug3lis, great info and glad to see it out there for EVERYONE to see.  Is there such a thing as an open-source smack down :slight_smile:
```

---
## \#57 Posted by: Surfer Posted at: 2017-12-08T16:37:34.163Z Reads: 146

```
Every time Frank shows up here, he is losing customers.
```

---
## \#58 Posted by: Surfer Posted at: 2017-12-08T16:40:02.583Z Reads: 144

```
Frank are you doing this on endless Sphere and all the other forums ?
```

---
## \#59 Posted by: trampa Posted at: 2017-12-08T16:42:06.780Z Reads: 143

```
Sorry for putting a discussion on. I wish you all a relaxing weekend. 

Cheers, Frank
```

---
## \#60 Posted by: b264 Posted at: 2017-12-08T17:00:15.146Z Reads: 149

```
[quote="mmaner, post:47, topic:40375"]
Furthermore, if there is someone who wants to completely rewrite the code so that none of BV/Trampa code is used making the software/firmware completely independant of the Trampa trademark (@Ackmaniac I'm looking at you), completely open source, not for re-sale available to the world at large I've got $1000 to give you.
[/quote]

Put me down for $100 on top of that, as long as it's a copylefted open-source license.

Also, I completely believe in open-source.  I run all open-source software on my machines.  However, I find it very difficult to believe that all of this is coming from the very person trying to kill off VESC with legal bullshit and trademarks.
```

---
## \#61 Posted by: gogomrrobot Posted at: 2017-12-08T17:25:59.548Z Reads: 145

```
You have to remember that Mongo, Redhat, MySQL as examples began as open source. And they do still have free editions available. As well as corporate / enterprise edition versions that provide extra features and support -- and they cost mega-bucks for that version. Just this past week we wanted to start using MongoDB at work... and the price for (3) nodes and sharding and memory storage headed into the $100,000's. Lol was a shock.  Even Linus Torvalds got paid $150,000,000 in RedHat stock when they went public. So there was / is some great open source wealth out there.

The difference though -- all of those products have open source editions and none tried to do a generic blanket all trademark name BS which I don't know is even enforceable. i.e. it's like saying can't use the word Linux... only RedHat can.  And Redhat isn't the only Linux commercial vendor... what about Debian, or Fedora, etc. Curious to see if Trampa takes somebody to court and it sticks.  Well probably too expensive to find out. Likely people will stop using the VESC name before that. But it would be interesting to test the law.
```

---
## \#62 Posted by: Kug3lis Posted at: 2017-12-08T17:35:00.397Z Reads: 140

```
Wtf cluster you there running at my current job we are running 33 server cluster for way less than 100k :D
```

---
## \#63 Posted by: gogomrrobot Posted at: 2017-12-08T17:39:01.141Z Reads: 138

```
[quote="Kug3lis, post:62, topic:40375, full:true"]
Wtf cluster you there running at my current job we are running 33 server cluster for way less than 100k :D
[/quote]

Yeah we have "Oracle" DBA's who don't understand the NoSQL pricing model likely they overpaid for something. It's a very large company... that's what they quoted... maybe some Tier 1 support from them too. You work for a startup so likely you didn't get dealt that way.

EDIT: Lol, let's take this offline... we gonna put people to sleep ;)
```

---
## \#64 Posted by: ATLesk8 Posted at: 2017-12-08T17:45:01.788Z Reads: 138

```
From a fairly new member as far as the guys in this thread go; I will never buy a single piece of Trampa hardware. This is an absolutely ridiculously atrocious way to alienate an entire community of a very niche market. Most people here aren't so brand loyal that they're willing to pay 2-3 1/2 times market value because it says Vesc...Get FOCed
```

---
## \#65 Posted by: longhairedboy Posted at: 2017-12-08T17:47:42.667Z Reads: 141

```
[quote="gogomrrobot, post:61, topic:40375"]
The difference though -- all of those products have open source editions and none tried to do a generic blanket all trademark name BS which I don't know is even enforceable. i.e. it's like saying can't use the word Linux... only RedHat can.  And Redhat isn't the only Linux commercial vendor... what about Debian, or Fedora, etc. Curious to see if Trampa takes somebody to court and it sticks.  Well probably too expensive to find out. Likely people will stop using the VESC name before that. But it would be interesting to test the law.
[/quote]

That's the scariest shit i've read all day and none of that even occurred to me, but it probably should have. I'm a web developer and have been using open source tools for 20 years. I watched mysql rise and get eaten, maria drop out of that, apache grow from shit bandaided together into the world's number one web service platform, endless policy and standards battles, and then this. 

If that stuck it would set the worst precedent we've ever seen for os legal buttfuckery. There's no way a sane judge with eyeballs and a proper legal team could let that happen. I'd be willing to hack pacer if it meant getting that out of the light.
```

---
## \#66 Posted by: mmaner Posted at: 2017-12-08T19:17:02.948Z Reads: 139

```
Looks like there's some money to be made here :slight_smile:
```

---
## \#67 Posted by: trampa Posted at: 2017-12-08T19:41:37.370Z Reads: 139

```
[quote="gogomrrobot, post:61, topic:40375"]
The difference though -- all of those products have open source editions and none tried to do a generic blanket all trademark name BS which I don't know is even enforceable.
[/quote]

The VESC TM policies are pretty much a straight copy of the Linux TM policies. Yes, Linux is trademarked! So there is not to much difference. No one complains about Linux and all the other well known OS projects having a TM. Funny.... Pretty much all of them have a TM and use a OS copyleft license. Probably for a good reason...
And there is nothing wrong about that.

Everyone wants the software to be Open source, and the very foundation of that is the OS-copyleft-license. So where is the problem? The GPL is giving everyone the right to use the code free of charge, as long as certain things are being respected. The code for VESC-Tool is GPLed and available. There is no blanket. 

Frank
```

---
## \#68 Posted by: gogomrrobot Posted at: 2017-12-08T19:53:23.517Z Reads: 137

```
Yeah but you are saying only Trampa can use the name VESC everyone else has to call it something else.

Vedder ESC = VESC
Linus Unix = Linux
```

---
## \#69 Posted by: PXSS Posted at: 2017-12-08T19:53:57.487Z Reads: 135

```
[quote="mmaner, post:47, topic:40375"]
can prove without doubt that the original VESC design was not BV's in a well documented and cited thesis
[/quote]

***I WAS NOT TALKING ABOUT THE VESC, I WAS TALKING ABOUT THE ANTISPARK SWITCH***

@longhairedboy
@trampa
```

---
## \#70 Posted by: longhairedboy Posted at: 2017-12-08T19:54:28.198Z Reads: 136

```
[quote="trampa, post:67, topic:40375"]
No one complains about Linux
[/quote]

Linux has been around since i was in highschool. the people complaining have grown tired, died, or given up on complaining publicly. But believe me, i'll bet there's a lot of people drinking themselves to sleep at night swearing Linus Torvald's name. Torvalds is a man with vision and of respect. Executing that vision and commanding that respect takes grit. A seriously accomplished individual of recognizable stature and class. And a lot of people hate the way he has treated  developers in the community. He's been known to engage in tyrannical tirades featuring personal attacks over simple semantics. 

Noone will ever complain about you the way they complain about Linus Torvalds or Linux.
```

---
## \#71 Posted by: trampa Posted at: 2017-12-08T20:05:38.198Z Reads: 134

```
However, I just want people, vendors, users etc to be aware of copyleft-licenses. This all I wanted to start a debate about. Those licenses are the only instrument available to allow sharing you copyright. 
It's a good thing they exist and you should be aware of how they work. 

Frank
```

---
## \#72 Posted by: Kug3lis Posted at: 2017-12-08T20:17:44.973Z Reads: 135

```
What do you want then you yourself not aware of this stuff? Please just stop your making fun of yourself already. You want others to be aware then you guys yourself are not aware not even 10% and coming here with shit storming trying to make everyone to do as you wish. 

The whole VESC is based of several reference designs and code is also not even 40% handwritten its pieced together solution on which you putted TM and now you ask everyone to be aware of license then you yourself not include any single dependency license that you use. So just please STOP it
```

---
## \#73 Posted by: chaka Posted at: 2017-12-08T20:23:43.772Z Reads: 133

```
Well it seems you were the one that needed the lecture. I am going to completely honest, you have contributed nothing but FUD to this community and @onloop is 100% correct. You have killed the VESC.
```

---
## \#74 Posted by: longhairedboy Posted at: 2017-12-08T20:35:24.299Z Reads: 136

```
[quote="chaka, post:73, topic:40375"]
@onloop is 100% correct
[/quote]

i'm too distracted by this particular fragment to even say something witty about it, suffice to say i just choked on my coke.
```

---
## \#75 Posted by: b264 Posted at: 2017-12-08T20:46:04.277Z Reads: 135

```
@frank Why don't you perpetually license the "vesc" letter combination to the general public?  What reason is it that you continue to choose not to do this?

Please, enlighten us.  Let's discuss it.  Because unless/until you do, the worst & most shady reasons will be assumed by the public at large.

Also, "VESC Tool" is already licensed under GPL (copyleft) and the VESC hardware itself, designs including the word "VESC",  is licensed under CC BY-SA 4.0 (share-alike), so it's unlikely you have any kind of solid case, anyway.  These two licenses *specifically* prevent what Stallman called "hoarding".

So it would seem on the outside all you are doing is losing face by trying to hoard.  And then opening a thread about not hoarding.
```

---
## \#76 Posted by: ATLesk8 Posted at: 2017-12-08T20:51:05.985Z Reads: 134

```
Somebody get Trampa a backhoe...They obviously enjoy digging their own vesc grave, so why not expedite the process?
```

---
## \#78 Posted by: trampa Posted at: 2017-12-08T23:43:21.662Z Reads: 132

```
@b264 this is completely off topic, but here are your answers.

a) Because you can't license a TM to the public. That would contradict its purpose.
b) A TM serves the purpose that customers/users can identify the original or a specific source. 
c) Benjamin owns it, so its up to him. 
d) The TM assures that only he can brand or license products/software that he approved to meet his quality standards.
e) without a TM, someone can hijack an OS project, grabbing a domain, using the same brand name and making the service look identical. Uninformed users could not see the difference and would believe they deal with the original source. 
f) products a poor quality, marketed under the same brand name, have a negative impact on the brand itself.
g) GPL and CC both don't license assigned TM's. They license the covered work only

This is quite informative: http://fossmarks.org/

Even the Open Source Initiative has a trademark: https://opensource.org/trademark-guidelines
And GNU as well! The biggest promoters of Open Source! 

List of OS projects owning the rights to their name: https://en.wikipedia.org/wiki/List_of_trademarked_open-source_software

So if everyone in the OS-World uses TMs, there is probably a very good reason for it.
And since you don't know what the future will bring, you better have a TM.

But this has nothing to do with the topic! 

Frank
```

---
## \#79 Posted by: gogomrrobot Posted at: 2017-12-09T00:04:33.246Z Reads: 132

```
YOU WANT TO WIN? You want to stick it to Jason and win our hearts? Lower the price to $150. Make it up in your boards. Make it up in other ways. Until then... it's all scum-baggery. I know your biggest issue.. is that you don't believe in us.  If the price is right and the feeling is right... you will take a small cut on a component and win. And win big. Your boards are sexy... it was a phase for me. They wobble a bit... but on the sexy still. The E-MTB's rule on the mountain.

You can have it all... and you can win.  You can be the reference design and what people aim for. And at a price point that people will have to consider. This is what winners do.  I think you pull out your calculator each time... and decide... "F them... not me". Reverse... back-peddle. Admit your mistake and survive... show humbleness and win. Your defiance... will destroy you.

Sorry this is some drinking talk but still true. 

EDIT: TMI before ;)
```

---
## \#80 Posted by: Deckoz Posted at: 2017-12-09T00:41:55.118Z Reads: 132

```
$150 is about right

$2-7 for the PCB
$107 BOM and maybe 1.5kWh to heat the oven and reflow
$4 of aluminum stock. And 2.6kWh(0.16¢/kWh) to mill.
```

---
## \#81 Posted by: Kug3lis Posted at: 2017-12-09T00:46:40.871Z Reads: 135

```
Your all this talk makes me want to go fork the code rewrite from scratch (I was intending to do because there are newer chips which are cheaper) Make it completely MIT proof and then release to the public and then I would like to see what your TM branded bullshit will look like against completely open source project?
```

---
## \#82 Posted by: PXSS Posted at: 2017-12-09T00:58:45.135Z Reads: 137

```
Do it! I would support you full on wherever I can.
```

---
## \#83 Posted by: gogomrrobot Posted at: 2017-12-09T01:13:20.668Z Reads: 138

```
[quote="Deckoz, post:80, topic:40375, full:true"]
$150 is about right

$2-7 for the PCB
$107 BOM and maybe 1.5kWh to heat the oven and reflow
$4 of aluminum stock. And 2.6kWh(0.16¢/kWh) to mill.
[/quote]

That's what @stewii said who identically built his clone VESC6 in small quantities. Even with the MP9250 motion tracking chip he paid $67 (50 pounds). For quantities of 5-10 units. In mass production maybe $50/each. Fuc i would put up money for 1000 units. Could still chip in $10 to BV. $90 profit roughly per VESC.... 180% roi? da fuq already

@stewii VESC6 clone: 
<img src="/uploads/db1493/original/3X/a/c/ac830b347eba65dc9b7042fa49929fed747eeca3.JPG" width="666" height="500">
```

---
## \#84 Posted by: Deckoz Posted at: 2017-12-09T01:18:59.463Z Reads: 132

```
Yea my prices above are for stweii esc that I started building. Prices are for 1. Ordering 10 BOM straight from digikey comes down to about $85.
```

---
## \#85 Posted by: Cobber Posted at: 2017-12-09T01:45:29.023Z Reads: 133

```
Seems this has turned into a discussion about general IP (Intellectual Property) rights, relative to a trademark or even a patent who knows why the application date is important and what it means?
```

---
## \#86 Posted by: gogomrrobot Posted at: 2017-12-09T01:50:52.831Z Reads: 134

```
[quote="Cobber, post:85, topic:40375, full:true"]
Seems this has turned into a discussion about general IP (Intellectual Property) rights, relative to a trademark or even a patent who knows why the application date is important and what it means?
[/quote]

Another Trampa shill... beats me up and cries like the English patient everytime i say something about them.

The Empire strikes back.. lol :slight_smile:
```

---
## \#87 Posted by: Cobber Posted at: 2017-12-09T02:02:43.273Z Reads: 136

```
[quote="gogomrrobot, post:86, topic:40375"]
Another Trampa shill... beats me up and cries like the English patient everytime i say something about them.

The Empire strikes back.. lol :slight_smile:
[/quote]

You are nonsensical dude? way off base, but I'm guessing nothing new there eh?
Way to turn a up and up discussion on the down low :thumbsup:
By all means sledge away, but you might be more effective if you are actually on topic and there is some truth in what you are saying...

I'm not talking about trampa at all as I said:

[quote="Cobber, post:85, topic:40375, full:true"]
Seems this has turned into a discussion about general IP (Intellectual Property) rights, relative to a trademark or even a patent who knows why the application date is important and what it means?
[/quote]

I think we can put a red mark against mrrobot as he has no idea, anyone else?
```

---
## \#88 Posted by: ATLesk8 Posted at: 2017-12-09T02:07:34.693Z Reads: 130

```
Yeah...I don't like that mr robot man used naughty words and hurt my feelings...safe space /s
```

---
## \#89 Posted by: gogomrrobot Posted at: 2017-12-09T02:09:07.977Z Reads: 131

```
You are a Trampa  shill... and @koralle and a few others

stop Cobber... please just stop...

<img src="/uploads/db1493/original/3X/1/c/1c3ef57f8e5a898af8da99915939a6932a92b383.PNG" width="281" height="499">
```

---
## \#90 Posted by: Kug3lis Posted at: 2017-12-09T02:16:14.553Z Reads: 128

```
tl;dr; of this topic is that Trampa wants to monopolize VESC and I guess it triggered the focbox sales with over 500 units sold :D Imagine how much he grieves about it :D
```

---
## \#91 Posted by: Cobber Posted at: 2017-12-09T02:17:08.674Z Reads: 130

```
you should publish the whole lot dude, but please don't clog up this discussion with rantings of your own inadequacies. 
Put it all in perspective for people... You should start your own topic ;)

**What does a trademark application date mean?**
From that date the owner of the mark has the right to use the mark in the marketplace unopposed by new users of the mark.

What that means in practice:
Fred Sunny has a trademark on Sunny Widget that he applied for last week and was granted yesterday.
Today if someone else markets a product as Sunny Widget he has the right to defend his mark with litigation to protect his business and the consumer.
But there are caveats:

1. If my name is Jim Sunny I can also market my Widget as Sunny Widget because Sunny is my name.

2. Jimbo Bob has been selling a Widget he makes that he also called a Sunny Widget since last year, the marketplace therefore knows his Widget as a Sunny Widget. Jimbo Bob can continue to sell his Sunny Widget because his use of the mark pre-dates Fred Sunny’s trademark application.

Whilst according to the letter of the law Jim and Jimbo should be able to continue selling their Sunny Widget, if Fred Sunny has deep pockets he can try to drive them out of the market with pointless litigation that he will lose but will end up costing Jim and Jimbo money and time to defend themselves against.
```

---
## \#92 Posted by: mmaner Posted at: 2017-12-09T03:00:54.357Z Reads: 129

```
[quote="Kug3lis, post:81, topic:40375"]
Your all this talk makes me want to go fork the code rewrite from scratch
[/quote]

Do it...for all of our sake please do it!  There are tons of people that would support you, including me. PM me and we can discuss.
```

---
## \#93 Posted by: trampa Posted at: 2017-12-09T10:46:29.290Z Reads: 129

```
Take a book, rewrite it, same story, other words, very inventive, very impressive, copyright is still with the original author, especially after making your intentions public in the first place.

If I would be desperate to write a novel, I would write up my own story and own chapters. 

Frank
```

---
## \#94 Posted by: DavidBanner Posted at: 2017-12-09T10:50:27.070Z Reads: 127

```
Frank,

I think you may be mistaken.

Here is an example of your analogy IRL: [https://www.theguardian.com/uk/2007/mar/28/danbrown.books](https://www.theguardian.com/uk/2007/mar/28/danbrown.books)

As for software, what you just described has been going on since before Steve Jobs owned a garage.
```

---
## \#95 Posted by: trampa Posted at: 2017-12-09T10:57:36.307Z Reads: 127

```
Honestly, I would rather commit to the code base, help to make it better and get in touch with the guy who put a lot of effort in and knows every detail.

I don't get the point about the obsession to rip things apart. 

Frank
```

---
## \#96 Posted by: DavidBanner Posted at: 2017-12-09T11:03:36.656Z Reads: 126

```
[quote="trampa, post:95, topic:40375"]
I don't get the point about the obsession to rip things apart.
[/quote]


That is the coder/DIY mindset :slight_smile:

Open it up, how does it work? Can I make it work better?

I could seen an approach where someone looks at the existing codebase/HW, then sits down at the drawing board and comes up with something of their own creation. We are all standing on the shoulders of giants....

There is a really cool series called Halt and Catch Fire, it explores the exact topics we are talking about, I think you might enjoy it, I know I did
```

---
## \#97 Posted by: DavidBanner Posted at: 2017-12-09T11:14:28.876Z Reads: 126

```
Here is a little gem of a conversation (allegedly) between Bill Gates and Steve Jobs, I think it speaks volumes as to how both companies were being operated (at the time anyway): 


Steve Jobs confronted Bill Gates after he announced Windows' GUI OS. "You’re stealing from us!” Bill replied "I think it's more like we both had this rich neighbor named Xerox and I broke into his house to steal the TV set and found out that you had already stolen it."
```

---
## \#98 Posted by: PXSS Posted at: 2017-12-09T14:00:27.944Z Reads: 123

```
[quote="trampa, post:95, topic:40375"]
I don't get the point about the obsession to rip things apart.
[/quote]

I think you do, especially since you are destroying the VESC in this community
```

---
## \#99 Posted by: chaka Posted at: 2017-12-09T16:17:27.721Z Reads: 123

```
@cobber has been trolling me in private too. The funny thing is he was positioning himself against Trampa in his messages.
```

---
## \#100 Posted by: Kug3lis Posted at: 2017-12-09T16:17:45.615Z Reads: 123

```
Dude, YOU HAVE ZERO understanding how software world works, if that was the case you would not have any single application today. Go read some literature before trying to argue with a person who is doing professional software development more than half of my life.

Plus who wants to commit the code base then this kind of shit happening? You just trashed the whole Benjamin work in front of many people.
```

---
## \#101 Posted by: gogomrrobot Posted at: 2017-12-09T16:39:44.066Z Reads: 130

```
[quote="chaka, post:99, topic:40375, full:true"]
@cobber has been trolling me in private too. The funny thing is he was positioning himself against Trampa in his messages.
[/quote]

It's all strategy, I have seen this before. I can't get into the specifics... but it was in 2005, I built a pay-per-click software... it was generating like $100k / week hard cash flow. They were going in the forums and saying blah blah and blah with all these shill accounts or paid pumpers. Until their accountant gave me a salacious  video and I had some proof (by hacking them) thru google and url search operators to mine their website (yes they didn't have a smart robot.txt crawler blocker...lol)  that they were shipping medication without medical records... they wouldn't give me back my money. I beat them all.... the whole ring later got arrested for dealing meds without Rx not before paying me my money. I literally had to do the worst things. It was awful... probably gave me some PTSD. That is why I just now stick to my day job... play with my computers and ride my skateboards...lol.

So when I see @Cobber and @trampa and @koralle it gives me flashbacks right way.

Think what they did with VESC.... rather than organically build love for it...they sought to buy its name and hijack us all to pay them their price gouging.  Like they are the law, the lord and the king... and off with our heads if we don't kneel. By "buying" Vedder they thought they bought the business. But technology doesn't work like that... money will flow to remove the middle man.  It's harder and harder to create 17-year long patents that create monopolies. Tech is poised to prevent that mostly.

Suffice to say... I am old and I been around.... I look young but it hurts every time I fall now... best to not go quietly I guess ;)
```

---
## \#102 Posted by: JohnnyMeduse Posted at: 2017-12-09T17:33:28.121Z Reads: 128

```
If you guy wonder what the origin of the VESC is, here is the link to the original thread in endless-sphere : https://endless-sphere.com/forums/viewtopic.php?f=35&t=63540&hilit=vesc

Fun Fact:. 
1- The name VESC wasn't use by Vedder until version 4.6. 
2- All the Master builder from this forum look like noobs. 
3- @psychotiller think that a 200$ esc is not that bad, and was buying stuff from @torqueboards ....
```

---
## \#103 Posted by: banjaxxed Posted at: 2017-12-09T18:23:05.755Z Reads: 128

```
To play devils advocate here the whole OS could have been locked up as proprietry code by now and ohlins & focboxes et al left on vesc 4.10 firmware, instead the vesc supports all the non-VESC clones, in saying that the VESC tool from vedder did eat a new focbox doing motor detection the other day, maybe it has the wrong MAC address 😂
```

---
## \#104 Posted by: mmaner Posted at: 2017-12-09T18:25:05.364Z Reads: 129

```
It would actually be better if the firmware and software was proprietary.  Then there would be more people coming out with alternative firmware and software and the VESC (tm) would disappear leaving a better ESC for skateboards in the market.
```

---
## \#105 Posted by: psychotiller Posted at: 2017-12-09T18:26:05.903Z Reads: 130

```
I was comparing price from the castle 8s escs I was using at the time...not sure what your point is about me buying stuff from Torque.
```

---
## \#106 Posted by: JohnnyMeduse Posted at: 2017-12-09T18:29:18.662Z Reads: 132

```
There wasn't any kind of point.... But since @longhairedboy wasn't around at that time, I couldn't found any good mom  joke, so that the second best I could find :sweat_smile: :sweat:
```

---
## \#107 Posted by: trampa Posted at: 2017-12-09T19:10:41.848Z Reads: 130

```
It will always be like that, since the code is GPLed. 
In consequence derived works also need to be GPLed and available to the public. This will be handled without compromise. 
And as some may have seen, the mobile versions are currently coded, so that APPs can be written that can interact with the Hardware seamless. 

I think that the FOCBOX is the best proof that a TM is no hurdle to sell hardware, especially not after applying very relaxed TM policies, derived from the Linux policies. 

Code is open, hardware will follow soon, fair use of TM is granted.

I have the feeling some people look to deep into a given horses maul. 

Frank
```

---
## \#108 Posted by: Bensaida Posted at: 2017-12-09T19:14:08.064Z Reads: 128

```
No matter what you say, youre just digging your own hole. Dont be surprised when you have a low low amount of sales..
```

---
## \#109 Posted by: rene Posted at: 2017-12-09T20:08:51.171Z Reads: 128

```
like there was so much competition before as everybody was using hobbyking/maytech etc. rc type of ESCs?
```

---
## \#110 Posted by: mmaner Posted at: 2017-12-09T20:52:42.320Z Reads: 126

```
No, it's different now. You got people like @Ackmaniac and @evoheyax that have developed software and 3rd party firmware for the VESC that were kinda tossed aside when Trampa came on the scene. 

There are tons others but I don't wanna do a population study. I want to show that there other people that have made contributions that could make more if given the opportunity and a chance if reward. 

This group/hobby/subculture (whatever) is so much more now than it was a year ago and massively more than it was just 2 years ago. My feeling is that Trampa is trying to cash in on that by stifling advancement for sake of profit. That bothers me a great deal, I don't like being used and manipulated especially for profit.

More importantly it's  bad for users, developers and manufacturers and vendors.
```

---
## \#111 Posted by: rene Posted at: 2017-12-09T21:43:40.740Z Reads: 125

```
I am still new to this scene.

But to get it right - Trampa has only secured the brand for B.V. - the code and hardware design will still be OS.

Production of hardware is not easy as we see with all those esk8 boards from China. 
There is lots of possibility to fail, do a costly mistake - having to garantee to customer etc. or payback.

Now Trampa sells the VESC V6 more expensive than other v4 hardware manufactures - which nearly all are copy cats with slightly improved designs. But as I understood Vedder wants to stay OS and also publish the v6 hardware design, or he maybe has already.

Right?

So its the same as Mozilla or better the Linux kernel lead by this other "nice humble" guy from Finnland.

And if the v6 hardware designs are also becoming OS - than there are options for like a focbox v2 (vesc v6 based) etc.

I understood that it was a surprise as Trampa secured the brand and all other manufactures had to change their product name.

But on the other side - was that not a great way to distinguish their products from crappy china copies using the same name by setting up their own product name? Like ENERTION with his nice focbox? 

And now to your point of having more great developers in the scene like @Ackmaniac or @evoheyax.
Would they have designed a ESC all alone? 
They are now able to contribute, because there was a code base already present. 
So everybody here is becoming a giant standing on shoulders of others.

If there are complains about Mr. Vedder not pulling their code changes, than for my understanding its Mr. Vedders "fault" like Linus Torvalds, who is pissing off so many kernel developers.

This is why I am so confused about all the emotions arising here on this thread / topic.

Only this morning I got aware of the other firmware beeing around made by @Ackmaniac -  that one sounds just awesome!

So why is B.V. "blocking" such a contributor to the overall project?

You wrote "3rd party firmware for the VESC that were kinda tossed aside when..." 
What do I need to read to understand - if I am wrong in my impression / view of reading this forum for 3 weeks now?

Cheers from Hamburg/Germany
```

---
## \#112 Posted by: mmaner Posted at: 2017-12-09T22:03:57.284Z Reads: 126

```
[quote="rene, post:111, topic:40375"]
Trampa has only secured the brand for B.V. - the code and hardware design will still be OS.
[/quote]

And all the implications that contains.  The main ones being that all the other VESC vendors had to spend time and money to change the name and PCB characteristics to comply with, and lets be clear, Frank at Trampa's, demands.  BV hasn't made these demands, Frank has either on his own or with BV's blessing (who knows).  

[quote="rene, post:111, topic:40375"]
Production of hardware is not easy as we see with all those esk8 boards from China.
[/quote]

Absolutely correct, but if think the designs cant be duplicated in China then you need to read more about what has happened with Maytech and some of the other manufacturers and their total disregard for copyrights.  Al this TM of Trampas has done is make more difficult for vendors outside of China.

[quote="rene, post:111, topic:40375"]
Now Trampa sells the VESC V6 more expensive than other v4 hardware manufactures - which nearly all are copy cats with slightly improved designs. But as I understood Vedder wants to stay OS and also publish the v6 hardware design, or he maybe has already.
[/quote]

At 3 or 4 times the cost of manufacturing, that's called price gouging.  The current assumption is that it will stay OS and the hardware designs will be published but to this point they have not.  There are some copies floating around of the V6 hardware design but BV nor Trampa have actually released them for others to manufacture, at least that's my understanding.

[quote="rene, post:111, topic:40375"]
there are options for like a focbox v2 (vesc v6 based) etc.
[/quote]

These used to be called a VESC, Frank locked that down.  WIth his recent history I honestly expect him to attempt to block the manufacture of V4 designs as well.

[quote="rene, post:111, topic:40375"]
was that not a great way to distinguish their products from crappy china copies using the same name by setting up their own product name? Like ENERTION with his nice focbox?
[/quote]

Maybe, maybe not.  What it has secured is the death of the VESC.  This is the beginning of the end.  The end result will be BV not making any money, Frank having screwed the entire community for profit and then loosing his ass.  Its just bad decision making all around.

[quote="rene, post:111, topic:40375"]
And now to your point of having more great developers in the scene like @Ackmaniac or @evoheyax.
Would they have designed a ESC all alone?
[/quote]

Once again...maybe, maybe not.  We will never know because Frank and BV have essentially ignored them while coopting their designs into the new V6 firmware.

[quote="rene, post:111, topic:40375"]
Only this morning I got aware of the other firmware beeing around made by @Ackmaniac -  that one sounds just awesome!
[/quote]

It is, works flawlessly and props to @Ackmaniac for making a mediocre product badass. 

[quote="rene, post:111, topic:40375"]
You wrote "3rd party firmware for the VESC that were kinda tossed aside when..." 
What do I need to read to understand - if I am wrong in my impression / view of reading this forum for 3 weeks now?
[/quote]

Dude, I don't even know where to start.  Search for topics that contain keywords like VESC6, Frank, Trampa, Trademark, Copyright, etc.

Let me be clear on this.  My issue is that I simply cannot watch profit mongering and the theft of ideas and not say anything.  I grew up in  small business home, my dad had a shoe store for 38 years.  My mom ran a arts and craft store.  Companies like Wal-Mart and Costco have made small businesses a thing of the past, other than service related businesses, by using hostile buying and selling practices, straight up extortion and lawyering up to cost people massive legal fees if they choose t fight...exactly what Frank is doing.
```

---
## \#113 Posted by: rene Posted at: 2017-12-09T23:53:57.211Z Reads: 122

```
Thanks @mmaner for taking the time to answer a newbee in such a detail.

[quote="mmaner, post:112, topic:40375"]
Let me be clear on this.  My issue is that I simply cannot watch profit mongering and the theft of ideas and not say anything.  I grew up in  small business home, my dad had a shoe store for 38 years.  My mom ran a arts and craft store.  Companies like Wal-Mart and Costco have made small businesses a thing of the past, other than service related businesses, by using hostile buying and selling practices, straight up extortion and lawyering up to cost people massive legal fees if they choose t fight...exactly what Frank is doing.
[/quote]

Well, I feel you - as beeing a business owner myself  who failed big in 2001 as the "New Economy" blew up.
Became millionaire on paper and 16 months later went bankrupt with a real dept of EUR -500.000 at the age of 28.

And I am still fighting my way back with my new business - where the big guys (Deutsche Telekom) like to copy me ideas and others did 100% copy cats of my product even incl. my text mispelling on their website.

But to get back to the topic.

[quote="mmaner, post:112, topic:40375"]
 >Trampa has only secured the brand for B.V. - the code and hardware design will still be OS.

And all the implications that contains.  The main ones being that all the other VESC vendors had to spend time and money to change the name and PCB characteristics to comply with, and lets be clear, Frank at Trampa's, demands.  BV hasn't made these demands, Frank has either on his own or with BV's blessing (who knows).  
[/quote]

OK - there was effort to be done. 
Let's be honest here - finding a new product name and change it on a website is not a big deal.
The two VESCs v4.12 I bought from Faraday here in germany two weeks ago do look as do the ones from maytech etc.

If I understood correctly lots of people are unhappy with the v4 hardware design as it like to blow up.
Those DRVs, the black chips, dont like ampere. I read a post from @onloop that this design had to change and he took the challenge.
I got so scared while reading all those blew up posts  that I ordered two focboxes from France and another two from ENERTION directly in that black whatevery sale.

So everybody was complaining - to me it looks like Trampa got the message transported to B.V. to improve and that they were willing to support him. I guess with time and money for the development of v6 (what happpend to v5 btw?)
I just bought the €20 Version of the VESC-Tool via PayPal and was happy to see that the money went directly to B.V.
And my order number is 1341 - so let me do the simple math 1341 x EUR 26.820 for B.V. if all bought at EUR 20
for working for two years. 

He lives in Sweden - and thats much more expensive as Germany. 

Dunno how he survives - but Vesc-Tools sales cant be it.


[quote="mmaner, post:112, topic:40375"]
At 3 or 4 times the cost of manufacturing, that's called price gouging.  The current assumption is that it will stay OS and the hardware designs will be published but to this point they have not.  There are some copies floating around of the V6 hardware design but BV nor Trampa have actually released them for others to manufacture, at least that's my understanding.
[/quote]

Sure that VESC v6 price is no bargain compared to ca. EUR140 I paid for each FocBox from the certified importer from France.
But someone had to pay the development of the new v6 hardware and this Vesc-Tool - somewhere I read about two years did it took B.V..

Than you got a design - need to start production in maybe 500 pcs. to start with. 
All money up front - but I am sure there where lots of mistakes in the first revision, and the second etc. 
Thats all money out of the window, as we call it here in germany.
Trampa is in the UK - its f**king expensive over there - and they are still in the EU.
Let's cut this down - all that add's up. 

And a lot of people here in the forum report that B.V. did not got lots of bonuses from other manufactures.

[quote="mmaner, post:112, topic:40375"]
>there are options for like a focbox v2 (vesc v6 based) etc.

These used to be called a VESC, Frank locked that down.  WIth his recent history I honestly expect him to attempt to block the manufacture of V4 designs as well.
[/quote]

Thats a feeling, an emotion. Emotions are great while in bed with our girls. 
But I did not came across of messages of Frank stateing this.

[quote="mmaner, post:112, topic:40375"]
>was that not a great way to distinguish their products from crappy china copies using the same name by setting up their own product name? Like ENERTION with his nice focbox?

Maybe, maybe not.  What it has secured is the death of the VESC.  This is the beginning of the end.  The end result will be BV not making any money, Frank having screwed the entire community for profit and then loosing his ass.  Its just bad decision making all around.
[/quote]

Death of the VESC - why?
Focbox sold awesome, more than 500 orders did ENERTION get on that BlackWTF thing weekend.
I will be waiting weeks until my Focboxes arrive in germany plus customs.

Still if B.V. does not close the project to private source - all stays the same. 
Even if he does - the source is public - it stays public.
The Vesc-Tools SRC must be still public otherwise how should @Ackmaniac develop his version of the tool.

Bad decisions? 
Because Trampa seems to kinda help B.V. to manage himself? 
That Frank always talks about contributing - and all code is freely around.
The VESC has its TM and is save against Chinas-copy-cats incl. bad quality.

Upstairs in my browser there is an ad from @onloop "Certified FOCBOX Suppliers" .
Why do the other manufactures do "certify" their VESC at B.V. - so they all stay together.
Like all the Linux Distos etc. do. 
That would make all stronger. 

[quote="mmaner, post:112, topic:40375"]
>And now to your point of having more great developers in the scene like @Ackmaniac or @evoheyax.
Would they have designed a ESC all alone?

Once again...maybe, maybe not.  We will never know because Frank and BV have essentially ignored them while coopting their designs into the new V6 firmware.
[/quote]

But the new V6 firmware is also free to everybody, even those first alternative v6 designs - I think I saw that firemware in the Vesc-Tool I downloaded - hardware version 60 i guess. 
So until there is the focbox v2 (aka vesc6) I will try @Ackmaniac firmware for my FocBox. 

To get to an end, we got the 10th here in germany already 0:35 o'clock.

To me it sounds like "feeling hurt" - thats OK!
But why not wait and see how B.V.  will drive the future.

Thats all like in the Linux world when systemd came around. etc. etc. 
Normal OS wars - but nobody dieds. 

Even @onloop wrote somewhere that he is f**king happy not to be DIY anymore - so ENERTION came from DIY grew up - got lots of hard knocks / shitstorm from the community - but that guys does stay up again and rides the chines lion and made an awesome Raptor 2.

Lets hope he cashes in a lot $$$, so he has funding for the Raptor 3 and can provide for his family forever.
And we get the focbox v2.

Sorry, that became a long response ... wanted to work on my build ... 


<img src="/uploads/db1493/original/3X/1/5/1550df99d0beabd79b62d94c34db7e43d8e0ace2.jpg" width="666" height="500">

PS: 
See those Vesc's on the left - they got some parts made to high - so they dont fit into that awesome cnc box!
:frowning:
```

---
## \#114 Posted by: Kug3lis Posted at: 2017-12-10T00:01:38.795Z Reads: 116

```
P.S. From technical side vesc6 is not a big difference from vesc4... The changed DRV chip because previous one was discontinued and some minor changes which you can make in a day... I went with own design of board getting rid of DRV and etc and done everything in two evenings so I don't know what kind of work they are talking about. From the software side, nothing much is different between 4 and 6 just some flags in the source code which defines which pin does what and what kind of DRV is used that's all whats done.
```

---
## \#115 Posted by: Kug3lis Posted at: 2017-12-10T00:03:44.692Z Reads: 114

```
Hardware is completely generic all ESC looks the same just different components which does the same thing. The whole thing is just software which idea was ripped from existing algorithm from big giants... 

I hate that now they want to monopolize "they" invention which is just thrown a bunch of things together as 2 years developed project...
```

---
## \#116 Posted by: Kug3lis Posted at: 2017-12-10T00:05:41.374Z Reads: 114

```
Also, the whole control algorithm is just converted math formulas to code that's all it's done.
```

---
## \#117 Posted by: Kug3lis Posted at: 2017-12-10T00:06:54.518Z Reads: 114

```
You can pick TI microprocessor, take TI InstaSpin library define some inputs outputs and damn you have the same FOC running.
```

---
## \#118 Posted by: Kug3lis Posted at: 2017-12-10T00:07:36.012Z Reads: 111

```
Here you go reference design for the same stm32 http://www.st.com/en/embedded-software/stsw-stm32100.html
```

---
## \#119 Posted by: mmaner Posted at: 2017-12-10T00:11:35.468Z Reads: 115

```
I'm just gonna hit the high points, about to go to dinner. 

[quote="rene, post:113, topic:40375"]
Thats a feeling, an emotion.
[/quote]

No sir, that's a guess.  An educated guess based on past behavior. Big difference. 

[quote="rene, post:113, topic:40375"]
Death of the VESC - why?
Focbox sold awesome, more than 500 orders
[/quote]

That's my point. Understand the FocBox is not a VESC.  @onloop was forced to change the name, as we're countless others. In fact, there is no VESC 4 in production. That's because if Frank. [quote="rene, post:113, topic:40375"]
Even if he does - the source is public - it stays public
[/quote]

The VESC 4 is public, the VESC 6 absolutely is not. 

[quote="rene, post:113, topic:40375"]
Bad decisions? 
Because Trampa seems to kinda help B.V. to manage himself?
[/quote]

That's pretty naive, you think Frank is only helping BV and not himself?

[quote="rene, post:113, topic:40375"]
To me it sounds like "feeling hurt" - thats OK!
But why not wait and see how B.V.  will drive the future.
[/quote]

It's not hurt, it's anger and disgust. What Frank has done is underhanded and driven by profit. Ben has taken features he never used before from 3rd party developers and incorporated then into the VESC 6 without so much as a thank you and then ignores their continued  contributions.  

I hope you see past the curtain on this...
```

---
## \#120 Posted by: mmaner Posted at: 2017-12-10T00:24:17.800Z Reads: 113

```
You should develop it, like I said PM me and we can figure out how to get you funded.
```

---
## \#121 Posted by: gogomrrobot Posted at: 2017-12-10T00:38:51.320Z Reads: 112

```
[quote="mmaner, post:120, topic:40375, full:true"]
You should develop it, like I said PM me and we can figure out how to get you funded.
[/quote]

i want in💰... puwease!
```

---
## \#122 Posted by: Nemesis Posted at: 2017-12-10T01:13:26.056Z Reads: 114

```
Epic thread....  i have no idea whats going on but, i actually felt a breeze from all the ball swinging, and then heard a wallop when @Kug3lis unfurled the mighty whang of knowledge. :blush:
```

---
## \#123 Posted by: Cobber Posted at: 2017-12-10T03:25:51.438Z Reads: 115

```
you should go back and read our conversations chaka, only one of us was slagging people off...

and mrrobot I think your tinfoil hat is too tight.

& As per the previous thread you started that has been deleted by admin where you made similar wild accusations directed towards me. You can not say in public that a business is price gouging as it is a legally defined term that describes illegal activity, such statements amount to liable and you will end up getting this thread closed and deleted like the last.
```

---
## \#124 Posted by: mmaner Posted at: 2017-12-10T03:57:37.950Z Reads: 115

```
[quote="Cobber, post:123, topic:40375"]
You can not say in public that a business is price gouging as it is a legally defined term that describes illegal activity, such statements amount to liable and you will end up getting this thread closed and deleted like the last.
[/quote]

That's the problem right there, both you and Frank think you can tell people what they can and cannot do by being a bully.  

Let me be the first to tell you...I live in America, I WILL say any damn thing I want to say.

You want to throw lawyers at it, go for it.  I bet I have access to more lawyers than you do considering the legal team i work with, the 2 I have on retainer for my dad's estate and the 1 I graduated college with who was at my wedding.
```

---
## \#126 Posted by: anorak234 Posted at: 2017-12-10T04:07:11.861Z Reads: 118

```
@mmaner @Cobber

Both of you cool it - yes, accusations have been made, but nothing came of it so let’s learn to ignore speech that isn’t helpful or positive.

Also, just because America is a land of free speech doesn’t mean that speech doesn’t have consequences in a social context.

 - I’m leaving @mmaner’s statement here because the flag was unnecessary but the language needs to be toned down.
```

---
## \#127 Posted by: gogomrrobot Posted at: 2017-12-10T04:07:55.376Z Reads: 114

```
Then what's your horse in this matter? Why all the passion lubber? Are you just `Late Night Frank` following all day Frank ;)

Besos
```

---
## \#128 Posted by: Deckoz Posted at: 2017-12-10T04:10:11.530Z Reads: 121

```
Thus thread is um..haha

-VESCTool is open source and available.
-VESC6.4 is OS, all you need is the schematic which is publicly available
-"VESC" is trademarked by trampa
-the hardware called "VESC6" by Trampa is not open source, like most hardware. Not every OS project provides Gerber's for pre-laid out hardware.

-speaking of open source actions like these such as TM and OS arguments. Is just asking for a fork. 

If you want to build VESC6's go get the schematic, design a board and stop complaining. You have everything you need publicly available. Don't expect every open source project to hold your hand and give you everything on a silver platter. Most OS projects just include schematics and no Gerber's as it forces people to design boards to fit their application.

Y'all. Wow..I can't even.

Better yet since y'all are helpless
http://vedder.se/forums/download/file.php?id=438&sid=42ec26f837a5c4e99e0badf82f78c272

The schematic has been available over a year...lol
```

---
## \#129 Posted by: mmaner Posted at: 2017-12-10T04:21:40.770Z Reads: 119

```
You are correct, my bad. Won't happen again.  I just get really passionate about seeing people taken advantage of is all. 

My apologies @Cobber, should have been so vocal. I still think you are wrong...really, really wrong...but I should have been more adult in my response.
```

---
## \#130 Posted by: ATLesk8 Posted at: 2017-12-10T04:54:15.047Z Reads: 120

```
I just want to let you know it's spelled libel...not liable
```

---
## \#131 Posted by: onepunchboard Posted at: 2017-12-10T04:56:40.198Z Reads: 122

```
you know, it all sounds like pharmacy industry.
everyone knows, the drugs are nt that expensive, developed by thousands of people. but only a company hold the right to fk everyone with over price. 
it's business and legal. However, it is simply wrong.
vesc6 is not essential to live, yet it is heart of esk8.
yes it is OS but that doesnt mean everyone has skill set equipment to make one
```

---
## \#133 Posted by: Deckoz Posted at: 2017-12-10T05:48:07.733Z Reads: 120

```
<img src="/uploads/db1493/original/3X/7/e/7eb6c6b9b1671f9e91460a6acc704fe74807b391.jpg" width="625" height="268">
```

---
## \#135 Posted by: Deckoz Posted at: 2017-12-10T05:52:09.337Z Reads: 121

```
@trampa... On a serious note since no one cares about the VESC6 you sell.

Where the Gummies at?
```

---
## \#136 Posted by: b264 Posted at: 2017-12-10T06:00:38.138Z Reads: 123

```
<img src="/uploads/db1493/original/3X/b/5/b567113ff022363c7ec8338fb4669c96be8465fb.jpg" width="500" height="500">
```

---
## \#138 Posted by: trampa Posted at: 2017-12-10T12:04:43.553Z Reads: 125

```
New Gummies molds are currently in the make. 
Not for Christmas... Sorry.

Would love to see people staying on topic. 
The topic is software and hardware and GPL.
rights and obligations. 

It is about the matter in general.
I'm amazed how fast things went off topic.

Frank
```

---
## \#139 Posted by: Mathias Posted at: 2017-12-11T22:35:05.658Z Reads: 121

```
@rene, you're nailing it. I couldn't agree more. I don't know if you found it already, but BV explained the trademark situation, and how he will continue the VESC project a while ago: 
[http://vedder.se/forums/viewtopic.php?f=6&t=733](http://vedder.se/forums/viewtopic.php?f=6&t=733)
I don't know how it happened, but the public opinion here is that @trampa stole stole something from the community. The reality is that the community still has everything that it had before and more. Except for the the name "Vedder".


[quote="mmaner, post:112, topic:40375"]
and lets be clear, Frank at Trampa's, demands.  BV hasn't made these demands, Frank has either on his own or with BV's blessing (who knows).
[/quote]

@mmaner, come on. Please read [BV's statement](http://vedder.se/forums/viewtopic.php?f=6&t=733) form May this year (yes, May!!). This statement btw also addresses several of your other accusations. Seriously, read it!

[quote="mmaner, post:112, topic:40375"]
And all the implications that contains.  The main ones being that all the other VESC vendors had to spend time and money to change the name and PCB characteristics to comply with
[/quote]
Aren't you being a bit dramatic here? As I recall it @trampa announced it in advance and told everyone that nobody has to throw away PCBs they already got. They could just black out the "VESC" with a marker or just put a sticker on it. The FOCBOX is a perfect example why the trademark is NOT a problem. Enertion could fork the 4.12 and make something better. Everyone pretended that it's gonna be the end of the world if you can't call it VESC-X any more, and look what terrible things have happened: none! The opposite, FOCBOX still benefits from the new firmware developments. And it's great that @Ackmaniac can go ahead and give it his own spin. And (finally something on topic!) it is also great that he is forced by the GPL to publish his changes. That's how it SHOULD work. Everyone benefits from everyone's improvements!

[quote="mmaner, post:112, topic:40375"]
Dude, I don't even know where to start.  Search for topics that contain keywords like VESC6, Frank, Trampa, Trademark, Copyright, etc.
[/quote]

Exactly! It's been chewed on over and over, and people still can't tell project, trademark, source, copyright, and license apart.

Trampa: "GPL has rules attached to it. The're not hard to follow."
This forum: "TRAMPA DIDN'T INVENT THE VESC!!!!"

[quote="Deckoz, post:128, topic:40375"]
Y'all. Wow..I can't even.

Better yet since y'all are helpless
http://vedder.se/forums/download/file.php?id=438&sid=42ec26f837a5c4e99e0badf82f78c272

The schematic has been available over a year...lol
[/quote]

Also this :point_up_2: :point_up_2: all the way!


Nobody forces anyone to deal with trampa if you want to be part of the VESC project. You can contribute, or just copy, modify and sell it. Just follow the law, which was not written by @trampa. He's just telling you the situation, the rules that everyone has to play by, including @trampa and BV. And it's is good that way. If you want to change or adapt, just publish your changes and inform everyone about the license. This way the VESC project can be a healthy OS ecosystem, and this has NOTHING to do with the trademark. So everyone please stop behaving like a baby who's lollipop @trampa stole. You still got it, you just can't call it VLollipop® any more...

Edit: I just realized: Frank isn't @Frank, but @Trampa. Sorry for the hundreds of wrong tags, @Frank! LOL
```

---
## \#140 Posted by: koralle Posted at: 2017-12-11T22:55:03.519Z Reads: 120

```
Thank god there are finally some voices of reason in this hate contest.

So many people completely misunderstand franks whole point.

[quote="mmaner, post:112, topic:40375"]
Companies like Wal-Mart and Costco have made small businesses a thing of the past
[/quote]
This shows that you have not understood in the slightest what Trampa/Frank are all about. They actually are the small business trying to succede and further develop the VESC.

[quote="mmaner, post:129, topic:40375"]
I just get really passionate about seeing people taken advantage of is all.
[/quote]
Who the ? is being taken advantage of here? If anyone, it used to be/ still is BV.
```

---
## \#141 Posted by: mmaner Posted at: 2017-12-12T04:15:10.729Z Reads: 119

```
[quote="Mathias, post:139, topic:40375"]
This statement btw also addresses several of your other accusations. Seriously, read it!
[/quote]

I have, doesn't carry water. 

[quote="Mathias, post:139, topic:40375"]
Aren't you being a bit dramatic here?
[/quote]

Nope.  

[quote="Mathias, post:139, topic:40375"]
This way the VESC project can be a healthy OS ecosystem
[/quote]

It could be, but it's not. It's not because there's a profit hungry asshat driving the car...and a wreck is inevitable.

Honestly, I'm not interested in your 'spin'. You are totally capable of having your own opinion, even if it's the wrong one.
```

---
## \#142 Posted by: mmaner Posted at: 2017-12-12T04:19:12.529Z Reads: 118

```
[quote="koralle, post:140, topic:40375"]
This shows that you have not understood in the slightest what Trampa/Frank are all about.
[/quote]

This shows that you've been drinking the kool-aid (wonder if they will sue me for using their brand name). 

[quote="koralle, post:140, topic:40375"]
They actually are the small business trying to succede and further develop the VESC.
[/quote]

Lol

[quote="koralle, post:140, topic:40375"]
Who the ? is being taken advantage of here? If anyone, it used to be/ still is BV.
[/quote]

Everyone that invested in the VESC's platform, everyone one who developed 3re party software/firmware for the VESC and has their ideas pilfered, everyone who enjoys the VESC platform and is watching it crash in flames from profiteering and terrible marketing.
```

---
## \#143 Posted by: Mathias Posted at: 2017-12-12T06:54:17.306Z Reads: 117

```
[quote="mmaner, post:141, topic:40375"]
I have, doesn't carry water.
[/quote]
I see... 
Fake news!


[quote="mmaner, post:141, topic:40375"]
profit hungry asshat driving the car
[/quote]
[quote="mmaner, post:141, topic:40375"]
You are totally capable of having your own opinion, even if it's the wrong one.
[/quote]

Dude...
[quote="mmaner, post:142, topic:40375"]
Everyone that invested in the VESC's platform, everyone one who developed 3re party software/firmware for the VESC and has their ideas pilfered, everyone who enjoys the VESC platform and is watching it crash in flames from profiteering and terrible marketing.
[/quote]

Since they can't get, use, modify, publish, re-brand, or sell the software, firmware, and hardware any more. 
Wait...
```

---
## \#144 Posted by: akira Posted at: 2017-12-12T08:40:56.247Z Reads: 117

```
Just as a side note, before Trampa came in the game, the HW was also fully open-source. This means that all schematics AND PCB files were released. It is not the case anymore. Trampa say they will release a reference design but this is very far from a HW open-source licence (which would force Trampa to release all files from their VESC design).
```

---
## \#145 Posted by: rene Posted at: 2017-12-12T10:51:22.731Z Reads: 117

```
The schematics are still open source - 
I come to the conclusion, that for us as community it is an adventage that the Vesc-6 PBC layouts are not available - because this will produce new different designs on the market. 

Maybe someone will do a pcb with two VESCs on it - for dual-motor setups. Saving space
```

---
## \#146 Posted by: trampa Posted at: 2017-12-12T11:28:51.553Z Reads: 117

```
@anorak234

Do we need to accept strong language and accusations? Like Asshat, drinking to much Kool-aid etc.
@koralle, are you really a kool-aid addict? 
There is nothing wrong about a good fight with words, as long as everyone behaves and can make their points, using appropriate language. Some stuff here is going way to far in my opinion.

I also don't get the point why it is so hard to stay on topic. 

Frank
```

---
## \#147 Posted by: gogomrrobot Posted at: 2017-12-12T12:28:04.022Z Reads: 115

```
The topic is itself a snooze-fest. Nobody outside of this website cares about the name VESC -- though correctly BV has trademarked the name. Will it hold up in court? idk... and frankly I don't care.

I would like to move forward with a plan. Lets have @Kug3lis, @mmaner and whomever want's in put together a community edition VESC6 -- whatever name we want to call it if it can't be called VESC6 then we will do a poll and pick one or just pick one if the name choices aren't good.

I want to have a trackable serial number ID on each VESC and make sure a specific donation amount goes to BV -- $10 - $15 or something that seems fair like that. I really still don't understand the math though. We don't simply have enough sales to fully support an income for him. Maybe it will get better.

Based on the cost... lets get between 100 to 1000 vesc6's <insert name>. Or do 100 at a time.  Let's get the community edition out there just so there is a community edition. I think I just want a small ROI. I am willing to invest  $10-20k. We should sell this product in the $150-$160 range. Or we can get behind @stewii ESCape. But I think we need to move him off of hand soldering and reflow oven in his own house and move to mass production. 

Let's do something and get on with this already.  The debate is boring and I need more VESC6 <not named that..lol>
```

---
## \#148 Posted by: longhairedboy Posted at: 2017-12-12T13:48:17.099Z Reads: 114

```
i'm done with all this. Who wants to make me a vesc6 pcb with my name on it? 

I'll pay you.
```

---
## \#149 Posted by: Kug3lis Posted at: 2017-12-12T13:52:27.356Z Reads: 114

```
:joy: :joy: :joy: 

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/e/8/e844fe145c8aeefca803e97c4ca035a5e0c51715.png"/>
```

---
## \#150 Posted by: mmaner Posted at: 2017-12-12T13:58:31.623Z Reads: 117

```
[quote="trampa, post:146, topic:40375"]
Do we need to accept strong language and accusations?
[/quote]

1.  If that hurts your feelings, you might not wanna be in a business that involves a bunch of skaters.  Furthermore, that's the nicest thing that you are referred to around here.
2.  They are only accusations until they are proven, which most have been.

[quote="trampa, post:146, topic:40375"]
I also don't get the point why it is so hard to stay on topic.
[/quote]

It is on topic.  The topic is "Open Source Software and Hardware.  Your Rights and Obligations...according to Frank who apparently thinks he rules the World".
```

---
## \#151 Posted by: TarzanHBK Posted at: 2017-12-13T09:42:02.832Z Reads: 115

```
I´m still wondering why noone opened a original Trampa Vesc6, compare it with the open source standard reference stuff and can tell the differences, so that others can use some improvements.
Why is still noone except @stewii doing some production?
```

---
## \#152 Posted by: Okami Posted at: 2017-12-14T18:31:16.521Z Reads: 109

```
I assume there are not enough interested parties to develop.. who knows maybe some are already doing it just not publishing enough?
```

---
## \#153 Posted by: longhairedboy Posted at: 2017-12-14T18:48:54.515Z Reads: 109

```
[quote="TarzanHBK, post:151, topic:40375"]
Why is still noone except @stewii doing some production?
[/quote]

i just bought a small desktop reflow oven. Everything i use is open source and there's no reason i can't pick and place my own shit. I'm starting with very simple things like my vedder/fecter eswitches and then moving up to VESCs and then VESC6 and possibly even try doing a DieBieMS if i get cocky.
```

---
## \#154 Posted by: Okami Posted at: 2017-12-14T19:38:23.558Z Reads: 102

```
Sounds almost like u will need a dedicated guy in your shop doing all of the circuit / pcbs things in future :slight_smile:
 
Or u just plan to be super resourceful with everything :slight_smile:

Anyways thumbs up, we definately need more independent esk8 related product / pcb developers out there :)
```

---

# Topic created by Onloop - Is the Ollin VESC using upgraded components?

### Replies: 97 Views: 6587

## \#1 Posted by: chaka Posted at: 2016-08-23T21:04:16.809Z Reads: 550

```
Topic split from http://www.electric-skateboard.builders/t/blew-up-my-vesc-but-why/7297/32

> Its marketing spin... Hes using all the parts as per vedder bom... unless he has changed the design of the vesc (which he hasnt) he is using the parts we are all using. 

Hey slick, this is one of the many components we have upgraded in our pursuit of a reliable system. I find it very strange that you are trying to slander the quality of our VESC's when you are using them to fix all of your raptors. If you would like to know more about why our VESC's are so robust feel free to inquire on a consultation.

 jclark@ollinboardcompany.com
<img src="/uploads/db1493/original/2X/8/812dbf61563b957bc14c68a34029d0ad3c53f14a.jpg" width="690" height="442">
Special thanks to @JTAG for the original recommendation on this upgrade.
```

---
## \#2 Posted by: sl33py Posted at: 2016-08-23T21:10:38.050Z Reads: 514

```
[quote="chaka, post:37, topic:7297"]
Special thanks to @JTAG for the original recommendation on this upgrade.
[/quote]


Hey @Chaka - you double up this cap at c37 (if i'm reading that right) - what's the result?  I might add this to the one i repair a DRV on (bought used w/ dead DRV already).

Thanks!
```

---
## \#3 Posted by: onloop Posted at: 2016-08-23T23:46:08.493Z Reads: 491

```
[quote="chaka, post:37, topic:7297"]
Hey slick, this is one of the many components we have upgraded
[/quote]

Hey Jerimiah.. don't you think the community deserves to know about your "many components" upgrades &  I am sure that's what Vedder wanted when he made his project open source....???

You know that keeping these mysterious-special-upgrades private you are directly violating the [creative commons license](https://creativecommons.org/licenses/by-sa/4.0/) that the VESC has been released under?

Either prove you have "many" upgrades or tune down the hype, slick.
```

---
## \#4 Posted by: JLabs Posted at: 2016-08-23T23:57:21.531Z Reads: 460

```
[quote="onloop, post:39, topic:7297"]
Either prove you have "many" upgrades or tune down the hype, slick.
[/quote]

You know, I get your job is stressful but there is no need to be rude. Why does someone buy a VESC from @chaka when it is almost double the cost? Because he has built a reputation for having the **best** vesc. He is obviously doing something right whether or not he is upgrading components. He just said one upgrade and told you to email him if you wanted the rest. There are a whole lot less people complaining about his vesc compared to yours. You may sell more but, the service he offers and the upgrades that come pre installed are obviously doing something. So I don't  appreciate you saying it a marketing spin, and bashing him.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-24T00:20:52.441Z Reads: 426

```
[quote="chaka, post:37, topic:7297"]
this is one of the many components we have upgraded in our pursuit of a reliable system
[/quote]

And if @onloop spent a lot of time fixing broken vescs (because chaka had to start with vedders original blueprints for components), you learn about these types of things. This is the problem with outsourcing all of your manufacturing. You become out of touch with the problems in the designs of your parts. I'm sure many of these upgrades, chaka has found out because he has to fix them when they brake. Going back through, you can figure out the root cuase of the failure. When @onloop s break, its a paper weight, or trashed, there's no repair service, because you don't have the tools or time to do it. Since you don't fix them, you just see a dvr failure for example from what someones post on here, and not the root that cause the dvr failure (like c37 failing). And these little fixes that make the vesc more robust don't go into your vescs. And then they keep braking, and you blame your customers for it.

Not all vescs are the same and chaka just showed one example of why.

[quote="chaka, post:37, topic:7297"]
I find it very strange that you are trying to slander the quality of our VESC's when you are using them to fix all of your raptors
[/quote]

Are you saying he's not using his own, but your vescs in some raptors?
```

---
## \#6 Posted by: furryfrog Posted at: 2016-08-24T00:52:14.124Z Reads: 387

```
Onloop is right, any changes to the VESC need to be documented for the community. According to the picture there has been a change to chaka's VESC bom, Where is this modified bom posted? Was it distributed here or perhaps on Vedders Site?
```

---
## \#7 Posted by: DougM Posted at: 2016-08-24T00:56:46.949Z Reads: 386

```
Back on target for a second, I want to offer another alternative possible scenario...

Tantalum caps really shouldn't be used as power filter caps.  they are sensitive to small voltage spikes and tend to thermally runaway.

I have had exactly the same event completely destroy one of my VESC's and I always trim the pins below the red power wire.  I have also had catastrophic failures in other devices that use tants.  I do not use them anymore for power filtering or decoupling.  In fact I don't use them at all.

It would be a really good idea for Vedder to design tants completely out of the next rev of VESC.

There's a great discussion [here](http://electronics.stackexchange.com/questions/99320/are-tantalum-capacitors-safe-for-use-in-new-designs)

DougM
```

---
## \#8 Posted by: onloop Posted at: 2016-08-24T01:17:25.142Z Reads: 373

```
[quote="evoheyax, post:41, topic:7297"]
You become out of touch with the problems in the designs of your parts. I'm sure many of these upgrades, chaka has found out because he has to fix them when they brake.
[/quote]

I didn't design the VESC, nor did Chaka, it's an open source project designed by Benjamin Vedder. The BOM & Gerber files are provided by the designer and the end result is a VESC.... 

If Chaka has identified problems with the VESC design & changed the Gerber files or the BOM components to improve the reliability of the VESC he should [submit a pull request](https://github.com/vedderb/bldc-hardware) & make it public so that Vedder & the rest of the community can benefit.

If he hasn't made "many changes" to improve the VESC he should not use language that suggests he has...
```

---
## \#9 Posted by: onloop Posted at: 2016-08-24T01:31:24.723Z Reads: 370

```
[quote="chaka, post:1, topic:8212"]
I find it very strange that you are trying to slander the quality of our VESC's when you are using them to fix all of your raptors.
[/quote]

I think your VESC are great.....

However, I think your marketing spin is starting to get the better of you. This statement above is a perfect example, why would we buy your VESC to fix our raptors when we are producing a few hundreds VESC each week in a factory in Texas? I have never authorised a single VESC to be used in our raptors.

If my customers want to pay you a premium instead of have a VESC replaced under warranty for free that is their call.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-08-24T01:35:41.114Z Reads: 354

```
[quote="onloop, post:44, topic:7297"]
I didn't design the VESC, nor did Chaka, it's an open source project designed by Benjamin Vedder.
[/quote]

I know that neither of you created it, it was Benjamin Vedder, but my point is that its hard for you to offer upgrades to the community of the vesc if you don't physically repair them when customers report problems. Being probabky the largest supplier, you have the biggest oppurtunity to find these problems. But you can't find these little things if you don't fix them and trace back the problems. It's though because the laws are clear with this case, but I think chaka deserves to profit from his improvements, just like vedder deserves to profit from designing and engineering the vesc. While the laws seem clear, it seems like you want to piggy back on his work, and haven't put anything like the effort chaka has into improving the vesc, just making and profiting from other peoples work.
```

---
## \#11 Posted by: Ulfberht Posted at: 2016-08-24T01:37:15.908Z Reads: 346

```
Upgrading components isn't necessarily a "design change", but they are mods that make the VESC perform better. You can split hairs and quote opensource rules all day long, but at the end of the day Ollinboardco is reigning as the number one supplier of VESC with the best warranty in the industry, while you are trying to sell VESC with known problems( ie. pins causing shorts) Don't be so jealous and take shots at Chaka, just up your game. No one wants you to fail, but you have to prove it...Chaka proves that shit every day. That's not hype, just common knowledge. :v:
```

---
## \#12 Posted by: onloop Posted at: 2016-08-24T01:46:59.973Z Reads: 343

```
[quote="Ulfberht, post:11, topic:8212"]
That's not hype, just common knowledge. :v:
[/quote]

if he has actually upgraded "many components" and he proves that then it will be common knowledge, if he hasn't it just means you guys are being fooled by marketing hype.

[quote="Ulfberht, post:11, topic:8212"]
VESC with the best warranty in the industry,
[/quote]

I think his repair service is fantastic, I applaud him for that.

However there is nothing written about any warranty, maybe you can link the community to the written terms & conditions that clearly state what this warranty covers? I doubt it covers user error.
```

---
## \#13 Posted by: Ulfberht Posted at: 2016-08-24T01:50:14.666Z Reads: 340

```
http://www.ollinboardcompany.com/product/vedder-s-speed-controller
"12 Month factory service warranty" You have to scroll down to see it, but it's in black and white.
```

---
## \#14 Posted by: evoheyax Posted at: 2016-08-24T01:56:05.423Z Reads: 336

```
[quote="onloop, post:12, topic:8212"]
I doubt it covers user error.
[/quote]


He has stated in emails to me that if I clearly doing something to break it, he will at worst charge you for parts and shipping. He said he hasn't had that happen yet actually. He doesn't blame his customers for breaking them unless it's blatant. It's hard to tell if a customer broke it being negligent or their was something else that broke it, like a faulty part or capacitor that needed beefing up.

There's not a single person yet to complain on this forum he refused to fix their vesc. And by his wait times and his pictures, it seems like hes pushing out quite a few vescs these days.

So yes, he does fix user errors, maybe at a slight price, but you don't offer that. And since it's difficult to split user error vs. a defect, he has on the defect side every time so far, even though the odds are some of them were user error.
```

---
## \#15 Posted by: guyguy Posted at: 2016-08-24T03:53:20.984Z Reads: 322

```
The creative commons license is a copyright license. It's not a patent or other form of IP protection. Very generally, copyrights protect rights associated with authorship and patents protect rights associated with inventions. 

You're right that the CC license does require him to indicate changes were made but only if he's producing a work that is subject copyright (something written, in a fixed medium). For example, if he published an updated schematic as his own without updating others via github or giving Vedder credit that would probably violate the CC license. To differentiate, this is not like a patent where you can prevent someone from using or modifying your methodology. If he's just updating his manufacturing process and not publishing anything he's free to do so - the copyright isn't relevant to the situation.
```

---
## \#16 Posted by: Pablo_702 Posted at: 2016-08-24T05:43:20.940Z Reads: 312

```
[quote="onloop, post:9, topic:8212"]
However, I think your marketing spin is starting to get the better of you.
[/quote]
Hahahaha this is comical 

"If my customers want to pay you a premium instead of have a VESC replaced under warranty for free that is their call" this should tell you something, jason i really like your products but i truly believe you are your worst enemy
```

---
## \#17 Posted by: Svenska Posted at: 2016-08-24T06:01:48.369Z Reads: 314

```
@chaka

I'd be interested to know what you changed/upgraded in the VESC too. I built a few myself and if you found ways for more reliability it would be sweet to have that documented somewhere. 

Without wanting to bang on the whole you violate the license thing, maybe think about the time and work Benjamin has put into it over the last years and given it to all of us for free. You are able to take it and make some money from it. Wouldn't it be nice to give back to him a little, for his education/development? Would you treat a friend of yours like that?
I guess you see where I'm going with that... Just be a decent person as you already proof you are with your reliable products and outstanding service.

Thanks, Svenska
```

---
## \#18 Posted by: onloop Posted at: 2016-08-24T10:43:38.475Z Reads: 309

```
[quote="guyguy, post:15, topic:8212"]
If he's just updating his manufacturing process and not publishing anything he's free to do so - the copyright isn't relevant to the situation.
[/quote]

The truth is, I really hope he is somehow making an improved VESC! Congratulations should be given.

This entire forum is based on pushing the envelope with constant innovations & it doesn't bother me whether he has done an official pull request or not...  at the end of the day everyone's goal is to make better esk8's & if his knowledge allows that it should be shared for the common good of the community.

But if it's true that knowledge is being held back from the community (&Vedder) that may somehow improve the VESC or make it more reliable, that would be a shame.

So please chaka, if you are going to say your VESC has "many upgrades" over a normal VESC BOM at least list what they are for the betterment of the community........
```

---
## \#20 Posted by: Heavy1 Posted at: 2016-08-24T11:32:38.160Z Reads: 309

```
Such a good topic, I guess my opinion is still torn. 

The community is all about paying it forward.

However, the community is also full of profitable businesses. This marketing/reality of product improvement is an edge for Chaka's business. But it would appear that contributing this information openly would indeed be detrimental to Chaka's business but overall benefit the community. 

I don't think it is fare to pressure Chaka to "do the right thing" by the community if it means he would be disadvantaging himself.

Should we then be pushing all vendors to openly share every improvement or tweak made to products? Outrunner motors, hub motors for example.
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-08-24T11:46:04.465Z Reads: 307

```
https://www.instagram.com/p/BJT1lxLByDj/?taken-by=longhairedboy

Can't we all just get along?
```

---
## \#22 Posted by: Svenska Posted at: 2016-08-24T11:49:18.757Z Reads: 301

```
@Heavy1

Yes, push all vendors to do the right thing and stay with the open source spirit if they are using/selling open source projects.
If it is their own development not based on an open source project they are welcome to do whatever.
```

---
## \#23 Posted by: Cptanpanic Posted at: 2016-08-24T11:50:09.535Z Reads: 297

```
Exactly, that is the purpose of Creative commons license.
```

---
## \#24 Posted by: mason Posted at: 2016-08-24T11:57:43.104Z Reads: 297

```
@torqueboards have y'all made any improvements we should know about?
```

---
## \#25 Posted by: Heavy1 Posted at: 2016-08-24T12:31:26.716Z Reads: 293

```
Can't really fault you on that 👍🏻
```

---
## \#26 Posted by: michichopf Posted at: 2016-08-24T13:00:53.498Z Reads: 301

```
Im not an expert when it comes to a Vesc but have some history with creative commons license.
It is not essentialy needed of you to openly advert every change you made. Only the changes that increased stability, power or anything that is measurable. If we run the same current through both vescs (ollin & Enertion) the same thing happens. If we hoock it up to the computer we see the same thing. As long as its not a mecanical difference or a measurable permofance enhacement its fair play. As long as its minor improvements (you could even call it your style or your preference).

Let me put it this way. If you use the exact same components but you are more carefull with its placement, the pins, double up on safety, its basically improved ye but not by design but by effort which is totally ok.
```

---
## \#27 Posted by: chaka Posted at: 2016-08-24T13:58:22.656Z Reads: 301

```
Every change I have made has been relayed to Benjamin. He has chosen not to update the BOM due to the higher cost of the parts we use. Does anyone honestly believe Jason is going to spend more money on components when he wont even pay for a few extra jst ports?  

What did we change? We use higher rated capacitors, better manufacturing processes and the VESC's are built by people who actually care about and are involved in the sport. The VESC is a wonderful piece of engineering and we given thousands of euros to Vedder to help him in his development. We also encourage others to send him small tokens of appreciation.

Jason on the other hand has done his best to give Vedder and the Vesc a bad reputation with his poor manufacturing and business practices. He has even gone as far as bad mouthing the VESC when things are not working out for him.

<img src="/uploads/db1493/original/2X/a/afd49500c04eb9d1584b6ada05446b103c49440b.png" width="690" height="326">
> enertionboards Actually the vesc design kinda sux.... there is no easy way to manufacture this...so stay tuned for our soon to be released custom vesc without the bulk cap board.

This creative commons argument continues to come up but nobody seems to remember the dual VESC design @onloop failed to launch. If he cares so much about the open source community he would have uploaded the gerber files.

When I updated Vedder/Fetcher anti-spark switch and made it usable for heavy current did I keep it to myself? No, I shared my OshPark files so others could simply order the pcb's. 
<a href="https://oshpark.com/shared_projects/XuqJkZzU"><img src="https://oshpark.com/assets/badge-5b7ec47045b78aef6eb9d83b3bac6b1920de805e9a0c227658eac6e19a045b9c.png" alt="Order from OSH Park"></img></a>


Please remember this all stems from @onloop lashing out at others when the quality of his VESC's were under attack. He was shown proof that we do indeed use higher rated components and he chose to change course and continue to lash out instead of apologizing for his slanderous behavior. And now his very own repair agent is showing proof that they are using our VESC's to perform repairs on raptors...
```

---
## \#28 Posted by: Svenska Posted at: 2016-08-24T14:12:41.369Z Reads: 293

```
@chaka 

[quote="chaka, post:27, topic:8212"]
Every change I have made has been relayed to Benjamin.
[/quote]

[quote="chaka, post:27, topic:8212"]
and we given thousands of euros to Vedder to help him in his development.
[/quote]

[quote="chaka, post:27, topic:8212"]
I shared my OshPark files
[/quote]

You my good Sir are a true scholar and gentleman. I extend my apologies to you and rest my case.

To clarify, I don't give 2 f&^* about any of that shop vs shop thing nonetheless I do care a lot about open source and will always pull people up to release their changes and as you have relayed them to Benjamin you did that part. He didn't think it worth releasing, that's his call. Its his baby...
```

---
## \#29 Posted by: rmrf Posted at: 2016-08-24T14:33:34.351Z Reads: 294

```
[quote="evoheyax, post:14, topic:8212"]
There's not a single person yet to complain on this forum he refused to fix their vesc. And by his wait times and his pictures, it seems like hes pushing out quite a few vescs these days.
[/quote]

Wrong.
[quote="squad, post:66, topic:2474"]
Chaka offered help at the beginning but then turned his back towards me and said he'll be not doing anymore business with me, so summing up he didn't repair any ollin VESC of mine. Funny thing is he even offered to replace the one that was fried but, obviously, didn't deliver. So myself as well as few (or maybe more?) people are on ollinboard company black list :joy::joy::joy:
[/quote]

It is sad however see @onloop and @chaka throwing shit at each other. Marketing is such marketing.
```

---
## \#30 Posted by: longhairedboy Posted at: 2016-08-24T14:37:55.851Z Reads: 292

```
[quote="@chaka, post:28, topic:8212"]
And now his very own repair agent is showing proof that they are using our VESC's to perform repairs on raptors...
[/quote]

No. I do not use Ollin VESCs to repair raptors. I use them in my builds and i use them when somebody sends me their raptor outside of Enertion support to do non-warranty custom work for which i charge money. I've done this twice now, and both times the customer supplied the Ollin VESC and i supplied only labor and testing. 

When i repair a Raptor i order ALL of the parts directly from Enertion. I don't pay for the parts, the customer doesn't pay for the parts, and Jason certainly is not going to pay for Ollin VESCs to replace shorted or fried Enertion VESCs when he's got Enertion VESCs basically on tap now. 

Everyone needs to calm the fuck down before i start calling thier moms and telling them they babies actin a fool.

One big reason I haven't had my own motors and mounts made is because i want to support the community and the businesses it has spawned. The sharing in this community can and should be benign. We can grow together. We can all profit. We can all benefit from everything we all learn everyday. That's how it should be. That's how i want to do business. Right now Enertion has the sickest belt drives around, and Ollin has the best VESCs. And unfortunately Maytech has my favorite remote at the moment but maybe one day i can do my own based on a similar design because frankly i don't like their lack of community involvement. Let your service, products, and thier quality speak for themselves. They speak to me every day. 

Is it too early to start drinking?
```

---
## \#31 Posted by: chaka Posted at: 2016-08-24T14:38:18.027Z Reads: 289

```
I actually repaired the same VESC 2 or 3 times, I also told him I would continue to repair VESC's for him once he fixed his mounting design. He was mounting the VESC in such a way as to short the vesc to a metal plate.

I don't enjoy throwing mud and I do my best to keep my views towards Jason to myself but I have to speak up at some point when he continues to drag my name into conversations in his VESC failure threads.
```

---
## \#32 Posted by: Svenska Posted at: 2016-08-24T14:50:46.106Z Reads: 286

```
@longhairedboy 

Why does that show up as a thing I said?????

Clarification:

## I DID NOT SAY THAT! 
I do not have this proof and I never said that. @chaka made this statement.
```

---
## \#33 Posted by: longhairedboy Posted at: 2016-08-24T14:55:25.327Z Reads: 289

```
[quote="Svenska, post:32, topic:8212"]
I DID NOT SAY THAT!
[/quote]

weird... gremlins i suppose. I updated my post.
```

---
## \#34 Posted by: Svenska Posted at: 2016-08-24T15:01:44.545Z Reads: 289

```
Thank you!
```

---
## \#35 Posted by: Blasto Posted at: 2016-08-24T15:27:17.602Z Reads: 287

```
While we are on the discussion of upgraded components, here is my educated guess on what could help the vesc be more stable:

-replace all 10uF 50V caps with 4.7uf 100V caps (same package)
-replace all 15uF 100V caps with 22uF 100V caps (stacked SMT 2220 pacakge), compensate for the lower capacitance on the 1206 caps and low ESL

What I've been wondering for a long time, and i guess I should just test it. Would adding a 50V TVS on the input of the vesc help prevent over voltage faillures, the problem with this is that the TVS would need to be huge to be able to handle the motor currents (20A+) @JTAG what do you think?
```

---
## \#36 Posted by: evoheyax Posted at: 2016-08-24T15:34:57.447Z Reads: 287

```
I'm sure, like chaka said happened here, that there's cases were he can't keep repairing the same vesc if you refuse to stop doing the thing that's breaking it. He wants you to keep riding, and it's cool that he even invests that much time into his customers to know what is going on in their build to figure out why it keeps breaking.

That was also buried inside of a build thread, I was specifically talking about you don't see threads of people complaining like you do with enertion vescs, where the sole purpose of the thread was to complain, and share their experience with the community.

If I were to reply on someone to fix something like my vesc if they were to break, I would also try not to take a piss on their work on the forum. Even then, I've seen this happen and chaka still fixes their vescs. I know I'd rather pay $20 for parts instead of $100 for a new vesc.

Based on the fact that enertion can sell them for $100, whether permanently, or for some period of time, says they must be costing Jason somewhere around $60-$70, around half the costs of chakas. If the cheaper parts were just as good, do you really think chaka would spend all that extra money on his vescs? Of course not. Me and many others have bought enertion vescs, they failed, was blamed that their setup broke it, went with chaka vescs in the same setup, and had no issues since. That speaks for itself...
```

---
## \#37 Posted by: Blasto Posted at: 2016-08-24T15:49:06.581Z Reads: 271

```
[quote="evoheyax, post:36, topic:8212"]
Me and many others have bought enertion vescs, they failed, was blamed that their setup broke it, went with chaka vescs in the same setup, and had no issues since. That speaks for itself...
[/quote]

I've busted some of my own VESC that I hand soldered in the same fashion as everyone else, DRV failure. I did not cheap out on components and followed the posted BOM. Could it be an un-updated BOM that is the cause here?

Also i stoped busting my drv's, less aggresive settings.
```

---
## \#38 Posted by: evoheyax Posted at: 2016-08-24T15:56:32.881Z Reads: 272

```
I'm not an expert in electrical engineering (though sometimes I wish I was studying it in school), so I can't say for sure yes. My hunch would be it is. If I'm not mistaken, I believe reading at some point on this forum that the c37 cap was linked to some drv failures. But it seems like drv failures are the most common, and thus there's likely several things that chakas changed to try to avoid them.

It would be cool if chaka posted his updated BOM for people like you, who are interested in building their own. But I can understand if he didn't want to do that, as his competitors would eat up all of his work. I'm sure if you messaged chaka, he would be glad to help you spit ball ideas and maybe even share his BOM with you.
```

---
## \#39 Posted by: Blasto Posted at: 2016-08-24T16:08:34.951Z Reads: 268

```
C37 is a 100V cap, a massive overvoltage would cause this guy to fail, thus my questioning on having a 50V TVS on the input to help prevent overvoltages
```

---
## \#40 Posted by: evoheyax Posted at: 2016-08-24T16:49:00.347Z Reads: 272

```
I know from my experience studying computer science that problems like this (ones that still exist in the main design after over a year of production) are often a chain reaction, thus why they still exist. There may not be one simple one size fits all fix. By repairing his vescs, chaka has had the chance to test ideas on people who have had issues (i.e., you keep blowing you drv chip, lets see if adding x, y or z stops it). It's a great position to be in to help further the development of the vesc. I'm actually a bit disappointed vedder hasn't adopted more of these changes that chaka has come up with. But it's his call as its his baby, and chaka will keep going with his mods, so it is what it is. Maybe an over-voltage causes this to fail, which in turn causes something else to fail, which ultimately cause a bigger chip to fail. I'm just speaking hypothetically, but these kinds of chains in my experience in software development are where the nasty bugs lye that stay in a product, even after its release. I can only imagine hardware has a similar possibility of having these kinds of chain reactions.
```

---
## \#41 Posted by: Blasto Posted at: 2016-08-24T16:59:54.846Z Reads: 263

```
I'm not looking for Chaka's secret sauce, that was just my educated guess. However I would like to know if adding a TVS would be good idea or just a waste of board space.
```

---
## \#42 Posted by: evoheyax Posted at: 2016-08-24T17:01:56.875Z Reads: 258

```
Message chaka, I'm sure he'll give you his insight.
```

---
## \#43 Posted by: Blasto Posted at: 2016-08-24T17:03:40.733Z Reads: 260

```
That's why I tagged JTAG, he's our man to answer this type of question.
```

---
## \#44 Posted by: chaka Posted at: 2016-08-24T17:10:08.990Z Reads: 264

```
Blasto pretty much nailed it with what we are doing to improve the vesc for the average user.  These are all things that drive up the cost of manufacturing so it is unlikely any vendor driven by profits will make these changes if they do not have to. 


Not sure if upgrading the tvs diode will do much. I have only had one fail and that was due to someone shorting the ppm pins.

The conformal coating definitely has produced some of the best results. And honestly, and I mean no offense to you Blasto, most failures are due to poor quality assembly and techniques.  I think most people are way too overconfident in their soldering skills and practices.
```

---
## \#45 Posted by: Blasto Posted at: 2016-08-24T17:17:20.069Z Reads: 264

```
[quote="chaka, post:44, topic:8212"]
And honestly, and I mean no offense to you Blasto, most failures are due to poor quality assembly and techniques.  I think most people are way too overconfident in their soldering skills and practices.
[/quote]

no offence taken, not sure why I would be.

But the idea of the TVS is to give the regen current an alternative current path in the case a BMS decides too cut out the charge path. I'll try it out, not sure how, all the BMS i'm using have big ass TVS's on them... need to get my hands on a chinese BMS
```

---
## \#46 Posted by: chaka Posted at: 2016-08-24T17:22:22.308Z Reads: 262

```
I was referring to your comment of blowing drv's even though you hand soldered them. You seemed to imply that it was the design rather than assembly or programming error.

Isn't the tvs diode only effecting the 5v rail?
```

---
## \#47 Posted by: torqueboards Posted at: 2016-08-24T17:26:16.306Z Reads: 263

```
@link5505 - We've made improvements but only based on what's been suggested and recommended by Ben.

I'm open to making even more changes if it makes it more reliable.

Our goal is to manufacture high quality VESCs. Low quality VESCs isn't what we want to sell or offer. So far, our track record is good and we also test each VESC twice.

We have stock now btw. Next batch should put is in stock with plans to never be out of stock.
```

---
## \#48 Posted by: Blasto Posted at: 2016-08-24T17:27:25.451Z Reads: 259

```
Yes there is one tvs on the 5V rail, but my suggestion is adding one on the input (50V 15-20A)

Oh and my soldering skills are spot on ;)
```

---
## \#49 Posted by: mason Posted at: 2016-08-24T17:32:58.260Z Reads: 255

```
@chaka do you mind uploading an improved BOM? I aswell as many others would appreciate it.
```

---
## \#50 Posted by: chaka Posted at: 2016-08-24T20:06:43.807Z Reads: 257

```
I have not written an updated BOM but Vedder will be releasing V6 BOM which has these updated components included. Once it is up I will be happy to cross reference the parts. Like I said earlier, Blasto has named most of the upgrades and it is a simple task to go on mouser to find what you need.

And really, none of this is secret knowledge. Anyone who has been paying attention to the development of v6 will know that the changes I made have been discussed thoroughly. I can't be expected to hold my competitors hands and tell them they should apply some updates that have been discussed or to cut the pins on P1 when it was stated over a year ago by Vedder himself.

In the end it is the difference of truly caring about the VESC open source project and being willing to do the research or simply being someone who is trying to extract as much as they can and publicly bad mouthing the design when you have used it up and soiled it's reputation.
```

---
## \#51 Posted by: Blasto Posted at: 2016-08-24T20:44:04.047Z Reads: 262

```
[quote="chaka, post:50, topic:8212"]
I have not written an updated BOM but Vedder will be releasing V6 BOM which has these updated components included.
[/quote]

Would be nice to have an ETA, but I know that is not under your control
```

---
## \#52 Posted by: onloop Posted at: 2016-08-25T01:20:47.491Z Reads: 268

```
[quote="chaka, post:50, topic:8212"]
In the end it is the difference of truly caring about the VESC open source project and being willing to do the research or simply being someone who is trying to extract as much as they can and publicly bad mouthing the design when you have used it up and soiled it's reputation.
[/quote]

If you truly cared about the esk8 community you would have been forthcoming about Vedder's BOM issues when you found them. It's an open source project, we are all meant to share...

Technically you are also the one "bad mouthing" the VESC design as you constantly claim the original parts in the BOM are inferior & that it can't handle heat and high current...

the scary thing is, Human lives are potentially at risk & you've been sitting back boasting about your superior knowledge & happily charging a premium for it. So Jerimiah, How exactly is that "truly caring"?  All this whilst simultaneously claiming that my business practices are questionable? 

It's obvious you are also trying to "extract" as much as possible from the VESC & that's fine you deserve too as much as anyone else.....  but if it wasn't for me probing hard to find ways to improve the VESC, this tit-for-tat-fiasco would have continued, more peoples builds may have resulted in failure and the VESC reputation would be further diminished. All while you sit idle in your VESC throne and watch it happen.

The truth is Jeremiah, to date you haven't really given much back to the community, you clearly have great VESC knowledge but you mostly keep it to yourself...You also refuse to repair people's VESC unless they came from you originally... this is obviously being done for commercial gains and that's fine, but just be a man & admit it.

Since you feel the need to constantly paint me as the "evil one" here are some points you might want to acknowledge.

1. I sell the VESC for $99USD with free worldwide shipping (I was the first to reach this price point) & I use all the parts as per Vedder's BOM & I would happily make changes to improve the VESC if they had of been documented, there is minimal if any profits at this price point, However I do this so that everyone can have an opportunity to build a decent esk8...
2. I was also the first Vendor to offer a comprehensive VESC replacement warranty so people aren't left empty handed, why? because I care about the community. This offer also prompted you to up your service warranty.... so ultimately the community is benefiting from my initiatives.
3. I FREELY host this forum for the benefit of the esk8 community & to facilitate the sharing of knowledge for those who are willing to participate.
4. I also allow you to promote your business for FREE on here.
5. I also offer FREE open source designs so people can make their own motor mounts.
6. Since Enertion started i have constantly battled to Lower esk8 part prices & improve product quality.
6. I have written hundreds of help articles so people can make better esk8s.
7. I have also made many instructional videos so the noobs can build up their knowledge much faster.

I have worked my arse off to build this industry up and this is to the benefit of everyone involved. Including you Jerimiah.

Anyway, I suppose I will finish by thanking you, we will be implementing these VESC BOM changes ASAP and also be striving to keep our prices low & manufacturing standards high.

The VESC is truly an awesome solution for everyone, so lets not let our egos & commercial interests get in the way of its evolution.

PEACE
```

---
## \#53 Posted by: chaka Posted at: 2016-08-25T01:52:46.201Z Reads: 255

```
> Would be nice to have an ETA, but I know that is not under your control

Best I can do is to keep sending him donations for his work. 

Vedder just received his revised pcb's last week so, fingers crossed, it will be posted to the github soon. One thing I am really excited about is a complete redesign of the bldc-tool so get your systems running linux/ubuntu if you want to use it! Although it will be fairly easy to port it over to win/osx if that is your flavor.
```

---
## \#54 Posted by: zmoney Posted at: 2016-08-25T02:00:48.601Z Reads: 257

```
https://media.giphy.com/media/uqPDIEPMODKne/giphy.gif
```

---
## \#55 Posted by: Sboard342 Posted at: 2016-08-25T02:24:32.007Z Reads: 257

```
I have experienced good and bad from many of the sellers on this site.  I understand there is a learning curve given the new designs. 

However, when it comes to VESCs Ollin is the only way to go.  I have four from Ollin and they are still running as strong as the day I received them.  And have always received within 3 weeks of ordering.

Relative to the Enertion VESC I paid $139 back in April and didn't receive it until July. It only lasted about about 2 weeks and 30 miles.  Now in order to have it replaced I need to buy an additional platinum warranty for it to be replaced at a price 57.00, making my total cost $196 and more waiting.  

Some manufactures just make better parts than others. I have been very happy with my Enertion motor mounts and Spacecell pro 4. 

http://www.electric-skateboard.builders/t/enertion-vesc-issue/7413
```

---
## \#56 Posted by: rodriguejoe1 Posted at: 2016-08-25T03:34:52.751Z Reads: 253

```
I would like to chime in as a noobie. In fact so new that I haven't received my Raptor from Enertion. I (we) the customer will pay more money for better components. Whether it is a skateboard component, a better dish washer, fridge or sparkplug. I am with the crowd that is sick and tired of cheap-READ- (profitable for the company bad for consumer) chinese made anything. Guys, BUILD A BETTER VESC even if it costs more money for the better components. Stay away from CHINESE=CHEAP. I want to use my board when I get it and not have it sitting there waiting for new VESCS to arrive. That's why we the customers will pay more money. I am putting together my 2nd board for my 21 year old son on paper. I will be reading and looking for the BEST components for my 2nd board regardless of price. Just my "customer" point of view. Also this back and forth does nothing for any of you vendors in my honest opinion. It just pushes potential customers away from your brands.
```

---
## \#57 Posted by: onloop Posted at: 2016-08-25T03:49:12.569Z Reads: 254

```
[quote="rodriguejoe1, post:56, topic:8212"]
BUILD A BETTER VESC even if it costs more money for the better components.
[/quote]

that's our plan..... constant innovation!.... we will also share "how we do it" with the community too.
```

---
## \#59 Posted by: jrpwit Posted at: 2016-08-25T04:09:09.653Z Reads: 255

```
Check out onloop's [The False Economy](http://www.electric-skateboard.builders/t/are-diy-electric-skateboards-cheaper-the-false-economy/165) thread. Here he states that his purpose is to provide better quality parts to make better electric skateboards.
```

---
## \#60 Posted by: KMeyerson Posted at: 2016-08-25T04:14:15.330Z Reads: 260

```
The VESC design works well under the correct circumstances and with good build quality. The acquisition of such a VESC is as much a challenge as the production there of.

I do agree that mods/alternate solutions in whole or in part must be documented clearly, however a BOM for a board can differ between batches by the same and alternate manufacturers and should not be the source of angst within our community. We should instead embrace the diversity we have been gifted with via the VESC and hope to improve the design such that varying component quality or style does not impact the performance so significantly.

The end solution is that instead of privately communicating with Vedder, we should all use his lovely forums to track our research. Perhaps we should publish component failure/repair rates and keep a public record of problems frequently encountered. As an open source project, ya'll should be totally okay staring there.
```

---
## \#61 Posted by: Pablo_702 Posted at: 2016-08-25T06:19:19.648Z Reads: 258

```
[quote="onloop, post:52, topic:8212"]
You also refuse to repair people's VESC unless they came from you originally
[/quote]

Do you repair other manufacturers vescs?
```

---
## \#62 Posted by: onloop Posted at: 2016-08-25T06:24:01.884Z Reads: 257

```
We do not currently offer a VESC repair service.
```

---
## \#63 Posted by: rmrf Posted at: 2016-08-25T13:33:52.660Z Reads: 254

```
[quote="chaka, post:53, topic:8212"]
One thing I am really excited about is a complete redesign of the bldc-tool
[/quote]


Can you please tell us a little bit more about it? What is so exciting that is coming?
```

---
## \#64 Posted by: chaka Posted at: 2016-08-25T13:51:17.849Z Reads: 249

```
The bldc-tool is being restructured to make it easier to make changes.
```

---
## \#65 Posted by: JTAG Posted at: 2016-08-25T13:54:34.740Z Reads: 255

```
@Blasto my apologies for the delayed reply, I was a little busy yesterday. 

At least one component is upgraded by @chaka  to a higher capacity model, we spoke about this a while ago after he saw my VESC's. I found it interesting/strange that vedder used 50V ceramic caps on places where up to 50V is applied [since capacity drops extremely fast when a ceramic cap is operated close to its designed voltage](https://en.wikipedia.org/wiki/Ceramic_capacitor#Voltage_dependence_of_capacitance). Yes this component is easily way more expensive (the cap alone costs 5 euro @ mouser = same price as DRV chip :fearful: ), but hey its that or very little low impedance capacity on the main power bus.

I would never claim that these type of upgrades will eliminate random blow-ups of VESC's. Lets approach its safe: I think that some component upgrades will reduce the damage in case of wrong settings / los of battery while braking.

A VESC (just like any other BLDC ESC) will most likely blow if you short any of its phase outputs with the other. There should always be at least some inductance in the line close to that what is configured as the motor inductance. The whole current monitoring + regulation is based on the presence of the motor inductance!

You can understand that if the motor inductance is configured incorrectly the current that realized vs. the current that is desired is very different ( since the parameters do not correspond with the real system ). So the current could exceed the max allowed values easily when motor parameters are wrong. (even the motor parameter measurement is sometimes wrong in its estimation).

Another way to easily kill any BLDC ESC is operate it close to its voltage limit, brake, and while breaking disconnect the battery. The ESC will boost the back EMF/energy trying to pump it to the battery, the battery however is gone and the only thing to pump the energy in is the CAPS. The energy storage capabilities of the caps are minimal, thus voltage will rise fast. The VESC has a system to disable when the input voltage is to high, but it might be to slow to react when there is no battery.
```

---
## \#66 Posted by: Blasto Posted at: 2016-08-25T14:57:08.214Z Reads: 241

```
[quote="JTAG, post:65, topic:8212"]
Another way to easily kill any BLDC ESC is operate it close to its voltage limit, brake, and while breaking disconnect the battery. The ESC will boost the back EMF/energy trying to pump it to the battery, the battery however is gone and the only thing to pump the energy in is the CAPS. The energy storage capabilities of the caps are minimal, thus voltage will rise fast. The VESC has a system to disable when the input voltage is to high, but it might be to slow to react when there is no battery.
[/quote]


This is exactly my motivation to having a 50V TVS at the input, the TVS will be much faster to react and give an alternative current path to avoid an overvoltage situation.
```

---
## \#67 Posted by: evoheyax Posted at: 2016-08-25T18:25:12.802Z Reads: 239

```
[quote="onloop, post:52, topic:8212"]
I was also the first Vendor to offer a comprehensive VESC replacement warranty so people aren't left empty handed
[/quote]

Are you talking about your platinum service? Chaka offered this a long time before you, and he is the reason you even offer it. There was a whole debate here, because he offered it before you, so what are you smoking?

[quote="onloop, post:52, topic:8212"]
I FREELY host this forum for the benefit of the esk8 community & to facilitate the sharing of knowledge for those who are willing to participate.
[/quote]

You host this forum cause if the industry doesn't grow, you have no customers to sell your products to. It also doubles up as freeing you up from having to give advice to people using your parts. You can point them to the forum, and have us answer them for free, instead of taking up your time, which is worth a lot of money.

[quote="onloop, post:52, topic:8212"]
I also offer FREE open source designs so people can make their own motor mounts.
[/quote]

You did this to show us how much they cost to be made, not cause you want others to make them. I tried to get them made from your designs, but unless I buy in huge bulk, they would have been over $200 USD each. So they are effectively useless, since the design requires more dimensions on a cnc machine then your new design, which you haven't released the files for.

[quote="onloop, post:52, topic:8212"]
I have written hundreds of help articles so people can make better esk8s.
[/quote]

If people don't know how to build them, you have no one to sell your parts to. So it's not about the goodness of your heart, it's about keeping a steady flow of customers, and it's a smart business move for you to inform people how to use your parts.

[quote="onloop, post:52, topic:8212"]
I have also made many instructional videos so the noobs can build up their knowledge much faster.
[/quote]

Same as above, the second you started making all these videos is around the same time your company started blowing up. It's a smart business move to inform your customers of how to use your products.

Look, at the end of the day, you are brilliant business man. You know what to pick your arguments about and how to effectively argue. You do a good job of spinning things you do that are crucial to the survival of your company as favors to the community.

You are growing the industry and you are allowing others to sell their products on the forum, and that I applaud you for. It's hard to argue that certain parts you sell like your motors are not high quality motors (whether they are over priced or not is a whole nother argument).

But your a business man. What features have you added to the vesc? Do you even know C? How deep is you electrical engineering education (do you have a degree in electrical engineering)? I just created the first 4wd board I've seen on this forum in a working state. I just created the first deck I've ever seen that was built from cnc milled 1/16th" veneers and pressed with a hollow core, and 100% Canadian maple (no CF of FG). And I invite you to participate in my thread, and you don't care to even say anything about these innovations. Your too caught up in your business to see things from a builders eye anymore. You outsource everything you can. Do you even own a cnc milling machine? Or a jig saw or a press or anything that can be used to fabricate parts?

I'm surprised to see Jerimiah actually rip into you, but he's been very patient, and I think he's finally done putting up with this hoax you have going of being for the community when you care more about keeping your business going instead of being willing to lose your company because you chose to use shitty Chinese factories multiple times to make shitty quality vescs. If you haven't significantly studied electrical engineering and can't explain everything that's happening at the board level, then stop hating on others that do. I am going out of my way to take more electrical physics class, and C class, just so I can understand the vesc better, and try to offer something to the community. Did you take through calc III? did you take general physics II with applied calculus? Have you taken computational physics (which I'm taking right now)? Stop acting like your smarter than everyone and be willing to admit your mistakes, and man up to them. If I can have my dream of starting a board company, and I make shitty boards, I won't blame my customers, but accept I picked the wrong company to make them, and accept that my company might go under because of that, instead of my customers bank accounts.
```

---
## \#68 Posted by: cesargrimmelprez Posted at: 2016-08-25T18:36:43.366Z Reads: 222

```
His motors arent overpiced, and the vesc com from texas... Please stop choosing sides, like @longhairedboy said, chaka's makes excellent vescs and enertion makes excellent drive systems... And the best parts, it works absolutely fantastic together, so stop the childish behavior and both shoukd work on further developping their own products...
```

---
## \#69 Posted by: mason Posted at: 2016-08-25T18:48:16.639Z Reads: 225

```
The VESCS only recently started coming from Macrofab. Previously, he has used multiple different vendors, one being Maytech.
```

---
## \#70 Posted by: evoheyax Posted at: 2016-08-25T18:49:17.338Z Reads: 228

```
for the last year before this new factory in texas, he went through 3 factories in china. I bought vescs from 2 of those factories, 1 was broken on arrival, the other broke the second day of use. I was told It was my fault, I likely configured them wrong or something. Bought from chaka, did the same thing to set them up in the same setup, and rode for 4 months and they still work great. 

Even now with this new texas factory, they ignored vedders warning about the pins needing to be clipped so it doesn't puncture the main positive lead to the cap board.

His drive system for a mono drive used to suck. His old motor mounts had a small screw to adjust tension. You need to locktite them or they will come loose due to vibrations. Both of the ones I bought, The screws broke off when trying to turn them and take them out. After the first one, I was extremly carful taking out the second screw, but the head still broke off, and the screw threads are stuck in there. They looked like shitty quality screws, and beyond that, a bigger screw should have been used their from the beginning so this would have never happened.

He also used to sell only 9mm belts for mono drive systems. He said they will work fine on hills, but they didn't I ate through 8 belts in 6 months of riding. Every time, I tried new belt tensions, because I was told it was either too lose or too tight. But the problem was that a 9mm belt can't handle 10%+ grades with a 200 pound rider. Having told him everything, he assured me I was doing something wrong and his products were great.

I wasted over $1000 on enertion products and I have nothing working 8 months later except a motor to show for it. His products are better now IMO than they ever have been, but he never once offered to replace ANYTHING (excpect after months of arguing, he ddi send me a 12mm belt, which fixed the issue and proves my point that he should never of sold 9mm belts for mono drive systems, despite requesting it and advertising it like crazy.

I have a right to be pissed off, because I was naive and fell for his marketing scams.

This isn't childish behavior, its using logic, experience, and science to back up my claims. So stop being a fan boy and realize that your experience may not have been everyone else's.
```

---
## \#71 Posted by: longhairedboy Posted at: 2016-08-25T18:52:32.873Z Reads: 221

```
[quote="evoheyax, post:70, topic:8212"]
Even now with this new texas factory, they ignored vedders warning about the pins needing to be clipped so it doesn't puncture the main positive lead to the cap board.
[/quote]

Yep. 2 minute fix with a dremel's sanding drum and some blue tape. Clipping still leaves sharp points of not done with flush snippers. 

Ollin's are very nicely snipped.
```

---
## \#72 Posted by: evoheyax Posted at: 2016-08-25T18:55:05.773Z Reads: 223

```
if you cut them to the right length before they are soldered on, this problem is 100% avoidable. I remove my canbus ports and solder wires straight through the board. I am careful with the wire length, so that I don't have pins sticking out. that could short something or poke something. It's about being aware of what your building and taking the time to build something right the first time.
```

---
## \#73 Posted by: longhairedboy Posted at: 2016-08-25T18:58:45.486Z Reads: 224

```
i want to do somethign similar with the USB ports so i can start having them accessible from outside the box.
```

---
## \#74 Posted by: evoheyax Posted at: 2016-08-25T19:05:55.356Z Reads: 224

```
[quote="longhairedboy, post:73, topic:8212, full:true"]
i want to do somethign similar with the USB ports so i can start having them accessible from outside the box.
[/quote]

YES!!! That's a great idea. The only good thing about the broken vescs I bought from enertion is I've been using them to practice my soldering skills, and learn to desolder ports correctly.
```

---
## \#75 Posted by: cesargrimmelprez Posted at: 2016-08-25T19:26:34.844Z Reads: 221

```
why am i a fanboy now? Im not talking past but im talking present... Im just repeating longhairedboy words... If i would be a fanboy id also say that his vescs are super awesome... Wich i did not do.. So keep your thoughts about me for yourself...
```

---
## \#76 Posted by: cesargrimmelprez Posted at: 2016-08-25T19:31:33.879Z Reads: 214

```
Would it aslo be possible to switch to micro usb (the one u get on a phone charger) usb type c (newest version of usb, alot of opportunities..)?
```

---
## \#77 Posted by: evoheyax Posted at: 2016-08-25T19:35:11.650Z Reads: 211

```
Sorry if I upset you, not my intentions at all. I've just had a very bad overall experience with enertion.

What benefits do you think the micro usb would have that makes you want it? Other than being smaller of course.
```

---
## \#78 Posted by: cesargrimmelprez Posted at: 2016-08-25T19:38:06.146Z Reads: 211

```
Smaller and i think that usb type is more common so youd always have a cable to connect it with ypur computer, and hahah no problem bro, i understand ypur frustration, i would be to, and behold me, i ordered my vesc from enertion a while ago before i read al these bad topics about it, and im really scared of braking it
```

---
## \#79 Posted by: evoheyax Posted at: 2016-08-25T19:50:09.145Z Reads: 216

```
I personally think these ones from Texas should be fine for the most part if you do that quick fix that longhairedboy suggested. But like chaka has said, I think he's done more to try to protect it from abuse or harder uses than than enertion. If your using all enertion parts, I think your less likely to have issues. It's not that their systems today suck, the designs are way better. And they are geared and powered efficiently. But when someone advertises warranties, and does nothing when problems arise, that's when I start to really have a problem. The math and science behind his products (besides the vesc) are great, it's just the way he's pushed inferior products in the past and letting his customers pay for his mistakes (whether that be a overlooked flaw in a design or choosing a bad manufacture).

The problem I've had with micro usb ports in the past is they are more fragile, and break quite easily if just a tad bit of pressure up or down is applied. It's been a while since I last looked at the pin schematics which would tell you if its possible or not. But if there's the same number of pins, it's likely possible. It would make stacking 4 of thes ports way easier and nice looking :P
```

---
## \#80 Posted by: zmoney Posted at: 2016-08-25T19:56:02.746Z Reads: 216

```
Well said.

> The end solution is that instead of privately communicating with Vedder, we should all use his lovely forums to track our research.
```

---
## \#81 Posted by: JohnnyMeduse Posted at: 2016-08-25T20:03:31.598Z Reads: 219

```
There is A forum on Vedder site, juste for that.
```

---
## \#82 Posted by: chaka Posted at: 2016-08-25T20:19:44.624Z Reads: 221

```
Exactly, all the info I have is freely available on Vedder's forum. Don't be lazy.
```

---
## \#83 Posted by: Maxid Posted at: 2016-08-25T20:24:09.617Z Reads: 213

```
I was like "wow somehow he got a point" - until you started listing courses trying to diss onloop because he might not have the same education. Taking some university courses means shit.

Sorry if I sound like an asshole but people that feel superior just because they listen to a professor talk are simply idiots.
You can at least back it up by showing the actual innovations you came up with and I compliment you for them.
But I know that there are people out there that miss the innovating or "work" part (not you obviously) and that makes me angry.
```

---
## \#84 Posted by: JohnnyMeduse Posted at: 2016-08-25T20:26:05.281Z Reads: 213

```
[quote="chaka, post:82, topic:8212"]
Don't be lazy.
[/quote]


C'mon it is my only reason to wake up...
```

---
## \#85 Posted by: sl33py Posted at: 2016-08-25T20:54:26.024Z Reads: 213

```
Wow - this thread has blown up...

[quote="rodriguejoe1, post:56, topic:8212"]
Stay away from CHINESE=CHEAP.
[/quote]

I think this is a common misconception.  There are quite a few things made in China that are made *extremely* well.  **It's all in the QC and design and oversight.**  When shopping for bottom dollar options - yes - usually a bad idea.  But it can also be made in mexico, or malasia, or india or ... (you get the point).  

[quote="rodriguejoe1, post:56, topic:8212"]
I will be reading and looking for the BEST components for my 2nd board regardless of price.
[/quote]

That's cool, but maybe not something most folks can do.  A lot of students here who are looking for the best bang for their buck.  And compromising for a less expensive option.  I get it, and typically buy top quality, but sometimes there's a less expensive option that works well (i have a few SK3's - not the best wires, but they work really well otherwise, and less than other options!)  When you can find them in stock.

[quote="rodriguejoe1, post:56, topic:8212"]
Also this back and forth does nothing for any of you vendors in my honest opinion. It just pushes potential customers away from your brands.
[/quote]

Totally agree.  It's disappointing to see vendors arguing back and forth.
```

---
## \#86 Posted by: chaka Posted at: 2016-08-25T21:18:23.312Z Reads: 204

```
There is a huge difference between losing ones sh%@ and defending a company you have worked very hard for as well as defending a piece of open source hardware I am heavily involved in.
```

---
## \#87 Posted by: rodriguejoe1 Posted at: 2016-08-25T22:22:50.711Z Reads: 209

```
You both make valid points. My son would probably go for the less expensive but functional product. I see him do this with his racing drone. He is young and does not have too much money to spend on big boy toys.  @chaka I definitively see that you were defending your position on a product you have spent countless hours and monies trying to make better for all of us.
SO... WHO MAKES THE BEST VESC???????
Oh no, here we go again!
```

---
## \#88 Posted by: mason Posted at: 2016-08-25T23:07:48.745Z Reads: 211

```
who makes a better VESC (opinions)

[poll]

- onloop
- chaka

[/poll]

edit: why did onloop move his post to the bottom?
```

---
## \#89 Posted by: onloop Posted at: 2016-08-25T23:13:35.303Z Reads: 214

```
I am not an engineer. I am not the smartest guy in the room either..... I am no better than anyone......

But I have a dream...

All I want to do is make better quality more reliable products, lower the cost to produce, improve my customer service & warranties, optimise my business processes & educate the masses about building awesome electric skateboards at home.

Get in my way and their will be a battle.

......so....yeah....I might not be the best educated but I won't fucking give up.... I'll admit my mistakes... and i will fight my way to the top...

Don't start a business if you ain't got the fight in you... you will need some fight in you to succeed... 

Peace.
```

---
## \#90 Posted by: guyguy Posted at: 2016-08-25T23:35:54.129Z Reads: 207

```
It may be fair to say your experience with Enertion was bad or that you had issues with his product -- what is not fair to do is to dismiss or minimize Onloop's contribution to the community because it's not a facet of the community you necessarily identify with i.e. the promotional side. I think there's this myth, especially amongst those that are technically minded that (1) sales and marketing is easy and that (2) innovation, great work or a great product will sell itself. The truth is (1) it isn't and (2) it won't. Nothing will kill a business faster than not being able to find or create a customer; not lack of innovation, not poor quality, nothing -- and it's really hard to do. This applies to promoting the community too - more new people helps to push the envelope forward. 

To further my point, every time Onloop creates a customer for himself in creating visibility for this community he creates a potential customer for Chaka and other builders. As a result, these other builders in the community have more time and money to spend on innovation instead of sales and marketing. For example, your first step in becoming an Ollinboard Co. customer was to first become an Enertion customer. It does really suck that your path was painful but the silver lining is that it eventually lead you to a product you seem to be happy with which you may not have found otherwise. Personally, I only found out about Ollinboard Co. and became a customer through the visibility Onloop has created. I don't think I'm the only one. Onloop should get loads of credit for that.
```

---
## \#91 Posted by: furryfrog Posted at: 2016-08-25T23:43:48.638Z Reads: 209

```
Well the answer to the topic title appears to be a yes. Unfortunate to the whole community that he is being tight lipped about the changes, Open source projects are open and upfront.

I can see why Onloop is upset, I believe he honestly thought that the Ollin Vesc using upgraded components was just marketing speak, He most likely thought that if it was changed it would be out in the open and a bom would be posted.

Onloop is probably not as naive now, and probably feeling dejected and stabbed in the back to a certain degree. My Assumpton is he created this place for everyone to get ahead, there is more than enough pie for everyone.

Its good this whole fiasco is out in the open now at least.
```

---
## \#92 Posted by: furryfrog Posted at: 2016-08-25T23:50:54.355Z Reads: 207

```
I agree with you, I did not know about Ollin, or Longhairboy's companys until I came here through enertions website. I found out about enertion and the Raptor before this site. Fiasco's like this must make Onloop question what the hell is he doing all this for sometimes.
```

---
## \#93 Posted by: Pablo_702 Posted at: 2016-08-26T00:26:43.538Z Reads: 208

```
Way easier to find and cheaper i should have at least 10 of those usb android cables
```

---
## \#94 Posted by: Sean555 Posted at: 2016-08-26T00:37:09.573Z Reads: 215

```
I agree.  @onloop before this forum all I bought was Chinese clones, now I'm purchasing from Enertion, @torqueboards, and @chaka for my first builds.   
I just want to take the time to take you 3, @Michaelinvegas, @JLabs, and everyone else that's posted builds and info on this site.  Can't wait till I have my first true self build!! You guys have been so helpful!!!!!
```

---
## \#95 Posted by: rodriguejoe1 Posted at: 2016-08-26T00:41:11.892Z Reads: 227

```
@furryfrog...ditto...That is exactly what is going on with me as I learn more about esk8s. I just purchased EVERYTHING from Enertion and I believe I made a good decision. I started reading a lot and decided to build one for my son, however more towards a Trampa. I am learning about products from chaka, longhairboy, Trampa and other builders like @guyguy said... but I got my foot in the door with ENERTION.

@onloop: I disagree with you onloop. It seems to me that you are a pretty smart guy. You don't necessarily need an advanced education. It starts with a passion for something you love to do, the desire to always be better at what you do and a heck of a lot of hard work. I am considered "edumacated" by most and a hard sell. Trust me when I tell you that my credit card will remind me just how smart you are this month after buying everything for my first build from you.
```

---
## \#96 Posted by: onloop Posted at: 2016-08-26T00:56:45.865Z Reads: 224

```
[quote="furryfrog, post:92, topic:8212"]
Fiasco's like this must make Onloop question what the hell is he doing all this for sometimes.
[/quote]

I must always remind myself that my business succes is secondary to the success of the community.... if people can't successfully build esk8.... if newcomers are unable to source parts from various locations/vendors... if folks are unable to choose what form their creation will look like.... unable to find the information they require .... etc etc......Well..... than there is no market...  there are no sales.... there are no successful businesses...

I need competition for my business to be successful & the community needs successful businesses to exist so that it can grow and attract new members to bolster the community numbers... excellence & innovation can only occur when the market is growing.... strength in numbers...

If we, the collective, plan to take this niche market mainstream... if we are to compete with the Chinese factories and the crowdfunded startups we need to remind ourselves we are all part of the electric skateboard builders movement..... 

Let's roll as one. Only together will we all prosper.
```

---
## \#97 Posted by: zmoney Posted at: 2016-08-26T01:52:26.609Z Reads: 220

```
annnnndd close thread

https://media.giphy.com/media/el0ou7lRocwSI/giphy.gif
```

---
## \#98 Posted by: longhairedboy Posted at: 2016-08-26T04:12:13.840Z Reads: 211

```
[quote="onloop, post:96, topic:8212"]
Let's roll as one. Only together will we all prosper.
[/quote]

I'm with you bro. This community of builders, bad asses,  and bad ass builders are going to fuck some commercial shit up yo. Let's bring it!
```

---
## \#99 Posted by: lowGuido Posted at: 2016-08-26T05:12:07.148Z Reads: 201

```

```

---

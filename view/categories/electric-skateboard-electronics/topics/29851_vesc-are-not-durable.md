# VESC are not durable!

### Replies: 33 Views: 2839

## \#1 Posted by: Fetteperson Posted at: 2017-08-06T08:11:00.416Z Reads: 355

```
Hello everyone

I thought, since this forum helped me a lot with my build, I would share my experience with DIY boards.

First, do not buy cheap parts.

Second, since the VESC is the only real esc for skateboards, you don't have a choice, and this is the problem... I spent to much money on cheap, or wrong parts for my build, until finally I had a perfect working dual-setup with max speed 50km/h and torque like a boss. 

1. Now here is the problem... after about 6 months of driving, maybe 500km, all the sudden, one day, it stopped working... after research... internal shortage. Changed the little chip on the VESC, but didn't help.

2. My best friend had also the same problems... after couple months of driving, one day, the VESC just didn't work. On the BLDC tool, everything seemed to be ok, but the motor(s) just didn't spin anymore.

One of the VESC came from esk8.de, the other from faradaymotion.com, both produce in Europe, as I know in Germany. So I don't think production quality is an issue.

Over all I can say now, that the VESC is just not durable for a long period. You really should think about building your own DIY board. For sure it is a lot of fun to build and to learn a lot, but the goal in the end, is to have a perfect working esk8, and not only for 6months...
At the moments, I ride my esk8 only with 1 motor (which sucks, if you are used to 2 motors) but I don't want to spend another 200$ for something that well break sooner or later.

Did you also have this kind of experience with the VESC?
```

---
## \#2 Posted by: trampa Posted at: 2017-08-06T13:45:58.226Z Reads: 310

```
There are a lot of different ESCs availabe that are based on the VESC-Project HW designs. You can't generalize the Hardware. Some vendors do output high quality and even improved the original designs a lot, while others worked in the opposite direction, trying to sell on price point. Second thing is your setup. A lot of users push way to much amps and use to high KV value motors etc. 
Some had their battery wires poking through the JST pins because manufacturers didn't cut the pins down etc. Some users knew that and finished the job themselves.

I never killed a single VESC-based piece of HW, while others managed to fry them within a short period. It has a lot to do with personal knowledge and skills. 

A consumer product can also fail within a couple of months! 

Frank
```

---
## \#3 Posted by: Hummie Posted at: 2017-08-06T14:01:14.173Z Reads: 288

```
What u mean personal knowledge and skill. Of the maker? other than making sure the pins aren't going in and putting on the right motor and settings the user seems uninvolved.  When u say people put in too many amps..the temp shutdown should deal with that danger no?
```

---
## \#4 Posted by: Listen Posted at: 2017-08-06T14:52:18.593Z Reads: 267

```
[quote="Hummie, post:3, topic:29851"]
When u say people put in too many amps..the temp shutdown should deal with that danger no?
[/quote]

Temp shutdown is an emergency procedure meant to protect against immediate destruction... But that doesn't mean you can't damage them other ways.  

Heat kills microchips. So ideally you'd want a VESC that is overkill for the application to get the most life out of it... But that's not how people do things.
```

---
## \#5 Posted by: trampa Posted at: 2017-08-06T15:13:03.441Z Reads: 250

```
That thing is called VESC SIX.

Frank
```

---
## \#6 Posted by: trampa Posted at: 2017-08-06T15:35:23.599Z Reads: 245

```
@Hummie

Other than: Correct gearing, motor KV, battery voltage, correct and reasonable settings, vibration elimination, cable routing and protection, cooling etc.

There is a lot you can do to keep your HW healthy.
Users tend to squeeze the max out of their gear and are disappointed if something fails. A consumer product is often limited by software and doesn't push things to the limits. 

Frank
```

---
## \#7 Posted by: evoheyax Posted at: 2017-08-06T16:13:31.349Z Reads: 234

```
This used to be a problem you couldn't avoid unless you bought Ollin board Co VESCs. Now, others have stepped up and made moddifications to the BOM and designs to improve reliability. With Ollin Board Co VESCs I have 8 and never had a failure due to operation, only my own stupidity (shorting on the bench, ripping off usb ports by leaving a trippable (an oh, I tripped) wire plugged in, ect).

Especially with the FOCBOX now, and others are folling suit, we are seeing much better quality VESCs.

Vedder did a great job with the VESC 4, but he never eliminated everything. Ollin Board Co found fixes that improved FOC reliability and decreased DRV errors. Vedder refused to modify the original BOM with them, as it slightly increased the cost of parts and said it was unnecessary.
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2017-08-06T16:18:06.805Z Reads: 222

```
ya i hate to sound like a parrot, but that FOCBOX!! its been a dream since i got my batch.. only issue i had was my ignorance of the correct settings. =)
```

---
## \#9 Posted by: psychotiller Posted at: 2017-08-06T17:31:00.096Z Reads: 213

```
Dude...Before you post threads like this you need to do about 3 years worth of reading. Reason why you ask? Because you are seriously ill informed. It's not the forum's fault either. You need to read. Either edit your post or ask the moderators to take it down. The information you've written here is ridiculous. All threads like this do is set false information in stone. Then new users come here, read it and assume it's true. It perpetuates ignorance.  READ!
```

---
## \#10 Posted by: Hummie Posted at: 2017-08-06T17:47:10.559Z Reads: 209

```
i think it's a good topic and appreciate him coming and telling us his experience with some of what are touted as reliable vescs with updated bits.   despite following the guidelines listed above there also seems to be success keeping under 60000 erpm, but I've had a vesc with updated bits fail on me as well and I'm well under the erpm safety line listed above.  I'd say this post more so brings to light the ignorance of everyone making vescs.  We're now at version 6 which is a fortune or the focbox and both of these haven't been tested in the real world enough for me to feel assured that they won't break either.
durability and reliability are so important especially on an eboard and so far the iterations of the vesc haven't been up to snuff in that category
```

---
## \#11 Posted by: psychotiller Posted at: 2017-08-06T17:50:41.544Z Reads: 198

```
[quote="Fetteperson, post:1, topic:29851"]
Second, since the VESC is the only real esc for skateboards, you don't have a choice, and this is the problem...
[/quote]

He could have asked a question though instead of this. His thread title alone is pretty misleading.
```

---
## \#12 Posted by: Hummie Posted at: 2017-08-06T17:54:04.877Z Reads: 192

```
i think the thread title is legit but maybe he hasn't been to hobbyking yet and seen all the escs.  but I bet he has and knows there's other escs out there and he just doesn't think they're even worth mentioning.  for me the vesc rocks and I don't consider anything else and 'm really hoping the new stuff is more reliable than the past.  expensive hobby at best and launch you on your face at worst with a vesc failure
```

---
## \#13 Posted by: psychotiller Posted at: 2017-08-06T17:58:01.799Z Reads: 185

```
I disagree, there are too many posts like this on the forum.
```

---
## \#14 Posted by: Silverline Posted at: 2017-08-06T17:58:10.361Z Reads: 180

```
If he had asked the question instead, you probably would had told him to use the search function  ;-)
```

---
## \#15 Posted by: psychotiller Posted at: 2017-08-06T18:01:08.291Z Reads: 179

```
Or, maybe I would have answered his question or given advice. Go thru the forum a little bit and tell me with certainty that I don't contribute.
```

---
## \#16 Posted by: Fetteperson Posted at: 2017-08-06T18:06:58.020Z Reads: 179

```
Hello, 
I think I have spent enough time on this forum. I also was really happy with my VESC. For me it seemed like a perfect product (next to those update difficulties). But if after 6 months of driving, it suddedly stops working while riding 20km/h... And a couple weeks later my friends Vesc also broke...
At the moment, my opinion is that you shouldn't go with a VESC if you want a reliable product which least 2 years.

If you say I didn't read enough... What did I miss for those failures. It's note like it broke after 1 week. And on top of that with a dual setup, the VESC limits are far away when riding safely ( <30km/h)
Would appriciate an answer.
```

---
## \#17 Posted by: Silverline Posted at: 2017-08-06T18:08:04.969Z Reads: 174

```
Chill down, nothing personally man.

For newbees like me, it`s nice with these threads, where experienced people can give some feedback. As has already been given. I have a vesc 4.12 from esk8.de and two FOCBOX`s in the mail. So usefull info is much appreciated
```

---
## \#18 Posted by: psychotiller Posted at: 2017-08-06T18:13:56.775Z Reads: 166

```
The vesc isn't a finished product. Not one manufacturer has ever said it was. It is still in continuous development. That being the case you did pretty well at 6mo. Without burning one out. There are a few builders that have made modifications to their VESC offerings and have had great results. Ollin for example. Though, I burned out 2 of those. Chaka fixed them for me. With all of the variables possible, being that we as end users can change and adjust all parameters in the VESC, it is impossible to say what causes one to burn DRV chips and Mosfets. It's impossible. 

Also, just curious, how many FVTs or Castle XL2's Or Sleeping Lion, or EzRuns have you used and burned out? How many VESC driven builds have you worked on?
I've probably burned out 6-8 vescs total, all of them except for one were repaired with success. @JohnnyMeduse will glady repair yours and update components most times to make them FOC worthy for $45. Did you ask him about his service before you wrote "VESC's are not durable"? Did you know about his service?
```

---
## \#19 Posted by: chaka Posted at: 2017-08-06T18:41:59.915Z Reads: 152

```
c,mon now. I have seen how you treat your VESC's ;)
```

---
## \#20 Posted by: Hummie Posted at: 2017-08-06T18:48:22.084Z Reads: 151

```
one day I will have my components in an enclosure, and that enclose won't be a 1/16" plastic bubble bolted to a board.  I'm skipping right from duct tape to rock solid.
```

---
## \#21 Posted by: NAF Posted at: 2017-08-06T18:54:41.325Z Reads: 147

```
Focbox, Ollin, Axle. All pretty bad ass and hard to kill.
```

---
## \#22 Posted by: psychotiller Posted at: 2017-08-06T18:59:18.329Z Reads: 149

```
1/8" you bass turd
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2017-08-06T19:06:31.356Z Reads: 152

```
Yep I can confirm The FocBox is bulletproof :wink:

https://www.instagram.com/p/BXdqGfBH7iw/
```

---
## \#24 Posted by: onepunchboard Posted at: 2017-08-06T21:43:01.613Z Reads: 143

```
Hi I'm new to here, and I'm here to complain about, **VESC 4.12**(Maytech). 

I purchased vesc 1 wk ago, now dead with **drvfault**. I have to admit that i pushed little too much. **> I put, 80amp motor with 80amp brake** with sk3 260kv motor, 6s lipo in 1:3 gear ratio. otherwise it becomes safety issue for even 60kg meat bag. 

But I hardly pushed throttle to the max, mostly just touching it. Not much of braking either. While it could caused by many thing, certainly not the temperature cuz I put large heatsink and temp never passed 40c on drv & fet. 

Neither the cable shorts, I checked every parts before connect to any power source. As there isn't definitive answer to the drv faults, I'm, as an average Joe, think drv cheap itself is the main cuz. I'm hopping that focbox last, finger crossed, I really can't trust this thing anymore.

 If it brakes down again with double the cash, I'm out of this hobby. It's risky and expensive.
```

---
## \#25 Posted by: psychotiller Posted at: 2017-08-06T22:00:22.921Z Reads: 138

```
[quote="onepunchboard, post:24, topic:29851"]
I purchased vesc 1 wk ago, now dead with drvfault. I have to admit that i pushed little too much. &gt; I put, 80amp motor with 80amp brake with sk3 260kv motor, 6s lipo
[/quote]

Knowing this. Would you say that it sucks and you shouldn't buy maytech or would you think you need to do more research and set your system up correctly? Contact @JohnnyMeduse to get your vesc repaired.
```

---
## \#26 Posted by: onepunchboard Posted at: 2017-08-06T23:35:30.202Z Reads: 130

```
I like vesc. it is super smooth, but the fact that I have to have 2 units to push 60kg off the ground with normal setting tells me that it is not durable, as subject stated. so called **_hobby grade_** doesn't break a sweat in 120amp. So I wouldn't say vesc sucks, but not great. It is still needs some development.

Fact that it does not have any kind of limitation to program in such a way, other than spec paper **50-240amp** says it is still an alpha product.

With production of vesc 6, it may start the war against many money grab indigogo projects, yet the price of the 6 is far much greedy at this point in time.

for that I rather buy boostedboard

Thanks for intro the fixer, but I'm going to try fixing myself.
```

---
## \#27 Posted by: psychotiller Posted at: 2017-08-06T23:39:36.907Z Reads: 125

```
The biggest problem is you are running 6s. Personally, at 6s I think you'd be better using n ezrun esc. If you want performance with a vesc you need a lower kv motor and at least 8s voltage. 10s ideally.
```

---
## \#28 Posted by: onepunchboard Posted at: 2017-08-06T23:47:37.128Z Reads: 128

```
Yeah, I know, I cheeped out and paying my lesson. Thankfully I only burned $500+. I'm stuck with this low end board for now. Anyways, focbox will be my last vesc. I'm ganna handle with care :wink:

**Bottom Line, Maytech is not reliable vesc, avoid at all cost.**
```

---
## \#29 Posted by: lrdesigns Posted at: 2017-08-07T00:43:43.277Z Reads: 123

```
My maytech's have been perfectly reliable. 7 months of commuting and I ride it like a mad man. 

Though Im on 12s dual. Each vesc is limited to 500w. Its only 12amps per vesc. I'm 110kg and have plenty of hill climb performance and top speed.   I would agree with @psychotiller that 6s is better to suited to RC car esc's.  

<img src="/uploads/db1493/original/3X/8/4/84b51f8f08f0172d875bddfc8095f6cd49c3a861.png" width="690" height="134">

You should be good with focbox, they are one of the most reliable.
```

---
## \#30 Posted by: onepunchboard Posted at: 2017-08-07T00:49:42.316Z Reads: 120

```
isn't batt max according to batt type u use?
```

---
## \#31 Posted by: lrdesigns Posted at: 2017-08-07T00:54:59.879Z Reads: 122

```
The maximum should not be more than what your battery can handle but its a good way to limit system power. Battery amps x voltage gives you your max system power.  My batteries can easily handle 100 amps but this setting makes it more ride-able and keeps things cool. 

My system is dual so its 24 amps x 44 volts = 1056w is the max watts my system can draw.
```

---
## \#32 Posted by: gliz5714 Posted at: 2017-08-09T14:13:43.538Z Reads: 95

```
=/

I was steered in the direction of getting a focbox for my initial board (just completed).  I may upgrade from a 6s in the future, but I don't believe I will be doing so for the next 6 months (at least).

No complaints off of my board though, don't need much torque for my commute and 20mph is plenty fast with a 295kv motor.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-08-09T14:24:48.196Z Reads: 94

```
[quote="Fetteperson, post:1, topic:29851"]
Did you also have this kind of experience with the VESC?
[/quote]

I'm using @chaka   Ollinboard 4.12 Vescs with heat sinks in dual drive on one build for over 1 year and on another build for around 8 months running them hard up and down hills with motor max 80a and Batt max 50a-60a and I have had zero issues.
```

---

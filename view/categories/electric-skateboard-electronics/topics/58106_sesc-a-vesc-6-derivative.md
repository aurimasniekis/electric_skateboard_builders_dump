# SESC a VESC 6 derivative

### Replies: 239 Views: 8116

## \#1 Posted by: secupol Posted at: 2018-06-07T05:17:13.142Z Reads: 707

```
VESC 6 clones were developed using drv8323 without using drv8301.
drv8323 has three current sensing amplifiers, so no separate amplifier is required to detect the three-phase current. However, Vesc 6 uses inline sensing method while sesc uses low side current sensing method.
The regulator also has a smaller output current than drv8301, so it is difficult to use the regulator except for power at the rf receiver or hall sensor for motor.
The SESC is compact and designed to keep up with VESC 6 features.

![sesc-v1-top|690x498](upload://bMxaxIjmHfBS4Q896uUBNT8ifFH.jpg)
[Top View]

![sesc-v1-bot|690x498](upload://5NOdSqdHwpnJVx7d30TSol3kMhr.jpg)
[Bottom View]

 
 (1)
https://youtu.be/XX38Unpmuto
[Sound Comparison]

(2)
https://youtu.be/KdXFNXOee0s
[Current Consumption Comparison, ERPM 6000, Duty 10% same condition]
```

---
## \#2 Posted by: Maxid Posted at: 2018-06-07T06:11:47.256Z Reads: 643

```
Does it come with a housing? Pricing? Availability? You are a little light on details ;)
```

---
## \#3 Posted by: lrdesigns Posted at: 2018-06-07T06:40:30.368Z Reads: 637

```
I like the compact size. Will it be made in Korea?
```

---
## \#4 Posted by: willumpie82 Posted at: 2018-06-07T06:58:02.556Z Reads: 634

```
looks really nice and clean, do you plan to open-source the design?
```

---
## \#5 Posted by: secupol Posted at: 2018-06-07T06:58:27.187Z Reads: 628

```
The housing has been developed but not mass-produced yet.
It is difficult to disclose price information here.
PCB size is 40mm x 80mm, motor connection is 4mm banana connector, power cable uses XT90 connector.
![sesc-case|690x388](upload://5pXPg9py49ONJaRwLhQWv3BKFjE.jpg)
```

---
## \#6 Posted by: secupol Posted at: 2018-06-07T06:59:46.301Z Reads: 607

```
PCB size is 40x80mm.
It was made in Korea.
```

---
## \#7 Posted by: secupol Posted at: 2018-06-07T07:01:08.034Z Reads: 600

```
Unfortunately, the data is hard to open.
```

---
## \#8 Posted by: Acido Posted at: 2018-06-07T07:42:17.915Z Reads: 589

```
You should produce few of them and stress test the shit out of them!

They look really nice and compact btw, the specs are the same?

Keep up with the nice work!
```

---
## \#9 Posted by: Maxid Posted at: 2018-06-07T07:47:50.008Z Reads: 583

```
Well without a ballpark number we have no idea if it is worth a shot. Are you aiming for a low price <100$ or a high price comparable to a "real" VESC6?
```

---
## \#10 Posted by: Hummie Posted at: 2018-06-07T07:49:49.279Z Reads: 579

```
why is it difficult to disclose price information here?  can we get it now without the box!  since it is trouble saying how much it costs..how much would you guess something like this would cost?
```

---
## \#11 Posted by: secupol Posted at: 2018-06-07T08:11:04.111Z Reads: 572

```
I'm fully aware of that.
So we did 12 cell buffered voltage, 52 volt input voltage, 10 amps continuous.
Some hardware specifications are not available.
For example, there are no external SPI and RF signal chips.
The only external interfaces have PPM signal, CAN communication, and UART communication.
UART works with I2C depending on the settings
```

---
## \#12 Posted by: secupol Posted at: 2018-06-07T08:14:10.922Z Reads: 551

```
Maybe 70 to 80 percent of that?
```

---
## \#13 Posted by: Acido Posted at: 2018-06-07T08:14:40.225Z Reads: 540

```
10amp continious will not be enaugh for e skates
```

---
## \#14 Posted by: secupol Posted at: 2018-06-07T08:19:10.149Z Reads: 546

```
I know about it.
We could only do so much testing because of the specifications of the power supply we had.
So we're going to do a higher constant current test.
```

---
## \#15 Posted by: secupol Posted at: 2018-06-07T08:20:35.065Z Reads: 540

```
It will cost 70 to 80 % 0f the VESC6.
```

---
## \#16 Posted by: AreaKruzer Posted at: 2018-06-07T08:21:17.671Z Reads: 542

```
70 to 80% MORE than VESC6 or 70 to 80% OF VESC6?
```

---
## \#17 Posted by: Maxid Posted at: 2018-06-07T08:22:08.376Z Reads: 548

```
80% of a real VESC6? :flushed: good luck with that. Including shipping from Korea and taxes I'd rather get a Focbox or the new controller by @esk8
```

---
## \#18 Posted by: Sebike Posted at: 2018-06-07T08:22:39.944Z Reads: 544

```
Around 300 usd..!? Ouch.
```

---
## \#19 Posted by: secupol Posted at: 2018-06-07T08:23:35.452Z Reads: 547

```
I made a mistake because I am not familiar with English.
70 to 80% of the VESC6
```

---
## \#20 Posted by: DeathCookies Posted at: 2018-06-07T08:25:44.132Z Reads: 551

```
Lets summarize
- you get a a vesc 6 derivative with much less functionality for nearly the same Price?
```

---
## \#21 Posted by: AreaKruzer Posted at: 2018-06-07T08:26:31.505Z Reads: 534

```
that is around USD240 to 250 per piece. At this price, a lot of members will hardly consider.

즉, 조각 당 USD240 ~ 250 정도입니다. 이 가격에서는 많은 회원들이 거의 고려하지 않을 것입니다.
```

---
## \#22 Posted by: Acido Posted at: 2018-06-07T08:33:38.608Z Reads: 530

```
Yeah... Thats not going to sell dude
Steewis vesc6 derivate costed 80$ and sold for less than 150$ if i remember well
Lower your profit margains or its not going to sell
```

---
## \#23 Posted by: secupol Posted at: 2018-06-07T08:34:07.690Z Reads: 526

```
I have a question.
Why would you suggest that a product derived should not be of that price?
Considering the component costs alone, only about $ 10 worth of parts were not used.
```

---
## \#24 Posted by: DeathCookies Posted at: 2018-06-07T08:35:53.015Z Reads: 517

```
[quote="DeathCookies, post:20, topic:58106"]
you get a a vesc 6 derivative with much less functionality for nearly the same Price?
[/quote]
I think that says all.

Your esc can only handle 10A continous but we Need about 30A or more! we will gain a Little bit of space in the enclosure to not run our Motors at their specs? seems like wasting.....
```

---
## \#25 Posted by: AreaKruzer Posted at: 2018-06-07T08:36:03.088Z Reads: 501

```
The reason many people looking for VESC6 is mostly for the stability and reliability of using FOC mode.

FOCBox now is able to run FOC mode with very much success and is half of the price. I believe many members are willing to buy 2 FOXBox than 1 of your SESC.
```

---
## \#26 Posted by: Acido Posted at: 2018-06-07T08:36:48.212Z Reads: 495

```
For 250$ i would expect it 150A cont lol or atleast a dual 50a esc like the new focbox
```

---
## \#27 Posted by: Kug3lis Posted at: 2018-06-07T08:38:07.529Z Reads: 496

```
Hey, you know that you have to release schematic if you modify it? Also the real part price of vesc6 is like under 100£
```

---
## \#28 Posted by: secupol Posted at: 2018-06-07T08:50:36.148Z Reads: 497

```
By the way,
Actual manufacturing costs are much higher than you think
It's just for the component cost.
```

---
## \#29 Posted by: secupol Posted at: 2018-06-07T08:51:28.967Z Reads: 489

```
You may be right.
I admit it.
```

---
## \#30 Posted by: secupol Posted at: 2018-06-07T08:53:01.065Z Reads: 482

```
Buy it if you want it.
I'm looking forward to it, too.
```

---
## \#31 Posted by: secupol Posted at: 2018-06-07T09:00:38.802Z Reads: 478

```
This means that the power supply in the video only outputs up to 10 amps of the motor current.
```

---
## \#32 Posted by: TarzanHBK Posted at: 2018-06-07T09:03:59.495Z Reads: 474

```
would be nice to get a video with high current and life data of the vesc, to see when it starts thermal throttling
```

---
## \#33 Posted by: secupol Posted at: 2018-06-07T09:07:05.112Z Reads: 472

```
Yes, I am planning the test.
```

---
## \#34 Posted by: secupol Posted at: 2018-06-07T09:16:03.851Z Reads: 470

```
Tell me where those rules are.
```

---
## \#35 Posted by: sk8l8r Posted at: 2018-06-07T09:39:30.721Z Reads: 470

```
its the cc licence 

"Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)" https://creativecommons.org/licenses/by-sa/4.0/

"ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original."
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-06-07T10:31:29.528Z Reads: 470

```
Do you even research the stuff you cloning? Like you know it's covered under GPL which requires to publish the changes to modified schematic
```

---
## \#37 Posted by: Kug3lis Posted at: 2018-06-07T10:34:54.725Z Reads: 468

```
What are you talking about, @stewii sells whole esc with case for less than you want also its not hand soldered...
```

---
## \#38 Posted by: Cobber Posted at: 2018-06-07T12:02:24.854Z Reads: 463

```
The OP has no choice but to open source the design, that is integral to the open source GPL, it is a condition of using Vedders base design. Other wise we will have frank in here raising the roof :fire:
```

---
## \#39 Posted by: Acido Posted at: 2018-06-07T12:30:34.518Z Reads: 457

```
Btw the first one he soldered by hand
```

---
## \#40 Posted by: banjaxxed Posted at: 2018-06-07T12:31:00.149Z Reads: 463

```
If you're only becoming aware of CC 'rules' now perhaps they do not apply to what you're doing...or so it would appear. Open-source is not really about what you can pirate to maximise commerical profit

But more importantly the price you've advertised is not going to happen, and especially not for a clone which utilises cheaper components than a true vesc6 derivative.

And as you've been informed, there are other vendors offering a real vesc6 clone populated PCB with same vesc6 BOM including an aluminium housing for about €150. Perhaps ebay is the place for this kind of naivety.

Who knows if future vesc tool F/W will even support something substantiually different like this.

Now sit in the corner with Flipsky, we want to have a talk with you after class
```

---
## \#41 Posted by: Acido Posted at: 2018-06-07T12:32:25.495Z Reads: 433

```
The first ones were
```

---
## \#42 Posted by: Kug3lis Posted at: 2018-06-07T12:37:45.825Z Reads: 435

```
Yep, I know I am just talking about the latest ones as price is till lower than he asked one :)
```

---
## \#43 Posted by: secupol Posted at: 2018-06-07T13:01:59.668Z Reads: 455

```
Attached is a schematics.
![SESC_V1_2|690x487](upload://eivnow3Qd0FdYUtPXZHXANoBP88.jpg)![SESC_V1_1|690x487](upload://9TpvXJIocne3pJzhCjlnMRzihR6.jpg)![SESC_V1_3|690x487](upload://mpjTpxrMOfmZb4CL6cCgKJTP68G.jpg)
```

---
## \#44 Posted by: secupol Posted at: 2018-06-07T13:10:15.035Z Reads: 423

```
I am not familiar with English.
So there seems to have been a misunderstanding.
The disclosure is made public.
But don't make me an unreasonable request.
```

---
## \#45 Posted by: Cobber Posted at: 2018-06-07T13:14:40.261Z Reads: 419

```
I'm releasing the _frank_ :octopus:
```

---
## \#46 Posted by: mmaner Posted at: 2018-06-07T13:16:54.370Z Reads: 424

```
[quote="Cobber, post:45, topic:58106"]
I’m releasing the *frank* :octopus:
[/quote]

Oh lord, now we'll never get him back in the corner :slight_smile:
```

---
## \#47 Posted by: trampa Posted at: 2018-06-07T13:19:15.309Z Reads: 425

```
The idea behind only releasing the schematics was pushing more innovation and make more different hardware hit the market. So if someone wants to design a motor controller he has a starting point and can make sure that the device will be VESC-compatible. The TM-policies allow vendors to point that out and use the VESC-Brand to describe the compatibility. 
We all know that hardware manufacturers don't like to publish their designs. The design is the basis for making business and giving it away would put small manufacturers in a situation where they potentially get striped out by bigger players, having more leverage in the market and more funds to make bigger batches. 
Open Source and hardware does only exist when you have a proper patent, and even then it is a difficult legal situation. So Benjamin does not give to much about the hardware. Compared to the software it's very little work to design a new controller.
```

---
## \#48 Posted by: Pedrodemio Posted at: 2018-06-07T13:28:41.072Z Reads: 415

```
I really liked this.

Even if the current is way lower than a VESC 6, it’s perfectly for a 4 wheel drive with smaller motors or low power hub motors
Currently you waste too much space on 4 esc’s

If the support something like 40A max it still would have a place when using smaller motors in dual drive

One suggestion I make is to make it available without the housing for a little bit lower cost, this way you can make the ultimate compact board designing a custom heatsink
```

---
## \#49 Posted by: secupol Posted at: 2018-06-07T13:36:31.172Z Reads: 415

```
It will probably be equal to the maximum current of vesc6.
However, the power supply used for the test was limited to 10A current, so the test was not conducted any further.
```

---
## \#50 Posted by: Kug3lis Posted at: 2018-06-07T13:45:31.695Z Reads: 405

```
Just to be clear it uses same mosfets as VESC6/ESCape/ESCALDE just in Automation standard so it will handle currents the same.

P.S. This will require at least 1mF capacitors at the power input.
```

---
## \#51 Posted by: secupol Posted at: 2018-06-07T13:56:23.633Z Reads: 404

```
Do not just judge by the capacitance of the capacitor.
I used a different kind of capacitor here.
Conductive Polymer
Aluminum Solid Electrolytic Capacitors.
This capacitor has a much smaller ESR and a much higher ripple current than ordinary aluminum capacitors.
So I was able to reduce the board size.
On the other hand, costs increased.
```

---
## \#52 Posted by: Kug3lis Posted at: 2018-06-07T14:16:54.194Z Reads: 399

```
its not the capacitors type which is important but capacitance itself, on high frequency switching those caps work as battery banks to provide surge of current. 0.3mF will not even compare to 1.4mF.
```

---
## \#53 Posted by: willumpie82 Posted at: 2018-06-07T14:17:17.834Z Reads: 392

```
not entirely right, PCB layout and copper thickness is an important factor, you don't want you pcb to act as a fuse.
```

---
## \#54 Posted by: Kug3lis Posted at: 2018-06-07T14:19:33.507Z Reads: 384

```
Thats another topic, I was talking about mosfets ;)
```

---
## \#55 Posted by: secupol Posted at: 2018-06-07T14:40:06.939Z Reads: 386

```
Polymer types and general electrolytic capacitors have better characteristics in the same switching circuit despite the low capacitance of the polymer type.
Please find a comparison between the two.
```

---
## \#56 Posted by: Kug3lis Posted at: 2018-06-07T14:45:52.253Z Reads: 386

```
Oh boy, how long do you work in electronics industry? Because I am not going to start explaining basics to person who "designed" vesc6 board...

EDIT: As there are people with no electronics background here I will explain: The capacitors work as intermediate current surge storage AKA battery which can deliver surge of current instantly because of low ESR. (As low resistance current will flow faster from capacitors than from battery through the leads) The bigger capacity the better performance you get out of it. It doesn't matter if you use best technology capacitors if they capacitance is low there is no energy to provide out of them. Snake oil will not provide more energy from same capacity :D
```

---
## \#57 Posted by: banjaxxed Posted at: 2018-06-07T14:52:46.990Z Reads: 395

```
Excellent Smithers
![frank|666x500](upload://bKhki3Hf58qqSXQeL0bvnk8PTbZ.png)
```

---
## \#58 Posted by: secupol Posted at: 2018-06-07T14:55:19.484Z Reads: 387

```
About 20 years..
Do you know what a capacitor for this purpose is called? If you are going to talk about a technical problem, please give a clear rationale.
```

---
## \#59 Posted by: Kug3lis Posted at: 2018-06-07T14:58:28.460Z Reads: 389

```
https://media.giphy.com/media/3owypkSIpM8xw6p7W0/giphy.gif
```

---
## \#60 Posted by: secupol Posted at: 2018-06-07T15:05:34.294Z Reads: 400

```
pls, read this doc
http://www.rubycon.co.jp/en/products/topics/t005.html

and see..
![a|500x326](upload://efAnAZDGQuJCPtfK2SInxuPlyEO.jpg)
![GBTcap_7|550x375](upload://aHQM60lN6pXkJIN0D9bHmsvoP9V.jpg)
```

---
## \#61 Posted by: Minim Posted at: 2018-06-07T15:07:38.831Z Reads: 381

```
The input caps can’t take off the “surge”. Isn’t it there mainly to take up voltage spikes that come when mosfet power off?
```

---
## \#62 Posted by: secupol Posted at: 2018-06-07T15:34:31.367Z Reads: 382

```
Please read the link above.
I can not explain it to you because I'm poor at using English.
```

---
## \#63 Posted by: Fiori Posted at: 2018-06-07T15:56:55.522Z Reads: 377

```
Can we please hold off from flaming this guy until we get more info? I am feeling like there is a language barrier here causing some confusion and unwarranted flaming. 

Nothing wrong with having a development post. This isn't strictly a marketplace, so he doesn't even have to post about prices yet.. It wasn't even posted in the marketplace section. 

I personally want to watch this, and other products being developed without the person being flamed for reasons that have more to do with sale than development.
```

---
## \#64 Posted by: Jc06505n Posted at: 2018-06-07T15:59:43.233Z Reads: 366

```
Agreed. No reason why anyone should come on the forum with whatever and be flamed
```

---
## \#65 Posted by: Donson Posted at: 2018-06-07T16:00:23.992Z Reads: 366

```
yes dont flaming this dude
```

---
## \#66 Posted by: Kug3lis Posted at: 2018-06-07T16:03:06.562Z Reads: 360

```
Just to make sure everybody understand I am not flaming, just telling him that he needs bigger caps not those caps used in motherboards as super duper ultra caps selling point. As currents in vesc reaches up to 200A and etc.. I believe trampa VESC6 would already used some duper caps as they have budget for it but I don't think they are any good for our application there power is over 3kW ;)
```

---
## \#67 Posted by: trampa Posted at: 2018-06-07T17:09:10.237Z Reads: 359

```
Benjamin's youtube channel will provide you guys some answers. He has a video about caps up.
```

---
## \#68 Posted by: secupol Posted at: 2018-06-07T18:09:03.302Z Reads: 369

```
If the motor current  is 165A, the current sensing amplifier is saturated.
Therefore, it can not reach 200A.
Realistically, VESC6 can not exceed 130A

Additional explanation
Amp output is 3.3V-1.65 or 0V-1.65(here 1.65V is ref voltage)
Therefore, taking an absolute value  1.65V
The amplification factor is 20
R is 0.0005
Ohm's Law is I=V/R
Imax = 1.65/0.0005/20 = 165A
Because of offset
Imax = 1.35/0.0005/20 = 135A
```

---
## \#69 Posted by: Deckoz Posted at: 2018-06-07T18:18:07.189Z Reads: 371

```
[quote="secupol, post:11, topic:58106"]
The only external interfaces have PPM signal, CAN communication, and UART communication.
UART works with I2C depending on the settings
[/quote]

first mistake, no sensor port, ya lost half your potential right there.

Edit: I see the pads on the bottom of the PCB, not sure why this wasn't a header instead of pads


Also back to the open source stuff, The Schematic must be open sourced following GPL. The gerbers you can keep to yourself.
```

---
## \#70 Posted by: SORRENTINO Posted at: 2018-06-07T18:21:56.278Z Reads: 357

```
@Kug3lis Hurry up already and release your DRVless esc :slight_smile:
```

---
## \#71 Posted by: secupol Posted at: 2018-06-07T18:26:00.446Z Reads: 360

```
In fact, when used in FoC mode, there is no need for sensor connection.
So I left points only in case someone was using it.
```

---
## \#72 Posted by: Deckoz Posted at: 2018-06-07T18:28:40.130Z Reads: 357

```
[quote="secupol, post:71, topic:58106"]
In fact, when used in FoC mode, there is no need for sensor connection.
[/quote]

We see very differently. There is a difference between sensored FOC and unsensored FOC. 

There's a good majority of people like myself that won't run boards without sensors, becuase there is a performance difference. FOC isn't a solve all...but atleast you have left the pads available
```

---
## \#73 Posted by: Kug3lis Posted at: 2018-06-07T19:04:14.341Z Reads: 349

```
I am out of this topic the guys really has like 0 knowledge about VESC :D or ESC in total :)

@secupol ADC doenst run constantly there is delay in between current readings ;) At those brakes you can even consume 500A if motor wants as you have direct connection to battery through open mosfet ;)
```

---
## \#74 Posted by: secupol Posted at: 2018-06-07T19:29:45.464Z Reads: 348

```
Your proof is groundless.
Can you prove it with a formula?
 
So if the current flows, everything will melt.

Additional explanation
Let's see what happens when 500A flows, whether it's a break or not.
1. The shunt resistor of the VESC6 is directly connected to the motor.
Therefore, the rated power of the shunt resistor is obtained as follows.
P = VxI = I ^ 2xR, 500A depending on your horse, P = 500x500x0.0005 = 125W
The rated power of the shunt resistor used in the VESC6 can not exceed 10W.

The maximum current that can flow through a shunt resistor with a rated power of 10W is:
Imax = √ (10W / R) = √ (10 / 0.0005) = 141A

2. If the motor current is 500A, the battery current is approximately. Below
Ibat = Imotor / √ 3= 500 / 1.732 = 288A
How many of them should be made in parallel to make this possible?
```

---
## \#75 Posted by: secupol Posted at: 2018-06-08T03:49:24.106Z Reads: 346

```
The main design directions of SESC are as follows.
1. Add a TVS diode to prevent the high voltage from the motor causing all breakdowns.
2. Using a new gate driver to reduce PCB size and using a type of Aluminum Organic Polymer capacitor for a link capacitor.

If you want to know the difference between ordinary aluminum capacitors and aluminum organic polymer capacitors or how they differ in performance, please refer to the link below.

http://www.rubycon.co.jp/en/products/topics/t005.html

![Comparison%20of%20VESCs|690x428](upload://2xDTM7C8aGOZ29NM8FG7U2OVcfZ.jpg)
If there is an error in the above comparison, please let us know.
```

---
## \#76 Posted by: Blasto Posted at: 2018-06-08T04:09:57.844Z Reads: 346

```
![image|690x426](upload://dwFjrKszbuhgH5NV634SCJuO6vU.jpg)

few corrections.

I like your layout :+1:
```

---
## \#77 Posted by: secupol Posted at: 2018-06-08T04:22:16.097Z Reads: 333

```
I know that used a TVS diode on the input side.
However, it does not generate a high voltage that is actually problematic at the input side.
Most of the problems are caused by the motor side.
So there was a problem with DRV8302 in VESC4.
But I do not know if the DRV8301 of VESC6 is causing any problems.
```

---
## \#78 Posted by: Naysh Posted at: 2018-06-08T04:37:47.477Z Reads: 331

```
What does @professor_shartsis say about this? He's good with formulas, got all kinds for esk8 calcs.
```

---
## \#79 Posted by: Blasto Posted at: 2018-06-08T04:41:26.416Z Reads: 336

```
Well, there goes the thread
```

---
## \#80 Posted by: chuttney1 Posted at: 2018-06-08T07:53:24.069Z Reads: 342

```
And from this I see this version uses a hardware implementation instead of SPI for the DRV8323.
```

---
## \#81 Posted by: secupol Posted at: 2018-06-19T09:17:47.510Z Reads: 338

```
SESC Test
Duty : 95%
VESC Limit : 60,000ERPM
Result : About 58,000ERPM

![20180618_130227|690x388](upload://fYzFSxcA0TV1Z79AiLZ3KVSuFt9.jpg)



https://youtu.be/mTBzYNN_H3s
```

---
## \#82 Posted by: Maxid Posted at: 2018-06-19T09:44:55.558Z Reads: 330

```
But VESC 6 only has a limit at 150.000 AFAIK :thinking:

The 60.000 limit was from the 4.12 era. I like the small size though. looks very compact
```

---
## \#83 Posted by: secupol Posted at: 2018-06-19T09:55:31.867Z Reads: 332

```
How can I give more than 60,000ERPM input?
It is always limited 60,000ERPM in VESC tool
```

---
## \#84 Posted by: banjaxxed Posted at: 2018-06-19T10:04:34.289Z Reads: 335

```
You need to flash with non-default no H/W limit F/W afaik
![image|690x197](upload://10owW4DORKLHyrnj9q0qApNxaIU.png)
```

---
## \#85 Posted by: secupol Posted at: 2018-06-19T10:09:53.469Z Reads: 329

```
Thank you.
First, I need to fix the firmware.
Because the hardware is different.
```

---
## \#86 Posted by: secupol Posted at: 2018-06-20T05:27:00.793Z Reads: 321

```
It was flashed to no hw limit fw binary.
but it is still limted to 60000erpm..
maybe it's problem of VESC tool app
```

---
## \#87 Posted by: Blasto Posted at: 2018-06-20T05:42:04.803Z Reads: 318

```
Run in foc, the fw limits will not apply. Other limit could be from your motor, you need a high kv high pole count motor.
```

---
## \#88 Posted by: secupol Posted at: 2018-06-20T05:45:24.277Z Reads: 314

```
It's running in foc and motor have 280kv, 14pole
It's enough
```

---
## \#89 Posted by: Blasto Posted at: 2018-06-20T05:51:40.455Z Reads: 318

```
Power supply voltage 30-36V?
```

---
## \#90 Posted by: secupol Posted at: 2018-06-20T05:53:27.205Z Reads: 316

```
36V/200W power supply
```

---
## \#91 Posted by: Blasto Posted at: 2018-06-20T06:02:16.693Z Reads: 322

```
With 50V input voltage, you will reach about 83Kerpm
```

---
## \#92 Posted by: secupol Posted at: 2018-06-21T03:42:55.133Z Reads: 326

```
Some pictures

1. size comparison
![size_comparison_sesc|690x388](upload://q2SS1PCl2lcqq9SXI2Dvlbqlaek.jpg)

2. back view
![back_sesc|690x388](upload://dbNAoqzXQ0Dh6t1gLh9gSnqztlj.jpg)

3. left view
![left_sesc|690x388](upload://beDF9IpSPiOZ9Ko00Adb7ekNKyl.jpg)

4. right view
![right_side_sesc|690x388](upload://mWir0yJKq3hthlmZtvsnnJcxdCr.jpg)

Made of full metal (aluminum) for good heat dissipation.

The test used VESC Tool to check the change of the FET temperature of the transmission when the motor current was 30A and to check whether the current control was performed when the temperature was increased to the temperature limit. However, too much heat was generated from the motor cable of motor side, I had an interruption.
It may need to test the transmission before it can be used in the field.

For reference, if you give foc_openloop 30 50 command in VESC Terminal, motor current 30A, ERPM will be returned to 50.

https://youtu.be/FBzBDKJyHDM
```

---
## \#93 Posted by: secupol Posted at: 2018-06-21T07:18:05.257Z Reads: 324

```
I try to test with 49V input.
72Kerpm.
![720000erpm|690x377](upload://bkX8MLt5x4fs6U4WozUYwW4UzCv.jpg)
```

---
## \#94 Posted by: secupol Posted at: 2018-06-21T07:40:01.585Z Reads: 318

```
What is the calculation formula?
```

---
## \#95 Posted by: bevilacqua Posted at: 2018-06-21T08:15:41.692Z Reads: 319

```
http://calc.esk8.it/ easy way
```

---
## \#96 Posted by: secupol Posted at: 2018-06-21T08:41:52.536Z Reads: 318

```
Why does it want to calculate 7 poles without using actual poles?
My motor have 14 poles.
But the test results are close to what you told me.
```

---
## \#97 Posted by: bevilacqua Posted at: 2018-06-21T08:49:39.082Z Reads: 319

```
7 Pole pairs= 14 poles. Standard pole count for eskate motors
```

---
## \#98 Posted by: TarzanHBK Posted at: 2018-06-21T08:51:49.667Z Reads: 319

```
Kv x Volt x polepairs = ERPM
```

---
## \#99 Posted by: secupol Posted at: 2018-06-26T02:03:54.961Z Reads: 327

```
The performance verification of the 36V / 200W power supply used to verify the performance of the VESC 6 clone SESC
Because the power and voltage is insufficient, 48V / 600W has received one seat.
The voltage was adjusted slightly to match the 95% of the 12S battery to 49V.
The motor is BRD5060-280KV, the maximum current is 52A.

First is the maximum ERPM test.
ERPM limits can be set on the VESC Tool. Currently, the time limit of 100000 is the maximum value
Since it is 80%, it should reach 80000ERPM.
Prior to that, depending on the motor performance, 280KV x 49V (input voltage) x 7 (motor pole pair) = 96040 is a physical theory limit.

The test result is about 79000 ERPM which is slightly less than the limit of 80000.
We are close to 98% so the result about the rotation speed is satisfactory.

![limit_erpm|640x480](upload://sAn0FaMjyunDTHWxdIpU89n5ZfN.jpg)

https://youtu.be/VKdl0w4V0VE
[erpm test]


Next is the maximum motor current test.
It is 52A in the motor specification, but when it is tested for about 20 seconds with 30A in the previous test,
Considering the slight smell of burning, we tested only 50A for 10 seconds.
The temperature rise of the FET in the transmission suddenly rises.
If you watch several vesc monitor videos, you will not be driving more than 10 seconds for more than 50A
Assuming that the transmission is driving the motor with sufficient power, it is assumed that the motor is driven.
For reference, sometimes video of 100A or more is not a single transmission, but two transmission motor currents.

https://youtu.be/f-HOA9NcoHk
```

---
## \#100 Posted by: secupol Posted at: 2018-06-28T10:12:02.643Z Reads: 315

```
![03|690x386](upload://mgvZcSivOowe5rGcOz7VO1x6tRh.jpg)
```

---
## \#101 Posted by: PXSS Posted at: 2018-06-28T11:47:20.578Z Reads: 308

```
I have a 2.5kW power supply. I am willing to beta test for you if you offer the esc at cost.
```

---
## \#102 Posted by: briman05 Posted at: 2018-06-28T15:04:06.281Z Reads: 307

```
If you wanted to run sensored on this how would you do it as I dont see a connector port of solder joints to support it
```

---
## \#103 Posted by: secupol Posted at: 2018-06-28T15:39:27.157Z Reads: 304

```
There are pads on the underside of the pcb board.

Look at the table and the bottom pic of pcb above.
```

---
## \#104 Posted by: secupol Posted at: 2018-06-28T15:41:06.704Z Reads: 308

```
Could you tell me about the test method and procedure?
```

---
## \#105 Posted by: secupol Posted at: 2018-07-01T06:45:05.785Z Reads: 298

```
![sesc_v1_spec|690x388](upload://tfWiReYKQlknkuyGmDQkcTFQ1MJ.jpg)
```

---
## \#106 Posted by: rpasichnyk Posted at: 2018-07-01T10:57:22.571Z Reads: 301

```
Please route 3.3V to the UART port :cry: Metr Pro bluetooth module needs that!
```

---
## \#107 Posted by: secupol Posted at: 2018-07-01T11:13:42.260Z Reads: 303

```
The user can easily change the output voltage to 3.3V.
You can select either 5V output or 3.3V output with 0 ohm resistor. Soldering can be done without a 0 ohm resistor.
```

---
## \#108 Posted by: TarzanHBK Posted at: 2018-07-03T07:57:25.206Z Reads: 292

```
Whats the total height in the enclosure?
```

---
## \#109 Posted by: secupol Posted at: 2018-07-03T08:22:02.442Z Reads: 297

```
![sesc_v1_heigt|690x388](upload://liMWnmhtdbFqMaJijcxTuEyJg4w.jpg)
```

---
## \#110 Posted by: willumpie82 Posted at: 2018-07-20T06:23:52.038Z Reads: 290

```
@secupol I still like your design, but how is that negative battery lead secured? if I look at the pictures it might be rubbing the micro USB port which has sharp-ish edges on the back, with our bumpy esk8's that will lead to the magic smoke to escape
```

---
## \#111 Posted by: secupol Posted at: 2018-07-20T06:48:02.649Z Reads: 285

```
I do not understand what you're talking about.
```

---
## \#112 Posted by: b264 Posted at: 2018-07-20T06:59:21.562Z Reads: 284

```
The microUSB jack that is soldered to the PCB is right next to the negative battery lead.  Under heave vibration it will fray through the negative lead insulation.
```

---
## \#113 Posted by: secupol Posted at: 2018-07-20T07:08:35.890Z Reads: 273

```
I do not understand why that is the problem.
Why is it that the insulated cable closes to the usb connector?
```

---
## \#114 Posted by: telnoi Posted at: 2018-07-20T07:16:42.470Z Reads: 271

```
Grab that black cable after you have the PCB installed in it's case and pull on it about 50 times. See if there are any marks on the insulation of the cable.

On my build, those cables are constantly moving around.
```

---
## \#115 Posted by: secupol Posted at: 2018-07-20T07:22:12.705Z Reads: 265

```
The case secures the cable.
And if you have any problematic photos, please show them.
```

---
## \#116 Posted by: b264 Posted at: 2018-07-20T07:23:52.847Z Reads: 265

```
@secupol Extreme vibration is something many folks here are skilled at dealing with, you should listen to their suggestions.  That looks like a place of failure and they're pointing that out to you.
```

---
## \#117 Posted by: secupol Posted at: 2018-07-20T07:28:27.060Z Reads: 271

```
I am sorry, but I can judge whether it is contents to listen or not. It is only speculation that I judged the picture, not the real one.
```

---
## \#118 Posted by: telnoi Posted at: 2018-07-20T07:28:33.938Z Reads: 273

```
That cable is not ridged. If there is a bit of slack, it could still move around upon sudden ''impacts'', e.g. jumping/sidewalks/potholes etc. Hold the cable in between your fingers and move it on one end. It will move on the other end too.

A bit of adhesive foam would already resolve the issue.
```

---
## \#119 Posted by: secupol Posted at: 2018-07-20T07:31:11.408Z Reads: 271

```
When the case is tightened, the cable is firmly fixed.
It looks like you are making an unreasonable pincushion when you look at the picture.
```

---
## \#120 Posted by: telnoi Posted at: 2018-07-20T07:33:53.872Z Reads: 273

```
Ok, I tried ;)
It's your product. If I were to purchase it, I'd still pull it apart knowing this and add a bit of sub 1 dollar security.
```

---
## \#121 Posted by: secupol Posted at: 2018-07-20T07:36:47.073Z Reads: 281

```
![20180720_163307|281x500](upload://7499QIw52QZvlWGMJXc2DXu3923.jpg)
```

---
## \#122 Posted by: telnoi Posted at: 2018-07-20T07:39:47.790Z Reads: 280

```
Yes, I know. I'm already stressed seeing that it's metal on cable without grommets isolating both, or I did not see that properly.
```

---
## \#123 Posted by: willumpie82 Posted at: 2018-07-20T07:54:14.762Z Reads: 279

```
@secupol, of course not my intention to make any flames going your way but it is just some worry i get when i see the pictures, I assume you are aiming for a quality product, just trying to help you iron-out potential reliability issues.

Silicon wire is super convenient, heat resistant, flexible,... and in practice most silicon insulated wire is able to stand some abuse but it is really soft and can easily be scarred, 
imo the hard mount in the case with is no strain/stress relieve creates another issue of potential shorting to the case, try bending the cable sharp a few times at the entrance and check the insulation, a simple solution could be to add some heat shrink around wire where it touches and exits the case
```

---
## \#124 Posted by: Kug3lis Posted at: 2018-07-20T09:09:17.320Z Reads: 272

```
Lool, the wire will be damaged after 100km guaranteed tried that myself, guess why we have grommets in our cases...
```

---
## \#125 Posted by: lrdesigns Posted at: 2018-07-20T09:13:28.975Z Reads: 273

```
It's not just the large vibrations that will cause damage. Micro vibrations from road texture will wear through components like an electric sander. On my first build with vesc 4, the caps were resting on plastic enclosure, after like 100km the caps aluminum casing had worn all the way through, just from resting on PE plastic. My caps had holes in them! So now everything is hot glued down so it can't rub.
```

---
## \#126 Posted by: Kug3lis Posted at: 2018-07-20T10:02:57.163Z Reads: 268

```
But dont mind me magical capacitors will cure all problems :D
```

---
## \#127 Posted by: StarLoad Posted at: 2018-07-20T16:31:48.304Z Reads: 262

```
Do you have a esk8? In my view, you are calculations that have never experienced a esk8.
Hummmm, you are not calculating the fear of vibration at all!
```

---
## \#128 Posted by: b264 Posted at: 2018-07-20T16:35:01.120Z Reads: 269

```
82 micro-magical-farads  

82 μMF
```

---
## \#129 Posted by: briman05 Posted at: 2018-07-20T16:36:13.145Z Reads: 272

```
I'm not seeing how a person would run dual vesc or sensored on this
```

---
## \#130 Posted by: mccloed Posted at: 2018-07-20T18:20:57.110Z Reads: 268

```
Hmm...Looks to me like you cannot run PPM and UART(bluetooth module) at the same time. At least on a single set up. Am I missing something?
```

---
## \#131 Posted by: sayekim Posted at: 2018-07-20T23:43:03.437Z Reads: 260

```
Sure you can(bus).

ppm port is not the same as the uart port.
```

---
## \#132 Posted by: SpeedyGonzales Posted at: 2018-10-11T20:48:55.133Z Reads: 237

```
Your design is brilliant and I don't understand why some of the guys here're chewing on your ass.
It is obvious to me that you are a professional. I wish I had your knowledge. I just don't feel like learning a new skill, so I will stick with mechanical engineering. Good luck.
```

---
## \#133 Posted by: brenternet Posted at: 2018-10-11T21:23:05.540Z Reads: 247

```
The design is good, aside from issues (easily fixed) that heavily experienced members here have pointed out. Instead of rectifying or even acknowledging the very real issues this chap has decided to go on the full defensive.

The cost is also a big hindrance. There's just no reason to save $50 on this over a vesc 6.6 that will produce consistent results like a damn work horse.

Fix a few things and half the price and this will contend. As it stands its an expensive box of fire in waiting.
```

---
## \#134 Posted by: secupol Posted at: 2018-12-28T10:20:18.922Z Reads: 243

```
New!!
![1280x924_spin_a|690x498](upload://wieZPG1wWDsgLbqHTRJpXYZ3Cnn.jpeg) 

FOC_SPIN(Left) : InstaSpin-FOC
MOTION_SPIN(Right) : VESC 6 derivative



![1280x924_motion_spin_top|690x498](upload://hWnwpF8m37Ac3czhbLXYOajvarp.jpeg) 
![1280x924_motion_spin_bottom|690x498](upload://ytU8noSl7UPFxm2cdhQsUNWiFRx.jpeg) 
![1280x924_motion_spin_with_heatsink|690x498](upload://a4fDvRF3w7w7n5UTwEJgID8xDFh.jpeg)
```

---
## \#135 Posted by: mishrasubhransu Posted at: 2018-12-28T10:27:26.322Z Reads: 235

```
What do you mean by insta_spin and motion_spin?
```

---
## \#136 Posted by: secupol Posted at: 2018-12-28T10:53:19.529Z Reads: 232

```
FOC-SPIN and MOTION-SPIN is model name as it is called FOC-BOX.
FOC-SPIN has TI(Texas Instruments)'s InstaSpin-FOC firmware.
MOTION-SPIN has VESC 6's firmware.
```

---
## \#137 Posted by: TowerCrisis Posted at: 2018-12-28T12:16:55.950Z Reads: 235

```
Woah, you're running different firmware on these? That's very interesting.

What's your pricing on these? They look VERY compact.


I put this thread on my watch list.

EDIT: I re-read through this whole thread. Interesting details, I found the speed and current limits.
```

---
## \#138 Posted by: secupol Posted at: 2018-12-28T12:28:36.605Z Reads: 232

```
MOTION-SPIN is the same as the vesc 6 specification.
FOC-SPIN will be the same as the vesc 6 specification.
```

---
## \#139 Posted by: Sn4pz Posted at: 2018-12-28T12:31:03.667Z Reads: 231

```
Big claims 🤔🤔🤔

Have any videos or something?
```

---
## \#140 Posted by: Andy87 Posted at: 2018-12-28T12:33:36.040Z Reads: 230

```
what are the changes to the previous version you made?
what´s the latest information about the constant current they can handle?
The max ERPM is at 100 000 right?
Any updates on the price or it is still around 250-280$ ?
```

---
## \#141 Posted by: Andy87 Posted at: 2018-12-28T12:34:39.028Z Reads: 225

```
@Sn4pz maybe you want to scroll through the thread?
there are a lot of information and i think also some videos he already posted.
```

---
## \#142 Posted by: Sn4pz Posted at: 2018-12-28T12:36:20.094Z Reads: 229

```
I was talking about the new designs, but yeah I should :p
```

---
## \#143 Posted by: Andy87 Posted at: 2018-12-28T12:38:33.437Z Reads: 229

```
nu he honestly doesn´t clame anything with his last post besides that they can run with VESC6 fw. :sweat_smile:
```

---
## \#144 Posted by: secupol Posted at: 2018-12-29T02:28:06.094Z Reads: 230

```
Short video for test

https://youtu.be/OApYL--lMH8
```

---
## \#145 Posted by: evoheyax Posted at: 2018-12-29T02:47:01.965Z Reads: 231

```
Looks good. Cool to see others working on it. But no sensor port and $250 no thank you. I'll stick to the the focbox or another vesc 6 version.
```

---
## \#146 Posted by: briman05 Posted at: 2018-12-29T02:48:16.151Z Reads: 230

```
Yeah I was thinking the same thing why not have the sensor port and no can or ppm
```

---
## \#147 Posted by: evoheyax Posted at: 2018-12-29T02:51:26.710Z Reads: 225

```
There's CAN, I see a CAN H and CAN L listed in the photo from June 30th. As is the ppm, it's just not a standard ppm port.
```

---
## \#148 Posted by: JohnnyMeduse Posted at: 2018-12-29T02:53:36.948Z Reads: 225

```
[quote="secupol, post:136, topic:58106"]
it is called FOC-BOX.
[/quote]

wow your are gunning for originality here :kissing_heart:
```

---
## \#149 Posted by: DerelictRobot Posted at: 2018-12-29T03:25:17.482Z Reads: 226

```
I think language barrier is a factor here. He explained the difference in models above. 

Let's try to give him the benefit of the doubt here- we want to encourage work like this and he's been posting a lot of data to a pretty tough crowd.
```

---
## \#150 Posted by: secupol Posted at: 2018-12-29T03:28:31.625Z Reads: 234

```
![1280x924_motion_spin_top_index|690x498](upload://3ddeIMKAoPxDrioxHtJQSUhZDti.jpeg) 
① USB Port
② CAN Port
     - CAN-H
     - CAN-L
     - CAN-GND
③ APP Port
     - V+(5V)
     - UART-TX
     - UART-RX
     - PPM or ADC (Selected by VESC Tool)
     - GND
④ Sensor Port
     - V+(5V)
     - HALL-A
     - HALL-B
     - HALL-C
     - Motor-Temperature
     - GND
```

---
## \#151 Posted by: b264 Posted at: 2018-12-29T03:35:34.535Z Reads: 226

```
This is awesome!  Fantastic work :slight_smile:
```

---
## \#152 Posted by: DerelictRobot Posted at: 2018-12-29T04:58:17.443Z Reads: 229

```
I appreciate you taking the time to document your work on this project. I think it's worth noting that you've showed more openness and willingness to share your work & data than a lot of projects I've seen on here. I find it strange when people are so quick to try to enforce someone else's license/share-alike clause.

Can I ask if this is more of a personal exercise or are you looking to sell these? Any update on an estimated cost per unit?
```

---
## \#153 Posted by: briman05 Posted at: 2018-12-29T15:30:13.517Z Reads: 226

```
Is it generally the 5v then temp then hall 1,2,3 then ground.
```

---
## \#154 Posted by: banjaxxed Posted at: 2018-12-29T16:55:03.386Z Reads: 228

```
This is cool but I just don’t see it making its way to adoption against the unity or vesc6 derivatives like the ESCape.

Given the disappearance of the ESCape there is a place for this, but the expectation would be the same price as the ESCape otherwise don’t see any take up no matter how dandy it is, I like the form factor
Edit: Completly forgot about the Flipsky v6 clone, that is the target product that took over from the ESCape, I don’t have any as I wasn’t impressed with how they introduced themselves on the forum
```

---
## \#155 Posted by: secupol Posted at: 2018-12-30T09:33:48.948Z Reads: 228

```
![dc_link_capacitors|690x388](upload://nQ6IuQp23C0p0lEyQQnLWDIpxOs.jpeg)
The above picture shows the stability of the power applied to the FET drain when the motor is driven by using two different types of capacitors using MOTION-SPIN.
As you can see, it is stable when polymer capacitors are used, but if you use general film capacitors, you will see a lot of swinging when driving the motor.
Despite having 10 times the capacity.
```

---
## \#156 Posted by: sofu Posted at: 2018-12-30T09:41:35.301Z Reads: 225

```
You know It's funny you mentioned flipsky as the target product... I've been talking with a few eskate manufacturers who source their own vescs (Arcboards and Hoyt run 4.12 single and dual respectively, for example) and got a somewhat detailed picture of what's going on over in the Asian esc market... tl;dr it seems Flipsky sort of came in and steamrolled over every vesc supplier (not counting other escs) in the market with insanely low prices (for suppliers), even running a couple out of the vesc business. Now it's the mad dash to the bottom in terms of price and quality for the rest 😬

So I think the reason they're not really handling the consumer sales side that well is because it doesn't really matter to them. They make most of their profits on the b2b side as basically the only competitive supplier...

Anyways sorry for derailing your thread @secupol :P good luck with the sesc, what you've done so far is super nice! It would be awesome to see an esc out of Korea that performs really well 👍
```

---
## \#157 Posted by: b264 Posted at: 2018-12-30T10:00:54.614Z Reads: 226

```
Don't buy the marketing jive from the capacitor-sellers

Farads matter, and this is a high-current situation demanding large quantities of electrons and nothing else will do.

We're not talking about a simple power supply ripple filter here.  This has a straight-up square-wave load.
```

---
## \#158 Posted by: secupol Posted at: 2018-12-30T10:20:50.917Z Reads: 217

```
This is an experiment to check FET drain voltage stability using MOTION-SPIN esc with two different capacitors.
When the polymer capacitor is used, it can be seen that the power source is stable without loose.
```

---
## \#159 Posted by: b264 Posted at: 2018-12-30T10:25:11.970Z Reads: 220

```
But firstly, "farads" is a scientific measurement so if it was really just as good, it would be just as many farads.

But secondly and most importantly, folks around here like to push stuff past the safe zone, and even if you extended the safe zone, they would push beyond the new boundary, and cheaping-out on filter caps could let some high voltage inductor flyback into the circuit

People around here are all about running a circuit at 99% rated voltage LoLz
```

---
## \#160 Posted by: secupol Posted at: 2018-12-30T10:43:09.255Z Reads: 222

```
As you say, the Farad is a scientific measure and the capacity is the most important parameter to use here. However, in a wide range of frequencies, common capacitors do not provide adequate capacitive characteristics. Test directly with two capacitors.
```

---
## \#161 Posted by: b264 Posted at: 2018-12-30T10:52:38.061Z Reads: 223

```
I'm aware of that.  You can also put small and ultra-cheap capacitors in parallel with the large ones to alter the spectral characteristic as well, even tailoring it to your specific needs.
```

---
## \#162 Posted by: banjaxxed Posted at: 2018-12-30T12:00:37.030Z Reads: 223

```
That business approach did work of course, still there are people who prefer to spend with vendors who maintain standards from a business ethics and tease out quality in their product line rather then depending on marginal profits from pumping product.

This is why I decided to pick up a Unity(& some couch foxboxes) from Enertion instead. I’m pretty sure @onloop realizes he found himself a unicorn 🦄 with @Deodand
```

---
## \#163 Posted by: sofu Posted at: 2018-12-30T12:21:04.143Z Reads: 226

```
Yeah for sure, I'm 100% in on the unity as well. I run nothing but focboxes and unities except one odd dual escape. It's a good product!
```

---
## \#164 Posted by: JTAG Posted at: 2018-12-30T14:14:49.414Z Reads: 225

```
The latest new trend in the capacitor world shows that indeed Polymer based capacitors perform a lot better then the regular, I am working on a new controller as well (solar car application) and am seeing the similar things as @secupol on their performance and size. Please keep in mind that most of the time in motor controller world you don't pick the bulk capacitor because of its capacitance, but mainly because of its current rating in combination with the impedance across a frequency range. Polymer capacitors will outperform every other capacitor style (accept for ceramic) in many cases by at least a factor of 3. As secupol said, please look into polymer caps specs and maybe order one to do some measurements, you'll be surprised. 

Could we also please lower the tone of criticism? Or translate it a bit into a constructive one preferably based on facts and comparisons? 

Shouting a lot and shouting hard will not prove your opinion, it will just crowd the topic and drown the opinions of others who don't spend their full day on the forum shouting back :stuck_out_tongue:.

(Yes there is a drawback as well, so far the noticeable drawback of polymer caps is the higher leakage current, but that is mainly an issue for long life battery powered application, which esk8 is not xD )
```

---
## \#165 Posted by: Steven1 Posted at: 2018-12-30T14:42:43.979Z Reads: 216

```
Any idea when you will have an initial batch for sale?
```

---
## \#166 Posted by: AlexBE Posted at: 2018-12-31T00:56:37.392Z Reads: 217

```
The problem you have here is that the leads are WAY too long on the larger capacitor. The leads look to be at least 10mm long which hugely increases your lead inductance. Remember that these caps are supposed to be mounted through a PCB, meaning the lead length is only ~1mm.

Also, how are you measuring the voltage rail? What is the loop area of your scope probe ground? You really need to have a custom scope lead soldered to a test point on your board to make this measurement properly. If you don't , the huge switching current from the motor leads will be inductively coupled to the scope probe.
```

---
## \#167 Posted by: secupol Posted at: 2019-01-01T00:26:17.167Z Reads: 210

```
What is the value from 1mm and 10mm?
Did you actually experiment with the difference between 10mm and 1mm?There was little difference in my experience.I would be grateful if you could convince yourself that there are other differences.
```

---
## \#168 Posted by: AlexBE Posted at: 2019-01-02T01:53:33.689Z Reads: 208

```
It's easy to measure if you have an inductance meter. The value will be ~100nH difference by adding the 10mm of wire. The most significant effect of this will be ringing in the main voltage when switching. 

Also think about the resistance, how much current are you expecting these caps to take? Ideally the caps will take the fundamental frequency of the FETs PWM, so at 50A continuous and 50% duty, you are getting 100A in the cap. I would be interested to see how warm your thin cap wires get. Of course you haven't loaded your system yet which is another huge problem.
```

---
## \#169 Posted by: willumpie82 Posted at: 2019-01-03T10:19:12.568Z Reads: 194

```
About the capacitors, yes it is about farads, but also the ESR and the peak currents, thats why the "modern" capacitors perform better, but this is application dependant. I guess in a simple power supply application it does not matter so much, in a motor drive application it does.

e.g. the picture Secupol posted about the ripple at the caps. the electrolithic vs polymer, the polymer is much more capable of delivering peak energy
```

---
## \#170 Posted by: AlexBE Posted at: 2019-01-04T02:27:47.743Z Reads: 190

```
Some of us in this thread are doubting that measurement though. Sure, modern polymer capacitors are good but 220uF vs 2200uF is a big difference. My problems with the measurement
* The lead length on the 2200uF cap
* How was the scope probe connected? Can't use a ground clip for this.
* Load on the circuit. I don't believe the circuit has been loaded sufficiently. Need to run at 50% duty, large current.
* 1uS per division is showing us the gate edge. Actually I don't believe it's showing us the gate edge, its showing the inductively coupled edge->probe loop. The purpose of the bulk capacitors is to take the actual FET current, so you really want to look at a whole switching cycle.
```

---
## \#171 Posted by: b264 Posted at: 2019-01-04T02:41:08.403Z Reads: 192

```
It all smells like Marketing Jive to me personally and less like actual science.
```

---
## \#172 Posted by: AlexBE Posted at: 2019-01-04T05:15:28.786Z Reads: 190

```
I'm a little more charitable, I think OP is just making the incorrect measurement and also not measuring properly. I have run into a similar problem in quadcopter racing. Measuring voltage rails with a scope is incredibly difficult when you have 50+ amps being switched so fast.
```

---
## \#173 Posted by: b264 Posted at: 2019-01-04T05:57:26.478Z Reads: 192

```
I don't necessarily think it's OP that's doing it...

I think it all starts with the seller or stakeholder of the company that makes the new polymer capacitors.  It's 2019, everything is marketing and you have to sort the truth out yourself.

Generally, if it's less farads I am extremely skeptical.  Last person I heard the same spiel from was trying to sell dirt-cheap ESCs.

If it really worked better at storing charges then it would be more farads.  You can always add a dirt-cheap picofarad and nanofarad ceramic in parallel to handle the higher frequencies.
```

---
## \#174 Posted by: Minim Posted at: 2019-01-04T06:16:34.509Z Reads: 187

```
Why are we not using 1fahrad caps if capacity is the only thing that matters? From my own testing on big quadcopters I had much better result with many small low esr caps then with a similar big one. It’s more about the low esr part than the capacity itself. These caps are not big enough to take care of a voltage drop it’s to remove harmful spikes and for that it needs to be “quick”.
```

---
## \#175 Posted by: b264 Posted at: 2019-01-04T07:25:38.001Z Reads: 187

```
A bigger capacitor in parallel with a smaller capacitor is "quick".
```

---
## \#176 Posted by: AlexBE Posted at: 2019-01-04T07:26:54.681Z Reads: 190

```
ahh sorry, I misinterpreted you. Yes absolutely the specs of components are out of wack with reality (see mosfet ratings). I think we are identifying two separate problems, one with capacitor specs, one with the tests/conclusions made in this thread.
```

---
## \#177 Posted by: AlexBE Posted at: 2019-01-04T07:28:54.867Z Reads: 193

```
Nobody said capacity is the only things that matters. Everything matters.
* cost
* size
* availability
* temperature rating
* package
* capacitance
* power handling
* ESR
* etc.....

Your suggestion of 1F cap fails on cost, size, availability, package at least.
```

---
## \#178 Posted by: b264 Posted at: 2019-01-04T07:29:34.996Z Reads: 186

```
And no 1F cap is available at 60V unless it's super-huge and super-heavy
```

---
## \#179 Posted by: AlexBE Posted at: 2019-01-04T07:33:28.100Z Reads: 197

```
Also, even placing a bunch of 350F 2.7V super caps in series/parallel you have the huge problem of the inductance of the leads to those capacitors. The problem of gate edges and 30khz 100A switching is solved by a combination of low inductance ceramic caps very close to the fets combined with large (~2000uF) electrolytics (polymer if you like) as close as possible to the fets. Vedder did a good youtube video showing how to simulate this kind of thing.
```

---
## \#180 Posted by: willumpie82 Posted at: 2019-01-04T10:24:20.423Z Reads: 201

```
@secupol, I think your product looks great, as I read this thread, your results are being questioned, probably because you have no track record with proven information. Why not invite a few well respected people from this community for beta testing?
```

---
## \#181 Posted by: secupol Posted at: 2019-01-13T09:06:23.751Z Reads: 205

```
![Inkedvesc-tool_connection%20-%20motion-spin_LI|690x377](upload://sc8VOhGauj7QZH1nhvPemrvYjxY.jpeg) ![20190113_175745|690x388](upload://6FfJID0Pm163xE1xrg4ldnaNExa.jpeg) ![20190113_175804|690x388](upload://9Hg7vVK255K6oAZMtSWpCsqbGdI.jpeg)
```

---
## \#182 Posted by: JTAG Posted at: 2019-01-13T12:17:06.007Z Reads: 196

```
Looks really good and compact!

I see that you use three ground phase shunts, that mean that you have adopted the firmware to support them. Could you shine some light on this? Also do you notice any performance difference with the in phase shut measuring that the VESC6 is doing?
```

---
## \#183 Posted by: secupol Posted at: 2019-01-13T12:36:17.532Z Reads: 193

```
The firmware and hardware are almost identical to VESC 6. It's just a different gate driver for MOSFET.
```

---
## \#184 Posted by: mishrasubhransu Posted at: 2019-01-13T15:26:28.973Z Reads: 191

```
Which one are you using? And is it better in some sense?
```

---
## \#185 Posted by: b264 Posted at: 2019-01-13T22:53:33.179Z Reads: 185

```
What are the rated absolute maximum voltage limits for the gate driver?
```

---
## \#186 Posted by: secupol Posted at: 2019-01-13T23:42:51.102Z Reads: 187

```
It is used DRV8323RS made by TI.
```

---
## \#187 Posted by: secupol Posted at: 2019-01-13T23:43:50.442Z Reads: 188

```
Maximum voltage is 60V
```

---
## \#188 Posted by: b264 Posted at: 2019-01-14T07:04:44.707Z Reads: 195

```
So still 10S max reliable, 12S for skates that don't have to be mission-critical dependable, and 13S for daredevils
```

---
## \#189 Posted by: secupol Posted at: 2019-01-14T09:33:15.119Z Reads: 200

```
Single Housing(W x L x H) : 52 x 84 x 17 mm
Dual Housing(W x L x H) : 102 x 84 x 17 mm
PCB Size (W x L x H) : 46 x 70 x 1.2 mm

![single_bottom|690x388](upload://s3tTMGTlUlMIIwwVuFeatysUOsC.jpeg) 
![single_inner|690x388](upload://15ReI6Qx2ZPi6JV1x0D5udhZRgs.jpeg) 
![dual_inner|690x388](upload://ftntxqZPhev1aG8MmoOl4q2JU76.jpeg) 
![dual_top|690x388](upload://vwTlV3AH9X70uZR0JRC7pnXLeu8.jpeg) ![dual_bottom|690x388](upload://aDwe8jFshiRT7wPdHptvp1850Ii.jpeg)
```

---
## \#190 Posted by: briman05 Posted at: 2019-01-14T13:36:49.256Z Reads: 189

```
So this vesc6 will only do 10s?
```

---
## \#191 Posted by: Andy87 Posted at: 2019-01-14T14:03:22.071Z Reads: 192

```
[quote="secupol, post:187, topic:58106, full:true"]
Maximum voltage is 60V
[/quote]

The same like every other vesc 4 and 6 we have here at the moment
```

---
## \#192 Posted by: b264 Posted at: 2019-01-14T15:00:26.523Z Reads: 189

```
The [VESC 7](https://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26293.html) is 75V, the rest are all 60V but those are absolute maximum hardware ratings and you should never approach those.
```

---
## \#193 Posted by: Sn4pz Posted at: 2019-01-14T15:14:58.108Z Reads: 185

```
I assume you feel the same way about the Unity, would the 
[details="Breaking Resistor"]
RHEOSTATIC BRAKE module
SAMPLE PRICE $30

[![Rheostatic%20Brake|690x432](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/d/5d9a0100a07741e21f3d61aee52f276ecf6940c7.jpeg)
Rheostatic Brake.jpg889x557 26.3 KB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/d/5d9a0100a07741e21f3d61aee52f276ecf6940c7.jpeg)

Battery: &lt;=12s
Operation voltage: 57V
Startup time: 200ms
Max current: 5A
Function: when brake reverse voltage is higher than operation voltage, Rheostatic Brake starts working and reduces the reverse voltage to protect ESCs.
[/details]
 change how you feel about the Unitys reliability with hard breaking on 12s? Or do you see it as unnecessary
```

---
## \#194 Posted by: b264 Posted at: 2019-01-14T15:25:55.653Z Reads: 194

```
You should never run an inductive load above about 75% of rated hardware voltage-- and especially on a square wave PWM digital drive.

Using any breaking resistor is not recommended because broken resistors only add ballast weight.  A braking resistor system might help but I still wouldn't do it.  I doubt 200ms is fast enough because it's the inductive kickback millisecond spikes that are the problem.  It definitely doesn't hurt though... you could in theory soak up anything under 200ms with caps.

But there's no reason to reduce the reliability and add failure modes by edging that close to physical hardware limits with an inductive load fed by square waves.  Not when you can just run it at 10S and make a beast esk8 that blows away any commercial prebuilt on the market and is reliable.

The braking resistor is awesome if you live or work on top of a big hill.  Could be a lifesaver.
```

---
## \#195 Posted by: Sn4pz Posted at: 2019-01-14T15:29:26.060Z Reads: 189

```
Alright so I shouldnt even bother with 12s :thinking:

10s Here I come i guess :man_shrugging:
```

---
## \#196 Posted by: b264 Posted at: 2019-01-14T15:31:35.954Z Reads: 189

```
A lot of folks use 12S on these, but I can't agree with them.  For a "toy" maybe but for a "tool" 12S doesn't make sense with the 60V gate drivers like VESC 4-6

Prepare for 37 folks to say "I did it, and it's fine" and remember the whole time that lots of people survive car wrecks but that doesn't make them safe.
```

---
## \#197 Posted by: PatRocks Posted at: 2019-01-14T15:38:18.946Z Reads: 190

```
First! 10 char

Edit: at the risk of sounding like I agree with 10s, that is sound logic!
```

---
## \#198 Posted by: linsus Posted at: 2019-01-14T16:32:36.676Z Reads: 188

```
I usually take my angle grinder and saw one group in half. That way I have 11.5S. Its abit safer, I promise.
```

---
## \#199 Posted by: b264 Posted at: 2019-01-14T16:34:41.165Z Reads: 189

```
Wouldn't 4 diodes in series with the charge port accomplish the same thing :rofl:

Just that then the BMS would never get to "balance" mode
```

---
## \#200 Posted by: linsus Posted at: 2019-01-14T16:38:45.421Z Reads: 196

```
You're beeing too practical about this!
```

---
## \#202 Posted by: Indiangummy Posted at: 2019-01-14T17:03:08.283Z Reads: 192

```
Why don't more people go 11s? Are chargers and bms that hard to find?
```

---
## \#203 Posted by: b264 Posted at: 2019-01-14T17:18:29.598Z Reads: 189

```
I would consider it.  I don't know how hard chargers are to find, any 12S BMS would work fine
```

---
## \#204 Posted by: Indiangummy Posted at: 2019-01-14T17:20:14.600Z Reads: 193

```

Im going 11s on my next build. i have only tried 10s so far. I found a charger on aliexpress and a 11s bms from bestech. I don't think i'l notice the difference but we'l see.
```

---
## \#205 Posted by: Benjamin899 Posted at: 2019-01-14T17:21:33.220Z Reads: 185

```
well you can build your own charger. There are some people who have done it.
```

---
## \#206 Posted by: b264 Posted at: 2019-01-14T17:21:50.584Z Reads: 183

```
You can use any 12S BMS if you leave the most-positive p-group unconnected
```

---
## \#207 Posted by: Indiangummy Posted at: 2019-01-14T17:30:08.841Z Reads: 187

```
yeah and you can use a power supply. i bought one since that was the easiest. same goes for the bms. just more convenient and same price as a 12s bms.
```

---
## \#208 Posted by: b264 Posted at: 2019-01-14T18:05:29.946Z Reads: 184

```
Not any power supply, only a modern one with current AND voltage limits.
```

---
## \#209 Posted by: Indiangummy Posted at: 2019-01-14T18:06:54.035Z Reads: 186

```
Yeah that's what I ment. DC variable power supply
```

---
## \#210 Posted by: Andy87 Posted at: 2019-01-14T19:20:27.591Z Reads: 187

```
My first build was 11s.
No issues to find a charger and a bms at all.
```

---
## \#211 Posted by: Indiangummy Posted at: 2019-01-14T19:21:19.908Z Reads: 182

```
If my haya ever shows up. 11s is the plan. Hopefully it's a good in between 12s and 10s.
```

---
## \#212 Posted by: Andy87 Posted at: 2019-01-14T19:22:44.385Z Reads: 184

```
I liked it very much with dual 6374 190kV motors.
More than enough speed for me and with the right gearing also the torque is fine.
```

---
## \#213 Posted by: banjaxxed Posted at: 2019-01-15T15:28:50.870Z Reads: 184

```
Maybe 11s is the new 13s :face_with_monocle:
```

---
## \#214 Posted by: chuttney1 Posted at: 2019-01-15T16:13:37.094Z Reads: 188

```
[quote="banjaxxed, post:213, topic:58106"]
Maybe 11s is the new 13s :face_with_monocle:
[/quote]

Not a chance.
```

---
## \#215 Posted by: telnoi Posted at: 2019-01-15T17:31:13.448Z Reads: 186

```
Fix for 12 s is 8xxx motors, 100a x2 bat amps and a 10s3p pack. Guaranteed you will hit the safe voltage range within seconds.
```

---
## \#216 Posted by: Andy87 Posted at: 2019-01-15T18:02:06.996Z Reads: 190

```
[quote="telnoi, post:215, topic:58106"]
Guaranteed you will hit the safe voltage range within seconds.
[/quote]

How you mean that?
```

---
## \#217 Posted by: telnoi Posted at: 2019-01-15T18:03:50.401Z Reads: 195

```
Voltage sag.
```

---
## \#218 Posted by: Andy87 Posted at: 2019-01-15T18:04:43.983Z Reads: 200

```
Ah ok got ya. Thought the other way round...voltage spikes when breaking.
```

---
## \#219 Posted by: secupol Posted at: 2019-01-25T03:09:50.733Z Reads: 204

```
MOTION-SPIN

![20190125_114238|690x388](upload://9NfjzuydUc09zURAehli78We6To.jpeg) ![20190125_114212|690x388](upload://fiNJY9y2ggUdBn3p6dLJbspeVbN.jpeg) ![20190125_114204|690x388](upload://dzZSYITlZMvOyBaJKQoRSvSAnRn.jpeg) ![20190125_114243|690x388](upload://2AZBF43fD8Uj13dRBBnUoMXL2NX.jpeg) ![20190125_114153|690x388](upload://emknd96mzJBbcWmtLpcXWbhEP63.jpeg)

MOTION-SPIN Motor's Sensor Connection
![motion_spin_sensor_connection|690x388](upload://jxDYGwCz5zf9NMiDe91JFz3IYBl.jpeg) 

MOTION-SPIN vs VESC 6
![20190125_114945|690x388](upload://EHZWcRHIdsQc4uZiHFk7ef5hDQ.jpeg)
```

---
## \#220 Posted by: Riako Posted at: 2019-01-25T03:45:43.398Z Reads: 199

```
Well done sir! I don't understand a lot of things here, but what I see looks good ;) 
I really like where your wires and connections come out! Smart design, less loosen space for slim enclosure!
```

---
## \#221 Posted by: secupol Posted at: 2019-01-25T06:28:46.174Z Reads: 203

```
Thank you!!
```

---
## \#222 Posted by: secupol Posted at: 2019-02-05T04:44:09.879Z Reads: 199

```
MOTION-SPIN Uphill Test
https://youtu.be/zTLbvHebKjI
```

---
## \#223 Posted by: Riako Posted at: 2019-02-05T19:44:33.989Z Reads: 195

```
:clap: awesome :tada:
```

---
## \#224 Posted by: Lionpuncher Posted at: 2019-02-05T19:48:15.280Z Reads: 197

```
Looks great @secupol. Looking forward to seeing another esc option in the wild. Will you be performing more tests before producing some for sale?
```

---
## \#225 Posted by: secupol Posted at: 2019-02-06T05:38:17.590Z Reads: 199

```
FOC-SPIN ESC Torque Test
FOC-SPIN is based InstaSpin-FOC from TI

https://youtu.be/hNVmiHplvjA
```

---
## \#226 Posted by: secupol Posted at: 2019-02-21T05:46:06.275Z Reads: 187

```
![12|690x388](upload://k5tbADxRV7J2ySAjlBlfKDpDIpt.jpeg) 
The firmware is updated latest
3.50
```

---
## \#227 Posted by: secupol Posted at: 2019-03-03T07:02:32.773Z Reads: 183

```

![20190302_173652|690x388](upload://ySKYI7MS7WEUZ2znY6NKy9oM8Mv.jpeg) 


![20190302_173701|690x388](upload://aXzZFnNplDQPco9pLnX16nM6PME.jpeg) 

MOTION-SPIN Dual

□ AUIRF7749L2TR Automotive Grade

□ DRV8323RS Smart Gate Driver 

□ Firmware : 3.50

□ VESC Tool 1.04

□ Size : 99.6(W) x 84.0(L) x 17.0(H) mm

□ VESC 6 Clone x 2
```

---
## \#228 Posted by: secupol Posted at: 2019-03-03T08:38:44.560Z Reads: 186

```
![vesc_tool_dongle|690x388](upload://2MZO9lHdXAu4atrMYo1g4rRKvTu.jpeg) 

[VESC Tool BLE Dongle]


Main Module : BGM111 (Silabs)

VESC Tool Mobile app compatable

VESC Configuation

VESC Monitoring
```

---
## \#229 Posted by: Friskies Posted at: 2019-03-03T10:49:09.623Z Reads: 181

```
Looks Awesome! 
Two small and easily implemented suggestions:

1 - Please put some silicon around the caps to hold them in place otherwise they will break off
2 - Please change to USB type-C
```

---
## \#230 Posted by: secupol Posted at: 2019-03-03T10:58:35.104Z Reads: 181

```
Thank you for a good idea.
```

---
## \#231 Posted by: FredrikHems Posted at: 2019-03-03T11:08:57.673Z Reads: 184

```
What is the price for the dual?
```

---
## \#232 Posted by: secupol Posted at: 2019-03-03T11:16:10.580Z Reads: 187

```
I sent a message.
```

---
## \#233 Posted by: Benjamin899 Posted at: 2019-03-03T19:07:50.888Z Reads: 183

```
can you give us the specs? like max Volt ect.
```

---
## \#234 Posted by: secupol Posted at: 2019-03-03T20:54:08.953Z Reads: 182

```
Only gate driver is different from vesc 6.
Therefore, almost all of them have similar specifications.
```

---
## \#235 Posted by: secupol Posted at: 2019-04-12T01:35:08.714Z Reads: 169

```
https://youtu.be/1kp0HdYu5nE
```

---
## \#236 Posted by: secupol Posted at: 2019-04-12T01:54:26.278Z Reads: 172

```
https://youtu.be/uWsZCqVjz0M
```

---
## \#237 Posted by: secupol Posted at: 2019-04-30T05:08:00.315Z Reads: 157

```
https://youtu.be/k-dlVECK7jY
```

---
## \#238 Posted by: Jonisonvespa Posted at: 2019-12-29T15:45:35.874Z Reads: 80

```
Hi there
Is there any feedback from these really wan to buy them if they actually work and are they 12s? I see gate voltage is 60v?
Thanks
```

---
## \#239 Posted by: zhanzhan Posted at: 2020-01-16T01:35:23.246Z Reads: 61

```
great job bro! I also designed a vesc6 which has 12 mosfets and uses drv8323 as gate driver. The size is a little bit smaller 40x70x20mm. I tested under 42v 1000w. Just works fine.
```

---
## \#240 Posted by: secupol Posted at: 2020-02-11T07:18:11.982Z Reads: 24

```
FOC Sensorless Start-up Test
VESC based HFI Vs Instaspin based from TI's Chip


https://youtu.be/4eWELlag0Pw
```

---

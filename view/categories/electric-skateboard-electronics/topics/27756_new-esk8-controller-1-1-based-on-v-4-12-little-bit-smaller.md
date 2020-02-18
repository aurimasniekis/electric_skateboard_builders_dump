# NEW ESK8 Controller 1.1 based on V 4.12 little bit smaller

### Replies: 84 Views: 7480

## \#1 Posted by: esk8 Posted at: 2017-07-16T06:23:34.788Z Reads: 566

```
Our modified V 4.12 is finally finished!

We were inspired by Chacka
And have thought that we should follow his way
There are still a few other components added
But I list that later.
We would appreciate your opinion
```

---
## \#2 Posted by: esk8 Posted at: 2017-07-16T06:26:35.896Z Reads: 553

```
<img src="/uploads/db1493/original/3X/a/e/ae5ad77f3c2f82bab73f8f67d5cbde12d821c36c.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/9/2/92e2e4db7f272164d7a89b66ca3469c190a8baf3.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/e/a/eaed73630426c1b0cb833c9f7afdb5ac67b30375.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/c/c/ccab733b8237749c2a3a89abbbfdaba2d8375af6.JPG" width="500" height="500">
```

---
## \#3 Posted by: esk8 Posted at: 2017-07-16T06:28:11.475Z Reads: 523

```
The diameter was 75mm x 65mm x 19mm
```

---
## \#4 Posted by: bigben Posted at: 2017-07-16T07:16:25.391Z Reads: 515

```
Well done. This looks very clean and tidy! When will they available and for how much?
```

---
## \#5 Posted by: Maxid Posted at: 2017-07-16T07:32:43.925Z Reads: 513

```
There seems to be a lot of unused real estate on that PCB. Other than that nice job. Do you see improvements in terms of FOC reliability with this version?
```

---
## \#6 Posted by: esk8 Posted at: 2017-07-17T17:55:51.399Z Reads: 499

```
What we have upgrade:

IRF7749L1 DirectFet-L8

Upgrade by C1,C8,C9,C39,C40,C42,C43,C44,C45,C49 from 10yF 50V to 4,7yF 100V
Extra upgrade by C46,C47 2 resistors extra 4,7yF 100V and to the C37, C51 we build
for more reserve on C48 2x 4,7yF 100V resistor.
R53,R54 WSLP2726 Shunts
And Micro USB
```

---
## \#7 Posted by: NAT-Frank Posted at: 2017-07-17T18:02:10.133Z Reads: 472

```
When will it be available ?
```

---
## \#8 Posted by: esk8 Posted at: 2017-07-17T18:02:32.176Z Reads: 472

```
We have it now in our shop
```

---
## \#9 Posted by: longjohn Posted at: 2017-07-17T18:05:35.974Z Reads: 466

```
200 euros including tax, excluding shipping
```

---
## \#10 Posted by: esk8 Posted at: 2017-07-17T18:18:43.154Z Reads: 478

```
<img src="/uploads/db1493/original/3X/6/5/65f0d6697e86b43f39be9384ce2e1f712060d8c3.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/5/6/566a6a0038069425ff466759db69e77174f9529f.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/6/9/690e898aaaeee95c15ff5f9021aca28ea0558598.JPG" width="500" height="500">
```

---
## \#11 Posted by: Benji-Yafal Posted at: 2017-07-21T08:15:00.650Z Reads: 447

```
So if i understand,

This Controller will solve the problem of overheating / Thanks to Direct Fets and the allu case.
It will also solve the probleme of unexpected Boost when Duty cycle Drop since 0.85 to 0.95 cause the current is mesured on all phases.

So it's a great improve compare to the 4.12 version.

May I right ?
```

---
## \#12 Posted by: lrdesigns Posted at: 2017-07-21T12:59:46.731Z Reads: 438

```
It looks really nice! Great work. Only complaint is I want the USB to point upwards. 

What's the reason for the large caps being two different types / sizes?
```

---
## \#13 Posted by: goldenHusky Posted at: 2017-07-21T13:06:48.473Z Reads: 425

```
[quote="lrdesigns, post:12, topic:27756"]
What's the reason for the large caps being two different types / sizes?
[/quote]

Caps offer different frequency behaviour according to their capacity. Caps with more capacity can not provide power instantly/ as fast as it would be needed, caps with smaller capacity can. By taking different sizes caps in parallel you are usually well prepared for fast load changes and prevent undervoltage errors.
```

---
## \#14 Posted by: Silverline Posted at: 2017-07-21T13:11:57.234Z Reads: 404

```
We need a Group buy in EU , with this new controller 😎
```

---
## \#15 Posted by: Maxid Posted at: 2017-07-21T13:41:05.961Z Reads: 395

```
They are from Germany - why would you need a groupbuy then?
```

---
## \#16 Posted by: Silverline Posted at: 2017-07-21T13:43:44.350Z Reads: 392

```
Better price.. isn't that the thing with Group buys ?
```

---
## \#17 Posted by: Maxid Posted at: 2017-07-21T13:45:46.126Z Reads: 393

```
AFAIK they don't even offer bulk pricing. GB are usually only done to save shipping costs from overseas.
```

---
## \#18 Posted by: NAF Posted at: 2017-07-21T13:47:53.567Z Reads: 395

```
Or mostly to cut down the price on bulk orders. Maybe esk8.de would reconsider offering bulk discounts.
```

---
## \#20 Posted by: Mikkiller Posted at: 2017-07-21T14:26:31.031Z Reads: 399

```
I'd be totally down for a VESC group buy if we can lower the price enough
```

---
## \#21 Posted by: esk8 Posted at: 2017-07-21T15:03:55.582Z Reads: 403

```
Thanks for your consideration
For a group buy.
Unfortunately I have to tell you,
That we have only used the best material
What it gives to the market
We also produce everything in Germany
Unfortunately, the producing cost is very high
We have only produced 100 pieces
Which is also unpopular for the price too
Only the housing cost us in production 50.- €
At the price of 199.- € we do not even have 10%
But we donate ourselves from this Money BV too.
Of the little money that keeps us
We wanted to show with this controller
What you can build so beautiful when you want!
But we are trying to produce a larger quantity
To bring the price down
So that we can go a little bit down with the price.
We will also produce a low budget controller
Only with heat sink and heat shrink tubing
This could make the price around 25-30 € cheaper
For this, we have to test first whether it is because of the heat.
And the USB and PPM cable was in the front from the case,
for better connecting.
Al the other Producer build the USB and the Ppm on Top,
what unfortunately was for the connections.
By this Controller you done must break the cables.

Regards Attila
```

---
## \#22 Posted by: mmaner Posted at: 2017-07-21T15:11:50.688Z Reads: 370

```
I love reading your posts, its like a haiku every time :).  Regarding your VESC design, you rocked it.  I like case/heatsink, should make the VESC run more fluid and resolve a lot of the hi AMP issues.  Just wanted you to know I appreciate your hard work brother.
```

---
## \#23 Posted by: esk8 Posted at: 2017-07-21T15:24:54.037Z Reads: 374

```
[quote="mmaner, post:22, topic:27756, full:true"]
I love reading your posts, its like a haiku every time :).  Regarding your VESC design, you rocked it.  I like case/heatsink, should make the VESC run more fluid and resolve a lot of the hi AMP issues.  Just wanted you to know I appreciate your hard work brother.
[/quote]


Thank you for the compliment,
But I have not done this al alone.
Which I also could not can make
But some customers from me were  friend´s
And these friends have helped me
Which put the NEW ESK8 Controller 1.1 on the legs
Stabiele legs
```

---
## \#24 Posted by: LukePL Posted at: 2017-07-21T15:41:03.787Z Reads: 364

```
Housing for 50 euro???? Send me the design I might be able to do it for much,much lower price!
```

---
## \#26 Posted by: olgamedt Posted at: 2017-07-22T12:30:58.617Z Reads: 342

```
Attilla are you turkish?
```

---
## \#27 Posted by: esk8 Posted at: 2017-07-22T14:58:50.131Z Reads: 341

```
No i am not Turkish
```

---
## \#28 Posted by: esk8 Posted at: 2017-07-24T04:06:15.654Z Reads: 338

```
I have a good news!
@nowind tell me thats our ESK8 C 1.1 running very good 
with the FW from the Vesc Tool and 10S/FOC.

He testing the controller in his holiday, and when he don't can
destroy it, then i think we have making a good job.
```

---
## \#29 Posted by: esk8 Posted at: 2017-07-28T12:49:17.088Z Reads: 345

```
<img src="/uploads/db1493/original/3X/c/4/c451f73694b538179d1ed02b7d3a39a561bb5d43.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/2/e/2e8501c0923dad4130ced887aaa58c60403a614d.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/b/8/b889427ceaf39250ec313024248a246b62ac0999.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/4/e/4e564f711ca264aa9ff338906dc832eba27f3c97.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/5/6/561a9367d460850079fb8a68d73459ce7176b0bc.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/4/9/496716fea27ee0002cd5914a4a2ce51b24d4ebd5.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/3/8/385edccb2bed513669c4f9b2d1a7b45bbf4dafe3.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/d/0/d0d317c31314f0f5d0ba0a883c08e71035184dc9.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/7/7/77c2c953a925d88f28df220c57b154264c96e48a.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/6/5/65d0f7931249c7ac8a0686c1f9cc6dce865bb863.JPG" width="281" height="500">
```

---
## \#30 Posted by: Silverline Posted at: 2017-07-28T15:48:19.563Z Reads: 312

```
Pretty damn awesome looking. What board are you building :-) ??
```

---
## \#31 Posted by: esk8 Posted at: 2017-07-28T15:56:39.972Z Reads: 314

```
The Board was finish, but i want upgrade the Board from V4.12
to our new esk8 1.1 Controller
```

---
## \#32 Posted by: esk8 Posted at: 2017-07-28T16:00:49.409Z Reads: 321

```
Now we have became the Motor with 25cm Sensored cable 
wit 6 Pin connector for the ESK8 1.1 controller and for al another Vesc too.
There was now in our shop in stock.

<img src="/uploads/db1493/original/3X/9/a/9a6eaa6de5976fbaac4f74528bbd037c7349e511.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/0/9/09501dc1d1b2b38da05bf93a290b78211c6434cb.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/e/2/e276814de14c01dc2ab6382f9dae0fafab2adb0c.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/2/8/286caa634f9200ddf6e984e7a59ff3dad4ea755f.JPG" width="500" height="500">
```

---
## \#33 Posted by: zeno Posted at: 2017-07-28T16:01:56.546Z Reads: 300

```
looking beautiful!
```

---
## \#34 Posted by: Silverline Posted at: 2017-07-28T19:54:20.663Z Reads: 303

```
Okay, but what board is it then ?

Do you plan building custom batteries for people ?
```

---
## \#35 Posted by: esk8 Posted at: 2017-07-29T13:53:31.960Z Reads: 310

```
I build this board from V 4.12 of ESK8 C 1.1 dual systems <img src="/uploads/db1493/original/3X/2/2/22981063d63e3890e72c0af0f9fae090fe9c1397.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/e/0e697f680bed91631677d7949b920fde860fa9a8.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/8/6/86d4bdbf23860d2d6b2ce14c6e7c2865fda68a3f.JPG" width="281" height="500">
```

---
## \#36 Posted by: esk8 Posted at: 2017-07-29T13:55:39.498Z Reads: 299

```
And yes we build custom batteries.<img src="/uploads/db1493/original/3X/6/b/6b4fa214f8c8f306f32e22e66488464e756b14e8.JPG" width="666" height="500">
```

---
## \#37 Posted by: esk8 Posted at: 2017-07-30T14:43:58.280Z Reads: 308

```
<img src="/uploads/db1493/original/3X/4/c/4c209ad74482a479b8776d51ab013422af5c4533.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/3/f3f8c3cbca9fc2d259346cddf7f10c1cd4084f23.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/a/eadea93de560dd519902edb541edadc57c7c0d23.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/9/a/9a41059977f375cc0e0c5d38db30c64fc8c49758.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/0/204fe6cc1f0fa3baaf115fb3b164bd7833625870.JPG" width="375" height="500">
```

---
## \#38 Posted by: Misery Posted at: 2017-07-31T16:24:22.590Z Reads: 287

```
This is nice really nice...
```

---
## \#39 Posted by: esk8 Posted at: 2017-08-09T05:26:03.388Z Reads: 280

```
 I was at the weekend in Hohenstaufen, at the German Downhill Championships, it was a mega fun. There was also a Uphill race between the semi-final and the final race. The people were very enthusiastic and a lot of questions were asked. Evolve was also there and has two boards available for the race. Once the new GTX and a GT, the GTX has just come to half. The GT is about 15 sec. Later on like my two boards. Afterwards, we measured the times with how much the Evolve have climbed the mountain. The top speed was at a good 20Kmh. With 100% rechargeable battery and the 1.5Km up. At the top the batteries were still at 62% after 1,5Km. We then tested it with my boards. My Bustin boards have reached a maximum speed of 39.5Kmh, started with 96% battery and above the battery was still 90%. Then we tried it with my MTB and it even went with 40.2Kmh.
Al Board have a great performance and working fine.
The organizer would like next year
To the downhill also make an electro Uphill race.
It is very close to France, Austria and Schweitz.
```

---
## \#40 Posted by: esk8 Posted at: 2017-08-09T06:10:20.052Z Reads: 285

```
<img src="/uploads/db1493/original/3X/a/0/a082108eb9e85cf635d314ca46d81d00fec49460.JPG" width="374" height="500">
```

---
## \#41 Posted by: esk8 Posted at: 2017-08-09T06:49:18.947Z Reads: 283

```
https://youtu.be/7eJ3bs0s5Rc
```

---
## \#42 Posted by: rich Posted at: 2017-08-18T10:43:55.298Z Reads: 285

```
Just received the esk8 1.1 controllers for my eMTB. Wow, looks like a masterpiece, nice and sturdy! Very well done @esk8, can't wait to test them :yum: 

I'm also surprised because of the size, the controllers look bigger on pics. So here a comparison with the standard V4.12. 

<img src="/uploads/db1493/original/3X/d/0/d086337660d448196c502c2fc3757ba447f2e9da.jpg" width="281" height="500">
```

---
## \#43 Posted by: karma Posted at: 2017-08-18T11:11:36.338Z Reads: 268

```
Nicely done @esk8! Will be nice to see some builds with this ESC!
```

---
## \#44 Posted by: esk8 Posted at: 2017-08-18T17:04:08.467Z Reads: 260

```
The exact diameters was:
L 77mm, W 68mm, H 20mm on the side where was the Elko´s 
and on the side where was the cable only 16mm.
So i think we have build wit the ESK8 1.1 the smallest housing.
And 95gr. weight.
```

---
## \#45 Posted by: Der6FingerJo Posted at: 2017-08-18T18:35:00.883Z Reads: 257

```
I know FOC isn't officially recommended, but what are your experiences so far on it? I really fell in love with the (lack of the) sound of FOC while i fried my 4.12 :smile:
```

---
## \#46 Posted by: JdogAwesome Posted at: 2017-08-18T20:12:07.920Z Reads: 254

```
Love the compact design, though I'm just curious what the difference is between this and the VESC 6 or FOCBOX?
```

---
## \#47 Posted by: Cobber Posted at: 2017-08-18T20:37:31.663Z Reads: 267

```
Looks sweet as bro! :sunglasses: 
How many cells in series & motor amps are you recommending this for?

edit: found it bro

**Summary:**
8V – 60V ( 3s to **12s** LiPo) max. 60.000 ERPM
**50A continuous** current, up to 240A (for some seconds)
FOC (Field Oriented Control) with automated motor detection via USB and BLDC-Tool, IMPORTANT: FOC is still in development, please be carful! Implementation of FOC only on you own responsibility and risk.
Integrated BEC 5V 1A output for external electronics (converter integrated)
Size: ca. 72mm x 68mm x 19mm
Current and volt measurement on all phases
Regenerative breaking
Sensored and sensorless operation
User interface for Windows, OSX and Linux
Updates through USB connection via BLDC-Tool SW
no passive or active cooling required (depends of course on your usage)
```

---
## \#48 Posted by: esk8 Posted at: 2017-08-19T17:40:21.995Z Reads: 254

```
Because the ESK8 1.1 controller is based on the V4.12
I have also adopted the values. precaution.
I can not say exactly how the Vesc6 and the FOCBox
are different.
For all three, the direct fets are used.
But I have not been on the FOCBox and on the Vesc6
The TDK capacitors SMD2220 with 15uF / 100v
Also the caps are with FOCBox and Vesc6 2x 680yF / 63V
The SMD 1206 is installed with the FOCBox
But I do not know whether 10uF / 50V or 4.7uF / 100V
And there are 9 pieces on the FOCBox.
We use 14 pieces SMD1206 with 4.7uF / 100V.
And the caps we have used 1 x 680yF / 63V and 1 x 1600yF / 63V
This reduces the current fluctuations to the minimum
Vesc6 have 3x shunt
FOCBox 2x
ESK8 1.1 2x

Everything else can only be answered by the BOM list.
Regarding the components where the difference is
```

---
## \#49 Posted by: esk8 Posted at: 2017-08-19T17:43:21.688Z Reads: 257

```
Vesc6
<img src="/uploads/db1493/original/3X/b/2/b25516f8f38ad330661b7f22534e0475041107ac.png" width="604" height="500"><img src="/uploads/db1493/original/3X/6/6/66bae68ff757589b81ce82a6ecf1050903510244.png" width="528" height="500">
```

---
## \#50 Posted by: esk8 Posted at: 2017-08-19T17:44:41.056Z Reads: 252

```
FOCBox
<img src="/uploads/db1493/original/3X/5/d/5d1a8bcf30008aec08fb5805266aad415422b6da.png" width="508" height="500"><img src="/uploads/db1493/original/3X/1/a/1a4e707926323effa12bbd5f34cd4c38016f7c7f.png" width="518" height="500">
```

---
## \#51 Posted by: esk8 Posted at: 2017-08-19T17:48:16.885Z Reads: 255

```
ESK8 1.1
<img src="/uploads/db1493/original/3X/a/e/ae5ad77f3c2f82bab73f8f67d5cbde12d821c36c.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/9/2/92e2e4db7f272164d7a89b66ca3469c190a8baf3.JPG" width="500" height="500">
```

---
## \#52 Posted by: notger Posted at: 2017-08-22T05:12:40.681Z Reads: 244

```
[quote="esk8, post:35, topic:27756"]
I build this board from V 4.12 of ESK8 C 1.1 dual systems
[/quote]

Hi,
whats actually the reason for using two antispark.
Would one for both VESCS (ah sorry ESK8 Controllers) get too hot ?
and whats your experience with the 40A Car Fuses do they handle high Current bursts well ?

greets

Notger
```

---
## \#53 Posted by: esk8 Posted at: 2017-08-22T06:17:12.828Z Reads: 244

```
https://youtu.be/srIfnb9vwxc
```

---
## \#54 Posted by: Der6FingerJo Posted at: 2017-08-22T19:22:33.454Z Reads: 238

```
Does anyone know where the UART TX and RX Pins are on this one? Couldn't find them on mine through trial and error :smile:
```

---
## \#55 Posted by: esk8 Posted at: 2017-08-23T04:22:06.882Z Reads: 245

```
[quote="Der6FingerJo, post:54, topic:27756, full:true"]
Does anyone know where the UART TX and RX Pins are on this one? Couldn't find them on mine through trial and error
[/quote]

<img src="/uploads/db1493/original/3X/6/6/669167d02957edc185e3991acb63d1d03b7a0c69.png" width="659" height="500">
```

---
## \#56 Posted by: rich Posted at: 2017-08-23T05:52:30.460Z Reads: 241

```
[quote="notger, post:52, topic:27756"]
whats actually the reason for using two antispark.
[/quote]

It seems that the esk8 controller 1.1 can deliver more power than the regular V4.12. So if you have dual system and ride uphill with full throttle the 40A fuse will blow (after 10 sec. receiving 60A). It's possible to solder a bigger fuse to the antispark but maybe it gets the bottleneck in the end that's why I'll use 2 antispark switches as well, the on/off switch is connected to both PCB's in parallel. 

I have another question @esk8, I can't find info about the assignment of PPM pins. Where is (-), (+) and (s) located? Or just show a picture with connected servo wire, thanks!
```

---
## \#57 Posted by: esk8 Posted at: 2017-08-23T07:28:35.603Z Reads: 248

```
[quote="rich, post:56, topic:27756"]
It seems that the esk8 controller 1.1 can deliver more power than the regular V4.12. So if you have dual system and ride uphill with full throttle the 40A fuse will blow (after 10 sec. receiving 60A). It's possible to solder a bigger fuse to the antispark but maybe it gets the bottleneck in the end that's why I'll use 2 antispark switches as well, the on/off switch is connected to both PCB's in parallel. 

I have another question @esk8, I can't find info about the assignment of PPM pins. Where is (-), (+) and (s) located? Or just show a picture with connected servo wire, thanks!
[/quote]


When you looking in front of the 3Pin the GND/black was on the right side and the White
comes beside the USB 
<img src="/uploads/db1493/original/3X/9/9/99020aefd726fc1ef86a7f9ee0cc5b64f1392971.jpeg" width="500" height="500">
```

---
## \#58 Posted by: telnoi Posted at: 2017-08-24T04:32:11.186Z Reads: 237

```
@esk8

I bought two. Is there a pinout chart available somewhere? I do not want to connect things in reverse :P
Canbus should be easy enough (just take the two middle pins), however receiver/ppm could be tricky.
```

---
## \#59 Posted by: rich Posted at: 2017-08-24T08:01:26.705Z Reads: 233

```
All your questions are answered with the 2 pics above :wink:
```

---
## \#60 Posted by: telnoi Posted at: 2017-08-24T08:57:20.462Z Reads: 231

```
Ah, stupid. Thanks!
```

---
## \#61 Posted by: telnoi Posted at: 2017-08-28T18:27:19.193Z Reads: 237

```
@esk8

I received my two units today. Sadly, one (or several) wires are soldered incorrectly. 
The + wire simply came loose after test fitting the unit, which required slightly bending the power wires. By judging how easily this one came loose, I doubt I should trust the solder job of the other wires...

https://youtu.be/EfQ-x-zKLwo
 
Does anybody know if these cases can be opened without causing damage?
I am seriously not in the mood for a return shipping for something that I can easily fix myself.

P.S. Never in my life have I been able to remove a properly soldered 12AWG wire...Even with an FPV race drone flying 120 km/h into the ground with the lipo being flung forward.
```

---
## \#62 Posted by: Silverline Posted at: 2017-08-28T18:50:31.396Z Reads: 230

```
Damn... that`s poor soldering...
```

---
## \#63 Posted by: esk8 Posted at: 2017-08-28T18:57:57.934Z Reads: 231

```
@telnoi
Sorry for this  and this was for me very unpleasantness!
You can send me back and i refund your the shipping cost.
Tell me please in PM you order Number that i know
the adresses where i must sending the new controller.
I have not enough controlling my solder work.
I al time controlling al soldering work.
but there is that I do a probably a fault.

Regards Attila
```

---
## \#64 Posted by: telnoi Posted at: 2017-08-28T20:43:30.659Z Reads: 226

```
Attila very quickly provided me with the info needed to fix the issue. I opened up the case and soldered the wire in place. Please note that if you do this without esk8.de's approval, you will void your warranty.

P.S. The PCB looks great. Very tidy, components all straight. The other wires were soldered correctly. There is no doubt in my mind that this is a high quality VESC.
```

---
## \#65 Posted by: telnoi Posted at: 2017-08-31T21:09:33.812Z Reads: 232

```
Having issues setting two up via CANBUS.
When enabling can FWD in the upper right corner using the correct ID for the slave (2), I get ''**no firmware response**''
and only one motor responds to the Tx.

**Master General**
<img src="/uploads/db1493/original/3X/6/8/68bc8957d5d459faf69f088e44103d123bef39d0.png" width="689" height="392">

**Master PPM**
<img src="/uploads/db1493/original/3X/c/7/c79334bf645776cb601666659b39f8c95a54bb97.png" width="690" height="396">

**Slave General**
<img src="/uploads/db1493/original/3X/b/c/bcbf214d2d9ad676dd5aceeae5bca4b4c9ec5853.png" width="690" height="401">

**Slave PPM**
<img src="/uploads/db1493/original/3X/2/b/2b1fa69de99092b8ce1f4cbbe50f68da16c12281.png" width="690" height="402">

**Setup**
<img src="/uploads/db1493/original/3X/7/8/7835c1841ecba0c3ed93fbf438f064eec94c0956.jpg" width="666" height="500">

Both VESCs are connected to an anti-spark plug with an Y cable/single xt-60 connector. 

The CANBUS cable is OK. Each individual ESC can be read/motors run.
CANBUS connection does not work.

Any ideas?
```

---
## \#66 Posted by: rich Posted at: 2017-08-31T22:46:30.479Z Reads: 224

```
Hey, I'm sure this will solve your problem:

ON THE SLAVE:
Read configuration
Set Controller ID to 1
In the app configuration **disable** "Multiple ESC's over CAN"!!! (enabled on master only)
"Send status over CAN" is already enabled.
Write configuration and reboot.

ON THE MASTER:
Read configuration
Set Controller ID to 0
"Multiple ESC's over CAN" is already enabled.
Write configuration and reboot.
```

---
## \#67 Posted by: telnoi Posted at: 2017-09-01T04:04:32.069Z Reads: 224

```
Thanks, but sadly that does not resolve the issue.
Those were the settings I tried first (I followed this tutorial http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/)/tried it again just now.

Same issue as before.
```

---
## \#68 Posted by: esk8 Posted at: 2017-09-26T04:31:47.623Z Reads: 223

```
https://youtu.be/xHZWANvvobY
```

---
## \#69 Posted by: Silverline Posted at: 2017-09-26T08:05:39.109Z Reads: 208

```
Why only 720P.....
```

---
## \#70 Posted by: Pimousse Posted at: 2017-09-26T12:10:07.848Z Reads: 199

```
@esk8 Did you split + and - wires at one edge of the board each ?
Regarding a old video of Vedder, as far as I understand this is not a good idea in matter of capacitance
https://youtu.be/x6lPdI9OVQg?t=12m58s

I don't know what is the real impact on the electronics, but could be more reliable to keep them close to each other, right ?
```

---
## \#71 Posted by: esk8 Posted at: 2017-09-27T04:47:14.364Z Reads: 183

```
I don't know why the Video was only in 720P 
I am looking in the settings by youtube but i don't find
it that i Kan make the P higher.
And i loaded the original vide by youtube down.
I must looking thats i loaded the Vide from the SD Card.
I hope than was it better.

Regards Attila
```

---
## \#72 Posted by: fuelre Posted at: 2017-09-27T13:36:53.218Z Reads: 184

```
[quote="Pimousse, post:70, topic:27756"]
@esk8 Did you split + and - wires at one edge of the board each ?
Regarding a old video of Vedder, as far as I understand this is not a good idea in matter of capacitance
VESC6 Thermal Analysis (measurements + simulation)

I don't know what is the real impact on the electronics, but could be more reliable to keep them close to each other, right ?
[/quote]

If I understand you correct, you are asking if he has the plus cable on the TOP side of the PCB and the minus cable on the BOTTOM?
Yes he is doing that, you can see that on the first and second pic in this thread.
I dont know if there is copper on the PCB where the cables are going. but if so, it is probably a groundplane which is the same as the minus cable. 
nether the less the 2 cables are running parallel (only separated by the PCB (probably 1,6mm thick)) to the solderpads.
Therefore it isn't a problem in my mind.

and what you are asking for is the inductivity, not the capacity, as Ben mentioned in his video
```

---
## \#73 Posted by: Pimousse Posted at: 2017-09-27T13:45:20.205Z Reads: 177

```
No, I meant that he put a red wire (assuming + one) on one edge (toes side) of his Mountainboard from electronics to battery box and black one on heels side.
You're right, it's inductivity.
```

---
## \#74 Posted by: fuelre Posted at: 2017-09-27T13:49:16.391Z Reads: 183

```
yes you are correct
```

---
## \#75 Posted by: esk8 Posted at: 2017-10-02T10:32:40.926Z Reads: 179

```
We testing in next time the ESK8 1.1 controller with the 
Sanyo 20700 cells with 10S/4P 

<img src="/uploads/db1493/original/3X/7/1/7104d58f33d98efda4fee7cd9dc632e21f4ff9c8.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/0/e/0e5fc4edd152e4122e4614c5828405de2e2aae8e.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/3/7/374fd2cc50525db89cba0fab867adf5852944b3b.JPG" width="281" height="500">
```

---
## \#76 Posted by: esk8 Posted at: 2017-10-04T14:18:42.477Z Reads: 167

```
https://youtu.be/xSnwU1vD5is
```

---
## \#77 Posted by: esk8 Posted at: 2017-10-11T06:40:09.960Z Reads: 163

```
https://youtu.be/UzJB-XYzPdI
```

---
## \#78 Posted by: joellind Posted at: 2017-10-11T07:55:23.586Z Reads: 161

```
How nice to see you further developing your products. Altough why don´t you answer your emails to your already existing customers?
```

---
## \#79 Posted by: esk8 Posted at: 2017-10-11T16:19:00.746Z Reads: 154

```
I was on vacation and I have it also on the HP communicated.
Unfortunately, I had an accident on holiday with my board.
Unfortunately, I was also in the hospital.
Therefore the replies to the emails have been delayed a bit.
This is not a new product and no further development.
This is just a video of what a customer sent me.
But the question itself, yes, I have sent you the new Wheel Pulley Monday!
```

---
## \#80 Posted by: GrecoMan Posted at: 2017-10-11T16:22:54.792Z Reads: 150

```
Oh man dude! Hope your ok!
```

---
## \#81 Posted by: esk8 Posted at: 2017-10-11T16:28:17.707Z Reads: 153

```
Yes thank you @ GrecoMan so slowly it will again,
I could hardly believe the first two weeks
do not can use my hands.
But we test all our products ourselves :grin:
```

---
## \#82 Posted by: joellind Posted at: 2017-10-11T20:42:55.729Z Reads: 144

```
okay I understand! 
Get well soon. I Guess the vesc was sent together to?
```

---
## \#83 Posted by: telnoi Posted at: 2017-10-14T07:58:41.799Z Reads: 134

```
Barely put my mountain board together and already thinking about upgrades ;)

Is it safe to run 12S on these, without adding additional caps?
*BLDC
*149KV

I already know I won't hit the ERPM limit with my setup.
```

---
## \#84 Posted by: esk8 Posted at: 2017-10-17T20:01:45.079Z Reads: 127

```
https://youtu.be/RgVthPpuI6E
```

---
## \#85 Posted by: esk8 Posted at: 2017-10-18T04:42:58.347Z Reads: 122

```
[quote="telnoi, post:83, topic:27756"]
Barely put my mountain board together and already thinking about upgrades :wink:

Is it safe to run 12S on these, without adding additional caps?
*BLDC
*149KV

I already know I won't hit the ERPM limit with my setup.
[/quote]


Unfortunately, I have no engine
what goes to 12S
But I'm sure you're using the system
can also drive with 12S
It would be very interesting to know how well
it works with 12S

But i came by 12S SK3 6374 149KV motor by 12S/50,4V over 60.000 ERPM. (67.586)
Ore i have a calculation error ?
```

---
## \#86 Posted by: telnoi Posted at: 2017-10-22T11:55:52.914Z Reads: 97

```
ok, a little over the ERPM limit..but I currently never push full throttle.
30 km/h is scary enough offroad here. Just looking for more power to go up hill.

Using 2x5000mah 6S 60C, I can set each VESC to 50A (maybe 40 to stay on the safe side, currently it is set to 25).

How much amps can I pull MAX using a single ESK8 anti-spark switch for both VESC? I already removed the fuse and bridged the two pads with 12AWG wire.
```

---

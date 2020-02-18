# Let the Fun Begin. The Pink Dragon Spine - hackable electric skateboard &#124; 3D printed &#124; Onda deck &#124; 6364S 63mm Motor &#124; LiFe 79,2 Wh (3000 mAh) &#124; VESC &#124; Faraday Motion &#124; Arduino &#124; Fusion 360

### Replies: 23 Views: 2961

## \#1 Posted by: aikokami Posted at: 2017-01-10T15:53:04.412Z Reads: 427

```
Once I saw “electric”, “vehicle” and “3D printed” I knew it had to be good (and I was right). Finally I had a chance to build my Pink Dragon Spine.

I got Onda core deck and [The Spine kit](http://shop.faradaymotion.com/shop/4-the-spine/80-spine-electronics-kit/?utm_source=aiko's%20build%20thread) including VESC and NodeMCU (Wi-fi module).

It all started from trying to figure out what do I need. I've used those components:
- [Faraday Motion Lightspeed 6364S 63mm Motor](https://goo.gl/l2Y4vO) 
- [VESC Motor Controller](https://goo.gl/fUt3nT)
- Capacitor + PCB
- HTD5-15MM Belt (525mm)
- HTD5-15mm Motor Pulley (16 teeth) (feather key + pinol screw)
- NodeMCU (Wi-fi module)
- Arduino Mini
- [LED ring 12 bit black](http://www.ebay.com/itm/401174790065)
- [63mm Motor Bracket](https://goo.gl/yuYrYo)
- [Onda Wheels with Gear-mount](https://goo.gl/DkIXdq)
- [Onda core deck, torsion shocks and trucks](http://shop.ondamotion.com/onda-truck/)


So here we go. Battery compartment had to be modified - current design is suitable for [LiPo](http://shop.faradaymotion.com/shop/1-electronics/54-battery-6s/) battery used by Faraday Motion. I had LiFePO4 in different size and I wanted to have lights on the back to be more visible. Fusion 360 was good enough to design/redesign all the components.

<img src="/uploads/db1493/original/3X/4/f/4f3e9d8ae3c460c65759ed185ef675b1f3247e51.png" width="689" height="317">

I needed a unicorn on the back as well. 

<img src="/uploads/db1493/original/3X/d/4/d45bc7b56ecec7d00aa108c414872995ab133520.jpg" width="316" height="500">

Placing my nick and slot for a dragon.

<img src="/uploads/db1493/original/3X/6/5/65f4c1909d46b68b046c849fdb1f242e1189c840.png" width="690" height="326">

Top lid was 6 hours print. 

<img src="/uploads/db1493/original/3X/a/c/acfe14907101423240b5032fcec3b5aa243851ea.jpg" width="690" height="388">

And it required some wet sanding.
<img src="/uploads/db1493/original/3X/8/c/8c93abfb163c5f0b6b4bc6b4690f870320c224ee.jpg" width="281" height="500">

Those parts are suitable for The Spine 2.0 by Faraday Motion
<img src="/uploads/db1493/original/3X/1/7/177f1f7bdf0db3c9220816495a105d445541022d.jpg" width="281" height="500">

•	Drive belt gear was printed with 75% infill. Top lid was printed with 20% infill because of its function. All other parts were printed with 50% infill.

<img src="/uploads/db1493/original/3X/f/4/f4195d8e6edd189b3b12a5a7f82bac935b2694ed.jpg" width="690" height="388">

•	Wall thickness of the parts is 1,6mm 
•	All parts were printed with 0,8mm nozzle on Ultimaker Original


I wanted Voltage meter on the side - and there was perfect space for having a display. Also - having fuse on the side sounded like a good idea. I failed few times with designing and printing something which would fit display, cables and fuse. This one went super bad.

<img src="/uploads/db1493/original/3X/f/b/fbafffa63a094cf9503dabc2977cd0e151c407e2.png" width="690" height="327">

Finally - this one looked good.

<img src="/uploads/db1493/original/3X/7/4/74129c418342d751b6bf759387a995bc7ba3d189.png" width="690" height="348">

Slicing was made in Cura.
<img src="/uploads/db1493/original/3X/c/e/cef4821117e7f7a516f01500e09d67b373df6962.png" width="690" height="366">

Tight fit. 

<img src="/uploads/db1493/original/3X/2/7/2740c94790007615e5527e9ec13917564404a1cb.jpg" width="690" height="388">

It fits!
<img src="/uploads/db1493/original/3X/4/3/436bbc0520d7fab88c958df94c60047deaaf95c6.jpg" width="690" height="388">

Making connector for battery and battery tester. 

<img src="/uploads/db1493/original/3X/7/0/70a2385dbd2255043cb90a49c2d53423d17590e4.jpg" width="666" height="500">

Unsoldering all factory pins cuz... well NodemCU (ESP8266) looked too big to fit nicely in the electronic box. I could make it nicer.

<img src="/uploads/db1493/original/3X/9/5/95c477da01efc61640ae32322ce0d49af70daedf.jpg" width="666" height="500">

After and before.
<img src="/uploads/db1493/original/3X/b/f/bf1a6d686f06652d0253ef6505a2d56927092993.jpg" width="690" height="358">

Arduino and LEDs on the back required 5V therefore I had to solder together DC/DC converter. 

<img src="/uploads/db1493/original/3X/b/6/b6eddafe3f353aeb097948514a9297eb67e59508.jpg" width="281" height="500">

And place it somewhere. 

<img src="/uploads/db1493/original/3X/c/6/c60c95d324f7ebdc5b7ecb2db5c8ffe0fce7ba38.jpg" width="690" height="388">

It would make sense to test it. First problem: few battery testers (LiPo battery voltage tester – low voltage buzzer alarm) did not recognize all 8 cells (just first 6) The problem appeared to be in battery tester not in the battery - last two pins were not connected to anything.... (ebay special). Tried another tester and this time it worked. All 8 cells were good.

<img src="/uploads/db1493/original/3X/8/1/81934ff94a00c3febce2cfe4eda8780b2271a1c7.jpg" width="377" height="500">



Mishaps:
•	Printing first battery compartment suitable for standard LiPo battery used by Faraday Motion, not for LiFe custom battery pack (wrong measurements).
•	Problem with battery testers which did not recognize all 8 cells of LiFe battery pack.
•	Printing top lid with support – with 0, 8 mm nozzle (instead of changing settings from suitable for 0,2mm nozzle) which made removing support material time consuming and not easy. 

<img src="/uploads/db1493/original/3X/d/f/dfbdfd32ea0edb559bde6281b8820dba7533477a.jpg" width="690" height="388">

•	Used VESC and motor started working without problems after connecting but motor was stuttering which gave a suspicion that it works sensor less. Order of the pins was reversed. Connector had to be taken apart and cables had to be moved. Other than that - works fine.

Time to put everything together
<img src="/uploads/db1493/original/3X/7/2/72c1f24e72cfcff5ba42ca3df512ca46653eebf2.jpg" width="281" height="500">


There is one part I'm missing for now - something to keep battery locked in place. For now it sits in the battery compartment thanks to foam.

<img src="/uploads/db1493/original/3X/f/e/febc1308b566433312492689cac642d881b3bf31.jpg" width="281" height="500">


It's alive!

<img src="/uploads/db1493/original/3X/b/7/b77ade69aafecf66529bd1de50117dfe824db94d.jpg" width="690" height="388">
```

---
## \#2 Posted by: mmaner Posted at: 2017-01-10T15:59:43.449Z Reads: 387

```
Nice build, way to get outside of known methods and just boy scout the hell out of it :slight_smile:
```

---
## \#3 Posted by: aikokami Posted at: 2017-01-10T16:10:46.063Z Reads: 379

```
Thanks. Planning to use it on a daily basis. Just have to wait for winter to pass.
```

---
## \#4 Posted by: ccostel Posted at: 2017-01-10T16:45:44.074Z Reads: 359

```
Dang! This is the most amazing and modded Spine in the company. Congrats on your impressive build Alicja. 

Cheers!
```

---
## \#5 Posted by: FredSaberhagen Posted at: 2017-01-10T22:51:50.590Z Reads: 331

```
Why is it called a "spine?"  Also - you have some serious skills.  I love how you modded, printed, and did so much yourself and made it your own ;-)  Can't wait to see some footage of it riding.  Haha it's like the sumo guy from street fighter 2...get it because e-Ondas... sorry.
```

---
## \#6 Posted by: saul Posted at: 2017-01-10T23:58:00.739Z Reads: 310

```
Nice build. i'm still not sure about the wifi control or having all the weight off one end, but the dragon makes it all worth it! :sunglasses:
```

---
## \#7 Posted by: aikokami Posted at: 2017-01-11T11:10:40.671Z Reads: 289

```
Well, it's the base for the vehicle. I have started with The Spine to have electric skateboard which is extensible in terms of software and hardware. Now I'm able to add new components and functionality over time.
```

---
## \#8 Posted by: aikokami Posted at: 2017-01-11T15:20:53.295Z Reads: 275

```
rear part could be smaller - I'll work on that some time. What you are unsure about? I would love to hear what you've been thinking about this part. Dragon is the most important thing in this build :D
```

---
## \#9 Posted by: Smirjl Posted at: 2017-01-19T11:37:57.016Z Reads: 248

```
Sure? I thougth most important part was the unicorn. By one side I feel that unicorn don't fit the name "dragon spine. By the other side I know that everybody needs and unicorn, so it's perfect where it is. 

I live your buld.
```

---
## \#10 Posted by: aikokami Posted at: 2017-01-27T14:50:15.635Z Reads: 236

```
I brought my baby to work today.

<img src="/uploads/db1493/original/3X/4/5/45aaf89e6bf353bf58f9a179a318a3e99667c7a6.jpg" width="690" height="388">
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2017-01-27T21:30:02.777Z Reads: 212

```
@aikokami can you post some ride videos? Like to see your rides in action
```

---
## \#12 Posted by: Guacamoleface Posted at: 2017-01-28T00:13:51.981Z Reads: 202

```
That looks dope! Good job!
My need of a 3D printer keeps increasing. So much possibilites :D
```

---
## \#13 Posted by: aikokami Posted at: 2017-01-28T12:56:34.850Z Reads: 198

```
[ride in the office](https://www.facebook.com/faradaymotion/videos/vb.790600320983031/1300266466683078/?type=2&theater&notif_t=video_comment&notif_id=1485581053324923) - more videos coming soon. I'll keep you posted.
```

---
## \#14 Posted by: Michaelinvegas Posted at: 2017-01-28T17:59:02.703Z Reads: 194

```
Lol...ok I forgot it's winter.....lol....

Yeah....inside riding in the office don't count! Lol
```

---
## \#15 Posted by: aikokami Posted at: 2017-02-02T13:19:37.549Z Reads: 173

```
I did not think about heating my battery cells and winter tires.. But it can be done :D
```

---
## \#16 Posted by: sharky Posted at: 2019-03-17T16:51:32.666Z Reads: 94

```
Nice build like the idea and the 3d printed parts
Hope youll post some vids where you ride it😁
Yeah an of course the color is nice
!!pink is faster!! 100%sure 😅
![IMG_5856|375x500](upload://sEuVSBr7tvjcBDwzPZYButJPDCA.jpeg) ![IMG_5847|375x500](upload://Ar0V5vTBtttS5B3YKWfqKVr6o5e.jpeg)
```

---
## \#17 Posted by: brenternet Posted at: 2019-03-17T17:59:17.425Z Reads: 80

```
This was 2 years ago bud.
```

---
## \#18 Posted by: KaramQ Posted at: 2019-03-17T18:09:52.780Z Reads: 77

```
What is up with people reviving 2 year old threads
```

---
## \#19 Posted by: mmaner Posted at: 2019-03-17T22:11:04.954Z Reads: 64

```
What's up with worriying about people reviving old threads?  It does hurt anything, especially if they are looking for info.
```

---
## \#20 Posted by: Sn4pz Posted at: 2019-03-17T22:13:03.093Z Reads: 66

```
I think he just wanted to flex his pink wheels? Lool
```

---
## \#21 Posted by: KaramQ Posted at: 2019-03-17T22:45:44.375Z Reads: 56

```
I don’t find it wrong, but why, the original listing owner hasn’t been active for like 2 years
```

---
## \#22 Posted by: dareno Posted at: 2019-03-17T22:53:53.850Z Reads: 58

```
Tells me the guy is reading his arse off.  Good thing.
```

---
## \#23 Posted by: sharky Posted at: 2019-03-18T14:27:14.308Z Reads: 40

```
tbh i was reading through a lot of stuff this day and ive overseen the fact tht this post has been 2 years old :slight_smile:
But maybe it motivates aikokami to post something again
kr
```

---

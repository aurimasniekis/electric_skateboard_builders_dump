# VESC FAQ &#124; What is FOC Field-oriented control

### Replies: 56 Views: 21096

## \#1 Posted by: onloop Posted at: 2015-11-05T23:58:14.406Z Reads: 1325

```
HERE IS WHAT WIKIPEDIA SAYS:

Vector control, also called field-oriented control (FOC), is a variable-frequency drive (VFD) control method where the stator currents of a three-phase AC electric motor are identified as two orthogonal components that can be visualized with a vector. One component defines the magnetic flux of the motor, the other the torque. The control system of the drive calculates from the flux and torque references given by the drive's speed control the corresponding current component references. Typically proportional-integral (PI) controllers are used to keep the measured current components at their reference values. The pulse-width modulation of the variable-frequency drive defines the transistor switching according to the stator voltage references that are the output of the PI current controllers.[1]

FOC is used to control the AC synchronous and induction motors.[2] It was originally developed for high-performance motor applications that are required to operate smoothly over the full speed range, generate full torque at zero speed, and have high dynamic performance including fast acceleration and deceleration. However, it is becoming increasingly attractive for lower performance applications as well due to FOC's motor size, cost and power consumption reduction superiority.[3][4] It is expected that with increasing computational power of the microprocessors it will eventually nearly universally displace single-variable scalar volts-per-Hertz (V/f) control.[5][6]


**What does this mean for electric skateboards?**
So far the most obvious change is the sound that comes from a motor. check this video out:
http://youtu.be/ISzeSLpZWbM

It should also make a big difference for hub motors, but there is no evidence of this yet.
Also it is meant to be more efficient, but also there is no data yet for this.
```

---
## \#2 Posted by: onloop Posted at: 2015-11-06T00:05:56.922Z Reads: 1020

```
Its also worth noting that V4.10 VESC will be compatible with FOC, Because FOC is implemented in the software you just need to upgrade the firmware of the vesc.

I am not sure that it will work on older version of VESC yet. will confirm later.
```

---
## \#3 Posted by: sl33py Posted at: 2015-11-06T00:33:23.029Z Reads: 993

```
Should work with v4.8 (and newer) which is what Vedder is testing w/ in this video.  He hasn't actually tested w/ v4.10 but says he expects it to be even slightly better than v4.8 he's using.
```

---
## \#4 Posted by: cmatson Posted at: 2015-11-06T02:43:36.797Z Reads: 949

```
This looks awesome! But we'll have to be capable of loading firmware onto our VESC if we hope to update (when It comes out) to this feature, right?
```

---
## \#5 Posted by: onloop Posted at: 2015-11-06T02:51:46.093Z Reads: 872

```
Yeah you will need to update firmware... but that's easy, you do it directly from the BLDC tool.
```

---
## \#6 Posted by: treenutter Posted at: 2015-11-06T03:14:31.524Z Reads: 823

```
Awesome. FOC is enough incentive for me to finally try installing the boot loader onto my VESC so I can apply firmware updates.

I assume that v4.8 and v4.10 are hardware versions. Is there a guide to help identify which version of VESC I've got?
```

---
## \#7 Posted by: elkick Posted at: 2015-11-06T06:09:47.381Z Reads: 765

```
It's written on your PCB.
```

---
## \#8 Posted by: Pato Posted at: 2015-11-06T09:38:51.075Z Reads: 738

```
How epic is this? For people who aren't familiar with motor control techniques, this is very advanced. It makes an all ready efficient control method (trapezoidal commutation) look basic. Mr Vedder you are a very smart person.

For anyone who wants to understand more on what FOC is, I found these articles give a good overview in regards to BLDC motors. 

http://www.eetimes.com/document.asp?doc_id=1279321

http://www.digikey.com/en/articles/techzone/2011/oct/increasing-motor-performance-with-field-oriented-control

I might write a new Thread on how an ESC works if people are interested? I'll start with an overview/summary and go into more detail if people want to know more.
```

---
## \#9 Posted by: Batou Posted at: 2015-11-06T11:38:19.858Z Reads: 670

```
Hi Pato ! thanks for the links. I Will definitely be interested in a thread explaining how the VESC works !
```

---
## \#10 Posted by: treenutter Posted at: 2015-11-06T15:27:54.213Z Reads: 646

```
@Pato I would also be interested in a summary!
```

---
## \#11 Posted by: treenutter Posted at: 2015-11-06T15:29:56.616Z Reads: 624

```
Thx @elkick . I found it on my PCB. Bah! I'm using hardware version 4.7. @sl33py is it confirmed that only 4.8+ will support FOC? This is the downside of early adoption!
```

---
## \#12 Posted by: elkick Posted at: 2015-11-06T16:24:06.173Z Reads: 596

```
FOC will work on 4.7 too according to Benjamin.
```

---
## \#13 Posted by: treenutter Posted at: 2015-11-06T16:31:22.818Z Reads: 592

```
W00T! Thanks @elkick !
```

---
## \#14 Posted by: cmatson Posted at: 2015-11-06T21:00:23.402Z Reads: 577

```
Agreed- the esc info thread sounds awesome
```

---
## \#15 Posted by: lox897 Posted at: 2015-11-06T22:12:58.346Z Reads: 562

```
I'd love to see that too. Hope you make it soon!
```

---
## \#16 Posted by: Pato Posted at: 2015-11-06T22:19:03.914Z Reads: 554

```
Ok will hopefully have a "How an ESC works" thread in the next few days!
```

---
## \#17 Posted by: jacobbloy Posted at: 2015-11-07T10:13:08.511Z Reads: 563

```
Don't all go rushing to upgrade to the lasted version of FW just because of FOC Vedder is still optimising but to get it working takes a learning curve to get the correct motor parameters, Vedder has sent me the FOC firmware and Iv been spending a lot of time getting my parameters correct! Not every one will have the equipment to do so! So for those who don't think they can do it just hold on to your panties Vedder will make the motor detection incorporate this soon!

For those who can do it make a good video of how to for the rest of us lol! I'll try doing the same once I'm competent I haven't made any mathematic mistakes;)
```

---
## \#18 Posted by: claudiofiore88 Posted at: 2015-11-07T17:47:21.563Z Reads: 551

```
Wow, that's really cool. I didn't know there were other ways to drive a brushless motor. It's amazing how much quieter it got. This could be useful when riding around at night around the neighborhood as to not disturb people sleeping.
```

---
## \#19 Posted by: locktight Posted at: 2015-11-09T23:21:09.409Z Reads: 540

```
Could you update us when he makes it work with motor detection. Or could you tell me where to look for the information. Thanks
```

---
## \#20 Posted by: BigAl Posted at: 2015-11-10T00:40:53.213Z Reads: 532

```
How bout you guys start posting the parameters for the motors you've already tested i.e. the enertion 190kv motors are --- --- --- etc...

BigAl...
```

---
## \#21 Posted by: psychotiller Posted at: 2015-11-10T02:13:31.031Z Reads: 479

```
Most people have, in their build threads, on 2 forums.
```

---
## \#22 Posted by: Braylon31 Posted at: 2015-11-15T07:46:32.065Z Reads: 471

```
By parameters you mean?
```

---
## \#23 Posted by: jacobbloy Posted at: 2015-11-15T09:08:33.050Z Reads: 465

```
FOC parameters are different but if they have been posted that awesome
```

---
## \#24 Posted by: BigAl Posted at: 2015-11-16T21:19:20.603Z Reads: 461

```
@psychotiller do you know of any build threads that have the parameters for the 190kv enertion motors?

Thanks
Al...
```

---
## \#25 Posted by: psychotiller Posted at: 2015-11-16T21:40:16.564Z Reads: 436

```
I would guess @onloop would know that info right off the top of his blue steel melon!
```

---
## \#26 Posted by: onloop Posted at: 2015-11-16T21:56:04.737Z Reads: 420

```
there are no builds using FOC, except vedders
```

---
## \#27 Posted by: BigAl Posted at: 2015-11-16T22:48:42.011Z Reads: 421

```
yeah, I didn't think so but @psychotiller sounded so sure, 2 forums and all!

Al...
```

---
## \#28 Posted by: psychotiller Posted at: 2015-11-16T23:24:29.857Z Reads: 407

```
Oh, I see, that was shit talking. Haha.
```

---
## \#29 Posted by: BigAl Posted at: 2015-11-16T23:35:09.834Z Reads: 414

```
rollin with the punches, I like it!

Al...
```

---
## \#30 Posted by: tomtnt Posted at: 2015-12-09T00:46:41.610Z Reads: 410

```
https://endless-sphere.com/forums/viewtopic.php?f=35&t=63540&start=1325


Looks like Vedder just posted the v2.3 update with FOC!  can't wait until this gets ported over to mac/windows
```

---
## \#31 Posted by: jeroenimo Posted at: 2015-12-09T01:09:55.213Z Reads: 405

```
Compile it on Linux, I usually run Ubuntu in a virtual machine. 

Virtualbox is free, and should work fine...
```

---
## \#32 Posted by: cmatson Posted at: 2015-12-09T03:44:43.653Z Reads: 396

```
Will it be as simple as updating the VESC through the BLDC software, or do you need something extra?
```

---
## \#33 Posted by: elkick Posted at: 2015-12-09T08:08:10.511Z Reads: 389

```
@jacobbloy, thanks again for supporting us with OSX & Win versions. Just a remark: the new OSX...2.3.zip is containing the 1.14 BLDC tool currently.
```

---
## \#34 Posted by: jacobbloy Posted at: 2015-12-09T08:22:02.689Z Reads: 374

```
Thanks I'll fix this.
```

---
## \#35 Posted by: elkick Posted at: 2015-12-09T14:16:35.612Z Reads: 370

```
Sorry Jacob, don't want to bother you: for FW2.3 the default FW-files for FW_46_47 (and FW_48) are missing in the Firmware zip-file.
```

---
## \#36 Posted by: jacobbloy Posted at: 2015-12-09T15:02:57.661Z Reads: 368

```
I took these files direct from GitHub And I have checked they are all there. Please redownload and check again.
```

---
## \#37 Posted by: elkick Posted at: 2015-12-09T15:37:34.433Z Reads: 367

```
Yes, you're right - it seems that I was just mixing it up with the old version somehow.
```

---
## \#38 Posted by: tomtnt Posted at: 2015-12-10T23:15:11.182Z Reads: 375

```
Hi Jacobbloy, Vedder just updated to v2.4 - any chance you can send out the OSX updates?

thanks!
```

---
## \#39 Posted by: Moja Posted at: 2015-12-19T07:13:52.706Z Reads: 392

```
Can Is FOC ready in 2.3? I can see some motor detection dialogue boxes in the tab but Im keen to get some suggestions on how to configure it for the Enertion r-spec 190kv motors
```

---
## \#40 Posted by: Hummie Posted at: 2016-01-04T07:35:35.736Z Reads: 454

```
I downloaded the latest bldc tool for Windows which I got somewhere on this site and I've been running basic bldc.  It has a FOC tab under the motor section and it looks a lot like the bldc tab with what look like tests that can have the results applied.  What to do?  Would my multimeter be good for measuring resistance or is it all done on the pc?  I'm worried I'll fry something at worst or have not ideal settings at best.  
Anyone have advice? The motors are 100kv
```

---
## \#41 Posted by: psychotiller Posted at: 2016-01-04T13:49:15.711Z Reads: 432

```
I had a chance to run the foc tests and apply them to my pneumatic. WOW! SUPER quiet. Almost no cogging from a standstill. This is with 150mm tires. Really impressive.
Running 10s and two 245kv 63mm motors.
```

---
## \#42 Posted by: Alex Posted at: 2016-01-05T02:21:56.507Z Reads: 425

```
Can you guys imagine FOC on hub motors! This has some serious potential for sneaky undercover shiz!
```

---
## \#43 Posted by: Hummie Posted at: 2016-01-05T04:11:18.206Z Reads: 442

```
I find with my hub motors even using the bldc program it's really quiet.  I like the noise actually. Should try foc in a day or two <img src="/uploads/db1493/original/2X/c/cde9bdbe27af7774166da26fdfe11f4bb127856d.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/8/85ef53bc282c9c35e367aaba3a0d07d3ec0ede59.jpeg" width="666" height="500">
```

---
## \#44 Posted by: Fababuba Posted at: 2016-01-05T04:20:37.742Z Reads: 397

```
@Hummie
What company makes those hub motors? I haven't seen them before and they look pretty nice.
```

---
## \#45 Posted by: Alex Posted at: 2016-01-05T04:23:01.798Z Reads: 394

```
I also like the noise but silence might be even more enjoyable. Just curious... Where do you get those cool hub motors?
```

---
## \#46 Posted by: Hummie Posted at: 2016-01-05T05:04:40.250Z Reads: 409

```
We are going to sell them.  There are only four made at this point. I promised people on endless-sphere I'd sell them for the manufacturing cost for the first 100.  I got the inspiration to make them there it was kind of a community project. Maybe hundred bucks as we are waiting on a good wheel manufacturer to give us a price for the rubber so I'm not casting second-rate rubber. After those hundred maybe 150 each 
I'll post up a video here in two days <img src="/uploads/db1493/original/2X/1/1cff5750871c2307e049bcadfcba22c9a0b00ae0.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/d/d5ca85a60f4e69e55d3bbc378c002f421e062c23.jpeg" width="375" height="500">
```

---
## \#47 Posted by: makepeace Posted at: 2016-05-08T15:34:03.892Z Reads: 351

```
What I still want to know, in a nutshell, is: is there an overall benefit of FOC for electric skateboard drives? For sure, I get that we get a quieter ride, but is this the only benefit? As far as I understand, FOC aims to linearlize the motor, and allow us to get max torque at zero speed. Does this factor in to reality. Are there any comprehensive comparisons between FOC and BLDC mode on the VESC to date? It would be really great if someone could do some control tests on a conventional setup (like 10s dual drive 190kv), testing flat land constant velocity performance, uphill constant velocity performance, flat land acceleration from stop, uphill acceleration from stop and then some braking tests, maybe flat land braking from 20km/h, and downhill braking. Would be really interesting to see those results and conclude on whether FOC is useful or not, in terms of performance. I'm still waiting for my VESCs from Enertion, and will happily do those sorts of tests for myself when I get them and post the results unless anyone else is keen to do them sooner?
```

---
## \#48 Posted by: Hummie Posted at: 2016-05-08T15:41:58.821Z Reads: 348

```
I get more power on bldc but the noise, while it sounds kinda nice like a jet engine I still prefer the silence.  I read the FOC is also more efficient.  I've never done testing but will do a bit today if the weather holds.
```

---
## \#49 Posted by: Ulfberht Posted at: 2016-05-08T22:53:52.672Z Reads: 360

```
Thanks @Hummie!! That sounds like something I would really like to know. :thumbsup:
```

---
## \#50 Posted by: laurnts Posted at: 2016-05-09T00:19:32.340Z Reads: 357

```
http://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/3002

This should answer some difficulties in understanding what is FOC
```

---
## \#51 Posted by: makepeace Posted at: 2016-05-09T11:23:23.318Z Reads: 340

```
Saw that @laurnts. I understand what FOC is, but what we want to know is, practically, does it work for us and what are the advantages/drawbacks as proven by testing? There is some science that needs doing.
```

---
## \#52 Posted by: trbt555 Posted at: 2016-05-09T12:20:27.808Z Reads: 344

```
[quote="makepeace, post:51, topic:419"]
Saw that @laurnts. I understand what FOC is, but what we want to know is, practically, does it work for us and what are the advantages/drawbacks as proven by testing?
[/quote]

There have been posts about that in the past.
I can't find the exact post right now but even Vedder himself stated that the advantages for an e-board may be limited to just the silent running. In that post he also states increased heating of the MOSFETS.

I'd also like to hear from an actual user what else is better with FOC compared to BLDC.
```

---
## \#53 Posted by: DeathCookies Posted at: 2016-05-09T12:42:27.526Z Reads: 326

```
FOC has more torque from standstill?
```

---
## \#54 Posted by: laurnts Posted at: 2016-05-09T13:34:44.317Z Reads: 347

```
Its hard to tell without testing equipments to understand FOC performance. I am personally not an electrician, so I couldn't tell alot about it. I think others could have tried, but personally I don't have the knowledge / background / testing tools to conduct the ideal test.

Its understandable that FOC advantage for eBoard is noticeably significant on silent running compared to others. Because lets say to test efficiency wise, it needs to be run for many miles under strict control. Yet the differences could only be ranging from 1% to around 10%, which is not alot for short distance commuter unlike cars in which can travel 10.000km per year.

Since FOC is modulating and not on - off switching, its understandable that is running hotter (phases never power down). In general the whole VESC should be warmer because more calculations are needed / involved. But how warm compared to BLDC could also be not that significant since.

But more torque on lower speed is something I could feel and logically right. Because it provides each ABC phases the right current needed for each rotor position, hence it works so well for torqueing the hell out of motor. However FOC is in a waveform, the amplitude of phases peak point is reduced, thats why less top speed.

The exact detail I can't tell really, should ask Vedder for that.
```

---
## \#55 Posted by: Hummie Posted at: 2016-05-09T15:51:35.954Z Reads: 349

```
I didn't do any testing other than riding around again.  In my experience riding the vesc I've been on bldc maybe 2 percent of the time and I switched to FOC quickly both times I tried because I've been looking for a quiet ride as long as the power is still largely there and it is.  At slow speed the bldc tool doesn't sound nice.  At high speed it kinda does 
For me the fets don't even get warm. The vesc may supposedly be more inefficient but I read the motor is running more efficiently and the system as a whole is therefore more efficient.  
I've read it can be dangerous to the vesc but I haven't had a problem on any of the four vescs I use it. 
I'd like to do some testing though and will have to get another watt meter as my last broke.  What kind of test?  Top speed and distance on one amp hour at 20mph are simple enough.   
Busted my can bus wire connection and waiting for another but if if I can get the hot glue to solve it again I'll at least steal my gf phone for some max speeds
```

---
## \#56 Posted by: Ulfberht Posted at: 2016-05-10T03:01:44.555Z Reads: 339

```
Here's a link to the VESC FOC page! Good stuff!!
http://vedder.se/forums/viewforum.php?f=5
```

---

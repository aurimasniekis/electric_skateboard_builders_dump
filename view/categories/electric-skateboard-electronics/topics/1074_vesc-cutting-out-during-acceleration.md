# VESC cutting out during acceleration

### Replies: 53 Views: 8337

## \#1 Posted by: Ross Posted at: 2016-01-22T00:12:01.084Z Reads: 432

```
Hi Guys,

One of my VESCs (of two connected via can bus) is cutting out during acceleration. It was running fine before. All that has changed is that Im using new batteries (12s Nanotech A-spec). When i connect to BLDC tool and go to real time data there are no error codes on either VESC. Is there anywhere els to look for errors like a log or something? Has anyone else had this issue?

Thanks!
```

---
## \#2 Posted by: Alex Posted at: 2016-01-22T01:42:04.388Z Reads: 426

```
I also have the same issue but I figured it was related to the current limiting feature and learned to deal with it. Mine seams to only do it occasionally. Does it happen to you fairly often?
```

---
## \#3 Posted by: Ross Posted at: 2016-01-22T02:11:23.294Z Reads: 419

```
It dose it every time. when i first turn it on i can use quite a bit of throttle before it cuts out. it will cut out for about 3 seconds then kick back in but each time less throttle can be used before triggering the cutout. after a few times you can barely use any throttle. Seems to be acting like a thermal cut out. I might have to get the thermal camera onto it, see if anythings getting hot.
```

---
## \#4 Posted by: Ross Posted at: 2016-01-22T03:16:40.792Z Reads: 413

```
Just jumped off and flipped her over as soon as it happened to see the red light on the right (master) VESC flash a couple of times then a second later back to green / blue lights and it works again. Looks like its resetting its self upon acceleration.
```

---
## \#5 Posted by: Ross Posted at: 2016-01-22T03:34:08.146Z Reads: 396

```
Is there any way to log the VESC data without having to do all that git hub stuff? I looked at how Vedder did it and the process seemed rather overwhelming.
```

---
## \#6 Posted by: trbt555 Posted at: 2016-01-22T05:53:09.000Z Reads: 393

```
I looked into that recently and apparently the video-logger code is outdated and doesn't work with new fw versions.
There's only one way: ride with a laptop.

Others may correct me here but I don't think the current limiting feature will cause your VESC to cop out the way it did.

I had this issue once, it turned out my voltage cutoff limits were set too high and when accelerating the voltage sagged below the limit.
I never was able to verify whether or not the VESC blinked red though.

I've been testing my dual motor setup with new VESCs from @chaka on the bench lately, and I've seen it happen a couple of times to one VESC.
No clue what's happening though.
```

---
## \#7 Posted by: trbt555 Posted at: 2016-01-22T09:58:19.634Z Reads: 384

```
I just came across [this post][1] on the VESC forum, which might be a clue.

How long are your battery wires ?
Mine are quite long, I might add a few capacitors and see if it changes anything.

  [1]: http://vedder.se/forums/viewtopic.php?f=7&t=53
```

---
## \#8 Posted by: Ross Posted at: 2016-02-08T10:37:18.495Z Reads: 363

```
Well i ordered another VESC and it arrived today. I switched them out and gave it a test ride. While the new board does not cut out, the other one (not the original problem one) now cuts out in the exact same way... :-( But it takes a bit more load before resetting. I'd say its tripping at around 40 amps, where as the one i removed was tripping at around 30 amps. So now i have two VESCs with the same problem. I should also mention that it takes around 1 second of 40 (ish) amp acceleration to trip. if you just flick it on and off quickly it will not trip. My battery wires are 8 AWG and fairly short, maybe 200mm so this is leading me to think that it may be a capacitor related issue? Maybe it only occurs at higher voltages? I am using 12S Lipo. In the thread that trbt555 shared, using larger capacitors fixed the (similar) issue.

Is any one else using 12S lipo and running VESC @ 50 amps max without issue?
```

---
## \#9 Posted by: Ross Posted at: 2016-02-08T10:38:26.871Z Reads: 342

```
Thanks for the link! :-)
```

---
## \#10 Posted by: trbt555 Posted at: 2016-02-08T11:08:15.054Z Reads: 338

```
Did you ever get to the bottom of this ?
If not, post screenshots of your BLDC settings.
Even better, post a link to the XML
```

---
## \#11 Posted by: Ross Posted at: 2016-02-08T11:31:45.296Z Reads: 336

```
Did you see my reply a couple of comments up from todays testing? Will try to get screenshots, but the more i think about it the more i think it has something to do with the new slightly smaller batteries that i am using. Hoping a big capacitor bank will solve it! It was running fine on my original (slightly larger physically) batteries. Although the new ones did cost twice as much! The old batteries (2 x 6s turnigy 45C 4500 mah) had 8 AWG where as the new ones (4 x 3S Nanotech A-Spec 65 - 100 C 4500 mah) have only 10 AWG wires, but they are extremely short (15mm). But again the power cables running back to the controllers are 8 AWG. so i wouldn't have thought that say 60mm of 10 AWG would make any difference.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-02-08T12:03:34.575Z Reads: 330

```
Sorry, I missed that post.
Just wondering, how are you reaching such high currents at 12S ?
I'm 95kg and hardly reach 30A going uphill on my 12S setup.

You could connect the caps from another vesc in parallel to find out if that helps. Heck, you could even connect an unused vesc in parallel just for it's caps.
```

---
## \#13 Posted by: Ross Posted at: 2016-02-08T12:59:00.533Z Reads: 329

```
Using the caps off the other board is a great idea! I hadn't even thought of that, and yeah i can just strap the whole spare VESC to the bottom of the board. Thanks! 

I have a 43" drop deck board and I'm basically trying to get as much acceleration as possible from two motors. Yes, even 40 amps is a great deal of acceleration! especially with 2 motors, it takes practice to be able to use. I could probably just (physically) use 50 amps with the test batteries, 60 was too much, but i think i can work up to it ;-) I like the sound of 6,000 watts haha
```

---
## \#14 Posted by: Moja Posted at: 2016-02-27T03:54:59.604Z Reads: 319

```
Im having a similar problem, I can get both motors running on a bench test. As soon as I go for a ride 10 seconds in the master VESC drops out and I'll get red flashing lights when I accelerate. I had this problem with the slave vesc, I re soldered the wires a bunch of times to rule out and bad wiring problems, ended up shorting it in the process, replaced it and now that motor runs fine. 
 Now the master VESC wont run properly. If I do a motor detection the motor jolts very briefly twice and says "bad motor detection" i can get the motor running again if I reverse the phase of the motor wires and power cycle the vesc a bunch of times, then things will seem fine, I can detect the motor, then again, as soon as I ride it will drop out after a little acceleration and when I throttle it the master VESC flashes red lights (three flashes, break, three flashes). 

 The strange thing is its still talking to the other motor and will spin at the same RPM as the slave motor. It will only spin upto the RPM of the slave motor so power becomes very weak. If I spin the master VESC's motor I can see the slave motor responding to the master motor's RPM through CANBUS. 

Any ideas?
```

---
## \#15 Posted by: Moja Posted at: 2016-02-27T03:56:47.321Z Reads: 304

```
I should add, Im using BLDC 2.8 with 4.10 VESC's with 2.8 firmware. I've tried re installing the firmware a bunch of times, I've had the same problem with multiple firmware and BLDC versions.
```

---
## \#16 Posted by: Hummie Posted at: 2016-02-27T04:56:00.552Z Reads: 303

```
Do your motors get hotter than before?  Sounds like a short
```

---
## \#17 Posted by: Moja Posted at: 2016-03-01T12:42:04.154Z Reads: 308

```
They seem fine, I can run the motors no problem when testing and I can get a few test rides in then the slave VESC will start cutting out and cutting back in seconds later.
```

---
## \#18 Posted by: Hummie Posted at: 2016-03-01T19:08:51.349Z Reads: 315

```
My motor seemed fine during pc testing as well but it's shorted.  Finding out if ur motor is shorted isn't obvious. A multimeter won't register the different phase resistance differences because they're so small. I got an LC meter off eBay for 30$.  It measures inductance and capacitance.  The inductance reading is very accurate and I can see what the problem is. But it would run the test and ride with minimal throttle but more than a bit of throttle and it would coast.  With forced repeated hard acceleration, going not far up a hill, it got very hot <img src="/uploads/db1493/original/2X/5/5181b43faf15137efb28d20adbc89768281e86d5.jpeg" width="666" height="500">
```

---
## \#19 Posted by: Moja Posted at: 2016-03-03T04:57:16.962Z Reads: 318

```
I can run the motor fine with my other VESC so I don't think there are any shorts. I assume the VESC is faulty. Pretty sick of screwing around with VESC's.
```

---
## \#20 Posted by: Dunkirk Posted at: 2016-03-28T20:23:17.651Z Reads: 325

```
I'm having these power cutting issues also. When going at slow speeds at flat area there is no cutouts but when accelerating or going uphill these cutoffs are really bad. My battery wire is pretty long (40cm).

No faultcodes on vesc FW 1.14
Motor max is 60A
Battery max is 40A
I'm running 10s

Does anyone made any solution to this problem? @Ross @Moja  
Sounds like capacitors should help. What kind of capacitors works best?
```

---
## \#21 Posted by: trbt555 Posted at: 2016-03-29T08:39:50.509Z Reads: 305

```
What are your battery voltage cutoff settings ?
I had a similar problem, my battery voltage was sagging too much under load.
Decreasing my lower cutoff limits solved the problem.
```

---
## \#22 Posted by: Dunkirk Posted at: 2016-03-29T09:36:13.886Z Reads: 298

```
I never thought of that. My cutoff start at 35V and ends to 33V. What kind of values you suggest to start with?
```

---
## \#23 Posted by: trbt555 Posted at: 2016-03-29T10:54:06.808Z Reads: 298

```
Which batteries are you using ?
```

---
## \#24 Posted by: Dunkirk Posted at: 2016-03-29T14:00:40.963Z Reads: 302

```
I am using two LG He2 5s2p in series. 

I picked up three 2200uF 50v capacitors and connected them to parallel. The original ones were 680uF 63V <img src="/uploads/db1493/original/2X/d/dc46ff8e0d7ddfaf85e3d4a5b7890cc426abf1ef.JPG" width="690" height="364"><img src="/uploads/db1493/original/2X/8/8de4fa003b06e926b1ff1208deb5a3f84cf041c9.JPG" width="613" height="500">

I will test the board tonight and report the results. If cutoffs still happens I have two 5s 5Ah 25c Zippys to test out.
```

---
## \#25 Posted by: chaka Posted at: 2016-03-29T14:38:35.798Z Reads: 291

```
@Dunkirk Your voltage cuttoff start is too low for a 10s2p he2 pack. Your voltage is going to sag really low when using a lot of throttle. Try setting your battery cutoff start @ 33v and end it @ 30v.  Be mindful of that little pack when you are riding and know that when you mash the throttle your voltage is dropping fast. I would drop your motor max down to 40 or 50 amps to stay safe.
```

---
## \#26 Posted by: Dunkirk Posted at: 2016-03-29T20:08:58.651Z Reads: 296

```
Thank you @chaka! I tried those values and it didn't work. I also tried to put values to zero. Didn't work.

I also tried those two 5s 5Ah 25c Zippys and Vesc is still cutting power.

After that I thought that it must be about the long wire, so I put a shorter wire. No change.
<img src="/uploads/db1493/original/2X/1/134c349568a3f73a517341ea8cc8d42bb7945872.jpeg" width="375" height="500">

Do you guys have any suggestion what to do next or where the problem is?
```

---
## \#27 Posted by: chaka Posted at: 2016-03-29T20:27:57.437Z Reads: 287

```
Are you sure it isn't the kama dropping out? Do you have another controller you can use?
```

---
## \#28 Posted by: Dunkirk Posted at: 2016-03-29T20:40:38.588Z Reads: 287

```
Not sure of that but I can try. The cutoffs are only happening when going over walking speed.
I have a Traxxas controller I try it out tomorrow.
```

---
## \#29 Posted by: Dunkirk Posted at: 2016-03-29T22:29:37.839Z Reads: 297

```
I had to try the Traxxas controller before going to sleep and there was no more cutoffs. Ride was unbelievable smooth! :sunglasses:

Thank you Chaka. You are a great asset to this community!:crown: I would never thought that the Kama is the problem.
```

---
## \#30 Posted by: brun Posted at: 2016-07-29T02:03:58.131Z Reads: 266

```
I just switched from my custom PPM remote (which worked under all loads) to the Karma Nunchuck and now I'm getting this same cutout under load.  I was experiencing this same problem a few months back and fixed it by moving the transmitter outside of the battery/ESC box and shortening the wires between my receiver and the ESC.   My guess is that under load, the high alternating current in the 3 wires was producing lots of interference.  My Hobby King ESC came with a ferrite ring on the PWM/VCC/GND wires that is there to suppress high freq noise.   I'll see if I can eliminate the problem by adding a ring and/or shortenting the wires to the nunchuck receiver.
```

---
## \#31 Posted by: brun Posted at: 2016-07-29T03:12:20.440Z Reads: 260

```
Nope...nope change after I added the ferrite ring.  Going to try a fully shielded connection between the receiver and VESC next.  Urgh!
```

---
## \#32 Posted by: brun Posted at: 2016-07-29T06:03:52.518Z Reads: 266

```
Confirmed it was not a voltage drop issue..  After riding for 4 miles on one battery I could not reproduce the problem.  Then I switched to a fresh battery and I could easily get the board to cut out under high load.
```

---
## \#33 Posted by: backinblack626 Posted at: 2016-10-08T15:26:32.051Z Reads: 232

```
So @brun you are ssaying that you confirmed it to be a bad battery causing your issue? I'm having similar issues with vesc cutting under full load or brake when hot or ridden for a little bit. I have another vesc I'm going to try with same setting and setup to see if it's a hardware issue. Also have another battery I will try as soon as all this rain stops here.
```

---
## \#34 Posted by: brun Posted at: 2016-10-08T19:25:55.170Z Reads: 233

```
No, a fresh battery is worse...pointing to EMI as a more likely issue.  

I thought it might be a power drop in the 5v to the receiver.  I added a 300uF cap to the receiver VCC/GND and didn't help.  Still, could be a big/complete power drop that the caps couldn't handle?  Maybe the ultimate test for the 5v theory is just powering the receiver with 4AA batteries.  

A while back I was having the same cut-out problem using an NRF2401 as a remote-receiver.  So I moved the receiver well away from the ESC (10cm or so) and that worked.  Based on that, I'm kinda convinced it's NOT main battery low-volt condition and has to be related to the remote. It's probably not an EMI issue on the wires running from the VESC to the remote either because the NRF had pretty long wires and it still worked.  

I've tried 10cm wires (same as the NRF) on the wii-mote and no success.  So I think the next thing to try is moving the wii-mote receiver very far....like 30 inch away from the VESC and motor.  Just in case there is some EMI on the wires, maybe try shielded wires, shielded CAT5 would...hard so solder though.  Wrapping the wires a few times around a ferrite ring is one technique too.  Also, maybe try 4AA batteries to run the remote in case it really is a large 5v power supply problem.   

Let me know what you can try.  This remote cut out problem is a plague!    My money is on radio noise.
```

---
## \#35 Posted by: brun Posted at: 2016-10-10T18:15:45.339Z Reads: 218

```
Is it possible to take advantage of the VESC's Positive and Negative ramping that seem to only be configurable in the nunchuck app when using a remote that connects via PPM?   

Otherwise...how do you guys manage smooth acceleration and deceleration using PWM input of the VESC and not get launched off the board if you hit the throttle a little too quickly?   When I used PPM previously, the way-too-fast throttle response was a huge problem...when I switched to the Wiimote, it was an incredible improvement.  Mine is only cutting out on me at very high loads going up steel hills so it's not a complete deal killer.  I'd switch over to PWM but only if I can set the ramping as I can with the Wii mote app.
```

---
## \#36 Posted by: Ross Posted at: 2016-10-27T11:33:42.156Z Reads: 205

```
Hi,

What voltage is everyone experiencing this problem running? I am running 12S and beginning to wonder whether the voltage is just to much. I have noticed the new VESCs are only rated to 10S. Also my VESC actually resets which is what causes my cut outs (which occurs at say 20 amp load) i think i may have said earlier on i replaced one of my VESCs with a new one and the problem did not go away. You can tell if the VESC is resetting by jumping off really quickly and checking the lights. they will be flashing if it resets. But this only lasts about 2-3 seconds so you have to be really quick!

On another note has anyone ever had their board stuck on full throttle!? I have noticed this happen before but only for a fraction of a second. Probably should not have ignored it haha. She took off at high speed today and i took a tumble. Im thinking this is possibly an interference problem. (using a Kama remote)
```

---
## \#37 Posted by: chewydinosaurs Posted at: 2017-01-17T00:53:10.103Z Reads: 182

```
I cant ride longer than 2 seconds while going less than 2mph, sometimes it wont even start from a stop, just jolt and cutout.....hm......running a 6s btw
```

---
## \#38 Posted by: Ackmaniac Posted at: 2017-01-17T01:41:01.830Z Reads: 180

```
Gentleman, please post Screenshots of your VESC settings.
```

---
## \#39 Posted by: chewydinosaurs Posted at: 2017-01-17T02:03:01.250Z Reads: 179

```
Motor runs fine when not connected to wheel but cutsout when connected to the wheel. <img src="/uploads/db1493/original/3X/5/4/5404d44f7726b6018e093a7186f1ed1563f5c7a5.png" width="690" height="388">
```

---
## \#40 Posted by: chewydinosaurs Posted at: 2017-01-17T02:04:02.240Z Reads: 175

```
I can only upload one photo as I'm new but here's another
<img src="/uploads/db1493/original/3X/0/d/0db14429366df2688b70cb799c4948d60311c2f7.png" width="690" height="388">
```

---
## \#41 Posted by: Ackmaniac Posted at: 2017-01-17T02:17:46.802Z Reads: 164

```
The bldc tab would be interesting. And which motors are you running and I guess you have a lipo battery
```

---
## \#42 Posted by: chewydinosaurs Posted at: 2017-01-17T02:54:31.193Z Reads: 172

```
Motor detect failed when connected to wheel, but when off of wheel went fine and applied values. I'm using an sk3 280kv motor with 2x3s lipos in series for a 6s in total. Yeah that's a low powered battery, but I should be able to at least move with a 6s. Could it be my connections? They're pretty much all soldered and seem fine to me but I guess I could redo them. <img src="/uploads/db1493/original/3X/3/b/3b2792200847d708780eefcf4c5e7156f666f008.png" width="690" height="388">
```

---
## \#43 Posted by: chewydinosaurs Posted at: 2017-01-17T05:06:57.441Z Reads: 173

```
I increased batt max to 40a which got me rolling to maybe 3-4mph, but it still cuts out randomly. Sometimes at a standstill it will just cutout without moving, and sometimes it will cutout when I'm just cruising. Ill try and get out tomorrow and test it as I did all this testing inside, but currently I have snow on the ground so I'm not sure.
```

---
## \#44 Posted by: Eboosted Posted at: 2017-01-17T05:22:47.146Z Reads: 172

```
If you fixed the problem by changing the remote, then why are you going back yo Niko kama nunchuck?
```

---
## \#45 Posted by: Eboosted Posted at: 2017-01-17T05:27:23.272Z Reads: 169

```
I'm having a similar issue, but with the Mini trigger Remote, on very light throttle from a dead stop it studders, if I give it more throttle the acceleration is smooth. I wonder if this is something we could set of the bldc tool.
```

---
## \#46 Posted by: Ackmaniac Posted at: 2017-01-17T10:08:09.500Z Reads: 171

```
First of all you should disable the application in the application tab before you run the motor detection. And what happens when you push to a higher speed and then give throttle? Does work then?

You can also try to raise the Startup boost to maybe 0.060. And please post a picture of the PPM tab to see if everything is correct there.
```

---
## \#47 Posted by: whitepony Posted at: 2017-01-17T21:23:24.538Z Reads: 161

```
I had similar issues with battery->vesc power connections too close to the receiver antenna/receiver->vesc connection. the moment you drew too much current, the reception would be busted.
```

---
## \#48 Posted by: chewydinosaurs Posted at: 2017-01-17T21:27:20.400Z Reads: 170

```
<img src="/uploads/db1493/original/3X/2/3/23c1794e647743d9dfba66a42fa226016502b1c3.png" width="690" height="388">
It doesn't matter if I push off and start the motor, or if I just start from a stop, I still get the same cutout result. I do need to replace my 36 spoke gear on my 70mm wheels as I'm getting larger 83mm wheels and my gear isn't exactly lined up on the wheel causing tensions changes in the timing belt. Do you think this could have any problem on it as the tension increases and decreases constantly changing the load on the motor?
```

---
## \#49 Posted by: whitepony Posted at: 2017-01-17T21:32:57.183Z Reads: 167

```
you could always leave your laptop connected to the vesc during these tests and if a cutout happens again, type in  "errors" or "fault" in the console of the BLDC tool to see the last DRV errors and what they were about. if the vesc isnt having any error codes, youll know its your receiver.
```

---
## \#50 Posted by: chewydinosaurs Posted at: 2017-01-17T21:39:57.841Z Reads: 162

```
Where's the console? Sorry I'm sort of new to more in depth programming stuff like consoles and terminals, but for some reason the error box in the real time data is cutoff no matter what way I resize the window. I also moved the receiver to a different area with no changes. The only positive change I can see so far is ever since I increased the max batt voltage I can atleast get going for 5-6 seconds, but then it almost seizes. When It goes out the wheel pretty much locks up and almost throws me off the board. I still think it may have an issue with my belt tension changing since the gear isn't center on the wheel but soon enough I'll have new parts
```

---
## \#51 Posted by: trancejunkiexxl Posted at: 2017-07-04T14:20:17.266Z Reads: 129

```
i know this is old but i found (slow speeds) prone to cogging and stalls but high speeds run fine with larger 63mm motors. So did battery cuttout not improve this problem only switching to another vesc? I also have experienced this and I am very interested in your progress in the last 5 months! Even adding sensor wires does not guarentee a smooth ride =)
```

---
## \#52 Posted by: chewydinosaurs Posted at: 2017-07-04T23:10:25.180Z Reads: 123

```
It was a tension issue, I have a custom motor mount and adding weight on top of the already tight belt cause the motor to just cut out. Loosened the tension and no more issues.
```

---
## \#53 Posted by: FinnishSnowmobiler Posted at: 2017-08-09T23:06:27.959Z Reads: 109

```
After two months of living with this depression causing issue I finally decided to get rid of it. The solution for me was to move the receiver away from the immediate closeness of the VESC. I have always had it sit just centimeters away from the VESC, and only by taping the receiver to the top of the board the issues were reduced dramatically.

I am currently planning on buying a longer wire for the receiver (against every recommendation... "Always keep your wires short, that keeps the problems away", completely new approach and it works!!).

So, apologies for reviving this thread but I really had to post the solution here as I feel it is my obligation. The issue is probably caused by electromagnetic radiation emitted by the VESC in some way. In which, I don't know, I'd be more than happy to read about it.

Cheers from Finland!
```

---

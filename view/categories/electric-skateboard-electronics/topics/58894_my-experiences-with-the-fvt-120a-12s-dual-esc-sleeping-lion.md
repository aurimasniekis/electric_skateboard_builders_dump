# My experiences with the FVT 120A 12S Dual ESC / Sleeping Lion

### Replies: 39 Views: 1960

## \#1 Posted by: nadir35 Posted at: 2018-06-14T19:13:17.672Z Reads: 315

```
Hi everyone,

I would like to share my experience with the FVT 120A Sleeping Lion twin ESC, and give some troubleshooting tips for anyone who considers this ESC.
![image|286x350](upload://4UcZdQXeJF7Evjvdrh5wjLwbnVH.jpg)
I got this ESC from alieexpress, however I saw there is also a version from APS. I chose to go with it since I was looking for a cheap and hopefully simple dual drive solution. I chose the 12s version, however I only used it with an 8s lipo battery. My setup was:2x6355 sk3@260kv, 15Tx36T, 12mm belts.

When I first hooked up everything , it seemed fine when riding. However I quickly noticed an array of problems:

* Problem 1 - The ESCs  were not synced up. One of the motors would start to spin earlier and have more throttle throughout. Individually calibrating the ESCs using the short wires would not solve this.
* Problem 2 - The same ESC taht would start up late would stutter randomly when pushing the throttle at any speed. Those microstutters were really annoying and probably unsafe for unexperienced riders at high speed.
* Problem 3 - I could not get the PC software to work properly with the ESC using the USB-link. I thought I was doing everything right, but I missed a tiny detail I guess..

Now after many emails and chats with the FVT support and my aliexpress seller, I think I finally have fixes for all these problems. I'd also like to add that while experimenting I tried different receivers, motors etc, so I am pretty sure these components were not the problem.

* Solution to problem 1
When having this problem I was hooking up the long signal wire to the receiver. For some reason, this seemed to be the problem. When calibrating each of the ESCs individually using the short wires, they worked fine and had the same throttle response. So my solution was to make a Y cable for the signal wire and feed the signal to the ESCs using the short wires.
* Solution to problem 2
After solving problem 3, the fix to this was to reset firmware back to 170818. The ESCs were shipped with 171103, which according to FVT support was the latest version. Weird :confused:
* Solution to problem 3
While connecting the USB-link to the PC using the short wires, I always had the long signal wire hooked up to the receiver. Apparently that is not ok!

Another thing: FVT support confirmed that it is ok to use the ESC with only 1 motor attached. I was considering this before I found the fixes to my problems :smiley: 

Now with everything solved, I finally have the ESC I expected to get. The throttle is similar to a car esc like HK X-Car Beast and the acceleration is immediate and a ton of fun. The brakes are pretty quiet and strong but take getting used to. At default settings, it builds up progressively for like 80% of the way , but if you push beyond that they get super strong and drag brake (I think), even if you have it turned off in settings.

In retrospect, I think it's probably not worth it to get for about 150€ considering that you can get two HK VESCs for that price. However if you really like the feeling of a car esc, and want to pull a lot of amps and have a lower voltage battery setup I think it can be worthwhile to get this ESC. Let's see how long it lasts for me, for now it only has around 150km on it :slight_smile: But I plan to ride it a lot more and ride it hard, my 12s single 6374 focbox setup feels tame compared to this one^^

Keep on riding!
![image|690x388](upload://sPpFZ7ek1d3XxeZS0BzEIHhprxB.jpg)
```

---
## \#2 Posted by: aMasheep Posted at: 2018-07-13T12:13:25.262Z Reads: 243

```
Hello!
Thank you for writing this. It's very god, but I have a few questions:
When you say short signal wires, do you mean the two wires which have only black and white? And do you now use these two wires for the signal from the remote control with a y-cable? Or do you use the long(glack,red,white) cable as the remote controll wire still?

And if you only use the small ones for the reciever, and for the programming, what do you use the long one for? :open_mouth: 

Best regards, and thanks again.
```

---
## \#3 Posted by: nadir35 Posted at: 2018-07-13T13:20:19.094Z Reads: 223

```
> When you say short signal wires, do you mean the two wires which have only black and white?

yes

> And do you now use these two wires for the signal from the remote control with a y-cable?

exactly

I use the 5v and ground from the long one to power the receiver.
```

---
## \#4 Posted by: aMasheep Posted at: 2018-07-13T13:27:26.649Z Reads: 194

```
Can you take a picture or two of how this is wired? It is a little hard to understand with words.
Thanks for the reply.
```

---
## \#5 Posted by: nadir35 Posted at: 2018-07-13T14:01:27.294Z Reads: 188

```
I can't, the board is for a friend...
I will try to describe:
Receiver pins:
* Signal - Y cable that connects to the white cables of the short wires
* 5v -  red wire from the long cable
* ground - black wire from long cable
```

---
## \#6 Posted by: aMasheep Posted at: 2018-07-19T19:20:57.959Z Reads: 169

```
Thanks alot for the reply! I've been so busy with work so that is why I haven't responded.

It worked perfectly! I did as you said, and reset the controller limits and it now rotates at the same time.

Thanks for your time. Best regards.
```

---
## \#7 Posted by: nadir35 Posted at: 2018-07-19T20:11:37.114Z Reads: 157

```
I'm glad my post could help someone, I wanted to give back to the community that taught me so much in some way and I'm happy I could do so.
```

---
## \#8 Posted by: Randel77 Posted at: 2018-08-02T17:44:05.690Z Reads: 140

```
Thanks for posting this, I just got this esc. It looks like you used an anti spark key on your build. the esc has an on/off switch so I'm wondering if the anti spark is necessary?  TIA!
```

---
## \#9 Posted by: direct_drive Posted at: 2018-08-02T17:56:58.706Z Reads: 144

```
Hey, sorry to potentially hijack things, but could you post a pic or two of your esc and also a link to where you bought it? I've had my eye on this thread and on the sleeping lion for my first build
```

---
## \#10 Posted by: Randel77 Posted at: 2018-08-02T23:47:46.427Z Reads: 148

```
I bought two on alibaba because there was a price break but I should only need one. I could sell you the other one with the usb link if your interested (no mark up lol) but I wouldn't want sell 
 it until I have my board up running so probably two weeks from now, which is about how long it took to get them from china. just let me know. I let the seller (Jenny) know that I was using it for an e-mtb so I'm hopping it has the right firmware flashed already and I don't need to use y cable for the short leads... we''ll see.
```

---
## \#11 Posted by: direct_drive Posted at: 2018-08-03T00:15:45.360Z Reads: 133

```
Hey! Thanks for getting back to me! Sounds like a plan... I'll take it off you (I can wait a couple of weeks). I'll drop you a pm, and if you could send over a couple an idea of price and a shipping cost to the uk that would be superb
```

---
## \#12 Posted by: nadir35 Posted at: 2018-08-03T17:17:54.671Z Reads: 133

```
[quote="Randel77, post:10, topic:58894"]
’m hopping it has the right firmware flashed already and I don’t need to use y cable for the short leads… we’'ll see.
[/quote]
There is some 2.0 something something firmware out on their website now, I tried it. The stuttering issue came back. For me, only 171103 works nicely.
```

---
## \#13 Posted by: nadir35 Posted at: 2018-08-03T17:21:34.902Z Reads: 123

```
I don't think its necessary, but I've read somewhere around here that these switches arent fully reliable or can maybe die after getting used a lot. I have had a similar car ESC for a long while though, and it still works fine, so maybe it is ok.
```

---
## \#14 Posted by: Randel77 Posted at: 2018-08-04T01:01:41.416Z Reads: 113

```
Nice. Thanks for letting me know. Do you know where I could get the firmware that's worked well for you?
```

---
## \#15 Posted by: nadir35 Posted at: 2018-08-04T14:17:37.632Z Reads: 111

```
its on their website under http://szfvt.com/en/download-25-5-6-6.html
```

---
## \#16 Posted by: aMasheep Posted at: 2018-08-05T13:05:08.804Z Reads: 116

```
Hello again!
Altough my project evolves slowly, I've now started testing. I am having some trouble with the ESC.
When It is hard at load, it suddently dies. I also have [this](https://www.amazon.co.uk/gp/product/B01BV3O79O/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1) power analyzer between the battery and the ESC. When the ESC stops under load, the power analyzer also shuts off, even though it is directly connected to the battery. I've tried without the power analyzer, and it still shuts off. Only a replug of the battery will fix it.

Because the power analyzer also blacks out, it leads me to believe that there is big voltage spikes from the motors occuring under load. (Under load means when accelerating from standstill when the motors are sort of "jiggeling" before i start to go forward, and when steep hills/tought terrain occur)
Is there any way I can check for these spikes? And does anyone know how to fix it? 
The only Idea that came to my mind were bigger capacitors for the ESC, which I find a bit risky thinkering with.

Sorry for the long post. 
Best regards.
```

---
## \#17 Posted by: nadir35 Posted at: 2018-08-08T17:50:59.830Z Reads: 100

```
I've maybe had something similar. The ESC blocks both wheels for me when I accelerate really really  hard. My only workaround is to be careful with the trigger.
```

---
## \#18 Posted by: aMasheep Posted at: 2018-08-08T20:07:48.258Z Reads: 102

```
Well, this doesn't look like a block, but more like the ESC shorting out.. What do you think?
```

---
## \#19 Posted by: nadir35 Posted at: 2018-08-09T18:45:21.473Z Reads: 102

```
Yes probably a short of some sorts, only occurs under very heavy load.
```

---
## \#20 Posted by: b1705 Posted at: 2018-08-25T14:40:14.762Z Reads: 100

```
what remote do you use with it?
```

---
## \#21 Posted by: nadir35 Posted at: 2018-08-25T20:49:31.854Z Reads: 92

```
It worked fine with mini remote, nanox remote and gt2b.
```

---
## \#22 Posted by: Randel77 Posted at: 2018-09-25T03:00:15.908Z Reads: 87

```
Hope I'm not hijacking This Thread. I have an update. I finally got my board put together and here's my experience so far, day one.
I bought a Chinese Mountain board with 18650 batteries,12s and 6375 ( non sensored) Motors. Goes 25 miles an hour on a flat surface . I took that setup and installed it on on mBS board.it's a ton of fun and the acceleration and braking is very smooth and reliable but I wanted more power.
 I built my new board with a new mBS comp 95 board with Matrix 2 trucks,2x5000mah lipo batteries, micro remote same as the Chinese board, 10s, Hobbie sky 6384 (sensored Motors) that I ordered on Amazon for about $90 a piece and an SVT sleeping lion twin motor ESC. 
  the new board weighs about 8 pounds less than the old board. Out of the box the board is unrideable / dangerous . I then set the settings with the original firmware that came with the ESC to very soft start, 30% braking, 3% neutral range  3%, throttle limit at 80%, start power at 11 The motors stop and start very close to each other so I did not use a Y connector yet. I haven't been able to use the sensor wires yet because the plug is different on the motor and ESC.
  
   with the new settings the board is much more rideable but still pretty sketchy. With the old board, if you were going 15 miles an hour and you push the throttle up to 100% you wouldn't go flying off the board same with the brakes. With the new board you can't do that or you will go flying. It's controllable but WAY more touchy.
    that's the bad part, the good part is the power borders on obscene!!
     I have a digital level that I used to measure a few hills around the area. I'm not sure how well of an indicator  the level is but on the first Hill the level measured 7.75 degrees. From a dead stop the old board will climb the hill fine but it definitely is  much slower than on a even surface you might get up to 10 or 12 miles an hour. The second Hill measured 16.5 degrees it may not look that steep in the pictures but I assure you it's fairly steep. From a dead stop the old board would climb the hill but maybe at three miles per hour.
     On the new board with the throttle at about 10-20% it will climb both hills like it doesn't know you're on it! no exaggeration , no hyperbole that's a fact. If you were to push the throttle to say 75%, you're going down! same thing with the brakes, they work well but if you push it over 50% you're going to go down.
     I love the amount of power  the new system has, but it is to way punchy! I'm going to contact the vendor to see what can be done but at this point I couldn't recommend the setup. I was worried that two vesc's wouldn't have enough punch but this is ridiculous. I've seen people eat it pretty hard on my old board and that thing is a kitten compared to this thing.
      For reference I'm 165.lbs. lots of High Impact Sports. Dirt bikes,kite boarding, you name it. If the acceleration / breaking was more manageable this thing would be exactly what I was looking for. Any help would be appreciated. Thanks!
```

---
## \#23 Posted by: Randel77 Posted at: 2018-09-25T03:11:52.233Z Reads: 82

```
![IMG_20180924_181613|234x500](upload://4StYn4CaY2G3kzF5EXIvp1OdDSx.jpeg) ![IMG_20180924_181951%20(1)|690x323](upload://vuvlfbylE1mBPbDGW5XuONFeh08.jpeg)
```

---
## \#24 Posted by: artSkate Posted at: 2018-12-11T20:50:46.436Z Reads: 74

```
Hi nadir35.  Art here.  Im trying to program my FVT sleeping lion.  What usb or programming box support FVT Sleeping Lion 5s-12s?  Thanks for your time.
```

---
## \#25 Posted by: bazis Posted at: 2018-12-11T21:28:47.864Z Reads: 74

```
I use this one
 http://s.aliexpress.com/b6BbERJR
```

---
## \#26 Posted by: nadir35 Posted at: 2018-12-11T22:20:29.696Z Reads: 75

```
yea i used this one aswell
```

---
## \#27 Posted by: artSkate Posted at: 2018-12-19T01:33:20.565Z Reads: 72

```
Hi aMasheep, Art here.  Did you ever get your esc set up to run smoothly?  Mine  randomly looses rc signal, and goes into a beeping mode.  It has happened at low and high speeds.  I tried different receivers and different remotes without luck.  Sometimes it work fine.  But its random.  I checked BEC voltage under load, and it remains at 4.92V.  Adjusting BEC voltage with programming software did not change it.  Short theory may be correctl.  I have a battery/cell monitor on my set up.  Sometimes it gives me a low voltage alarm (not at any extreme load) as I lose rc signal.  My battery is 10s5P 15AH-sustains 100A continues or 200A burst.  I dont think a slow speed acceleration would strain that battery.
```

---
## \#28 Posted by: aMasheep Posted at: 2018-12-19T20:23:19.367Z Reads: 69

```
No, that battery should be able to sustain the current draw. I used recycled batteriets from old laptops which sags a lot under load, and I've only managed to pull 1800watts to my knowledge. I do have the problem with the controller loosing connection(obviously from RF congestion) but  I got to borrow one from a friend and it works much better. I have seen dropouts on that one also one time, but I haven't tried to resolve the problem yet. 
What controllers have you tried?

What you can do: try to take the receiver away from the ESC as it can interfere with the signals.

Also, does your dropouts last for 5 sec or is it fast? What firmware do you use?

Please give me more Info, I will try to help as best as I can.
Best regards.
```

---
## \#29 Posted by: artSkate Posted at: 2018-12-19T22:27:10.871Z Reads: 63

```
Thanks for getting back to me.

Im using one of those mini controllers.  (This one I think) :https://www.ebay.com/itm/Mini-2-4Ghz-Remote-Controller-Receiver-ESC-USB-Charging-for-Electric-Skateboard/272826376972?hash=item3f85b8230c:g:ddIAAOSwI4BZskUk:rk:2:pf:0)

  The original receiver for the mini controller did not work properly at all.  I bought a different receiver with a little antennae.  That one worked better.  It does seem like if I (or any part of me) gets in between transmitter and receiver, I loose signal.  Signal loss is brief, just a second or so (at higher speed that is enough to jolt the board hard enough for me to fly off of it.

I tried two different mini controllers without luck.  What controller/receiver worked for you?

I use the firmware that came with the ESC.  It's the same one that fvt website has:  20180614.  It is the only one that fvt website has.

I did move receiver away from the esc.  I think it helped a little.  When I was riding around yesterday (just to test it out) it seemed to come on sometimes when im just getting going, or sometimes when Im cruising at decent speed.  Holding the controller closer to the receiver does work, but I dont want to rely on that for safe riding.
```

---
## \#30 Posted by: aMasheep Posted at: 2018-12-21T00:53:11.581Z Reads: 63

```
Hmm I see.
It really sounds like you just have the same controller reliability issues as me. I've heard that the controller you bought is also all in all a worse controller than the regular mini controller found here: https://www.ebay.com/itm/Electric-Skateboard-2-4GHz-Remote-Controller-Transmitter-Receiver-Binding-Plug/272733085845?epid=20005946328&hash=item3f8028a095:g:rfIAAOSwqxdcB21U

This controller is known for better reliability, although mine was broken.. My friend bought exactly the same one and it's much better.

If you want to fix your existing controller, I can't help you as I don't have a degree in that field.. I've tried some things with mine but it has only made it worse. 

I think your best bet is to go for the remote type I linked you. If you are happy with the firmware then good. I have a couple of other firmwares you can try out if you want, but it probably won't fix the controller issues.

Best regards.
```

---
## \#31 Posted by: artSkate Posted at: 2018-12-21T03:33:35.978Z Reads: 61

```
Thanks for the reply.  I would like to try different software with this esc.  It seems like it may be relevant to my case.  I started a thread with fvt rc issues.  I do think the remote and receiver combo i have is crap.  I did do this alteration, that helped my connectivity a lot.  Ill attach a link to the video.  Basically, I replaced my transmitter antennae.  It extended my range and resolved connectivity problem.  Here is a vid of what I did for the remote and esc.  Ill direct message you my email address.  If you can send me different software versions for this esc, Ill much appreciate it.  Thanks.

https://www.youtube.com/watch?v=uOlDoRoJI6k
```

---
## \#32 Posted by: aMasheep Posted at: 2018-12-21T11:17:30.894Z Reads: 58

```
Looks like a nice ride. Good thinking with the reciever and transmitter!
btw: does your drivetrain make a lot of noise? I am using chains right now and they are kind of loud.. I am thinking about moving to belts, and just buy the wheels you have there off of ali express. But I will first have to smoothen up the ride, as its quite rough and uncontrollable now.

I will send you the firmwares in PM now, If you figure out which of the firmwares that yields a better riding experience, please write back with the firmware and the settings you use, would help a lot :smile: 

Best regards.
```

---
## \#33 Posted by: artSkate Posted at: 2018-12-21T14:40:31.947Z Reads: 53

```
Thanks aMasheep.

Belts are a bit quieter than chains.  I will send you a video with how mine sounds.

With my current set up, the board is rideable.  But is not a forgiving ride.  I rode 5 miles yesterday.  My thumb was numb from trying not to piss off the angry lion.  My legs were smoked because of fast acceleration and breaking.
```

---
## \#34 Posted by: graydonhope Posted at: 2019-05-10T03:29:47.181Z Reads: 33

```
Hey @nadir35 !

I know I am a little late to the party here... So I am building my own board and am considering buying the FVT 120A for my 10s setup. I wanted to know if its possible to control this using an Arduino? I have been struggling to find an ESC that can be controlled by that. I have heard you can do it with VESC's, but it seems a lot more complicated and maybe not ideal for the setup I am trying to make.

Just wanted to know what sort of experience you had with this (if any)..

Thanks!
```

---
## \#35 Posted by: nadir35 Posted at: 2019-05-10T05:27:08.146Z Reads: 31

```
From my experience of trying to make arduino control work with a non-VESC, it is just not worth it. The old fashioned remote and receiver is far less hassle and more reliable. 

I would advise on going the VESC route. I was hesitant at first which led me to getting this ESC, but with current dual VESC prices I don't see a reason to not go the VESC route. It really isnt all that complicated once you put some time into it. (I was afraid of that at first too)
```

---
## \#36 Posted by: graydonhope Posted at: 2019-05-10T14:47:50.031Z Reads: 29

```
Thanks for the answer.. Yeah I believe I am going to go with the VESC, however I just realized my Turnigy Aerodrive SK3 doesn't have some sensor wires? It just has the 3 main wires. Is it still compatible with the VESC? Is it still compatible with using the arduino as well then? Or would my motor need to have these sensor wires?

The wires I am referring to: ![PNG|690x360](upload://2dcNsnB0CuWSZ8wE8ldBFgtJYTE.jpeg)
```

---
## \#37 Posted by: graydonhope Posted at: 2019-05-10T14:51:13.930Z Reads: 30

```
After some further research, I realized that it should still work without those sensor wires it will just be less "smooth". Hopefully it will still be programmable by the Arduino and not too challenging! I plan to use the PPM default settings on the VESC and just attach the signal wire to the arduino.

Thanks again
```

---
## \#38 Posted by: nadir35 Posted at: 2019-05-10T15:29:32.150Z Reads: 27

```
u are right with the sensor wires, however i advise you to do some further arduino research... the signal your arduino will be transmitting will probably have not high enough of a frequency which will lead to motor jitters... atleast thats what i had with a car esc, maybe it works  with vesc
```

---
## \#39 Posted by: graydonhope Posted at: 2019-05-10T16:43:38.163Z Reads: 26

```
That is a great point which I never would have thought about. I looked into it and found a post where someone had a similar issue. The default frequency for the Servo library is 50Hz but can be modified for any value you would like. This specific user changed his to 400Hz as that was the recommended value of his ESC. 

However, he also mentioned that increasing the frequency may cause high current output due to fast phase but his ESc could handle it. How am I able to tell if the VESC can handle high current? 

My apologies for being so new to the topic. Electricity isn't one of my strengths, but I am trying to learn. 

**All in all, I can modify the frequency but it may cause a high current....**
```

---

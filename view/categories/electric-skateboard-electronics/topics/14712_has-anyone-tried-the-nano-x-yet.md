# Has anyone tried the nano-x yet?

### Replies: 96 Views: 5681

## \#1 Posted by: Evan Posted at: 2016-12-15T08:27:43.471Z Reads: 390

```
I've got it, tried it and very satisfied with it. But one thing I would like to discuss is the beginner/expert mode. From the BLDC tool it shows that in the beginner mode the acceleration is smoothly which the maximum throttle percentage is around 83% and brakes gently. On the other hand, expert mode would accelerate like a beast that goes up to 100% right away also brakes like it has a 6 pistons caliper on. 

This morning I pulled my back muscle because hit full throttle accidently in expert mode when I was trying to go forward in the beginning. Which launched the board from me and my body tried balancing it back then. :joy: CRAZY throttle sensitivity.

Anyone used it yet? How do you guys think?

However, this remote is so good that the design of it is so compact and light that couldn't even feel it in my bag. Big thanks to Jason, bring this lovely stuff to us.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-12-15T09:31:26.256Z Reads: 366

```
Did you adjust the PPM settings? Can you post a screenshot of them.
```

---
## \#3 Posted by: Evan Posted at: 2016-12-15T09:38:24.797Z Reads: 362

```
I tried but what I'm trying to say is the original mode setup difference between the expert/beginner when they're made in the remote itself. Couldn't change separately because these two mode were made like this. I'll post some pics later. Been scared to stay in beginner mode now lol.
```

---
## \#4 Posted by: Evan Posted at: 2016-12-15T09:56:25.408Z Reads: 352

```
First one: beginner mode full throttle, second one: expert mode full throttle.
Can't tell much tho.

<img src="/uploads/db1493/original/3X/c/7/c7a3119c2bd384c2b14d42d8eb0b0020e635055a.png" width="690" height="471">

<img src="/uploads/db1493/original/3X/e/e/ee3871c0ef39eecc4ecc8ba8da7fde0e2b44005a.png" width="690" height="465">
```

---
## \#5 Posted by: yaca Posted at: 2016-12-15T10:05:41.304Z Reads: 321

```
Set max Pulsewith to 2,06 and then turn the throttle trim to neutral 50%. After that set min pulsewith.
 
What is your Motor Max value? Try to lower that to calm down the beast.
```

---
## \#6 Posted by: Schulerbible Posted at: 2016-12-15T10:17:35.585Z Reads: 312

```
I just connected the controller to my board and let the motors spin. Feels sooo nice but breaks hard!!! I need to change that before jumping on the board!
```

---
## \#7 Posted by: Evan Posted at: 2016-12-15T10:26:04.296Z Reads: 315

```
Motor max is 50 and brake is 50 as well...yeah I'll try it but that means no 100% output anymore? I'm just amazed by the factory setting of expert mode compares to my old enertion remote which even reacts softer the the beginner mode lol.
```

---
## \#8 Posted by: Evan Posted at: 2016-12-15T10:26:43.208Z Reads: 314

```
Watch your back, I mean literally don't pull your back LAMO. :joy:
```

---
## \#9 Posted by: susplus Posted at: 2016-12-15T10:27:54.373Z Reads: 302

```
still waiting form mine to arrive :( still waiting....still waiting
```

---
## \#10 Posted by: Evan Posted at: 2016-12-15T10:29:33.644Z Reads: 298

```
You'll get it soon don't worry bro. Where you at?
```

---
## \#11 Posted by: Ackmaniac Posted at: 2016-12-15T11:05:49.941Z Reads: 299

```
Can you also post a screenshot when the throttle is in center and another one when the throttle is at full brake.
You can also use my firmware mod to adjust it more precise. Then you would have a center position.
```

---
## \#12 Posted by: yaca Posted at: 2016-12-15T11:41:58.687Z Reads: 297

```
I assume you have an dual motor setup, right? Two vescs with 50 amps motor max in total 100 amps is pretty much (for me). Of course with  2 x 40 amps the board has less power but that's what you want. You can also try the firmware from @Ackmaniac. Here in wattmode you can also reduce the power of the board and the triggerrange is greater. But at first calibrate the remote with the right values of pulsewith and center it with the throttle trim on the remote or as he mentioned in @ackmaniacs firmware you can also adjust center pulsewith.
```

---
## \#13 Posted by: Evan Posted at: 2016-12-15T19:18:29.286Z Reads: 274

```
Well the first thing I did was center the throttle position, it came with like 54% or so? Then I adjusted it but still toooooo powerful. Alright I'll try to lower the motor max, new remote = new setup. I've totally ignored that fact.
```

---
## \#14 Posted by: Evan Posted at: 2016-12-17T22:44:44.968Z Reads: 278

```
Okay so I figured out what's the best configuration for me. Reseted the remote min pulsewidth to 2.10 then max to 1.00 in order to neutral the throttle. After that, seemed like my motor max and mix were too high so downgraded them to 40amp and -20amp. 

Here we are! In beginner mode is easy to ride in urban area which accelerates fine and brakes gently that can allow me to mess around not worry about getting any trouble. Expert mode still works like a beast, instant acceleration and harsh braking - trying not get killed by it!


<img src="/uploads/db1493/original/3X/8/5/858fcb8549032730af71955b8c46e37902a7237c.png" width="666" height="500">

beginner mode:

<img src="/uploads/db1493/original/3X/a/0/a0534048508368ed31d6bd3b8e539656d7b86cb6.png" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/2/02d2e3336c851ed77c9ee556b8e1c0b47636ec54.png" width="666" height="500">

expert mode:

<img src="/uploads/db1493/original/3X/7/1/71299d205703abc03efedff5d871a8895704e20d.png" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/4/44f5b90cb7b8db611d3cdc6cda2aae4b105a9e59.png" width="666" height="500">
```

---
## \#15 Posted by: Ackmaniac Posted at: 2016-12-18T00:12:49.569Z Reads: 237

```
Just a stupid question. But could it be that you always move the thrigger fully. Should mean full brake and fully acceleration? And the correct values for min and max pulsewith would be 1,05 and 2,05. Otherwise you can't brake and accelerate fully.
```

---
## \#16 Posted by: Evan Posted at: 2016-12-18T00:41:35.474Z Reads: 246

```
Uh you mean when I am riding or doing the bldc adjustment? I'm not following your first question bro. And pulsewidth was like, I tried 2.00-2.10 then 2.10 gave me a better throttle range distribution. I'm not a bldc expert at all but I reckon I'm good with this setting? Or 1.05 and 2.05 is really needed? I can still fully accelerate and brake in expert mode.(intense power) But like you said, in beginner mode it runs a bit....kinda soft? Is it normal or...? LOL I'm questioning myself a lot.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2016-12-18T01:05:39.388Z Reads: 254

```
I asked that question because some people use full throttle or fully brake all the time because they think there should be some kind of ramping.
If you want to have less power in expert mode especially at the lower throttle range then i recommend to use my firmware. There you could adjust the throttle curve to your needs.
```

---
## \#18 Posted by: Evan Posted at: 2016-12-18T01:10:01.267Z Reads: 251

```
Oh yeah I got you now.Definitely will give it a shot. Reading your idea right now. SWEET!
```

---
## \#19 Posted by: SeanHacker Posted at: 2016-12-18T01:53:08.452Z Reads: 258

```
@Ackmaniac's firmware/bldc_tool is awesome dude. Definitely give it a try. You will see a MAJOR difference in how you can control your board. I bought a Raptor 1 as my first eboard and it was sooooo crazy in acceleration. I could barely handle it. Threw me off a bunch until I used wattage control. Smooth as ever now.
```

---
## \#20 Posted by: Evan Posted at: 2016-12-18T09:45:16.368Z Reads: 257

```
After spending almost a whole day testing the goodie @Ackmaniac made, I gotta say thank you so much and it literally give a different board to me. Absolutely amazing.

One question : can space cell pro 4 handle 30amps battery max? Dual motors which means 60amps battery max? I've tested it for a couple mins seems okay but kinda wondering.
```

---
## \#21 Posted by: kyo Posted at: 2016-12-18T11:46:03.118Z Reads: 237

```
Can i use this wattage control with nunchuck?
```

---
## \#22 Posted by: Schulerbible Posted at: 2016-12-18T12:50:51.994Z Reads: 235

```
@Evan could you please explain where you downloaded the firmware and how to set that up. I guess all other Nano-X users will face similar issues. That would be fantastic! Maybe with some screenshots about your settings.
```

---
## \#23 Posted by: Ackmaniac Posted at: 2016-12-18T13:15:44.731Z Reads: 238

```
I don't think it is a NANO-X problem. It is the normal behavior of the VESC. And at the beginning you need to get used to the power. But with throttle curve adjustment you can soften the power at lower range without loosing the full power option.

You can get the software here. Nunchuk is also supported. But i never tested it because i have no Nunchuk. It should work but please test it with care. When you buy a HM-10 bluetooth module then you can also connect your Android smartphone to the VESC and watch realtime data, change drive modes and make videos.

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286

PS. Donations are very welcome
[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4R86CGGZDVE9W)
```

---
## \#24 Posted by: Evan Posted at: 2016-12-19T08:48:43.376Z Reads: 227

```
After messing around with the new bldc tool, I've got the best setup I need.
 So I changed the max pulsewidth from 79% to 85% which allowed it has the ability to go uphill with more power also accelerate faster otherwise it would've been like a kid's toy eboard, tooo soft. On the other hand, tuned up the min pulsewidth from 1.05 to 1.25 so even in beginner mode it can still fully stop. Battery max was raised up to 30a then 30*3.7*10S = define batt max to 1110. Remember I use dual enertion motors. Finally, since I had no idea what throttle curve was like, I ended up with duplicating @Ackmaniac's example and it worked perfectly. Without it, nano-x still operates like a wild beast. Probably I will stick in beginner mode forever because expert mode is considerably way too crazy. Now I can die peacefully. :innocent:



 <img src="/uploads/db1493/original/3X/2/8/28116a6ef3fb37afa653aae98b6ddf9273490e45.png" width="666" height="500">


"Beginner mode"
<img src="/uploads/db1493/original/3X/8/f/8f3e3de61e7e5e439dec62e0ca407a39fe2ff241.png" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/8/f800d5a449ca88b3499fd3996550f377ff04481d.png" width="666" height="500">

"Expert mode"
<img src="/uploads/db1493/original/3X/5/c/5cdda4d51ad7f4e5d098b455f87c014b978db0fd.png" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/2/b20bf08541a40b0e1504b99149e899b84778e020.png" width="666" height="500">

Nice curve OH YEAH

<img src="/uploads/db1493/original/3X/4/5/45ebbbbef71a76a774dcd943a8c293f9fd2cc1bd.png" width="666" height="500">
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-12-19T09:04:53.215Z Reads: 196

```
OK, let's make it a bit more complicated.
When you switch to expert mode then i recommend to set the full values for the pulsewidth again, 1,05 and 2.05. Because this way you can use the whole trigger range of the remote.
And at the beginning i recommend to leave the brake curve linear. I changed it in my picture only to show the possibility. You should try it linear first and find out if you want more or less.

And with the throttle curve you can fine tune it.
The way the throttle curve works is the following:
In number **1** of the picture you can see that at 25% throttle you get only 12,5% of the power. When you don't use the throttle curve then you get 25% power because it is linear. So instead of 277 Watt (1100 * 25%) you get 139 Watt (1100 * 12,5%).
In number **2** of the picture you can see that at 50% throttle you get only 32% of the power. When you don't use the throttle curve then you get 50% power because it is linear.  So instead of 555 Watt (1100 * 50%) you get 355 Watt (1100 * 32%).
In number **3** of the picture you can see that at 75% throttle you get only 60% of the power. When you don't use the throttle curve then you get 75% power because it is linear.  So instead of 832 Watt (1100 * 25%) you get 666 Watt (1100 * 60%).

<img src="/uploads/db1493/original/3X/9/b/9b901c9d1396cde432d1acd6bd2565d727640eb6.png" width="527" height="500">
```

---
## \#26 Posted by: Evan Posted at: 2016-12-19T09:53:13.790Z Reads: 189

```
Actually, I always change modes when I'm riding my board. Let's say...when I want to go up a incline or I encounter a strong wind then I will change to expert mode. I had a huge epic crash about 2 months ago and what I learned from it was : son, you can ride your board with slow speed and that's not going to destroy your board. Anyway, @Ackmaniac, your tribute is worthless. Can I cry in your arms?
```

---
## \#27 Posted by: Evan Posted at: 2016-12-19T10:10:56.759Z Reads: 185

```
OH by the way, bldc display shows that even with my setting, in expert mode the throttle can still hit 0% and 100%. Doesn't that mean okay? It counts?
```

---
## \#28 Posted by: Ackmaniac Posted at: 2016-12-19T10:17:01.030Z Reads: 188

```
It just hit's 100 % power at already around 85% throttle in your setup. But don't care right now. First get used to it in beginners mode and when you are ready for it make a new setup for expert mode.
```

---
## \#29 Posted by: Evan Posted at: 2016-12-20T05:11:32.441Z Reads: 182

```
I've got another issue. It had no throttle(brake)-curve when I turned on the board or the remote.(got connected) So I found out that everytime I had to flip up the board then engaged full throttle in order to get acceleration-curve, full brake to get the brake-curve.(even separated)  @Ackmaniac have you ever heard this before? Perhaps only happened with nano-x?
```

---
## \#30 Posted by: Ackmaniac Posted at: 2016-12-20T08:39:16.938Z Reads: 181

```
I don't understand completely. Please be a bit more precise.

The VESC software doesn't give a signal when you go more than 20% below the minimum or over the maximum ppm signal. Because then it thinks your signal gone wild.
So i recommend to set the values to the correct ones. 1,05, 1,54 , 2,05 in your case.
And the throttle curve works as long as there is a ppm signal.
```

---
## \#31 Posted by: Evan Posted at: 2016-12-20T10:49:25.355Z Reads: 170

```
I just tried all the values that correspond with the expert mode, problem still remained. It was like, I let my board rolling while I was standing on it and it was on, then I turned off the remote then turned it back on, it accelerated wild and braked harshly again. I had to fully stop once with full brake-throttle range then used beginner mode(or lifted up the board) to full-throttled it once as well so it could operate as ideal. Uh, not sure what the problem is but I well currently use this method as no other option. :grimacing:
```

---
## \#32 Posted by: Ackmaniac Posted at: 2016-12-20T12:30:12.425Z Reads: 167

```
You should post some screenshots of the ppm screen in full throttle, full brake and idle in expert and in beginner mode. Or get in contact with @onloop because he also lives in Adelaide.
```

---
## \#33 Posted by: Evan Posted at: 2016-12-22T06:57:40.265Z Reads: 162

```
They were as same as I posted....problem still remained. Strange....anybody has this issue aw well?
```

---
## \#34 Posted by: yaca Posted at: 2016-12-22T09:34:46.974Z Reads: 158

```
Did you set the correct values of pulsewith? It's difficult to help if you ignore the advices.
```

---
## \#35 Posted by: Evan Posted at: 2016-12-22T09:59:42.169Z Reads: 168

```
uh I had tried everything even the right setup which was 1.05, 1.54 and 2.05. Now the problem is just it can't initiate throttle-curve if I don't full-accelerate and full-brake in the first bind-to-go process..... Also I used soft rpm limit and it gave me a wonderful control ability, SWEET.

I'm still waiting for more people to get into nano-x and maybe someone will set it up with new bldc tool and engage throttle setup then we can have a discussion about it. Seems like only me getting this issue on forum now.
```

---
## \#36 Posted by: Strawbs Posted at: 2016-12-24T04:09:05.475Z Reads: 161

```
I am unable to bind the Nano-x to my VESC.  Has anyone else had this problem?
```

---
## \#37 Posted by: onloop Posted at: 2016-12-24T04:26:11.681Z Reads: 159

```
[quote="Strawbs, post:36, topic:14712, full:true"]
I am unable to bind the Nano-x to my VESC.  Has anyone else had this problem?
[/quote]

It's automatic, don't do anything & it should work (turn on esc first)
```

---
## \#38 Posted by: Strawbs Posted at: 2016-12-24T20:46:45.149Z Reads: 164

```
I've been trying all morning.  The green light continues to flash.  same with the receiver (red flashing light).  I've let it sit there flashing green for over an hour and still would not connect.  Last night it connected, the motors were spinning and everything. Now, this morning its flashing green again.
```

---
## \#39 Posted by: Strawbs Posted at: 2016-12-24T20:53:00.053Z Reads: 170

```
Ok, I got the remote to bind again just now... But after shutting the board and remote off, and restarting, the remote goes through the binding procedure again, and sometimes will not re-connect.... It seems like the remote will not permanently bind with the receiver.
```

---
## \#40 Posted by: Eboosted Posted at: 2016-12-25T00:43:18.892Z Reads: 171

```
This remote seems to have quite some issues
```

---
## \#41 Posted by: SageTX Posted at: 2016-12-30T18:05:04.059Z Reads: 160

```
I am also unable to bind my controller.  My steps --
1. power receiver with cable to CH1
2. power transmitter.
3. wait
I've tried the bind channel, which will bind the remote (lights stop flashing), but no power when throttle up.
Any suggestions??  @onloop? 

https://www.youtube.com/watch?v=ZSwSttYR1Ic
```

---
## \#42 Posted by: JohnnyMeduse Posted at: 2016-12-30T18:09:50.138Z Reads: 154

```
WAIT........ more time.
```

---
## \#43 Posted by: SageTX Posted at: 2016-12-30T18:18:04.867Z Reads: 156

```
[quote="Blasto, post:354, topic:7891, full:true"]
I did a quick setup video with a brand new nanoX
[/quote]

His bound right up. Been connected for 5 min now.  Still waiting............
```

---
## \#44 Posted by: Blasto Posted at: 2016-12-30T18:18:25.902Z Reads: 158

```
Turn the remote on first, chan1 is the right one
```

---
## \#45 Posted by: SageTX Posted at: 2016-12-30T18:20:17.157Z Reads: 161

```
Trying that now.  still not binding.
```

---
## \#46 Posted by: SageTX Posted at: 2016-12-30T18:26:06.725Z Reads: 165

```
Still nothing. This should be really simple.  Anything else I can try?
```

---
## \#47 Posted by: SageTX Posted at: 2016-12-30T18:59:23.471Z Reads: 162

```
What's this button?  Does this need to be pressed for first time binding?  Maybe mine didn't get connected at the factory??
<img src="/uploads/db1493/original/3X/5/8/58269295ad57ac72e7e1dfb889b3f2c6e3f82f69.jpg" width="690" height="388">
```

---
## \#48 Posted by: JohnnyMeduse Posted at: 2016-12-30T19:08:46.726Z Reads: 164

```
<img src="/uploads/db1493/original/3X/e/c/ecea3def0f5fed4f38db0b23dfeb1377f39467b6.JPG" width="375" height="500">
```

---
## \#49 Posted by: SageTX Posted at: 2016-12-30T19:14:42.563Z Reads: 164

```
Oh. Missed that.  thanks.  Still I can't get it to bind. About to give up.
```

---
## \#50 Posted by: JohnnyMeduse Posted at: 2016-12-30T19:17:10.095Z Reads: 162

```
just close everything down for about 5 to 10 min (take a coffee and refresh your mind before giving up :sunglasses:) then retry using the binding procedure.
```

---
## \#51 Posted by: SageTX Posted at: 2016-12-31T03:35:46.496Z Reads: 162

```
Bound once. (by chance after sitting 8 hours)
Set Min/Max/Center pulswidth
seemed to work fine.

turned off board.
turned on board.

WONT CONNECT!!!!  This is infuriating.  NOTHING has changed.  


Transmitter first --
https://www.youtube.com/watch?v=7Ph02cdSo8E


Receiver (board) First --
https://www.youtube.com/watch?v=KF94Xd-yNGs

Whats the dealio???
```

---
## \#52 Posted by: JohnnyMeduse Posted at: 2016-12-31T03:53:47.018Z Reads: 160

```
can you post some picture

Edit : have you try to reverse you servo connector
```

---
## \#53 Posted by: SageTX Posted at: 2016-12-31T04:42:29.313Z Reads: 162

```
Yes.  I have,  but it connected once and worked once.  Then simply after power off, it wont connect again.   Pics coming,  but you really can't see much.  Vesc side is glued in.  Works with mini remote/receiver. Signal wire is on inside, power  in middle, ground outside, CH1. <img src="/uploads/db1493/original/3X/0/f/0ff5262674bd27c394870d48895ad4866bf9ddfc.jpg" width="281" height="500">
```

---
## \#54 Posted by: SageTX Posted at: 2016-12-31T05:04:55.292Z Reads: 158

```
here's a little longer video of the connection problems.

https://youtu.be/pr31eum9Tbs
```

---
## \#55 Posted by: Blasto Posted at: 2016-12-31T05:22:45.520Z Reads: 155

```
You shouldn't need to physically change the plug. Not sure what it does when it binds in the bind slot...

Just leave it chan1, and give it a min
```

---
## \#56 Posted by: SageTX Posted at: 2016-12-31T05:39:11.673Z Reads: 158

```
I've done that.  It just won't connect.
```

---
## \#57 Posted by: Blasto Posted at: 2016-12-31T05:43:40.382Z Reads: 160

```
How about a real boring 3min video of it trying to bind on chan1 only, nothing else, just let it blink
```

---
## \#58 Posted by: SageTX Posted at: 2016-12-31T06:19:22.341Z Reads: 164

```
Here it is. 
First 3.5 min board first. 
Second 3.5 min remote first 

https://youtu.be/LiPB3fBELYw
```

---
## \#59 Posted by: Blasto Posted at: 2016-12-31T07:06:02.827Z Reads: 164

```
Huh... something wrong here, well you have all your evidence to contact support with
```

---
## \#60 Posted by: RadElectrics Posted at: 2016-12-31T09:21:21.740Z Reads: 161

```
I have the new nano-x remote, and I'd like to use in my Raptor 1, from Enertion, (Build, October 2016).

How can I remove the winning Bluetooth console from my board without major surgery?  The wires have been set in with black hot glue.  On the console as well as on the vesc... 

I also want to put connectors on the ends of the wires to make it easier to do this next time...

Reading through this thread does give me some concern though....  Will it even work once I've went through the trouble of installing the nano?
```

---
## \#61 Posted by: Ackmaniac Posted at: 2016-12-31T10:15:52.787Z Reads: 154

```
I see that you have a Bluetooth module connected to the VESC. Can you please remove that one and try the bind process again. There shouldn't be any interference with the receiver and I never experienced a problem but who knows.
```

---
## \#62 Posted by: i2oadsweepei2 Posted at: 2016-12-31T14:09:29.692Z Reads: 150

```
I use spectrum 2.4g radios and receivers in rc's. Sometimes the radio and receiver don't like to be close when binding. I've helped a few people solve their problem by asking them to stand back 10' when turning on the remote. When all else is failing, just try it.
Good luck. I have one coming too...
```

---
## \#63 Posted by: SageTX Posted at: 2016-12-31T17:10:59.899Z Reads: 149

```
Just tried disconnecting bluetooth. still won't connect.
```

---
## \#64 Posted by: SageTX Posted at: 2016-12-31T17:12:45.317Z Reads: 145

```
Just tried the distance test. Still won't connect.
```

---
## \#65 Posted by: i2oadsweepei2 Posted at: 2016-12-31T17:34:36.999Z Reads: 146

```
Bummer. I'll be watching this to see if you have any luck. All the best and Happy New Year.
```

---
## \#66 Posted by: JohnnyMeduse Posted at: 2016-12-31T17:35:02.645Z Reads: 146

```
have you try to charge the remote.. or maybe try to contact enertion support.
```

---
## \#67 Posted by: SageTX Posted at: 2016-12-31T17:38:07.192Z Reads: 150

```
Fully charged remote during this process, after first initial try to bind.  Just contacted Enertion Support for help and directed them to this chain.
```

---
## \#68 Posted by: SageTX Posted at: 2016-12-31T18:07:45.199Z Reads: 150

```
Just for comparison, so all other things can be disregarded, here is a short clip with the Mini remote sync.

https://www.youtube.com/watch?v=j_IiQRXUfC0
```

---
## \#69 Posted by: nick191 Posted at: 2017-01-02T10:21:57.511Z Reads: 139

```
Mine is doing the same as yours and enertion support linked me to this is there a solution? @SageTX
```

---
## \#70 Posted by: fedestanco Posted at: 2017-01-02T12:32:53.885Z Reads: 138

```
I saw you are using transparent hot glue to keep the connector steady. By experience I can tell you that 80% of transparent hot glue in the market IS NOT ELECTRICAL INSULATOR. If this is your case, you are probably shorting some wires of the servo.
```

---
## \#71 Posted by: SageTX Posted at: 2017-01-03T03:17:18.419Z Reads: 129

```
[quote="fedestanco, post:70, topic:14712"]
80% of transparent hot glue in the market IS NOT ELECTRICAL INSULATOR
[/quote]

Wow. This I did not know.  I was just using it for vibration control. I'll remove it and see if it helps.

This did not help, however, the MIni remote works just fine, so shouldn't be the problem.
```

---
## \#72 Posted by: Blasto Posted at: 2017-01-03T03:22:16.378Z Reads: 131

```
Hey i just had the situation where my nanoX was not connecting. I got pissed and moved the receiver away from the vesc and it connected....

@SageTX
```

---
## \#73 Posted by: SageTX Posted at: 2017-01-03T03:33:25.399Z Reads: 131

```
this didn't work.  put receiver outside of enclosure, still no dice.
```

---
## \#74 Posted by: SageTX Posted at: 2017-01-03T06:05:13.136Z Reads: 130

```
Not yet....
```

---
## \#75 Posted by: PXSS Posted at: 2017-01-03T06:10:23.062Z Reads: 130

```
Dude. You need to get refunded...
```

---
## \#76 Posted by: nick191 Posted at: 2017-01-04T11:18:52.332Z Reads: 126

```
@onloop any easy fix???
```

---
## \#77 Posted by: ghola36 Posted at: 2017-01-06T06:24:36.147Z Reads: 124

```
Is anyone else who pre-ordered still waiting for their nano-x?
```

---
## \#78 Posted by: Kaden56 Posted at: 2017-01-06T07:21:32.561Z Reads: 125

```
I'm am back and forth on whether or not to take the nano x out of it's box with all of the bind issues i've been seeing. My electronics are a pretty tight fit in my enclosure so I don't love taking the enclosure on and off. Should I do it or just stick with my gt2b?!
```

---
## \#79 Posted by: Kaden56 Posted at: 2017-01-06T21:37:31.632Z Reads: 122

```
My enclosure isn't the easiest to take on and off and now I wish I wouldn't have taken it off and just stuck with the gt2b. I'm getting the same problems as everyone else with binding. Any ideas? Binds first time, then never again.
```

---
## \#80 Posted by: mmaner Posted at: 2017-01-06T22:42:07.272Z Reads: 124

```
I just connected Enertion Nano-X and had binding issues.  I moved the RX away from the VESC and issues are gone.  I don't know if that's because of proximity to the VESC or if the connector cable needs to be straight (looped wire, induction effect?).  I've turned it ON/OFF over a dozen times, no issues at all.
```

---
## \#81 Posted by: Blasto Posted at: 2017-01-07T07:18:43.778Z Reads: 121

```
I just got the Channel 2 function to work, the output is a 0-5V DC signal and not a ppm signal. So you can connect it directly to a small 5V relay to control leds
```

---
## \#82 Posted by: Eboosted Posted at: 2017-01-07T13:48:20.236Z Reads: 120

```
Has anyone got any luck with the nano x or everyone has binding issues?
```

---
## \#83 Posted by: i2oadsweepei2 Posted at: 2017-01-07T14:10:40.079Z Reads: 117

```
I got mine yesterday from the group buy. If I have time today I'll try to set it up and report back.
```

---
## \#84 Posted by: Hardwiring Posted at: 2017-03-29T10:21:09.377Z Reads: 96

```
So how are nano-x controllers surviving out there in the wild?
```

---
## \#85 Posted by: Pr0dy Posted at: 2017-03-29T10:30:42.325Z Reads: 104

```
It's pretty great, I got no issues so far :)
```

---
## \#86 Posted by: Tuomalar Posted at: 2017-03-29T11:01:25.343Z Reads: 104

```
Still waiting rest of my parts... However my nano-x binded right away when i connected it.
```

---
## \#87 Posted by: fraannk Posted at: 2017-03-29T11:02:55.492Z Reads: 104

```
I ordered mine in January, but haven't got it yet. I really hope the get stock at the 31st of March..
```

---
## \#88 Posted by: Tuomalar Posted at: 2017-03-29T11:04:16.416Z Reads: 103

```
You should contact Enertion and ask where your remote is.
```

---
## \#89 Posted by: fraannk Posted at: 2017-03-29T11:05:03.245Z Reads: 102

```
I did, and they said it was because of the chinese new year. :)
```

---
## \#90 Posted by: Hardwiring Posted at: 2017-03-29T13:19:49.671Z Reads: 100

```
Thanks, how often are you having to charge the little beauty?  Also that range do get?
Thanks
```

---
## \#91 Posted by: FinnishSnowmobiler Posted at: 2017-04-02T15:00:42.351Z Reads: 97

```
Hi,

I tried contacting Enertion in their chat. I asked if the schedule for nano-x's is still valid. What I got in response was a simple yes. Hopefully they arrive soon as I'm stoked to get my board's final component!
```

---
## \#92 Posted by: will_manners Posted at: 2017-04-09T12:56:31.138Z Reads: 94

```
So I'm currently considering a GT2B mod or this. Honestly I think I'd prefer a GT2B but the only issue is that the mod for these costs an exorbitant amount of money in Australia, to the point where the nano-x is substantially cheaper than the GT2B mod. 

Although I am hesitant after reading all the binding issues people had with theirs. Is it safe to assume that all of its issues have been ironed out by this stage?
```

---
## \#93 Posted by: fraannk Posted at: 2017-04-09T13:16:04.513Z Reads: 90

```
Well, I don't believe anyone has got any of the new batch, since it has been out of stock for 4 months now. I'm still waiting for mine and I ordered early January...
```

---
## \#94 Posted by: will_manners Posted at: 2017-04-09T13:19:58.024Z Reads: 90

```
Well Jason's website stock should've arrived on the 31st last month so I'd imagine people will be getting theirs soon.
```

---
## \#95 Posted by: fraannk Posted at: 2017-04-09T13:22:41.765Z Reads: 90

```
I messaged them, and they haven't received them yet. They should be there soon though. :)
```

---
## \#96 Posted by: FinnishSnowmobiler Posted at: 2017-04-18T17:22:25.702Z Reads: 81

```


Hi @onloop, 

When can we expect the nano-x controllers to ship?

Kindly, Finnishsnowmobiler
```

---

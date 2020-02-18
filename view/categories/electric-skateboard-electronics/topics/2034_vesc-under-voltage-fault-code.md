# Vesc UNDER_VOLTAGE fault code

### Replies: 20 Views: 2452

## \#1 Posted by: evoheyax Posted at: 2016-03-29T03:35:27.341Z Reads: 192

```
After an amazing, fast and fun ride up a long gradual uphill, my master vesc seems to have kicked itself to the curb.

Having just hooked it up to see the fault code, I am getting an UNDER_VOLTAGE fault code.

Visually inspecting the vesc, it seems good. I can't find anything that looks loose, or burnt.

I was riding fine one second, seemed to hit the heat limit, then cut off and now, I get no motor movement.

btw, using carvon dual + space cell + dual vesc, issue is with the master vesc.

What does this mean and what can be done? Below are my settings, please let me know if you see something wrong.

<img src="/uploads/db1493/original/2X/1/1c179ca4b2ee8b1be8faad174b0bec7c153c76b5.png" width="690" height="342"><img src="/uploads/db1493/original/2X/3/37a841634c8867633b90bdc89b4ad18313736fa3.png" width="690" height="341"><img src="/uploads/db1493/original/2X/1/120ef4a48b277b20601e8ac55dc8aa2e802bf58a.png" width="690" height="330">
```

---
## \#2 Posted by: chaka Posted at: 2016-03-29T14:28:24.739Z Reads: 171

```
Do you have any scorching on the top right side of your drv8302? Any reason why you have your battery max set at 15 amps! That is really low and it has been a common theme in a lot of VESC failures. The battery pack you are using should handle 60 amps but I do not know what the bms is set to for overcurrent protection.

I have a feeling you never overheated your vesc and were experiencing a backoff strategy from having such a low battery max.
 
I personally have not blown a VESC but I never limit my battery max any lower than my motor max. I use really big battery packs with 12s 90amp bms modules so I do not need to compromise my settings with low battery current limits.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-03-29T15:25:15.331Z Reads: 168

```
The reason is because of the space cell. I'm splitting the space cell current between 2 VESC. The space cell has a 30 amp fuse, so I can't draw more than 30 amps or I'll blow the fuse. This means I can't draw more than 15 amps per VESC, or combined, they will go over the 30 amo fuse and blow it. I'm starting to regret buying a space cell and thinking I should have just built my own battery.

These are what onloop recommends as VESC space cell settings.

I don't see any marks near the dvr, that was the first place I was checked, expecting a scorch mark, as I have seen in others.

I will contact onloop about it and see what can be done. If he can't offer any help, I will buy my next VESC from you, as you seem to offer a better warranty against this fragile board.
```

---
## \#4 Posted by: chaka Posted at: 2016-03-29T17:11:47.062Z Reads: 156

```
I wouldn't give up on that pack just yet. You can probably lower the motor current down to 30 amps on each VESC and be trouble free.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-03-29T17:56:15.277Z Reads: 148

```
Should I switch the 30 amp fuse with a 60 amp fuse?

You said lower to 30 amp per VESC, do you mean increase? Since I'm only at 15 amps per VESC now.

Also, do you offer a VESC repair service? I need to get up and running ASAP, as I'm back to taking the bus again.
```

---
## \#6 Posted by: RunPlayBack Posted at: 2016-03-29T19:15:25.354Z Reads: 146

```
Sorry to hear that man, seems like you were getting some good mileage too :( I'm running almost the same settings except I have:

Battery cut off start: 35.20 V
Battery cut off end: 33.20 V

I am curious as well about the optimized Bat Max: 30 amps for the Space Cell BMS. Do belt drive and hub motors generate the same exact draw from the battery? Can we raise Bat Max past 30 amps or is that asking for trouble? Maybe @onloop can help?
```

---
## \#7 Posted by: chaka Posted at: 2016-03-29T20:22:06.695Z Reads: 139

```
@evoheyax Sorry but I only service hardware made here in the shop. 

@RunPlayBack is running more aggressive settings than you and not having issues. 

Is there a chance you might just have a poor motor wire connection somewhere?
```

---
## \#8 Posted by: evoheyax Posted at: 2016-03-29T20:47:32.657Z Reads: 136

```
Possible, but unlikely. I spent quite a bit of time soldering every wire together. I made sure every joint was clean and well connected.

Assuming onloop won't help me out here, what is your warranty on your vescs?

I think its definitely linked whatever is causing the vesc to ramp back on hills. The problem occurred while climbing a hill, just after experiencing a slow down by the vesc. I had been climbing an uphill of 2-3% grade for at least 2 miles straight.

The reality is, onloop looks at his situation and not all possibilities. That is quite clear from his raptor fiasco. Why would you ever build a battery only capable of pulling 15 amps per motor on a dual drive?

The reality is, I was fine riding on flat ground, and even short hills. The problem is when I encounter these 2+ mile long hills that most people don't live around.

You have think outside the box to test all circumstances possible (This is the argument we discussed in my software development class today, which is more or less the same for any product, be it software or physical), and having had no feedback from onloop in the past few days since having vesc issue, and lots from you chaka, I don't see why I should buy onloops vescs anymore.

I didn't expect this to happen, as I was assured by onloops comments that the space cell + dual vescs configured correctly are pretty much guaranteed to work well. I configured it as onloop as stated, was very careful handling them (I know all about esd from working on computers, and used a regulated lab power supply), soldered carefully, yet I'm still faced with 2 broken vescs. (one was broken on arrival due getting 3.2 volts instead ofo 5 on the ppm). Yet through all of my problems, I have have yet to even get a peep from onloop. Having had his back through everything lately, I starting too fall onto the other side now.

Now the balls in your hands @onloop. What will you do?
```

---
## \#9 Posted by: chaka Posted at: 2016-03-29T22:27:10.963Z Reads: 128

```
> what is your warranty on your vescs?

Basically if you buy a VESC from me and it stops working, send it to me and I will bring it back to life. I may charge a little for components if it was an obvious short circuit due to user error or something similar but I haven't found the need to do so yet.

I wouldn't be too hard on Jason. He most likely is taking a little time to recoup. I am sure he will get back to you soon.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-03-30T01:25:07.126Z Reads: 121

```
From what he's said before once you flash your vesc's firmware you void your warranty with him which is stupid because I can't connect and configure to test them until I flash the firmware (at least with mine, since they had a super old firmware).

How much quickly can you ship to San Francisco if I ordered one today? I believe the other should still work since I'm not getting any error codes from it. After having this happen, I'm fine paying more to have the peace of mind if the VESC can really break this easily.
```

---
## \#11 Posted by: cmatson Posted at: 2016-03-30T02:12:39.302Z Reads: 129

```
[quote="evoheyax, post:10, topic:2034"]
From what he's said before once you flash your vesc's firmware you void your warranty with him which is stupid because I can't connect and configure to test them until I flash the firmware 
[/quote]

It is pretty easy to mess up a firmware update, so I'm assuming that is the logic behind it. If you were to (as a result of a user error) incorrectly update the firmware and then want a replacement this is his way to work around that. Plus, there have been a lot of weird things with FOC being super picky and killing DRV chips.. 

As for the VESC's shutting off, it seems unlikely that if it happens so quickly on your board, @onloop hasn't ever seen this problem on his Raptor. My point is, I don't think he'd make a space cell with this ratings, recommend those settings, and build raptors with the same space cell if he knew the settings couldn't be handled by the VESC's.

 I mean he has been preaching the whole idea of going higher voltage to decrease heat and amp draw for a while now.. 

Do you think as @chaka suggested it could be because your VESC's can't breathe enough in your CNC'd deck? even with a fan I don't how much it'd really help without adequate airflow.   

What firmware version did yours come with anyways?
```

---
## \#12 Posted by: onloop Posted at: 2016-03-30T02:28:22.114Z Reads: 124

```
Hi @evoheyax.

this statement from @chaka seems fairly spot on to me.

[quote="evoheyax, post:8, topic:2034"]
The reality is, I was fine riding on flat ground, and even short hills. The problem is when I encounter these 2+ mile long hills that most people don't live around.
[/quote]

[quote="chaka, post:2, topic:2034"]
I have a feeling you never overheated your vesc and were experiencing a backoff strategy from having such a low battery max.
[/quote]

**Warning rant coming...**

Firstly, I would love to be able to offer an unlimited warranty, solve everyone's faults instantly & repair everyone's DIY eboards for them free of charge. The issue with that is my business would shut down within weeks and my overall customer service would be terrible, I am a one man band.. I also seriously doubt @chaka would be willing offer this service unless you can prove that the VESC is actually the problem.

The reality is at some point in this diyesk8 game people need to take some responsibility, they need to understand that they are basically constructing eboards out of various mixed parts that have never been tested together, some parts are hand made in people's garages, this stuff is all relatively new & perhaps even considered experimental so unknown faults are 100% guaranteed to happen. Let me reiterate, I guarantee that some people will have failures! Especially when mixing parts. If you want me to fix your eboard you need to buy a raptor, then any fault is covered by warranty and you wont pay a cent.

Moving on, Lets delve into the Carvon motors for a minute. Firstly, They have never been tested by the maker with the VESC, the VESC designer has also never tested the Carvon connected to the VESC, I have never tested the VESC, Space Cell Or Carvon hubs together. So your board is an experiment.

Lets get technical, the motors themselves are retro-fitted hobbyking brushless outrunners with a outwheel bolted on, they are 149KV which is nearly double what they need to be with a 90mm wheel diameter...

 - the theoretical carvon hub motor top speed with space cell is 57mph (66mp if bat fully charged) - that is ridiculous
 - there is no mechanical torque advantage - huge current draw, low RPM
 - the vesc is a current (15A per motor) bottleneck - motors can't draw enough current to reach optimal RPM

the fact that this setup is even working is a surprise...

I have been working with hub motors for over a year now... getting ones to work well is very very very complex!

Don't get me wrong, I feel for you, I understand your frustration & I apologise that your board isn't working...

**But I cannot take responsibility for it, the ball is in your court.**


----------


[quote="evoheyax, post:8, topic:2034"]
Assuming onloop won't help me out here

The reality is, onloop looks at his situation and not all possibilities. That is quite clear from his raptor fiasco. Why would you ever build a battery only capable of pulling 15 amps per motor on a dual drive?
[/quote]

I designed an efficient system that works very well with my parts, pumping high amps is not the solution, it took years of trial & error & testing... If you would like to send your entire board to me, ill diagnose the fault, i'll redesign the power system and ill define the maximum limitations that the product can work too, I'll build in safety functions to prevent it from failing and catching on fire. I will make it as perfect as possible, however ill have to charge you a consultancy fee and it will take several months maybe a year.
```

---
## \#13 Posted by: evoheyax Posted at: 2016-03-30T03:10:12.344Z Reads: 108

```
I don't expect you to make my board work. I did take a risk, in the sense that this is a new territory. However, I need to make the best of the situation.

To me, this means 2 thing:
- paying extra to have a warranty.
- trying to max my amp output to the motors.

carvon motors can take 80 amps per motor max, vesc can take 50 max, the bms of the space cell can take 60 amps, or 30 amps per motor. So my question is, can I replace the 30 amp circuit breaker with a 60 amp circuit breaker. Or do you know of any reason why this would not work? I'm worried about the gauge of the wire not being able to handle the increased current. Besides reselling the space cell, which is perfect in every other way besides this current limitation, this seems like the next obvious choice. Obviously, that would void my warranty, which I'm fine with, since I know this battery doesn't seem to have any faults. And yes, that would be an experiment and would be on me, regardless of what you say. but what is your opinion @onloop?

What I think I'm frustrated about is it the vesc has all these limits to PREVENT it from breaking. If I set them right, hitting that limit should not break it. And if hitting one of those limits CAN break it, then it should be noted somewhere that anyone can find. I feel like the vesc information is scarce and scattered. There is no list that breaks down fault codes, and finding everything I needed to get it up and running is scared among 10 threads, and vedders site. Now thats not your fault @onloop, but its something I see is easy to change.
```

---
## \#14 Posted by: evoheyax Posted at: 2016-03-30T03:36:27.439Z Reads: 111

```
The firmware was 1.14. The only mac bldc tool I could find was 2.15, so I had to update to that before I could use it. I understand its easy to mess up. But maybe ship them with the current version of firmware?

I have said this before and will say it again, I would gladly pay another $10 or $15 to know I have the latest firmware and that it has been tested to work before shipping.

Also, the manufacturing defect rate may only be 3%, but that is not the rate of people having issues with the vesc. I can't say what it is, but having read all material on this forum and on vedders site before even turning one on, taking every precaution possible, and to end up with one doa and the other now broken, and all the other complaints, that 3% is quite low. I have a feeling that many mess it up and never say anything, so getting an accurate % of people having issues at some point in time with the vesc is difficult.  But its surely higher than 3%, or else charging almost double for a no questions asked warranty makes no sense.
```

---
## \#15 Posted by: cmatson Posted at: 2016-03-30T04:09:09.187Z Reads: 107

```
I completely agree that a lot of people have killed a VESC.. heck, I wrecked my first Enertion VESC. But I'd say it's mostly user error as opposed to factory defects and untested scenarios like yours. 

As for the BLDC tool, i'm currently using the v1.14 on my macbook pro with both of my VESC's- besides the one port issue that was explained in the mac BLDC tool thread it hasn't given me any problems. Not trying to shoot you down by any means- just saying the 1.14 on Mac isn't *tooo* hard to find. 

All that said, I am 100% in agreement with your warranty point. I think a prime solution would be to offer two different VESC options: one, just the baseline cheapo with a simple warranty against factory faults. The second, a more extensive warranty that covers things like DRV faults for something like the first year (I'd say if nothing goes wrong in the first year, then you've got the VESC down pretty good and don't need the warranty beyond that).
```

---
## \#16 Posted by: onloop Posted at: 2016-03-30T08:16:49.375Z Reads: 104

```

You could bypass the BMS for discharge, then just use current limiting in the VESC. Set it to 30A each motor and see how it goes..

The likely problem is that you are using a motor that will always be running suboptimally. They are not really designed for hill climbing, the motor KV is very high for a hub motor. Its max RPM at that voltage is around 6200. I would imagine during your hill climb that RPM is only around 1500RPM.

I am not an electronics engineer, but I assume that your motor is constantly trying to spin faster to reduce the load but it can't because there is no more current being sent to it. So the result is an error.

I would image you want your motor spinning at or near its MAX RPM so that it is running efficiently.... If you send more current it might help the motor to spin faster... But there is also a chance it doesn't have enough torque at that voltage to climb the hill any faster, the load is not being reduced & the motor cannot ever reach its optimal RPM range. That is why it is important to build the motor for the task or use gearing to reduce the RPM.

I am sure someone else could probably explain this better. I just know that motors like to spin at their optimal RPM. Your motors can't.
```

---
## \#17 Posted by: evoheyax Posted at: 2016-03-30T16:41:03.125Z Reads: 96

```
I can see what your saying. I can only get 5 miles or 25 minutes of riding time per charge. But after a good push, the power is pretty good, and I can go plenty fast. Maybe 5 seconds to get up to 25 mph. I was cruising up that slight hill at 30 mph. The rush at those speeds 😛

Do I need to bypass the bms? From what I've read the bms can support 60 amps of discharge, so shouldn't I be able to pull 30 amps per motor through the bms @onloop?
```

---
## \#18 Posted by: cmatson Posted at: 2016-04-04T02:10:08.992Z Reads: 83

```

I believe the reasoning behind the 30amp fuse is that a 60amp fuse can burst higher than it is rated for a split second before blowing. 

Bursting over 60 amps for any amount of time would kill the BMS, so the safe option was to go 30 amps. 

I would start by simply taking out the fuse, and running the VESC's with 30amps a piece. Then, if that doesn't work for any  given reason, it isn't difficult to open up the battery and just bypass the BMS at the source.
```

---
## \#19 Posted by: evoheyax Posted at: 2016-04-04T04:14:47.231Z Reads: 80

```
That makes sense. But if it bursts more than 60 amps, that would kill thhe BMS, so wouldn't the best option be to just bypass the BMS and power the VESCs without the BMS?

Thank you for your input :)
```

---
## \#20 Posted by: cmatson Posted at: 2016-04-04T04:42:02.392Z Reads: 77

```
You could go either way: I'd just set the VESC's to max out at 60amps and use the BMS at first. 

Maybe even set each VESC to 28amps instead of 30 to give yourself a little breathing room.. 

Like I said though, internally bypassing the BMS isn't difficult, so if you just wanted to go that route from the start, you could always do that as well. It would just be a matter of cutting open the space cell, routing both the positive and negative leads (coming directly from the cells) around the BMS, and then taping it back up.
```

---

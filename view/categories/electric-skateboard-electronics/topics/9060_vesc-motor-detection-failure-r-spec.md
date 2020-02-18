# VESC motor detection failure - R-SPEC

### Replies: 61 Views: 4515

## \#1 Posted by: arfintr Posted at: 2016-09-06T13:38:53.520Z Reads: 284

```
Here's the background:
-New VESC out of the box 2 weeks on the shelf in the garage.
-Re-soldered my own battery connector
-Soldered on the included motor bullets
-Plugged into my enertion r-spec 6374
-Set the BLDC software to approximate values for a 4s battery
-Had bad motor detection no matter what values i played around with.
-The motor "kicks" or stutters initially, then stops immediately
-Then for the slow run, i get a stuttery slow crawl
-Tried restarting vesc, un plugging, the usual

I am completely lost as to what to do next...
Thanks for the help...
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-09-06T13:55:00.529Z Reads: 272

```
[quote="arfintr, post:1, topic:9060"]
-Set the BLDC software to approximate values for a 4s battery
[/quote]

What exactly did you do in this step?
```

---
## \#3 Posted by: Blasto Posted at: 2016-09-06T13:58:35.841Z Reads: 265

```
Leave your "maximum input voltage" at 57V
```

---
## \#4 Posted by: Rikki Posted at: 2016-09-06T22:02:42.066Z Reads: 256

```
Afrin, and I are working on this together.
4s battery values were things like the battery cut offs. So i changed them to suit a 4s.
I also tried changing the maximum input voltage back to 57V.
Motor is still clunking just as before...
Still getting the "bad motor detection" text
Any other thoughts/solutions???
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-09-06T22:08:37.226Z Reads: 248

```
Maybe it is you battery... your motor is probably to much demanding on the current and the battery can't provide enough power, I have the same problem using 3S for R-spec motor.
```

---
## \#6 Posted by: Rikki Posted at: 2016-09-06T23:14:36.990Z Reads: 245

```
It should be able to handle the current... I have seen people run the exact same setup with a 4s. I have an extra 4s battery, so I guess I charge it up and run them both in series. So you were having the exact same problem? What battery did you use that fixed your problem?
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-09-06T23:35:50.638Z Reads: 241

```
A custom 10s4p, I'm usually using the 3s to do motor detection and test vesc with a small 5065 motor, but on r-spec that doesn't work, these motor are just beast.
```

---
## \#8 Posted by: Rikki Posted at: 2016-09-06T23:59:52.245Z Reads: 235

```
Thanks for the tip, I give it a try when I get home.
The motor does spin when I use 4s, it just jumps and stutters.
When I use the arrows keys, it stutter once, then runs smooth if I hold the key.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-09-07T00:08:35.763Z Reads: 228

```
because, when you use the arrow, your taking max 3amp, a motor detection can draw more than that
```

---
## \#10 Posted by: Hummie Posted at: 2016-09-07T06:40:52.185Z Reads: 219

```
When u do the test for FOC check the resistance and inductance numbers and compare it to a known good motor that's the same model
```

---
## \#11 Posted by: Rikki Posted at: 2016-09-07T07:35:45.806Z Reads: 207

```
Bit of an update.
I ran the test again this afternoon and i noticed in the real time data the fault code "abs_over_current"
The current spiked at around 32 amps.
```

---
## \#12 Posted by: baxter Posted at: 2016-09-07T10:18:26.956Z Reads: 193

```
Have you tried updating the firmware on the vesc?
```

---
## \#13 Posted by: Rikki Posted at: 2016-09-07T10:47:37.221Z Reads: 183

```
No I haven't tried that yet. Is that easy to do, as I have not looked into it.
My VESC is a 4.12 if that helps. I was hoping to leave firmware updates and such as more of a last option and try to fix the issues by ensuring setting/batteries/connections are correct.
```

---
## \#14 Posted by: baxter Posted at: 2016-09-07T10:51:37.019Z Reads: 176

```
It is easy, but be careful. I am sure you will find a thread on the forum for how to do it.
```

---
## \#15 Posted by: Rikki Posted at: 2016-09-07T10:55:37.807Z Reads: 169

```
My vesc is on 4.18 firmware right now. Is there a more recent one??
```

---
## \#16 Posted by: PB1 Posted at: 2016-09-07T11:03:50.535Z Reads: 176

```
Hi Rikki, I've seen the same issue when I tried to configure my VESCs using one 4S or 5S battery. "motor detection failed". Also R-SPECs and other motors. 

In my case the solution was to configure the VESC with the full 10S voltage. Before I used the full voltage I triple checked that everything was correct. 


Disclaimers: I'm no real expert in VESC, but got all of my 5 VESCs working in various builds. 
I know that some people recommend (or used to recommend) that it's better to configure a VESC using a lower voltage or lab power supply. This didn't work for me. 

Procedure that worked for me: 
- triple check everything will be connected properly
- hook up battery, VESC and motor (no belt)
- set low voltage cut-offs according to your battery pack (edited: leave upper voltage limit @ 57v according to @chaka)  
- set battery and motor amps limits to a low value (e.g. 10 amps, just to be cautios)
- run motor detection
- set battery amps and motor amps to desired / recommended values

One more thing: make sure that the shrink wrap on your R-SPEC is ok and cannot come loose.
```

---
## \#17 Posted by: Rikki Posted at: 2016-09-07T11:13:40.258Z Reads: 168

```
Yeah I've got 2 4s batteries that I will hook up as soon as I get connectors tomorrow.
Did all 5 of yours vesc's have the same issue on 4-5s?
```

---
## \#18 Posted by: PB1 Posted at: 2016-09-07T11:29:31.398Z Reads: 165

```
Hmmm, first I tried motor detection using a 14V or so power supply. I could set the values and program the VESC, but no motor detection. Just stuttering or not even that. This was with an SK3 6364 213kv
Then used 3 4S in series for 12S to do that motor detection and it worked. 

Exactly the same for another single motor build, this time with a big R-SPEC and 10S. Again tried with the power supply, then one 5S battery, didn't work. I could read and write the values, but no motor detection. 

Then the same with my hummie hubs. 

So now I just use the power supply for initial hook-up, checking FW and values, setting initial values. 
Than use the full battery pack for motor detection as described above.
```

---
## \#19 Posted by: Rikki Posted at: 2016-09-07T11:34:32.332Z Reads: 162

```
I hope 8s will be ok, because that is what i have and plan to run.
```

---
## \#20 Posted by: Blasto Posted at: 2016-09-07T12:39:09.785Z Reads: 164

```
[quote="Rikki, post:11, topic:9060"]
fault code "abs_over_current"The current spiked at around 32 amps.
[/quote]

Did you change the abs max current? Should stay at 130A
```

---
## \#21 Posted by: bigpianist Posted at: 2016-09-07T12:52:01.469Z Reads: 156

```
Your VESCS may have the current ramp bug in their firmware. I know this because mine did this. Check this post>>     http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262         
If you're not careful you can burn out your DRV chip while doing motor detections.
```

---
## \#22 Posted by: Blasto Posted at: 2016-09-07T13:07:18.400Z Reads: 151

```
[quote="bigpianist, post:21, topic:9060"]
Your VESCS may have the current ramp bug in their firmware. I know this because mine did this.
[/quote]

This wouldn't affect the motor detection
```

---
## \#23 Posted by: bigpianist Posted at: 2016-09-07T13:13:37.011Z Reads: 149

```
[quote="Blasto, post:22, topic:9060"]
This wouldn't affect the motor detection
[/quote]

Are you sure? The "spike" in current could be because the Vesc is ramping it up too fast because of the bug. This is the only explanation I have from my experiences.
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2016-09-07T13:48:11.925Z Reads: 143

```
This bug have been correct in the new 2.18 firmware. And like @Blasto said it shouldn't affect the motor detection.
```

---
## \#25 Posted by: chaka Posted at: 2016-09-07T14:43:06.717Z Reads: 143

```
Please don't recommend resetting the max voltage limit. This is bad practice and can lead to a a total loss of brakes. The max voltage limit is to protect the vesc components, leave it at 57v.
```

---
## \#26 Posted by: PB1 Posted at: 2016-09-07T15:37:47.693Z Reads: 137

```
Ok,  thanks for letting us know.  Suppose we all need our brakes.
```

---
## \#27 Posted by: chaka Posted at: 2016-09-07T15:41:56.444Z Reads: 137

```
If you are running huge motors you may want to drop it down to 55v if you are running 12s. You can get some really quick spikes in voltage that could pop some components during throttle bursts and sudden braking. Sometimes the stm chip can't react fast enough to protect the components so a little more buffer is good...sometimes.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-09-07T15:42:56.038Z Reads: 135

```
I did all my Vesc setup including motor detection with a Lab power supply set at 12v with no problems at all. 
The 32a during motor detection seems way off. 
Maybe a short in the motor or bad solder joint on phase wires.
```

---
## \#29 Posted by: Rikki Posted at: 2016-09-07T21:16:28.312Z Reads: 132

```
How much amperage should an r-spec motor be drawing in a motor detection?
```

---
## \#30 Posted by: Namasaki Posted at: 2016-09-08T13:18:11.989Z Reads: 128

```
My power supply only delivers 5a max. 
So I'm guessing the motor detection should draw less than 5a at 12v
```

---
## \#31 Posted by: Jinra Posted at: 2016-09-08T13:51:26.112Z Reads: 128

```
You set detection current. It should be at 3A by default
```

---
## \#32 Posted by: DeathCookies Posted at: 2016-09-08T13:52:39.118Z Reads: 126

```
You got it working with a power supply 12V 5A?
I have read these days that many people have problems with detection when they use a low voltage (  <4S )
```

---
## \#33 Posted by: Namasaki Posted at: 2016-09-08T15:34:59.498Z Reads: 125

```
Chaka uses 12v. I just followed his lead and it worked perfectly on both of my dual Vescs and AP 190kv motors.
```

---
## \#34 Posted by: Namasaki Posted at: 2016-09-08T15:40:31.899Z Reads: 126

```
Where exactly is that setting on bldc tool?
```

---
## \#35 Posted by: DeathCookies Posted at: 2016-09-08T20:19:11.993Z Reads: 128

```
[quote="Namasaki, post:34, topic:9060, full:true"]
Where exactly is that setting on bldc tool?
[/quote]

Next to the button "start detection" is a value input called "Current". I think 6A is standard.
```

---
## \#36 Posted by: Rikki Posted at: 2016-09-09T10:17:58.882Z Reads: 126

```
This evening I tried the detection test with 8s
I still had spikes of 32amps during the test.
I then tried using the arrow keys. I had spikes of 20amps. 
Both of these tests were with the tested till test amp level at 6.0 amps.
Here is a video of the test, I'm not sure what going on and I hope the sound helps to diagnose the problem.

The first 3 runs are from the detection test and the rest are from me pressing the arrow keys.
```

---
## \#37 Posted by: Jinra Posted at: 2016-09-09T10:39:28.237Z Reads: 131

```
sounds normal to me. It always takes more energy to start up a motor from standstill. Having a burst for a small fraction of a second is normal.
```

---
## \#38 Posted by: Rikki Posted at: 2016-09-09T10:41:31.777Z Reads: 135

```
The motor is still "spluttering"
I'm working on the video
The test keeps failing
```

---
## \#39 Posted by: Jinra Posted at: 2016-09-09T10:48:34.696Z Reads: 141

```
Ah got it. Wasn't aware of context. Is this sensorless, and have you tried swapping the phase wires around?
```

---
## \#40 Posted by: Rikki Posted at: 2016-09-09T10:57:06.295Z Reads: 152

```
Its an R-spec motor and yeah and do you mean the wires going to the motor?
```

---
## \#41 Posted by: Rikki Posted at: 2016-09-09T10:58:42.233Z Reads: 150

```
https://vimeo.com/182071790
Thats the video with the motor detection first, then 4 times where i held the arrow keys
```

---
## \#42 Posted by: Jinra Posted at: 2016-09-09T12:29:51.953Z Reads: 144

```
careful holding the truck like that while the motor is spinning, another member of the forum gashed up his thumb really bad doing the exact same thing. When you turn the motor by hand (still connected) does it spin pretty freely, or is there resistance when you turn?
```

---
## \#43 Posted by: Rikki Posted at: 2016-09-09T12:31:17.228Z Reads: 140

```
It spins freely and smooth.
No resistance
```

---
## \#44 Posted by: Blasto Posted at: 2016-09-09T12:39:53.113Z Reads: 134

```
Is your detection current set at 6A? Try to increase it to 7-8A
```

---
## \#45 Posted by: Rikki Posted at: 2016-09-10T00:23:12.759Z Reads: 129

```
Tried swapping wires around - Same error
Tried setting it to 7-8A - Same error
Ive contacted enertion, they said I could claim my warranty and get a new vesc shipped to me.
I really have no clue what else to try...?????
```

---
## \#46 Posted by: Blasto Posted at: 2016-09-10T00:29:02.972Z Reads: 126

```
Well fuck... My last guess would be a cold solder on the shunts...

If you want to try to fix yourself, apply only flux on the shunt pads, and reflow the solder
```

---
## \#47 Posted by: JohnnyMeduse Posted at: 2016-09-10T00:29:06.506Z Reads: 125

```
sound like a bad VESC ... do you have any picture ? Also for safety reason, you should not try to hold by hand the motor and the trucks.
```

---
## \#48 Posted by: Rikki Posted at: 2016-09-10T05:58:15.711Z Reads: 127

```
<img src="/uploads/db1493/original/3X/1/0/10ef10cd08bd04fb6b3265f226ab8f0821c64645.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/a/a/aafd98ead8776b044afed4eaf6f6d6e9c69a6a69.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/3/c/3c33ecb28eba30f9fe285759573a3d44e9d54df7.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/7/3/7365e3d7a6b00d1f95701d4860f9325bb045f8b9.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/1/b/1bf1ddc5a4c40ad23d717ba79861cd880bff4335.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/c/7/c77f0db523e035273c61c58f40bba1e51c84c910.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/3/2/32191dd3a6bb6928e7852d9429f282c2cb84e7cb.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/a/3/a35d4cbe0a2f1e04adfe3329321717091f1b93d2.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/9/5/95f164c1f49b5ab7c2fb326dd128371c6320f2a8.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/7/8/781e7d8320cfabae162db0c6c2f6ab2e9e813d16.jpg" width="669" height="499"><img src="/uploads/db1493/original/3X/c/e/cec68645ca022a445fe4c5b3b018e57e52c1cc3c.jpg" width="669" height="499">
```

---
## \#49 Posted by: Hummie Posted at: 2016-09-10T06:49:53.029Z Reads: 120

```
Do the FOC test and get the resistance and inductance numbers and compare them to the same model. 
Did u do the FOC test?
```

---
## \#50 Posted by: Rikki Posted at: 2016-09-10T06:58:24.508Z Reads: 119

```
I haven't tried a FOC test.
Will I be able to do one even if my normal motor detection test doesn't work?
```

---
## \#51 Posted by: Rikki Posted at: 2016-09-10T07:05:00.769Z Reads: 124

```
I've read that switching from BLDC to FOC can be bad for a VESC.
What do I need to do to ensure that I'm not damaging anything on the VESC?
```

---
## \#52 Posted by: Hummie Posted at: 2016-09-10T15:18:29.900Z Reads: 120

```
I don't know if it wil work or if it even has to work to get those two numbers. 

The risks I'm not sure but I think u redownload or reboot or something. I never had a problem going back and forth
```

---
## \#53 Posted by: lospollos Posted at: 2016-09-23T17:45:14.486Z Reads: 105

```
I didn't get my motor detection to work either with a 3s battery. But I can still ride the thing pretty smoothly without having done the detection. Not sure if it's a good idea though...
```

---
## \#54 Posted by: Blasto Posted at: 2016-09-23T18:40:16.453Z Reads: 107

```
When doing your detection w a 3S, make sure your minimum input voltage is set to 10V. You might be hitting a lvco state
```

---
## \#55 Posted by: lospollos Posted at: 2016-09-23T18:49:24.163Z Reads: 108

```
I had it at default which is 8V I think.
```

---
## \#56 Posted by: Blasto Posted at: 2016-09-23T18:51:50.713Z Reads: 107

```
Also set 3S values for "battery cutoff start & end"
```

---
## \#57 Posted by: lospollos Posted at: 2016-09-26T19:21:24.591Z Reads: 106

```
Thanks for the tip, I got the motor detection to work now. I also had ppm app set to "current no reverse with brake" the first time i tried it, so that might have been another issue.
```

---
## \#58 Posted by: Mikenopolis Posted at: 2018-04-18T02:16:04.096Z Reads: 45

```
These motors were working before I took it off and shipped it back to Carvon to upgrade from V3 to V4. I thought I would just plug back in and it would work since it was just an wheel adapter change and not hall sensor or motor change...it just stuttered so now I’m starting over. Emphasis on starting, since motor detection fail (Video). 

This is a 10a3p 25r pack with FocBoxes. FOC, sensors. Any ideas?

https://youtu.be/XlHTI3LVVxA
```

---
## \#60 Posted by: JohnnyMeduse Posted at: 2018-04-18T02:24:03.963Z Reads: 46

```
Sorry .... 

Put the D value it higher up to 0,1 or 0,15 and increase the ERPM to 500
```

---
## \#61 Posted by: Mikenopolis Posted at: 2018-04-18T02:39:12.668Z Reads: 44

```
Thanks I’ll try that later. I’m assuming it’s the same with FOC? The video was BLDC just for test...FOC was failing detection as well
```

---
## \#62 Posted by: JohnnyMeduse Posted at: 2018-04-18T02:55:15.634Z Reads: 43

```
Did you have the R=0 problem ??? If so, Use @Ackmaniac because that a firmware issue from vedder firmware
```

---

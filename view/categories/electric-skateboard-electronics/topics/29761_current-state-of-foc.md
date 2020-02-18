# Current state of FOC?

### Replies: 47 Views: 2046

## \#1 Posted by: lilracerboi Posted at: 2017-08-05T03:59:59.630Z Reads: 213

```
What's the current state of FOC? If there's any at all.
I've got one of @chaka's  sensored motors and have been running it sensorless.
Decided I'd like to try sensored and figured I'd also try out FOC again, though I don't know if sensored and FOC are good together.

This brings me to my question above. It's been awhile since FOC was introduced, so I figured the testing phase should be long gone.
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-05T04:04:39.813Z Reads: 213

```
what vesc do you have?
```

---
## \#3 Posted by: lilracerboi Posted at: 2017-08-05T04:18:00.212Z Reads: 206

```
It's a 4.12 HW from @torqueboards. I know the newer ones run better than it.
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-05T04:20:04.887Z Reads: 204

```
I wouldn't try FOC with anything other than an Ollin, Enertion (FOCBOX), or Axle VESC. And even then I'd only try it out running sub 55k eRPM, most likely hubs for me.
```

---
## \#5 Posted by: lilracerboi Posted at: 2017-08-05T04:22:58.923Z Reads: 196

```
Figured as much. Too broke for one of those right now, but I want one in the future so I can build another board from old parts.

Thanks for the info.

Edit: Is the Raptor 2 running FOC? I'd assume so 'cause, you know....."FOCBOX".
```

---
## \#6 Posted by: torqueboards Posted at: 2017-08-05T04:34:40.719Z Reads: 193

```
I have a few setups on FOC and FOC Sensored and personally I don't have much issues running in FOC. If you program it correctly it should be perfectly fine.
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-05T04:59:49.123Z Reads: 191

```
Yes it is. 

@torqueboards Hey Dexter, what voltage and kv are you running?
```

---
## \#8 Posted by: torqueboards Posted at: 2017-08-05T05:21:31.841Z Reads: 187

```
12S on 75KV Hub Motors or 6355 190KV on 12S.
```

---
## \#9 Posted by: scepterr Posted at: 2017-08-05T05:23:37.836Z Reads: 188

```
I'm using a FOCBOX with an E-Go2 motor in FOC sensored for the past week with no issue with as much abuse as I can put it through, though it is a relatively low power motor.
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-05T05:23:40.034Z Reads: 186

```
Guess it's a toss up :P I'll probably run it on my hubs on my next build
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-08-05T05:28:07.794Z Reads: 185

```
I want to run FOC on my 10s dual FOCBOX 6374 190kv build but I'm terrrified of killing one!
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2017-08-05T05:29:30.346Z Reads: 180

```
running FOC mode on FOCBOX with TB 6355.. its sick and fast on 12s. too fast for me, once you get going it ramps up very quickly.. starts need a lil push when unsensored for me, but the acceleration is fun.
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-08-05T05:30:02.187Z Reads: 177

```
Foc??

10 char
```

---
## \#14 Posted by: Jinra Posted at: 2017-08-05T05:30:03.540Z Reads: 174

```
FOCBOX has a transistor that shuts off before your drv can fry, you should be safe with it.
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-08-05T05:30:46.273Z Reads: 174

```
That is good news!
```

---
## \#16 Posted by: Aggdaddy Posted at: 2017-08-05T05:46:33.355Z Reads: 171

```
running FOC on dual vesc-x 10s5p, dual 6355 190kv   sensored.

no issues.

max speed attained 28mph.  195lb rider.

Gets too wobbly beyond that speed.  I might be able to get it to go faster if I tighten up the trucks, but 28mph is good enough for me.
```

---
## \#17 Posted by: Jinra Posted at: 2017-08-05T05:48:34.467Z Reads: 163

```
I have a drag race against the Raptor 2 this sunday.. I might switch to FOC for the extra low end torque everyone talks about...
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-08-05T05:56:59.392Z Reads: 161

```
I just built a 10s2p lipo pack that is 10ah and 150c. I really want to make it 3p 15ah and run FOC for torque!
```

---
## \#19 Posted by: Yecrtz Posted at: 2017-08-05T06:31:34.225Z Reads: 157

```
Using FOC now for 9 months without issues with torqueboards vesc. 192kv/10s. Just make sure you properly do your detection. And maybe some luck (some nasty stories are drifting around here).
```

---
## \#20 Posted by: jbruce Posted at: 2017-08-05T06:43:50.781Z Reads: 156

```
@Jinra @chaka 
Do ollin vescs also have the transistor that shuts off before the drv could get fried?
```

---
## \#21 Posted by: pennyboard Posted at: 2017-08-05T07:05:05.054Z Reads: 152

```
I've been running 6s FOC sensored on one of your July 2016 vescs with your 6355 motor. 
So far it's run great, and I'm planning on upping it to 12s in a few days. Can you for-see me having any problems with that?
```

---
## \#22 Posted by: lilracerboi Posted at: 2017-08-05T23:09:04.162Z Reads: 126

```
Thanks for the inputs.
Seems like it'd be alright to use, but I'll give it a try when I get a spare VESC in my hands.
Can't risk burning this one.

Running noise less at low speeds is great for campus riding, but not necessary.
```

---
## \#23 Posted by: Jinra Posted at: 2017-08-05T23:44:06.463Z Reads: 122

```
Welp, just tried out some FOC on my 10s 230kv board with @chaka VESCs and it starts stuttering at 47k eRPM and throws an overcurrent fault

>Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 269.9
Current filtered : 130.8
Voltage          : 31.28
Duty             : 0.79
RPM              : 47556.9
Tacho            : 28178
Cycles running   : 14
TIM duty         : 6595
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 32.23

Gonna stop trying before I burn my DRV. Guess FOC is a no go on this board.
```

---
## \#24 Posted by: trancejunkiexxl Posted at: 2017-08-06T05:35:12.795Z Reads: 110

```
damn dude did you get ejected from board ?
```

---
## \#25 Posted by: Jinra Posted at: 2017-08-06T05:37:31.572Z Reads: 109

```
No this was bench testing. I don't ride unless I'm sure it works fine on bench.
```

---
## \#26 Posted by: trancejunkiexxl Posted at: 2017-08-06T05:39:12.286Z Reads: 109

```
i should have bench tested, i went straight for a ride and got ejected! XD my motor max is too high though i think.. this time i had protection lol
```

---
## \#27 Posted by: Jinra Posted at: 2017-08-06T05:41:01.642Z Reads: 105

```
I think I'll only ever use FOC on hubs on VESC4's given the drastically lower eRPM.
```

---
## \#28 Posted by: Eboosted Posted at: 2017-08-06T05:55:29.453Z Reads: 108

```
@Jinra what setup are you going to run against the Raptor 2? Your current setup is always the most reliable, bad things usually happen with cars (I work in a performance car shop) everybody always want to tweek settings to the max before a drag race and those are the ones that first fail on the road, you don't want to experiment that with your board on a public race. 

I'd up the VESC settings and beat the shit out of the board riding it for at least 1 full day, then, if everything works perfect, I'll set up the race.
```

---
## \#29 Posted by: Jinra Posted at: 2017-08-06T05:57:48.279Z Reads: 110

```
I changed it back to BLDC, just thought i'd see how FOC works, but I guess it doesn't.. at least on my setup. I'm pretty sure I set everything up right.

I'm 10s 230kv BLDC running hybrid sensors. One of the mini-usb ports on my Ollin VESC broke off, so I had to replace one of them with an Axle VESC. Other than that the only change I made was upping the max current ramp setup another .02 to .1 now.
```

---
## \#30 Posted by: chaka Posted at: 2017-08-06T06:33:38.436Z Reads: 108

```
FOC detection can be difficult on smaller diameter motors. The bldc tools can sometimes give the wrong settings by reading the resistance incorrectly.
```

---
## \#31 Posted by: Jinra Posted at: 2017-08-06T06:35:33.106Z Reads: 108

```
I ran detection on 6355's. Did it a couple times as well to make sure the discrepancy wasn't too drastic.
```

---
## \#32 Posted by: chaka Posted at: 2017-08-06T06:39:12.021Z Reads: 107

```
Like I said it is hit or miss. I have found that with the correct settings FOC will work fine with most motors. Finding the correct settings with detection alone can be difficult.
```

---
## \#33 Posted by: Jinra Posted at: 2017-08-06T06:47:20.156Z Reads: 100

```
Aw well, guess it wasn't meant to be then.
```

---
## \#34 Posted by: Eboosted Posted at: 2017-08-06T07:09:55.558Z Reads: 99

```
15/36 pulleys on 97mm ABECs?
```

---
## \#35 Posted by: Jinra Posted at: 2017-08-06T07:10:13.356Z Reads: 99

```
Yes, but they weren't on when I was testing.
```

---
## \#36 Posted by: Eboosted Posted at: 2017-08-06T07:11:10.516Z Reads: 101

```
I'm pretty sure you will beat the Raptor 2
```

---
## \#37 Posted by: Jinra Posted at: 2017-08-06T07:13:08.159Z Reads: 101

```
I honestly dont know.. I've seen vids on youtube and everything and I'm not sure mine accelerates as fast; especially against the performance in this video. Guess we'll find out.. haha

https://youtu.be/TfwjzQyUDPI?t=63
```

---
## \#38 Posted by: Eboosted Posted at: 2017-08-06T07:14:35.571Z Reads: 99

```
Can you add 8 more cells for a 12S setup before the match? Just limit ERPM for the 230kv motor.
```

---
## \#39 Posted by: Jinra Posted at: 2017-08-06T07:15:41.278Z Reads: 100

```
The enclosure's already packed tight. Also, my DRV will likely burn at 12s 230kv. 

Didn't you just tell me not to fiddle with my board before a match haha
```

---
## \#40 Posted by: Eboosted Posted at: 2017-08-06T07:17:52.475Z Reads: 97

```
Yeah, but damn! I would love to see you beating the Raptor 2, even though I have one on order
```

---
## \#41 Posted by: psychotiller Posted at: 2017-08-06T07:23:47.813Z Reads: 96

```
How is it on BLDC?
```

---
## \#42 Posted by: Jinra Posted at: 2017-08-06T07:25:30.959Z Reads: 96

```
Been great on BLDC so far, but if the torque isn't enough to send me flying, it's never enough for me.
```

---
## \#43 Posted by: darkkevind Posted at: 2017-08-06T08:06:05.734Z Reads: 91

```
How do you find the correct settings then? Trial and error?
```

---
## \#44 Posted by: Jinra Posted at: 2017-08-06T18:57:09.484Z Reads: 81

```
BTW is it just me or is your motor supposed to sound like a banshee when you measure R and L in FOC detection. Sort of sounds like a 56k modem but a lot louder.
```

---
## \#45 Posted by: psychotiller Posted at: 2017-08-06T19:02:02.643Z Reads: 80

```
First time I heard that I was posititive I ruined everything! Bahaha, but then I rode the evil spirit powered beast.
```

---
## \#46 Posted by: pshaw Posted at: 2017-08-06T21:10:35.369Z Reads: 77

```
Has anyone successfully run FOC on dual 6374 on 12S?
```

---
## \#47 Posted by: flywithgriff Posted at: 2017-08-07T01:25:43.886Z Reads: 67

```
I'll be sure to listen for this magical tune when I set up my dual 6374 10s build!
```

---

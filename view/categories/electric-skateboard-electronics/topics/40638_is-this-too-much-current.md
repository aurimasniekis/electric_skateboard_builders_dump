# Is this too much current?

### Replies: 35 Views: 2201

## \#1 Posted by: Eboosted Posted at: 2017-12-11T02:25:12.553Z Reads: 321

```
My board feels pretty powerful, but I'm not sure if I should decrease the current limits, what do you guys think?

I'm running 12S4P on Samsung 30Qs (datasheet says 15A but Mooch test has shown it's a pretty good/safe 20A battery)

Motor Max 90A
Motor Min -60A
Battery Max 40A
Battery Min -20A

On this chart I can see I'm pulling a lot of current, should I be  concerned? Is it possible log the temperature via this datalog?

<img src="/uploads/db1493/original/3X/9/f/9fb4708de4b1b00b6f6aef935ea209b926edf65a.png" width="520" height="500">
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-12-11T02:31:13.421Z Reads: 301

```
Look perfect to me 👌

If usually keep upping my current until something blows, then back to the highest settings that worked and call it done haha.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2017-12-11T02:33:24.572Z Reads: 297

```
This data is for one or two VESC’s?
```

---
## \#4 Posted by: Eboosted Posted at: 2017-12-11T02:37:39.879Z Reads: 294

```
I'm holding +65A on each motor during full acceleration which could take 5-6 seconds, I wonder how much could my temps be raising
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-12-11T02:42:04.635Z Reads: 280

```
Your motor temps?  Or the Vesc?
```

---
## \#6 Posted by: Eboosted Posted at: 2017-12-11T03:41:55.582Z Reads: 263

```
The vesc had its own temp sensor but it's disabled on VESC analyzer
```

---
## \#7 Posted by: saul Posted at: 2017-12-11T17:58:06.052Z Reads: 228

```
[quote="Eboosted, post:4, topic:40638, full:true"]
I'm holding +65A on each motor during full acceleration which could take 5-6 seconds, I wonder how much could my temps be raising
[/quote]

you're really pushing those batteries...
I guess its working so you can keep going, but lowering your settings would probably give you some extra cycles on that pack. and you'll get some extra mileage per charge!

Max limits are cool if you want speed, torque, big numbers..
but Max efficiency are the numbers I use! and search for! huge difference!
```

---
## \#8 Posted by: egzplicit Posted at: 2017-12-11T18:08:55.350Z Reads: 213

```
I think battery max is what you need to worry more than motor max. U do run the cells at 20A/cell but like you say, only for peaks that are no longer than 10s. If you don’t go up a really long hill, that’s fine but I wouldn’t go higher. Maybe motors can do a bit more but I don’t think you should increase battery max anymore.

Edit: Oh you meant decrease, lol. I run 30q at 15A per cell as per spec, 20A for short bursts should still be ok I think. Motor max seems a bit high but again if you monitor your rides you’ll see these are spikes and don’t last very long.
```

---
## \#9 Posted by: E1Allen Posted at: 2017-12-11T19:06:34.603Z Reads: 199

```
What motors and gear ratio are you running? That is high amps.
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-12-11T19:45:25.863Z Reads: 190

```
You only peaked at a little over 30A per VESC, they can handle that current for much longer than a few seconds at a time.

Most of my builds run settings of  30-40A Battery and 100-120A motor on all 4 motors. Having extra power for bursts is awesome, if I ask for too much my VESC's back me off once the motor or VESC temps hit the thermal limts.
```

---
## \#11 Posted by: Eboosted Posted at: 2017-12-11T21:34:04.794Z Reads: 179

```
[quote="E1Allen, post:9, topic:40638, full:true"]
What motors and gear ratio are you running? That is high amps.
[/quote]

I'm runing dual 6374 190KV motors on 15/40 ratio on 107mm wheels.
```

---
## \#12 Posted by: Eboosted Posted at: 2017-12-11T21:35:20.271Z Reads: 179

```
Well today I started to have DRV issues, so I wonder if it'd be related to the high current output.

<img src="/uploads/db1493/original/3X/7/d/7d81523a5a6cd62ced01ae789213415ae1819ae5.png" width="243" height="500">
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-12-11T21:52:22.459Z Reads: 171

```
Thats an over current code not DRV. Ive seen that before, I raised the absolute current threshold on my builds that run high motor amps and that code went away.

But that code does pop for other reasons like DRV....
```

---
## \#14 Posted by: Eboosted Posted at: 2017-12-11T22:00:10.777Z Reads: 169

```
How much have you raised your abs. current value?
```

---
## \#15 Posted by: Eboosted Posted at: 2017-12-11T22:01:20.927Z Reads: 167

```
I had also this one on my way home:

<img src="/uploads/db1493/original/3X/9/6/96e5a1486ec55199bd22ff56874fe3edb3790033.png" width="243" height="500">
```

---
## \#16 Posted by: BigBoyToys Posted at: 2017-12-11T22:15:33.848Z Reads: 164

```
On my carvon V2's with 100A motor and 37.5A battery I have it set to 150A.

On my trampa with 100A 80A settings I have it at 200A.
```

---
## \#17 Posted by: E1Allen Posted at: 2017-12-11T22:40:44.505Z Reads: 162

```
That's interesting how much motor amps you are pulling.  I have same setup but with 18/36 gearing.  I have batt max 60a and motor set to 65a each.  Even pulling hard up a hill I didn't hit max motor amps.  I had to slow down at 37mph because things get wobbly.  Metr data is from one vesc

https://metr.at/r/T6UPp
```

---
## \#18 Posted by: Eboosted Posted at: 2017-12-11T23:29:16.333Z Reads: 150

```
[quote="E1Allen, post:17, topic:40638"]
or amps you are pulling.  I have same setup but with 18/36 gearing.  I have batt max 60a and motor set to 65a each.  Eve
[/quote]

Well my settings are way more aggressive on motor max 90A vs your 60A and way less agressive on batt max 40A vs yours at 60A.

What battery setup and cells are you runing?
```

---
## \#19 Posted by: E1Allen Posted at: 2017-12-12T00:36:04.341Z Reads: 144

```
12s  8ah lipo. So not really worried about amp draw @25c continuous.  I'll be switching to 12s on 30q soon as my friend builds my pack.  So even if I wasn't hitting motor max of 65a, increasing the max motor amps to 90a would create a noticable difference?

Mine are maytech sensored running hybrid so they are sensorless at that point. According to maytech site and Psychotiller store the max continuous motor amps is 65 so that's where I put it.
```

---
## \#20 Posted by: Eboosted Posted at: 2017-12-12T00:48:24.371Z Reads: 141

```
Try to raise the motor amps from 65A to 80A and see if you feel a differewnce, in my case was a huge improvement even though my battery amps were only 40A per VESC
```

---
## \#21 Posted by: E1Allen Posted at: 2017-12-12T01:14:48.142Z Reads: 127

```
I get what you're saying.  How that makes an improvement is beyond me if it wasn't even reaching 65a
```

---
## \#22 Posted by: E1Allen Posted at: 2017-12-12T01:33:06.339Z Reads: 119

```
Also when I had 16/36 with 97mm wheels I couldn't stay on the board of I gave it full throttle.  Now it's a little more tamed.
```

---
## \#23 Posted by: Eboosted Posted at: 2017-12-12T01:41:27.275Z Reads: 116

```
FWIW I'm on ackmaniac firmware runing FOC
```

---
## \#24 Posted by: E1Allen Posted at: 2017-12-12T02:15:10.520Z Reads: 112

```
Gotta be worth something I guess
```

---
## \#25 Posted by: BigBoyToys Posted at: 2017-12-12T04:05:47.203Z Reads: 108

```
Raising motor amps settings  from 60 to 80 is very noticeable. I get what u are saying about your logs not showing you even max your current settings but I havent found a motor yet that didnt respond noticeably to increased motor amps.
```

---
## \#26 Posted by: Eboosted Posted at: 2017-12-12T04:44:24.161Z Reads: 105

```
Well, here back reporting...

I decreased motor max to 85A and battery max to 35A and the DRV error seems to went away, at least didn't show on my way back home.

I'll make some logs tomorrow to see how the current was affected in a full throttle pull
```

---
## \#27 Posted by: pshaw Posted at: 2017-12-12T05:02:35.955Z Reads: 99

```
I had my trampa at 120 motor amps and I would get abs error even when upping max abs to 150. 

It was only if I floored it from a dead stop. If I was going 2-3mph then floored it this wouldn’t happen. 

FWIW
```

---
## \#28 Posted by: E1Allen Posted at: 2017-12-12T07:16:16.826Z Reads: 99

```
[quote="BigBoyToys, post:25, topic:40638, full:true"]
Raising motor amps settings  from 60 to 80 is very noticeable. I get what u are saying about your logs not showing you even max your current settings but I havent found a motor yet that didnt respond noticeably to increased motor amps.
[/quote]

I hear ya.  It has to be the programming in the vesc. I just figured I was getting the max the motors could offer.  But at their rated 3550w I would need to pull 70-80a depending on voltage @12s
```

---
## \#29 Posted by: BigBoyToys Posted at: 2017-12-12T08:04:47.396Z Reads: 94

```
I dont actually know how Abs current is calculated but I havent seen that code since I started setting my abs current as such. I add my battery amp setting to my motor amp setting then add few percent on top. Ie. 40 battery amps plus 100 motor amps =130A + 10A exrta =150A= Abs Current setting.
```

---
## \#30 Posted by: PXSS Posted at: 2017-12-12T11:14:32.801Z Reads: 89

```
Your abs current should be 20-30 amps higher than you highest current (either batt or motor). They dont add. You may hit a really short transient that goes over your motor or batt max but it won't give out an error until it goes above absolute max. 

At the level that you're pulling current though, you might require a larger overhead, which would be why 150 works perfectly for you. 

---

You are more likely to hit your motor current limit at very low speeds. For example full throttle from zero. 
The reason all motors react well to increasing motor amps is that your 100% throttle end point moves to a higher power at low speeds. During high speed, you'll more than likely always hit your batt max beforehand. 

Adjusting motor max is like messing with the throttle curve
```

---
## \#31 Posted by: BigBoyToys Posted at: 2017-12-12T17:03:50.539Z Reads: 80

```
Thanks for shedding some light on that!
```

---
## \#32 Posted by: E1Allen Posted at: 2017-12-12T17:10:19.914Z Reads: 79

```
[quote="PXSS, post:30, topic:40638"]
Adjusting motor max is like messing with the throttle curve
[/quote]

Which makes some sense about upping motor amps would give a noticable difference if it's like changing the throttle curve. @BigBoyToys
```

---
## \#33 Posted by: Eboosted Posted at: 2017-12-14T06:36:27.776Z Reads: 73

```
My antispark switch died today, stucked in the open position. This excess of current is starting to brake stuff :grinning:

Both mosfets got shorted, I guess that's why I been getting some undervoltage faults since one week ago, it semms that 1 mosfet died first then the other one.

I'm buying 10 IRFS7530-7PPBF MOSFET to have them in stock.
```

---
## \#34 Posted by: PXSS Posted at: 2017-12-14T10:52:58.069Z Reads: 72

```
I'm guessing you still don't have a fuse inline? 
I'm not looking forward to your next battery fire
```

---
## \#35 Posted by: BigBoyToys Posted at: 2017-12-14T16:55:14.296Z Reads: 62

```
Ive blown many  AS switches with various number and grades of mosfets from high current. Im not sure your mosfets are the weak link. If the trace on the PCM get too hot the mosfets will slide around any end up shorting. Id love to here if your mosfet upgrade solves your issue though.
```

---

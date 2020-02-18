# Pros &amp; cons: 10s4p vs 12s3p

### Replies: 52 Views: 3563

## \#1 Posted by: lennylogs Posted at: 2018-01-23T22:52:41.625Z Reads: 593

```
I can't decide...

The 10s will have longer range but lower top speed, and the 12s will have shorter range and higher top speed....is there anything else that I should consider? Torque? Voltage sag differences? 

According to the range calculator, calc.esk8.today, the range difference doesn't seem to be that significant. 

What do you guys think???
```

---
## \#2 Posted by: lowGuido Posted at: 2018-01-23T23:04:45.114Z Reads: 582

```
its only 4 cells difference. not a great deal. id go with 10S for that extra bit of juice because I rarely skate up to 50km/h.
```

---
## \#3 Posted by: thisguyhere Posted at: 2018-01-23T23:17:00.246Z Reads: 573

```
i'd go with the 10s4p is range is more important, you'll get about 10% more watthours.

![image|165x70](upload://x0YBhO385LgT2M21MxyeGEj9QEz.png)

but i prefer 12s performance, all my boards are 12s.  i find with a 10s, performance is pretty lacking at end of charge.  with a 12s it's super strong until lower voltage cutoff.
```

---
## \#4 Posted by: E1Allen Posted at: 2018-01-24T00:05:40.108Z Reads: 544

```
More volts!! Pro.
```

---
## \#5 Posted by: b264 Posted at: 2018-01-24T00:17:23.936Z Reads: 531

```
Go with 10S for sure if you're using VESC controllers
```

---
## \#6 Posted by: lennylogs Posted at: 2018-01-24T00:22:12.057Z Reads: 524

```
Why is that?
```

---
## \#7 Posted by: lennylogs Posted at: 2018-01-24T00:23:28.540Z Reads: 523

```
Okay thanks. I was wondering about that
```

---
## \#8 Posted by: b264 Posted at: 2018-01-24T00:32:27.257Z Reads: 521

```
Because the parts used in the vesc circuit shouldn’t be run that high, especially with a reactive load like motor windings. I’m not trying to run my controller on the razor edge of what’s possible because it increases failure rate. I’d prefer if the board failing on me was kept to an extreme minimum, especially if it means I lose brakes and definitely if it means a $150+ part is the thing failing

Lots of people run at 12S but I also hear of lots of failures.  To me, not failing is a very important metric and thus I can't consider it.  Most consumer electronics are designed with a 40% margin at least, the components in the VESC being rated at 60V and 63V means 8S would meet that criteria, so 10S is already over the normal.  12S is too close
```

---
## \#9 Posted by: ATLesk8 Posted at: 2018-01-24T00:53:48.862Z Reads: 492

```
What about running 12S with fairly conservative VESC settings? Is it necessarily a voltage issue or an amperage issue? Genuinely curious?
```

---
## \#10 Posted by: GrecoMan Posted at: 2018-01-24T00:55:07.727Z Reads: 484

```
Higher voltage = lower current (amperage)

most of the components on the vesc are limited to 60v, but we need to leave some headroom. the components weren’t meant to be pushed to the extent that 12s pushes them.
```

---
## \#11 Posted by: b264 Posted at: 2018-01-24T00:59:50.754Z Reads: 468

```
[quote="ATLesk8, post:9, topic:44459"]
Is it necessarily a voltage issue or an amperage issue?
[/quote]

The voltage limits are hard limits; can never exceed and each individual part has some variance in manufacturing tolerance, so just because one works up to voltage X doesn't mean another will work to voltage X

The current limits are not hard limits at all, and are only limited by heat .. so the parts can't get too hot.  If, for example, you were to cool the unit more agressively, or tune it down in software, you could adjust current performance.  But not voltage maximums.
```

---
## \#12 Posted by: lennylogs Posted at: 2018-01-24T01:32:50.039Z Reads: 438

```
When you say vesc, are you referring to both the focbox and the vesc 6?
```

---
## \#13 Posted by: lowGuido Posted at: 2018-01-24T01:56:23.000Z Reads: 431

```
[quote="GrecoMan, post:10, topic:44459"]
Higher voltage = lower current (amperage)
[/quote]

this is not a thing. 
can people please stop saying this.
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-01-24T01:57:31.236Z Reads: 412

```
wait what? please explain.
```

---
## \#15 Posted by: lowGuido Posted at: 2018-01-24T02:03:50.709Z Reads: 420

```
higher voltage does NOT equal lower current. in most normal applications higher voltage actually equals higher current.
its ohms law V=I*R
so what no one ever mentions is R! you actually need to change the load in order to get lower currents from higher voltages.

so what you should be saying is: similar torque can be had from a higher voltage with lower current if you use a lower kV motor.

however with the same motor and un governed torque you will always draw more current with more voltage.

this "higher voltage = lower current" thing is missing half the equation and its pretty misleading to the noobs.
```

---
## \#16 Posted by: GrecoMan Posted at: 2018-01-24T02:06:23.174Z Reads: 414

```
ahh yea ok. sorry. should be more clear next time 

so this is right?
higher voltage + lower kV motor = lower current?
```

---
## \#17 Posted by: lowGuido Posted at: 2018-01-24T02:07:34.403Z Reads: 411

```
yeah. don't worry. its not just you... I see that +V = -I thrown around on this forum daily.
```

---
## \#18 Posted by: jmasta Posted at: 2018-01-24T06:42:36.091Z Reads: 403

```
[quote="lowGuido, post:15, topic:44459"]
higher voltage does NOT equal lower current. in most normal applications higher voltage actually equals higher current.

its ohms law V=I/R
[/quote]

I feel this is a bit of a misinterpretation of Ohm's Law and might be confusing to some.  The relation is **V=I*R**, which is the voltage drop across a resistor.  So yes, for a constant R, higher current equates to a higher voltage drop

But what we really care about is power.  Power gets things done; resistance does not.

The important equation for our purposes is: **P=V*I**

Simply put, less current is required at a higher voltage to achieve the same electrical power power output:

*   2000W / 37.0V = **54A** _@10s_
*  2000W / 44.4V = **45A** _@12s_

But really... higher voltages just give you the ability to produce more power.  12S can produce 20% more power than 10S at the same current.  Using the same example, 54A on 12S produces 2400W



---
_Back to the topic at hand:_   _10s4p vs 12s3p_
---

**10s4p will have better range and less voltage sag than 12s3p**. Because at the end of the day you have 4 more cells and about 10% more watt-hours, as others have said

_Example:_ At 2000W, 10s4p would draw 13.5A/cell, while 12s3p would draw 15A/cell

So the current draw _per cell_ is actually less on 10s4p than 12s3p, which means slightly less voltage sag.  And it has higher capacity (higher watt-hours), which means slightly better range.

 If you wanted a fair comparison, assume both battery configurations are limited to 15A/cell.  In that case, the 10s4p battery can produce 2222W, while the 12s3p battery can only do 2000W.  So the power difference between the 10s and 12s (from above) is actually offset in this case, since you are really comparing 40 batteries to 36

---
Long story short, 12S can produce more power than 10S for the same [total] current.  But a 10s3p battery can produce more power than 12s4p for the same per-cell current



_Overall the difference is not worth stressing about... go ride your skateboard_ :slightly_smiling_face:

---

**TL;DR:** More batteries = More better
---
```

---
## \#20 Posted by: scepterr Posted at: 2018-01-24T06:45:59.397Z Reads: 373

```
I think what @GrecoMan meant was that for the same  watt output at higher voltage the current has to be less than current at a lower voltage
12v * 10a=120w
10v * 12a=120w
So however many watts you draw at a higher voltage it's lower amps than lower voltage
```

---
## \#21 Posted by: b264 Posted at: 2018-01-24T06:56:51.401Z Reads: 374

```
We should all start over and call this thread "Pros & cons: 10S6P vs 12S5P" so the number of cells is the same.  Because I think that's more in-line with the OP's intent.  **More cells is always moar better.**  But for the above, I'd use 10S6P
```

---
## \#24 Posted by: Sirshaunsta Posted at: 2018-01-25T21:24:55.434Z Reads: 337

```
This is why I went with 10s for vesc/focbox the erpm limit can easily be surpassed using 12s which would fry your shit. Also even being too close to the erpm limit can be bad as people have reported malfunction under 60 000rpm as well so it's important to leave headway as I believe it was @GrecoMan said.
```

---
## \#25 Posted by: lennylogs Posted at: 2018-01-25T21:31:17.896Z Reads: 324

```
what about the vesc 6?
```

---
## \#26 Posted by: Sirshaunsta Posted at: 2018-01-25T21:37:05.685Z Reads: 319

```
The vesc 6 is rated for 20amps higher continuous draw than the torqueboards/diy or focbox controllers so in theory they could handle a good bit more than the others but I don't trust labels do you? So even still I would probably stick with 10s but that's just me sticking to the safe side. Im sure it's possible that one could handle the added power though @lennylogs
```

---
## \#27 Posted by: Sirshaunsta Posted at: 2018-01-25T21:43:36.826Z Reads: 308

```
Plus you then have to think about your wire and connector limits, xt90 cables are only rated for 90amp continuous, I'd say that 10 amps below is cutting it pretty close and might cause some sag/power loss due to heat
```

---
## \#28 Posted by: FredrikHems Posted at: 2018-01-25T21:54:03.343Z Reads: 301

```
JFYI the standard vesc 4.xx hw can only take 27a continuous. I dont know if the vesc 6 actually can handle 80a continuous, but I am pretty sure it can handle more than 20a compared to the standard vesc 4.xx hw.
```

---
## \#29 Posted by: Ackmaniac Posted at: 2018-01-25T21:58:14.022Z Reads: 300

```
Comparing 10S6P to 12S5P I would choose 12S because of less current for wire and VESC at the battery circuit while having the same max power and higher possible top speed. In this szenario the current for each cell is the same. And to reach the same top speed you can choose a lower kv motor which results in more torque and by this less average current at the motor.
With 10S4P or 12S3P it depends if you want speed or range.
```

---
## \#30 Posted by: lennylogs Posted at: 2018-01-25T23:30:36.868Z Reads: 286

```
It’s interesting so many people are saying this considering how many 12s builds you see on here that at least seem to be running well....not to mention all the people selling 12s builds as well. I wonder what esc boosted uses since they have a 12s battery. 

I think I’ll go with 10s4p as it’s my first build and I don’t want to risk ruining my focboxs. Plus 25/30 mph should be fast enough (having said that, the 22mph top speed on my boosted definitely leaves me wanting more)
```

---
## \#31 Posted by: FredrikHems Posted at: 2018-01-26T06:28:43.081Z Reads: 273

```
Huh, what? I havent said anything about voltage? The only thing I have written here was about amps...
```

---
## \#32 Posted by: junwoo091400 Posted at: 2018-01-26T06:38:45.165Z Reads: 273

```
I wanna set some things clear. As far as my Physics Knowledge goes

=> the VoltageXCurrent is a Power from the BATTERY, Not to the MOTOR.

This is because of 'Back-EMF'. And Back-EMF is proportional to Angular-Speed, by Faraday's Law.

So, actually, Battery Voltage is Divided into 2 Parts: "Back-EMF" and "Internal Resistance*I"

The equation is now : " V_bat = (K_u [V/(rad/s)]) x w [rad/s] + i [Ampere] x r [Ohm] "

So, with 'Higher V_bat', you can Either put that amount into 'Rotational Speed' OR 'Current'.

-> Higher Voltage = Higher Current (if, same Rotation-Speed). >> More Torque.
-> Higher Voltage = Higher Rotational-Speed (if, same Current). >> More Speed.
```

---
## \#33 Posted by: Skunk Posted at: 2018-07-23T03:30:22.768Z Reads: 224

```
Damn it I want to go fast but I also need this thing to be reliable. Would rather not fry my focbox
```

---
## \#34 Posted by: Wraith Posted at: 2018-07-23T03:45:23.039Z Reads: 222

```
did anyone ever make a seperate thread for 10s6p vs 12s5p like @b264 commented? lol I'd be real interested in that as I'm going to be going with a 60 cell pack and would be interested in the pros and cons when running with that many cells. Also because I'm curious how some motors need to have a 12s instead of a 10s, specifically the carvon SD XLs and SD Rs as stated in the carvon site.
```

---
## \#35 Posted by: Skunk Posted at: 2018-07-23T04:52:26.706Z Reads: 216

```
Will the vesc6 change the risks of running 12s?
```

---
## \#36 Posted by: b264 Posted at: 2018-07-23T05:09:18.005Z Reads: 211

```
VESC6 still uses the 60V DRV83XX IC.  @Kug3lis is working one something that can do higher voltages, I think.
```

---
## \#37 Posted by: Wraith Posted at: 2018-07-23T05:49:45.350Z Reads: 205

```
What about dual Escapes with the housings? I don't wanna risk busting a vesc if I run 12s for the first time :laughing: would get the higher voltage for sure as I think many others on the forum are burning focboxes on 12s
```

---
## \#38 Posted by: sk8l8r Posted at: 2018-07-23T10:33:53.195Z Reads: 195

```
[quote="Wraith, post:37, topic:44459"]
I think many others on the forum are burning focboxes on 12s
[/quote]

my first time with foxboxes and I was quite worried, no problems on 13s so far at least so I would be really confident with a 12s setup :)
```

---
## \#39 Posted by: Wraith Posted at: 2018-07-23T11:09:09.270Z Reads: 189

```
Thats great to hear. Funny as I just checked out your sick build earlier! Looking forward to see how it performs in the long run. 😄 so running dual focboxes is fine on 12s or 13s as long as I set it up correctly?
```

---
## \#40 Posted by: sk8l8r Posted at: 2018-07-23T11:22:45.383Z Reads: 190

```
can only say I've had no problems and I was quite scared to setup my focboxes - check what your doing recheck and have someone else check to keep things safe I would say :)

EDIT: I think what I'm saying don't use a trial and error process with foxboxes
```

---
## \#41 Posted by: Wraith Posted at: 2018-07-23T11:42:38.523Z Reads: 188

```
Yeah I wouldnt want to put focboxes under trial and error either. Does this only apply to focboxes or does this apply to vescs as well? I’ll post my initial settings once I have it all together and ready. Would be happy to have your input on it once I get to post! :smile:
```

---
## \#42 Posted by: wafflejock Posted at: 2018-07-23T16:28:36.669Z Reads: 181

```
I ran 12S on a 4.x (old hardware) and didn't have an issue.  Only problem with running 12S I've seen is if you have a high kv motor (something over 200) and high voltage you can end up over the 60,000 ERPM limit (with 14 pole motor which is pretty typical that means about 8500 wheel RPM).  With those motors being 85 or 110kv don't really see you getting anywhere near that limit (8500/85 = 100V, so would need 100V or more to get over that limit at which point you'd be toasting other components from over voltage anyhow).  Given the cost of the components would say you should be able to reach out to their support to verify everything before you finish wiring/testing yourself to see what they say.
```

---
## \#43 Posted by: Skunk Posted at: 2018-08-01T10:14:01.954Z Reads: 158

```
[quote="Wraith, post:34, topic:44459"]
did anyone ever make a seperate thread for 10s6p vs 12s5p like @b264 commented?
[/quote]

Would be great. Esk8 calculator told me the range is basically the same but the top speed is quite different.  It's 3 am, I'm ordering my battery tomorrow and still struggling to make up my mind. 
I know I definitely don't want to be stuck in the twenties and barely get into the 30s. 
But I also know I can't afford to replace Speed controls  if I f****** a 12s setup.
```

---
## \#44 Posted by: Wraith Posted at: 2018-08-01T10:17:45.315Z Reads: 149

```
I have the same concerns but I decided to go 12s. Going to check on whats the safest settings to go for. I think a properly configured vesc would save the batteries and motors even on 12s
```

---
## \#45 Posted by: Skunk Posted at: 2018-08-01T10:22:22.475Z Reads: 150

```
As worried as I am about my focbox, I think I'd be really disappointed if the board I was building had me stuck in the mid to high twenties. Not that I want to go 35 everywhere I just want to be able to do it when I want to.I
```

---
## \#46 Posted by: Wraith Posted at: 2018-08-01T10:23:00.398Z Reads: 147

```
Also I know I won’t have to touch my batteries for the foreseeable future on 12s cause I’ll have enough to supplier beefier vescs or motors that do come out
```

---
## \#47 Posted by: Wraith Posted at: 2018-08-01T10:24:22.862Z Reads: 144

```
Yeah I think there are a number of builds right now doing fine on 12s so I do plan on checking their settings and using them as a jump off point if i dint just outright take their values as is
```

---
## \#48 Posted by: Skunk Posted at: 2018-08-01T10:25:34.468Z Reads: 145

```
I'm glad @psychotiller is a super patient awesome guy because I've changed my mind on my battery several times a day over the last week. He's answered every question I had and it's just waiting for me to pay him to start my order at this point. Guess I'll have to message him and tell him I change my mind yet again lol
I think........ ha
```

---
## \#49 Posted by: Wraith Posted at: 2018-08-01T10:30:33.969Z Reads: 140

```
Yeah I’ve been asking @psychotiller  alot about enclosures for the hummie deck that can double stack the 12s5p and he’s been cool about me asking despite not placing an order or anything so I can’t help but commend him for it! 

Honestly if I could’ve ordered the battery pack and enclosure from him I wouldn’t even give it a second thought but shipping battery packa from US to Asia is a tricky business which he also says so himself
```

---
## \#50 Posted by: Skunk Posted at: 2018-08-01T10:39:01.566Z Reads: 137

```
Yeah I was going to go for a stacked battery but then  I realized I could get 60 cells in there if I mounted my speed controllers topside. Went ahead and grabbed the Dual heat sink enclosure for them
```

---
## \#51 Posted by: Wraith Posted at: 2018-08-01T10:40:30.400Z Reads: 133

```
Those are the dual enclosures by @Kug3lis?
```

---
## \#52 Posted by: Skunk Posted at: 2018-08-01T10:42:33.210Z Reads: 139

```
Yes. It's super clean and the pictures really don't do it justice. I was surprised how Compact and small it is. But I was also surprised how small the FOCbox are.
```

---
## \#53 Posted by: Wraith Posted at: 2018-08-01T10:43:44.535Z Reads: 141

```
That’s awesome! I’m actually considering the heat sinks so I can still mount it underside and make a cutout in whatever enclosuee I end up going with. Can’t doubt the high quality stuff that @Kug3lis makes
```

---
## \#54 Posted by: Gabegds2001 Posted at: 2019-07-01T22:55:11.799Z Reads: 60

```
I know this is an old thread, but im thinking of buying either a 10s4p samsung 30q pack or a 12s3p pack. I have a 4.12 vesc and a 149kv motor. Im worried i wont have very much speed with 10s, but i want reliability from my vesc. Will 12s3p and a 149kv motor be pushing the limits?
```

---
## \#55 Posted by: wafflejock Posted at: 2019-07-01T23:25:00.461Z Reads: 58

```
Should be all good I was also running 149kv 6374 from turnigy.  Basically so long as motor rpm stays under 8500 with typical magnet/pole arrangement then can just divide 8500 by the kv to get max voltage you could apply before going over 60k eRPM which causes the DRV to blow pretty often it seems.  You'd be safe up to 8500/149 = 57 volts 12S fully charged lipo cells are 4.2 x 12=50.4
```

---

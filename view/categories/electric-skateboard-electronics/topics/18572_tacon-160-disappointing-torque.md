# Tacon 160 disappointing torque

### Replies: 10 Views: 1023

## \#1 Posted by: saul Posted at: 2017-03-05T02:42:19.525Z Reads: 138

```
So I recently switched from a 6355 190kv to a tacon 160 6364 245.

I"m running 8s 10ah lipo with a vesc. 50A motor 30A batt.
14/36t on 80mm kegels.

I got the top speed increase I expected. maybe a bit more. from 20mph to 24mph.
range is still about 16 miles. but My hill climb torque is sad, and if I full throttle on my usually speed runs it feels like the vesc is heating up and losing power....

I expected a bit less torque from upping the kv, but this almost gives up when I push it hard. while on the top end it feels like it still wants to pull more. so maybe more power (55-60A motor) will help it run better? 
or I have just hit the limit of a relatively high kv, mid voltage setup? 

Not interested in theory, Just want to know if anyone else has a single drive with 230kv+ on 8s?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-03-05T02:59:16.596Z Reads: 137

```
More current will help I've run it on 8s but with a 120a esc so I'd say current is ur issue
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-05T03:53:03.905Z Reads: 126

```
The Tacon  160 is a good motor. But 50a motor current is really low.
The max efficiency current is 75a
So you can turn your motor max to 75a and try it.
If you still want more power, you can increase battery max amps as high as 50a

<img src="/uploads/db1493/original/3X/4/8/488044c8ce0f07958b18f46f214ce5a6adcaaede.png" width="490" height="397">
```

---
## \#4 Posted by: Hummie Posted at: 2017-03-05T04:06:29.934Z Reads: 117

```
Motor max is misleading as its for fractions of time. U can run 200 motor amps and 75 battery and u will only hit 75 true amps
```

---
## \#5 Posted by: Okami Posted at: 2017-03-05T20:45:34.361Z Reads: 94

```
This should be sticked somewhere in Vesc settings as default.. :D I think @Ackmaniac tried to improve the situation by including tooltips in his latest Bldc tool release.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-03-05T22:36:48.667Z Reads: 89

```
I am sorry to tell and sorry to see that hummy still gives these wrong advices. Please don't use 200 motor amps. 
You can raise the motor amps for more torgue. But I wouldn't recommend more than 100 amps. But that will not fix your heat issue. It will be even worse.

So you have 2 options. 
Go back to the 190 kv motor and use a 10 or 12S battery for more speed. 
Or you add heat sinks to the vesc to keep it cooler.
```

---
## \#7 Posted by: Hummie Posted at: 2017-03-06T00:13:15.357Z Reads: 74

```
Uhu o. I see this again. Too bad @devin is banned.  A rationale of why 200 is bad is needed. I ride it.  It's the best performance I've had. Maybe the vesc, also on foc, will die a sooner death but I still think a temp cut-off will happen first.  Never happenened

The way the escs most often work it seems being at a low speed requires being at a low  duty cycle, and this would be a reducer of low speed power, but the "motor amp" variable allows changeable low speed power beyond what just the battery amp limit would allow, as its constrained by the duty cycle: at lower speed it gives less power and it ramps it up. Kinda two ramping a.  It is the power decider!  You change the battery amp and motor amp limits and it's a different animal. What kind o animal do u want to ride. But u made the variable or consistent wattage program so u know that at low speed the motor amp limit is the power decider.
As far as heat.. It's prett consistent with power output and even though at 200 motor amps u get 200 amps, it is for such fast frequency that the induction of the motor smoothes it...and you'll be at a much lower true amperage when averaged "on time" is put in context off the full time period. No torque spikes and no magnetic saturation of the stator
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-03-06T09:10:58.150Z Reads: 60

```
Because you disable the overcurrent protection of the VESC with this high settings. We went through this shit already many times and my advice's are simply ignored by you.
And 200 amps would be only usable with watt control. In current control the board becomes uncontrollable. But you never mention this.
```

---
## \#9 Posted by: treenutter Posted at: 2017-03-06T20:12:14.885Z Reads: 46

```
@Ackmaniac @Hummie We all appreciate your help but pls respect @saul 's request for practical advice about improving his torque OK? There are PLENTY of discussions already about the theoretical and practical use of much higher motor amps.
```

---
## \#10 Posted by: Hummie Posted at: 2017-03-06T20:48:31.877Z Reads: 44

```
im in current control.  I have consistent power output at every rpm, far from uncontrollable.    yes your advice is ignored and doing fine.  looking for facts not advice and considering you keep saying what i'm doing is impossible...

this is about as practical or easy as it gets for improving torque.  you adjust the settings on the vesc
```

---

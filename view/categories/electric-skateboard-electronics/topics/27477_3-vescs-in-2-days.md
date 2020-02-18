# 3 VESC&rsquo;s in 2 days

### Replies: 22 Views: 1177

## \#1 Posted by: mmaner Posted at: 2017-07-13T00:58:59.472Z Reads: 196

```
So... My kid was on his board yesterday which has x2 MEB VESC's in BLDC mode.  One motor stopped completely and the other was cogging at any throttle level.  Turns out both VESC's are showing DRV errors. 


Before I checked the errors I figured it was a VESC so I gave him my beater board to ride.  He went about half a mile and the remote stopped responding.  He walked it back home, I checked when I got home and DAMNIT another DRV error on a TB VESC in FOC mode.

I've racked my brain searching for what might have caused 3 dead VESC's in 2 days, but I'm not coming up with anything.  

Both battery packs are well above the cutoff threshold, and the BMS should have stopped anything over 60 amps.  If you have an idea, please enlighten me. 

Anyways, @JohnnyMeduse you wanna work your mojo on 3 VESC'S for me?
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-13T01:06:43.157Z Reads: 192

```
That sucks! Was he skating on ice and going fill throttle and then full brake repeatedly?!?
```

---
## \#3 Posted by: mmaner Posted at: 2017-07-13T01:08:15.254Z Reads: 188

```
Nope, he goes pretty fast...at least it's fast for me, around 20mph, but nothing it if the ordinary.  Not very ling rides either. Also, if it matters, I've got a 3000va UPS that we charge the boards on.
```

---
## \#4 Posted by: JLabs Posted at: 2017-07-13T01:10:17.499Z Reads: 180

```
Did you have a peek at your ERPM limit? Sounds like he exceeded them. [quote="mmaner, post:3, topic:27477"]
I've got a 3000va UPS that we charge the boards on.
[/quote]

Not exactly sure what that is
```

---
## \#5 Posted by: Jinra Posted at: 2017-07-13T01:20:14.436Z Reads: 164

```
^Agreed, what eRPM is 20mph on your setup?

Also, were the first two VESCs in CAN or split PPM?
```

---
## \#6 Posted by: mmaner Posted at: 2017-07-13T01:38:48.636Z Reads: 147

```
Yeah, the ERPM was limited to 60k.  A UPS is a battery backup system, this one is active meaning it powers peripherals via the batteries  and charged the batteries via the house power.  It delivers a very steady volt and amp load.
```

---
## \#7 Posted by: mmaner Posted at: 2017-07-13T01:39:56.389Z Reads: 143

```
I do t know what the ERPM is 20mph, but I did have the limit set.  It was configured with can bus.
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-13T01:41:39.385Z Reads: 140

```
was there anything reused between board 1 and board 2? Like adapters, controller receiver, battery, etc?
```

---
## \#9 Posted by: mmaner Posted at: 2017-07-13T01:44:24.888Z Reads: 141

```
Nope, they were to totally separate builds. 

I changed the wheels out on his dual motor build a couple if weeks ago, he was running 83mm and wanted to try 97mm.  Other than that nothing has changed on his build in almost a year.

My single motor FOC build has been finished for a few weeks, nothing changes out recently, sine I co.oletes the build.
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-13T01:46:42.417Z Reads: 134

```
I can understand why the single FOC build blew, but not sure about the other one, though it does sound like one VESC might've friend the other through the CAN connection. Perhaps the additional current needed for acceleration on bigger wheels blew out the VESC which caused a chain reaction to blow out the other VESC.
```

---
## \#11 Posted by: mmaner Posted at: 2017-07-13T01:49:25.573Z Reads: 128

```
This is weird, it appears the primary VESC is fine as long as it's not connected to the secondary.  I just reset it to defaults and plug it up to the same 10s pack and one of the motors and it runs perfectly.  

The secondary is all res blinky lights and other sadness. The same on the single motor build (the FOC setup).
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-13T01:50:58.511Z Reads: 128

```
Ah okay, maybe the slave was sending it's fault to the master VESC, not really sure how it works. But at least you one VESC saved! This is why I won't even touch FOC until VESC6, though I might try with the focbox.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-07-13T02:05:20.956Z Reads: 122

```
[quote="mmaner, post:1, topic:27477"]
I got home and DAMNIT another DRV error on a TB VESC in FOC mode.
[/quote]

TB vesc doesn't have enough capacity for foc, (they usually miss the c26 capacitor) and if your to hard on them you might burn them in foc configuration
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-07-13T02:06:48.907Z Reads: 120

```
FocBox isn't call FOCbox for nothing 😉, I have run them in foc since unit 001 without any problem.
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-13T02:07:44.147Z Reads: 119

```
right on ;) I'm just extra cautious because falling off at 35 mph is no fun
```

---
## \#16 Posted by: mmaner Posted at: 2017-07-13T03:10:50.138Z Reads: 114

```
I've got 2 coming, gonna rebuild the spud with them and maybe some.MBS gear.
```

---
## \#17 Posted by: torqueboards Posted at: 2017-07-13T06:10:35.220Z Reads: 102

```
@JohnnyMeduse - That was before. We haven't been missing a C26 cap for a long time. I ride on FOC with no issues. Have people with TORQUE Rocket FreeFlow's on FOC with no issues.
```

---
## \#18 Posted by: Jinra Posted at: 2017-07-13T06:14:55.588Z Reads: 103

```
Guess the real question now is if it was an old TB VESC or new :)

Do you have the C26 cap on the single VESC @mmaner?
```

---
## \#19 Posted by: mmaner Posted at: 2017-07-13T16:45:15.772Z Reads: 72

```
I don't know if it had the c26, already packed up on its way back to @torqueboards.  I wasn't even gonna ask for a replacement, I'd had the VESC since December but as usual Dexter comes through. 

I'll prolly send the other off for repair to @JohnnyMeduse, I'm getting a stack of them now. 😀
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-07-13T16:52:07.081Z Reads: 72

```
Haha that how I like them 😜 Stack and ready to be reapair 

Also @torqueboards, event with C26... the original design still prove to have some flaws over FOC, C26 make it more stable, but if you push it to hard there is still some risk involve.
```

---
## \#21 Posted by: pennyboard Posted at: 2017-07-13T17:09:05.629Z Reads: 66

```
Can confirm, I just configured my TB vesc newly repaired by @JohnnyMeduse on 6s FOC and worked great once it was set-up.   
Although it took about 5 tries to get BLDC tool to correctly measure Lambda cause the motor wouldn't spin-up

edit: this TB vesc was purchased in July 2016, if anyone's curious
```

---
## \#22 Posted by: pennyboard Posted at: 2017-07-13T17:12:31.690Z Reads: 64

```
Could you elaborate on how unstable the TB vesc is in FOC? I was planning to run dual 6355s with a Ollin VESC on one motor and TB vesc on the other with a Y-servo splitter. Am I asking for disaster with that set-up?
```

---

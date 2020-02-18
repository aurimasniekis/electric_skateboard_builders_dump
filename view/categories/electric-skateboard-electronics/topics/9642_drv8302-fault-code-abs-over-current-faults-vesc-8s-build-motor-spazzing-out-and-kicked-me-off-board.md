# DRV8302 &amp; FAULT_CODE_ABS_OVER_CURRENT faults, VESC, 8s build, Motor Spazzing Out and kicked me off board

### Replies: 64 Views: 4935

## \#1 Posted by: Carvin_Ginger Posted at: 2016-09-15T15:51:25.357Z Reads: 381

```
Hey Guys.  I used this forum a lot when making my first build.  I rode it for about a week with a large tupperware underneath and then this past weekend I broke the battery and VESC to 2 smaller containers so i have more clearance underneath.

<img src="/uploads/db1493/original/3X/3/3/33fcb8c11a64bfd438b593349301c35908807c45.jpeg" width="375" height="500">

My Problem:

A couple days ago I got kicked off the board because the motor locked up.  It appears as though the motor is going forward and backward at the same time, "spazzing out."  This happens when I am accelerating.  Here is my setup:

2 X 4s 5000 mah Turnigy Lipo batteries
Torque Boards 190kv 6355 motor
VESC

Here are the fault codes:

The following faults were registered since start:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 103.8
Current filtered : 134.4
Voltage          : 32.07
Duty             : 0.00
RPM              : 18807.6
Tacho            : 100494
Cycles running   : 14004
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 32.18

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 136.9
Current filtered : 143.6
Voltage          : 31.86
Duty             : 0.00
RPM              : 18828.4
Tacho            : 102948
Cycles running   : 22857
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 32.56

Fault            : FAULT_CODE_DRV8302
Current          : 2.1
Current filtered : 0.3
Voltage          : 32.27
Duty             : 0.01
RPM              : 22.1
Tacho            : 103341
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 32.50

The following faults were registered since start:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 103.8
Current filtered : 134.4
Voltage          : 32.07
Duty             : 0.00
RPM              : 18807.6
Tacho            : 100494
Cycles running   : 14004
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 32.18

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 136.9
Current filtered : 143.6
Voltage          : 31.86
Duty             : 0.00
RPM              : 18828.4
Tacho            : 102948
Cycles running   : 22857
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 32.56

Fault            : FAULT_CODE_DRV8302
Current          : 2.1
Current filtered : 0.3
Voltage          : 32.27
Duty             : 0.01
RPM              : 22.1
Tacho            : 103341
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 32.50

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.3
Voltage          : 32.27
Duty             : 0.01
RPM              : 0.0
Tacho            : 137367
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 29.28

The following faults were registered since start:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 103.8
Current filtered : 134.4
Voltage          : 32.07
Duty             : 0.00
RPM              : 18807.6
Tacho            : 100494
Cycles running   : 14004
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 32.18

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 136.9
Current filtered : 143.6
Voltage          : 31.86
Duty             : 0.00
RPM              : 18828.4
Tacho            : 102948
Cycles running   : 22857
TIM duty         : 263
TIM val samp     : 131
TIM current samp : 26505
TIM top          : 52747
Comm step        : 3
Temperature      : 32.56

Fault            : FAULT_CODE_DRV8302
Current          : 2.1
Current filtered : 0.3
Voltage          : 32.27
Duty             : 0.01
RPM              : 22.1
Tacho            : 103341
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 32.50

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.3
Voltage          : 32.27
Duty             : 0.01
RPM              : 0.0
Tacho            : 137367
Cycles running   : 2
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 4
Temperature      : 29.28

Fault            : FAULT_CODE_DRV8302
Current          : 0.6
Current filtered : 0.1
Voltage          : 32.33
Duty             : 0.00
RPM              : 4.1
Tacho            : 138535
Cycles running   : 0
TIM duty         : 17
TIM val samp     : 1416
TIM current samp : 3516
TIM top          : 4200
Comm step        : 2
Temperature      : 29.49

Fault            : FAULT_CODE_DRV8302
Current          : 0.7
Current filtered : -0.1
Voltage          : 32.30
Duty             : 0.00
RPM              : 1.8
Tacho            : 138535
Cycles running   : 0
TIM duty         : 18
TIM val samp     : 1416
TIM current samp : 3516
TIM top          : 4200
Comm step        : 2
Temperature      : 29.23


Thank you for your help guys.
```

---
## \#2 Posted by: sl33py Posted at: 2016-09-15T17:15:47.075Z Reads: 320

```
Hey @Carvin_Ginger - doesn't look good to me.  The ABS over current error is relatively easy to fix by adjusting your settings.  BUT the DRV8302 error likely means a dead DRV chip.  So even if you adjust the ABS configuration settings, likely the chip will still need to be replaced.

I had similar ABS and another error related to my configuration in BLDC tool.  You can give us the screen shots of your BLDC settings/config and folks can comment.

But again the DRV chip most likely is in need of replacement.

Hope this helps and good luck!
```

---
## \#3 Posted by: Carvin_Ginger Posted at: 2016-09-15T17:20:37.003Z Reads: 318

```
thanks for the reply sl33py.

Here is a screenshot of my bldc settings

<img src="/uploads/db1493/original/3X/b/f/bf2f6172d0937971e438b65f979340172dea7c4d.png" width="690" height="431">
```

---
## \#4 Posted by: Carvin_Ginger Posted at: 2016-09-15T17:21:57.933Z Reads: 308

```
and motor:

<img src="/uploads/db1493/original/3X/b/5/b555628f14d918fab082c205994c515c0d6b7506.png" width="690" height="431">
```

---
## \#5 Posted by: Carvin_Ginger Posted at: 2016-09-15T17:22:32.472Z Reads: 302

```
could i just increase the absolute max amps by a little?
```

---
## \#6 Posted by: cesargrimmelprez Posted at: 2016-09-15T18:41:53.492Z Reads: 298

```
your vesc is dead...
```

---
## \#7 Posted by: Carvin_Ginger Posted at: 2016-09-15T18:46:59.318Z Reads: 296

```
i can't replace the drv?  you think its toast for real?
```

---
## \#8 Posted by: cesargrimmelprez Posted at: 2016-09-15T18:48:33.889Z Reads: 291

```
if you want to replace it, you need to have sick soldering skills and special tools
```

---
## \#9 Posted by: Carvin_Ginger Posted at: 2016-09-15T18:50:56.505Z Reads: 293

```
i know some people, the chip itself is $7 ish.

It doesn't look easy to me
```

---
## \#10 Posted by: Carvin_Ginger Posted at: 2016-09-15T22:31:20.730Z Reads: 290

```
Here is what it does on throttle 

https://youtu.be/DB7qBuskZJE
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-15T22:46:23.181Z Reads: 286

```
It sounds like maybe the motor wires shorted and blew the drv and caused the over current errors. Could you try spinning the motor can by hand (with everything plugged in and on) and seeing if there is resistance when you turn?

If there is then the phase wires are shorted somewhere.
```

---
## \#12 Posted by: Carvin_Ginger Posted at: 2016-09-15T22:48:49.166Z Reads: 281

```
Shorting In the motor? Btw. What is the extra wire with jst connector for?
```

---
## \#13 Posted by: Carvin_Ginger Posted at: 2016-09-15T22:50:57.903Z Reads: 274

```
It still works sometimes too
```

---
## \#14 Posted by: Jinra Posted at: 2016-09-15T22:53:09.752Z Reads: 266

```
extra wire on the motor is the sensor wire. Is there resistance while turning?
```

---
## \#15 Posted by: Carvin_Ginger Posted at: 2016-09-15T23:01:58.190Z Reads: 262

```
No resistance. Same on and off when I rotate wheel.
```

---
## \#16 Posted by: Carvin_Ginger Posted at: 2016-09-16T00:32:33.859Z Reads: 263

```
Probably going to just get a new VESC.  Unless someone can put a new drv on for me? People and prices?
```

---
## \#17 Posted by: chinzw Posted at: 2016-09-16T00:41:38.638Z Reads: 263

```
Check your "Max Current Ramp Step", i had my motor doing the same thing and it was that setting that was defaulting to 50 when it should be 0.04

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#18 Posted by: Carvin_Ginger Posted at: 2016-09-16T01:00:59.586Z Reads: 259

```
@torqueboards this is the issue i was chatting with you about on your site.

I'm KRis.
```

---
## \#19 Posted by: Carvin_Ginger Posted at: 2016-09-16T01:15:35.536Z Reads: 252

```
@chaka could yo replace the DRV on one of Dexter's VESCs?
```

---
## \#20 Posted by: chaka Posted at: 2016-09-16T16:59:43.287Z Reads: 244

```
Hey Carvin, we no longer repair VESC's from questionable sources. They always ended up failing again after a short period of time. I think dexter has some sort of warranty on his products so you might want to see if he will take care of you.

If he leaves you hanging buy one from us and we will send it out right away, we have them in stock and ready to ship. Our VESC's come with a 1 year service warranty. Something goes wrong, send it in and we repair or replace it.
```

---
## \#21 Posted by: Carvin_Ginger Posted at: 2016-09-16T21:35:12.178Z Reads: 229

```
I didn't realize torque boards vescs were questionable :(.
```

---
## \#22 Posted by: lilracerboi Posted at: 2016-09-16T22:47:30.126Z Reads: 234

```
There could still be a possible short in the motor. I remember when I got my Space Cell in and tried riding, it suddenly spazzed out a little and would just shake on throttle, which would mean something is wrong with the 3 phase wires.

I had no resistance when turning the motor either, so I went ahead and opened the motor up to insulate the 3 phase wires. It worked with zero issues after that.

On a side note, I had something weird happen to my old VESC where I kept getting a DRV error when I would let the motor come to a stop after hitting the throttle. It magically disappeared though, when I did another motor detection.
```

---
## \#23 Posted by: chinzw Posted at: 2016-09-16T23:38:11.230Z Reads: 229

```
I don't think they are. I did get mine shipped with the max ramp step bug, and defaulting to 50, which was causing that exact behavior you're getting.
```

---
## \#24 Posted by: chaka Posted at: 2016-09-17T00:09:13.458Z Reads: 225

```
@Carvin_Ginger  By questionable, I mean I do not know what components, pcb materials ect are used. This is why we only service VESC's made here in our shop. The VESC is not something easily manufactured cheaply and will continue to be haunted by those that try to find every possible way of saving money in bringing it to market.

 There really is no reason why your vesc will spontaneously fail unless you short your phase wires or run a high kv at high voltage. If it fails for some unknown reason it is usually a manufacturing fault.
```

---
## \#25 Posted by: Carvin_Ginger Posted at: 2016-09-17T00:44:34.056Z Reads: 217

```
The VESC was working intermittently yesterday, and now it won't respond at all to motor detection.  Every fault is DRV8302. 

I did manage to find a friend who replaces small chips like this for a living, so I may get out of this with minimal repair costs :).

How much should I pay him for the troubles?
```

---
## \#26 Posted by: Namasaki Posted at: 2016-09-17T04:40:41.497Z Reads: 209

```
Kris, check the solder joints on your phase wires. If one of your wires is not making connection the motor will act just like yours is. Jittering back and forth. I had this same thing happen and it was a bad solder joint on one phase wire.
This might be the cause of the drv fault as well.
And would also explain why it fail intermittently.

remove the shrink wrap and pull and twist  the connectors to see if they come loose. 
Check both the vesc's and motor's connectors and check the solder joints at the vesc.
Also your motor may have a disconnection of one of the phase wires internally.
If you could get your hands on another motor to try. or if you have an ohm meter you can check for continuity between the motor wires with the motor unplugged there should be continuity between all three wires.
```

---
## \#27 Posted by: Carvin_Ginger Posted at: 2016-09-18T00:10:08.998Z Reads: 197

```
@Namasaki I took apart the motor and checked the solder joins on the VESC. Everything looks insulated soldered well.

Now the VESC just throws the drv8302 faults and won't spin or detect. 

I did find a friend that can swap in a new drv8302. I will see if that works.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-09-18T00:17:32.337Z Reads: 196

```
if you have a volt/ohm meter check for continuity between motor phase wires with the wires disconnected from the vesc.
also check continuity from the connectors  at the end of the vesc phase wires and the solder joints on the vesc pub
You could have a cold solder joint that looks ok but is not ok.
```

---
## \#29 Posted by: Carvin_Ginger Posted at: 2016-09-18T00:50:42.127Z Reads: 192

```
I guess it wouldn't hurt to resolver them. I'm borderline getting a new VESC entirely.  Prolly from @chaka
```

---
## \#30 Posted by: Carvin_Ginger Posted at: 2016-09-18T01:04:48.040Z Reads: 185

```
@Namasaki I ohmed out the VESC and it was solid. I'm not familiar enough with the brushless motor to know what to look for.  I broke it open and looked at the wires and they were insulated, but besides that I don't know what to look for.
```

---
## \#31 Posted by: Namasaki Posted at: 2016-09-18T01:07:27.653Z Reads: 190

```
Your motors where acting like one of your phase wires was disconnected not shorted.
Putting the motor out of phase and making it jump back and forth instead of spinning.
Just check for continuity between all 3 phase wires.
There should be continuity between all 3 of them like there connected together.
<img src="/uploads/db1493/original/3X/4/4/44fb9acf7746d1f8b2eb2ca741710fa238cf53a3.png" width="333" height="151">
See how all 3 wires are connected in the middle
Inspect all your solder joints closely. The solder should be shinny not dull looking. If its dull looking, that is a sign of possible cold joint. Take it apart and clean it and solder it again preferably with a new connector and trim the wire and basically start the process new.
You really need a high power soldering gun 200-300 watts to solder these heavy connectors and wires.
I know that people are doing it with low power soldering pencils. But there is risk of cold joints without the proper tools.
When soldiering, the trick is in and out fast! You need high power to heat the joint quickly so that you don't burn all the flux away.
```

---
## \#32 Posted by: Carvin_Ginger Posted at: 2016-09-18T19:24:57.437Z Reads: 175

```
@Namasaki I ohmed out from the connectors to the vesc and they checked out.

I then ohmed from the connectors to the Motor, and found then the copper on the top was all connected to each phase wire.  is that normal?
```

---
## \#33 Posted by: Namasaki Posted at: 2016-09-18T21:22:20.871Z Reads: 173

```
[quote="Carvin_Ginger, post:32, topic:9642"]
I then ohmed from the connectors to the Motor, and found then the copper on the top was all connected to each phase wire.  is that normal?
[/quote]
Not sure what you mean by "the copper on top"
```

---
## \#34 Posted by: Carvin_Ginger Posted at: 2016-09-18T21:29:14.275Z Reads: 166

```
Where the phase wire insulation ends and the copper wires are exposed at the "top" of the motor as I put it. Each strand of copper wire that goes to the spools ohms out as being connected to each phase wire.

It doesn't appear as though they are shorting anywhere either.
```

---
## \#35 Posted by: TarzanHBK Posted at: 2016-09-18T22:23:39.688Z Reads: 167

```
check your solderings at the vesc, your motor wires and your battery. 140 Amps through your vesc are definatly not a good way to go. and check that before you replace your drv, because if there is something wrong, you just burn another chip down.
```

---
## \#36 Posted by: Carvin_Ginger Posted at: 2016-09-18T22:28:23.204Z Reads: 173

```
@Namasaki i took some pics:

<img src="/uploads/db1493/original/3X/f/7/f7e840fc0be344224bb76edb3c661962cd90a3d7.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/a/5a9afb59cd58776abbdb3e40487ab95b16f71581.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/0/10b4476e6062d0e67040b08c106ecbc500492594.jpeg" width="666" height="500">

The third pic joint is visibly loose.

Could these joints be the problem?
```

---
## \#37 Posted by: Namasaki Posted at: 2016-09-18T23:09:36.818Z Reads: 162

```
That does not look good. There should be no continuity between any of the phase wires and the motor housing. The solder joint and wire close  to it needs to be covered with shrink wrap
As you may know, The wire for the stator coils is insulated with a special clear coating. So that they don't short out.
```

---
## \#38 Posted by: Namasaki Posted at: 2016-09-18T23:13:34.006Z Reads: 163

```
CONTINUITY BETWEEN ALL PHASE WIRES
<img src="/uploads/db1493/original/3X/a/a/aa39fbf02935f071c4326df1a894f02274acf8f1.JPG" width="375" height="500">
```

---
## \#39 Posted by: Namasaki Posted at: 2016-09-18T23:14:25.645Z Reads: 165

```
NO CONTINUITY HERE
<img src="/uploads/db1493/original/3X/f/6/f61c2bbf7663000d84b414f0a69b934041ac8c72.JPG" width="375" height="500">
```

---
## \#40 Posted by: Namasaki Posted at: 2016-09-18T23:15:14.251Z Reads: 170

```
NO CONTINUITY HERE
<img src="/uploads/db1493/original/3X/3/b/3b67dab281fddc7b68f6c312be38bed408eabf26.JPG" width="375" height="500">
```

---
## \#41 Posted by: Carvin_Ginger Posted at: 2016-09-19T00:08:07.058Z Reads: 165

```
as far as i can tell the motor is just fine.  went in and soldered the loose wire and then shrink wrapped everything.  I'm just going to get a new VESC at this point.

It's a little frustrating to start a new hobby and have the VESC go so soon.  $100 down the drain to diyelectricskateboards.com.  His policy is that you can pay $75 for a warranty after the fact and get 1 replacement.  So if I am reading that right, after shipping, for the same price, I can get another....

Any suggestions on a ESC?  Should I get that replacement or go with someone else?

Seems like you have to pay ~$160 to get a VESC with warranty that will actually work.
```

---
## \#42 Posted by: Blasto Posted at: 2016-09-19T00:23:49.368Z Reads: 166

```
Continuity through each phase is normal, there's about 0.1 ohm in between each phase (*** depending on each motor) you won't be able to mesure that kind of resistance w a normal multimeter.

The other photos, the windings of the motor have a isolating coating on them, don't scratch it off, it can cause the motor to fail pre maturaly. So it's pefectly normal you can't mesure anything that way.

The motor phase should be isolated with heat shrink, did you remove it?
```

---
## \#43 Posted by: Carvin_Ginger Posted at: 2016-09-19T01:50:36.143Z Reads: 158

```
I removed the heat shrink to check the joints. One was loose and then I just finished wrapping them up again.

I think I have been desperately trying to find an alternative reason to not buy a new esc, but I'm facing the truth.

I will probably shell out $150-$170 on a new one.

ADVISE:  don't buy a VESC without warranty. maybe don't buy a VESC?

I got mine from @torqueboards.
```

---
## \#44 Posted by: Namasaki Posted at: 2016-09-19T02:56:23.205Z Reads: 154

```
I got 2 Vescs with heat sinks from Chaka. 
Expensive but they have worked perfectly from day one.  And I do a lot of hard up hill driving. 
The loose joint on your motor could have been causing the problem that you had with the motor not spinning but jerking back and forth. 
You should hook it back up to your Vesc and try it. 
I believe the consensus is that if you want the best quality Vesc with the best warranty then get the Chaka Vesc from Ollinboards.
```

---
## \#45 Posted by: Carvin_Ginger Posted at: 2016-09-19T21:26:30.448Z Reads: 152

```
@chaka I'm going to order a VESC from you tonight. Not sure which to select if you could help.

I need xt60 battery with 5.5 mm bullet connectors.

I think I want the heat sink and definitely it to be all shrink wrapped.

I am running an 8s single motor 190kv.  I live in the flat lands.

I had bought a @torqueboards VESC 2 weeks ago and it broke, but I'm not thrilled with his return policy.  

Pls help. Thanks!
```

---
## \#46 Posted by: sl33py Posted at: 2016-09-19T21:37:31.308Z Reads: 148

```
[quote="Carvin_Ginger, post:45, topic:9642"]
but I'm not thrilled with his return policy.
[/quote]


You get what you pay for.  He is pretty clear in the description on warranty options (none included, $60 upgrade to warranty):
[quote]VESC BLDC Warranty
No frills, affordable VESC with no warranty. At our current price 
point, we would not be able to provide a full warranty on VESCs. 
However, they are tested before shipment.
The VESC is highly susceptible to damage if used incorrectly. It is 
still and a beta product. Enjoy being on the cutting edge at an 
affordable price! We do our best to get you up and running with no 
problems. Please watch our YouTube Videos on setup.
We do extensive testing, loading the bootloader/firmware, testing 
BLDC  mode, motor detection and testing FOC mode. We run the tests 2-3 
times. If we are able to do the following with no issues, the VESC 
is ready to be shipped.
Still want VESC Warranty? Purchase our [additional warranty VESC BLDC with Warranty](diy-electric-skateboard-kits-parts/vesc-1-year-warranty/).[/quote]

A $60 and few bucks USPS to send back seems like the best and least $ option.  Ollin's VESC's are gorgeous and will work well for you too...  but it's ultimately another $100 you can choose to spend or not.  Yes there are a few extra caps he's refined (and Vedder didn't include in the current BOM), but for your minimal setup i don't think you absolutely need it.  

A DRV chip is only about $6.  Have any friends who can do SMD re-work or repair?  some flux, heatgun w/ reducer tip, and about 20-30 min if you are going slow and it should be done.

I have one to repair myself (bought dead), but would probably pay the $60 to get another from @Torqueboards.  

GL!
```

---
## \#47 Posted by: Carvin_Ginger Posted at: 2016-09-19T21:51:55.008Z Reads: 137

```
It's $75 after the fact for @torqueboards warranty and it covers 1 replacement for one year. So ultimately i would be paying ~$95 to get a replacement (with shipping) and no additional coverage if it has the same issue.

So basically i would just be buying an additional VESC with no warranty.

I would recommend for people buying these products to get an Enertion Platinum VESC (with warranty) or @chaka VESC that includes warranty.  ~$160-180 for a VESC with 1 year warranty is a lot better than the $100 I spent to be cheap and now will spend $180 to be safe.
```

---
## \#48 Posted by: torqueboards Posted at: 2016-09-19T22:17:55.518Z Reads: 135

```
@Carvin_Ginger - You can go ahead and pay the $60 and I can send you a replacement upon receiving the broken DRV option. However, I would probably recommend you go with Chaka. That way any future issues are resolved. We offer more of a no frills, you know what to do with it VESC.

And/or you can purchase from Chaka. Chaka hands down has the best warranty but you pay for it. :thumbsup: 

If I had more time or resources to repair DRV's for everyone I would.

You do need to know and understand that the VESC is BETA. VESC 6.0 will be a lot more robust and stable. Sorry for your experience with the VESC. For as many people who break their VESC there are hundreds of people who use it on a daily basis.
```

---
## \#49 Posted by: Carvin_Ginger Posted at: 2016-09-19T22:22:13.116Z Reads: 135

```
@torqueboards I get it.  Some people have no issues, some people fry their DRV every time they turn on their boards.

For your credit everything else worked great,  The mount, belt, pulley and motor.

I am mostly frustrated that I had the board for a week and now its dead :(.
```

---
## \#50 Posted by: chaka Posted at: 2016-09-19T22:26:03.216Z Reads: 128

```
@Carvin_Ginger We will be glad to have you as a customer! Our VESC listing has a drop down menu with many different connector options. Our warranty is unlimited, if your fry it several times we will still repair your VESC. 

After 1 year we may ask you to pay for components but honestly we will probably just take care of it beyond a year. We make these here in the shop so repair cost are very low.
```

---
## \#51 Posted by: Carvin_Ginger Posted at: 2016-09-19T22:53:19.624Z Reads: 125

```
i'm halfway thru the order @chaka
```

---
## \#52 Posted by: Carvin_Ginger Posted at: 2016-09-19T23:06:19.865Z Reads: 129

```
ok, ordered.  hopefully @chaka can get it to me soon so I can get my board going!
```

---
## \#53 Posted by: sl33py Posted at: 2016-09-19T23:51:12.160Z Reads: 129

```
[quote="Carvin_Ginger, post:49, topic:9642"]
some people fry their DRV every time they turn on their boards.
[/quote]


If you are frying your DRV every time i'd be willing to bet it's configured or setup improperly.  Either too high KV, or some missuse frying the chip.  

Given the correct components and general good quality assembly - these things are not _that fragile_.  I have 6 from at least 4 different places (1 remaining direct from Ben) and except 2 i killed from my own stupidity - all going strong.  the 2 i killed was bench testing 12s - hard start/stops repeatedly troubleshooting the ABS and other over voltage error.  Adjusted the settings fixed error, but testing it i killed 2 drv's.

You'll have great luck w/ @Chaka's VESC's.  If you want to send your dead one to me i'll see if i can repair and return to you?  If able to fix it's a spare, you just pay materials and shipping.  PM me.  (and no i'm not going into VESC repair business, just trying to help a brother out).  I have a 10 pack of the DRV's for mine (back-up) and want to practice repair (did 2 with assistance from a friend).
```

---
## \#54 Posted by: Carvin_Ginger Posted at: 2016-09-20T00:34:43.778Z Reads: 125

```
My setup (in detail)

2 X 4s 5000 mah turnigy 25c lipos
Torque boards 190kv motor
VESC torque boards
Torque boards mount
36 to 16 pulley with 12mm belt torque boards

I did not have a xt90 anti spark, but I want to switch out my current xt60 loop key with one with the new Chaka VESC I'm getting.

Any other things I should add?
```

---
## \#55 Posted by: Carvin_Ginger Posted at: 2016-09-20T00:42:11.747Z Reads: 123

```
@chaka already got my tracking number :) and will be in the postal system tomorrow AM.

These guys know service.
```

---
## \#56 Posted by: Carvin_Ginger Posted at: 2016-09-22T20:59:06.675Z Reads: 118

```
Update:

I got my board back together with everything but the VESC (should be here tomorrow).

I took it out around my hood to make sure nothing was rattling.  The motor (or belt) keeps catching every 20-30 ft.  Anyone have a similar problem?  Is this a motor problem?
```

---
## \#57 Posted by: Carvin_Ginger Posted at: 2016-09-22T21:06:35.691Z Reads: 114

```
I hope this sound is normal?

https://youtu.be/MPWyyjqNVtU
```

---
## \#58 Posted by: chinzw Posted at: 2016-09-22T21:18:13.641Z Reads: 108

```
That sounds like your belt is SUPER tight. You should be able to press down the belt with 1 finger and see it slack
```

---
## \#59 Posted by: Carvin_Ginger Posted at: 2016-09-22T21:21:55.192Z Reads: 110

```
Here's an up close

https://youtu.be/84utX6_P0DI
```

---
## \#60 Posted by: chinzw Posted at: 2016-09-22T21:47:52.011Z Reads: 115

```
That looks fine for belt tension. You can try removing the belt and see if the noise is coming from the wheel. If its not then its probably you motor, which you can open up, clean and lube the bearings.
Also, if you have a snap ring on the shaft, check if its hitting the motor mount, i had that happen to me and it made an awful sound.
```

---
## \#61 Posted by: Carvin_Ginger Posted at: 2016-09-22T22:55:48.293Z Reads: 114

```
Extremely bare bones. This is the VESC

http://www.electric-skateboard.builders/t/vesc-drv-pins-misaligned-causing-faults/10001

Shame doesn't cover manufacturer defects.
```

---
## \#62 Posted by: torqueboards Posted at: 2016-09-22T23:09:54.174Z Reads: 112

```
Sure.. Send it back. I'll send you a new one.

We cover all 100% manufacture defects.
```

---
## \#63 Posted by: Carvin_Ginger Posted at: 2016-09-22T23:14:20.053Z Reads: 108

```
@torqueboards  Bogus.  When I first mentioned the problem you said I had to pay $75 to send back for a one time replacement.  Now that I've sold it for parts and an experienced person inspected it you are offering a free replacement.
```

---
## \#64 Posted by: torqueboards Posted at: 2016-09-22T23:36:17.416Z Reads: 102

```
Never ever did you ever mention it was a manufacture fault and/or show any proof. You just said it doesn't work. Do you know how many times I've heard that? A day later, it's oh JK I got it :). That issue doesn't even prove that's the issue either. Those pins aren't even misaligned that bad and happens to be a one off issue. I'm pretty sure that wasn't the cause of the issue. Sorry for trying to help you and put things at ease for you..I might as well have not offered?
```

---

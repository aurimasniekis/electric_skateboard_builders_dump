# Dead VESC DRV- How did I kill it?

### Replies: 7 Views: 2742

## \#1 Posted by: Qwiksand Posted at: 2016-03-15T02:59:56.413Z Reads: 228

```
I had my VESC from OllinBoardCo up and running for about a week with no problems, but that all ended Saturday afternoon...

It died under very innocuous circumstances; I was giving short, back-and-forth rides to my 45lb kid on the sidewalk when it just stopped responding. I power cycled it (big mistake, wish I would have pulled the fault code doh!) and still nothing. I then go inside and hook it up to the computer and pull faults and get the dreaded DRV_8302. VESC still connects/reads/writes fine, but any attempt to drive the motor results in 3 red LED flashes and a DRV code.

There are no obvious shorts and it has never been wet. I kept the shrink wrap on and all leads were well connected and insulated. After this happened and I removed it from the board, I removed the shrink wrap to see if I could see any glaring anomalies (yeah right, how in the hell do you wizards solder these things?!?), but there was just a little dust.

Earlier in the day, I was playing with the motor current and absolute current settings as well as FOC. Here are the settings and results...

Vesc 4.11 hardware with c18 mod done by chaka, 4.15 firmware. Single Bigfoot 160 245kv on 8s Lipo. 15/40 gearing on 83mm wheels- top speeds between 25-26mph on the flats.

Motor Mode: BLDC
Motor Current: 70a
Batt Current: 60a
Abs Current: 130a
Results: Mostly excellent, this was the setting I used most of the week and put probably 50 miles on. I was able to induce the occasional cut-out on full power starts. When I pulled that code, I got a couple of ABS over current (just barely, like 130.3 amps). So, of course I up the absolute current- saw a post of Vedder's where he says do not go above 150 ABS amps, so on to the next setting.

Motor Mode: BLDC
Motor Current: 70a
Batt Current: 60a
Abs Current: 150a
Results: Great! No codes, but I wanted a bit more so I upped the motor amps

Motor Mode: BLDC
Motor Current: 90a
Batt Current: 60a
Abs Current: 150a
Results: Very sweet acceleration and the mid to full power range felt great and just dangerous enough to be exciting. Cool, now lets try it on FOC...

Motor Mode: FOC
Motor Current: 90a
Batt Current: 60a
Abs Current: 150a
Results: Major cut-outs on full throttle accelerations (all slow rolling starts as starting from a dead stop feels bizarre to me). I pulled the codes and got an ABS over current of well over 200 amps! (I didn't save this one, unfortunately). 

So I reflashed back to the BLDC, 90amp motor, 60amp battery, 150amp absolute and was happy. It was using this exact setting that the DRV died, but under next to no load with me giving baby rides.

FOC mode on this motor was working as intended, except when I would coast at moderate speeds (maybe over 15mph) and then try to throttle back into the power very slightly, I would get a buzz-like short sound and slight braking force as it felt like the motor was trying to sync back up? The faster you go, the more braking force was encountered and it made the board difficult to control under FOC.

What do you think? Were my amps too high? Did I do damage with the FOC over current? Motor never got over 55c (infrared thermometer immediately after some hard hill pulls) and I never saw any mosfet heat related codes, but I wasn't actively monitoring during any of these rides either.

I've got an e-mail into chaka for return/repair service, so hopefully I'll be up and running again here shortly.
```

---
## \#2 Posted by: chaka Posted at: 2016-03-15T15:34:51.651Z Reads: 200

```
You drove it pretty hard but I also push my VESC's to their limits. I have yet to push the absolute max past the defualt setting though. You will want to dial the absolute max back down to the defualt setting and bring the current max down to 80 amps after you get the VESC back. I think you said you were running 8s, have you had any issues with the overtemp cutoff?

If you feel you need more power you may want to jump up to a dual drive or up your voltage and lower your KV otherwise you will continue to have issues with overcurrent and overtemp.
```

---
## \#3 Posted by: Qwiksand Posted at: 2016-03-15T17:39:50.415Z Reads: 193

```
Thanks chaka, I'll dial the currents down once I get it back from you. Dropped it off in the mail this morning to you.

As far as over temps, I can't be certain. I would occasionally get a little slowing on some hills, but I was always fairly close to my low-voltage thresholds as well. If the mosfets hit temp cut-off, will it leave a fault code? I've never seen an over temperature code if that's the case.

I was running on 8s, but I've got a 10s battery here to try out now as well. Honestly, the board had plenty of grunt on 70amp motor, 130amp absolute- I was just pushing to see what the limits were!

I hope these posts don't come off as though I'm disappointed with the VESC? Quite the opposite actually, I can't believe how much power/features come from such a tiny device driving tiny motors.
```

---
## \#4 Posted by: chaka Posted at: 2016-03-21T17:46:51.519Z Reads: 170

```
@Qwiksand I started testing the VESC. It had a small strand of copper bridging two pins on the drv. After I removed it BLDC mode worked fine without any fault codes. FOC is acting really funky so I will try replacing the chip and see if that solves the issue. I'll have more time this evening to make the replacement and bring it back to normal operation.
```

---
## \#5 Posted by: Qwiksand Posted at: 2016-03-21T22:26:42.755Z Reads: 157

```
Sounds great, thanks for working so quickly- I know you are a busy dude!  

I'm actually relieved that you found a physical fault (shorted pins) as the way this one quit had me scratching my head.
```

---
## \#6 Posted by: chaka Posted at: 2016-03-24T16:35:22.469Z Reads: 153

```
@ Qwiksand, I replaced the drv8302 and it is back to normal operation. I tested on FOC and there are no longer any fault codes. I also tinned those crimp connections for you. 

Did you still want to add the heatsinks? If you want the heat sink package just purchase the listing on my site and I'll add it before sending it out today. [http://www.ollinboardcompany.com/product/vedder-s-speed-controller-heat-sink-package][1]  No charge for the repair, you have always been super chill;) 


  [1]: http://www.ollinboardcompany.com/product/vedder-s-speed-controller-heat-sink-package
```

---
## \#7 Posted by: Qwiksand Posted at: 2016-03-24T20:38:56.133Z Reads: 145

```
Thanks man. Payment has been made, also ordered a kama connector. I really appreciate your customer service, especially this post-purchase support.
```

---

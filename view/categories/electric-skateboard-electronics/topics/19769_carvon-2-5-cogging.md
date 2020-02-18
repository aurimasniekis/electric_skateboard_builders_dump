# Carvon 2.5 Cogging

### Replies: 31 Views: 1801

## \#1 Posted by: mikey Posted at: 2017-03-27T15:36:14.946Z Reads: 183

```
Anyone have Carvon 2.5 cogging issues?

It happens for me 1 out of 5 times. When accelerating, usually at low speeds (i always push start).
It makes a clicking type of noise and doesn't produce any power. As soon as it happens Im afraid im going to blow a vesc so I let off on the trigger and try again.

My setup is **Dual Carvon 2.5 | 12s1P 26650 a123 lifepo4** 
Link: https://tinyurl.com/kfgynnd
Vescs are in FOC and connected to the receiver with a Y-cable. 

The settings on each vesc are:
**Current Limits**
Motor Max: 60.00 A
Motor Min: -60.00 A
Bat Max: 15.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A

**Voltage Limits**
Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V

I guess I can live with it. But its slightly nerve racking because its random. And I don't feel comfortable letting friends ride it for that reason. Whats the cause of this and what settings should I tweak to eliminate this?
```

---
## \#2 Posted by: Michael319 Posted at: 2017-03-27T16:01:14.379Z Reads: 169

```
I have a single 2.5, I've never had that issue.
```

---
## \#3 Posted by: Blasto Posted at: 2017-03-27T16:06:02.902Z Reads: 165

```
Could the 12s1p pack be sagging? Try lowering you cutoff atart and end to 33V and 30V?
```

---
## \#4 Posted by: mikey Posted at: 2017-03-27T16:20:35.116Z Reads: 154

```
Did you mean "Battery cut off start" from 35.20V to 30V?
```

---
## \#5 Posted by: Blasto Posted at: 2017-03-27T16:22:01.855Z Reads: 150

```
No sorry, cut off start 33V and cutoff end 30V
```

---
## \#6 Posted by: mikey Posted at: 2017-03-27T16:22:26.982Z Reads: 142

```
Could this issue be a bad soldering job on the bullet connectors? I de-soldered the bullet connectors on the motor side so I could wrap them with that paracord. :frowning:
```

---
## \#7 Posted by: laurnts Posted at: 2017-03-27T16:28:07.304Z Reads: 138

```
It looks like you have very low amp discharge with those 12s1p pack. Although you use th3 bigger brother of 18650 I think the discharge is still too low.
```

---
## \#8 Posted by: laurnts Posted at: 2017-03-27T16:29:58.302Z Reads: 131

```
However clicking sound seems to be incompatible firmware. If BLDC mode sensorless is okay, then most likely firmware not compatible with bldc tool or vesc hw version.
```

---
## \#9 Posted by: makevoid Posted at: 2017-03-27T16:42:08.013Z Reads: 125

```
Check for bad connections (bad soldering joints like @mikey suggests), loose bullet connectors, make sure there is no strain on the cables that go into the motor,  that the cables/connectors are not exposed in any point and that  they aren't making contact between themselves... etc.
```

---
## \#10 Posted by: saul Posted at: 2017-03-27T17:30:41.999Z Reads: 123

```
a123 cells can do 50a/120a. you can up the battery current to at least 20a-25a each. 
I would get a bigger battery...thats only like 5-6 miles?
```

---
## \#11 Posted by: Mrmoonlight Posted at: 2017-03-27T17:45:05.838Z Reads: 117

```
I just spoke with Jerry regarding this issue.
Try using BLDC instead of FOC and see if that solves your problem. I have a similar issue running FOC on my V2.5. At slow speeds and if there's a slight uphill, I get some cogging. If I give it a good push, it runs fine. Also, I had the clicking noise when I had it set up on an Enertion and DIY electric VESC, but when I installed the Ollins, the clicking went away. Cogging was also much better, but still not perfect. It would be okay if I wasn't in the city where there's a lot of stop and go. I'm also running a single, so I'm not sure if a dual has something to do with it. 

I run my v2.5 on BLDC and I have no issues with cogging and no clicking noises. Do you have vids?
```

---
## \#12 Posted by: mikey Posted at: 2017-03-27T18:15:44.287Z Reads: 110

```
Thanks! Ill take a video as soon as the weather gets better.

Man, I hope I dont have to run it in BLDC. I really enjoy how my setup runs right now.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-03-27T18:55:37.500Z Reads: 101

```
You can also try raising your motor max current to 80a. 
 I was able to improve low speed torque this way. 
I used to run at 60a and now I'm running both my boards at 80a with no harm to motors or Vescs. 
Just check the temp of your motors with your hand periodically to make sure there not over heating.
```

---
## \#14 Posted by: Mrmoonlight Posted at: 2017-03-27T18:59:12.929Z Reads: 100

```
Yeah, I really like FOC, but BLDC just runs so much smoother. I'm hoping VESC 6 and the new V3 sensored motors will solve the problems with FOC.
```

---
## \#15 Posted by: RunPlayBack Posted at: 2017-03-28T16:22:46.593Z Reads: 89

```
80a with the V2.5? Interesting I need to try this! What was the battery setup you have for both boards again?
```

---
## \#16 Posted by: Mrmoonlight Posted at: 2017-03-28T16:38:25.355Z Reads: 88

```
So are you running FOC at 80a with minimal cogging? How hard/long do you typically ride?
```

---
## \#17 Posted by: Namasaki Posted at: 2017-03-28T16:47:53.304Z Reads: 89

```
Both of my current setups are 
10s Lipo
Dual 6355 190kv motors 
15/36 pulleys with 9mm belts
Ollin Vesc's with heatsinks 
BLDC mode
Motor max 80a
Battery max 50a
If I recall, my Carvon V2.0 where rated for 80a
And I would imagine the V2.5 are as well. 
I ran my Carvons at 12s with TB 120a ESC's
I never got cogging accelerating on flat ground
```

---
## \#18 Posted by: Namasaki Posted at: 2017-03-28T16:49:38.181Z Reads: 89

```
I have not yet tried FOC
```

---
## \#19 Posted by: Mrmoonlight Posted at: 2017-03-28T17:37:34.769Z Reads: 88

```
I run my V2.5 on BLDC with my Motor Max at 60A. No issues with cogging. I can go from a complete stop. 
I run my Carvon V2 on FOC at 60A with no cogging issues. If I run my V2.5 on FOC, I get minor cogging.
```

---
## \#20 Posted by: Hummie Posted at: 2017-03-28T18:23:11.538Z Reads: 87

```
total of 30 amps limit with two motors seems very low
```

---
## \#21 Posted by: mikey Posted at: 2017-03-28T19:07:41.026Z Reads: 80

```
[quote="Hummie, post:20, topic:19769, full:true"]
total of 30 amps limit with two motors seems very low
[/quote]

What do you recommend?

I'm thinking of going BLDC with Bat Max at 25A on each. 
Not sure about Bat Min. Currently Bat Min is at -12.00 A
```

---
## \#22 Posted by: Hummie Posted at: 2017-03-28T19:11:56.163Z Reads: 77

```
12s 1p with the cells I dont know but I ride 70 battery on each vescs sometimes.  whatever your battery can do.
```

---
## \#23 Posted by: sman987 Posted at: 2017-03-28T21:36:42.803Z Reads: 74

```
I have the v2.5 does anyone know how to take the motor off??? i did damage to the hanger but the motors fine i would like to replace the hanger has anyone taken them off before???
```

---
## \#25 Posted by: caustin Posted at: 2017-03-28T22:11:56.662Z Reads: 74

```
Have never taken them apart that fully, interested to hear if others have advice. Post a picture if you can of location of the hanger damage. How did you mangle the hanger and not the hubs?
```

---
## \#26 Posted by: sman987 Posted at: 2017-03-28T22:41:28.673Z Reads: 75

```
I have a single and the wheel fell off because of me not  tightening it up
```

---
## \#27 Posted by: mikey Posted at: 2017-03-29T02:16:45.997Z Reads: 74

```
**UPDATE**
So i switched everything over to BLDC. I was still failing motor detection but with one vesc. 
I was getting "ABS_OVER_CURRENT". I checked the connections and tried again and got "UNDER_VOLTAGE" and the battery turned off.

Then I put the battery on the charger and ate dinner. It finished charging before I was done. 

Hooked it up again this time only one vesc, and it passed motor detection. I was going to unplug and testdrive it but right before I turned it off I saw I was getting "ABS_OVER_CURRENT" again. Then back to normal. It seems like its going in and out of it. 

Could this have been causing the cogging too?

Oh also. I talked with Dexter at DIY (thats where I got my battery, its also discontinued). The BMS is capable with 30amp/80amps. Im assuming thats 30A continuous / 80A max.
```

---
## \#30 Posted by: mikey Posted at: 2017-03-29T16:54:59.488Z Reads: 66

```
Does anyone know why one of my vescs shows "ABS_OVER_CURRENT" then back to none about every 30 seconds?
```

---
## \#31 Posted by: STREETSURFER Posted at: 2017-03-30T00:28:11.128Z Reads: 63

```
With my carvon v2 single, I get abs over current when I overload the vesc with braking or accelerating too hard.
```

---
## \#32 Posted by: mikey Posted at: 2017-03-30T04:04:24.268Z Reads: 59

```
Yeah im not doing anything. Its literally sitting on my desk idle unpsidedown. The remote isn't even on but it still goes in and out of abs over current.

Ollin said they will replace the vesc in question.
```

---
## \#33 Posted by: STREETSURFER Posted at: 2017-03-30T18:13:10.771Z Reads: 55

```
Yeah it sounds like a DRV related error code, hopefully it isn't the hubs causing the problem. If you don't have this problem sorted out by April 15th, I'll be in NYC and could offer you a hand with diagnosing the problem. We spoke about puch mopeds in the past if you remember me.
```

---
## \#34 Posted by: mikey Posted at: 2017-03-31T15:48:11.952Z Reads: 47

```
omg yeah! I sent my vesc into Ollin for repair already though. I narrowed it down to that one vesc because It still happened when I hooked it up to another motor.
```

---

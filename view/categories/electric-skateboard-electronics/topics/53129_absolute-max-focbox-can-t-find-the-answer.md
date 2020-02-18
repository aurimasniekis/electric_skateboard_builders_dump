# Absolute max focbox.. can’t find the answer

### Replies: 23 Views: 1781

## \#1 Posted by: Juvaknin Posted at: 2018-04-22T15:30:09.454Z Reads: 286

```
Cant find good answer. Sorry. 
The absolute max by defualt is 130A
What is this value?.?
And if im using 2 motors 2 focboxs, i should use 130A on each vesc? Or 65/65 each?.. or what?..
Using 10s 4p battery 30Q type. 
Motor 125kv 
Thanks...
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-04-22T15:34:47.991Z Reads: 282

```
Well you will never achieve that since your battery can only discharge 80 amps and split into 2 that's 40 amps per vesc and motor max should be around 60-80 could play with those values
```

---
## \#3 Posted by: Juvaknin Posted at: 2018-04-22T15:38:03.648Z Reads: 273

```
So i dont need to change it? It can be 130A on each vesc?
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2018-04-22T15:39:28.126Z Reads: 270

```
Do at your own risk, wouldnt recommend that , anyways bigger question where you get a 125kv motor from
```

---
## \#5 Posted by: Juvaknin Posted at: 2018-04-22T15:45:05.012Z Reads: 255

```
So what is the risk?.. what value is recommended?..
Got from someone who ordered them dont know where :) some china.....
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-22T15:46:51.088Z Reads: 247

```
[quote="Exiledd_Top, post:2, topic:53129"]
40 amps per vesc and motor max should be around 60-80 could play with those values
[/quote]
10 character
```

---
## \#7 Posted by: Juvaknin Posted at: 2018-04-22T15:47:58.968Z Reads: 237

```
Ok. Thanks
```

---
## \#8 Posted by: Hummie Posted at: 2018-04-22T15:50:18.514Z Reads: 239

```
theres the battery and the motor and I think a max setting beyond that I think.  you could put the motor amp setting up to the 120 I think without a problem as it doesn't decide the amps from the battery and you just need set your battery amps relatated to the cell limits.  ..and make sure the max isn't holding you back from the other settings
```

---
## \#9 Posted by: Deckoz Posted at: 2018-04-22T15:51:43.982Z Reads: 239

```
Abs max is for the fet side. Nothing to do with the battery amps. It's to prevent damage to the fets if the motor current spikes.
```

---
## \#10 Posted by: GrecoMan Posted at: 2018-04-22T15:54:27.145Z Reads: 234

```
DO NOT change that setting.
```

---
## \#11 Posted by: Hummie Posted at: 2018-04-22T15:54:37.470Z Reads: 231

```
isn't it an over-ride limit for the battery and motor amp limits,...or sounds like youre saying it's just on the motor side and just a limit for motor amps?   be pretty weird having a higher battery than motor amp limiti to begin with.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-04-22T16:08:15.452Z Reads: 221

```
It's in case there is a short, or you hit the gas but the motor is in magnetic lock from no sensors or high enough bemf and the current spikes, and the motor squeels. 

For the battery it is just DRV_OVER_CURRENT both in and out, and the control is shut down for a moment and resumes.  Motor side is abs_over_current at least from what I've seen, abs_over_currents are full shutdown of the DRV causing the MCU to reboot. 

I could be wrong. But those are the scenarios I've seen these faults..
```

---
## \#13 Posted by: Mathias Posted at: 2018-04-22T16:45:15.459Z Reads: 206

```
VESC tool help: 
![image|613x217](upload://f8LlQ821NK5eCAbVEpTSZB27RkQ.png)

Do not change it. The spikes happen all the time and are largely independent of the battery current (can happen between capacitor and motors). With 65 A you'd get constant cutouts of acceleration and braking, which might throw you off your board. It is not about your battery or motor current, it is about what the VESC can handle for a few microseconds before it notices and shuts down. 130 is high enough to not happen during normal operation and low enough to not damage your VESC.
```

---
## \#14 Posted by: Juvaknin Posted at: 2018-04-22T17:28:57.374Z Reads: 190

```
Thanks guys, got it.
```

---
## \#15 Posted by: Eboosted Posted at: 2018-04-22T17:58:22.230Z Reads: 179

```
If you are going above that limit then you do have a problem
```

---
## \#16 Posted by: lrdesigns Posted at: 2018-04-23T07:34:54.516Z Reads: 170

```
Some guys set ABS lower thinking it was safer, but it causes the vesc to reboot. :confounded: Which will most likley make you crash. :face_with_head_bandage:

130a seems good on the old 4.1 vescs, so I feel like you could go a little higher on a focbox.  But really it will make no difference unless you are getting unusual reboots. 

Set the battery amps at a safe level for your battery (40aX2), and motor can be much higher 60-120 ish as the motor amps can be higher when accelerating from a stand still. 

Oh and yes, what is the 125kv motor you speak of?
```

---
## \#17 Posted by: Juvaknin Posted at: 2018-04-23T17:54:49.423Z Reads: 153

```
Turnigy D5035-125KV Sensored motor. 

If im conncted to my bms(50A-BMS) you think battery max 20A and motor max 45A will be fine? Or i will be powerless with this settings?..
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-04-24T00:13:12.035Z Reads: 136

```
Good starting point. Depends on gearing, weight, skating experience, board length and setup etc.
```

---
## \#19 Posted by: TheManShaker Posted at: 2018-04-25T08:29:09.131Z Reads: 135

```
Turnigy has one sensored. It´s the D5035 with 45 Max Amp 8-12s
```

---
## \#20 Posted by: lrdesigns Posted at: 2018-04-26T05:56:46.284Z Reads: 127

```
The answer is don't change abs max, unless you really really know what your doing. 

And for anyone wants to know how far you can push a focbox for aboslute kill yourself power this is the settings. 

@Deckoz  
_"On my 13s5p with dual 6374_

_I run on each Focbox_
_50 Batt Max_
_-15 Batt Min_

_125 Motor Max_
_-65 Motor Min_

_190 ABS max._

_Lol stupid power…"_

https://www.electric-skateboard.builders/t/6355-6374-or-6384/53449/72?u=lrdesigns
```

---
## \#21 Posted by: Deckoz Posted at: 2018-04-26T12:32:44.426Z Reads: 118

```
You need a no limit firmware to do anything like that..... Otherwise motor max and Abs max are limited...

I'm editing this Because I don't want people confused with my ways.

- The copper pours, mixed with the thermal mass of the heatsinks make the focbox really only able to handle around 2500w continuous for a few minutes. Additional thermal mass(aluminum is needed) to run more, but still I wouldn't go to much past 50 Bat max, unless the foxbox gets a revision with 3 or 4oz pours. The 2oz will deal with up to around 100a burst, but not continuous (you'll eventually make the fets reflow themselves).

- regarding the fets. The fets on the focbox are rated up to 75v, and 250a provided they are kept below 60c. My motor amp settings may be high, but it really only affects low end acceleration. As motor max must conform to battery max as duty cycle increases. These are not continuous settings, they are for burst acceleration. If this doesn't make sense.. look up some of my other posts about motor current dropping as duty increases.

Please don't try this unless you know what your doing, and can match your outputs to your load(weight) and can keep the temps down. Another side note, amps normally aren't the ESC killer, heat is. But heat is generated by current(amps). If you cannot calculate your bldc, or foc values by hand with manual tests to verify the automatic detection settings, do not do this.
```

---
## \#22 Posted by: Namasaki Posted at: 2018-04-26T17:15:25.282Z Reads: 96

```
The absolute max is a last resort cutoff in case the softy back off strategy fails. 
Setting it too low is a big mistake. 
According to Vedder’s site you can set it between 130a and 150a per Vesc. 
I have been running mine at 140a for a long time with no issues.
```

---
## \#23 Posted by: onepunchboard Posted at: 2018-04-26T23:17:23.176Z Reads: 85

```
Ive done 120motor 150 abs i thought that was fast. you are insane dekoz XD. I can't even pull trigger all the way.
```

---

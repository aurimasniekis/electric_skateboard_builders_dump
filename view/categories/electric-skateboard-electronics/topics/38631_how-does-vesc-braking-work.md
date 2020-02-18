# How does VESC braking work?

### Replies: 31 Views: 3856

## \#1 Posted by: danielz Posted at: 2017-11-17T15:26:32.729Z Reads: 312

```
Is maximum braking power determined solely by the batterys maximum charge current (Therefore to increase braking power you have to add battery capacity). Or can the VESC dissipate braking energy via heat? 

Im a little confused as there is a negative 'current brake max' setting and a battery 'max regen' option.

Thank you.
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-11-17T15:34:04.285Z Reads: 314

```
You are limited by the battery pack you use. That means the limitation may lie with the cells, or with the BMS. 

Braking current arrives at the pack the same way charging current does. Your pack needs to be able to charge at the current your brakes can provide. 

If you send too much current into there you could either overcharge your cells or trip your BMS.
```

---
## \#3 Posted by: danielz Posted at: 2017-11-17T15:44:23.083Z Reads: 309

```
So if i set 'battery current max regen' to -10a. No matter what i set 'negative motor current max' to, it will only brake at -10a? In other words 'negative motor current max'set at either -10 or -40 will feel exactly the same, because -10 is max regen.

Oh and I dont use a BMS.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-11-17T15:49:50.651Z Reads: 297

```
say your max charge current for each cell is 4 amps. If you had a 2P that would be 8 amps maximum charge current. but even with a 3P, you don't just go down to -12amps and call it a day. Things can get sketchy down there, so i'd say keep it around -8. 

then set you negative motor amps to like -40 or thereabouts and you should brake like a bicycle, or at least start approaching that ideal. You'll need to adjust for your weight, and maybe compromise on the force of the brakes for your application.
```

---
## \#5 Posted by: danielz Posted at: 2017-11-17T16:05:26.018Z Reads: 294

```
Thanks

I understand all that side of it, its how the VESC works that is baffling and why is has two sets of braking currents (One from motor to VESC and one from VESC to battery) if braking strength is always limited by the battery max regen value.

I guess the only way to test is to leave battery max regen locked at -10a. And try incrementally increasing 'negative max motor current' above -10a.  If  the  brake strength increases, it must be dumping excess energy other than into batteries via heat.

Ive tried googling the answer but ive found nothing conclusive. Ill be back....
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-11-17T16:50:22.919Z Reads: 276

```
damn haha I run -20a batt min and -60a motor min
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-11-17T17:27:58.972Z Reads: 263

```
how big is your pack?
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-11-17T17:30:16.637Z Reads: 264

```
10s6p but limited to 5a charge
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-11-17T18:03:14.764Z Reads: 255

```
my BMS limits me to 6amps allegedly but i use -8 batt regen and a -50 on the motor side. 

Ever have a problem braking down hill and causing a reset?
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-11-17T18:04:18.778Z Reads: 253

```
nope. only problems i’ve had are brakes cutting out on full charge. not related to that though
```

---
## \#11 Posted by: NickTheDude Posted at: 2017-11-17T18:15:44.279Z Reads: 261

```
The difference between motor max and batt max has to do with duty cycle. Duty is basically the decimal of top no load speed your motor is currently running at. Its also the ratio of amps in the motor to amps coming from the battery. Eg If the VESC is pulling 10A from the battery, and the motor is spinning at 0.5 duty the motor will be at 20A which is how you can have 2 limits at the same time.

Since RPM = V * kV, if you lower RPM then you need to lower voltage as well since kV is constant. Because of this, the voltage in the motor is not constant, while the voltage coming out of the battery is. The amperage on either side needs to be different for the same amount of power to be moving through the system on either side. Duty just represents that difference.

Duty cycle is lowest at low speed, so the ratio of motor amps to battery amps is high. Say you were at 0.05 duty and you were pulling 10A out of the battery, you'd have 200A in the motor, that's enough to knock you on your ass, so you'd set a motor max limit to something smaller, usually people set it around 40-100A. The same concepts apply to breaking.
```

---
## \#12 Posted by: egzplicit Posted at: 2017-11-17T18:25:56.967Z Reads: 247

```
[quote="GrecoMan, post:8, topic:38631, full:true"]
10s6p but limited to 5a charge
[/quote]

It also depends what limits it to 5A. A typical 18650 can charge at 4A per cell. 6p means six parallel cells so you can push up to 24A and each cell still gets only 4A. If the 5A limit is from the BMS and u use it for discharge as  well, you can’t put battery min to more than -5A. If the limit is your charging port then you can still push up to 24A back (assuming the BMS allows it, if it’s used for discharge as well).

I run -12A per vesc (so -24A per total) on a 10s4p. Rated value is 4*4 so 16A but taking duty cycle into account I will generate 24A only if I apply full brakes from 100% duty cycle. Since I never do a full brake from top speed, I never actually push 24A back into the pack. And if I do, it’s for a good reason (emergency braking) and it will be a short spike so damage is minimal.
```

---
## \#13 Posted by: danielz Posted at: 2017-11-18T19:14:06.306Z Reads: 229

```
That makes perfect sense if the voltage in the motor is varied, is that only in duty cycle mode? In current control mode is the motor voltage constant and the current controlled directly.

I did a little testing today and it seems even with max regen locked to 10a, increasing negative max motor current does increase braking. It started raining, Ill have to double check tomorrow, maybe im imaging it.
```

---
## \#14 Posted by: MysticalDork Posted at: 2017-11-18T19:33:08.407Z Reads: 221

```
No, you're not imagining it. Increasing the minimum motor current improves braking especially at low speed. This is true in all control modes.
```

---
## \#15 Posted by: WARMAN Posted at: 2017-11-18T21:11:52.262Z Reads: 223

```
[quote="longhairedboy, post:9, topic:38631"]
Ever have a problem braking down hill and causing a reset?
[/quote]

[quote="GrecoMan, post:10, topic:38631"]
only problems i’ve had are brakes cutting out on full charge. not related to that though
[/quote]

Both valid reasons for bypassing the bms for charge only!
```

---
## \#16 Posted by: Namasaki Posted at: 2017-11-20T05:13:41.308Z Reads: 256

```
[quote="WARMAN, post:15, topic:38631"]
Both valid reasons for bypassing the bms for charge only!
[/quote]

I discharge through a bms and ride my brakes downhill on a full battery and get no reset. 
Watching my voltage while doing so, it appears evident that my bms monitors the regen charge and prevents charging when the battery reaches the overcharge detection voltage which is set at 4.28v
I have reached that voltage and continued riding the brakes downhill. My battery voltage would not exceed that limit but held there until I reached the bottom and let off the brakes. At that time the bms proceeded to trim the battery back down to 42v while I was coasting. 
During this test there was no reset and no overheating. 
This test was with the Bestech HCX-D223V1
I can't say if this is the same for other bms's.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-11-20T05:15:30.111Z Reads: 250

```
Here is an old thread with info on brake settings. 
http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#18 Posted by: Hummie Posted at: 2017-11-20T06:07:25.807Z Reads: 244

```
are there resistors in that bms that are capable of burning off as much energy as youre using going downhill?  wondering where the energy is going if not the battery.
```

---
## \#19 Posted by: MysticalDork Posted at: 2017-11-20T06:11:55.111Z Reads: 238

```
It's my understanding that the vesc can "recirculate" the regenerated power through the windings of the motor and the mosfets of the vesc to allow braking without generating any net power to the battery. The heat is spread between the motor and the fets.
```

---
## \#20 Posted by: Hummie Posted at: 2017-11-20T06:29:23.545Z Reads: 240

```
if the battery isn't connected and you brake its a quick doom, how would it be any different in this situation?  How exactly would it "recirculate" if you know?  sounds like it would have to be shorting the leads to brake
```

---
## \#21 Posted by: MysticalDork Posted at: 2017-11-20T06:37:46.097Z Reads: 235

```
Pretty much. Controlled shorting of the leads using the fets.
```

---
## \#22 Posted by: Namasaki Posted at: 2017-11-20T12:32:46.164Z Reads: 226

```
The bms I mentioned has some decent heat sinks on the fets it also has a heat sensor and would shut down if over heated. 
I wouldn't recommend braking a mile downhill with a full battery. 
My test was on a fairy short hill.
```

---
## \#23 Posted by: danielz Posted at: 2017-11-20T22:13:36.565Z Reads: 220

```
Yep confirmed, is seems maximum braking power is independent of maximum battery charging current limit. The excess energy must be wasted as heat like any other form of braking. Higher charge rate batteries are still the best way to go though, for better efficiency and to keep the motors cooler.
```

---
## \#24 Posted by: Ackmaniac Posted at: 2017-11-21T00:09:04.468Z Reads: 207

```
Let's say your settings are -50 A Motor min and -10 A Battery min.

When you do a full brake the VESC will try to achieve 50A brake power because with the remotes trigger you control the motor min value. Which means at half trigger the VESC will try to reach 25A brake power, at 3/4 trigger 32.5 A and at full trigger 50 A.

When you go full speed and brake full immediately then the duty cycle goes down. Because of back EMF which goes in the other direction but that's to much details.
So in reality the duty cycle drops to around 60% in this case.

At 60% 50A at the motor would be 30A (60% of 50A) at the battery. But battery min only allows -10. So the brakes wouldn't be as strong as the trigger tells the VESC. It will only brake with 16.6A (10 A / 0.6) at the motor.

While you continue braking the wheels becomes slower and the duty cycle quickly drops. So at 40% duty cycle the VESC still want's to reach 50 A brake power but that would mean 20A at the battery. But 10 A are the maximum so it will only brake with 25A at the motor.

At 20% duty cycle it is possible for the VESC to brake with 50A at the motor. 

So it is good to have a high battery min value. I for example set the settings about 50% higher than the max charge of the battery would allow. With 4A max each cell in a 4P setup that would be 16A. But i set it to 24A because i think it doesn't hurt the cell when you brake hard from time to time. And you reach these high amps only for like 2 or 3 seconds. And i try to brake gently at high speeds during my normal rides but want full brake power if i need it in a emergency scenario.

I think that charging the cells with a power supply at high amps damages the cells much more because it is a constant charge instead of a short pulse. But maybe i am wrong with my theory.
```

---
## \#25 Posted by: Charles_Chan Posted at: 2018-04-18T08:28:05.773Z Reads: 151

```
Hi everyone, do you know how to setup the force of brake via vesc-tool, to make skateboard can stop complete when i push the throttle to maximum? thanks
```

---
## \#26 Posted by: Exiledd_Top Posted at: 2018-04-18T15:06:59.931Z Reads: 143

```
Increase "motor min regen" its usually at -40 some have it at -60 at most play with those values vesc has a smooth throttle you generally don't want to stop completely at full break instantly asking for trouble that's what ESC's are for if your into that stuff.
```

---
## \#27 Posted by: briman05 Posted at: 2018-04-18T18:02:26.298Z Reads: 139

```
So I have Racerstar motors that has max current is 46A.  I have a 10s4p battery made of samsung 30q which has a discharge current of 15A and for a BMS i have a Bestech190 that has a max charge current of 10A. I'm running dual setup  So for motor max and min it should be 46 and -46 and for battery min it should be -5?
```

---
## \#28 Posted by: Deckoz Posted at: 2018-04-18T19:28:26.402Z Reads: 134

```
Are you bypassing the bms for discharge?

If so...
4p* 20a = 80a/2 ESC.. or 60 if you wanna use the 15a rating.

40a bat max per esc

3ah*4p = (12ah * 2c charge)/2esc = -12 bat min.

For simplicity for the motor...
Motor max 46
Motor min -46
```

---
## \#29 Posted by: danielz Posted at: 2018-04-18T19:54:36.729Z Reads: 133

```
Just correcting my comment from a few months ago. I was wrong. All braking is by regen. 

The reason for a separate regen current setting and negative battery current settings is to do with braking efficiency at difference speeds. So  low c rated batteries will break more poorly at higher speeds, but catch up with high rated batteries at lower braking speeds. The vesc designer guy explained it on his forum a few days ago.
```

---
## \#30 Posted by: briman05 Posted at: 2018-04-18T20:53:10.223Z Reads: 131

```
I guess I would be bypassing the bms for discharging because it is a 10a charging with no discharging.  It was from the group buy the TGH did in novemebr

http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D190.html

https://www.electric-skateboard.builders/t/us-bestech-charge-only-bms-modules/37797/115?u=briman05
```

---
## \#31 Posted by: Charles_Chan Posted at: 2018-04-19T04:03:10.982Z Reads: 116

```
Thank you very much all of your help, I am trying it. thanks so much.
```

---

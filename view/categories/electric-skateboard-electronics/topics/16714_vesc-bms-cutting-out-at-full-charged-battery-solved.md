# Vesc/BMS cutting out at full charged battery (Solved)

### Replies: 45 Views: 4443

## \#1 Posted by: Eboosted Posted at: 2017-01-26T19:07:15.755Z Reads: 246

```
If I ride my dual motors Loaded Vanguard with 10S4P after a full charge the VESC reboots itself at braking, if I ride it until the battery decreases at 95% the issue is gone and braking is perfect. 

I'm guessing the regenerative breaking increases the voltage of the pack over a given limit so it cuts outs in order keep it safe. 

What parameter should I change in the VESC to fix this issue?
```

---
## \#2 Posted by: Randyc1 Posted at: 2017-01-26T19:14:18.013Z Reads: 243

```
But max battery voltage to 56V
```

---
## \#3 Posted by: Eboosted Posted at: 2017-01-26T19:20:43.345Z Reads: 239

```
But it's already at 57V, should I lower it to 56V or should I increase it to 58V?

[img]http://i.imgur.com/IC6cNPW.jpg[/img]
```

---
## \#4 Posted by: Randyc1 Posted at: 2017-01-26T19:31:06.007Z Reads: 231

```
Hmmmm ? 
I had same issue but my Max was at 43v before i put it higher .

not sure what the prob is now ?
```

---
## \#5 Posted by: lox897 Posted at: 2017-01-26T20:43:24.604Z Reads: 212

```
Your battery max is very low. What batteries are you running?
```

---
## \#6 Posted by: lox897 Posted at: 2017-01-26T20:44:01.505Z Reads: 215

```
LEAVE MAXIMUM INPUT VOLTAGE AT 57V or you may damage the VESC
```

---
## \#7 Posted by: lox897 Posted at: 2017-01-26T20:44:53.391Z Reads: 214

```
Try and ride it and when you get the error plug in a laptop and check the fault
```

---
## \#8 Posted by: Eboosted Posted at: 2017-01-26T20:50:17.985Z Reads: 209

```
I'm runing 10S4P battery with Samsung 25R so 37V 80A. 

So, do you suggest to leave the value at 57V?
```

---
## \#9 Posted by: lox897 Posted at: 2017-01-26T20:51:26.726Z Reads: 207

```
Battery max needs to be 80 then. Maximum input voltage needs to be 57v
```

---
## \#10 Posted by: Eboosted Posted at: 2017-01-26T21:11:16.004Z Reads: 201

```
You mean Batt Max in Amps? change 30A to 80A?

I'm runing 2 VESC and the battery max discharge capacity for my Samsung 25R 10S4P should be 80A (40A or each VESC), as suggested by @ackmaniac I set this Batt Max to 30A

Please confirm if I understood correctly and this is the value you are refering to as I don't want to burn another VESC :cold_sweat:

[img]http://i.imgur.com/tNp3YWB.jpg[/img]
```

---
## \#11 Posted by: lox897 Posted at: 2017-01-26T21:14:14.110Z Reads: 191

```
Oh sorry, I didn't know you were running two vesc.. You could change it to 40 on each vesc unless your BMS is 60 amp
```

---
## \#12 Posted by: Eboosted Posted at: 2017-01-26T21:49:47.819Z Reads: 192

```
BMS is 60A, do you think this could be causing the cutting out issue?
```

---
## \#13 Posted by: Alextech Posted at: 2017-01-26T21:55:08.120Z Reads: 197

```
Your should reduce the amount of current allowed to be recycled back into your battery.  This can casue voltage spikes and trigger the over voltage,  also some BMS do not allow any regenerative braking beacuse it thinks it is a short,  depending on your bms.  My recommendation is to lower your regeneration to 10 amps.  I personally use this and runs a 12s4p effectively.
```

---
## \#14 Posted by: lox897 Posted at: 2017-01-26T21:58:07.354Z Reads: 192

```
That would mean 5 per vesc, correct @Alextech?
```

---
## \#15 Posted by: lox897 Posted at: 2017-01-26T21:58:47.326Z Reads: 193

```
Leave your battery max at 30 then. That wont be causing the issues, it is likely your battery regen as Alex explained.
```

---
## \#16 Posted by: Alextech Posted at: 2017-01-26T21:59:05.005Z Reads: 196

```
Yeah,  10 characters.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-01-26T22:15:20.835Z Reads: 196

```
Which BMS do you have in between?

When the VESC drops out during braking with a fully charged battery then the VESCs try to get rid of the power by charging it into the battery. But the BMS in between says no no no no, because for the BMS the Battery is already full. So the VESC can't get rid of the power and shuts down for safety reasons. Otherwise it would would overheat in a couple of seconds (maybe even less than a second). So i recommend to bypass the BMS for discharging and charging by the VESC and only use it for charging with a charger.
This doesn't count for a smart BMS which can handle the amps even at a full charge. But it seems that you don't have one of those.
After that you can set the battery min value to the value you like. Officially the manufacturer says 4 A maximum for each cell. So 16 A in total for your 4P Battery. 
But you can also go higher. Because this is only if you would charge it contentiously with these amps. But on the board you reach these values only when you brake very hard at full speed. And then only for a couple of seconds (maybe not even a second).
And i think it is better to have more brake power when something goes wrong on the streets instead of being worried that the cells might get a bit stressed.
And there are also articles where they say that short charge bursts are also good for the cell. Continuous charging at a high amperage damages the cells more.
```

---
## \#18 Posted by: PXSS Posted at: 2017-01-27T00:09:47.450Z Reads: 181

```
Can you link to said article that says charging at bursts higher than your max continuous in spec sheet is good for your cells? I call bs knowing what I know about how the chemistry in 18650 cells work.
```

---
## \#19 Posted by: Eboosted Posted at: 2017-01-27T00:20:29.948Z Reads: 184

```
@ackmaniac the BMS I have is the Battery Support 10S 60A

Is there anyway to avoid the cutoff by changing VESC settings?, I would not like to change the wiring of the battery at this point, everything is wrapped up and ready, however if there is nothing we could do software wise, I'll work on the wiring
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-01-27T00:31:35.619Z Reads: 200

```
No you can't change the setting of the vesc without risk of blowing it... the drv is only rated 60v.
```

---
## \#21 Posted by: Eboosted Posted at: 2017-02-09T06:31:29.917Z Reads: 193

```
I read the fault codes from terminal:

Fault : FAULT_CODE_OVER_VOLTAGE
Current : -14.2
Current filtered : -14.3
Voltage : 57.35
Duty : 0.27
RPM : 21833.1
Tacho : 453339
Cycles running : 10841
TIM duty : 3498
TIM val samp : 1748
TIM current samp : 8175
TIM top : 12854
Comm step : 5
Temperature : 48.62

Fault : FAULT_CODE_OVER_VOLTAGE
Current : -20.3
Current filtered : -15.9
Voltage : 57.41
Duty : 0.20
RPM : 17775.2
Tacho : 464138
Cycles running : 4798
TIM duty : 3221
TIM val samp : 1610
TIM current samp : 9744
TIM top : 16268
Comm step : 2
Temperature : 46.49

Fault : FAULT_CODE_OVER_VOLTAGE
Current : -11.4
Current filtered : -11.5
Voltage : 57.45
Duty : 0.23
RPM : 17776.1
Tacho : 486449
Cycles running : 6651
TIM duty : 3358
TIM val samp : 1677
TIM current samp : 8969
TIM top : 14583
Comm step : 3
Temperature : 47.65

Fault : FAULT_CODE_OVER_VOLTAGE
Current : -23.3
Current filtered : -16.5
Voltage : 57.63
Duty : 0.14
RPM : 14073.5
Tacho : 505408
Cycles running : 4414
TIM duty : 2848
TIM val samp : 1426
TIM current samp : 11865
TIM top : 20877
Comm step : 2
Temperature : 48.48

Fault : FAULT_CODE_OVER_VOLTAGE
Current : -34.5
Current filtered : -22.3
Voltage : 57.68
Duty : 0.10
RPM : 11553.5
Tacho : 522941
Cycles running : 3915
TIM duty : 2513
TIM val samp : 1264
TIM current samp : 13767
TIM top : 25007
Comm step : 1
Temperature : 51.99

So, this limit is being exceeded:
<img src="/uploads/db1493/original/3X/3/1/31f1a2b9c9e77bf82bc7c7b4588a7b12e81a921b.png" width="690" height="347">

So, I decided to make some tests today:

1. Decreased battery min (regen) from -8.00 to -5.00A
VESC still cutted out but a little less frecuently
Brakes were sluggish

2. Decreased battery min (regen) to -2.00A
Brakes force was almost non existent
VESC didn't cut out once

3. Increased Maximum input voltage from 57V to 58V
VESC cutted out at 58.7V (same problem, more voltage, less safe)

4. Reduced Motor min (regen) from -60.00A to -30.00A
Same issue, no change on feeling of the board on braking, VESC still cutted out

I'm out of ideas on what to test next, what would you guys suggest in order to avoid this that won't be charging the board at 89%, do you think it could have something to do with the small motor pulley?
```

---
## \#22 Posted by: PXSS Posted at: 2017-02-09T06:42:32.897Z Reads: 174

```
What battery do you have??? Even a 12S pack should not reach 57V
```

---
## \#23 Posted by: Alextech Posted at: 2017-02-09T07:15:56.303Z Reads: 178

```
Are you running a BMS? some are known to not take Regen Current.
```

---
## \#24 Posted by: Eboosted Posted at: 2017-02-09T14:44:17.103Z Reads: 191

```
I have a 10S4P with battery supports 10S 60A BMS made by @barajabali

The regen is very high and it overcharges the battery at >57V spikes at full batt charge.
```

---
## \#25 Posted by: Eboosted Posted at: 2017-02-14T06:36:47.948Z Reads: 188

```
Ok guys I fixed the problem.

The culprit was the BMS, it was cutting regen supply from the motors during braking in order to protect the battery to be charged more than 42V, nevertheless the motors kept spinning, hence braking and regenerating and the flow of current had nowhere to go, so it was being stored in the VESC raising the voltage until overcharge fault was thrown.

I changed this wiring:
BMS for charge and discharge
[img]http://i.imgur.com/hLX4AcM.jpg[/img]

to this:
BMS for charge only
[img]http://i.imgur.com/oeNLTjn.jpg[/img]
```

---
## \#26 Posted by: Luke Posted at: 2017-02-14T07:55:04.812Z Reads: 178

```
Hey there, Ive been worrying about this exact problem for a while now. I dont see how this solves the problem (although I'm happy for you that it has)
as far as I know, The issue is that when the battery is full and you brake, the VESC cannot dump any current into the cells, because the BMS tells the vesc that the cells are full.
Then the VESC is shutting down to protect itself.
Is what you have done the following:
When charging via regular wall charger, the charge goes through the BMS, this means that at a full charge, your cells are sitting at a nice happy 4.2 V
BUT when you brake with your motors, they send current straight to the cells, bypassing the BMS, so the cells may get to 42.1 V or something, but at least nothing shuts down.
Does the BMS not freak out at that point, telling the vesc that there's the problem (I keep thinking of a skateboard as a community talking to each other so that I can shred the streets)
```

---
## \#27 Posted by: PXSS Posted at: 2017-02-14T11:38:44.233Z Reads: 172

```
The BMS is not hooked up to the VESC so even if it shuts off power from the charger, the power is nit coming from there. 

@Eboosted, I suggest you add a fuse so you don't blow anything up now that you're bypassing the BMS
```

---
## \#28 Posted by: deucesdown Posted at: 2017-02-14T15:13:16.253Z Reads: 170

```
Is the general answer to this, to under charge slightly, maybe 0.5v? Your brakes then work even right off the charger, and you get more cycle life for your cells by 1. not overcharging during braking, 2. not charging to max
```

---
## \#29 Posted by: Eboosted Posted at: 2017-02-14T15:20:11.012Z Reads: 168

```
@PXSS I'll set a fuse between the battery and VESCs, unfortunately there no much space and the 80A fuse and fuse holder are extremely big.

Has anyone found a small and suitable fuse and holder for this application?

@deucesdown, if you check the charge on each cell the voltage at full charge sits between 41.6-41.00V so charging a little bit more won't cause any issues, some people charge it until 42.5V or even 43V, cell won't be automatically damaged, on the other hand this will be donr only for a fraction of time, I'd say between 1 and 2 minutes of riding.
```

---
## \#30 Posted by: LukeL Posted at: 2017-02-14T15:47:49.621Z Reads: 159

```
Isn't the maximum input voltage setting on the BLDC tool supposed to stop this?

I know a lot of people say to leave it at 57V to stop the vesc switching off but if you're discharging without a BMS shouldn't this setting stop you overcharging the battery?
```

---
## \#31 Posted by: PXSS Posted at: 2017-02-14T15:53:37.081Z Reads: 156

```
Not really. That setting is meant to protect the VESC from over voltage and not the battery. Setting it at 42V would only cause the vesc to shut off sooner.

2 options are set to 57v and slightly overcharge when braking or set it to 42v and not overcharge but shut off when braking
```

---
## \#32 Posted by: PXSS Posted at: 2017-02-14T16:00:05.964Z Reads: 155

```
Won't even happen for that long. It'll literally only happen while you are actively braking enough to charge the pack above 42v. As soon as you stop braking, the voltage should settle back down.
```

---
## \#33 Posted by: Eboosted Posted at: 2017-02-14T16:03:24.635Z Reads: 155

```
I rather have a 0.5% less battery cycles than loosing brakes at a street crossing
```

---
## \#34 Posted by: Sebike Posted at: 2017-09-13T12:26:39.241Z Reads: 125

```
Don't want to start a new thread as this seems to be similar to what I experienced today, but could you guys check my error log and see if this would in fact be the same issue as @Eboosted experienced? 

Not sure when I received this error code as board was on for several hours, but at the beginning of the ride with full batt. I had several losses of brakes when going down a very very minor slope at almost zero speed.. Had those brake cutouts a few times and avoided to go downhill and no more brake issues since.

 <img src="/uploads/db1493/original/3X/2/4/24f0fee895cd55561052196c09a7a632f773514a.png" width="281" height="500">
```

---
## \#35 Posted by: Eboosted Posted at: 2017-09-13T16:26:25.047Z Reads: 119

```
Are you discharging through bms?
```

---
## \#36 Posted by: Sebike Posted at: 2017-09-13T16:38:37.666Z Reads: 117

```
Yes. Same BMS as you had I believe. SuPower 10s 60A
```

---
## \#37 Posted by: scepterr Posted at: 2017-09-13T17:28:05.922Z Reads: 116

```
You went above the 57V max input limit
```

---
## \#38 Posted by: Sebike Posted at: 2017-09-13T22:02:14.291Z Reads: 116

```
Yes, and why was that /how could one avoid that?
```

---
## \#39 Posted by: scepterr Posted at: 2017-09-13T22:18:58.761Z Reads: 117

```
Breaking on full battery caused it, you could increase the limit to 58. Or just be mindful when full battery
```

---
## \#40 Posted by: Eboosted Posted at: 2017-09-13T22:43:21.650Z Reads: 116

```
There are ony two ways to avoid this:

1. Use the BMS for charging only, you will loose all battery protection features of the BMS for discharge

2. Charge up to 41.5V SOC (state of charge) instead than 42v, using a custom charger or soething similar than this:

<img src="/uploads/db1493/original/3X/7/9/798f7e4db91fc9295493d8a0a5d8be73544c6c07.jpg" width="442" height="500">
```

---
## \#41 Posted by: cryo Posted at: 2017-10-28T23:13:48.336Z Reads: 103

```
Couldn't there be a simpler software solution to this like an option for the vesc to just disable regen braking altogether when batteries are above a certain voltage?
```

---
## \#42 Posted by: Eboosted Posted at: 2017-10-29T02:11:29.955Z Reads: 96

```
No option st the momentu unfortunately
```

---
## \#43 Posted by: cryo Posted at: 2017-10-29T02:15:00.157Z Reads: 98

```
Paging @Ackmaniac :joy:
```

---
## \#44 Posted by: Ackmaniac Posted at: 2017-10-29T02:53:39.894Z Reads: 98

```
In a prototype i am already trying to adjust the brake power to stay within limits. Problem is that in Eboosted's case the result might be the same because the BMS shut's down immediately so the power can't go anywhere. So it doesn't really matter if it try's to reduce the power a little. What i have in mind is for my next 13S build. Just want to know if it is possible to do that. And there a reduced brake power is still better than no brake power. But i expect it to never touch these limits.

But long story short. **Use the BMS only for charging**. Or simply get rid of it and charge your cells with a external balance charger. Or don't use any of those and check your single cells voltage every now and then and if needed charge the single pack individually so that it fit's the others.
But don't integrate the BMS in the cycle with the VESC. It's useless. And most times the BMS fails instead of the cells. And if the cells fail then mostly because one cell cell looses connection. And the BMS balance current can never ever compensate that.
```

---
## \#45 Posted by: neobrain Posted at: 2017-12-15T20:14:36.438Z Reads: 81

```
Hi Ackmaniac,
i reallywould like to talk to u. 
its understandable that u tell the people to bring the bms into the charge circuit.
This is for pilot safety reason. the rider should have the same brake in all usecases, if full or empty battery. 
If battery is full and u brake, u cook ur batteries and u have less live cicle for the batteries, BUT brakeing is always the same and feels good..

But for me i really would prefer to have less brakeing power, which gets more and more braking, the more u ride and the voltage of batteries gets down. so u get way more cicles out of ur batterie. 

so iam really interested in the extended super vesc, which can handle the maximum voltage for brakeing. 
That would be so awesome.. So.. how can i help u?

f
```

---

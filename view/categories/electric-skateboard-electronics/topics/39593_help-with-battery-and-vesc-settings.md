# Help with battery and vesc settings

### Replies: 10 Views: 603

## \#1 Posted by: Lumaci Posted at: 2017-11-29T01:03:54.150Z Reads: 106

```
Currently setting up my vesc, i've been maxing it all out at max 20 amps but now i wanna redo it all and find the "perfect" settings for it but i need help with the battery.

I use a Meepo Board battery for my board since its what i had laying around, its using ICR 18650 S3 cells i dont understand much about the cells but what would my maximum allowed amp draw be in a 10s2p config with those cells at 4400mah together? Each cells is 2200mAh.


Edit, honestly not even sure if its the right cells, Might be LG MF1 18650 3.7V 2200MAH LI-ION BATTERY after ive taken a look at it.
```

---
## \#2 Posted by: Matthias Posted at: 2017-11-29T02:24:50.585Z Reads: 111

```
[quote="Lumaci, post:1, topic:39593"]
ICR 18650 S3
[/quote]
https://www.tme.eu/en/Document/851884e7c9339fa73b5bf66663baac51/ACCU-ICR18650-2.2.pdf
According to that document, the maximum continuous C-rate of your cell is 1.5. That implies that, as I understand it, you can draw 1.5x your energy (4400mAh) continuously -- So your cells can comfortably discharge at a rate of ~6.6A. I didn't see any information about burst currents,  but that information may be more pertinent to what you are trying to determine.
```

---
## \#3 Posted by: DAddYE Posted at: 2018-12-16T23:44:09.825Z Reads: 139

```
So l, you’re saying that with for example a 10s3p of 30q would be safe have -30/-30 on 2 motors?
```

---
## \#4 Posted by: trampa Posted at: 2018-12-17T08:19:36.063Z Reads: 113

```
If you apply two Motors and two ESCs to your system you use half the value for Max Motor and max Battery Regen. You will never pull full brakes at full speed, since that would send you flying. This would be the only scenario where you could theoretically push the Amps you defined in the software. The only other scenario that would generate the full Amp values for a longer period of time would be riding down a ridiculous steep hill at full speed with full brakes applied. The hill would need to be steep enough to keep you at full speed although you brake hard.
 
Conclusion:
The rider has a Amp flow limiter built into his throttle finger. 
The battery will never see the full 30 to 40A and high Amp flow will be seen for a very short period only. Remember: When you brake, you slow down and reduce the Amps therefore. 

Once the speed is lower and you can start to apply full brakes, the motor will not generate at full voltage and the VESC-Software will scale up the voltage towards the battery and lower the Amps towards the battery. 
Example for a 12S setup at half duty cycle: 25V and 30A at motor side equals 50V 15A at battery side. 
While your motor generates 30A, your battery only sees 15A with a fast dropping tendency. 

The battery ratings you can find in the spec sheet of your cell refer to a steady charge, applied for an extended period of time. Regen braking causes spikes, that is the nature of regen braking. If you want good brakes, you have to accept that the spikes are higher than the continuous charge rating of the cell. The best thing you can do is use a lot of parallel cells, resulting in a bigger battery pack. Or use high C-rated LiPos, which can deliver and swallow more Amps. 

When do you need strong brakes? At speed you will need them. Better put your health before the health of your battery. On E-Boards, your battery is the only device that is suitable to swallow the braking energy. When you close the gate towards your battery, you can't store the braking energy and in consequence the VESC will cut back the max achievable braking power. You will loose your capability to brake down your board when you need the brakes most! This is not a good idea. 

If you use symmetric settings there is also no need for funky Watt control modes found in another fork of VESC-Tool. If your basic settings are good, you don't need a patch to straighten things out again. 
The board will ride perfectly smooth and the throttle will be very linear. Ad some ramping time if you think that the throttle is to sensitive. 

What is most stressing for the battery is riding down steep hills for a longer period of time while constantly applying a lot of brakes. If you ride down such hills, you probably want/need good brakes and your battery + software-settings should be capable of handling that scenario. If your board has a 12S2P battery and you live in San Francisco, something is wrong already. A highly geared down 12S5P setup would be the solution.
```

---
## \#5 Posted by: mtuan293 Posted at: 2018-12-17T09:08:16.060Z Reads: 97

```
[quote="trampa, post:60, topic:77861"]
The battery ratings you can find in the spec sheet of your cell refer to a steady charge, applied for an extended period of time. Regen braking causes spikes, that is the nature of regen braking. If you want good brakes, you have to accept that the spikes are higher than the continuous charge rating of the cell.
[/quote]

Thanks for this advice. I'm always afraid of over charging my battery pack therefore I set batt regen to match the spec sheet, and have shitty brakes :smiley:

[quote="trampa, post:60, topic:77861"]
What is most stressing for the battery is riding down steep hills for a longer period of time while constantly applying a lot of brakes. If you ride down such hills, you probably want/need good brakes and your battery + software-settings should be capable of handling that scenario. If your board has a 12S2P battery and you live in San Francisco, something is wrong already. A highly geared down 12S5P setup would be the solution.
[/quote]
Fuck me I have a 10s2p pack and I live in Utah. Lots of hills here :neutral_face:
```

---
## \#6 Posted by: trampa Posted at: 2018-12-17T09:11:25.749Z Reads: 90

```
That will not help you to prevent overcharging! Overcharging happens when you charge beyond 4.21V. This can be done with 1A charging just as good as with 15A charging current. If you do not start your ride on top of a hill with fully charged batteries, you will always drain more than you put back in. Otherwise we would ride a perpetual motion machine, which doesn't exist.
```

---
## \#7 Posted by: mtuan293 Posted at: 2018-12-17T09:15:41.354Z Reads: 90

```
[quote="trampa, post:62, topic:77861"]
you will always drain more than you put back in. Otherwise we would ride a perpetual motion machine, which doesn’t exist.
[/quote]

I know there are things with efficiency when converting from chemical energy to mechanical energy. So ideally, if you have 100% efficiency, will you be able to gain the amount of energy you lose when going uphill by going down that same exact hill?
```

---
## \#8 Posted by: trampa Posted at: 2018-12-17T09:30:44.721Z Reads: 79

```
Ideally.....
```

---
## \#9 Posted by: DAddYE Posted at: 2018-12-17T11:04:35.518Z Reads: 63

```
Thanks for your explanation. Very informative. So if 30q are rated 4A, and I have a 3p, do you think I can set as battery max regen -60A total? Consider that living in SF means going down hill pretty often. What values would you suggest?
```

---
## \#10 Posted by: trampa Posted at: 2018-12-17T11:07:12.772Z Reads: 62

```
I would suggest to build a battery that is more suitable for eating hills. 
I would suggest to monitor the cell temperature to get an idea of how much thermal strain you put onto the battery.
```

---

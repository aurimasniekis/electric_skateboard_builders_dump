# Battery voltage and max input setting

### Replies: 35 Views: 3622

## \#1 Posted by: Evan Posted at: 2016-08-13T10:45:28.588Z Reads: 298

```
Using space pro4 10s battery. Did exactly the same setup as Jacob said in his video which was max input at 42 V when my battery was around 75% juice, ran perfectly. Then charging the battery to full but it started cutting itself off.

Connecting to BLDC tool everything seemed fine, didn't break any chip or ic stuff down which was a big relief. Found out the realtime data keept saying OVER VOLTAGE when I was using the remote to run the motor and motor detection failed and said "bad detection results and overvoltage error".

Well the question is can I just put 43v instead of 42v on max voltage input? Already tried put different amps on motor or battery but didn't make a difference. Only put 43V on max input would make everything running smoothly. Just wondering has anyone encountered this scenario and why would some people put 42V and nothing happened on their 10s board?
```

---
## \#2 Posted by: crameur Posted at: 2016-08-13T10:51:58.494Z Reads: 285

```
Yes you can, I don't know what batteries are in the space cell but standard LiPo are charged at 4,2V per cell so 42V. However if using 43V helps you putting 43V wont hurt your VESC. But you may check your charger because it seems like you're overcharging your pack.
```

---
## \#3 Posted by: Evan Posted at: 2016-08-13T11:07:02.672Z Reads: 271

```
Uh the bldc tool showed around 97% juice the voltage was like 41.4V then I used remote to crank it. Sometimes too much throttle it ran to 42v (just a instant, strange) then cut off. But when I run 42v for max voltage for motor detection it didn't cut off I thought its because didn't use full throttle.

I think I didn't overcharge the battery, as soon as I saw the charger showed green light then I disconnected them...but the fact was before that the battery itself already showed 100%. :nerd:
```

---
## \#4 Posted by: Namasaki Posted at: 2016-08-13T14:07:12.911Z Reads: 252

```
When riding, there will be some voltage sag caused by load which prevents over voltage fault when max is set at 42v
When bench testing, the absence of load reduces that voltage sag. 
Try setting max at 42.5 and if it still shuts down, set it at 43v. 
I don't think setting the max voltage 1 volt high is gonna cause any problem.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-08-13T14:11:26.974Z Reads: 251

```
It's normal for the battery to show 100% before the charger's green light comes on. Keep charging until the green light comes on. 
And you don't have to unplug the charger as soon as the green light comes on. The BMS will not allow the battery to over charge. And the if charger's output is 42v, it can't charge the battery higher than 42v.
```

---
## \#6 Posted by: chaka Posted at: 2016-08-13T14:18:54.570Z Reads: 239

```
Leave the max voltage setting at 57v. Its purpose is to save the electronics from overvoltage.  Setting it at 42v puts yourself in danger of losing brakes.  In what video did Jacob recommend this?
```

---
## \#7 Posted by: Randyc1 Posted at: 2016-08-13T14:59:35.191Z Reads: 219

```
Chaka is correct !,

 I have a 10s battery also and my Max Vol is set at 43V But ...when you Begin to ride on a fully charged 42v battery then you use BRAKES you Generate Voltage and this bring it over my 43V Max setting and cutts Off !!

I have yet not changed the setting to 57 V but i will to avoid this problem again .  This will happen in only the first few min of riding if braking ,untill Batt V drops a little.
```

---
## \#8 Posted by: E-Boarding Posted at: 2016-08-13T16:19:15.082Z Reads: 210

```
I had the same problem with the space cell and set the limit to 42.6V
```

---
## \#9 Posted by: Evan Posted at: 2016-08-13T22:12:05.869Z Reads: 194

```
[HERE](https://www.youtube.com/watch?v=4XHODLiXaJY&index=18&list=PLICpQdAXJazRzoXJByGA_5wd-B4cifmbh)

Okay so just wanna make sure that I can put 57v on my 10s pro4? Wow that's impressive didn't even think of that. I thought only 12s would use 57v setup....
```

---
## \#10 Posted by: ikjahaa Posted at: 2016-08-13T22:28:14.180Z Reads: 185

```
Even for 6s ?
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-13T22:32:07.243Z Reads: 174

```
I would just leave battery max alone at 57v, there's no reason you should have to change it.
```

---
## \#12 Posted by: chaka Posted at: 2016-08-13T23:22:56.801Z Reads: 168

```
The bms will protect the pack and the "shut off" should allow for brief peaks in voltage where the vesc is more sensitive.
```

---
## \#13 Posted by: elkick Posted at: 2016-08-14T08:32:01.227Z Reads: 161

```
The advice in that video tutorial to limit the max input voltage like this is completely wrong. And it is causing a lot of over voltage issues people are having with their VESC.
```

---
## \#14 Posted by: Evan Posted at: 2016-08-14T09:12:31.582Z Reads: 158

```
Well I was one of those guys lol
```

---
## \#15 Posted by: ikjahaa Posted at: 2016-08-14T12:41:05.636Z Reads: 156

```
perhaps some explanation by @jacobbloy why he did it that way in the video ?
```

---
## \#16 Posted by: jacobbloy Posted at: 2016-08-14T23:58:50.513Z Reads: 149

```
this is only done after you know your battery pack. the vesc will have voltage spikes when braking and this could be well over 10v for a very short 2-5ms. i know my pack doesn't charge over 41v so setting it to 42v has no problem me on most situations, the voltage spike happens when the motor stops spinning very quickly the motor in a geared system will slow down a lot slower with weight on the board and this generally means that more current less voltage.

the vesc is a very temperamental peace of hardware when you do not understand all aspects of the operation and the problem is even if i explained every thing i knew about it in my videos i would still miss things as i don't know every thing. also many would not understand or watch the whole video.

you don't have to set your voltage cut of settings at all if you have a good bms
```

---
## \#17 Posted by: jacobbloy Posted at: 2016-08-15T00:02:44.220Z Reads: 139

```
it also seems that the some vesc could have a voltage tolerance issue, get a good voltage meter test your battery voltage then test it on the vesc real time data you might find its a couple of V out
```

---
## \#18 Posted by: Evan Posted at: 2016-08-15T08:25:24.123Z Reads: 133

```
Thanks Jacob.
```

---
## \#19 Posted by: elkick Posted at: 2016-08-16T06:43:32.452Z Reads: 131

```
[quote="jacobbloy, post:16, topic:7589"]
i know my pack doesn't charge over 41v so setting it to 42v has no problem me on most situations,
[/quote]
The max input voltage value has nothing to do with the pack charging and setting that value below 57V is not helping there at all. @chaka mentioned this already in his above contribution as well. It creates unnecessary over_voltage_error messages all the time and the forums are full of it.

On a side note: the same applies to the general Enertion VESCs  presets "multiple ESC over CAN" which creates some additional issues (I am not indicating that this was you, but again, it's unnecessary).
```

---
## \#20 Posted by: jacobbloy Posted at: 2016-08-16T07:43:39.712Z Reads: 131

```
I wasn't saying it has any thing to do with charging, I was saying that my battery doesn't charge past 41v and I don't have any over voltage problems while setting it to 42v. But setting it to 42v stops my vesc from pushing 45v into a 42v battery pack when braking. But as I said if you have a BMS then there no need to worry about this.

As for multiple ESC over can, this is needed for running 2x vesc over can. What courses problems with the keys not working on your keyboard is having can Fardwarding enabled. But this is also required if you want to program 2x vesc from 1 USB port so in a application like the raptor it is good. But the same conflict can be caused by having 2x applications enabled at once like being in current mode in both ppm and UART and having UART and PPM set at the same time. But for my self I just quickly set my vesc to no application when wanting to debug and such with BLDC TOOL and my keyboard keys.
```

---
## \#21 Posted by: Randyc1 Posted at: 2016-08-16T11:57:12.256Z Reads: 124

```
Jacob when your battery is full charge 41V and you brake hard , its does'nt trigger over voltage and cutt off , since your Max is only 42V ??
```

---
## \#22 Posted by: t1m0007 Posted at: 2016-08-29T23:59:16.160Z Reads: 116

```
https://youtu.be/4XHODLiXaJY this one
```

---
## \#23 Posted by: randomguy27 Posted at: 2016-09-20T00:09:44.412Z Reads: 104

```
how do i know what settings i can used for what i have battery 8.8AH 24V  18650 Lithium-ion and 1200W Brushless Hall Sensor Direct Current for the motor and how would i go about adjusting and changing the stuff. is there an application?
```

---
## \#24 Posted by: Hummie Posted at: 2016-09-20T00:44:36.818Z Reads: 104

```
Why is there a max voltage?

The two low voltsge cut offs are very important if u don't use a bms and will slow u than almost stop u when they are hit and not damage ur batteries. U probably know 

I dont know specifically those 18650 and I think u can drain them down to about 3 each but look at a discharge graph and find where they drop off.
```

---
## \#25 Posted by: LukeL Posted at: 2017-02-12T22:53:20.758Z Reads: 76

```
[quote="elkick, post:19, topic:7589"]
The max input voltage value has nothing to do with the pack charging
[/quote]

is this true if you don't have a BMS?

What vesc setting stops it from over charging your battery? or do you just assume regen from braking is so small that this is not a problem
```

---
## \#26 Posted by: Nisse977 Posted at: 2019-11-06T10:29:43.454Z Reads: 22

```
Sorry for reviving an old thread, but I rather do that then start a new one about the same subject :slight_smile:

I wonder **how** the VESC will cut if I would use this max voltage setting as a protector for the battery?. Will it ramp down the regen amps, or will it do actual short cuts or will it cut of and not come on again for many seconds?

I ask about this because I live on a hill, so there for I am afraid to overvolt my pack to much when going down my 8 degree 400 meter long hillroad. I fully understand that cut = means no brakes ;)

Until now I usually do not charge my board at home, I use it for commuting to work, and charge it at work so I do not have the hill-problem with a fully charged board.

**One time I did charge the board fully (4.2v per cell) at home and then went out riding with my family. After just 30 seconds into the ride, my son went in front of me with his bike and I had to brake, the board braked for a second then it let go and died on me = no go and of course no brakes... I jumped off** :open_mouth:

After checking the electronics I found that the VESC was dead... It was a Flipsky dual FSESC4.20 and one side of it was dead.
It looked like the BMS had cut the power to the VESC when I braked, and that cut killed the VESC...

So I would much rather prefer to have the VESC ramping down the brakecurrent or do "ABS-like" cutting wile braking then to have the BMS cutoff and break the VESC so I have no brakes at all....

What do you other guys do, are you running the leads straight to the VESC, not through the BMS and allowing higher voltages to hit the cells during short bursts of regen?
How high voltage per cell do you allow, 4,25-4,35V ?

Thanks in advance!
```

---
## \#27 Posted by: Hummie Posted at: 2019-11-07T07:08:47.707Z Reads: 20

```
[quote="Nisse977, post:26, topic:7589"]
How high voltage per cell do you allow, 4,25-4,35V ?
[/quote]
Depending on the battery chemistry and how fast it’s charged it might get to 4.35 but could drop down to 4.2 in moments.  You can charge ion cells much higher before bursting into flames
```

---
## \#28 Posted by: Santino Posted at: 2019-11-08T05:14:50.127Z Reads: 16

```
In that case I would charge the battery to 4.1V ; to give me more time for a emergency brake, full stop....Also you will get longer life span of you cells...charging at 80% it's not bad at all....You could also get a bigger battery, so you do not loose much range by charging at a lower capability...
```

---
## \#29 Posted by: Nisse977 Posted at: 2019-11-08T08:14:37.282Z Reads: 14

```
Thanks for the responses!

Today I have a **12S3P 10Ah** battery that I made out of used **Sanyo 18650GA** (3350mAh, 10A) cells. It gives me about **40-50km real range** with my type of riding, whitch is good to me, but the cells are not new, they still have the capacity, but not the current output, so they sag alot during power output and spike during input (regen). When charging at home, I charge only to about 3.80-3.90V to be able to handle the downhill. But when charging at work I charge to about 4.13-4.14V.

During winter I will build a battery out of brand new **Molicell 21700-P42A cells** (4000mAh, 30A). I have already ordered them :slight_smile:
It will be the same setup = 12S3P because that fits my board very well. The P42A cells have at least **3x times the current** output compared to my old cells (and 12Ah in total = 50-60km range), so I assume they will sag less and spike less = I can charge them higher at home because they will spike less going downhill. But at the same time I will probably rise the regen current setting (battery Min) due to the P42A cells ability to handle more chargecurrent, so maybe they will spike some anyway... Only the real world test will show.

When going down my 8 degree hill at about 30-35km/h, at full brake the regen current maxes out at 10A that is my Battery Min setting. That brake power Is not enough to slow down the board at that speed, but enough to stop it from accelerating more. That is 3,3A per cell, and that is what they can take in chargecurrent read from the specs. The P42A are supposed to be able to handle 8,4A per cell = 25,2A in regen/chargecurrent. I guess I would use 10-15A to keep the board at a safe constant speed downhill, and more if I must brake to a stop.
Only the real test will show how muck the cells will spike.

Do you think I can safely test to set the Input Max Voltage low to see what happens during braking (on a flat road) or do you think that there is risk of braking the VESC by doing so? I assume the VESC should be able to take it, but I do not know.
```

---
## \#30 Posted by: Evan Posted at: 2019-11-08T23:10:34.094Z Reads: 14

```
I've always wondering people with huge motors and fast setup going above 60kph(trampa riders lol)..... how do they stop? How come their battery pack can handle that kinda regen...
```

---
## \#31 Posted by: Hummie Posted at: 2019-11-09T00:10:55.902Z Reads: 15

```
 the manufacturers state a charge current intended up to full voltage but if youre charging for shorter periods and when not as close to full you're able to charge at a much higher rate.

   Ive thrown a 3v and a 4v 30Q cell together in parallel and I cant even say for sure either cell increased temp but minutes later they were close to balanced and a lot of current had been transferred.    maybe a more revealing test would be throwing a 4v cell in with a bunch of 4.2 cells to see if it gets warm.

big motor or little would matter very little.
```

---
## \#32 Posted by: Nisse977 Posted at: 2019-11-14T15:21:35.772Z Reads: 15

```
That is a good question.

Bigger motors or higher speed will generate higher amps to the battery as your wrote. Maybe they run with much larger capacity batterypacks, if they don´t do that, I guess they will just abuse their batteries then swap them out after a while. 

From what I can se on Trampas webpage about batteries, there is alot info about how many **lipo** packs you can put in their batteryboxes, not li-ion. And some lipos do come with an 5C chargerating. If that is a good real working thing, I do not know, but 5C into a 12S 16Ah pack is 80A of regen power, that is alot more stopping power than my 10 or 12Ah li-ion batterypack (my old one takes 10A and the new will manage 25A regen current).
```

---
## \#33 Posted by: Hummie Posted at: 2019-11-14T19:02:18.910Z Reads: 14

```


A bigger motor won’t increase the charge current and 95% decided by the kv.    The higher the kv the more amps produced for the same braking performance.

the manufacturer’s stated charge rates are very conservative and you can do much more for short periods without risk especially at lower voltage.  They state such a rate as intended continuously all the way up to 4.2 volts which is when it would be most detrimental
```

---
## \#34 Posted by: Nisse977 Posted at: 2019-11-15T10:18:55.659Z Reads: 11

```
Thanks for the reply! You say size does not matter then :smiley: :smile:

Okey, so beltdriven higher kv motors will generate more current compared to hubmotors that are bigger with lower kv. But beltdrive make the motors geared down, so do they generate about the same current because of that compared to directdrive hubmotors?
```

---
## \#35 Posted by: Hummie Posted at: 2019-11-15T16:13:50.045Z Reads: 8

```
I think it will produce amps when braking the reverse of how it would perform as a motor so a bigger gearing will require less amps to drive the motor and also will produce less amps when used as a generator.
```

---

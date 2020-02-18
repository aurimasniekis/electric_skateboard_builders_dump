# How to safely calculate max regen current?

### Replies: 23 Views: 1171

## \#1 Posted by: Skatejitsu Posted at: 2019-04-01T18:13:58.813Z Reads: 285

```
10s8p pack with Sony VTC6 cells.  I have my max discharge for my battery set to 92A which seems fine.  My braking feels weak and I have that set to 46A max regen and a pretty aggressive braking curve set in FOC software.

How do I calculate safe regen current for this setup?  I have a charge only BMS so current is going right from unity to battery.
```

---
## \#2 Posted by: sharky Posted at: 2019-04-01T18:47:38.406Z Reads: 280

```
![IMG_6298|281x499](upload://h5py3Z2qQ9JV36ETlSjz4ZuiwXT.png) 
Hey nan im running a 10s4p dual setup and those ar my settings
The breaking should be set with a negative value as far as i know
But be careful if you use the charging when breaking function dobt put a too high value in there
```

---
## \#3 Posted by: skatardude10 Posted at: 2019-04-01T18:49:13.934Z Reads: 270

```
I'm finding a charge current of 3A. To calculate max Regen, take the max charge rate * P count.

8 * 3 = 24A. If you have dual focboxes or vescs, it would be half that, or 12A Regen per. Negative of course.

This is relatively conservative, it may be just fine setting a couple amps more Regen, 26-28A total, or 13-14A per vesc.
```

---
## \#4 Posted by: sharky Posted at: 2019-04-01T18:50:04.061Z Reads: 270

```
Also read this sonewhere in the forum 
You can sumarize it to.    
Motor Max = Power at low speed.  50a
Battery Max = Total Power or Power at high speed
Motor Min = Brake power at mid to low speed
Battery Min = Brake power at high speed
```

---
## \#5 Posted by: lrdesigns Posted at: 2019-04-02T02:42:59.110Z Reads: 242

```
There is no definitive answer to this question because the data sheet only states max charge rate from empty to full. Usually around 1 hour or 1c. But esk8 use is pulse charge for a few seconds. 

If you want a conservative setting you take the max charge rate in the data sheet and X the number of cells in Parallel. For example if that is 3amp and you have a 8p pack. That would be 3x8=24 amps. Then in vesc settings battery regen -24 amps. /2 if you run dual motors/vescs. (On Focbox Unity I think it has only one battery setting so you don’t need to divide by two.) 

Motor regen current is not important to battery safety as the battery regen current is actually what is going back into the pack. If you set the motor regen really high you will get more low speed brake power. High battery regen will effect high speed brake power more.

With all that said it is a good idea to run higher than conservative if it means you will not crash into something at high speed due to not enough brakes. It may just shorten the cycle life of the battery instead of your own life. :wink:

If your battery gets hot from breaking you must live at the top of a huge mountain. Hot is bad. 

Since 1c on VTC6 8p pack is -24 amps, 2c should be -48 amps and would theoretically change the battery in 30mins. Personally I still think that is a conservative setting as you would would need to brake at full power for 30 minutes to achieve that 2c charge. Impossible on a skateboard unless you get towed by a car?

https://www.kronium.cz/uploads/SONY_US18650VTC6.pdf

Official

https://files.dcpower.eu/datasheets/sony/us18650-vtc6.pdf
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-04-02T03:33:30.274Z Reads: 211

```
as @skatardude10 has said, the limit is 3a for continuous charging. in my experience, you can use 1.5x that and still  be ok. the burst charge current shouldn't do any real damage to the cells. the limiting factor for alot of 18650s and charging them is how hot they get. for a short few seconds of braking, you would be fine setting your regen to 35-40 amps at most. i wouldn't risk anything above that. also, if you plan on going down a mountain pass and riding the breaks at max, set regen at the safe guarantee of 24a.... if you dont have enough braking power with that, you can still mess with your mac brake current, just dont touch the regen current
```

---
## \#7 Posted by: Skatejitsu Posted at: 2019-04-02T12:06:34.866Z Reads: 177

```
Great in-depth explanation, thanks!
```

---
## \#8 Posted by: Acido Posted at: 2019-04-02T12:24:38.226Z Reads: 175

```
P number x max charge for the cells x 1.5 / number of vescs

Im using 2x and i didnt notiece any damage in the cells
```

---
## \#9 Posted by: Bjork3n Posted at: 2019-04-02T12:35:52.383Z Reads: 163

```
Is this the same for 30Q? 
10s4p = -24A total is safe?
```

---
## \#10 Posted by: meesie Posted at: 2019-04-02T15:46:46.913Z Reads: 153

```
just gonna leave this here:

www.esk8-calculators.com
```

---
## \#11 Posted by: Jinra Posted at: 2019-04-02T15:49:06.237Z Reads: 153

```
I use -30a total for safety. The way I brake I'm sure a reasonable amount of current is going back to the batteries, probably around half that.

Also FWIW this -30a total is what the Raptor 2 uses by default as well.
```

---
## \#12 Posted by: Bjork3n Posted at: 2019-04-02T16:39:43.348Z Reads: 142

```
From what I've seen the raptor 2 uses -10A on each vesc?
```

---
## \#13 Posted by: Jinra Posted at: 2019-04-02T16:43:56.669Z Reads: 139

```
currrently -15a, it might have been lower in the past.
```

---
## \#14 Posted by: Acido Posted at: 2019-04-03T06:04:27.093Z Reads: 128

```
Yes, that should be alright
Since I have one motor im using -40 on a 10s4p 
You wont be breaking with more than 5-10A for like 10seconds anyways
```

---
## \#15 Posted by: sayekim Posted at: 2019-04-03T14:44:32.555Z Reads: 122

```
Should we not also consider the voltage of the cells on a fully charged battery?

If there is no bms involved and you have cut off value of 57volts on the esc then when you would brake on a fully charge battery going at x speed at full brakes you would easily hit this value and the esc would cut off power but never mind that
I want to know how bad this is to the battery since you would be going way over the 4.2 volts per cell to 4.75 in a 12s setup. 

With a bms included in my case and most others, my bms will cut off power when going over 51,x volts which I suppose is a lot less bad but still you would be over charging the cells. 

How bad is this over charging anyway?

Sorry for being a bit off topic but considering you are already going to decrease batt min to a lower value then spec you would hit these over volts even sooner so it is sort of related.
```

---
## \#16 Posted by: linsus Posted at: 2019-04-03T16:52:39.267Z Reads: 112

```
You need a pretty big freaking hill to be able to impact the pack. Just a few seconds on a full charge wont do alot. If you have the possibility, charge to 4.1-4.15ish. Will give a few more cycles and you wont have to be paranoid about the brake issue.
```

---
## \#17 Posted by: Battosaii Posted at: 2019-04-03T17:25:39.874Z Reads: 110

```
Dual 6355 on 12s4p I use 80a max motor and -65a for brakes and do -12a brake Regen. I use the same settings on my 4wd build but I have a 12s8p but the brakes I lowered that to -50 cause 4wd has way more braking power
```

---
## \#18 Posted by: skatardude10 Posted at: 2019-04-03T17:38:10.959Z Reads: 107

```
I wish more standard BMSs would balance charge up to 4-4.1v without requiring an expensive programmable BMS. Community made BMSs are great for this, but also relatively expensive compared to the cheap, small charge only options. 😑
```

---
## \#19 Posted by: janpom Posted at: 2019-04-03T17:46:18.257Z Reads: 105

```
You can just charge to 4.1 * S total voltage, e.g. 41V for 10S pack. It won't balance your cells but it's definitely not necessary to balance on each charge, especially if you don't charge to full.

Then just charge to full occasionally to get the cells balanced.
```

---
## \#20 Posted by: skatardude10 Posted at: 2019-04-03T17:53:22.080Z Reads: 100

```
That is true, I am just mildly concerned when using lowish (4-5P) under high discharge (25-35A VTC5a or just pushing any cell near or beyond it's max discharge) the balance drifting more between full balance charges than standard discharge rates or higher P packs. My 25rs sag a lot so I always do a full balance charge before riding, and balance sometimes takes a while. It'd be nice to know you always get a full balance but save some life on your cells without going to full charge voltage. This would leave headroom for braking as well. If i had a diebiems I'd for sure set to 4.0-4.1v.
```

---
## \#21 Posted by: janpom Posted at: 2019-04-03T18:18:44.323Z Reads: 94

```
Makes sense. You could use the LLT Power Smart BMS. It's relatively cheap.
```

---
## \#22 Posted by: linsus Posted at: 2019-04-03T20:44:00.426Z Reads: 90

```
Diff between my supower 12s and diebie is like.. 40 bucks? You get what you buy.
```

---
## \#23 Posted by: pookybear Posted at: 2019-04-24T05:57:45.756Z Reads: 65

```
Is brake regen the same as battery min?
```

---

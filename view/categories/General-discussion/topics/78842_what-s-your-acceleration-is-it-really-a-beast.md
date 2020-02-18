# What’s your acceleration? Is it really a beast?

### Replies: 48 Views: 901

## \#1 Posted by: pat.speed Posted at: 2018-12-24T06:35:55.965Z Reads: 284

```
So I was discussing acceleration on another thread with @rusins and I think this would be a cool way to compare how powerful your board really is once you are actually on it.

The easiest way to calculate your acceleration is to first use @Kug3lis’s calculator and enter your values to get your max wheel torque in Nm. (this feature may be added in later. Here’s the link https://calc.3dservisas.eu)

Once you have your rotational torque you can translate it into forward force by dividing by the radius of your wheel. In my case 0.0485, I have 97mm wheels. All measurements should be in meters or the same units.

This gives me 16.5Nm / 0.0485 = 340Nm of force

Finally we can use the formula acceleration = force / mass. A = 340/60 (I weight 60kg...Yes, I am a midget)

Therefore acceleration = 5.7m/s/s or 5.7m/s^2. This means for every second I travel I will gain 5.7m/s of speed. So theoretically it will take me about 3-4 seconds to reach top speed.

What’s your max acceleration? Would you beat me? Smoke me? Or get smoked by me?
```

---
## \#2 Posted by: AlexBE Posted at: 2018-12-24T07:09:03.876Z Reads: 260

```
Alternately, tape your phone to your board and use an accelerometer app on a fairly smooth path. Or plot speed vs time from VESC telemetry.
```

---
## \#3 Posted by: 257 Posted at: 2018-12-24T07:11:29.412Z Reads: 265

```
Been awhile since physics 101 but..

![image|281x499](upload://9pZJDzWU1tRsh8hNQ5UmO9jkCPI.jpeg) 

18.432 Nm / 0.05 m = 368.64 Nm force 

160 lbs x 0.454 kg = 72.64 kg

Accel = 368.64 / 72.64 = 5.075 m/s^2

5.7 - 5.075 = 0.625

Looks like you just smoked me by 0.625 m/s^2
```

---
## \#4 Posted by: evoheyax Posted at: 2018-12-24T07:11:52.529Z Reads: 245

```
Yea, I don't buy that calculator. IT says I only get 2.36 Nm total between 4 motors, with 12kw of power, lol. That's def not right. I get 0-20mph in 3 seconds. Seriously, good luck staying on at full throttle.
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-12-24T07:22:55.959Z Reads: 241

```
Well u doubt then forumala itself ;) 

Formula is simple 60 / (2 * PI * kV) * Motor current = Nm

I guess u use hub motors and 3kW ea so around 60A and 80kV and gear ratio is 1

((60/(2 * 3.14 * 80))*60)*4 = 28.6624203822 Nm

Any direct drive sucks at torque pretty badly
```

---
## \#6 Posted by: pat.speed Posted at: 2018-12-24T07:23:28.691Z Reads: 230

```
Try it again, it was updated recently as it used to only count the single motor torque
```

---
## \#7 Posted by: pat.speed Posted at: 2018-12-24T07:25:24.877Z Reads: 225

```
Oooooh sounds like a close and race, this would be a fun way to race people in different countries haha
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-12-24T07:26:27.962Z Reads: 224

```
Is your wheel diameter 97mm or just radius? Because radius is half diameter... So for e.g. 107mm is 53.5mm

![image|355x323](upload://gYJ9AlEFeUmWOpDvdujBUKjoeyH.png)
```

---
## \#9 Posted by: pat.speed Posted at: 2018-12-24T07:28:57.873Z Reads: 216

```
Ahhh bollocks I did entered diameter. Instead of radius. Thank you, it’s meant to be radius though right?
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-12-24T07:29:38.951Z Reads: 212

```
Yes, when I will be back in hotel I will write down some more thoery on acceleration and etc stuff.
```

---
## \#11 Posted by: pat.speed Posted at: 2018-12-24T07:32:28.286Z Reads: 206

```
I’m not sure if radius is right though as that means I’m accelerating at about 20km/h which cannot be correct, can it?
```

---
## \#12 Posted by: pat.speed Posted at: 2018-12-24T07:34:48.354Z Reads: 197

```
I just entered your rough values and it says 25Nm, maybe you entered something wrong last time
```

---
## \#13 Posted by: 257 Posted at: 2018-12-24T07:35:23.078Z Reads: 186

```
Hell yeah we could get everyone’s acceleration numbers and start a ranked leaderboard thread lol
```

---
## \#14 Posted by: pat.speed Posted at: 2018-12-24T07:35:44.626Z Reads: 191

```
Sounds cool, great idea
```

---
## \#15 Posted by: Kug3lis Posted at: 2018-12-24T07:45:44.707Z Reads: 191

```
He probably run quad hub motor setup which is around 80kV motors 1:1 gear ratio, 3kW motor power rating
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-12-24T07:47:47.499Z Reads: 191

```
Shit I wrote 60 but phone converted it to 6 for some reason

EDIT: nvm it suppose to be around 30 something he wrote incorrectly...

![image|690x410](upload://vaGDodMLKLJrffMi2yqjRyRyf6w.png)
```

---
## \#17 Posted by: pat.speed Posted at: 2018-12-24T07:53:07.153Z Reads: 177

```
Are you sure it’s not meant to be divided by diameter as I’m getting about 5.5m/s/s acceleration which seems a bit high
```

---
## \#18 Posted by: pennyboard Posted at: 2018-12-24T07:55:13.047Z Reads: 177

```
I really like this concept but I feel like there's a big difference between theoretical acceleration and what you can put to the ground without belts slipping, rider falling off, etc. I think it'd be really cool for people to post their 150 foot drag times. And would be interesting to compare to production boards as well.

If anyone's curious, I got 5.49 m/s/s acceleration using the calculator and my mass of 77 kg.
```

---
## \#19 Posted by: Jc06505n Posted at: 2018-12-24T07:55:58.871Z Reads: 175

```
[quote="257, post:13, topic:78842"]
Hell yeah we could get everyone’s acceleration numbers and start a ranked leaderboard thread lol
[/quote]

I’ve been actually thinking of making an Esk8 leaderboard app that would take data and show leaderboards (similar to the boosted showdown this past summer). There would be different leaderboards based on city, state, country, continent/region, Fraction (think NY Collective vs Baesk8) and Globally. Builds would also be ranked based on Theory Specs vs Real World Preformance and would be given classes and ranks. Based on the data put in one would be able to see were their board would stack theoretically next to production and other builds via theoretical drag race and charts like Skatemetric does. 

Don’t know about how popular it would be and if the work towards starting it would be even worth it.
```

---
## \#20 Posted by: pat.speed Posted at: 2018-12-24T07:56:26.614Z Reads: 163

```
Yeah I’m getting about 5.6m/s/s at 60kg but that seams far too high to me. That’s almost 20km/h every second, I’d be reach top speed in just under 3secs
```

---
## \#21 Posted by: pennyboard Posted at: 2018-12-24T07:58:52.830Z Reads: 153

```
What's your top speed? I feel like my board reaches 30mph in around 3-4 seconds and I usually don't even max out my motors
```

---
## \#22 Posted by: pat.speed Posted at: 2018-12-24T07:59:54.347Z Reads: 150

```
About 37mph because I geared it down as I didn’t need the speed
```

---
## \#23 Posted by: rusins Posted at: 2018-12-24T08:03:29.238Z Reads: 147

```
3-4 seconds to reach top speed sounds about right. And I like the idea of actually measuring in the real world how fast we reach our top speeds, because then battery limits come into play as well as other things, like, being able to control the board, in my case. :smiley:

 I have current limits set to 30A per motor, because otherwise I need to hold on to the front of my board when starting up, but also need to stand up for control before max speed gets reached, and that's too dangerous of a maneuver :smiley:
```

---
## \#24 Posted by: pat.speed Posted at: 2018-12-24T08:05:47.135Z Reads: 140

```
Haha same, I’ve lost traction on fast starts sometimes if the roads rough. 

I tried to drag race my little brother the other week on his single motor board I was off like a rocket but he was lagging behind doing a burnout hahah
```

---
## \#25 Posted by: Bjork3n Posted at: 2018-12-24T08:06:08.978Z Reads: 140

```
Are you guys finding that acceleration is better in FOC compared to BLDC?
I feel that when the bldc reaches some momentum it really pushes hard :)
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-12-24T08:07:21.227Z Reads: 153

```
Motor torque is calculated in calculator by diving motor power rating by maximum battery voltage for e.g:

Power Rating 3000W and at 12S maximum voltage is 50.4V so maximum current is 3000W/50.4V = 59.5238095238A (60A)

Torque is calculated by this formula:

![{\displaystyle K_{\mathrm {T} }={\frac {\tau }{I_{A}}}={\frac {60}{2\pi \cdot K_{V}}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/e5be5d25f8db6677fa9c398d3ccf0625eac98b48)

so for 170kV motor torque with 3kW power is:

![60/(2 ÏÃ170)Ã60](https://www4f.wolframalpha.com/Calculate/MSP/MSP728109h6e5fa2e4e61f000020aice25g80b29cf?MSPStoreType=image/gif&amp;s=43) = 3.3Nm

The board has 1:3 gear ratio so we multiple 3.3Nm by 3 as gear ratios multiply the torque. We get 9.9Nm per motor at ideal conditions.

Now as we get torque (angular force) we can calculate the actual wheel to force:

![Torque applied to wheel results in force on edge](https://www.school-for-champions.com/science/images/force_torque_wheel.gif)

By using this formula (for 200mm radius wheels):

F = T/R = Torque / Radius of the wheel

F = T/R = 9.9 N*m / 0.1m  = 99N

Now we have force. By using F = ma formula we can calculate acceleration.

a = F/m = 99N / 100kg = 0.99m/s^2

So 50km/h will be reached by calculating this way:

![image|294x96](upload://leQJw2HKievpbeO8jgSkMbLvQzI.jpeg) 

Vf = is final speed Vi = is initial speed

Vf = 50km/h = 13.89m/s

so t =(13.89m/s - 0m/s) / 0.99m/s^2 = 14.03s

# It would take 14s for single motor with 1:3 gear ratio and 3kW (60A) power to reach the 50km/h speed in the ideal world without any friction resistance and etc stuff and if you kept your throttle full power and motor was consuming full power 60A at all the time.
```

---
## \#27 Posted by: pat.speed Posted at: 2018-12-24T08:07:23.053Z Reads: 142

```
I run bldc and when reaching about 15km/h it really pulls and I nearly shit myself every time
```

---
## \#28 Posted by: Bjork3n Posted at: 2018-12-24T08:09:53.550Z Reads: 141

```
Couldnt describe it better haha.
"im ready , im ready...Holy shit"..

https://www.youtube.com/watch?v=90DWXmj55_g
```

---
## \#29 Posted by: Kug3lis Posted at: 2018-12-24T08:15:17.200Z Reads: 135

```
Just to understand how absurd these numbers are lets take my board for e.g.

Here is specs:

Dual motor gear drive
kv: 180kV
gear ratio: 1:5
motor current: 150A/ea
Wheel size: 203mm = 101.5mm radius
Full curb weight: 110kg

Nm/A = 60 / 2 * π * 185 = 60 / 2 * 3.14 * 185 = 0.05164400069 Nm/A

Nm (Full Power) = 0.05164400069 Nm/A * 150A = 7.7466001035 Nm (per motor)

Nm (After gear box) = 7.7466001035 * 5 = 38.7330005175Nm (per motor at wheel)

Force = 38.7330005175Nm / 0.1015m  = 381.6059164286 N (per motor)

Total force both wheels  = 763.2118328572 N

a = 763.2118328572 N / 110kg = 6.9382893896 m/s^2

so to reach 50km/h (13.89m/s) at best conditions

t = (13.89m/s - 0m/s) / 6.9382893896 m/s^2 = **2.0019343703s**
```

---
## \#30 Posted by: pat.speed Posted at: 2018-12-24T08:22:52.834Z Reads: 128

```
All these figures are cool for comparing but I doubt any of us can reach 50km/h in less than 3 seconds
```

---
## \#31 Posted by: Kug3lis Posted at: 2018-12-24T08:24:50.185Z Reads: 127

```
Plus ESC does not provide that exact power at start up sometimes its even higher current as at low duty 0.1 voltage is like 5V :D
```

---
## \#32 Posted by: TowerCrisis Posted at: 2018-12-24T12:30:52.595Z Reads: 121

```
![Screenshot_20181224-042716|690x448](upload://pBEn6GhNfayKZzWQseG6b6p9nVB.png) 
![13834450|282x282](upload://2DAf9NxcSPsMI4vhmuGmX7XIcpA.jpeg) 

(In all seriousness, thank you for that thorough analysis!)
```

---
## \#33 Posted by: billappleton Posted at: 2018-12-24T15:15:58.602Z Reads: 111

```
I am looking for the best way to reduce my acceleration on FOCBOX Unity

If I hit the remote too hard the board will throw me off
```

---
## \#34 Posted by: FredrikHems Posted at: 2018-12-24T15:18:14.173Z Reads: 111

```
[quote="billappleton, post:33, topic:78842"]
reduce my acceleration
[/quote]
What??? 
Jk, just lower your motor max current. Could also lower batt max if thats not enough.
```

---
## \#35 Posted by: billappleton Posted at: 2018-12-24T15:38:12.618Z Reads: 113

```
i lowered battery max from 60 to 50 and that did help

is lowering the motor better?

what about the "ramp to start" and "ramp to brake" settings in the Unity Tool?
```

---
## \#36 Posted by: FredrikHems Posted at: 2018-12-24T15:57:06.554Z Reads: 109

```
Motor max is basically the max amps that you can use at low speed, like when accelerating. Batt max is basically the max amps that you can use at high speed. Therefore its normal to lower motor max first, and if that isnt enought, you can lower batt max. This is obviously very simplifyed, but it kind of works like this. 
I havent adjusted the «ramp» settings, so cant say for sure.
```

---
## \#37 Posted by: evoheyax Posted at: 2018-12-24T21:24:49.660Z Reads: 103

```
It's an interesting comparison... According to this, a 3:1 gear ratio with a 190kv motor 4wd would have about 36Nm vs my 28.66Nm.

But your leaving out key factors about the motor design that affect torque. I threw 30a per motor through the v1 hummie hubs and 30a through the new, double stator sized v4 hummie hubs, and the torque is completely different and much better. Same settings, same kv, same controllers, same battery, same voltage, completely different amount of torque...
```

---
## \#38 Posted by: SkaterBoy58 Posted at: 2018-12-24T21:55:53.394Z Reads: 99

```
Some of your force will be used to overcome pavement surface wheel frictional resistance and even more force will be used to overcome air resistance and the balance will be used to accelerate.
and of course if you are going uphill there is force required to overcome gravity
I have an excel sheet to calculate all of these
```

---
## \#39 Posted by: pat.speed Posted at: 2018-12-24T21:56:20.111Z Reads: 99

```
Well apparently motor size doesnt affect torque output...aparrently
```

---
## \#40 Posted by: skatardude10 Posted at: 2018-12-24T22:37:21.992Z Reads: 99

```
2.818 m/s/s. 

Calculated, should take my board and my weight ~7 seconds to reach 70km/hr. 

With real world testing it took me 7 seconds to reach 65km/hr, and another 5 seconds to reach 70km/hr.

So to answer OPs title, acceleration wise, no. Not a beast.
```

---
## \#41 Posted by: Battosaii Posted at: 2018-12-24T22:47:43.511Z Reads: 94

```
is it me or does the calculator not work atm? at first i thought it was my phone so i tried on my laptop and nada.
```

---
## \#42 Posted by: Kug3lis Posted at: 2018-12-24T23:07:47.355Z Reads: 101

```
https://en.wikipedia.org/wiki/Motor_constants#Motor_Torque_constant
```

---
## \#43 Posted by: evoheyax Posted at: 2018-12-24T23:13:16.922Z Reads: 102

```
You are correct. But also, it doesn't take into consideration stator saturation. This is for example what I expereinced. So even though I threw 30a at each vesc, the motor couldn't use it all to create torque.
```

---
## \#44 Posted by: Kug3lis Posted at: 2018-12-24T23:15:35.672Z Reads: 102

```
Yes, plus the motor consume power not esc pushes power to it. ESC just limits how much motor can suck out of battery.

These all numbers are just some basic form of formulas which would never produce exact same amount of power in real world as it is not a single formula for everything there are thousands more formulas involved in everything.
```

---
## \#45 Posted by: RadCat84 Posted at: 2019-05-27T22:37:40.370Z Reads: 70

```
Im using a 2.4ghz rc remote simple one with no modes. How do i increase acceleration on the unity with the UI app, what is the easiest way?
```

---
## \#46 Posted by: ZachTetra Posted at: 2019-05-27T22:50:17.473Z Reads: 70

```
Raise the motor amps limit?  Remote had nothing to do with it
```

---
## \#48 Posted by: kalebludlow Posted at: 2019-05-27T23:11:16.735Z Reads: 65

```
Could also mess around with the throttle curve to get something a bit more satisfying
```

---
## \#49 Posted by: IndyPilot Posted at: 2019-05-28T06:41:38.627Z Reads: 43

```
Enough with the math, let’s race...
```

---

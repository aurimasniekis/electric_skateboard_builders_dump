# First build - need help &#124; single SK-6374 192kV, Vedder VESC, 2x 3S 7500mAh 40C

### Replies: 11 Views: 1116

## \#1 Posted by: saybot Posted at: 2017-07-17T17:36:06.563Z Reads: 158

```
Hi guys,
i reading this forum for a long time so i decided to build my own e-longboard.
First of all i order some parts:
- Rayne Hellcat desk
- Caliber trucks
- 97mm blank wheel

- motor and wheel puley printed in 3d printer (40:15)

- Maytech SK-6374 192kV sensored motor (http://www.michobby.com/product/maytech-6374-190kv-brushless-sensor-motor-for-electric-skateboardse-bike/)

- Remote controller (http://www.michobby.com/product/maytech-new-2-4ghz-wireless-remote-controller-with-receiver-for-electric-skateboard-longboard/)

- motor mount customized made in CNC

- Vedder VESC (http://www.michobby.com/product/vedder-vesc-speed-controller/)

- Vedder anti-spark switch + led switch ( from esk8 GoldenHusky )

- 2 x battery 3s 7500mAh 40C battery (http://www.dx.com/p/11-1v-7500mah-40c-mobile-power-battery-pack-for-car-start-464026#.WWzw74jyhPY)

- Voltmeter (https://pl.aliexpress.com/item/2017-Hot-Sell-Waterproof-Battery-Meter-DC-3-0-30V-Auto-Car-Gauge-Digital-Voltmeter-LED/32806295616.html?spm=a2g0s.9042311.0.0.NiNArp)

<img src="/uploads/db1493/original/3X/d/3/d3e842196aae00f0672d230bea3e9e871740c8bb.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/b/3/b344abf4304ffa5789fe12f2ff4857c78f22fe0d.JPG" width="375" height="500">


<img src="/uploads/db1493/original/3X/2/b/2b7649ae743fcf81476abdaf18f556ef621fbd11.JPG" width="666" height="500">

I've got almost all parts on place - just waiting for batteries. 
Then ill start to mount everyting.
My first question is about wire schema. 
1) Is it prepared well? Should i change something?
2) where i should connect sensor wire from motor? To VESC?
3) how many Ampers should have fuse in Vedder anti-spark switch?
4) what charger should i use for this build?
<img src="/uploads/db1493/original/3X/c/9/c9990174f2ce71f3631193e48127f91af1fbcf1d.png" width="690" height="227">
```

---
## \#2 Posted by: Sander Posted at: 2017-07-17T17:41:10.116Z Reads: 130

```
For the motor, connect the sensor wires where it says "Optional hall-sensor or pulse encoder" on the very top left.
<img src="/uploads/db1493/original/3X/2/6/26e5a011d85c4d35155bdd337da4d723d9992d49.jpg" width="690" height="460">

Max current for your motor is 65A, so to be safe have a 60A fuse.

The max Ampere you can pull from your battery is 7.5Ah * 40C = 300Amps (just to so u know)
```

---
## \#3 Posted by: saybot Posted at: 2017-07-17T17:43:05.105Z Reads: 119

```
thx Sander
```

---
## \#4 Posted by: oren Posted at: 2017-07-18T04:29:51.251Z Reads: 96

```
I've been using the B6AC V2 charger. It's not the fastest but it's inexpensive and has been working well.
https://hobbyking.com/en_us/imax-b6ac-v2-professional-balance-charger-discharger.html
```

---
## \#5 Posted by: wafflejock Posted at: 2017-07-18T06:16:13.816Z Reads: 94

```
Charger all depends on how much you want to spend on it and how long you want to wait for a full charge basically.  Since you effectively have 7.5Ah 6S if you were to charge at a 1C rate which is always safe then you'd be charging at 7.5A (can usually go 2C or higher with these high discharge rate batteries but would check manufacturer specs if you're interested in faster charge times and don't care about the cost of the charger).

Basically since you have 6S fully charged that's 25.2V.  If you wanted to charge at 1C you'd be done charging in about an hour when fully empty but would be charging at a rate of 7.5A, at that rate the charger needs to be able to handle at bare minimum 7.5A*25.2V = 189W (assuming 20% loss in the charger can do 189W*1.2=226W)  So basically need a 230W charger to charge at that rate, if you cut the charger power in half to 115W you can charge at half the amps 1/2C rate which is good for long term cycles for the cells but will be slow (2hrs to fully charge + some balancing time).  With a 40W charger you'd have to cut the amperage down, so 40W/25.2V ~= 1.5A, so to fill 7.5Ah at 1.5A it takes 7.5Ah/1.5A = 5hrs to fully charge.  My setup I use a 80W charger with 2 5S 5Ah batteries, I charge them separately at 3.6A so it takes about an hour and 45min to fully charge each one if I deplete them completely (usually I just top them back up from 3.6V per cell so I'm actually filling like 3400mAh or less juice back in the pack and charge times are closer to 45min-1hr per battery).

Someone please correct me if I goofed on the math or explanation here anywhere.

---

Instead of getting a more expensive charger you might also consider just doubling up on the cheap ones and charging both batteries with different chargers.

---

Or if you want to make it rain :slight_smile:

https://hobbyking.com/en_us/turnigy-reaktor-300w-20a-ac-dc-synchronous-balance-charger-discharger-eu-plug.html 

Be sure with whatever charger(s) you choose they have the right plug/transformer built in or comes along with it for your region.
```

---
## \#6 Posted by: saybot Posted at: 2018-02-21T17:17:15.316Z Reads: 60

```
after few month ifinally i found some time so i back to the my started project with E-longboard.
Ive changed baterry from poor lipo to li-ion Samsung 25r with Bestech 10s BMS. Then i build spot welder and make 10s4p battery
I design my enclosure in Solidworks and printed in 2 piece with 3d printer.

![IMG_0352|281x499](upload://brYQvfmW90zmDTgj72INx5sXnqT.JPG)![IMG_0353|281x499](upload://sWF2EJMIyqR6f2isGBEkNel7Re.JPG)![IMG_0228|375x500](upload://68pEWThuc1jSy3bLUh1kFKsXFRc.JPG)![IMG_0230|666x500](upload://f9iUFVYoJyhOHbuC5yQ8FLeKX3o.JPG)![IMG_0351|375x500](upload://tiAyMUrMgSQirp6SoSEWrTn2uwx.JPG)![IMG_0229|375x500](upload://jWCeNkrEO16trqXjlHrv5Ghegds.JPG)

Ive got question, 
1) is it necessary to use antispark switch when my BMS have e-switch? I have lack of space in my enclosure so good if i can resign with antispark switch. I have also antispark XT90 before vesc

2)E-switch wires must be bridged during charging?

3) how to resolve power led switch which is ligh up (with very low light) when system is off
```

---
## \#7 Posted by: Acido Posted at: 2018-02-21T17:40:01.257Z Reads: 55

```
If you are going to use that multimeter for a long time and not only for eskate i reccomend getting  one from a reputable brand.

And also to get aluminum pulleys since these will wear for sure
```

---
## \#8 Posted by: Acido Posted at: 2018-02-21T17:40:51.955Z Reads: 55

```
If you want to be able to have a modular setup, ability to remove stuff like vesc or disconnect the battery without sparks and simple, than yes you need one
```

---
## \#9 Posted by: saybot Posted at: 2018-02-28T12:32:59.771Z Reads: 52

```
my project almost done:
finish setup:
deck:Rayne Hellcat desk

trucks: Caliber trucks II

wheel: 97mm blank wheel

motor and wheel puley printed in 3d printer (ratio 40:15)

Maytech SK-6374 192kV sensored: http://www.michobby.com/…/maytech-6374-190kv-brushless-sen…/

BMS :my own specification http://www.bestechpower.com/37v10spcmbmspcb…/PCM-D223V1.html

motor mount: cnc aluminium

Vedder VESC (http://www.michobby.com/prod…/vedder-vesc-speed-controller/6)

Vedder anti-spark switch

Battery: 10s4p Samsung 25R - 36v, 10Ah, max continous 80A

enclosure: designed in SolidWorks, printed in 3d ptiner


![28279079_10215784985883472_9038044537619354944_n|281x500](upload://kSWHXarAULk6INWI9ss77FOP1W6.jpg)![28276896_10215779272580643_9547392116226497_n|375x500](upload://i091YeRwlAbbeYicUSqDb53qZVS.jpg)![28238815_10215779271100606_4266941080082354147_o|666x500](upload://jm4Oi36kGjcuFVFnAzIpXJ6Doux.jpg)![28424527_10215779270860600_4760554386507065348_o|666x500](upload://3ty4sgd8WKDuHsUyqa3fv9zx7uE.jpg)![28280019_10215784982243381_2680864558752574110_n|281x500](upload://9LHPKuQKm95o0wrx3Eu6VtwnsRI.jpg)
```

---
## \#10 Posted by: saybot Posted at: 2018-12-12T10:05:34.030Z Reads: 29

```
After a year of riding i felt i need to change something.
The goal was to make something more stylish than ive got now with little bit more improvements.
So i run solidworks with inspiration of boostedboard style and that is my effects of work.

In this project ill use: 
- loaded vanguard clone deck (camber shape not included in SW sketches)
- torque wide track
- 2x SK-6374 (buy one more since ive got one) or 2x6355
- battery will stay but in another shape 10s4p - i've already little bit changed shape of original boosted enclosure to fit more batteries.
- dual vesc still dont know which one will be the best Dual Foc box, or Dual vest from maytech or maybe someone suggest another solution for 2 motos.

Tracks with motor mount, skid plate and cover cap (skid plate and cover cap can be exchangeable) is already done - final version is nice and clean. Now ill start to make both enclosures.

![2|690x426](upload://21oaSeVNuqzo4cutXazuw24vT2k.png) ![1|690x416](upload://mfcqdGCFy2TEU6h3ysJkoaTrO0l.png) ![3|690x426](upload://3J90txQK7NepGYPiAMipIBZWIyZ.jpeg) ![4|690x416](upload://bLXevDlzKXRwNIjtjMiU17PCA3F.png) ![IMG_1600|375x500](upload://xdZ4hRVhogLXjPKsmRIrAIJJjLo.jpeg) ![5|690x421](upload://n9yIDL9Ii4kiLnAHzSWgl0NCtSb.jpeg) ![IMG_1846|375x500](upload://dzT4iK1cfhuJ7b0Ja4LYfPbwqS5.jpeg) ![IMG_1847|375x500](upload://iNuRzsabrSrfSmTN39B1bAvbyDo.jpeg) ![IMG_2377|281x500](upload://eC9XJR08cYpPAah14nDlfDoBrcV.jpeg) ![6|690x426](upload://utWFi4f8zNuasvEhzacP0xwZvkX.png) ![IMG_1597|375x500](upload://iJr1HqyToeX9Z5u7I2S338kfjX.jpeg) ![IMG_1599|375x500](upload://9HuPPiOGokkQm04n67aAnHkcGkW.jpeg) ![IMG_1845|375x500](upload://j4gkn3MUWxGqREvQKE12vshGXUP.jpeg)
```

---
## \#11 Posted by: JibeBigo Posted at: 2018-12-12T10:26:00.464Z Reads: 24

```
Those trucks are wide AF, if feel this will change the feel of the loaded deck and imo defeats the purpose of using it.
I might be telling bs though :joy:
```

---

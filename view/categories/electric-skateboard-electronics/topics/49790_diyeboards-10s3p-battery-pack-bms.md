# Diyeboards 10s3p battery pack BMS?

### Replies: 5 Views: 857

## \#1 Posted by: JULMTL Posted at: 2018-03-22T00:28:36.699Z Reads: 160

```
Hi guys, I am currently working on my first build and would like to know if my setup would work! 

-190 kv 6374 motor torque board
- diy electric vesc
- http://www.diyeboard.com/10s3p-lg-18650-lithium-battery-pack-36v-66ah-238wh-p-631.html

My main issue is the battery back found this on from diyeboards that would fit my budget. Do I need a bms for my setup? Trying to keep my build simple and easy since im new to this. Trying to avoid soldering. I need to go at least 10 miles and around 25mph. Im 170lb.

Another battery option would be 2 5s 8000mAh 30c lipo from hobby king  would that be better? 

Thank you! Any advice is appreciated!
```

---
## \#2 Posted by: myreala Posted at: 2018-03-22T00:50:02.698Z Reads: 143

```
[quote="JULMTL, post:1, topic:49790"]
Do I need a bms for my setup?
[/quote]

That pack has a charge only BMS inside. You just need to limit discharge value in VESC. I think max discharge for that pack is probably 30A, which is not much.

The DIY pack is 6.6 Ah but  2 5s 8000mAh 30c would be 8 Ah. The lipos do out perform that pack in both discharge current and capacity. You just need to figure out the dimensions, and which one works better for you.

You can also use lipo's with a BMS to avoid using a balance charger.
```

---
## \#3 Posted by: JULMTL Posted at: 2018-03-22T04:50:05.860Z Reads: 118

```
Li-ons seems a lot easier and safer for charging. Will I be able to reach 10miles range and 25mph with that pack? with the 6374 motor and 83mm wheels.

thanks :)
```

---
## \#4 Posted by: myreala Posted at: 2018-03-22T04:57:13.221Z Reads: 117

```
Yes, you'll get about 13 Miles on that pack and 25Mph on 83mm wheels if you use 15/40 gear ratio.
 http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":40,"wheel-size":83}|
```

---
## \#5 Posted by: myreala Posted at: 2018-03-22T05:49:57.423Z Reads: 108

```
My bad that was no load speed, to get 25 mph, you need 15/36 pulley, and 90 mm Wheels. 

http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":90}|
```

---

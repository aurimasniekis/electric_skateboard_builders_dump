# Wheel torque, motor torque, gear ratios. Am I doing this right?

### Replies: 15 Views: 1107

## \#1 Posted by: lennarn Posted at: 2018-06-22T21:17:31.058Z Reads: 233

```
My esk8 build plan/BOM:

I'm planning to build a single motor belt driven board to get me up steep hills and go thrillingly fast. I weigh around 85 kg but I want to support some extra heavy users or luggage. This is going to be a sort of stream-of-consciousness type writing down my thoughts post and I need some advice telling me if I'm doing it right, if my math is off, etc.Here goes!

I found a few 4000W motors that seem appropriately powerful without breaking the bank:

motor: aps 6384s £90 (I want sensored motors so I can use FOC to start from standstill and increase efficiency)
130kv: 
https://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-130kv-4000w/
200kv: 
https://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-200kv-4000w/

I want to use a 12 cell LiPo pack (12S) to have a lot of power, so I'm operating at 44.4v nominal:

130kv*44.4v=5772rpm
200kv*44.4v=8880rpm

Since I want to use the ABEC11 107mm flywheel, it was recommended to use a 44T wheel pulley (can't find the source for this statement). I am definitely not decided on gear ratio.

Pulleys: HTD3, 15mm belt, 16T/44T 
gear ratio 1:2.75
https://www.beltingonline.com/16-tooth-htd3-pulley-16-3m-15f-7737?zenid=089bs39h0ps2hqt2jdo4d4cc24
https://www.beltingonline.com/44-tooth-htd3-pulley-44-3m-15f-7749?zenid=089bs39h0ps2hqt2jdo4d4cc24

Driven rpm at this ratio:
_5772rpm/2.75 = 2099_
_8880rpm/2.75 = 3229_

Circumference of 107mm wheel: 336.15mm

Speed calculations:
_130kv:_
_2099 rpm * 336.15mm = 705578,85mm/min_
_v/60000 = 11,76 m/s = 42kph_

_200kv:_
_3229 rpm * 336.15 mm = 1085461,965mm/min_
_v/60000 = 18,1 m/s = 65kph_

**How much torque do I need from the motor ??**
Torque T = Fr, F = ma
Worst case scenario mass 120 kg
Desired acceleration 0-10 m/s in 5s (arbitrary numbers here)
_F = 120 kg * 2 m/s^2 = 240N_
_r = 107/2 = 53 mm = 0.053 m_
_T = Fr = 240N * 0.053m = 12.72Nm_

For the 130kv motor, max torque = 5.8Nm (according to sales page). **Does this mean I need a gear ratio such that: 13Nm/5.8Nm = 2,24 ?** If that is the case I should have enough wheel torque with this motor given a ratio of 2.75 which should give me a max wheel torque of 15,95 Nm.

For the 200kv motor, max torque is listed as 3.8Nm.
13/3.8 = 3,42: Seems like I'd need more of an unconventional gear ratio to make it work with this motor.

**Is my math completely bonkers? What haven't I thought of that is absolutely critical?**
I'll probably make another post later in the electrical category for the rest of the stuff, with ESC, battery &c.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-22T22:20:10.361Z Reads: 199

```
I doubt you need 13Nm for a board to move, in comparison I have a single drive board with a 190kV 6364 motor on 10s and a 2:1 gear ratio on 83mm wheels. I doubt the motor would make more than 2.5Nm so times that by my gear ratio and I would only have 5Nm at the wheel. This board is pretty powerful and takes me up every hill I’ve come to so far, although I am only 60kg. Top speed is about 40km/h
```

---
## \#3 Posted by: Jedi Posted at: 2018-06-22T22:33:35.621Z Reads: 195

```
You may want to use 5m pulleys instead, much easier to find. 

I wouldn't waste too much time doing the math. Any motor 160-200kv is proven to be the sweet spot.
```

---
## \#4 Posted by: moon Posted at: 2018-06-22T22:44:47.407Z Reads: 189

```
Yeah theres not much use stressing about the math, the motors you are using aren't unorthodox 

Maybe you can use this to help

http://calc.esk8.today/
```

---
## \#5 Posted by: lennarn Posted at: 2018-06-23T13:18:54.453Z Reads: 167

```
Thanks for giving me some realistic numbers to compare with! I guess my tendency is to over engineer things rather than building exactly to meet demands.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-06-23T13:19:49.414Z Reads: 158

```
Having a look at other builds will also give you a good idea of what sort of set up you will need
```

---
## \#7 Posted by: lennarn Posted at: 2018-06-23T13:24:06.626Z Reads: 152

```
I've been looking at a few builds but I haven't come across any that give exact numbers for torque.
```

---
## \#8 Posted by: professor_shartsis Posted at: 2018-06-23T15:01:15.246Z Reads: 151

```
[quote="lennarn, post:7, topic:59778, full:true"]
I’ve been looking at a few builds but I haven’t come across any that give exact numbers for torque.
[/quote]

for torque in newton meters per motor amp:

60 / (2 * pi * kv) = torque newton meter per motor amp = KT

then multiply the KT times your motor current limit to approximate motor torque in newton meters for low speeds or roughly KT times the battery current limit to approximate torque for high rpms.

next multiply the motor torque times the gear reduction ratio for wheel torque.

wheel thrust comes from relationship between the wheel torque and wheel diameter-- 

(wheel torque in newton meters * 1000mm) / ((1/2) * wheel diameter in mm) = wheel thrust in newtons per motor

then multiply the wheel thrust times the number of motors for vehicle thrust.

“max torque” in newton meters recommended by the manufacturer divided by the KT gives you the maximum motor current that they recommend to prevent overheating...
```

---
## \#9 Posted by: Craftycarpenter Posted at: 2018-08-19T15:23:06.561Z Reads: 124

```
Hopefully someone can help me out with my 1st build!
I have a 245kv aerodrive motor, 10s lipo, using hk sk8 esc/vesc, 12t motor pulley 40t wheel pulley with 83mm wheels! Ran like a dream, truck loads of power and more than enough torque to get me up hills!
I've just swapped the wheels over for 110mm rough stuff wheels and a 36t wheel pulley and the toque has all but gone! :( seriously struggles up hill now!
I made the newbie mistake of glueing on the 12t motor pulley(aerodrive motor has cylindrical shaft) what can I do to get the torque back? ![IMG_7641|375x500](upload://aiNnxcWQ5ikve5FvcJeIV3sdEs1.JPG)
```

---
## \#10 Posted by: professor_shartsis Posted at: 2018-08-19T16:15:38.430Z Reads: 109

```
[quote="Craftycarpenter, post:9, topic:59778"]
I have a 245kv aerodrive motor, 10s lipo, using hk sk8 esc/vesc, 12t motor pulley **40t wheel pulley with 83mm wheels**! Ran like a dream, truck loads of power and more than enough torque to get me up hills!
I’ve just swapped the wheels over for **110mm rough stuff wheels and a 36t wheel pulley** and the toque has all but gone! :frowning: seriously struggles up hill now!
I made the newbie mistake of glueing on the 12t motor pulley(aerodrive motor has cylindrical shaft) **what can I do to get the torque back?**
[/quote]


you need a ~54t wheel pulley to have roughly the same thrust with the 110mm wheel as you had before with the 83mm 40t wheel (4.5:1 gear ratio is needed).

take a look at the green line, bottom left chart (vehicle thrust in pounds) -- 83mm @ 40t/12t vs 110m @ 36t/12t vs 110mm @ 54t/12t:

https://image.ibb.co/huqBoK/83mm_vs_110mm.gif
```

---
## \#11 Posted by: Jmding Posted at: 2018-08-19T16:25:30.714Z Reads: 104

```
Pick a top speed and back out a gear ratio from there. That way you will maximize the torque available from your drive train. The 200 kv motor will be more efficient and more powerful than the 160 kv motor because the windings are thicker and there are fewer turns, you can make up for the extra speed with mechanical gearing. That said, careful with 12s 200 kv combo, as best practice with VESC 4 is to keep it at or under 60k erpm. Also, the higher kv setup might jump into ground clearance issues depending on your pulley setup. Also, availability of larger wheel pulleys is spotty, so you may have to 3d print

I haven't run the numbers but I suspect that If you are running a pair of 63xx motors, and keep top speed below 35 mph, you will have more than enough torque for any situation
```

---
## \#12 Posted by: professor_shartsis Posted at: 2018-08-19T17:51:14.831Z Reads: 95

```
& another option apart from changing to a 54t wheel pulley would be to add a second motor & keep the 36t wheel pulley... this option gives more peak thrust, more top speed and more efficiency at constant speed than you had previously with the single drive 83mm 40t wheel option.
```

---
## \#13 Posted by: Craftycarpenter Posted at: 2018-08-20T04:40:58.247Z Reads: 89

```
Thanks for the info dudes! 
I've had a brief search for 54t wheel pulley not seen any as yet. 
I'm running a single motor at present, the motor is too long to fit 2 on these caliber 2 trucks unless it's possible to mount them in opposite directions (one in front of the wheel one behind) I appreciate this wouldn't really look very ![IMG_7639|666x500](upload://vNvyfvG3qJzYrJNCj6ZdblLAXJ7.JPG)nice!
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-08-20T14:01:29.235Z Reads: 75

```
[quote="Craftycarpenter, post:13, topic:59778"]
Thanks for the info dudes!
I’ve had a brief search for 54t wheel pulley not seen any as yet.
I’m running a single motor at present, **the motor is too long to fit 2 on these caliber 2 trucks** unless it’s possible to mount them in opposite directions (one in front of the wheel one behind) I appreciate this wouldn’t really look very
[/quote]


@Craftycarpenter have you considered mounting one on the front truck and one on the rear truck?
```

---
## \#15 Posted by: Jmding Posted at: 2018-08-20T15:16:53.194Z Reads: 73

```
You'll have to make your own 56t pulley. There's no other source. But the files are online so you should be able to 3d print one fairly easily if you have access to a printer.
```

---

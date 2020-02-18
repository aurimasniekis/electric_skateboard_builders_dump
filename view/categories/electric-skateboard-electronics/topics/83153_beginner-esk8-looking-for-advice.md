# Beginner ESK8 Looking For Advice

### Replies: 33 Views: 716

## \#1 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:15:28.288Z Reads: 146

```
Hi All,

Bit of background information for you all. I have primarily been involved with mechanical engineering throughout my career and have little electrical knowledge. After many months of looking at Boosted Boards I decided I will challenge myself to make a DIY ESK8. I have been looking at a variety of components but have become lost in all the numbers and letters. Below I have summarised the components I think suit what I want and have also listed some questions I have regarding my build. Please note I am from the UK and parts seem to be hard to get hold of (unless I am looking the wrong place). I would like this board to have more torque than speed. 25mph is more than enough for myself but its getting up hills that I need. All advice regarding these issues or potential improvements will be appreciated :grinning:

* My current chosen battery setup is 2 x Turnigy 5000mAh 5S 30C connected in series. See link below:
* https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack-xt-90.html

* My current chosen dual motor setup is 2 x Turnigy Aerodrome SK3 6374 192KV motor. See link below:
* https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

* Other useful information is that I would like to use the Orangutang 80mm Kegel wheels within my setup.

Now, time for the questions!

Firstly, I need a VESC. I have no idea what VESC to look for with my chosen battery and motor setup. Any recommendations? Hobby King sell a Turnigy SK8-ESC 4.12. Is this any good? See link below:
https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html

Secondly, I want an inline fuse to protect my VESC as I know they cost a considerable amount. With my motor and battery setup what size fuse would be ideal?

Thirdly, I don't know what gear ratio would be wise for my setup? I see on the market they have a variety of gear ratios but don't really understand how they directly affect my setup. If anyone could enlighten me that would be brilliant!

I would appreciate all recommendations! If my battery and motor selection is not amazing please let me know :grinning:

Thanks,
Connor
```

---
## \#2 Posted by: Benjamin899 Posted at: 2019-02-04T17:23:38.436Z Reads: 126

```
Search for Calculator and you will find what gearing you desire. But the diameter of the kegels are also important, so that your wheel pulley has enough space to the ground.
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-02-04T17:24:46.957Z Reads: 120

```
Generally we don't use that ESC...lots of people don't like it.  Try a Torque Boards 4.12 since it's the same price but we'll regarded

Look up fuses that have high voltage (50V or higher) and high amperage (80A).  Anything that can be replaced is preferable
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-02-04T17:26:53.458Z Reads: 110

```
Use this and fix the numbers

https://calc.3dservisas.eu/?Tc7BCsIwEATQf8m5SBJbq17T0pMSENq79RDB0kCP4r93Z9aKt7e7kyFvcw_JnM3rmWdTyHCVYb-rxUu4iZ0no7CkAgLWWg4NJlepkfG6Z6cTZnTgnv_e5Yitp-IWbDRAYnkgf0VjCt83Y2pFR0v2_CI8bfeJ3665izNckqivnEa5Bh_DIjyR3QW91IA72er5swI=
```

---
## \#5 Posted by: Blitz Posted at: 2019-02-04T17:29:17.582Z Reads: 99

```

Plain and simple.

http://calc.esk8.it/
```

---
## \#6 Posted by: Andy87 Posted at: 2019-02-04T17:29:21.179Z Reads: 99

```
Here is the calculator 
https://calc.3dservisas.eu/?Pc8xD8IgEAXg_8JszFGgVVc0ThoSE7srQ00kJelo_O_ee6jbd8fdA17mFiezM89Hnc1Ki7MWbj2ol3hRW0cmpaciBkSExR6VDc2Y6VqfmVZZkdEDmAxtryZ0Oyr9xCgXSDR78h90n3hOHVQbIa9Y93CJ36TCZw_spRn2JH7Q7i-RbQzncQGZlo8nuHHEOBYzbtuKeX8A

If speed is not your goal I would go with a lower kV like 150-190.
The sk3 are unsensored motors. Pretty solid, but you will need a small push from stand still to take off. If you don’t mind than it’s ok, if no, better get sensored. If you want to stick with hobbyking get the sk8 motors.

I would have a look at the graphen lipos, they more expensive, but also perform better and hold more charge cycles.

With those vescs you need to set your bat max current below 35a to don’t overheat them.
I would have a look for used focboxes instead.
There also other oportunities but for this we need to know how much you want to spend on the vescs.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-02-04T17:32:22.944Z Reads: 99

```
[quote="ZachTetra, post:3, topic:83153"]
200A or higher
[/quote]

That’s way too high...
For this board 80a is more than enough.

The right fuses can be found on mouser
https://www.mouser.de/Circuit-Protection/Fuses/Automotive-Fuses/_/N-ba8b5?P=1ylo5uuZ1z0z4z3
```

---
## \#8 Posted by: Arzamenable Posted at: 2019-02-04T17:36:24.581Z Reads: 98

```
The flipsky vesc 4.20 is pretty good and small form factor. It’s a dual controller so no canbus wires to fool with. 

It runs FOC well at your voltage, 10s. Some might chime in and say 6374 motors will demand more amps and a bigger controller would be better. 

6369s and shorter 63mm motor cans might also be good for you unless you weigh more than 200lbs.
```

---
## \#9 Posted by: Andy87 Posted at: 2019-02-04T17:38:43.279Z Reads: 97

```
[quote="Arzamenable, post:8, topic:83153"]
flipsky vesc 4.20
[/quote]

Let’s add a „plus“ to it 😜
The Flipsky vesc 4.20 dual plus seem to be way more reliable than the dual 4.20 and there is no big price difference.
```

---
## \#10 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:41:39.189Z Reads: 94

```
Perhaps a motor such as the one in the link below:
https://hobbyking.com/en_us/turnigy-sk8-6364-190kv-sensored-brushless-motor-14p.html

Just don't know how reliable the SK8 ones are?

Any particular model of FOCBOX or are they all the same?
```

---
## \#11 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:43:37.912Z Reads: 86

```
Makes sense to buy one VESC instead of two! I guess this works with my proposed motors and battery?
```

---
## \#12 Posted by: Arzamenable Posted at: 2019-02-04T17:43:50.750Z Reads: 85

```
![image|666x500](upload://x6qIcJNiQ1WuKePu1xVWGEygaih.jpeg) 

I have the 150kv version. Nice motor, but wide. Might be tough to fit duals in on a narrow truck.
```

---
## \#13 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:44:18.707Z Reads: 84

```
80A in line fuse?
```

---
## \#14 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:45:10.039Z Reads: 88

```
Don't think I could put both motors next to each other with my trucks. Was planning to mount one like yours and the other on the underside of the board.
```

---
## \#15 Posted by: Arzamenable Posted at: 2019-02-04T17:48:15.043Z Reads: 95

```


It’s doable, but close. 

[quote="dareno, post:25, topic:71607"]
[![new%20build%20007|355x266](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/b/f/bfa40880e52eb81680a4249f1e3f1e55106c1541_1_666x500.JPG)
new build 007.JPG4032x3024 2.13 MB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/f/bfa40880e52eb81680a4249f1e3f1e55106c1541.JPG)

Not sure if this will help but I measured it again with the tb mounts and its actually 178mm between mounts with little or no clearance between the motors as you can see. If you can achieve that distance then the motors will work. Thats with the mounts pushed as far as I could without losing enough axle for the wheels with 15mm belts. Tight as a ducks arse it
[/quote]
```

---
## \#16 Posted by: Andy87 Posted at: 2019-02-04T17:50:10.003Z Reads: 92

```
Yap the motors are the right ones.
Maybe go with 149kV version.

I can’t speak out of personal experience, but from what I read here people had some issues in the beginning with the sk8 but lately they seem to be solid.
Sk3 and sk8 are longer than the motor size point out, so have a look in the specs what’s the real length so that you can fit it on your trucks.

If you not fixed to hobbyking than maytech sealed and unsealed are a very good choice for solid motors. 
@okp sell the sealed version 6374 in 150kV or the 6355 in 190kV
https://www.unikboards.com/en/boutique/moteur-skateboard-electrique-6374/
He might also have some focboxes left for sale.
```

---
## \#17 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:51:21.780Z Reads: 79

```
Why 149KV instead of 190KV?
```

---
## \#18 Posted by: ConnorMalins08 Posted at: 2019-02-04T17:52:36.831Z Reads: 81

```
Does look good though. What KV rating are they?
```

---
## \#19 Posted by: Andy87 Posted at: 2019-02-04T17:53:31.380Z Reads: 82

```
If you go with the Flipsky dual 4.20 plus than 80a is more than enough.
You can have a look on the data sheet in mouser.
Those are slow blow fuses, I can’t say you exactly but the 80a fuse can handle 100-120a for more than 10s if I remember right.
So that should be enough.
I use the 100a on my mountain boards and that is pretty good there.
```

---
## \#20 Posted by: Andy87 Posted at: 2019-02-04T17:54:11.906Z Reads: 83

```
Lower kV is higher torque but less top speed.
```

---
## \#21 Posted by: Arzamenable Posted at: 2019-02-04T17:55:37.927Z Reads: 79

```
https://alienpowersystem.com/product-category/e-board-kits/

These guys are in the UK I think. If I ever needed a crazy custom motor, they are the folks I’d buy from. 

You are probably looking at 15 tooth motor pulleys and 32 tooth wheel pulleys. 80mm wheels are fairly small. These ratios are pretty close to what evolve uses.
```

---
## \#22 Posted by: Arzamenable Posted at: 2019-02-04T18:01:13.865Z Reads: 77

```
I second @Andy87 note on both the kv rating and motor vendor. Unikboards is solid. 

I got 149kv for a off-road build that never happened. 170kv is a nice balance. 

I have a 200kv 4wd (6369) that still has enough torque to break 12mm belts if Starts are too aggressive.
```

---
## \#23 Posted by: ConnorMalins08 Posted at: 2019-02-04T18:05:24.393Z Reads: 76

```
Is a 170KV dual motor setup, Flipsky 4.20 dual and two turnigy 5000mah 5s 30C batteries in series an ideal configuration?
```

---
## \#24 Posted by: Arzamenable Posted at: 2019-02-04T18:15:43.671Z Reads: 77

```
![image|506x499](upload://oauGuUGqDltLehEdVft25ZPZsGl.jpeg) 

This is running a flipsky 4.20, smaller 5060 motors at 150kv motors (stock evolve) running at 40a battery max each (total 80amps from battery).

It is punchy and fun, but isn’t going to win any races, tops out around low 20s. 

The battery is 10s5p li-ion cells. I’ve started using lipo on raceboards. They have been disappointing for distance riding. 

The mechanics you are leaning toward seem reasonable/workable. What are your energy requirements? Are lipos new to you or are you an RC guy with the background?
```

---
## \#25 Posted by: ConnorMalins08 Posted at: 2019-02-04T19:39:51.386Z Reads: 65

```
Everything is new to me! I just want a board that is has a load of torque with a top speed of around 25mph. I'm using it to get to and from work. There are a few hills along the way so that's where the torque comes in but who doesn't like speed :)
```

---
## \#26 Posted by: mynamesmatt Posted at: 2019-02-04T22:22:31.198Z Reads: 66

```
the sk8 6374's are great motors. just a shame they're so fucking long. dual sk3 6374's will fit on tb218s but the sk8 ones will be a very very tight squeeze. with my mounts it wouldn't fit so i used the FatBoy 230mm hangar instead. left me with a bit of leeway
![20190201_222136|374x500](upload://1a5mJx7ZUulIEKdOq0rYUu25CoY.jpeg)
```

---
## \#27 Posted by: ConnorMalins08 Posted at: 2019-02-05T15:05:07.201Z Reads: 63

```
That's a nice setup, what gearing and size wheels do you have?
```

---
## \#28 Posted by: mynamesmatt Posted at: 2019-02-05T21:36:06.727Z Reads: 54

```
at the moment they're 107s on 16/36 but I'll be changing to 40t soon
```

---
## \#29 Posted by: ConnorMalins08 Posted at: 2019-02-06T13:22:27.333Z Reads: 43

```
Hi All,

Following your advice I put together a little schematic detailing component specs and configuration. Let me know what you think! What could be better and why?

Not sure whether to have 83mm or 110mm wheels? Done the ESK8 calculation and it seems the board won't have a very high top speed but I assume it will have plenty of torque.![ESK8%20Wiring%20Diagram|690x429](upload://lEXn3m5glmM9kfInoTTiUDwwgM1.jpeg)
```

---
## \#30 Posted by: Mich21050 Posted at: 2019-02-06T13:24:11.402Z Reads: 44

```
Normally you connect your loop key on the positive side. :slight_smile:
Otherwise it looks good.
```

---
## \#31 Posted by: dg798 Posted at: 2019-02-06T14:10:50.357Z Reads: 42

```
Also don’t forget about charging the batteries. Are you gonna balance charge them or use a bms?
```

---
## \#32 Posted by: atenner Posted at: 2019-02-06T14:57:08.629Z Reads: 41

```
if you are still looking for wheels and pulleys for you build, I’ll leave this here 

https://www.electric-skateboard.builders/t/for-sale-htd5m-wheel-motor-pulley-s-and-90mm-wheels/83131

I’m in the UK too
```

---
## \#33 Posted by: Arzamenable Posted at: 2019-02-06T17:59:44.307Z Reads: 34

```
I think you should go for bigger wheels if they are both available to you. I’ve rarely thought to myself, “I seem to be floating over these cracks on the road too easily, maybe smaller urethane might liven things up”.  Nice schematic.
```

---

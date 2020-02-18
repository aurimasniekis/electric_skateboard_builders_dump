# Finalizing a Build

### Replies: 18 Views: 451

## \#1 Posted by: KeivanM Posted at: 2018-08-10T14:26:35.406Z Reads: 172

```
Hello Guys, I am posting on here because I am about to finalize a build buying wise and I want to make sure I have all the right parts before starting to build. Also keep note I am 17 years old and the point of this board is SPEEEEDDDD


So far: I have:
-Deck from Ebay
-Deck hardware from ebay
-Deck Griptape from ebay
-97mm Wheels (ABEC) from ebay (I might buy some 107mm if I have some money left)
-[2x Hobby King 192kv 6347 Motor SK3](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us)
-[2x Drive Wheel Pulley 36T, 12mm](products/36t-abec11-drive-wheel-pulley-only)
-[2.4 Ghz Remote & Reciever](collections/remote-controller/products/torqueboards-2-4ghz-mini-remote-controller)
[Torque Boards 218mm trucks](products/torqueboards-218mm-trucks)
-[2x FOC BOX](https://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/)
-2x Motor Mounts from marcmt88@hotmail.com
-20T HTD5 15mm Motor Pulley from DIYELECTRICSKATEBOARD
-[12s4p Battery with Enclosure ](products/electric-skateboard-battery-epower-pack-12s4p?variant=1307453325335)


My questions now are:

1.Should I buy a 18T 12mm Motor Pulley instead?
2.What length and width Pulley Timing Belt should I purchase if I stay with what I have/ or change to the 18t 12mm?
3.Do I need to buy [this1 ](products/male-to-male-servo-connector?variant=712555003927) [this2](products/dual-esc-xt90-parallel-connector?variant=712413216791) or [this3](products/torque-esc-can-bus-connector?variant=712406925335) ?
4. Am I missing anything? or logistics wise is this wrong?

Any input will be very very appreciated thank you so much in advance!!!!! :smile:
```

---
## \#2 Posted by: Colson003 Posted at: 2018-08-10T14:49:31.890Z Reads: 146

```
1. See how you like the 20t pulley first
2. Use this: https://www.bbman.com/belt-length-calculator/
3. You need the first and the third. If you buy the xt90 parallel connector you’ll need to cut the xt60 connector from the 2x Focbox and solder on an xt90 to both of them.
```

---
## \#3 Posted by: KeivanM Posted at: 2018-08-10T15:35:20.567Z Reads: 122

```
That website doesn’t give me a value when I put all the info in
```

---
## \#4 Posted by: KeivanM Posted at: 2018-08-11T16:16:37.757Z Reads: 98

```
How do I use that calculator and what do I put for that last value?? Does anyone know what belt length I need, I know I need a 12mm HTD 5
```

---
## \#5 Posted by: Colson003 Posted at: 2018-08-11T16:17:55.341Z Reads: 92

```
The center to center distance? You’ll have to ask @marcmt88 he should know what belt length you need
```

---
## \#6 Posted by: KeivanM Posted at: 2018-08-11T16:24:14.911Z Reads: 91

```
@marcmt88, I bought motor mounts from you a while back, do you know that distance?
```

---
## \#7 Posted by: marcmt88 Posted at: 2018-08-11T19:50:49.511Z Reads: 83

```
Currently away from my shop...let u know by tomorrow.
```

---
## \#8 Posted by: dareno Posted at: 2018-08-11T22:00:55.229Z Reads: 77

```
You shouldn't need the male to male servo lead as the focbox comes with a pre-soldered servo lead.
The can bus cable (item 3) is a must to connect both boxes together. Do your research on canbus connections on here before you set it up though this is very important as you can easily fry your vesc's if its not set up correctly.  
I personally like 15mm belts especially with this much power and have only experienced belt skipping with 12mm although your choice of mount with dual idlers should help in this regard.
This thing is going to fly my friend, according to the esk8 calc you should get over 40mph with this build and that takes some skill to ride.  
I'm just in the process of setting up my 12s 4p and 6374s witth 16/36 so will let you know how that goes to give you an idea of performance you can expect.  Good luck and stay safe
```

---
## \#9 Posted by: pat.speed Posted at: 2018-08-11T22:33:44.158Z Reads: 69

```
Please wear full gear going those speeds, knee pads, helmet and gloves at the very least, elbows and hip gear should also be worn. This is coming from my experience taking a fall at about 50-60km/h with only a helmet, I still have cuts grazes and a potentially fractured finger from about a month ago
```

---
## \#10 Posted by: KeivanM Posted at: 2018-08-11T23:53:19.441Z Reads: 67

```
Okay thank you so much.
```

---
## \#11 Posted by: KeivanM Posted at: 2018-08-11T23:53:43.428Z Reads: 61

```
Okay will do, thank you!
```

---
## \#12 Posted by: mynamesmatt Posted at: 2018-08-11T23:54:46.131Z Reads: 56

```
completely agree with @pat.speed. Also, if you're wanting that high of a gear ratio, I'd be going for a lower kv 6374 (like 150kv or something) this way you'll get a little bit more torque
```

---
## \#13 Posted by: Schulerbible Posted at: 2018-08-12T00:12:04.951Z Reads: 56

```
If an Evolve can handle a gearing ratio of 2:1 (32:16) then he should be fine with 6374s, 192KV and 1.8:1. I got myself two 170 KV just in case but don’t  think there is much of a difference.
```

---
## \#14 Posted by: dareno Posted at: 2018-08-12T00:22:56.122Z Reads: 57

```
So just took out my board with the new battery for a test run.  Very careful test run too as my focboxes are now outside of my enclosure.  Clocked it at 35mph on the flat and it was still climbing and I can attest that the 218 tb trucks get very unstable at that speed with standard bushings.  Gearing is 16/36 on dual 192's sk8's and  12s4p 30q.  Torque was incredible compared to the 10s 3p.  You have to weigh up what you want from the board.  I like to carve and I like power but to get the trucks stable I had to tighten them up too much for any kind of carving and losing that torque is not an option for me but I am a big heavy guy.  
Time to play with bushings and throttle curves oh and the braking too, very nearly did a good impression of superman.  Its actually scaring me a bit :sweat_smile:
```

---
## \#15 Posted by: marcmt88 Posted at: 2018-08-12T03:22:38.454Z Reads: 54

```
Hey Keivan,
You bought the long arm with C-C is ~100mm.
```

---
## \#16 Posted by: KeivanM Posted at: 2018-08-15T05:18:43.946Z Reads: 46

```
Okay thank you.
```

---
## \#17 Posted by: KeivanM Posted at: 2018-08-15T13:45:13.777Z Reads: 39

```
So wait do I need a 345mm belt?
```

---
## \#18 Posted by: marcmt88 Posted at: 2018-08-15T14:39:50.008Z Reads: 30

```
Belt size depends on the pulley ratio of your setup.  Best is to setup your drive system, wrap a string around to measure.
```

---

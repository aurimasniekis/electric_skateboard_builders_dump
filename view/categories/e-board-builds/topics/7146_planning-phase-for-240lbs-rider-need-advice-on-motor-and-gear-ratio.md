# Planning phase for 240lbs rider. Need advice on motor and gear ratio

### Replies: 21 Views: 2174

## \#1 Posted by: gasparrobi Posted at: 2016-08-04T23:18:55.656Z Reads: 153

```
Hello!
I have been reading this thread for a few days and now I'm 80% confident in the specs of my build but I need some advice to choose the right motor and gear ratio. I am 240lbs but I'm in the process of losing weight so hopefully in a few months I will go down to about 200-210. I'm planning to order everything from @torqueboards and esk8.de

Updated plan:

* Single motor setup with torqueboards' kit with 83mm wheels

* 6355 170kv motor

* VESC

* 16T/36T gear ratio

* 10s3p Li-ion battery pack

My calculations:
<img src="/uploads/db1493/original/2X/f/fe3d5082db967b5f2e9622478c8e3c0baf5f7135.png" width="690" height="336">

I would only need about 30-35kp/h speed. Does this setup have enough torque? I'm not planning to go on steep hills at all, mostly flat.
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-04T23:30:56.847Z Reads: 141

```
Single motor at your weight I'd go with a 6374 motor instead. If you want to only go 30-35km/h drop the gearing to 14/36 for increased torque. Make sure you're using at least 12mm pulleys and belts.
```

---
## \#3 Posted by: Pablo_702 Posted at: 2016-08-04T23:34:59.647Z Reads: 139

```
Dexter is good man at torqueboards im a big bones guy mysefl at 200 lbs and recently finished my first build , i haven ridden a different board besides mine but im loving it its been very reliable so far i would say a turnigy sk3 6374 149kv would be a better choice considering the load (240 lbs) im running a single 149kv and this motoris a beast another thing you hae to consider is top speed you are trying to achieve, as with a higher kv motor u can reach higher speeds but less needed torque for our case, wich can be remedy with the righ gearing i did the calculations for my build when i was building it and i think the top speed was 21 or 22 mph wich at first i was like i want to go faster but believe me 20 mph on a longboard its hella fast and also when i was testing my board for the first time i got up to 20 mph really quick and ran out of balls i had a lot of throthle and momentum left i say judging on how much throtle and how quick this thing is close to 30 mph
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-08-04T23:43:04.539Z Reads: 129

```
What gearing are you using @Pablo_702?
```

---
## \#5 Posted by: Pablo_702 Posted at: 2016-08-04T23:46:52.736Z Reads: 124

```
16/36 on 83mm @50.4 V
```

---
## \#6 Posted by: gasparrobi Posted at: 2016-08-04T23:49:53.873Z Reads: 124

```
Well, then I just have to find a source which has the 149kv motor in stock :/ I can't find it anywhere but I agree with you, I don't want to go faster than 20mph and more torque would be better for me. 
But when I do the calculation the rpm goes very low. It should be around 7-8000 at 3.6 volts, right? @Pablo_702 

<img src="/uploads/db1493/original/2X/a/a9d00bfc082a1ed0bfc4543513098391d4f4b6d9.png" width="690" height="373">
```

---
## \#7 Posted by: Pablo_702 Posted at: 2016-08-04T23:57:25.740Z Reads: 119

```
on the i dont remeber how to manually do the calculations its in the forum somewhere but yes i remember when i was doing my homework the the erpm were crazy low, have you thought about going 12s? it will be more powerfull and less heat, are u planning to use a vesc?
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-05T00:04:27.154Z Reads: 117

```
@Pablo_702 Here you guys go

http://calc.esk8.it/
```

---
## \#9 Posted by: Pablo_702 Posted at: 2016-08-05T00:13:06.823Z Reads: 118

```
Top Speed
28.58 mph - 46 km/h

22.87 mph - 36.8 km/h

(weighted)

see thats what i got it says 22.87 weighted but im sure its more like the top speed of 28.58 mph maybe if @Michaelinvegas wants to test its final speed hes more than welcome to gps it for science of course
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-05T00:14:46.281Z Reads: 109

```
You can usually get pretty close to max speed as efficiency generally rises the faster you go.
```

---
## \#11 Posted by: gasparrobi Posted at: 2016-08-05T00:19:09.769Z Reads: 109

```
Hm, as this will be my first build I don't know what to expect with a 149kv motor at low rpm. Even with a 12s battery it works way below the recommended 8-9000 rpm. What effect does it have on the vesc, battery or the motor? and how important is it to reach the recommended rpm?
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-05T00:20:06.105Z Reads: 102

```
I don't think you have anything to worry about. Plenty of people run the SK3 149kv at 12s. I think the recommendation is there for efficiency.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-08-05T01:24:49.965Z Reads: 104

```
I'm going 14t ... More than enough torque

And yes...its prob higher since the board isn't at 70-80 efficiency all the time...

Be careful at those speeds bud...something abt eating shit at 20+ mph that just sucks lol
```

---
## \#14 Posted by: Pablo_702 Posted at: 2016-08-05T01:27:50.970Z Reads: 100

```
u down to testing real top speed on mine?
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-08-05T01:28:32.132Z Reads: 101

```
Lol need a flat run
```

---
## \#16 Posted by: Pablo_702 Posted at: 2016-08-05T01:29:12.188Z Reads: 99

```
time and location
```

---
## \#17 Posted by: Jeff Posted at: 2016-08-05T01:37:10.771Z Reads: 99

```
Not sure if you figured everything out yet but my build might give you some insight: http://www.electric-skateboard.builders/t/carbon-python-hi5ber-python-caliber-ii-s-single-6374-hi-output-vesc-12s-lipo/2208

One time I took it up hills at 270lbs (220lbs + 50 lbs in my backpack) and it handled it no problem.
```

---
## \#18 Posted by: gasparrobi Posted at: 2016-08-05T08:30:53.788Z Reads: 91

```
yeah I think I will go for the 170kv option in the end but I'm still doing some research.
```

---
## \#19 Posted by: WeeChumlee Posted at: 2016-08-05T10:51:23.216Z Reads: 93

```
Hi
I am +- 200lbs and use the 6374 170KV motor on 8S.
15T x 44T gearing and 97mm wheels.
Speed is fine for me and it goes up all the hills in my area without a problem.
VESC did get to warm though on steep hills so now use a ESC very similar to TB 12S ESC.
Actually prefer this board to my dual 6355 240KV 8S board with VESCs.
```

---
## \#20 Posted by: gasparrobi Posted at: 2016-08-05T21:11:05.818Z Reads: 82

```
Looks like I will able to source almost everything, the only part missing is a custom 10S3P - 18650 battery pack. Is there anyone in europe who would build it to fit this layout that I have planned here?:
<img src="/uploads/db1493/original/2X/9/996642d9ee5b7c27b94a7bec6a9fee71073793e0.jpg" width="690" height="395">
```

---
## \#21 Posted by: jujet Posted at: 2016-11-01T14:22:45.824Z Reads: 51

```
I'm also interested in this.

How about the enclosures? 

Where are you getting those ?
```

---

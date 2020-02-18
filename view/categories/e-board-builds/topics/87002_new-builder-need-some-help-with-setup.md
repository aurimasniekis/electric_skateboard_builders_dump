# New builder need some help with setup

### Replies: 22 Views: 345

## \#1 Posted by: danzis Posted at: 2019-03-13T00:10:11.159Z Reads: 118

```
hey guys so i looked in this web for days and got so much information and i build myself  setup wich is not the best i know because im choosin not to make a psycho batterypack on the first build .

2 motor : Turnigy Aerodrive SK3 - 6364-245KV Brushless Outrunner Motor

2 battery: ZIPPY Compact 4500mAh 6s 40c Lipo Pack w/XT90

2 ESC:  FVT 2-6S LiPo Battery 120A Waterproof sensored sensorless Brushless Car ESC For 1/8 1/10 RC Car Model 

board: SDS 7-ply Maple Mountain Board, 32 x 8.5-Inch 
or atom 90 mountain board 

controller: HobbyKing® ™HK-GT2B 3CH 2.4GHz Transmitter and Receiver w/Rechargable Li-ion Battery]

and if i forgot somthing let me know !!


i want to know what pullys to use ?

and i want to know if my setup is going to work well? 

about the mount of the motor im not sure wich one will fit?

do i need to connect between the esc's? and if yes so explain how 

how do i connect the controler reciver to work on 2 esc's?

 i know thet i need at least 10 ~12 s but its first build and i want to stars in easy. and in the future if this setup will work i will add another 2 pack of battery and get the 12s power .and a better range.
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-03-13T00:55:02.433Z Reads: 91

```
With 245 kv motors you can't do 12s realistically, if you use standard pulleys and wheel diameter (15:36 and 90mm), you'll max out at 24mph at 6s already

Also those ESCs will only do 6s so you can't upgrade them

Recommendation is either get a real skateboard ESC and battery, or go with what you have and never upgrade it

http://calc.esk8.it/#%7B%22batt-type-lipo%22:1,%22batt-cells%22:6,%22motor-kv%22:245,%22system-efficiency%22:85,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:36,%22wheel-size%22:90%7D%7C
```

---
## \#3 Posted by: brenternet Posted at: 2019-03-13T01:02:02.417Z Reads: 82

```
As a community we need to look in to how these new users are finding information for builds on the forum. Because this is a shit build (no offence OP).

Where did you research this information?
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-03-13T01:16:25.712Z Reads: 79

```
Probs from a YouTube video
```

---
## \#5 Posted by: maxchilton Posted at: 2019-03-13T01:39:17.964Z Reads: 81

```
[quote="brenternet, post:3, topic:87002, full:true"]
As a community we need to look in to how these new users are finding information for builds on the forum. Because this is a shit build (no offence OP).

Where did you research this information?
[/quote]


that's a build list from the early days of esk8... back when we used RC components, made our own mounts and drilled our own wheel pulley.  lol
```

---
## \#6 Posted by: danzis Posted at: 2019-03-13T09:02:12.567Z Reads: 60

```
Actually its all from here never looked in youtube for setup only . And maybe the topic i looked is to old , so you can tell me what esc to use ? @ZachTetra 
And another thing is i dont understand waht is the problem with the battery 
 The idae is to first built the board so go slow and in the future to add battery and making it in parralel and series to get best voltage and mha 12 c and 8000mah
```

---
## \#7 Posted by: BillGordon Posted at: 2019-03-13T09:05:04.456Z Reads: 55

```
That was firmly but delicately handled.
```

---
## \#8 Posted by: ZachTetra Posted at: 2019-03-13T09:05:18.230Z Reads: 54

```
The battery is fine but the RPM/V of the motor is so high you're gonna go faster than a Boosted with the 6s battery

Good options are the Torque ESC from DIY Electric Skateboards, if you use their motor (190kv) you can just plug and play, then do some experimentation later when you're ready
```

---
## \#9 Posted by: danzis Posted at: 2019-03-13T09:09:53.969Z Reads: 53

```
Can you link me to this esc i cant find it , and if i will stay with the same motor i sayed (245kv) it will be a problem ?
```

---
## \#10 Posted by: BillGordon Posted at: 2019-03-13T09:10:15.306Z Reads: 53

```
Don't get defensive, my man. You asked for help and there's some wicked smart folks here (I am not one of them) who will help out. They have already used all the parts you listed and have moved on because much better stuff is available. 

Try not to argue and just learn.
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-03-13T09:13:34.939Z Reads: 49

```
https:///products/torque-esc-bldc-electronic-speed-controller

https:///collections/electric-skateboard-conversion-kit/products/pro1-electric-skateboard-conversion-kit
```

---
## \#12 Posted by: danzis Posted at: 2019-03-13T09:38:58.777Z Reads: 44

```
Ohh ok so the price is double . 
Is there a diffrent esc or its the best option ? 
And it will run the 245kv motor with 6s lipo ?
 and ty zach for replay so fast @ZachTetra
```

---
## \#13 Posted by: meesie Posted at: 2019-03-13T09:49:25.554Z Reads: 42

```
for an electric skateboard the best option is to use a VESC. VESC's are programmable on your PC with lots of safety options and smoother startup control etc. a normal ESC from hobbyking is not as adjustable as the VESC and doesnt have all those safety options (low voltage cutoff and temparature cutoff. important!)

i would recommend you to go for a VESC rather than a normal ESC.
If you're planning to build a mountainboard, you will want to use 12S but with low kv motors like 170KV or maybe even lower. then djust your gearing accordingly.
Also, try to check out other people's  MTB build threads to see what they use.

best of luck with your build!
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-03-13T09:52:03.679Z Reads: 40

```
There is no reliable ESC for skateboards for less than that unless you risk the Chinese ones (please don't)

That motor is too fast, 190-170 kv is what you want
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-03-13T09:56:21.971Z Reads: 38

```
IF you use that motor on a mountain board, the wheels and ratio you want are...
- 14:42 this is the highest ratio you can hope for without expensive custom parts
- 150mm wheels, this is a common tire size and any bigger will make you to fast

You'll top out at 27mph on 6s


More power and lower voltage means lots of amps, your setup will get HOT
```

---
## \#16 Posted by: meesie Posted at: 2019-03-13T09:59:09.906Z Reads: 37

```
he's planning on a mountainboard i believe, zach :slight_smile:
```

---
## \#18 Posted by: danzis Posted at: 2019-03-13T16:49:33.929Z Reads: 29

```
Ok so i looked for the 190 kv sk3 and it seems to be more power and it need a biger battery (more s and more mah) because the motor have more volt so im asking again about the 245 kv ,
its not the best that i can get with the lipo pack that i want? This motor can run-with a 12s lipo pack ? Or its to much for this motor? 
 consider the problem that because im new to this world i dont want to make at first build a lipo parallel and sereis with bms its to much dangerous with the shiity knowledge that i have right now @ZachTetra
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-03-13T17:11:26.725Z Reads: 26

```
You limit power with the ESC, motor and battery should be over spec

245kv will work only at 6s because it's to fast

You can use 4s batteries and go from 4s to 8s and you'd be okay but it wouldn't last long, to many amps

Try these motors maybe

https://flipsky.net/collections/e-skateboard/products/motor-h5045
```

---
## \#20 Posted by: danzis Posted at: 2019-03-13T17:36:53.645Z Reads: 22

```

195kv can work with 6s lipo ?
how much speed do i get from a 195kv motor with the 6s start setup ? 
mybe it will be better motor for me for the upgrade idea.
```

---
## \#21 Posted by: ZachTetra Posted at: 2019-03-13T17:39:16.893Z Reads: 23

```
Use this, it will let you get a rough idea of performance

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:6,%22motor-kv%22:195,%22system-efficiency%22:85,%22motor-pulley-teeth%22:14,%22wheel-pulley-teeth%22:42,%22wheel-size%22:150}|

This one has more detail, use it once you know what you want

https://calc.3dservisas.eu/
```

---
## \#22 Posted by: danzis Posted at: 2019-03-18T17:43:04.037Z Reads: 17

```
HOW IS THIS FOR START?
![ELECTRIC%20MTB|690x388](upload://p1IxYN5JkxpWsLcxZ9ENEUBuXk9.png)
```

---
## \#23 Posted by: Swaight Posted at: 2019-03-18T19:50:07.461Z Reads: 13

```
Hey guys this is my first build and im wondering if anyone could look over this design and tell me if it would work.![1|690x318](upload://2biaRQcATSDNjsZv6X2mzcuEFri.jpeg)
```

---

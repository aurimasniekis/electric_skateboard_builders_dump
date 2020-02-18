# Smallest motor that packs a punch

### Replies: 33 Views: 1109

## \#1 Posted by: DeathByBacon Posted at: 2018-06-21T09:23:34.194Z Reads: 298

```
What's the smallest motor you can use on a single drive build that's capable of carrying 200lbs of load and can still go uphill? Building a light, stealthy, easy to carry, round-the-neighborhood board.
```

---
## \#2 Posted by: b264 Posted at: 2018-06-21T09:25:20.449Z Reads: 301

```
A single 5065 motor at 140kv geared-down at 15:40 or 15:44 and running at 10S on 107mm wheels
```

---
## \#3 Posted by: trampa Posted at: 2018-06-21T10:14:04.683Z Reads: 287

```
uphill is very relative. 10% or 20%....Makes a hughe difference. Also going up hill slow is putting more strain on things. Going uphill fast is a lot more easy to achieve. Brands fool people by posting videos of fast uphill runns. Users think fast and steep hill climbing must be very hard to achieve. Slow and steep is the challenge....

https://vesc-project.com/calculators

6364 or 6374 is quite good for singles. Longer is better, more diameter is better. KV around 140-160.
Housing should not be closed, so you get good airflow.

Frank
```

---
## \#4 Posted by: Blitz Posted at: 2018-06-21T10:27:57.200Z Reads: 261

```
[quote="trampa, post:3, topic:59585"]
going up hill slow is putting more strain on things. Going uphill fast is a lot more easy to achieve
[/quote]

My mind is blown any reading material you can share so that I could understand this concept?

Is this something about gearing?
```

---
## \#5 Posted by: DeathByBacon Posted at: 2018-06-21T10:30:38.584Z Reads: 247

```
Any specific brand of 5065? 107mm wheels might be a bit too big for a stealth build though.
```

---
## \#6 Posted by: Blitz Posted at: 2018-06-21T10:30:49.192Z Reads: 243

```
My single 190kv 2000w 6364 motor on 9s lipos,

can pull me up a steep looking hill at like 30km/h
and it's top speed is a bit over 40 km/h.

Gearing: 90mm wheels 36/15
```

---
## \#7 Posted by: DeathByBacon Posted at: 2018-06-21T10:34:04.342Z Reads: 238

```
I was thinking the 6374 really fits the bill. I was just thinking if there was something smaller that's still up to the task.

I think I understand that bit about going fast uphill and deliberately going slow bit and I agree.
```

---
## \#8 Posted by: trampa Posted at: 2018-06-21T10:34:50.587Z Reads: 228

```
E-Motors are efficient at high RPM, but inefficient at low RPM and high torque output. 
Going up a hill slow, you will push a lot of Amps to generate the torque you need and you travel up the hill for a longer period of time, since you are slower.
```

---
## \#9 Posted by: DeathByBacon Posted at: 2018-06-21T10:35:36.023Z Reads: 226

```
How about braking downhill, how does it perform? What are your ESC settings for this kind of setup?
```

---
## \#10 Posted by: Blitz Posted at: 2018-06-21T10:37:48.692Z Reads: 231

```
Braking downhill, Kinda sucks, I think i got it on -40a 
But I get belt skips on a 15mm kit.

I can go up this hill at 33km/h easily if I catch a bit of speed before hitting the hill.
![Screenshot%20from%20201t8-06-21%2011-33-35|631x500](upload://nVx8rzLXmrlpEQuodq0p8MzdjxO.png)![Screenshot%20from%202018-06-21%2011-32-49|561x499](upload://jglVv2gESdThmyga50gXxJjUWjJ.png)
```

---
## \#11 Posted by: b264 Posted at: 2018-06-21T10:37:54.640Z Reads: 220

```
On smaller wheels, lower the gear ratio like 15:36 or 15:40 instead of 15:40 or 15:44
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2018-06-21T10:39:26.059Z Reads: 214

```
Going fast uphill stresses the battery more, as you're pulling higher power, but is easier on the motor and motor controller, as they don't have to perform at high power (current=torque) as long.

Going slow uphill inverses this relation, low battery power, but ends up heating your motor and motor controller more, as they have to sustain high current for longer.
```

---
## \#13 Posted by: trampa Posted at: 2018-06-21T10:54:11.961Z Reads: 211

```
But battery output should match the power of the boards motor anyway + you can define the max battery drain in VESC-Tool. What usually creates temp cutouts on hills is the motor heating up due to high Amp flow in the spools. Small commuter boards usually have smaller batteries, which is an issue for up hill performance, top speed performance and the brakes. Scaling down the battery creates issues....

It's quite amazing what hills you can climb using a single 6364 or 6374 motor, as long as you can go fast enough up the hill and when the battery has enough voltage and P count.
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2018-06-21T11:14:41.246Z Reads: 205

```
[quote="trampa, post:13, topic:59585"]
battery output should match the power of the boards motor anyway
[/quote]

Yes, but battery current and motor current can still be very different between them.

For example difference between battery and motor current:
High speed: Power 1000W, battery voltage 40V -> battery current 25A, motor operating at higher RPMs might see 30V -> 33.3A
low speed: Power 200W, battery voltage 40V -> battery current 5A, motor operating at low RPMs might see 6V -> 33.3A

In both cases the motor is producing the same torque, because same motor currents, which let's say is the torque needed to not gain or loose speed, but power use is very different between the high and low speed examples. High speed/ low time uphill would have battery hotter and motor controller + motor cooler, whereas the low speed/ high time would see the battery cooler and motor controller and motor hotter.
```

---
## \#15 Posted by: trampa Posted at: 2018-06-21T11:29:28.165Z Reads: 195

```
Correct Mr Muffin! I want to work on a nice diagram showing how things actually are linked together.
This is the part most people don't understand when setting up their boards. A good diagram would help.

If you want to climb hills, you probably also ride down those hills and you want to use the brakes in that case. So you are aiming at a battery that can cope with the Amp flow. And this is the issue when building small and light boards. The battery is usually not capable enough and overstrained when braking for a longer period of time.

https://www.electric-skateboard.builders/t/vesc-how-to-get-better-brakes/59461/23?u=trampa
```

---
## \#16 Posted by: SimosMCmuffin Posted at: 2018-06-21T11:37:39.487Z Reads: 186

```
[quote="trampa, post:15, topic:59585"]
If you want to climb hills, you probably also ride down those hills and you want to use the brakes in that case. So you are aiming at a battery that can cope with the Amp flow.
[/quote]

Using different battery max vs. motor max settings also allows you to use more acceleration or brake at lower speeds, because you can crank/regen higher motor currents, while still being under the power limit. Battery is always going to be more stressed at higher speeds, unless you limit the battery max currents, which the VESC then compensates by decreasing motor currents at higher speeds.
```

---
## \#17 Posted by: PDXroses Posted at: 2018-06-24T18:49:24.516Z Reads: 152

```
@trampa, I have a 10s3p and two motors. After a km of an uphill climb averaging ~10%, the board gets weak and then just stops. After I let it rest for a few minutes, it’s able to climb the hill again, but for a shorter distance this time. Is there something in the dual VESCs that I can change? Do you have any insights you can share?  Thanks.
```

---
## \#18 Posted by: trampa Posted at: 2018-06-25T07:18:14.984Z Reads: 141

```
What kind of motor, gearing, wheel diameter, ESC? Without those infos nobody can help.
```

---
## \#19 Posted by: Cobber Posted at: 2018-06-25T07:41:36.706Z Reads: 141

```
The smallest motor that packs a punch (for weight) will be something with a long stator with a small diameter. For the weight a 4092 inrunner has big torque. Either need a custom wind or a big gear reduction. @MoeStooge has made it work a handful of times so you just need to be creative or order a custom from Alien.
```

---
## \#20 Posted by: MoeStooge Posted at: 2018-06-25T14:06:59.471Z Reads: 130

```
This little fella (4092) makes 4200w. 8:1 gearing on 8s makes 34mph on 70mm wheels. Have used this setup to pull a 190lb friend on a DH board back up the hill multiple times. Honestly this single will rival many dual motor setups in acceleration and speed. ![Screenshot_20180604-082522|281x500](upload://l7wMqTSERxueqRlZ943vw0sOobv.jpg) ![IMG_20180624_165922296|690x388](upload://3lPw7xOhOrX9N6AN1V6pk0jpMWh.jpg) ![IMG_20180624_165928083|690x388](upload://4tzUVBbgETf0MHTJrjGQrcxetK3.jpg) ![IMG_20180623_130202620_HDR|690x388](upload://apZKTeIOAg01BQyKe7tNd9Myhdg.jpg)
```

---
## \#21 Posted by: Cobber Posted at: 2018-06-25T14:12:07.617Z Reads: 120

```
looks badass MoeBro :dark_sunglasses:
```

---
## \#22 Posted by: Blitz Posted at: 2018-06-25T14:19:42.491Z Reads: 116

```

and what esc did you pair with it and whats the breaking feel like, choppy, loss of traction when breaking hard?
```

---
## \#23 Posted by: MoeStooge Posted at: 2018-06-25T14:30:32.473Z Reads: 113

```
Toro 200a beast. Braking is decent, it's front drive. Don't notice tortional twist with the 3-link on accel, decel.  Toe side turns on hard accel does get wheel spin. Drawbacks of a single.
```

---
## \#24 Posted by: Nordle Posted at: 2018-06-25T14:45:04.554Z Reads: 108

```
Haha thats a nice one:) does it make a lot of noise (the small gears i mean)
```

---
## \#25 Posted by: PDXroses Posted at: 2018-06-25T15:20:22.963Z Reads: 107

```
Whoops. Two Alien motors 6355’s, two VESCs connector by canbus, 97mm wheels with 15/38 gearing. This is my second build with the same components, but this one isn’t able to tackle the hills the first one used to. That first one is outa commission so I can’t compare.  Could it be the VESC settings?  I changed the bullet connectors  from 5.5 to 3.0. Can’t be that right?  RC is the same. Batteries are the same Samsung 18650. Belt tension isn’t too tight. I’m still 160lbs. What in the world is causing the board to stall halfway up the hill now when I used to go the full distance?  Thanks for any insights you may have, Frank.
```

---
## \#26 Posted by: Adam0311 Posted at: 2018-06-25T15:31:49.293Z Reads: 109

```
I have a single 6355 170kv motor with 12s2p pack that gives me 8-10 mile range and pushes my 210lbs up hills without difficulties. 15mm belt is critical for our weight on a single. The entire board with free board bindings weighs in at 14lbs. Without the bindings it’s probably about 11lbs. Great for cruising to a bar or restaurant and stuffing the board under a table then riding back home.![image|375x500](upload://lXxph1YMyVOyZZSWwI1Z3Hd5QPI.jpeg)![image|666x500](upload://2BCTw50JSO56KPIMh1wNWWRuX5Z.jpeg)
```

---
## \#27 Posted by: trampa Posted at: 2018-06-25T15:37:25.087Z Reads: 108

```
You have to check the temperature of the motor and VESC. Mobile VESC-Tool with BLE dongle helps to read the temp values while you ride.

3.0mm bullets are to small. 4.0mm is what you want.
```

---
## \#28 Posted by: MoeStooge Posted at: 2018-06-25T18:14:18.559Z Reads: 99

```
Gears are mod.8 (32p). They make less noise than mod 1.5 steel on steel.
```

---
## \#29 Posted by: Cobber Posted at: 2018-06-25T18:33:33.740Z Reads: 95

```
3.0mm bullets are tiny :frowning:
http://www.elektromodellflug.de/oldpage/hochstromst/hochstromstecker.htm
good for maybe 20a cont?
but like frank said, check what is getting hot
```

---
## \#30 Posted by: PDXroses Posted at: 2018-06-25T19:11:10.600Z Reads: 87

```
Frank, Cobber, thanks and you’re right. I poked a bunch a holes in the enclosure and the hill climb is already better. Today is also Cooke (65F).  I misstated the bullets. I have 4.0’s not 3.0’s so I should be ok there.  Now water and dust concerns. Haha.
```

---
## \#31 Posted by: Holyman92 Posted at: 2018-06-25T19:39:22.223Z Reads: 82

```
my 10s5p single rear drive 6374 takes me up a 30%-35% incline doing roughly 5mph the speed stays constant through the climb my gearing is 15/32 w/ 100mm all terrain mbs wheels. 

as a final note, the board can probaby go faster up the hill IF i didnt have to ride a little over 10 miles to get there lol
```

---
## \#32 Posted by: Adam0311 Posted at: 2018-06-25T22:08:10.977Z Reads: 80

```
Swapping to 36t wheel pulley would get you up faster...at the cost of some top end speed.
```

---
## \#33 Posted by: Holyman92 Posted at: 2018-06-25T23:35:00.253Z Reads: 75

```
I don't go up it often anymore it's literally the steepest and probably the only large incline like tht around here, minus the parking garages and what have you
```

---

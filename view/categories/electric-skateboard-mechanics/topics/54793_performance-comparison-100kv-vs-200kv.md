# Performance comparison 100kv vs 200kv

### Replies: 8 Views: 1232

## \#1 Posted by: DeathCookies Posted at: 2018-05-08T11:40:44.997Z Reads: 181

```
We have one battery (44V 200 cont. A) and two Motors (100 and 200kv)

A. If we have one 2:1 (100kv) and one 4:1 (200kv) reduction.
B. if we have the same reduction.

What would be the estimated wh-consumption at 5mph / 15 mph / 35 mph? i dont want exactly numbers i just want to Analyse the relation between These factors.
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-05-08T13:26:11.445Z Reads: 155

```
if the 100kv and 200kv motors are the same size, same copper volume, and the gearing is adjusted for each, and the same electrical wattage and voltage is applied to both, the higher kv produces more mechanical watts for the same electrical watts, or you could say the higher kv can produce the same mechanical power as the lower kv with less copper loss (ohmic heating).

[quote="professor_shartsis, post:136, topic:7246, full:true"]
km is the same:

**100kv - 10 turns - 1 cross section - 0.1ohm**

60/(2 * pi * 100kv)=0.09549296585513720146133 newton meters torque per motor amp

(4v battery - 0v bemf) / 0.1ohm = 40a motor & battery current at 0rpm

4v * 40a = 160w electrical

40a * 0.09549296585513720146133nm/a = 3.819718634205488058453nm

3.819718634205488058453nm / sqrt(160w electrical) = **0.3019752726269222102173km**

**200kv** - **5 turns - 2 cross section - 0.025ohm**

60/(2 * pi * 200kv)=0.04774648292756860073067 newton meters torque per motor amp

(4v battery - 0v bemf) / 0.025 ohm = 160a motor & battery current at 0rpm

4v * 160a = 640w electrical

160a * 0.04774648292756860073067nm/a = 7.639437268410976116907nm

7.639437268410976116907nm / sqrt(640w electrical) = **0.3019752726269222102173km**

^km (torque per square root of watt) is the same

**1:1 gearing - 10mph ground speed**

**100kv** - **10 turns - 1 cross section - 0.1ohm**

1000rpm = 104.719755 radians per second

(11v battery - 10v bemf) / 0.1ohm = 10a motor/battery current

torque per amp: 60/(2 * pi * KV) = 0.095492nm/a

10a * 0.095492nm/a = 0.95492newton meters torque

11v battery * 10a current = 110w electrical

0.95492newton meters torque * 104.719755 radians per second = 99.99w mechanical

copper loss: 10a * 10a * 0.1ohm = 10w

wheel torque at 10mph @ 110w electrical = 0.95492nm * 1 gear reduction = 0.95 newton meters

**summary: 10mph ground speed, 0.95nm wheel torque,** **99.99w mechanical, 110w electrical, 10w copper loss**

**2.150:1 gearing - 10mph ground speed**

**200kv** **- 5 turns - 2 cross section - 0.025ohm**

2150rpm = 225.14747 radians per second

(11v battery - 10.75v bemf) / 0.025ohm = 10a motor/battery current

torque per amp: 60/(2 * pi * KV) = 0.047746nm/a

10a * 0.047746nm/a = 0.47746 newton meters torque

11v battery * 10a current = 110w electrical

0.47746 newton meters torque * 225.14747 radians per second = 107.49w mechanical

copper loss: 10a * 10a * 0.025ohm = 2.5w

wheel torque at 10mph @ 110w electrical = 0.47746nm * 2.15 gear reduction = 1.02 newton meters

**summary: 10mph ground speed**, **1.02nm wheel torque, 107.5w mechanical, 110w electrical, 2.5w copper loss**

^same ground speed, same voltage battery, same battery current and motor current, different gearing & the higher kv appears more efficient… it would seem if the 100kv is at constant speed @ 10mph from the load, with the same ground speed & load the 200kv is still accelerating because there is more torque at the wheel…
[/quote]
```

---
## \#3 Posted by: Acido Posted at: 2018-05-08T13:28:08.868Z Reads: 129

```
electric motors like to spin fast more than pull hard

but the ESCs come in to play here so go with a lower kv
```

---
## \#4 Posted by: DeathCookies Posted at: 2018-05-08T13:45:40.569Z Reads: 124

```
You mean because of ERPM Limit? Focbox does not have this Problem (130k i believe?).

Or did you mean something else?
```

---
## \#5 Posted by: DeathCookies Posted at: 2018-05-08T13:48:46.277Z Reads: 125

```
You were the Person i liked to get an answer from! I just forgot the nick and so i did not tag you in the first place.

I really like your Charts and Knowledge. Where do you get the Charts from?

So i should aim for a 200kv Motor instead of 100kv? What about friction loss due to the different gearing (200kv spins more = more fiction loss) or is it insignificant?
```

---
## \#6 Posted by: professor_shartsis Posted at: 2018-05-08T13:54:11.510Z Reads: 120

```
the actual difference in efficiency between 100kv vs 200kv to me seems slight, but the efficiency does improve the higher and higher the kv goes for the same km assuming the gearing is adjusted.

in my humble opinion adding motors is the real way to improve efficiency.... for example consider 2 motors at 100a motor amp setting or 4 motors at 50a motor amp setting... vehicle performance would be nearly identical, but ohmic heating per motor would be 1/4th wth 4 motors compared to 2 motors. total ohmic heating of all motors combined would be half. same performance with half the loss means more efficiency.
```

---
## \#7 Posted by: DeathCookies Posted at: 2018-05-08T13:59:32.223Z Reads: 111

```
[quote="professor_shartsis, post:6, topic:54793"]
in my humble opinion adding motors is the real way to improve efficiency… for example consider 2 motors at 100a motor amp setting or 4 motors at 50a motor amp setting… vehicle performance would be nearly identical, but ohmic heating per motor would be 1/4th wth 4 motors compared to 2 motors. total ohmic heating of all motors combined would be half. same performance with half the loss means more efficiency.
[/quote]

I am totally with you! Thats the only practical way for better Performance. But sometimes we are nailed to boundaries....

I am Setting up a street carver build. i did not want to make it 4 wheeled only 2 wheeled (Less costs/maintance/weight and i do not think that i have Performance issues and Need 4 motors).
Now i have to decide which Motor i take.
https://hobbyking.com/en_us/turnigy-sk8-6354-140kv-sensored-brushless-motor-14p.html
versus
https://hobbyking.com/en_us/turnigy-sk8-6354-200kv-sensored-brushless-motor-14p.html
```

---
## \#8 Posted by: Acido Posted at: 2018-05-08T17:46:53.040Z Reads: 83

```
2 6374s are overkill especially if you set them on 60a each the board will just fly off from your legs lol 
6355s are really good for dual
```

---

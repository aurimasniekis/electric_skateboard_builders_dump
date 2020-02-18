# How many watts u pull while accelerating / cruising?

### Replies: 28 Views: 1004

## \#1 Posted by: Okami Posted at: 2018-06-15T16:15:45.038Z Reads: 242

```
This should be a poll type topic.. but im open to text replies.

Board setup / rider weight would also be welcome.

---
So far on flat (asphalt) surface, with:

* **8inch** (dual drive) ;

* **9inch** pneumatic (single drive) setups:
---

 I hardly manage more than:
* **1100 - 1200W peak power.**

I weight **93kg**. That might be **180lbs** or so. 

---
For cruising, usually no more than:
* **400-600W** is consumed. 

Yesterday I got to about **750W** when going almost max speed (~35-40kph / ~22mph)

I imagine going over 40kph might require more than 1kw..

Also, a side note, I still live in the 'old world' and doesnt have vesc on either of the boards. So the wattmeter might not be 100% accurate but i believe max deviation should be in 10% range

---

I understand there should be some vesc overlay topics but i wanted to create this one to once again collect some more data and maybe to show that not always 3kw of power is needed

---

Battery wise ive got **2.9 kw capable battery** (dual drive) and **1.3 kw (single drive)**
```

---
## \#2 Posted by: rey8801 Posted at: 2018-06-15T16:21:47.095Z Reads: 224

```
Dueal 90mm hub motors from diyeboard. Dual VESC 4.12 Maytech BLDC Sensorless.

Motor max 50A / Motor min -50A
Battery max 30A / Battery min -6

10s3p Samsung 30Q battery

Top speed around 40Km/h. Nice Torque. Rider weight 76Kg.
Cruising at high speed (for my board) between 400-700W (total for both motors).
Peak power during fast accelleration 1500-1600W.

Nice Thread!

Edit: we should also add the battery type.
```

---
## \#3 Posted by: squishy654 Posted at: 2018-06-15T16:26:41.526Z Reads: 206

```
To find the real world answer you need to plug a watt meter in-line with your battery and then monitor it during a full pull...obviously fat poeple will get higher numbers, lol
```

---
## \#4 Posted by: Okami Posted at: 2018-06-15T19:06:13.037Z Reads: 174

```
Interesting numbers.

 I guess vesc might be able to deliver more power quicker than the chinese dual esc or 'tuned down' 6s car esc.

As about battery. For dual config ive got 10s4p **Sony VTC 4 cells**. 

**Theorethical max power ~2.9kw** = (~80A x 36v) 

---

For my single drive ive got **6s6p Sanyo GA**.

**Theorethical max power ~1300W** = (60A X 21.6v)

Will probably try to update my original post with battery info

---
@squishy654 ive got inline wattmeter on both setups. That is my data source.
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-06-15T19:25:11.936Z Reads: 152

```
15/32 107mm Superfly 10S4P dual 6374 on ackmaniac w/ various watt limits.

I always draw the max wattage set when accelerating. 900W limit = draw 900W.  1700W limit = draw 1700W

If I reduce the throttle, it reduces watts drawn, but if I'm out for fun I'm usually gunning it.
```

---
## \#6 Posted by: 91stantheman Posted at: 2018-06-15T19:31:34.701Z Reads: 142

```
What trucks you running to fit dual 6374's?
```

---
## \#7 Posted by: Brontech Posted at: 2018-06-15T19:35:06.922Z Reads: 148

```
These Work.
collections/longboard-trucks/products/torqueboards-218mm-trucks
```

---
## \#8 Posted by: wafflejock Posted at: 2018-06-15T19:36:32.873Z Reads: 149

```
https://metr.at/r/hmtOO <-- old post but my new data looks roughly the same https://metr.at/r/7me43  Can see some blips in voltage where my second battery is disconnecting some... need to spread the xt-90 connectors on that one a bit so it's a tighter fit.  Not causing significant issues but not ideal.  In general about 400-600W range most of the time.  I'm on "normal" mode in the metr options which is 20A at battery and 40A at motor peak.  I weigh about 115lbs and riding flat land around Chicago.
```

---
## \#9 Posted by: Brontech Posted at: 2018-06-15T19:40:50.959Z Reads: 144

```
I run single TB 6374 190KV (BLDC Sensorless), TB Vesc 4, and 2x6s Graphine Lipo batteries,15/40 15mm Drivetrain.
60 Motor max  -45 motor min
35 Bat Max      -20 Bat Min
I'm 55 KG.

I max at around 1100 Watts when powering up a steep hill or around 1000 when accelerating hard.
When cruising, I average around 500 Watts.
Not Sure about my wattage at max speed, would have to test that on my next ride..
```

---
## \#10 Posted by: skatardude10 Posted at: 2018-06-15T19:42:38.381Z Reads: 142

```
TB218s 1010
```

---
## \#11 Posted by: Ackmaniac Posted at: 2018-06-15T19:56:36.881Z Reads: 141

```
85kg with gear

Dual 12S8P motor max 80A max 192kv 15/36 97mm :
normal riding 2500 watts (1250 each)
3500watts (1750 each) when i need more (there are these days)

Dual 12S4P motor max 80A 170kv 16/62 175mm street pneumatics:
3000 watts (1500 each)
no higher mode as the board becomes too unstable at speed

Dual 13S7P motor max 100A 170kv 10/50 200mm pneumatics (Offroad):
3500 watts (1750 each) could deal with more but for now it's fine
Offrod motor max is more important because most of the time you are not near max speed.
```

---
## \#12 Posted by: ducktaperules Posted at: 2018-06-15T21:39:27.291Z Reads: 126

```
i can confirm.

150KG rider with dual 6374 motors on dual focbox and 12s.
Cruising only uses a few hundred watts but going up some of the larger hills in our area fast i can use ~2000W.

Even at my weight my board really accelerates quickly and I cant go to full throttle for more than a second or so before it starts to get to much. During some abusive testing in a car-park doing full throttle acceleration from standstill in FOC I have managed to pull around 5500W peak. Its genuinely terrifying and no normal person needs this much power.
```

---
## \#13 Posted by: squishy654 Posted at: 2018-06-15T22:28:50.136Z Reads: 110

```
What watt meter are you using that can handle this much amperage?
```

---
## \#14 Posted by: pat.speed Posted at: 2018-06-15T22:30:12.213Z Reads: 110

```
There’s some on eBay rated for 150a at 60v
```

---
## \#15 Posted by: squishy654 Posted at: 2018-06-15T22:32:54.642Z Reads: 108

```
Perfect!!


10 char
```

---
## \#16 Posted by: 91stantheman Posted at: 2018-06-16T01:22:29.251Z Reads: 104

```
That thing must be so freaking rowdy. I'm running a single and it too me a month or so to finally get used to it.
```

---
## \#17 Posted by: E1Allen Posted at: 2018-06-16T03:50:56.356Z Reads: 103

```
Dual 6374 on 12s6p FocBox.  15/36 on 107mm.
I weigh around 180lbs

I've managed to pull almost 5000w battery and 7000w motor from a rolling start.  It Makes me wish I had bindings. Cruising varies but at roughly 33mph I'll consume about 1500w.

I only run one BT module so I just double the necessary values to get total output.

https://metr.at/r/3ACuH
```

---
## \#18 Posted by: wafflejock Posted at: 2018-06-16T04:03:33.668Z Reads: 98

```
How did you jump to 18 mph in the middle there?  Thought at first might have just been a GPS glitch but having a hard time understanding the path from the data.
```

---
## \#19 Posted by: abenny Posted at: 2018-06-16T04:11:13.485Z Reads: 97

```
i dont know my readings while cruising but on a ride my peak wattage is ~1700 with ~59 peak amp draw.
 running 2x4s zippy batteries in series with 2x 6355 260kv sk3 motors
```

---
## \#20 Posted by: E1Allen Posted at: 2018-06-16T12:32:04.281Z Reads: 89

```
Sometimes it glitches
```

---
## \#21 Posted by: wafflejock Posted at: 2018-06-16T13:32:53.445Z Reads: 83

```
Gotcha yah I'm just used to seeing smoother correspondence between the amperage and velocity so think that data is hard to trust when it shows weirdness like that.  Appears as though you bombed down something, gaining velocity without using charge and then just a short spike of amps at the end 🤔
```

---
## \#22 Posted by: E1Allen Posted at: 2018-06-16T13:55:05.701Z Reads: 80

```
Hard to continue spiking amps when you let off the throttle.  I have multiple pulls with similar data. Doesn't take long to reach to speed like that anyways
```

---
## \#23 Posted by: Deckoz Posted at: 2018-06-16T13:55:14.131Z Reads: 81

```
My max battery amps I've seen on my dual 13s, is 43A/ESC, at around 46V. Which is about 2000W per motor. 

My battery amperage isn't very high due to my weight, and even lower the higher the charge. But my board also has no problem putting out 117A to the motors at low duty cycle. 2000W per esc on hard acceleration is pretty much all I can make it draw - even though the total output of my battery is ~5400 watts, I have never seen the board use the last 1400 available with me on it. I have seen it be used on a 200lb friend of mine. I just don't have the mass to require the watts..
```

---
## \#24 Posted by: wafflejock Posted at: 2018-06-16T14:44:16.992Z Reads: 73

```
Yeah the part with the spike and just before it makes sense just looks like it's dropping out some of the earlier acceleration you were doing.  Surprised to see that much dip in voltage but suppose when you're pulling that many amps it is going to dip more significantly too.
```

---
## \#25 Posted by: Vanarian Posted at: 2018-06-16T15:26:54.371Z Reads: 70

```
Wait what, how the hell can you max more motor Watts than Battery Watts ? BTW I'm pretty much same weight than you so this gives me an idea of how much peak watts I might be drawing.
```

---
## \#26 Posted by: E1Allen Posted at: 2018-06-16T15:41:57.786Z Reads: 66

```
Yeah, if you split the voltage drop and compare it to discharge graphs it's pretty close to normal.
```

---
## \#27 Posted by: E1Allen Posted at: 2018-06-16T15:43:38.197Z Reads: 68

```
Somewhere on this forum is some maths explaining phase current draw compared to battery current.  Has to do with duty cycle.  I just know you can pull more phase amps at low duty cycle because of it.
```

---
## \#28 Posted by: Vanarian Posted at: 2018-06-16T16:30:12.421Z Reads: 60

```
I assumed that the ESC converts into more phase amps and less voltage depending on duty cycle (which is why people complained about no 100% duty cycle on previous VESC because it "lowered" a tiny bit the top speed), and the highest the duty cycle, the closest the phase amps and motor voltage from battery amps and voltage ?
```

---

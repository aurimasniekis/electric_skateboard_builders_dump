# What is the correct ESC Amp calculation?

### Replies: 6 Views: 2965

## \#1 Posted by: matock Posted at: 2017-11-12T06:53:04.948Z Reads: 193

```
Hi everybody,

I'm building my first board. After reading a lot, lot, lot on that topic I need some clarity about how to harmonize batteries, motor and ESC.

Many say that the ESC amperage must be higher than what the battery can deliver (peak = A x C). Seems to be quite logical to avoid an ESC burn. So, with a battery configuration 5000mAh-20C they advise to have an ESC of at least 120A or 150A.

I understood also that a VESC is much better than RC ESC for an eSk8 (soft start, brake, recycling brake power, noise, etc). But all VESC I seen draw only 50A and most of the motors need 70-80A. So what? Something I missed?

Let's get an example:
- Lipo batteries 2x 4S-5000mAh-20C in serial, which will provide a max of 2960W (5A x 20C = 100A max, 8S x 3.7V = 29.6V, 100A x 29.6V = 2960W max)
- VESC 50A
- motor SK3 6474 168KV 2400W 80A

The batteries can provide more than the motor needs but ESC is in the middle and will burn. If I configure a 50A limit into the VESC, I  underutilize the motor capabilities, no?

Some sensored motors even consume 3000W. Is it compatible?

I would apreciate - and many others I guess - your fedback. Thanks a lot.

Jo
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-12T07:04:20.580Z Reads: 186

```
The general rule of thumb is to have the esc be able to handle more power than the motor will draw, and have the battery be able to more than the esc. Of course there are other considerations and this isn't always possible. 

That's the beauty of the vesc compared to regular car or plane ESCs. It has the ability to monitor its own current draw and temperature, and protect itself from overheating or otherwise damaging itself, whereas a regular esc that is underspecced will just go until it burns out. 

That's how you can get away with a 50amp vesc and a 150amp battery and 60amp motor.

Also, as with most ground vehicles, an esk8 will only pull maximum power when accelerating from a standstill or accelerating hard up a steep hill. Cruising at speed uses only a fraction of the power. A 50-amp vesc can handle well over 50 amps for a few seconds of hard acceleration, and once you're going, you'll only pull a dozen amps or so.


Setting a realistic current limit in the vesc will limit the motor's potential, but you can always use one of the upgraded vesc spinoffs like the Focbox, AXLE, Ollin v1.1, or even a vesc6 if you really want to push some crazy power. They all feature more robust cooling and better mosfets to handle more current.
```

---
## \#3 Posted by: lowGuido Posted at: 2017-11-12T07:15:44.365Z Reads: 168

```
[quote="matock, post:1, topic:38078"]
with a battery configuration 5000mAh-20C they advise to have an ESC of at least 120A or 150A.
[/quote]

not entirely true.
there are a lot of things to consider here.
first of all these numbers are only ratings. a lot of which are over rated. a 150A ESC from hobby king will most likely not be able to handle a full 150A, but hey lets imagine that it can to make things a little simpler.

here's how the ratings work:

BATTERIES
the current from batteries all depends on the load. if you put a short across a 5Ah 20C battery it will likely draw more than 100A from that battery. you will also likely start a fire or at the very least damage the battery.
so when a manufacturer tells you that the battery is 5Ah 20C (100A) they are actually saying "please don't draw more than 100A from this battery"

ESC's
ESC's work by switching a bunch of FETs back and fourth at various frequency's (not getting into it) anyway FETs are a microscopic semiconducting junction that will burn out at a certain point so they are also rated at a max current.
ESC's are generaly rated by adding up how many FETs are in the ESC and then adding the rating of each FET.
not a super accurate way of doing it.. thats why chinesium ratings are to be taken with a grain of salt.
VESC is rated to the actual rating of the FET that it uses which is 50A
again, you can draw more that the rated current through the ESC by making the load greater and guess what happens?
you burn it.

MOTORS
motors are generally rated on the current that the wire used in the winding is rated to.
again, put enough load on it and you can burn the winding's out.

Current ratings are not there to be matched up with components as such, but rather as a guideline of what not to do with it. if that makes sense..
i mean they kinda can be used to match up... you wouldn't run a 60A motor off a 20A ESC  for example. but I think you get what I mean... guidelines.
```

---
## \#4 Posted by: matock Posted at: 2017-11-13T12:25:43.273Z Reads: 111

```
Thank you MysticalDork and lowGuido, this is clearer now. 
I will opt for a VESC and I will limit the power to 50A.
```

---
## \#5 Posted by: egzplicit Posted at: 2017-11-13T13:14:30.949Z Reads: 107

```
[quote="matock, post:1, topic:38078"]
The batteries can provide more than the motor needs but ESC is in the middle and will burn. If I configure a 50A limit into the VESC, I  underutilize the motor capabilities, no?
[/quote]

VESCs have battery max and motor max. You can still push more than 50A on the motor even if the battery max is 50A: this is because of duty cycle. At low and mid speeds you might be pulling 50A from the battery but not at full voltage, that allows the controller to push more than 50A into the motors. W = Ah * Volts. If you pull 50A at 42v from the battery that’s 2100W but when the vesc is at 50% duty cycle it means 21v. At 21v it can push 100A into the motor (2100W total power / 21v = 100A). So you see how you can pull 50A from the battery and match the vesc rated Ah but still push 100Ah into the motor.
```

---
## \#6 Posted by: matock Posted at: 2017-11-15T11:10:41.888Z Reads: 90

```
Indeed, you are right.I didn't pay attention on the motor voltage, I was focussed only on the battery voltage.
This shows how VESC is much better than a simple ESC.
Very thank you.
```

---

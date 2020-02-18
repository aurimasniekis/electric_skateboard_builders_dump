# 3D printer capacitive proxmitiy sensor problem

### Replies: 12 Views: 8131

## \#1 Posted by: DeathCookies Posted at: 2016-10-02T17:03:19.914Z Reads: 76

```
Hey folk,
currently i am having issues with my proximity sensor for my 3D printer.

I am going to replace my Z_MIN_ENDSTOP with a capacitive proximity sensor which is installed next to my extruder.
The sensor is running on 6-36V but the RAMPS 1.4 uses 5V for the endstops.

So i had wired my sensor like this:
http://1.bp.blogspot.com/-6VcowyDvQmI/VRc83GpH2uI/AAAAAAAAGrE/Fhod5g2fKfU/s1600/induction%2Bdistance%2Bsensor%2Band%2B3d%2Bprinting%2Bbed%2Bleveling%2B2.jpeg

The problem is that a normal endstop has 0V (triggered) and 5V (open). Somehow my sensor is outputting 3,4V (triggered) and 4,7V (open). Therefore my printer recognizes the sensor as always open (because it will never output 0V...)

Can someone help me out?

1. Why does it output 3,4V instead of 0V?
2. Is there a firmware setting that i could manipulate to recoginze 3,4V as triggered?
3 Do you have any other suggestions to solve my problem?

I really appreciate any help! Thanks in advance
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2016-10-02T18:26:41.968Z Reads: 52

```
Do you have the datasheet for the sensor? Hard to say for sure, if we don't know what's going on inside the sensor.
Maybe it's output is an open collector?
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-10-02T18:33:56.323Z Reads: 51

```
[quote="SimosMCmuffin, post:2, topic:10512"]
Do you have the datasheet for the sensor?
[/quote]

https://www.amazon.de/gp/product/B00SO2ATWK/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2016-10-02T18:48:37.078Z Reads: 45

```
Ok, dug around for some data and found this: "Metal housing, output type: PNP NO (Normally Open)"

I'm guessing at this point that the output IS an open collector, so you need to provide pull up resistor for the output.

Have you measured the voltage of the OUT pin with a multimeter when you trigger the sensor?

EDIT: correction, it is not an open collector output, due it being a PNP transistor. Refer more to this site http://www.ab.com/en/epub/catalogs/12772/6543185/12041221/12041723/Output-Types.html
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2016-10-02T19:07:35.497Z Reads: 43

```
I recommend watching this video:
https://www.youtube.com/watch?v=PtwquSJ1zgw
```

---
## \#6 Posted by: chinzw Posted at: 2016-10-02T19:29:54.696Z Reads: 41

```
Want to simplify your life and avoid any more sensor problem? Just use a diode instead of the voltage drop resistors.
1N4001 on the signal wire, facing the probe and connect the + and - to 12v.

So you would have the wiring like this:
RAMPS --> ->|- --> SENSOR

Then in marlin i have:
#define Z_MIN_PROBE_ENDSTOP_INVERTING false // set to true to invert the logic of the endstop.

If your limit switches dont need pullups, you can use this:
#define ENDSTOPPULLUPS // Comment this out (using // at the start of the line) to disable the endstop pullup resistors

Of if you do need pullups for you limits use this:
#if DISABLED(ENDSTOPPULLUPS)
  // fine endstop settings: Individual pullups. will be ignored if ENDSTOPPULLUPS is defined
  #define ENDSTOPPULLUP_XMAX
  #define ENDSTOPPULLUP_YMAX
  #define ENDSTOPPULLUP_ZMAX
  #define ENDSTOPPULLUP_XMIN
  #define ENDSTOPPULLUP_YMIN
  #define ENDSTOPPULLUP_ZMIN
  //#define ENDSTOPPULLUP_ZMIN_PROBE
#endif
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-10-02T20:42:09.834Z Reads: 31

```
[quote="chinzw, post:6, topic:10512"]
Want to simplify your life and avoid any more sensor problem?
[/quote]

Yes, that sounds nice!
[quote="chinzw, post:6, topic:10512"]
RAMPS --&gt; -&gt;|- --&gt; SENSOR
[/quote]
So i just need a 1N4001 diode between the sensor and the ramps input signal?

[quote="chinzw, post:6, topic:10512"]
facing the probe and connect the + and - to 12v.
[/quote]

The wirings i have found always say that i need to attach negative and signal to the RAMPS. Your solution would be to connect only the signal to the RAMPS?

Do i destroy my ramps when the signal input has 12V? I think i have read that i need for the sensors 5V.

Thank you very much for the help.
```

---
## \#8 Posted by: chinzw Posted at: 2016-10-03T01:14:24.633Z Reads: 27

```
1N4001 should work, actually, pretty much any diode will work, i used 4001 cause i had them around.
There should be no 12v going TO the ramps since the diode prevents this from happening, it will basically close the circuit from the ramps.
I have it wired up like that and had 0 problems, and if you happen to do something really wrong, most of the time you'll just fry that IO PIN, which in the ramps we have min/max for every axis and almost never use 2 limits per axis, so you have 3 extra IO PINs you can fry :slight_smile:
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-10-03T13:01:06.640Z Reads: 20

```
[quote="chinzw, post:8, topic:10512"]
1N4001
[/quote]

There are two states:
- triggered
- open

In one of the two states there will be current going through the sensor wire.
If i attach the sensor (+ and -) to 12V from my psu the sensor wire will have 12V (imo too much for the ramps)

So i attached the the two resistors like shown in the previous picture.
Then i will have 4,7V and 3V but i need 4,7V and 0V.

So your advise would be to hook up a diode between the sensor wire and the ramps.

Does this diode block only the 3V or does it block the 4,7V too?

I dont get it atm... but thank you for your help :) it is appreciated

edit: @chinzw maybe you could make a picture of your wiring to explain it better?
```

---
## \#10 Posted by: DougM Posted at: 2016-10-03T15:36:54.162Z Reads: 12

```
I think it would be better to use either a 5v Zener diode in conjunction with the current limit resistor (put the resistor between the diode and the sensor and go down to 10k or maybe 47k) or a cool trick is to use a 5v shunt regulator so the V-in is on the sensor side and the V-out is on the logic side and gnd goes to gnd.
```

---
## \#11 Posted by: chinzw Posted at: 2016-10-03T16:51:59.505Z Reads: 10

```
There's no 12v going to the ramps, since there's a diode. Just read this here, search for "Kostas Karouzos":
http://opensourceecology.org/wiki/Research_On_Inductive_Proximity_Sensors
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-10-03T17:58:17.903Z Reads: 9

```
I just got it working. Thank you all for the help. :thumbsup:
This thread can be closed
```

---

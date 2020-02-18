# Prevent battery drainage when Eskate is left turned on

### Replies: 11 Views: 572

## \#1 Posted by: drassak Posted at: 2018-02-09T10:20:02.901Z Reads: 170

```
Hello All,
I’ve been reading this forum for a while but never posted.

Yesterday I killed my freshly built 10S 10Ah lipo pack. I basically left my board turned on for a week. The 2 VESC and the RC receiver drained the pack to the core and the pack ended up swollen and down to 0.5V per cell…

My question is : Is there a way to prevent battery drainage if the board is accidentally left turned on ?

•	The VESC has a cut-off feature that prevent to rev up the motor if a low V value is hit but the VESC is still running an will keep on using a bit of power. Can it be set up so that it completely turn off if the voltage falls low ?
•	I use a BMS that has a built-in 2.9V cut off ( http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html ).
However I have to bypass it in discharge because it’s limited to 60A and i run my dual at 45A per motor. Do you think I can still use it in discharge ?
Also the datasheet reads it has a 200µA (200µA/h ?? ) static power consumption, does it mean that if I leave it wired on discharge it will use 0.2mA/h ?
•	I was thinking putting a low batt buzzer like this (https://hobbyking.com/fr_fr/hobbykingtm-lipoly-low-voltage-alarm-2s-4s.html ) but idk what’s the static power consumption and if i would drain or unbalance the pack on the long run ?

if you have any suggestion

Thanks !
```

---
## \#2 Posted by: laurnts Posted at: 2018-02-09T10:28:58.971Z Reads: 158

```
Use BMS and dont use electronic switch.
BMS should prevent this, but when you bypass it then its not doing what it should do.
I also have this issue 2x because of using electronic switch / accidental switching back on due to slight force on the switch its self. Now I am using loop key, works like a charm.
```

---
## \#3 Posted by: drassak Posted at: 2018-02-09T10:33:14.374Z Reads: 151

```
thanks for the feedback, the loop key prevent the accidental powering on but not if you "forgot" to remove it.

I am thinking of remove the bypass on the BMS but do you think 60A is enough for a street dual meant to climb som hills?
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-02-09T10:49:44.024Z Reads: 138

```
The simplest is never forget to turn off and check if it really did, do it a lot of times and it will become natural

The other way is modify the electronic switch to work as a soft latch and have it connected to a micro controller, make it turn off after x amount of time without remote input
```

---
## \#5 Posted by: GunnarK Posted at: 2018-02-09T10:58:54.465Z Reads: 130

```
I have a BMS installed as well but I also have a percentage indicator after the BMS which is backlight

![IMG_20171030_104708|666x500](upload://aUGMhBh9wlQITfrzOnvywm9A5Qx.jpg)

This way I can spot from across the room if my board is still on!
```

---
## \#6 Posted by: pat.speed Posted at: 2018-02-09T11:11:38.703Z Reads: 125

```
Yeah this is a good way. I have my tail lights linked to my board's switch so the lights will only turn off when I turn the board off. They are so bright that you can't miss them
```

---
## \#7 Posted by: drassak Posted at: 2018-02-09T11:16:06.504Z Reads: 120

```
thank for your feedback now i'm think about putting a LED on the side of the enclosure. Do you know if I can take the 5V off the slave VESC?
I also a have a UBEC, but never used it since it is for 6S and my battery is 10S. I was wondering if plugging a UBEC on only 6 cells out of the 10 would unbalance the whole thing.
```

---
## \#8 Posted by: Vanarian Posted at: 2018-02-09T11:43:23.375Z Reads: 116

```
A good point would be to be able to unplug your batteries ? Just in case I mean, if you have an easy access to them.
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-02-09T21:48:56.634Z Reads: 89

```
Sure, you can take about 1A of each VESC, just don't join the 5V of both together
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-02-10T00:05:33.125Z Reads: 79

```
i used to forget all the time too, but after installing headlights lights it's kind of hard to not notice when it's powered on.
```

---
## \#11 Posted by: krloz Posted at: 2018-02-10T11:06:34.508Z Reads: 54

```
You can wire some leds directly to battery as well. Then you don't have to touch the vesc power.
I mean after the switch obviously
```

---

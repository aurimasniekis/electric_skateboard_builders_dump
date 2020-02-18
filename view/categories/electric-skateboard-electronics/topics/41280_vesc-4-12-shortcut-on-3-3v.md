# VESC 4.12 Shortcut on 3.3V

### Replies: 7 Views: 811

## \#1 Posted by: fred Posted at: 2017-12-17T20:45:18.260Z Reads: 135

```
hey,

i have a problem with 2 VESC HW 4.12.
the both of them are new and gets really hot when power on.

At the beginning (15 min before noticing the heat) i've reprogrammed them with the latest version of the boot and software using an st-link v2.

Then configured them using ppm and can slave and master mode.

At this point i notice the temperature rising and disconnect them.

After a sont small test i identified the heat source to be the voltage regulator (VREG) 5V to 3.3V  (579-TC2117-3.3VDBTR)

During the test one of my esc (the second one) stop fonctionig (VREG output became couple of hundred mV instead of 3.3V)

VESC 1:
The resistance from 3.3 to GND is about 14 ohms

VESC 2: 
The resistance from 3.3 to GND is about 0.7 ohms
I desoldered VREG and mesurd from 3.3 to GND  0.7 ohms

Did some on incounter the same probleme?
Could i get some guidance on what to do the identify the problem.

Thank's
Fred
```

---
## \#2 Posted by: ugothakd Posted at: 2017-12-17T22:03:45.671Z Reads: 109

```
Can transceiver? What gets hot?
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-12-17T22:06:18.333Z Reads: 99

```
https://www.electric-skateboard.builders/t/vesc-capicators-problem/10949/11?u=johnnymeduse
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-12-17T22:08:08.339Z Reads: 100

```
When the can cable is connected you should always power up you two Vesc simultaneously, or else it will most likely blow up the Can Transceiver U401.

you could always change U401, or remove it on each vesc and use split PPM cable.
```

---
## \#5 Posted by: hackware Posted at: 2017-12-18T02:32:03.637Z Reads: 80

```
wow...   really...?

i'm working on a 4 wheel drive (4 focbox)...

u401 will almost always die then...

horrible design flaw...

william...
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-12-18T02:34:54.006Z Reads: 74

```
You can use multiple remote transceivers, like @BigBoyToys does in is 4WD Trampa.
```

---
## \#7 Posted by: fred Posted at: 2017-12-18T14:42:53.246Z Reads: 50

```
Thanks, i made the modification ( remove the can transceiver ) and used a split PPM cable, everything work properly. I will order two new transceiver, i am really grateful to know why they failed, so it wont happen again!
```

---

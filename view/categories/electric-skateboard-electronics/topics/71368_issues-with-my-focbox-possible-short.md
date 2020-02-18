# Issues with my FOCBOX (possible short?)

### Replies: 7 Views: 183

## \#1 Posted by: Rysa Posted at: 2018-10-16T04:18:11.779Z Reads: 55

```
So i'm having some issues with both of my FOCBOX's. I had a small spark inside my XT60 when plugging the FOCBOX to my battery, however all leads seem to be wired correctly and its a 42V 18650 battery pack that seems to be at an acceptable voltage. When i plug my battery in i get 5v out of all 5v pins but no lights and nothing out of the 3.3v pin. I had read that i can do a continuity check with my multimeter over the c25 capacitor to test if the 5v had been shorted to ground, which it appears it has.

per @JohnnyMeduse post [No power to Enertion Vesc](https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8)

Does this suggest theres an internal short over the CAN transceiver (u401)? And if so, Is there anything i can do to fix this, and can anyone suggest how this might have occurred? here are some photos of my setup…



FOCBOX 1:
[![IMG_6764|666x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/c/0/c0867c06b8f08ba74747d69e8673f66a8f55784a_1_666x500.jpeg)
IMG_6764.JPG4032x3024 1.61 MB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/0/c0867c06b8f08ba74747d69e8673f66a8f55784a.jpeg)

 
FOCBOX 2:
[![IMG_3067|666x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/0/2/0209acbd4d6dc423afb50b268439ee109c30a241_1_666x500.jpeg)
IMG_3067.JPG4032x3024 1.69 MB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/0/2/0209acbd4d6dc423afb50b268439ee109c30a241.jpeg)

 
Battery:
[![IMG_7295|375x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/9/0/90addf3e6e020ba2245f1215ead093dae219d75c_1_375x500.jpeg)
IMG_7295.JPG3024x4032 2.43 MB
](https://www.electric-skateboard.builders/uploads/db1493/original/3X/9/0/90addf3e6e020ba2245f1215ead093dae219d75c.jpeg)

Thanks for your time everyone, appreciate any ideas!
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-10-16T04:22:54.939Z Reads: 48

```
[quote="Rysa, post:1, topic:71368"]
Does this suggest theres an internal short over the CAN transceiver (u401)?
[/quote]

Yes... You can either replace those Can chip or Removing them and use split PPM cable.
```

---
## \#3 Posted by: Rysa Posted at: 2018-10-16T04:37:02.378Z Reads: 48

```
Do you have any idea how this sort of thing could have occurred? last thing i want to do is replace the chip and then the same thing happens again.
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-10-16T04:39:26.878Z Reads: 48

```
Dont unplug single focbox while they are both on and CAN bus connected it instantly kills CAN chip

EDIT: u can make Y adapter and zip tie each focbox so it wouldn't disconnect by itself.
```

---
## \#5 Posted by: Rysa Posted at: 2018-10-16T05:04:34.745Z Reads: 41

```
Good tip will keep that in mind! it seemed to happen when i plugged in a single FOCBOX on its own, as thats when i saw a spark in the XT60 (which appears to be burnt at the terminals), but ill definitely only plug/unplug from the single XT90 Y adaptor i made up from now on!
```

---
## \#6 Posted by: Rysa Posted at: 2018-10-16T05:06:30.735Z Reads: 40

```
Also any ideas how hard it will be to replace the chip on my own? willing to give it a crack, just not sure where to start...
```

---
## \#7 Posted by: Kug3lis Posted at: 2018-10-16T05:46:05.962Z Reads: 34

```
Easiest way is to get hot air station and just heat that chip up and remove it and and then solder new in. Also u will need probably replace can termination resistor R40* next to chip

This is how my Y splitter looks with zip ties

![image|375x500](upload://yyg90ozuDcuaNx4diH5awQNMEYa.jpeg)
```

---

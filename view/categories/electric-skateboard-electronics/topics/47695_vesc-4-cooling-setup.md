# VESC 4 cooling setup

### Replies: 22 Views: 1375

## \#1 Posted by: Ingvarjedi Posted at: 2018-02-27T20:26:17.178Z Reads: 188

```
Hi people
How can I make VESC4 cooling?
I want the cooling to be turned on when I work with the VESC4
and the fan speed increased from the increase in the temperature of the VESC4. Is it relational?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-27T20:28:41.750Z Reads: 183

```
heatsink...?
```

---
## \#3 Posted by: b264 Posted at: 2018-02-27T20:34:27.632Z Reads: 180

```
You can redeisgn the VESC4 PCB, manufacture your own controllers, adding an output on an unused MCU pin and make a custom modification to the firmware to control the fan.

Or you can just make an analog circuit that ventilates your enclosure proportional to enclosure temperature.

This is the whole "Y" part of "DIY"  :stuck_out_tongue:
```

---
## \#4 Posted by: Ingvarjedi Posted at: 2018-02-27T20:43:21.108Z Reads: 167

```
It's so complicated.
Easier to make forced cooling from a separate battery)))
```

---
## \#5 Posted by: b264 Posted at: 2018-02-27T20:44:41.300Z Reads: 154

```
You can buy very good electric skateboards already pre-engineered from Metroboard

:stuck_out_tongue:
```

---
## \#6 Posted by: GrecoMan Posted at: 2018-02-27T20:46:20.468Z Reads: 147

```
that’s a negative soldier. i made my heatsink in less than 5 minutes
```

---
## \#7 Posted by: Ingvarjedi Posted at: 2018-02-27T20:52:08.999Z Reads: 139

```
How? Was it integrated into the VESC or does it work separately?
```

---
## \#8 Posted by: GrecoMan Posted at: 2018-02-27T20:53:40.082Z Reads: 140

```
do you know what a heatsink is?

it’s a piece of aluminum screwed onto the vesc, contacts the FET’s with thermal pads, it also contacts the DRV
```

---
## \#9 Posted by: Ingvarjedi Posted at: 2018-02-27T20:56:20.242Z Reads: 139

```
Yes, i know)
```

---
## \#10 Posted by: ElskerShadow Posted at: 2018-02-27T21:02:18.298Z Reads: 136

```
Maybe use @Kug3lis vesc box ?
```

---
## \#11 Posted by: Ingvarjedi Posted at: 2018-02-27T21:18:48.669Z Reads: 130

```
I have VESC 4)
```

---
## \#12 Posted by: Ingvarjedi Posted at: 2018-02-27T21:18:56.963Z Reads: 130

```
Is it necessary to put a fuse on 80A?
```

---
## \#13 Posted by: abenny Posted at: 2018-02-27T21:44:39.777Z Reads: 125

```
his whole post is asking about how to get sufficient power to a fan...heatsink is an obvious minimum in this case as a fan alone wouldnt do much...he wants to actively cool his vesc by a fan and heatsink; a heatsink alone is passively cooled
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-02-27T21:46:16.727Z Reads: 120

```
my point is, the vesc really doesn’t need that much cooling. also, a fan will do pretty much nothing unless it’s in a small individually sealed box
```

---
## \#15 Posted by: abenny Posted at: 2018-02-27T21:49:48.252Z Reads: 121

```
i agree with you on this. a heatsink (ie. passive cooling) is more than what is necessary for a vesc 4. the heat removal increase from adding a fan to it would be minimal and would likely only give a slight temperature decrease with minimal to no performance increase...
the bottom line is essentially that if it was beneficial to actively cool vescs, the manufacturers would be doing it already.

But if @Ingvarjedi wants to do it , more power to him, its all in the diy spirit after all :smiley:
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-02-27T22:13:56.238Z Reads: 114

```
https://shop.3dservisas.eu/products/aluminium-case-for-vesc-v4-12-bldc-motor-controller
```

---
## \#17 Posted by: Cobber Posted at: 2018-02-27T22:18:08.058Z Reads: 112

```
lots of heatsinks here ready to go: https://www.moddiy.com/categories/Heatsinks-%26-Cooling/

Kugies case is better but...
```

---
## \#18 Posted by: Vanarian Posted at: 2018-02-27T22:38:08.004Z Reads: 100

```
I'm fucking proud of you :joy: @Kug3lis see? My _obsession_ starts bearing fruits!
```

---
## \#19 Posted by: b264 Posted at: 2018-02-27T22:43:07.684Z Reads: 99

```
[quote="Ingvarjedi, post:11, topic:47695, full:true"]
I have VESC 4)
[/quote]

He has them for VESC4
```

---
## \#20 Posted by: Ingvarjedi Posted at: 2018-02-28T05:23:54.038Z Reads: 87

```
Watch this video.
But this is a bicycle and the engine is probably more powerful

https://www.youtube.com/watch?v=UwVQQ_LY5bc
```

---
## \#21 Posted by: Ingvarjedi Posted at: 2018-02-28T05:25:52.719Z Reads: 85

```
Which radiator is better?
1. Small for each chip?
2/ A large radiator covering the entire area of ​​the VESC?
```

---
## \#22 Posted by: abenny Posted at: 2018-03-03T18:59:29.184Z Reads: 65

```
with my basic knowledge in heat transfer id assume a larger aluminum piece. Q(the heat transfered) = h*A*DeltaT
h is the convective heat transfer coefficient, and delta T is the difference in temp between the surface of aluminum and air
where A is the surface area of heat transfer on the air side of the heatsink....more surface area = more 
heat transferred...in theory.
```

---

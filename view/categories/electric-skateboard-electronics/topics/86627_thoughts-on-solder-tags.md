# Thoughts on solder tags

### Replies: 9 Views: 401

## \#1 Posted by: ZachTetra Posted at: 2019-03-09T04:14:19.549Z Reads: 133

```
How good are the u-solder tags on NKON batteries (30Q)?  I didn't see any fish paper on the positive terminals, but my option for a spot welder is a car battery and some 12v automotive relays in parallel with a basic timing circuit so I'm not sure my welds will be good either.

The enclosure will see heavy mechanical abuse so the cells will too (there is gonna be 15mm between the enclosure and the ground and the axle distance is 32", and I ride over lots of sidewalk edges) so I need the most durable option above all

Between the tags and spotty welding what do you guys recommend?
```

---
## \#2 Posted by: pat.speed Posted at: 2019-03-09T11:38:07.140Z Reads: 106

```
Build a welder using a microwave transformer and timing circuit on aliexpress. Total should be around $50, allows changes of power as well as pulse length. 

I found it great for building my 12s3p
```

---
## \#3 Posted by: StefanMe Posted at: 2019-03-09T11:43:05.847Z Reads: 100

```
https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v3/

The best thing u could buy...
```

---
## \#4 Posted by: TowerCrisis Posted at: 2019-03-10T03:26:11.836Z Reads: 66

```
"Typically one 40Ah 440A battery delivers enough current to get good welds with 0.15mm nickel strips and even 0.25mm nickel strips. For thicker nickel strips maybe you will need bigger battery (max. 800 CCA)

The Welder generates a double pulse, where the first one is 12% of the time of the second one by default. Pulse time of the main pulse is adjustable by the rotary encoder and displayed on the screen in ms so you can exactly adjust the time. Its adjustable from 1 … 100 ms by default. (adjustable up to 500ms in the system menu)"

This seems like a really quality welder. Why don't more people use this?
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-03-10T03:27:38.151Z Reads: 63

```
It hurts to spend money that doesn't go on the board?
```

---
## \#6 Posted by: mishrasubhransu Posted at: 2019-03-10T03:57:26.498Z Reads: 62

```
Use NESE. High current capability, safer(in my opinion), easy to DIY,  cheaper and serviceability of cells. 

parts here: https://18650.lt/ and updated files from Agnius(creator) here:
https://www.electric-skateboard.builders/t/n-e-s-e-nese-no-solder-module-battery-packs/36847/951?u=mishrasubhransu
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-03-10T04:25:06.549Z Reads: 53

```
I was thinking of something like that...its same deck as yours but with smaller wheels and more stuff so space is already tight, I think you lose a centimeter in each direction per module?
```

---
## \#8 Posted by: gmurad Posted at: 2019-04-28T16:04:48.893Z Reads: 30

```
Did you end up using the u-solder tags? I'm using NESE for the next build but seeing that NKON will ship with the c-tags on already (for a charge) and the PCBs that are available these days I'm thinking this can be a really good alternative to build a battery pack without a spot welder.
```

---
## \#9 Posted by: ZachTetra Posted at: 2019-04-28T16:09:19.871Z Reads: 26

```
I'mSo I fucked up and bought used cells...I was gonna use the tags until someone sold 48 almost new cells with a 80a BMS and a bunch of other stuff for less than the cells would be new

Gonna use cell holders instead, they can hold 10A without melting so I'll bulk them up with 10awg and try to pull 20A, if they get hot I'll get a welder and add tags to to bridge them to the wires

In terms of feasibility, the tags are good alternative, just need a soldering iron and the PCBs
```

---

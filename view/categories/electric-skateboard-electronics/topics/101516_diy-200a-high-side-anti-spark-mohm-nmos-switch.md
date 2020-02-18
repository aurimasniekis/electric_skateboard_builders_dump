# DIY 200A High-side Anti-spark mOhm NMOS switch

### Replies: 11 Views: 1060

## \#1 Posted by: VinFar Posted at: 2019-09-08T20:26:46.156Z Reads: 104

```
Hey everyone,

I'm new to this forum and currently working on a Anti-spark switch for my boards.

All the available projects didn't fit my needs, so I decided to design my own switch.
In my opinion, they all were too big, or too expensive or didn't have the feature I needed.

![front|607x500](upload://iZpiVQ6Xl9ZwCTNLHpmMX77ah1p.png) 
![front_with_copperbar|690x396](upload://ty6W58keEt7WbBzrumvjKQM29H9.png)
![with_heatsink|690x425](upload://pLvo3i1yxugbtkGrojTG6jovLlo.png) 
![heatsink|690x435](upload://jQwNrRW0mWUMsBlZDi56nRT1Z2H.png)

## It has the following features:
  - dimensions: 74mm x 38mm
  - theoretically Rdson of 90 uOhm
  - maximum current of around 200A (more with additional copper and cooling)
  - maximum voltage of 60V
  - 12V 50mA LDO output
  - controlled dI/dt with capacitor and current limiting resistor
  - two IRFS7530 N-channel MOSFET
  - BQ76200PWR High Side MOSFET Driver
  - A holder for a LittleFuse BF1
  - 4 pin JST XH connector for an external switch
  - exposed pcb traces to add solder or a copper bar for lower resistance

### LDO
The 12V LDO is only used to drive an LED that is included in my switch. It won't deliver much current, due to the high heat dissipation: 38V delta voltage means 0.38W for every 10mA, which is much for such a small package.
You can leave it unused if you want.

### FUSE
As seen by other Anti-Spark switches I went with the LittleFuse BF1. It can be soldered directly to the PCB, so there is no need of screw terminals. However, there are 6.5 mm screw holes. You can also use a copper strip in replacement for the fuse.

### controlled pre-charge
The MOSFET are connected to the Driver over an RC element to slowly turn on the MOSFET in order to have controlled dI/dt for high capacitive loads.

### low-cost
If you order the PCB on JLCPCB ( 1.8€ for 5 pcs)  and the parts from mouser, it will only cost around 30€ (you can use fewer MOSFET to decrease the prize). The SMD components can be soldered with a little bit of skill and a standard soldering iron.

### exposed PCB traces
The PCB traces for the power lines are exposed so that a copper bar or additional solder can be attached to it, to decrease the resistance. [like this copper bar](https://www.ebay.de/itm/Kupfer-Stange-Kupferschiene-Cu-von-10x3-40x3-mm-Abm-Lange-wahlbar/121251176827?var=420221612781&hash=item1c3b22217b:m:mVAqh4BAUsxgg77E7nHCCew)

### The project is available on GitHub under [this link](https://github.com/VinFar/High-Side-NMOS-Antispark-Switch)

I will improve and finalize the PCB in the next days and order some at JLCPCB in the next days and see if everything is working as expected. Especially if the PCB can handle the current.

I'll get back to you as soon as I know the details.

If you have any suggestion or question, feel free to comment!
```

---
## \#2 Posted by: skatardude10 Posted at: 2019-09-08T23:13:30.066Z Reads: 88

```
Nice man, would love to see how this holds up over time.
```

---
## \#3 Posted by: Schulerbible Posted at: 2019-09-08T23:25:51.748Z Reads: 85

```
How much OZ copper do you get? I wanted to make a fuse holder but then figured out I'd need to use 4-5 oz copper to be able to push thru the amps which turned out to be way too expensive....
```

---
## \#4 Posted by: VinFar Posted at: 2019-09-09T07:19:33.699Z Reads: 85

```
@Schulerbible I think 1oz will be fine, if copper strips and solder is added to the traces. In this way you can enlarge the cross section of the traces. We will see if this is working.
At JLC you can also order 2oz, but this will increase the price dramatically.

Also I decided to use 4 FETs instead of 2 on the PCB.
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-09-09T07:43:55.782Z Reads: 78

```
Nice work!

If you haven't you should check out my designs as well.

https://www.electric-skateboard.builders/t/some-open-source-antispark-designs-that-work/100418?u=gamer43

I use the ltc7004 gate driver instead. While the easyeda design calls for the IPB014N06N, I would recommend the TPW1R306PL,L1Q, it's cheaper and has double sided cooling.
```

---
## \#6 Posted by: VinFar Posted at: 2019-09-09T08:27:32.173Z Reads: 68

```
@Gamer43 Thanks, your FETs look great! I will have a closer look this evening and probably use them, as they are much smaller.
```

---
## \#7 Posted by: VinFar Posted at: 2019-09-09T20:08:20.926Z Reads: 64

```
Hey,

I made an upgraded version with the MOSFETs from @Gamer43.

![front|690x315](upload://1FFJih5KPk8xBiVIA2dROT8vm5t.png)
![back|690x315](upload://eFbU9fpposYDVgKzwxAHczNYSL.png)
![PCB|690x372](upload://9yyUn8JzvdXjmPpWSgWm1ljofAr.png) 

The PCB now has space for 10 MOSFETs, which will end up in theoretically Rdson of around 90 uOhm. I'll check how high the actual resistance is.

In order for the tracks to be able to carry the current, it is necessary to solder on [such copper rails](https://www.ebay.de/itm/Kupfer-Stange-Kupferschiene-Cu-von-10x3-40x3-mm-Abm-Lange-wahlbar/121251176827?var=420221612781&hash=item1c3b22217b:m:mVAqh4BAUsxgg77E7nHCCew). Or simply apply a lot of solder.

I will come to back to you, when I received a bunch of PCBs
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-09-09T22:37:18.824Z Reads: 56

```
The maximum specified Rdson is 1.29mohms, so 10 of them will be 130 uohms worst case.

From my experience, most of the resistance will actually come from the PCB and the wire joints. Soldering on 12 AWG to the PCB traces got the total resistance of 1oz PCB that was 2inches wide from 3miliohms to about 600uohm. 
You really should not need more than four MOSFETs in parallel, as even with 12 AWG, I still encountered much higher resistances elsewhere in the PCB.
```

---
## \#9 Posted by: Movation Posted at: 2019-09-10T23:26:22.431Z Reads: 44

```
Fantastic Project following...
```

---
## \#10 Posted by: VinFar Posted at: 2019-09-11T19:34:16.506Z Reads: 38

```
Hey,

I finished the PCB and already ordered them at JLCPCB (10€ for 10pcs :grinning:). I also designed an aluminum heatsink that directly attach to the top FETs. I think I will just use the upper 5 FETs, cause they will have a low enough resistance.

The copper bars have dimension of 10mm x 3mm which end up in a resistance of 0.6 mOhm per meter, so for a length of 70mm 41.53 uOhm. I will solder them to PCB, which will hopefully work.
The holes in the copper bars are not necessary, so I will leave them out or just not use the fuse and use a copper bar instead.

![front|607x500](upload://iZpiVQ6Xl9ZwCTNLHpmMX77ah1p.png) 
![front_with_copperbar|690x396](upload://ty6W58keEt7WbBzrumvjKQM29H9.png)
![with_heatsink|690x425](upload://pLvo3i1yxugbtkGrojTG6jovLlo.png) 
![heatsink|690x435](upload://jQwNrRW0mWUMsBlZDi56nRT1Z2H.png)

The aluminum heatsink can be milled using a CNC machine. It has cut outs for the JST connector and for screws to mount it to the PCB.

Hopefully, this all works as expected :sweat_smile:
```

---
## \#11 Posted by: Movation Posted at: 2019-09-11T22:41:41.432Z Reads: 37

```
Keen to try it out. Had a lot of luck with building OG Vedder design but this is way more  elegant. I dont have a cnc but I think I could use a aluminum plate with a copper shim over the fets.
Fantastic work.
```

---

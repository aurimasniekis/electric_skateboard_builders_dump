# Building your own VESC?

### Replies: 12 Views: 3166

## \#1 Posted by: Muke Posted at: 2017-11-24T15:44:58.037Z Reads: 281

```
Has anyone build a self made VESC yet?
I would love to give it a try but I haven't found much information about people doing it on their own.
Vedders open source project info could be enough.

As a note: I would do it for fun and to learn something.
```

---
## \#2 Posted by: FredrikHems Posted at: 2017-11-24T17:28:24.168Z Reads: 269

```
Yes, there is Actually a dude on the forum Who are building a 6.4HW based one right now.

Edit: here you go

https://www.electric-skateboard.builders/t/hw6-4-based-esc/37579/79
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-11-24T18:22:00.569Z Reads: 257

```
It's entirely possible, but it's still a fairly involved project, especially with the SMD soldering (and the ground pad under the DRV). There are quite a few places that will do low volume production of PCBs cheaply, and all the components are listed in vedder's BOM.
```

---
## \#4 Posted by: stewii Posted at: 2017-11-24T21:20:27.864Z Reads: 239

```
I don’t think it is an involved project. It is a DIY project, And with the right tools it’s not that hard. The DRV is not the only component with a ground pad, the CAN and nRF chips as well. I am thinking of making an order and get the PCB assembled from factory, but I need at least 20 units order.
```

---
## \#5 Posted by: chuttney1 Posted at: 2017-11-25T05:34:43.627Z Reads: 206

```
Before all this VESC 6.0 and VESC 6.4 HW talk, I made a VESC 4.7 with the DRV8302 and ended up just buying already made ones in the past. I ran afoul with the DRV8302 not working after the first try and coming to a long thought decision.... In the end, I spent over $1000 doing this project. Think twice about tossing this much money into a hobby like this.

Heres the steps:
1. Find schematic and send files of PCB files made in a CAD program such as EAGLE or KiCAD to the PCB house
2. Wait three weeks for PCB to arrive from China or less 
3. Gather your components and solder paste from Digikey or Mouser
4. Get a soldering iron with adjustable temperature knob or hot air soldering station or infrared toaster over
5. Assembly is solder place on PCB pad before component
6. Double check while placing component into the right spot.
7. Solder everything on one side before moving to the next side
8. Test using low voltage such as 24V to upload the firmware and know it works with motor
9. Test at the voltage to be run at such as 10S and hope you don't get a DRV error.
10. If no DRV error. You have just done everything correctly.
```

---
## \#6 Posted by: aigenic Posted at: 2017-11-25T07:34:55.897Z Reads: 175

```
Here is original @torqueboards question about it on [endless shpere](https://endless-sphere.com/forums/viewtopic.php?f=35&t=74304&hilit=vesc+solder)

you might find there something usefull, also search the spehere, because there might be even more info...

EDIT: Another link I found: https://endless-sphere.com/forums/viewtopic.php?f=35&t=63540
```

---
## \#7 Posted by: Muke Posted at: 2017-11-25T11:35:00.689Z Reads: 167

```
Thanks a lot guys! I see the diy VESC project more as a fun thing to learn something than a cutting cost mesure.
In addition to that I can produce the PCB parts at university for cheap and I already have a decent soldering iron, I just need to buy a SMD tip.
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-11-27T00:54:48.337Z Reads: 150

```
You'll still need either hot air or a reflow oven to do the DRV chip and the others with pads underneath them.
```

---
## \#9 Posted by: emepror Posted at: 2017-11-27T03:43:03.228Z Reads: 138

```
Hot air is highly recommended for the entire project, its not fun soldering that many components even with a really good soldering iron. 

Its cheaper money wise but not time wise (i got it to $90 a VESC, that being said ive blown 2 of the three ive built)

definitely a fun project if you want to learn about SMD assembly, also helps with learning about the design of the board a little bit. 

@Muke the lab I was able to use at my school had a pneumatic solder paste dispenser and a nice microscope, those were invaluable to me, if your university can make PCB's then you may have access to that equipment too. Definitely worth investigating.
```

---
## \#10 Posted by: Kug3lis Posted at: 2017-11-27T03:46:52.022Z Reads: 124

```
I can tell from experience just having right tools means nothing when it comes to SMT soldering, you also need experience and knowledge for it...
```

---
## \#11 Posted by: Muke Posted at: 2017-11-27T11:04:10.840Z Reads: 107

```
Thank you! I think I will delay this project for a while and gather experience building an electric skateboard with bought parts first.
University will be stressful soon, so I won't have the time to do both project before summer anyway. Maybe this way I will be able to finish the skateboard before the exams start.
```

---
## \#12 Posted by: Muke Posted at: 2017-11-27T11:05:06.478Z Reads: 105

```
Thank you! You helped me out a lot with both of my topics!
```

---

# Open Source Hardware and the VESC derivatives

### Replies: 10 Views: 1430

## \#1 Posted by: akhlut Posted at: 2017-08-18T14:37:09.874Z Reads: 158

```
@onloop @chaka @esk8

Where are the repos for the various derivatives?  I thought I found the design files for the VESC-X/FOCBOX, but the link is dead and for the others I've come up empty.

Given that they all should be carrying the same license as the [VESC](https://github.com/vedderb/bldc-hardware) where are the repos?

VESC is covered under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), therefore the following derivatives should be distributed under the same license:

[Ollin ESC v1.1](http://www.ollinboardcompany.com/product/ollin-esc-v1-1)

[ESK8.de ESK8 controller 1.1](https://store7570530.ecwid.com/#!/Original-ESK8-controller-1-1-mit-direct-Fet´s-Made-in-Germany/p/88140891/category=15255004)

[Enertion FOCBOX](http://www.enertionboards.com/how-to-build-eboard/vesc-x-design-files/)

I'm not asking for the heatsinks - those are proprietary to each of the designs.  Just the PCB design files.

Thanks in advance!
```

---
## \#2 Posted by: chaka Posted at: 2017-08-18T14:41:25.768Z Reads: 152

```
We are all using the original design files and schematics. KiCad is very easy to use and "free", check it out. You might find a whole new world open up if you invest a little time and learn a new skill. ;)
```

---
## \#3 Posted by: akhlut Posted at: 2017-08-18T15:03:43.595Z Reads: 146

```
I know eagle pretty well, and I could pour some time into KiCad.  

But that's not the issue.

If this is [OSHW](https://www.oshwa.org/definition/), where are the design files?  

ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

Not picking  fight here.  Just want to build cool stuff and stand on the shoulders of giants.
```

---
## \#4 Posted by: Deckoz Posted at: 2017-08-19T00:26:38.349Z Reads: 128

```
I think what he means is the base schematic or reference schematic so he can design a board.

https://github.com/vedderb/bldc-hardware/tree/master/design

This should be all you need.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-08-19T01:30:14.171Z Reads: 117

```
I think it all really depends on how much pressure consumers put onto the people who are modifying the source code.
```

---
## \#6 Posted by: gogomrrobot Posted at: 2017-09-17T13:11:49.788Z Reads: 91

```
[quote="chaka, post:2, topic:30966"]
KiCad
[/quote]

Exciting times.  Probably a dumb question as I am a noob to PCB's.  With VESC6 all the gerber/bom files will be released soon is my understanding. Or they are under development by Benjamin.

What does it take to create a workable VESC6 from the hardware design?  You can just send it out to a service that will create a PCB from it with all the components like capacitors, motor wires, and pin connectors ( I don't know what they  all are exactly are -- hall sensors, canbus, etc), USB micro port ?

In fact, is that Trampa's VESC6 essentially minus the aluminum cnc'ed cover/mould ?

I am curious and want to build my own VESC6 but I can't stomach $650 (shipped) for two VESC6's for each build.
```

---
## \#7 Posted by: ThierryGTLTS Posted at: 2017-09-17T14:06:10.498Z Reads: 83

```
You just have to wait.

Frank from Trampa says that that will be released soon.

Thierry
```

---
## \#8 Posted by: Surfer Posted at: 2017-09-17T15:57:33.656Z Reads: 75

```
Yes, take a sit and wait, if you think they will release the files you want, it will not happen, maybe when the vesc 99 is released.
Jason already said, he give enough to the community, he will not release that files, only just a PDF and with this you cannot do anything. Open source for business seems to not work well.
```

---
## \#9 Posted by: akira Posted at: 2017-09-17T16:27:58.749Z Reads: 71

```
That is true for Enertion but not or Trampa/Ben.
They told several times on this forum that a fully fonctionnal HW release of the VESC6 will be done (including a PCB and not only schematics). I also very much waiting for it. 
Maybe Franck has a more precise idea of the release time.
```

---
## \#10 Posted by: gogomrrobot Posted at: 2017-09-17T16:49:27.620Z Reads: 67

```
OK... but see this thread, they quoted Ben says he is working on the reference hardware design right now at the moment.  That was two weeks ago.  I am a believer.

https://www.electric-skateboard.builders/t/vesc-6-released-and-the-forum-is-open/32265

Benjamin writes tonight:

_VESC Tool has been a huge amount of work and there are also many updates and new functions in the firmware. I will work on a reference hardware design in the next days. It will essentially be the same as the VESC6, but a square PCB with SMD electrolytic capacitors, mounting holes and a few other changes. It should work as a PCB only and not require a case for mounting. Hopefully people can adapt it easily if they want to make different cases_
```

---

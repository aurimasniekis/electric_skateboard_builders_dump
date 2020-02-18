# DieBieESC-HiAmp based on VESC6 HW

### Replies: 13 Views: 2953

## \#1 Posted by: JTAG Posted at: 2017-08-16T21:23:26.373Z Reads: 343

```
To complement my open source [BMS project](http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639) I am designing an opensource waterproof Hi-Amp version of the VESC6 for use in my higher current demanding and rough for electronics electronic vehicles ( E-scooter and boat ). 

I want to improve / add the following features:

* Higher current capability 
* Add fuse to power path
* Waterproof
* Isolated CAN interface
* EMC filter CAN interface
* Rugged data and power connectors
* ESD safe
* Analog input filtering

I have split the hardware in two parts to keep the PCB cost low and the whole assembly "compact". The main board that carries all power electronics will look a bit like this:

<img src="/uploads/db1493/original/3X/d/a/da3569e4386e0231cddd28f8ef83fde2612d7242.png" width="690" height="380">

<img src="/uploads/db1493/original/3X/5/8/585691c797aba69becd0a05b622b94f5f98510e2.png" width="690" height="378">

The buffer / top PCB will look like this:

<img src="/uploads/db1493/original/3X/1/0/10a21c86442fc9a2ab3488ecee592647d5a76a72.png" width="690" height="376">

<img src="/uploads/db1493/original/3X/b/d/bd86d73554a1cf72c3d27a75b4d85fc0d7d10c92.png" width="690" height="380">

And both boards combined:

<img src="/uploads/db1493/original/3X/6/b/6b38e7fe1c4058a13edf5c485788d52567c89768.png" width="690" height="378">

<img src="/uploads/db1493/original/3X/b/2/b297158a0bdc22d05b1f0a0ab5138f1918cd3d63.png" width="690" height="380">

<img src="/uploads/db1493/original/3X/8/d/8d28a618998cfe63aa4cdd2d56e5df3eeb2795d8.png" width="690" height="380">

Eventually everything will be potted like [these guys](http://www.sinusleistungssteller.de/Menue_SLS.html) did:
<img src="/uploads/db1493/original/3X/3/e/3ee99cfc94f81ab585d0a53a183da8822622a260.png" width="345" height="230">

If you see I overlooked something please point me to it and ill try to fix it :smiley:.
```

---
## \#2 Posted by: akira Posted at: 2017-08-16T21:26:53.885Z Reads: 315

```
Damn'it !! You're also going to watercool it ??
This is the real thing !! 
Great project !
```

---
## \#3 Posted by: JTAG Posted at: 2017-08-16T21:33:11.340Z Reads: 311

```
Yes! That's the plan for the boat :innocent:.
```

---
## \#4 Posted by: hexakopter Posted at: 2017-08-19T22:47:42.242Z Reads: 290

```
[quote="JTAG, post:1, topic:30829"]
If you see I overlooked something please point me to it and ill try to fix it
[/quote]


Don't you think the total gate charge of two parallel IRF7749 MOSFETs is to much for the DRV830X? I know from calculations back in the days that with the IRFS7530 the MOSFET driver was really at its limit, when not slightly over its limit. So the Direct FETs have a lower total gate charge then the D2Pak's from the "old VESC design", but two in parallel result in general to a total charge higher than the IRFS7530's.
Haven't looked deeper in your design, but that is the first thing I noticed. Maybe it would be a good idea to use different MOSFET driver like for example rew and raphael did in their designs. That would also open the possibility to go with a higher voltage like a max of 80V or so when also the other parts are designed for that.
When I remember correctly the Toshiba TPW1R306PL looked quite good for me with a lot lower gate charge and smaller, so maybe more than two in parallel should be possible.
```

---
## \#5 Posted by: JTAG Posted at: 2017-08-20T18:58:47.914Z Reads: 272

```
Thanks for responding, always nice to hear the thoughts of a colleague VESC like HW designer! The field of power electronics is so big that it is easy to overlook some limitations.

Yes, the total gate capacitance will be about 35% higher with this ESC design with respect to the VESC4.
The VESC on the old VESC the worst case total gate capacitance is 438nC (single IRFS7730), with my design I plan to implement a dual IRF7749L2 resulting in a worst case total gate capacitance of 600nC. 

I think (and hope) it will work because of the following reasons: 1) I will respect the max current output of the DRV by using 10R gate resistance per FET instead of the usual 4R7. 2) I accept the higher required deadtime and the possible lower allowed switching frequency. I plan to use this ESC with low ERPM setups so that wont be an issue. 

In the future I would indeed like to experiment with a different FET driver and possibly go to higher voltages, for now I first want to match the performance of the VESC6 and hopefully maybe even exceed the current specs. 

Over the period of the coming couple of days I will hopefully make some serious progress to finalise the PCB design. I cant wait to get some physical experience on motor control.
```

---
## \#6 Posted by: Mikeomania12 Posted at: 2017-08-21T17:01:42.992Z Reads: 240

```
This is amazing. Cant wait for the day i get my hands on this one
```

---
## \#7 Posted by: thisforumisretarded Posted at: 2017-08-21T20:35:03.824Z Reads: 230

```
very nice!
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-08-21T21:31:17.878Z Reads: 226

```
This thing is looking amazing, and crazy beefy! Though im curious as to why you need so many capacitors, it seems a bit excessive lol. Also @hexakopter the TPW1R306PL looks like an amazing and cheap fet!
```

---
## \#9 Posted by: jlcortex Posted at: 2017-10-15T21:14:01.652Z Reads: 216

```
nice project, has you build and tested this design?
```

---
## \#10 Posted by: Steve-81 Posted at: 2017-10-16T10:15:07.149Z Reads: 208

```
I'm curious too where this projekt stands. I'm already looking forward to get the BMS in my hands, so now I would love to see where the ESK projekt is going to :)
```

---
## \#11 Posted by: lrdesigns Posted at: 2018-09-27T03:02:15.485Z Reads: 144

```
Did this project make it to prototype stage? Its really cool. I'm sure everyone wants to see an update if there is any.
```

---
## \#12 Posted by: JTAG Posted at: 2018-09-27T06:25:11.246Z Reads: 139

```
Yes some progress was made, but also quite a few insights where gained. First the progress! 

(I only made the capacitor board for now, had now big inspirations to solve the power electronics problem yet because the copper thickness I think I need are not available in the regular pcb productions).

![IMG_20180905_145308|666x500](upload://dMdcXHmipoXHZWVdvsdvhqAK23P.jpeg) 

![IMG_20180905_145318|666x500](upload://i4uQZ7mTDw33y4HHiDXkqJ02N5h.jpeg) 

The shown power terminals are a recent release of wurth, by pressing down on the plastic the wire terminal can be removed. They spec them up to 120A, I intent to use them for development only.

The frist images are a mocup of what I thought was the best approach to solve the cooling of the fets and shunts, I am / was still struggling with the heating of the PCB at these currents. I am still looking for a way to solve that, likely with aluminium substrate PCB's (does anybody know a company who can make single layer aluminium substrate pcb with copper anywhere between 200um to 400um or more?).
```

---
## \#13 Posted by: gecko242 Posted at: 2019-02-07T16:54:42.303Z Reads: 68

```
Hey this is awesome! I had plans for a similar project. I got to the point of assembling boards but faced some issues getting it up and running and havent had the motivation (or budget) to keep going with it since. 

Have you made any more progress? I would be willing to lend a hand on the design side if that will help?

On a side note, those wurth terminals are awesome, we had the rep round at work and he dropped off a few sample boards of all of their redcube terminals.
```

---

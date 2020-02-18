# Hacking a cheap dual motor ESC to work with 10S

### Replies: 21 Views: 632

## \#1 Posted by: Mike_Lemon Posted at: 2018-09-10T22:22:12.546Z Reads: 139

```
Hello, 

I've bought one of those ESC's a while ago:

[Cheap ESC](https://teemoboard.com/products/esc-mother-board-for-electric-skateboard)

and knowing these work with 10S I inspected the hardware and realized these can also work with 12S so out of curiosity I've connected em to one of my 12S batteries and yes this does work but has it's own glitches I believe because of the software and all current measurements so my question is if someone has experience with does such things:
 
what components to you have to replace(probably some resistors) to make such a thing work with 12S of even better how'd you change the software to be compatible with that?
```

---
## \#2 Posted by: Battosaii Posted at: 2018-09-10T22:27:53.727Z Reads: 128

```
The software on those cheap esc are locked by the manufactures. You can't adjust them at all.
```

---
## \#3 Posted by: evoheyax Posted at: 2018-09-10T22:27:56.826Z Reads: 125

```
What you posted is an esc, not a vesc. A vesc is a specific platform of esc.

In terms of modifying it, your better off going with an open source esc, such as the vesc. That source is closed, so good luck modifying it. On top of that, the performance gains and other control you gain from an open source esc like the vesc is priceless.

It’s getting cheaper and cheaper for a dual vesc. And will just keep getting cheaper
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2018-09-10T22:32:11.909Z Reads: 112

```
Hardmods are sexy 😃 if only it was dirt cheap to mess with
```

---
## \#5 Posted by: Mike_Lemon Posted at: 2018-09-10T22:34:49.195Z Reads: 110

```
Took a note and edited didn't noticeI typed VESC in the title.

The Vesc is the worst open source platform ever.... 
the thing just constantly fails every 2 meters of riding for everyone around the globe from all manufacturers and it still super expensive and will ever remain dues to the bad component decision and 4 layer board design(which doesn't give anything sins the wires are soldered on everywhere and won't allow you to stick it flat) 
But I'm sure there is a way to maybe change the shunt or some voltage sense resistors on this board somewhere and that's why I'm asking the community to check if someone has some experience with doing such a thing on that ESC without spending hours of reverse engineering.
```

---
## \#6 Posted by: Mike_Lemon Posted at: 2018-09-10T22:36:08.781Z Reads: 97

```
Once a single dude on the internet messes with it it is super easy for everyone trust me it's called collab and learning.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2018-09-10T22:37:20.332Z Reads: 91

```
I fell in love with Fusée Gelée
```

---
## \#8 Posted by: Mike_Lemon Posted at: 2018-09-10T22:37:55.755Z Reads: 90

```
Where is it?
```

---
## \#9 Posted by: kalebludlow Posted at: 2018-09-10T22:41:41.510Z Reads: 86

```
Am I the only person that didn't understand most of this?
```

---
## \#10 Posted by: b264 Posted at: 2018-09-10T22:44:23.079Z Reads: 83

```
I'm confused because he keeps referring to open-source but this whole thread is about a closed-source ESC so no, I don't understand much of it at all
```

---
## \#11 Posted by: kalebludlow Posted at: 2018-09-10T22:45:27.788Z Reads: 78

```
Thank you. Thought my brain was broken because I haven't had my morning coffee yet
```

---
## \#12 Posted by: Mike_Lemon Posted at: 2018-09-10T22:49:22.938Z Reads: 78

```
@evoheyax just mentioned the VESC there and why we should stick to it while I explained why you should not.... 

What's so hard to understand?
```

---
## \#13 Posted by: Jmding Posted at: 2018-09-10T22:53:13.718Z Reads: 78

```
Its possible the 10s vs 12s configuration of this ESC is just a shunt across a couple connectors somewhere on the board.  You should try contacting @dickyho and other vendors that sell this ESC and see if any of them know
```

---
## \#14 Posted by: Battosaii Posted at: 2018-09-11T00:02:28.085Z Reads: 74

```
I know my evidence is anicdotal but I've been running very high power through 6 Focbox that I own and 2  Vesc X well over 1000 miles and the only failures I've had from all of them were my fault. Once I blew a drv throttling a motor trying to see what direction it spun with out doing a motor detection in FOC... The other was when I had 2 phase wires touch at a bad time.
```

---
## \#15 Posted by: Mike_Lemon Posted at: 2018-09-11T14:10:56.805Z Reads: 63

```
When I tried to run it on 12S with my hub motors without any load it ran buitifully but actually running it a load on it sometimes gets stuck and even shunts down for a little while
```

---
## \#16 Posted by: Okami Posted at: 2018-09-11T14:17:48.905Z Reads: 65

```
I dont remember where I saw it but max volts were stated as 50v, i think.

So u shouldnt really charge up fully, i think.

On aliexpress I also found same esc for owlboard or other brand and it was listed as only 12A capable, which could be very true. (So 24A total for dual)
```

---
## \#17 Posted by: Mike_Lemon Posted at: 2018-09-11T19:48:02.373Z Reads: 59

```
Still I want the remote to be compatible with that so it can display the right battery lever on the remote.
```

---
## \#18 Posted by: Okami Posted at: 2018-09-18T11:04:51.852Z Reads: 44

```
@Lumaci

In the other thread u mentioned custom firmware and running 12s. 

Mind to share a few more details how u made it work?
```

---
## \#19 Posted by: Lumaci Posted at: 2018-09-18T11:15:23.348Z Reads: 40

```
The exposed PCB ones just need to be resoldered, the old ones has a few spots for different voltages.

The covered one needs to have the firmware tweaked in the factory.
```

---
## \#20 Posted by: Okami Posted at: 2018-09-18T12:18:59.601Z Reads: 35

```
Yeh but they usually state 10s.. and did u get custom firmware personally or someone else had it done ?
```

---
## \#21 Posted by: Lumaci Posted at: 2018-09-18T12:20:09.343Z Reads: 33

```
Yeah ive had custom "made" speed controllers over a little while ago since i got a mate thats making a esk8 rental thing right now and he wants his own custom made boards.


They claim they can even go as far as 13s on the new ones.
```

---

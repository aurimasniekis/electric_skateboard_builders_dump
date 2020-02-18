# First Build - Commuter - WIP - 3Dprint - Gunmetal Trucks - SK3 6374 192kV - 10S2P - FocBox

### Replies: 13 Views: 258

## \#1 Posted by: MadMaxDK Posted at: 2019-05-17T17:11:40.920Z Reads: 96

```
Hi guys,

So this is my first build. I've been lurking in this forum for the past year. My main goal is to design and fabricate most of the mechanical parts myself. I'm almost ready to start assembling everything, but before i have the cnc guys at work fabricate my motor mount, i would love some input from you guys.

I've designed it in Fusion 360, taking inspiration from some of the mounts i've come across. Initially i made the truck mounting ring as a 2 part component to be clamped together, but decided against that. Pressfit with a grub screw seems to be more stable.


![Behind|622x500](upload://mbDw7l4v2tRiExPe9AqUsc2dalm.jpeg) ![front|690x480](upload://proBITjKm3Q0VYeN4nIbtrf5kUS.jpeg) 

https://a360.co/2HDDjxE

For the batteries i took some inspiration from @Winfly. The hardware is going to be a 10S2P setup using LG HG2 Cells. I've got a Bestech bms to handle balancing.

![Battery|542x500](upload://9a40hiJsgCOcwj6Ux8CxwdcTagp.jpeg)  

My current plan is to mount each 2s2p module under the deck using this 3d printed enclosure. Hoping for a semi flexible setup. But the whole enclosure thing is still undecided.

![Battery|371x499](upload://2qXkySLKQDdImAKreiuYneHRdST.jpeg) ![enclosure%20bottom|455x499](upload://6xCllWPGmyLL438b4CnfzrRhCme.jpeg) 

Motor control is handled by a FocBox, and the plan is to reuse an old GT2b remote for control, until i find the time to make one of the arduino remotes on this site. Switching on and off will be done using an XT90 loopkey. I remember seeing a 3dprinted handle for one of those somewhere.

Oh, almost forgot the most important parts, the board is a Rayne Killswitch with Gunmetal trucks and wheels are 97mm reflective wheels from Lazyrolling.

Some pictures of the prototyping proces.

https://photos.app.goo.gl/FW6Vk5qbTa7hqcBw7

https://photos.app.goo.gl/WNdc9ym82YpT5DsN9

https://photos.app.goo.gl/WrKptWdFNgmkdxi78

https://photos.app.goo.gl/4AvTxZ4mNr2dFkY2A
```

---
## \#2 Posted by: Jinra Posted at: 2019-05-17T17:15:19.322Z Reads: 90

```
That mount is guaranteed to break
```

---
## \#3 Posted by: MadMaxDK Posted at: 2019-05-17T17:17:11.524Z Reads: 88

```
Yes, a 3d printed mount like that will never hold up, it's just a mockup before i have it fabricated in alu.
```

---
## \#4 Posted by: Jinra Posted at: 2019-05-17T17:18:28.603Z Reads: 86

```
:+1: Also why HG2s? they're known to be poor performers in contrast to other similarly spec'd cells like 30q's and vtc6's
```

---
## \#5 Posted by: MadMaxDK Posted at: 2019-05-17T17:25:25.566Z Reads: 84

```
I chose the HG2 cells for their higher discharge rate. I bought them last summer, if buying now, i'm not sure i would make the same choice, but for now, it's what i've got.
```

---
## \#6 Posted by: Fraserrazor Posted at: 2019-05-17T17:51:05.836Z Reads: 79

```
![image|602x419](upload://xXSgqVB7RvbNjZ8v9j9u8kbz91Z.png) 

I would still be wary of these sections of the motor mount design. What grade of aluminium do you intend to use for the motor mounts? Maybe use the stress analysis tool in fusion 360 to check the highlighted areas as I would probably add an extra few mm just to be on the safe side.

One more thing. I would argue that securing the motor mount to the truck using a single grub screw is not the most future proof design, even with hanger profiles like paris trucks. If a single screw fails at speed the motors and mount will both come off worse.

Other than that looks pretty clean, would be cool if you add holes for crossbars
```

---
## \#7 Posted by: brenternet Posted at: 2019-05-17T17:53:09.048Z Reads: 72

```
What do you imagine would happen at those points out of interest?
```

---
## \#8 Posted by: Fraserrazor Posted at: 2019-05-17T18:04:28.114Z Reads: 72

```
I mean hopefully the mount has suitable thickness in which case it won't be such a problem but if you look at the photos there is a step which creates the thin wall. It isn't bad in the short term but I'd rather comment a concern as I know the ebay mounts and less 'beafy' designs are liable to break over a period of time 

https://www.electric-skateboard.builders/t/broken-torqueboards-motor-mount/6205/2
https://www.electric-skateboard.builders/t/revisit-bad-motor-mount-designs/37075
```

---
## \#9 Posted by: Bor.inc Posted at: 2019-05-17T18:22:54.418Z Reads: 62

```
love the deck, I also ride it atm and its so nice :heart_eyes:
```

---
## \#10 Posted by: MadMaxDK Posted at: 2019-05-17T18:24:58.107Z Reads: 59

```
I appreciate your concern and comments! I see what you mean with the lack of material at the end of the mount. I will add a few mm there just to be safe.

For now, the mount is meant for a single setup, but when i upgrade to a dual, i will add some cross bars.
```

---
## \#11 Posted by: MadMaxDK Posted at: 2019-05-17T18:29:15.509Z Reads: 61

```
To be honest, i dont know anything about aluminium grades. My plan was to take it to the cnc guy at the place where i work, and pretty much go with his recommendation.
```

---
## \#12 Posted by: Fraserrazor Posted at: 2019-05-17T18:30:15.871Z Reads: 61

```
Yeah sounds fine just interested that's all :+1:
```

---
## \#13 Posted by: Dirt_Bag Posted at: 2019-05-17T20:20:44.530Z Reads: 50

```
Just spend $20 and order a @boardnamics one, its similiar to your design but a bit better
```

---

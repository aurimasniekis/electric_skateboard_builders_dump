# Relay ON/OFF Switch With No Visible Spark

### Replies: 15 Views: 1454

## \#1 Posted by: darkkevind Posted at: 2017-07-17T16:07:44.684Z Reads: 176

```
Hi Guys,
Just wanted to share my discovery with you. I recently rebuilt my board with a new battery and enclosure and I wanted a new (proper) switch.

I discovered a latching relay that was rated for 120A and has a coil voltage of 24v. I then found a 'centre off' rocker switch which I wired up to the relay. I fed 8s 33.6v (from my main battery) to a linear voltage regulator that steps the 33.6v down to 24v in order to switch the relay. 

Rock the switch one way, it connects and the battery voltage & Amps are allowed to flow through it, rock it the other way and it disconnects. The beauty of it being a latching relay is that it doesn't use any power while it's allowing the current to flow, it's a one-time, power to flick the switch one way or another then it's at rest.

The best part of this, is that (I took the top cover off the relay to expose the components and copper), there's absolutely no visible spark or arc. Fair enough, it doesn't feed the power slowly to the VESC like the XT90 anti-spark switch does, so I could still be potentially damaging the caps, but I was under the impression, if there was no spark or arc, there was no issue. Correct me if I'm wrong.

Anyway, I've been using it like that for about 6 or 7 rides now, turning it off and then on again when stopping for a rest or a snack and it's shown no signs of issues.

<img src="/uploads/db1493/original/3X/7/4/74364e6510b3f047eaca9bc33cf3b9bddc4bfa14.jpg" width="690" height="387">

What do you guys think?
```

---
## \#2 Posted by: TranxFu Posted at: 2017-07-17T17:14:17.217Z Reads: 162

```
its hard to find an actual relay that is not crap in the intertwebs without spending too much. If you have the space and actually have a quality relay go for it... But this takes up 2x or 3x the space of an antispark ? 

Personally I think relays,ssr and stuff is over engineering and not needed :)
```

---
## \#3 Posted by: darkkevind Posted at: 2017-07-17T17:30:42.420Z Reads: 154

```
The relay is only the L shaped black object with the white writing at the top of the photo. It's about the same footprint as a vedder anti-spark PCB, but it is a bit thicker.
```

---
## \#4 Posted by: TranxFu Posted at: 2017-07-17T17:42:10.169Z Reads: 149

```
Yep, but the step down regulator also takes up some space
```

---
## \#5 Posted by: smurf Posted at: 2017-07-17T17:48:45.693Z Reads: 136

```
I have looked into relays as the BMS I have is designed to use two of them. They are available in 36v coils. I have noticed when you start calling them contactors the price goes down. I thought that the caps where used to smooth out the voltage ripple not protect the inrush current. Please correct me if I'm wrong.
```

---
## \#6 Posted by: Martinsp Posted at: 2017-07-17T18:09:40.790Z Reads: 127

```
With batteries there is no ripple to smooth out. It is as DC as it can be :D The caps are used as external decoupling for the battery wires.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-17T18:36:59.184Z Reads: 121

```
The step down regulator is tucked underneath the switch there, in the blue heat shrink, it's very small indeed.
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-17T18:38:33.462Z Reads: 121

```
So why, for example, does the xt90 plug let a low rate of current through, then almost immediately the full current/voltage? Is it literally just so that it doesn't spark? I thought it was to protect the components from a surge of current?
```

---
## \#9 Posted by: ShutterShock Posted at: 2017-07-17T18:40:06.076Z Reads: 117

```
Yes it's literally just so that the spark doesn't vaporize the metal on the connectors and cause them to go bad over time, from my understanding of it anyway.
```

---
## \#10 Posted by: darkkevind Posted at: 2017-07-17T18:49:31.154Z Reads: 110

```
Wow, I didn't know that. Thanks :thumbsup:
```

---
## \#11 Posted by: Martinsp Posted at: 2017-07-17T21:18:48.960Z Reads: 98

```
Yeah that is right, it damages the connectors. At 10S it just destroys them :D every time i connected it before i made a proper switch the spark just burnt a piece of my connector :D
```

---
## \#12 Posted by: Charles Posted at: 2017-08-03T22:22:40.881Z Reads: 75

```
Hey I was wondering how you wired your relay .i have been trying to do the same thing <img src="/uploads/db1493/original/3X/b/2/b2bf18209382dea882b75751db36ca4df76245cb.JPG" width="690" height="169"> like that but no luck : I was wondering if you could tel, me if I'm doing anything wrong
```

---
## \#13 Posted by: darkkevind Posted at: 2017-08-03T22:33:00.257Z Reads: 75

```
<img src="/uploads/db1493/original/3X/4/7/47af2c7d5c879e8b05773773442186946419658d.png" width="403" height="500">
```

---
## \#14 Posted by: Charles Posted at: 2017-08-03T22:35:02.497Z Reads: 69

```
what about if you have a bms
```

---
## \#15 Posted by: darkkevind Posted at: 2017-08-03T22:35:58.090Z Reads: 68

```
Doesn't matter, you still have a power source the same...
```

---

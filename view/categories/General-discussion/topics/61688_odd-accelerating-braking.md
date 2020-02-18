# Odd accelerating/braking

### Replies: 12 Views: 384

## \#1 Posted by: Brontech Posted at: 2018-07-12T20:17:13.771Z Reads: 92

```
So I've been having this issue lately, with my board randomly accelerating and braking when out riding. This issue started to appear when I was going though high vibration areas, like in rough pavement and grass, but then started to just happen most rides. The board would start to have a mind of its own and will accelerate for a second, then slow down or brake.
I've insulated the phase wires inside of the enclosure and that got rid of the issue magically for a week or two, but then when I was riding in grass, the issue came back..
I just opened up the enclosure to find all three phase wires fully insulated and there would be no way for them to interfere with each other...

What could be the issue to this?
Any advice would be greatly appreciated :slight_smile:

Edit: Going to try and reinforce and replace the receiver cable to see if that fixes anything..
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-07-12T20:25:30.760Z Reads: 80

```
post your vesc settings, screenshots pls
```

---
## \#3 Posted by: Brontech Posted at: 2018-07-12T22:16:02.799Z Reads: 76

```
Here ya go :slight_smile:
Replaced the receiver wire and changed some setting in the Tool, going to go for a test ride and see if the issue is still there..
![vbn|690x368](upload://5PhMazygEjMlqlpErE24mcBx478.PNG)
![Capturetdg|690x371](upload://nRt0XZjGixFjYUFEi7cBoU71jZ7.PNG)
![fghj|690x375](upload://9NEzbz0tQmGAxUV2nRf6cSTGOyC.PNG)
![fghdgh|690x374](upload://cDohEa17jGAqwN48RRNp4eB3a5B.PNG)
![dhghfh|690x373](upload://hNSUhCz11YH1ohPHyWEScK4v5Fv.PNG)
![dfhgdg|690x379](upload://gKgiyDJWQw9rxGICTSM3dSLpRnl.PNG)
![dhgdghdt|690x373](upload://bRHHgsItp9qUklSUBrZROqdyEwg.PNG)
Let me know what other settings you have to view, thanks!
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-07-12T23:05:58.670Z Reads: 62

```
what kind of battery do you have because in the second screenshot the values seem rly wrong for any kind of battery. Meaning what S count?
```

---
## \#5 Posted by: Brontech Posted at: 2018-07-12T23:08:22.619Z Reads: 60

```
I have 2x 6s 8000Mah Graphene Lipo packs in series.
Throttles when cells reach 3.5V
Hard cutoff when cells reach 3.4V
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-07-12T23:11:38.705Z Reads: 60

```
ok. a bit low for my taste but still tolerable.
is your remote fully charged, maybe the connection is spotty.
```

---
## \#7 Posted by: sayekim Posted at: 2018-07-12T23:17:43.571Z Reads: 61

```
Sounds like the receiver is the problem here. Keep the receiver as far away as possible from the phase wires and battery wires. Also be sure that the receiver plug is in all the way. 

I had a similar problem and it was the placement of the receiver that caused this in conjunction with my focboxes moving around in the enclosure because the velcro strap glue let go from the focboxes when they got hot and it made them move to eventually interfere with the receiver. 

My post about it here: 

https://www.electric-skateboard.builders/t/has-anyone-amped-up-the-meepo-board-hub/51715/40?u=sayekim

And recently I had this problem again but this time it was the plug into the receiver that was getting loose from vibrations. I think I’m going to hot glue that sucker in or use ducttape in the meantime to hold it in place.
```

---
## \#8 Posted by: Brontech Posted at: 2018-07-12T23:30:14.990Z Reads: 55

```
Alright, going to move my receiver to another part of my enclosure and see if this issue persists..
Thanks for the help!
```

---
## \#9 Posted by: banjaxxed Posted at: 2018-07-13T10:43:12.334Z Reads: 47

```
Hot glue down the receiver ports as well, vibration could be shaking them loose

I also took my receiver board out of the little plastic case and used a bit of kapton tape to insulate it and hold it down both on the receiver end and the ESC end

A ferrite ring might also be good to eliminate interference, clamped on the receiver wire
https://ae01.alicdn.com/kf/HTB1UPqPef6H8KJjSspmq6z2WXXa8/5-Pcs-5mm-Clip-On-Ferrite-Ring-Core-Noise-Suppressor-For-EMI-RFI-Clip-Cable-Active.jpg_640x640.jpg
```

---
## \#10 Posted by: lennarn Posted at: 2018-07-13T13:19:37.490Z Reads: 36

```
A little off topic but can you explain how the ferrite ring works?
```

---
## \#11 Posted by: banjaxxed Posted at: 2018-07-13T13:36:06.424Z Reads: 31

```
My understanding is that is blocks electromagnetic interference noise (EMI) steming from the ESC during voltage switching that has a frequency that is well under the 2.4ghz frequency that your receiver operates on, essentially leaving a clean signal
```

---
## \#12 Posted by: BigBrit Posted at: 2018-07-13T13:47:24.808Z Reads: 31

```
A ferrite ring acts as an EMI suppressor. Esentially when you have a wire you have an antenna that can transmit anything thats on it and can receive unwanted RF signals.  The Ferrite ring acts as a low pass filter essentially converting this unwanted RF into heat.

Thats the ELI5 of it anyways
```

---

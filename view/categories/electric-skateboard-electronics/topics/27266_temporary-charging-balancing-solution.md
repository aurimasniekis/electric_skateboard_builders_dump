# Temporary Charging (balancing) Solution

### Replies: 21 Views: 1625

## \#1 Posted by: darkkevind Posted at: 2017-07-10T19:18:53.615Z Reads: 130

```
Just wanted to share my desperation caused by waiting for my BMS too turn up from China.

I've linked up 8 x TP4056's to each cell of my 8s4p li-ion pack I just made using my DIY ATV battery powered spot welder.

Welder:
<img src="/uploads/db1493/original/3X/3/b/3b45741d696e67f9d2a959142ece89230d5a55bf.jpg" width="690" height="388">

At the moment I'm plugging in 8 usb chargers to each TP4056 to balance them, but when they're balanced I'm just using my 33.6v 2A mains charger...

Bit hacky, but I'm so desperate to get back on my board in this sunshine, I can't wait for my BMS too arrive! Lol.

I did try hooking up one 5v 10A power supply to all of the TP4056 boards, but that can't be done without isolating each boards' power supply (it just causes a short).

This is entirely temporary, but if you could be bothered and had the means, this could be a permanent charging solution. You'd just need to carry around 8 usb phone chargers and find 8 spare power sockets in close proximity to each other! Lmao! 😂

<img src="/uploads/db1493/original/3X/8/f/8f3a8d41674d13ae83f03a03ce658a254146c754.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/6/7/6752bf9d6ef7991e06b26cf7c40859879a7e4448.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/9/1/91dcd8c0118cdd48988688db300a712b169451a4.jpg" width="690" height="388">
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-10T21:11:25.398Z Reads: 111

```
This is funny because I bought 50 of the little TP5046 modules and never did anything with them. You may have inspired some science
```

---
## \#3 Posted by: Okami Posted at: 2017-07-10T22:10:44.725Z Reads: 104

```
hah yes, way to go @darkkevind ! I heard about this TP4056 idea along time ago but this is the first time I see someone actually did it! :D

Do you also have a picture of more than one plug connected to the pcbs/sockets of the modules?
```

---
## \#4 Posted by: darkkevind Posted at: 2017-07-10T22:48:20.779Z Reads: 103

```
Yup

<img src="/uploads/db1493/original/3X/a/6/a6c34e9abc161b3a6c715c6ced8f3eb64e8d791b.jpg" width="690" height="388">
```

---
## \#5 Posted by: Okami Posted at: 2017-07-10T22:53:30.335Z Reads: 97

```
hah only 3 so far, it probably looks way crazy when all of them would be plugged in.. would be a big series of wall adapters lined together to charge the cell group / supply the current to each module :)

Maybe some sort of adapter with 4 sockets built into one would be the best for the thing you are doing hah :D
```

---
## \#6 Posted by: darkkevind Posted at: 2017-07-10T22:58:58.700Z Reads: 92

```
I didn't want to go and unplug them from the kitchen and bedroom again! Lol

I did have 8 on there last night. Running off of a double socket in the wall with two, 4 gang extension cords off of those...!🤣

Still... They're balanced beautifully! 😁
```

---
## \#7 Posted by: Okami Posted at: 2017-07-10T23:02:48.800Z Reads: 91

```
Good to hear it performs nicely!

All of the little red lights probably make a nice unison .. especially giving off a good feeling once you see the green light on them hah :D
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-10T23:04:37.240Z Reads: 84

```
Love seeing those green lights :smile:
```

---
## \#9 Posted by: wafflejock Posted at: 2017-07-10T23:49:21.460Z Reads: 81

```
This is awesome and ridiculous have a small pile of these too.  Was just thinking you could tie all the input +/- on those to a bus bar of sorts and give it a power supply with enough amps for all of them to simultaneously charge.
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2017-07-10T23:51:31.604Z Reads: 77

```
yeah, those things take what, 5V1A tops? it'd be pretty easy to rig up a 5V10A PSU and connect it to their power pins.... or am i missing something?
```

---
## \#11 Posted by: Montiey Posted at: 2017-07-11T00:05:22.398Z Reads: 78

```
Hold my beer-

Cheap BMS, here I come!
```

---
## \#12 Posted by: darkkevind Posted at: 2017-07-11T06:43:18.130Z Reads: 70

```
No you can't do that unfortunately because it creates a short of the batteries that are in series.
They need their own isolated power source. You can do that with a DC-DC isolating converter though and one power source.

@faithfulpuppy
```

---
## \#13 Posted by: wafflejock Posted at: 2017-07-11T14:25:15.972Z Reads: 60

```
Hmm I don't understand or you don't understand not sure which one :) the in ports on the lipo chargers are expecting 5V there shouldn't be any power flowing from one to the other each charger would be in parallel with the one next to it so they'd all just have whatever 5V supply you put on there for charging, no?
```

---
## \#14 Posted by: darkkevind Posted at: 2017-07-11T15:06:13.997Z Reads: 56

```
No think about it, each cell, after the first 'balance wire' (which is connected to the positive of the first TP4056), you have the negative of that TP4056 connected to the positive of the next cell (because the cells are in series), so the next TP4056's positive connection is ultimately connected to the negative of the previous cell's neg. Doing this ultimately creates shorts or at least current feedback that the TP4056 boards do not like. I blew 10 of them messing around with this.
```

---
## \#15 Posted by: wafflejock Posted at: 2017-07-11T15:08:27.165Z Reads: 53

```
Gotcha yeah maybe some diodes could work to block the current from flowing back but I guess it's sort of defeating the simple goofy nature of how it is.

Originally was just thinking about the input side where they'd all be parallel connecting.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-07-11T15:14:33.199Z Reads: 54

```
Yeah that's all I thought about at first! lol

You can use one power source though but only if you have a DC-DC isolated converter in line before every TP4056.
```

---
## \#17 Posted by: Hummie Posted at: 2017-07-11T15:21:29.778Z Reads: 59

```
I almost bought a bunch of those. They're   cheap but a lot of work and charge so slow.  
These two things together is cheaper maybe but a lot faster and very simple
http://www.trcelectronics.com/48-volt-power-supplies-chassis-5.shtml<img src="/uploads/db1493/original/3X/1/2/128874f669cc26ac631a0330f1c230b5e3ee5318.png" width="333" height="500">
```

---
## \#18 Posted by: Montiey Posted at: 2017-07-31T12:52:21.951Z Reads: 47

```
You would need one on every pack. I discovered this when my voltage monitor went full nuclear after connecting it to two of my packs with a parallel balance lead- I just needed to use 2 packs that were also in parallel, not on either side of the series.
```

---
## \#19 Posted by: pat.speed Posted at: 2017-11-22T09:32:40.219Z Reads: 36

```
Wouldn't this charger overcharge the batteries? Since the voltage doesn't taper off when the cells reach full charge or does it do this?
```

---
## \#20 Posted by: Hummie Posted at: 2017-11-22T16:05:50.322Z Reads: 29

```
I didn't make this but since the devices are intended for lipo they should be fine.   and do they need to taper? as long as they don't overcharge I think is the important part
```

---
## \#21 Posted by: pat.speed Posted at: 2017-11-23T23:41:29.757Z Reads: 23

```
 I don't know exactly I just assumed they did need to taper off as with hobby style chargers as the batteries start to reach full charge the amps drop down to about 1 amp or less
```

---

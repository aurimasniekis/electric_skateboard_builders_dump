# 10s4p charging using this wire ok?

### Replies: 13 Views: 594

## \#1 Posted by: chickengun Posted at: 2018-10-11T00:52:02.167Z Reads: 134

```
I bought the charging port from my electric scooter (xiaomi m365, see picture) because I would like to use it on a new esk8 build, so that I can use the scooter's power supply to charge a 10s4p battery pack that I will spot welder. The power supply can output 1.7A at 42V DC.
![IMG_20181011_024548|690x279](upload://r1OMsMPREFyXUgGjgFNdwpUtPgT.jpeg)
![IMG_20181011_024559|690x482](upload://wxwzotE9XeBsSMMx279WnXGLXVH.jpeg) 

I noticed the wires are quite thin (written on it: 105 °C, 30 V). I was planning to use the Bestech HCX-D223V1 BMS. You think it's ok to use or do you think thicker wires are better?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-11T01:51:42.926Z Reads: 122

```
thicker wire is always better. i use 22awg for my charger and its perfect. If you have a power supply give it a shot and see if it works
```

---
## \#3 Posted by: baxtred Posted at: 2018-10-11T04:10:20.270Z Reads: 109

```
At 1.7 amps, they should be fine. I am using two wires in parallel of 20 awg for 4 amps to ensure they don't heat up at all. Using a GX12 4 pin plug for charging.

If you have spare wire around, a single 22 awg would be the right specifications for under 2 amps.
```

---
## \#4 Posted by: Holyman92 Posted at: 2018-10-11T15:43:54.044Z Reads: 86

```
Just made this pack last night and it charged just fine. Ownboard uses the same cable

![received_852727888256954|281x500](upload://vAGwZBOTbMePQonScFPUcGj3pF7.jpeg)
```

---
## \#5 Posted by: KrisKraanen Posted at: 2018-10-11T16:39:32.557Z Reads: 76

```
any suggestions for 8s charging? what gauge do i need what plug is good?
```

---
## \#6 Posted by: psychotiller Posted at: 2018-10-11T17:22:36.183Z Reads: 70

```
Those wires are fine with 2a charging. We've used them with a 4 amp 42v charger
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-10-11T17:27:41.954Z Reads: 63

```
doesn’t look like mine... 😂🤔
```

---
## \#8 Posted by: Holyman92 Posted at: 2018-10-11T17:40:59.492Z Reads: 61

```
Urs is next XD I told u I had 1 to make before urs haha don't worry I start working on it tonight... u wanted 10s3p right
```

---
## \#9 Posted by: dareno Posted at: 2018-10-11T19:15:50.539Z Reads: 56

```
That will be fine on 1.7amp, I use a 4amp 12s with the same size and its fine.  Charge it outside of the board first if you're worried.  I always do that as a matter of course to be safe.
```

---
## \#10 Posted by: accrobrandon Posted at: 2018-10-11T19:19:44.639Z Reads: 53

```
heres my 2 cents since i got smart with silicone wire and all that... (rough numbers) 22awg is rated at 8amps iirc, 20awg is 12amps which would be the better choice or at least doubling up the 22awg, a jst connector is rated at 5amps before it gets hot and pushing its limits...

with all that said, and now cuz i have an 8amp fast charger for my board im rolling with my 20awg charge wires and just upgrading the connection from charge port to battery wire w/ 3.5mm bullet connectors supposedly good for 20amps.... and will fit thru the charge port nut. =)
```

---
## \#11 Posted by: b264 Posted at: 2018-10-11T19:25:57.411Z Reads: 50

```
You can use 24AWG for 4A but it's pushing it.  It's better to use 22AWG for 4A.

If you're charging at 1.7A all of them will be fine, but I would still design it to be able to take a 4A charge anyway.
```

---
## \#12 Posted by: GrecoMan Posted at: 2018-10-11T19:40:40.257Z Reads: 44

```
yea 10s3p in that weird ass config we talked about

btw i’m not actually mad haha 🤣🤣
```

---
## \#13 Posted by: Holyman92 Posted at: 2018-10-11T19:57:06.275Z Reads: 40

```
I know haha and alright
```

---

# Where to place antispark switch from the DIYeboard 10s5p battery connected to two VESCs in parallel?

### Replies: 20 Views: 875

## \#1 Posted by: Fraserrazor Posted at: 2018-07-15T15:16:39.609Z Reads: 156

```
![image|690x331](upload://qKcTx0aZn5xyfku7Hyl1cKhCmyH.jpg)

As you can see in the diagram, the switch provided by diyeboard connects directly to their ESC. This, however, is a problem as I am running to VESCs connected in parallel which means only one of the VESCs will have the switch connected to it. Firstly, will this be a problem and if so how where can I cut and place the switch to act as antispark switch for both VESCs?
```

---
## \#2 Posted by: PartyPoison Posted at: 2018-07-15T15:45:02.557Z Reads: 142

```
I think that diagram is ok,
The anti spark is for both vesc,
Wiring goes likes this
Battery output - anti spark - output to parallel vesc...
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2018-07-15T15:46:38.395Z Reads: 137

```
im not sure i understand the issue - if the switch connects to the battery then it should turn the battery on and off, right?
```

---
## \#4 Posted by: Fraserrazor Posted at: 2018-07-15T15:55:25.308Z Reads: 129

```
The diagram is one option. At the moment the switch does not connect to the battery.
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2018-07-15T15:57:15.602Z Reads: 128

```
place the switch between the xt90s on the battery and the parallel connector to the vescs
```

---
## \#6 Posted by: Fraserrazor Posted at: 2018-07-15T16:05:39.178Z Reads: 125

```
![image|388x287](upload://A2lvCZxOjPCAiFUM6a39QKRDY8W.jpg)
```

---
## \#7 Posted by: Fraserrazor Posted at: 2018-07-15T16:06:07.951Z Reads: 120

```
Its a 4pin switch as shown so where should the connections be?
```

---
## \#8 Posted by: faithfulpuppy Posted at: 2018-07-15T16:06:58.781Z Reads: 122

```
wait, is it just a little pushbutton switch or is this an antispark switch that is actuated by a pushbutton?
```

---
## \#9 Posted by: Fraserrazor Posted at: 2018-07-15T16:09:43.421Z Reads: 119

```
The switch is part of the package from DIYeboard 10s5p battery. I asked if it was an antispark switch and customer service said it was. However, I am still unsure.
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2018-07-15T16:11:11.829Z Reads: 114

```
could you please post a link to the battery kit you're referring to?
```

---
## \#11 Posted by: Fraserrazor Posted at: 2018-07-15T16:12:31.765Z Reads: 114

```
http://www.diyeboard.com/10s5p-360wh-18650-battery-power-kit-with-bmscharger-enclosure-p-572.html
```

---
## \#12 Posted by: faithfulpuppy Posted at: 2018-07-15T16:14:21.097Z Reads: 110

```
just that switch on its own is not antispark, it has to connect to some other kind of switch (built into the ESC for DIYeboards) to be able to actually handle the power of an eboard. Sorry :(
```

---
## \#13 Posted by: Fraserrazor Posted at: 2018-07-15T16:15:30.207Z Reads: 111

```
Okay cheers I'll probably do an antispark switch MOD in that case, thanks anyway.
```

---
## \#14 Posted by: BensonYong Posted at: 2018-07-16T10:38:17.452Z Reads: 92

```
![%E9%98%B2%E7%81%AB%E8%8A%B1%E5%BC%80%E5%85%B3%E6%8E%A5%E7%BA%BF%E5%9B%BE4-1%20%E5%B0%8F%E5%83%8F%E7%B4%A0|690x269](upload://jih1X2ax57u6AqO7FULzLcM82qt.jpg)

connect like this diagram .https://flipsky.net/collections/accessories/products/anti-spark-switch
```

---
## \#15 Posted by: Fraserrazor Posted at: 2018-07-16T10:42:29.581Z Reads: 90

```
Cheers, this is what I am currently going to use as my antispark. Thanks for the clear diagram! :+1:
```

---
## \#16 Posted by: Fraserrazor Posted at: 2018-07-16T10:48:18.455Z Reads: 88

```
What would be the advantage of choosing the additional 40A car fuse?
My battery is outputting 50A so I think I should leave this out.
```

---
## \#17 Posted by: BensonYong Posted at: 2018-07-16T11:33:09.262Z Reads: 76

```
The fuse protects the skateboard when a short circuit occurs. There will be very few short circuits, so I think you can get rid of it.
```

---
## \#18 Posted by: Wraith Posted at: 2018-07-16T14:38:33.534Z Reads: 67

```
How does this antispark switch compare to the pricier TB anti spark switch? Not sure which would be better between the two. I’m planning on running a 10s5p 30q wirh a 10s bestech bms but no clear choice yet for a anti spark switch.
```

---
## \#19 Posted by: BensonYong Posted at: 2018-07-19T01:23:37.484Z Reads: 51

```
I don't have a deep research on the TB anti spark switch, but I believe that TB's products are also trustworthy.
```

---
## \#20 Posted by: Wraith Posted at: 2018-07-19T01:27:07.971Z Reads: 53

```
Thanks! I'll definitely consider the TB anti-spark switch. Only thing that may be abit finniky is the TB mounts but otherwise everything else appears to work quite well.
```

---

# Vesc power problem

### Replies: 37 Views: 2804

## \#1 Posted by: Dmsj97 Posted at: 2016-07-08T21:41:44.096Z Reads: 151

```
I can not get any power to my vesc, i have a space cell pro 3. Tell me if i did something wrong<img src="/uploads/db1493/original/2X/c/c009f6958f70962689ad6972d76aa7e37144f506.jpg" width="212" height="500">
```

---
## \#2 Posted by: Dmsj97 Posted at: 2016-07-08T21:42:11.840Z Reads: 148

```
Dont make fun of my solder job btw
```

---
## \#3 Posted by: vitormhenrique Posted at: 2016-07-08T21:43:10.071Z Reads: 146

```
[quote="Dmsj97, post:1, topic:5785"]
Tell me if i did something wrong
[/quote]


At least you need to tell us what you did.....
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-08T21:43:11.656Z Reads: 144

```
Test the voltage of the leads from the space cell while on to make sure it's outputting correctly. Also are those leads for the VESC? they're awfully close to shorting, stick some electrical tape or heatshrink on them.
```

---
## \#5 Posted by: vitormhenrique Posted at: 2016-07-08T21:45:52.444Z Reads: 148

```
[quote="Jinra, post:4, topic:5785"]
they're awfully close to shorting
[/quote]

Yeap, if there are not shorted already, I would not plug this vesc on a battery like this.... 

You need to use electrical tape at least....
```

---
## \#6 Posted by: Dmsj97 Posted at: 2016-07-08T21:52:34.845Z Reads: 145

```
I heat shrinked it, still wont power on, do i have the reciver wires connected correctly
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-08T21:54:26.441Z Reads: 142

```
Did you test the voltage of the space cell leads? The picture doesn't tell us much, can you take a pic of the whole VESC and how the leads go onto the it?
```

---
## \#8 Posted by: Dmsj97 Posted at: 2016-07-08T21:58:53.664Z Reads: 140

```
<img src="/uploads/db1493/original/2X/a/ad64a85f9b84b739b722ff3441b2003a65458211.jpg" width="690" height="327">i really dont know what could be wrong like i think i did everything right, nevermind im retarded i connected + to -
```

---
## \#9 Posted by: Jinra Posted at: 2016-07-08T22:01:25.318Z Reads: 134

```
Oh man, hope you didn't blow out your VESC. The middle phase wire seems like it has some carbon from a short as well.
```

---
## \#10 Posted by: cmatson Posted at: 2016-07-08T22:03:24.037Z Reads: 133

```
Ya, looks like your phase wires touched and blew your vesc.. 

The middle one looks shorted at @Jinra said..
```

---
## \#11 Posted by: Nowind Posted at: 2016-07-08T22:03:38.228Z Reads: 130

```
 Your power wires are black on red on the XT plug !
 This looks not right !
 Also the phase wires are not isulated and maybe shorted !
```

---
## \#12 Posted by: cmatson Posted at: 2016-07-08T22:05:02.322Z Reads: 131

```
Ya it looks like your xt60 is also on backwards mate..
```

---
## \#13 Posted by: Jinra Posted at: 2016-07-08T22:07:39.005Z Reads: 125

```
He mentioned it below the pic :P
```

---
## \#14 Posted by: Dmsj97 Posted at: 2016-07-08T22:17:40.613Z Reads: 123

```
I flipped around and still nothing
```

---
## \#15 Posted by: chipoi84 Posted at: 2016-07-08T22:18:28.257Z Reads: 122

```
You blew the BMS. Everything else is probably fine.
```

---
## \#16 Posted by: Dmsj97 Posted at: 2016-07-08T22:20:13.683Z Reads: 126

```
<img src="/uploads/db1493/original/2X/a/ad64a85f9b84b739b722ff3441b2003a65458211.jpg" width="690" height="327">are the reciver wires connected correctly
```

---
## \#17 Posted by: Jinra Posted at: 2016-07-08T22:20:14.888Z Reads: 124

```
I dont think his BMS blew given there's a 40A fuse on there. He most likely blew his VESC.

@dmsj97 can you check for signs of shorts on the VESC (black marks)? Check the caps too if you can.
```

---
## \#18 Posted by: Dmsj97 Posted at: 2016-07-08T22:20:45.238Z Reads: 127

```
No black marks or anything, no smell either
```

---
## \#19 Posted by: Jinra Posted at: 2016-07-08T22:21:41.513Z Reads: 122

```
Does the space cell still turn on when not plugged in?
```

---
## \#20 Posted by: chipoi84 Posted at: 2016-07-08T22:21:50.612Z Reads: 125

```
No, it is the bms, and possibly the fuse as well. The same thing happened when I was trying to help someone with their setup. I bet if he removed the heatshrink and bypass the bms the vesc will power on.
```

---
## \#21 Posted by: Dmsj97 Posted at: 2016-07-08T22:23:08.345Z Reads: 117

```
The space cell turns on shows a battery voltage
```

---
## \#22 Posted by: chipoi84 Posted at: 2016-07-08T22:24:22.304Z Reads: 114

```
I stand corrected then. I guess the battery and the bms is fine, but not the vesc.
```

---
## \#23 Posted by: Dmsj97 Posted at: 2016-07-08T22:27:06.770Z Reads: 115

```
Well your all wrong everything is fine, just the fuse blew
```

---
## \#24 Posted by: Dmsj97 Posted at: 2016-07-08T22:28:19.498Z Reads: 115

```
<img src="/uploads/db1493/original/2X/a/a36396e2716c7400ab54dd495a85b0aff2ab3774.jpg" width="288" height="500">
```

---
## \#25 Posted by: Jinra Posted at: 2016-07-08T22:29:06.144Z Reads: 114

```
Fuses don't get enough love around here ;) Seriously though, insulate those phase wires.
```

---
## \#26 Posted by: Dmsj97 Posted at: 2016-07-08T22:29:49.516Z Reads: 112

```
Well i still cant get a signal to my remote im gonna need help with that
```

---
## \#27 Posted by: Jinra Posted at: 2016-07-08T22:33:08.042Z Reads: 110

```
are they soldered on the VESC? are any of them shorting?
```

---
## \#28 Posted by: Dmsj97 Posted at: 2016-07-08T22:41:15.334Z Reads: 110

```
<img src="/uploads/db1493/original/2X/c/c009f6958f70962689ad6972d76aa7e37144f506.jpg" width="212" height="500">
```

---
## \#29 Posted by: Dmsj97 Posted at: 2016-07-08T22:42:49.576Z Reads: 107

```
Its solder on and not that i can tell
```

---
## \#30 Posted by: treenutter Posted at: 2016-07-09T03:04:46.758Z Reads: 96

```
[quote="Dmsj97, post:2, topic:5785, full:true"]
Dont make fun of my solder job btw
[/quote]


@Dmsj97 I don't think anyone would make fun. However, it is worth noting that every one one of those soldered connections should be redone. It looks like your iron isn't hot enough, or you're not tinning your wires before you make the connections. Make sure to cover each one of them with heat shrink. Hopefully your VESC survived the short caused by the reversed power connector, and you only need to replace the fuse to get it up and running again. GL!
```

---
## \#31 Posted by: lox897 Posted at: 2016-07-09T07:07:57.444Z Reads: 87

```
Watch some videos on soldering xt60s. That is what I did, it really helps.
```

---
## \#32 Posted by: Dmsj97 Posted at: 2016-07-11T21:20:39.735Z Reads: 80

```
I have no idea what im doing with this vesc, i thought i knew what to do but i cant even find a way to get the bldc tool. I cant get my reciver to work, i give up.
```

---
## \#33 Posted by: Jinra Posted at: 2016-07-11T21:22:59.627Z Reads: 84

```
I programmed my first one this past weekend and it was fairly straight forward. The first obstacle I ran into was that I was accidentally using a micro USB cable without data pins, so you might want to check for that. There's also this if you haven't already seen it

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#34 Posted by: Dmsj97 Posted at: 2016-07-13T19:29:38.676Z Reads: 73

```
when ever i try to connect my vesc to my windows computer it will connect then about 10 seconds later a little read box will appear in the bottom right corner that says no firmware read response. I have no idea what that means. please help me with this god forsaken vesc.
```

---
## \#35 Posted by: Jinra Posted at: 2016-07-13T20:04:16.823Z Reads: 68

```
Where did you get the VESC from? Sounds like it's missing firmware. Go to the firmware tab to flash it.
```

---
## \#36 Posted by: Dmsj97 Posted at: 2016-07-13T20:17:17.904Z Reads: 65

```
Well i tryed that but the whole thing is it wont stay connected
```

---
## \#37 Posted by: Blasto Posted at: 2016-07-14T02:45:35.250Z Reads: 63

```
The microcontroller is probably damaged from having reverse the polarity, the fets-drv probably blown from having the motor leads touching (if you tried running the motor)

That little blue led only means the drv is outputting 5V... Doesn't mean it's not blown.

There's no polarity protection on the input of the vesc... Plus you blown a 40A fuse, that current needed to flow somewhere, dead vesc

For all it's worth, your receiver leads seem to be connected correctly, just add some heat shrink and a tack of hot glue for strain relief.
```

---

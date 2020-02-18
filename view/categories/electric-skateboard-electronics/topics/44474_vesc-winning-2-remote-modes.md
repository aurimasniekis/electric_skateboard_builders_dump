# Vesc Winning 2 Remote modes

### Replies: 11 Views: 594

## \#1 Posted by: Lumaci Posted at: 2018-01-24T01:58:50.255Z Reads: 107

```
Been using this Winning 2 remote for a while, and I noticed it has a lot of different buttons but they all seems useless.

Is there a way I can give them a use? Such as the switch on the back can be used to go from Low Speed to high speed?

And the reverse button, make that one work? It says i can hold it for 3 seconds and it should do reverse but doesn't work.


And also I have a button I can press for 5 seconds that triggers a CH2 mode on the remote that in theory would allow me to do other stuff with Arduino can that be used for something in the vesc?

I'm using Vesc Project latest firmware, and a Vesc 4.12 with Metr and Winning 2.4 remote.
```

---
## \#2 Posted by: Bensaida Posted at: 2018-01-24T01:59:56.453Z Reads: 103

```
same. on my old maytech remote on my echo, speed modes worked like normal, but on the winning v2 remote, speed modes dont work. I would like to know a fix!
```

---
## \#3 Posted by: cwazy1 Posted at: 2018-01-24T02:53:50.602Z Reads: 90

```
1. make sure you do the ppm calibration as soon as you turn on the remote every time. This means turning on the remote, engage full throttle, engage full brake. Then turn on board. 

2. the slow speed/high speed switch on the back just limits ppm pulsewidth. Depending on how your acceleration is setup, it may work, or may not. Depends on if you have current mode/power mode/duty mode.
```

---
## \#4 Posted by: mmaner Posted at: 2018-01-24T02:58:12.312Z Reads: 79

```
You can use the channel 2 button in conjunction with a turning switch to turn lights in and off.
```

---
## \#5 Posted by: Bensaida Posted at: 2018-01-24T03:14:04.224Z Reads: 74

```
link?! 10ch
```

---
## \#6 Posted by: mmaner Posted at: 2018-01-24T03:17:08.593Z Reads: 74

```
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F202128822555

![turnigy reciever controlled switch 072417|533x407](upload://abCpzV0Fo834ksyAwyvhQhSzqqv.jpg)
```

---
## \#7 Posted by: Bensaida Posted at: 2018-01-24T03:17:55.406Z Reads: 68

```
would i need to solder anything? also what does that plug do, the one top right of diagram?
```

---
## \#8 Posted by: mmaner Posted at: 2018-01-24T03:18:56.548Z Reads: 67

```
Yeah, you would need to solder. The plug connects to the on the receiver.
```

---
## \#9 Posted by: Bensaida Posted at: 2018-01-24T03:19:35.567Z Reads: 66

```
i dont have a soldering iron :(
```

---
## \#10 Posted by: mmaner Posted at: 2018-01-24T03:20:54.941Z Reads: 63

```
Talk to @GrecoMan.  I bet if you ordered the pieces, shipped to him, he would solder the connections for a nominal fee.
```

---
## \#11 Posted by: GrecoMan Posted at: 2018-01-24T03:27:34.178Z Reads: 61

```
i’ll do just about anything for a nominal fee 😉

thanks for the shout tho.

@Bensaida PM me if you wanna chat
```

---

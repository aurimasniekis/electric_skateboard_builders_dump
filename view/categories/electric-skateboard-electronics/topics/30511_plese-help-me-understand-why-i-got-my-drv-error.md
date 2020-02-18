# Plese help me understand why i got my drv error

### Replies: 4 Views: 523

## \#1 Posted by: Der6FingerJo Posted at: 2017-08-13T19:10:12.146Z Reads: 88

```
Hi everyone!

Today my esk8.de VESC 4.12 failed on me and i got the DRV error, but i want to understand why that happened before buying my next control or fixing this one.

I'm using a SK3 6374 168KV Motor with 97mm wheels and 48:12 reduction onm 10S. I'd consider my riding style and this setup as fairly efficient, i rarely use more than half of the throttle (still learning how to longboard) and it ran fine for a week in BLDC mode, but sometimes it would stop responding to my remote and i don't know if it was the VESC or my Arduino remote system.

Now today i tried FOC and rode for about 3km slightly uphill and went that same route back with light braking. On the way back i hit a relatively big crack on the street, not that serious that my motor hit the ground but a bit more than the usual bumps in the street and from that moment on the VESC wouldn't respond to my commands anymore and the red LED flashed.

What i want to know now is if those bumps are known to hurt the ESC or if it's more likely to be caused by the FOC.

I am thankful for any input on this! (also on which VESC to buy next, FOCBOX?)

Here is my electronics box under the board and my VESC Settings:
<img src="/uploads/db1493/original/3X/8/a/8ac35eea38278cf9ab5b9a301531e97a318c4705.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/f/bf5285370ac78727ba19b49607ae7eb2ff9e3fca.jpg" width="666" height="500">
The Motor wires aren't under strain when mounted and i don't think they touched somewhere, i'm using MT60 connectors for the motor.<img src="/uploads/db1493/original/3X/4/b/4b7c706ab49e6b29589a174f4527cd2f23286c10.PNG" width="690" height="413"><img src="/uploads/db1493/original/3X/8/6/868fece613b362c90a6ff2b2586809a7e69f4238.PNG" width="690" height="401"><img src="/uploads/db1493/original/3X/1/7/176e2e3210f7b6a67ab3c36212b92484d43664ac.PNG" width="690" height="411"><img src="/uploads/db1493/original/3X/f/7/f742576125eef29598b340e13b93be531166830e.PNG" width="690" height="412">
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-08-14T00:05:45.798Z Reads: 67

```
I think it's either motor is shorted wire or the vesc4.12 is faulty. and fox is not recommended. my vesc 4.12 fried too with no reason. generally I think 4.12 is unreliable. 
go with modified oilin''s, focbox, vesc6.0 
I'm using focbox I just ran 12km non stop with some hills and still works. 
focbox has some fuse to stop drvfault, at least that's what I heard, but I still don't use foc anyways.
```

---
## \#3 Posted by: Montiey Posted at: 2017-08-14T02:04:41.755Z Reads: 58

```
I had my VESC pop a fault after a long while of working fine. I punched it into reverse from a standstill… To this day I refuse to use reverse! That being said, it was the same exact chip that I'd had on the VESC after giving it the 'ol reverse-polarity treatment. If that caused it, the effects were delayed that long.

Sorry, but we can really only tell you what *not* to do (50,000 ERPM limit, maybe no reverse, no FOC). there's nothing that can fix a toast DRV chip other than swapping it. Ollinboard co will repair their VESCs for free or a reasonable charge given the circumstances- where did you buy yours from?
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-08-14T04:07:41.847Z Reads: 51

```
Bought mine from esk8.de but a friend of mine can change the chip for me. Unfortunately I totally fell in love with FOC while using it :sweat:
```

---

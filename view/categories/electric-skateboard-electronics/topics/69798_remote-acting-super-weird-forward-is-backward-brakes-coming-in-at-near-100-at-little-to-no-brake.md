# Remote acting super weird. Forward is backward, brakes coming in at near 100% at little to no brake

### Replies: 12 Views: 224

## \#1 Posted by: kylepls Posted at: 2018-10-02T00:32:14.615Z Reads: 86

```
Title pretty much says it all. I bought an Enertion remote on here a while ago and it's never felt right. First, the brakes come in at near 100% (locking the wheels) (with a rider) when applying the slightest amount of brake on the remote. And the weirdest part is that the remote changes polarity mid-operation (gas = brake and brake = gas). I took a video of this so you guys could better understand. The weird shit happens at **1:36**, the rest of it is just cringy uncensored motor stuff.

https://drive.google.com/file/d/1AN-e4ZlQLB3ulBpJb_tPy_gKHtxZffjx/view?usp=sharing

I really have no idea what's happening here. I'm using the Ackmaniac vesc firmware v2.54. The vescs are connected via a ppm splitter.

Thank you all so much!
```

---
## \#2 Posted by: Holyman92 Posted at: 2018-10-02T00:35:44.758Z Reads: 74

```
can u try running it w/o the ppm splitter and just using the motors individually and see if both vesc produce the same result w/o the splitter?
```

---
## \#3 Posted by: kylepls Posted at: 2018-10-02T00:46:50.375Z Reads: 73

```
Sure thing! I'll have to try that tomorrow though.
```

---
## \#4 Posted by: kylepls Posted at: 2018-10-02T19:13:42.043Z Reads: 48

```
I went without the motors this time and just watched the PPM signal on my computer. I just disconnected the signal wire from the second VESC and went up and down on the throttle for a few minutes until the signal flipped.

https://drive.google.com/file/d/1AGfXE9lCzHfObjUcGBA_TQnlohtJ-uaG/view?usp=sharing

[Link](https://drive.google.com/file/d/1AGfXE9lCzHfObjUcGBA_TQnlohtJ-uaG/view?usp=sharing)
```

---
## \#5 Posted by: kuphjr Posted at: 2018-10-03T01:41:11.602Z Reads: 38

```
I am not that familiar with the Enertion remote, but I know it is similar to many others.  Can you go over the exact procedure you did to pair the transmitter and remote? In what order did you turn on the board, remote or connect the transmitter? Did you need to use a jumper wire to set up the remote?

Also a few pictures of the wiring couldn't hurt.
```

---
## \#6 Posted by: b264 Posted at: 2018-10-03T02:00:00.385Z Reads: 35

```
As soon as you turn the remote on, push all the way forward and all the way backward before you turn the board on.  Does that change anything?
```

---
## \#7 Posted by: dg798 Posted at: 2018-10-03T02:33:41.191Z Reads: 32

```
I was about to post that if no one said anything. I had the same problem and then I saw on the forum that you need to calibrate it before each ride.
```

---
## \#8 Posted by: ShutterShock Posted at: 2018-10-03T02:43:28.719Z Reads: 29

```
Yeah exact same thing here.  If you don't push the throttle all the way forward and then all the way brake before it connects to the receiver, it will act exactly as he says, full throttle and full brake even when barely touching it
```

---
## \#9 Posted by: kylepls Posted at: 2018-10-03T04:39:48.419Z Reads: 23

```
Well, shoot. I went to rebind the receiver and managed to fuck something up. For whatever reason, the remote will now not bind to the receiver. When the receiver turns on it blinks 3-4 times slowly and then goes into the rapid blinking mode (pretty sure that's pairing). Inserting and removing the bind key before turning on doesn't do anything. FFFFFFFFFFFFFFFFFFFFFFFF

For reference, I was following this tutorial.
https://www.youtube.com/watch?v=6PpOspZYh7U

If any of you have a spare nano receiver I'd love to buy it. :slight_smile:
```

---
## \#10 Posted by: threebysix Posted at: 2018-10-03T04:54:33.295Z Reads: 23

```
Does the same problem of rapid blinking and not binding occurring for both ch1 and ch2?
```

---
## \#11 Posted by: sayekim Posted at: 2018-10-03T09:28:15.439Z Reads: 16

```
I was told by enertion support that that rapid blinking is a faulty receiver. I had this problem too. They sent me a new nano-x after a lot of explaining to them what happened.

I would try to use a bind key if you have one to pair it again just in case their answer was wrong.

I had no problem with pairing my old nano-x remote to the new receiver with a bind key.
```

---
## \#12 Posted by: kylepls Posted at: 2018-10-03T15:31:14.177Z Reads: 14

```
Yep. I definitely broke it :(
```

---

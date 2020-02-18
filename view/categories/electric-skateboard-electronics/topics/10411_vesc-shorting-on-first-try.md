# Vesc shorting on first try

### Replies: 12 Views: 1713

## \#1 Posted by: xiniyo Posted at: 2016-09-30T13:50:10.238Z Reads: 143

```
My vesc(enertionboards) burned a bit of the pcb.
On the first test i used a 3s lipo to power up the vesc for testing purpose.
directly the pcb just burned away, see attachment.
just on the other side of the red wire.
<img src="/uploads/db1493/original/3X/5/a/5a917577a356a97d3f68a3d010722810347f5de8.jpg" width="690" height="339">

3s(zippy 3s 30c 5000mh) could be a bit too much power so i tried a 9v battery later with same kind of result(with sparks). used a bit of metal to bridge the gap.

Could anyone point out if there is something wrong on this vesc?

the other side.
<img src="/uploads/db1493/original/3X/4/2/42305228cd030fe36dea11e855fbb7904ae6b007.jpg" width="690" height="313">

There wasn't anything else burning or smoking.

ps. where the red wire is soldered on the pcb was touching the regulator on the left.
```

---
## \#2 Posted by: SORRENTINO Posted at: 2016-09-30T20:22:07.195Z Reads: 111

```
So power was shorting on ground side?
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2016-09-30T21:32:40.481Z Reads: 95

```
<img src="/uploads/db1493/original/3X/1/1/11dc52a906297940bf3664f14fbbd1947aeddf2b.jpg" width="690" height="313">

I'm guessing you saw the sparking at the circled area?

If yes, then that means that you are just shorting out your battery. That solder job needs to be cleaned up, not a big job, but I don't know if you own a soldering iron.
```

---
## \#4 Posted by: RogerD Posted at: 2016-10-01T08:52:32.556Z Reads: 76

```
I reckon he is referring to the underside of the red wire - other side of the pcb. 1st photo, bottom middle just left of the white molex connector, where the solder has burned away all around the base of the cable foot.
```

---
## \#5 Posted by: xiniyo Posted at: 2016-10-03T06:45:55.806Z Reads: 67

```
Yep RogerD is right,
After work ill try to bridge that gap.
i did try to desolder the motor wires, but my soldering iron isnt hot enough.
```

---
## \#6 Posted by: trbt555 Posted at: 2016-10-03T07:04:13.351Z Reads: 68

```
Don't attempt repair yourself.
Another example of shoddy quality, your vendor should stand by his product and offer you a solution.
```

---
## \#7 Posted by: JTAG Posted at: 2016-10-03T14:22:33.830Z Reads: 62

```
I don't know the design of the Enertion CAP PCB but something tells me + / - are the wrong way around somewhere.
```

---
## \#8 Posted by: JTAG Posted at: 2016-10-03T14:24:28.820Z Reads: 60

```
<img src="/uploads/db1493/original/3X/f/e/fe6c35a2deaa7684703eee47a8a34833592d5e5d.jpg" width="500" height="500">

Yep, compare your XT60 orientation to this picture. If you connect the battery again there is a decent risk the caps will pop :P.

Edit: wrong picture xD.
```

---
## \#9 Posted by: Jinra Posted at: 2016-10-03T14:50:07.772Z Reads: 49

```
wow nice catch, the xt60 is totally on the wrong way
```

---
## \#10 Posted by: xiniyo Posted at: 2016-10-03T19:02:11.247Z Reads: 44

```
Keen eye @JTAG
we got a blue light now :smile:
ill make a adapter for it, soon ill test it with the blcd tool.
```

---
## \#11 Posted by: SORRENTINO Posted at: 2016-10-03T19:09:00.560Z Reads: 42

```
<img src="/uploads/db1493/original/3X/b/8/b8f96fedcef565bb55cd0bbbb108eea818cf7bb0.jpg" width="666" height="500">
Should make one of these next time ( smoke stopper ) would have saved you from the shorting
```

---
## \#12 Posted by: sl33py Posted at: 2016-10-03T19:21:30.660Z Reads: 38

```
This was clearly not built correctly.  If there was a surge in connecting this backwards it may have damaged the VESC.  I would connect with @EnertionSupport and see what they say before you swap the connector or try to make an adapter.

GL!
```

---

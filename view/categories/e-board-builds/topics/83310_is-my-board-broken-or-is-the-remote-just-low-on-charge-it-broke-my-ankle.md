# Is my board broken or is the remote just low on charge? - It broke my ankle

### Replies: 13 Views: 273

## \#1 Posted by: MaxMalouf Posted at: 2019-02-06T02:34:32.022Z Reads: 134

```
So about 3 weeks ago I was riding my board which is a:
- dual 6374
-10s4p Sony VTC6
- dual focbox.

I was getting weird disconnects and a few faults were coming up on phone through the Bluetooth module. Anyway, the disconnects seemed like they were gone and I went to floor it, accelerated extremely quick up to about 15kmph then it cut out. After it cut out, it cut back in, throwing me off the board. I landed really awkwardly on my foot and broke my ankle then had to get surgery.

I realised that it could be my remote low on battery as the battery light was flashing on it. However, I was also getting these faults on my phone. I got 2 faults throughout the ride. 

FAULT_CODE_ABS_OVER_CURRENT 
and a DRV fault. (I'll have to get the exact one.)

could these faults be caused by my remote being low on battery? or is it a bigger problem like a loose connection or a broken focbox???

Just a little scared to be testing it, if it was anything more than the remote. 
Thanks
```

---
## \#2 Posted by: CoolRextreme Posted at: 2019-02-06T04:03:42.150Z Reads: 114

```
Look up "FAULT_CODE_ABS_OVER_CURRENT" In the search bar of this forum.
You will find a plethora of information. More then even I know :slight_smile:

It is deff not your remote though. It's the Focbox. I believe (and this is me not knowing a ton about VESC parts) you over-amped your Foc (were you taking any hills or large bumps?)
That would explain the over-current code.

The DRV I THINK does something along the lines of regulating current and/or protecting your vesc. 

All I know is it's definitely the focbox. It MAY be fixable. Use the search on this forum :+1:
```

---
## \#3 Posted by: MaxMalouf Posted at: 2019-02-06T04:21:39.767Z Reads: 107

```
@CoolRextreme yeah ive tried, ill have to just keep reading. i wasnt doing any large hills on the day. i was doing much much more on my previous rides. no large bumps either, i dont recall... real shame
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-02-06T04:34:14.811Z Reads: 96

```
its kinda quarky... ive gotten the error when i got my vesc wet, but may be caused by other things.

says it all in the name "ABS_OVER_CURRENT"

^vesc sensing too much current or atleast over what you configured. can be caused by shorts
```

---
## \#5 Posted by: MaxMalouf Posted at: 2019-02-06T04:36:28.885Z Reads: 92

```
ohh okay, yeah could be that, i will review my wiring and give it all a good check over.
thanks for the help
```

---
## \#6 Posted by: Andy87 Posted at: 2019-02-06T04:41:06.405Z Reads: 86

```
Yeah have a look on your wiring.
Lose connections, bad solder joins (open up your heatshrink at xt and bullet connectors and check that), also check your capacitors on the focbox and the pcb in general. If the capacitor legs are lose that can cause the over current fault too.
The drv fault is probably just what inline with the over current fault after. If the drv fault is permanent than your drv need to be replaced too.
```

---
## \#7 Posted by: MaxMalouf Posted at: 2019-02-06T04:44:11.105Z Reads: 82

```
well i got the abs over current fault maybe 4 or 5 times and got the drv only popped up once.
I will do a full check over the wiring
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-02-06T05:18:45.871Z Reads: 71

```
@JohnnyMeduse this guy knows how to repair vescs 😉
```

---
## \#9 Posted by: dareno Posted at: 2019-02-06T07:12:22.215Z Reads: 51

```
I recently had a similar incident with not so drastic results fortunately.  I pulled away hard and the board accelerated cleanly then stopped.  Felt like it stopped but in hindsight was probably just a cut out.  Under full motion a lack of power when leaning forward can feel like a brick wall.  I thought maybe a connection problem but when I investigated it was a loose connection on my phase wiring.  That loose connection can cause the same fault code.  I had abs notes in the fault log.  Check your cabling and make sure you have everything double shrink tubed.
```

---
## \#10 Posted by: MaxMalouf Posted at: 2019-02-06T07:32:35.269Z Reads: 49

```
@dareno YES that is exactly what happened to me! Except after I hit that brick wall, it applied full power half a second later!

I ended up with the inside of my ankle bouncing onto the concrete while I was basically sitting on the outside of my ankle, hard to explain
```

---
## \#11 Posted by: dareno Posted at: 2019-02-06T07:57:33.537Z Reads: 44

```
Same exact occurrence but I was doing an impression of superman at the time.  Its so hard to trust the machine after a fail that you need to find the issue before you can rely on it.  There will be something physical wrong trust me on this.  When you find it you will be so much more confident on your creation.
```

---
## \#12 Posted by: MaxMalouf Posted at: 2019-02-06T08:09:23.426Z Reads: 43

```
@dareno yeah definitely I wish it was as simple as the remote, I've spent way too much time repairing this bloddy thing
```

---
## \#13 Posted by: dareno Posted at: 2019-02-06T08:20:22.332Z Reads: 40

```
No way!  the remote is the one thing that you need to have utmost confidence in.  I was terrified it was mine.  Once I found the issue I was happy as a pig in shit because I could trust my gear again.
```

---

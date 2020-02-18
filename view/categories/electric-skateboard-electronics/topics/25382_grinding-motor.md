# &lsquo;Grinding&rsquo; Motor

### Replies: 11 Views: 824

## \#1 Posted by: darkkevind Posted at: 2017-06-14T17:42:39.448Z Reads: 123

```
Does anyone know what the grind/judder is with my motor?

If I really soft start it's ok, but even when I'm half throttle, then go full throttle, it sounds like there's an issue with how the power's being delivered to the motor, like there's a mismatch. Imagine the timing being off on an internal combustion engine... That's what it feels like.

Ps. I'm running FOC and have done the necessary detections. (That I know of)

https://youtu.be/UlPGatvHv8M
```

---
## \#2 Posted by: Wolfcola Posted at: 2017-06-14T17:49:59.563Z Reads: 114

```
Is there a pulley on the motor shaft? And does it make this noise in BLDC mode?
```

---
## \#3 Posted by: anorak234 Posted at: 2017-06-14T17:50:38.888Z Reads: 113

```
magnet is probably loose - video won't load for me but I've had this happen before where it's low quality glue holding the magnets and they come loose to grind against everything else. Just try opening it up, and carefully examine the magnets. If one (or multiple) is loose, add a bit of epoxy once you have it back in place and you're good to go
```

---
## \#4 Posted by: darkkevind Posted at: 2017-06-14T18:13:35.873Z Reads: 101

```
I've not tried it in BLDC lately, but it never used to make that noise.

It's only since I got my new VESC, so I think it may just be a setting...
```

---
## \#5 Posted by: arussellsaw Posted at: 2017-06-14T18:14:49.273Z Reads: 95

```
What is your ERPM limit set to? and are you limiting ERPM with negative torque? that has an effect like that as far as i know
```

---
## \#6 Posted by: darkkevind Posted at: 2017-06-14T18:15:03.344Z Reads: 90

```
Is it easy to take the motor can off? It's it just those small screws holding it on? I imagine not as it'll take the shaft out too...
```

---
## \#7 Posted by: anorak234 Posted at: 2017-06-14T18:21:29.371Z Reads: 80

```
I don't exactly remember what it was... but it's like legos - if you document how you take it apart you can always put it back together. Just don't unwind or break any of the copper windings
```

---
## \#8 Posted by: darkkevind Posted at: 2017-06-14T19:04:03.411Z Reads: 79

```
ERPM is set to 60000.

It only does this when I put the power down. Like when I'm cruising, and then throttle further, when it's putting a bit more load on the motor, it does this...

Here are my settings.
<img src="/uploads/db1493/original/3X/f/5/f5642a95b167bce6e776408006ae8c14cbbbc1e6.PNG" width="690" height="328">
```

---
## \#9 Posted by: Hummie Posted at: 2017-06-14T19:57:16.616Z Reads: 66

```
Don't take the screws apart as that'll take the shaft off, just shoot off the c-clip with a screw driver and pull the rotor off.  Watch ur fingers putting it back.  And get ready for the c-clip to launch
```

---
## \#10 Posted by: darkkevind Posted at: 2017-06-15T14:38:46.740Z Reads: 52

```
OK, I've not taken the motor apart yet because I wanted to try a couple of experiments before doing that.

It seems that it's an issue with running FOC. At low current it works fine, as soon as you ramp it up it starts to 'grind' and if you full throttle from zero it's horrific! See my demo videos below....

Running FOC:
https://www.youtube.com/watch?v=w6IYzTdecIA

Running BLDC:
https://www.youtube.com/watch?v=6v222BnhUsc

It seems it's much happier in BLDC so I think I'll leave it like that for now. If anyone has any suggestions about why it's doing that in FOC mode I'd be grateful to hear them. At this point, I'm ruling out a motor problem.
```

---
## \#11 Posted by: TSG_AU Posted at: 2017-06-16T02:54:07.583Z Reads: 38

```
What are your settings under the FOC tab?
```

---

# I have new motors to put on my scramboard turning 6374 149kv do I need to set vescs?

### Replies: 13 Views: 217

## \#1 Posted by: Jcammarata4 Posted at: 2019-04-29T17:19:26.615Z Reads: 77

```
Do I need to re program scramboard vescs from original motors to my new motors or can I just replace and go....sorry kinda a noob at repairs new motors are 6374 149kv......old motors were 6380 250kv
```

---
## \#2 Posted by: Skunk Posted at: 2019-04-29T17:26:13.793Z Reads: 73

```
You'll need to set things up again.  Run motor detection.  What vesc is in the board?
```

---
## \#3 Posted by: Jcammarata4 Posted at: 2019-04-29T17:57:02.941Z Reads: 64

```
Think they are maytec50amp v4.12
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-04-29T19:50:57.976Z Reads: 52

```
they may predate the 50A good on FOC version, it has a super-duper sticker over the Caps
```

---
## \#5 Posted by: Jcammarata4 Posted at: 2019-04-29T23:35:12.926Z Reads: 39

```
Not sure I follow
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-04-30T02:57:26.139Z Reads: 36

```
Maybe an older version of maytech which don’t do 12s foc very well, newer ones have a sticker over the capacitors
```

---
## \#7 Posted by: Jcammarata4 Posted at: 2019-04-30T19:09:23.969Z Reads: 31

```
opened up my board its a maytec super esc 50a will this sync up with my ordered motors which are turnigy 6374 149kv
```

---
## \#8 Posted by: Jcammarata4 Posted at: 2019-04-30T19:13:05.744Z Reads: 30

```
and i plan on running this on my 10s4p battery. sorry for the most likely noob questions but i dont want to make mistakes or lose anymore ride time.
```

---
## \#9 Posted by: Jcammarata4 Posted at: 2019-04-30T19:14:38.714Z Reads: 30

```
please be a YES!! i believe i did research this correctly  ..i think it should be ok..am i right?
```

---
## \#10 Posted by: banjaxxed Posted at: 2019-04-30T22:12:14.775Z Reads: 28

```
You are right, 10s and foc not a problem. You could even go to 12s at some stage
```

---
## \#11 Posted by: rich Posted at: 2019-04-30T22:39:34.285Z Reads: 27

```
[quote="Jcammarata4, post:7, topic:92215"]
turnigy 6374 149kv
[/quote]

Don't forget to use the brass tube which came with the motor. You have to cut it exactly to fill 100% of the gap between motor bearing (6mm below the motor plate) and pulley. It is necessary because the SK8 motor has no circlip to secure the bell and shaft.

According to FOC if it doesn't work with your esc you can accelerate but can't brake (cut off) so don't go downhill, test it at home first time.
```

---
## \#12 Posted by: Jcammarata4 Posted at: 2019-05-01T13:17:44.880Z Reads: 22

```
Awww ya. Great news thank you. I will maybe have a vesc program question or two I assume. Also got a Bt chip from flipsky since I was already gonna be doing surgery. And installed a USB extension port from vesc to exterior of casing.to make it easier to get to  instead of opening up everything .When I receive motors I will post the issues if any. This has been very helpful thank you again.
```

---
## \#13 Posted by: Jcammarata4 Posted at: 2019-05-07T16:04:25.374Z Reads: 13

```
hey i have some vesc programming questions......motors are installed...i set up to my pc....vescs are connected and shows in vesc tool. i did the wizards and they seem to work and save....but motors arent reacting consistantly.....i think i just need someone with a clue to tell me what ive missed here.....can u help please....
```

---

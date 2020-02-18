# Vesc randomly shutting off

### Replies: 8 Views: 829

## \#1 Posted by: GrecoMan Posted at: 2017-08-20T18:30:55.214Z Reads: 101

```
Hello, I know there are plenty of threads about this topic already but I couldn't find anything that could be triggering my problem.  Basically the vesc just feels like it will turn off for a couple seconds randomly.  Sometimes it happens when im accelerating and sometimes it happens when I try to brake, not accelerating hard or braking hard.  Has happened 2-3 times but today was the last straw when I was trying to brake to keep myself from going into an extremely busy street at about 15mph, there was a car behind me and I was forced to jump off and almost get hit by the car behind me.  I'm running the diy vesc, 6s2p epower pack with a single tacon bigfoot 245kv motor.  I don't think it's a motor short because I haven't ever seen any sort of spark from the motor, any help is appreciated :slight_smile:
```

---
## \#2 Posted by: bigben Posted at: 2017-08-20T18:33:57.023Z Reads: 101

```
Can you post screenshots of your vesc settings? That would be a good starting place for folk to help you.
```

---
## \#3 Posted by: Ishayc Posted at: 2017-08-21T10:54:25.107Z Reads: 81

```
I run the same setup and no issues.
Post your vesc settings
```

---
## \#4 Posted by: TehAtheist Posted at: 2017-08-21T13:22:45.860Z Reads: 68

```
What remote are you using?

If you're using the winning remote, you'll neet to setup the failsafe.
Otherwise when your remote has signal issue's (standard for the winning remote :fearful:) and it disconnected, it'll fully break instead of going into "neutral".
You can check for this issue when you're watching the green bar in your VESC settings, disconnect your remote and if the percentage goes to 0, that's your issue.

Otherwise, a bad connection between the motorwires and the vesc (like a loose connector) could cause the same issue.
```

---
## \#5 Posted by: Bataleon Posted at: 2017-08-21T14:18:52.907Z Reads: 60

```
Next time it happens, plug your VESC into your PC (don't restart your VESC), start the BLDC tool, click the "Terminal" tab. Then type in `faults` and click "Send".

If it's a VESC fault, you'll see it shown here.

<img src="/uploads/db1493/original/3X/2/7/2748f32e7c21308320f5d42216506106e5a86a34.jpg" width="690" height="386">
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-08-21T17:08:00.569Z Reads: 49

```
I've got the GT2B.  I think I may have just fixed it by leaving a bit of the reciever antenna out of the enclosure.  I havent tested it yet, but I do know I programmed the vesc to coast if I loose connection so that definitely could have been the problem, will test later today
```

---
## \#7 Posted by: Surfer Posted at: 2017-08-21T17:17:27.407Z Reads: 43

```
Same thing was happening to me, just was a loose tab on the 🔋 and the sparks in that tab are not your friend, almost killed my pack. I hope you find out soon the problem, good luck!!
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-08-21T17:24:14.764Z Reads: 41

```
Oh man, I hope that's not the problem.  If so maybe Dexter will be able to do a repair for me, I've loved everything about this battery so far :confounded:

@torqueboards
```

---

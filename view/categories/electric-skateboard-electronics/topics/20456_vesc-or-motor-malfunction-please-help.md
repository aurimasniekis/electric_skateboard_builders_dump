# Vesc Or Motor Malfunction? Please help!

### Replies: 33 Views: 1552

## \#1 Posted by: Wallgreeens Posted at: 2017-04-06T19:10:27.788Z Reads: 102

```
I have a LHB with that has been giving me this problem.  I have the 12s Li-ion 43v  and just swapped out 2 ollin vescs for 2 Vesc X hoping it would solve the problem, but it did not.  LHB swapped out the vescs and it was working fine for about a mile.  After I fully charged the board this problem began happening again. I tried switching around the motor wires that lead into the board and it worked again for about 10 seconds and then lost most power and went back to this again.  I'm fairly new to this, so any advice would be greatly appreciated.  In the video I am giving the board as much power as it can get.  
https://www.youtube.com/watch?v=zTGIlZ-kTDc
```

---
## \#2 Posted by: Alextech Posted at: 2017-04-06T19:15:18.278Z Reads: 94

```
Loose Phase wire?
```

---
## \#3 Posted by: Wallgreeens Posted at: 2017-04-06T19:20:49.382Z Reads: 93

```
I hope so, which one is a phase wire?
```

---
## \#4 Posted by: Blasto Posted at: 2017-04-06T19:25:49.441Z Reads: 94

```
looks like your traction control is kicking in for some reason... I suspect something is up with the setup that is near the camera (motor pulley vesc)
```

---
## \#5 Posted by: Wallgreeens Posted at: 2017-04-06T19:28:24.496Z Reads: 92

```
Thanks for the advice, what do you suggest that I do?  The motors seem to spin freely when they are not engaged.
```

---
## \#6 Posted by: Blasto Posted at: 2017-04-06T19:33:01.911Z Reads: 87

```
Well, first having the vesc settings will help.

Next, you can disable the traction control on the master so you can know which side is being a douche bag.
```

---
## \#7 Posted by: Wallgreeens Posted at: 2017-04-06T19:41:19.822Z Reads: 87

```
Cool, thanks for the advice.  I'm at work for a few more hours, but that will be the first thing that I do.  I took off the belts after your comment, but I can't get into the board until I get off work.  What program would I use to read the Vesc Settings on a Enertion Vesc X? BLDC tool?
```

---
## \#8 Posted by: Blasto Posted at: 2017-04-06T19:45:16.060Z Reads: 83

```
yes just need the bldc tool
```

---
## \#9 Posted by: Wallgreeens Posted at: 2017-04-06T19:59:21.788Z Reads: 81

```
I spoke with LHB he said "The problem looks like some kind of short, or possibly a loose CAN bus connection. I'm willing to bet its a loose wire."
```

---
## \#10 Posted by: Blasto Posted at: 2017-04-06T20:02:49.375Z Reads: 76

```
[quote="Wallgreeens, post:9, topic:20456, full:true"]
I spoke with LHB he said "The problem looks like some kind of short, or possibly a loose CAN bus connection. I'm willing to bet its a loose wire."
[/quote]

I don't want to undermind LHB, but only one motor would be running if that was the case. 

in this case both motors are running, but slowly, because one of the motors is being held back from the traction control. If you disable the traction control, one of your motors will run like it is supposed to and the other will be sluggish, then we work from there.
```

---
## \#11 Posted by: Wallgreeens Posted at: 2017-04-06T20:23:46.967Z Reads: 77

```
Thanks, your logic does make sense.  I'll be sure to check it out when I get off work.  What I also don't understand is how 2 separate sets of vescs can have the same problem.
```

---
## \#12 Posted by: Mikenopolis Posted at: 2017-04-06T20:39:18.533Z Reads: 76

```
I don't have a solution, but just wanted to comment on my motor's similar behavior

I bought a Raptor that had a physically damaged motor that did the same. After detaching the broken motor, the good motor did that same stuttering because of likely because of traction control.
```

---
## \#13 Posted by: Wallgreeens Posted at: 2017-04-06T20:39:56.088Z Reads: 75

```
You ever get it running?
```

---
## \#14 Posted by: Mikenopolis Posted at: 2017-04-06T20:46:49.932Z Reads: 77

```
yeah. once I disconnected the canbus cable and re-detected the motor with the single vesc, the motor act normal again. that's how I would test your issue if it turns out not to be a simple loose cable. Test each motor on it's own
```

---
## \#15 Posted by: Wallgreeens Posted at: 2017-04-06T20:48:54.000Z Reads: 76

```
Sounds good, I'll try that once I get home.
```

---
## \#16 Posted by: JLabs Posted at: 2017-04-06T21:03:45.422Z Reads: 74

```
If need be you can change over to a servo splitter instead of canbus. You will lose some functionality but people on the forum have better luck with it. I (nock on wood) have not had issues with canbus.
```

---
## \#17 Posted by: Wallgreeens Posted at: 2017-04-06T21:32:35.500Z Reads: 71

```
I'll keep that in mind if I continue to have failures.
```

---
## \#18 Posted by: Wallgreeens Posted at: 2017-04-07T00:33:00.833Z Reads: 66

```
I cracked the board open and plugged one vesc x into the computer using the bldc tool to read.  The first one read just fine and spun like it should.  The second motor plugged into the same vesc was very fidgity and did not run properly.  I also got a bad detection reading.  If anyone has any ideas at this point let me know.  I'm pretty new to this, but I'm thinking the problem may be the motor.
```

---
## \#25 Posted by: JLabs Posted at: 2017-04-07T03:40:35.952Z Reads: 66

```
Please do not create duplicate topics, we try to keep the forum organized.
```

---
## \#26 Posted by: Jebe Posted at: 2017-04-07T03:45:17.102Z Reads: 64

```
pull the motor apart anc remove the heat shrink - check the solder connections between the silicon cables and the motor winding cables. Then re shrink it.
Not sure I would trust that motor anymore.
A. might cause issues with your vescs
B. You might faceplant at speed.
```

---
## \#19 Posted by: Blasto Posted at: 2017-04-07T03:55:56.372Z Reads: 60

```
On the vesc that had the good detection, plug the other motor and do a detection again
```

---
## \#27 Posted by: Wallgreeens Posted at: 2017-04-07T04:05:28.868Z Reads: 57

```
That's some pretty decent logic.  What motor has similar dimensions as this motor and will work on a dual setup with the one enertion motor left.
```

---
## \#28 Posted by: Pantologist Posted at: 2017-04-07T04:09:10.155Z Reads: 56

```
Sounds like the windings are shorting or connected to each other.
```

---
## \#20 Posted by: Wallgreeens Posted at: 2017-04-07T04:09:21.815Z Reads: 58

```
One of the motors works great, but the other was giving me problems.  It was not working at first. Then,  it would work and when I would turn it a little the motor would shoot a spark and stop.  It did that twice, but now it's just working fine.
```

---
## \#29 Posted by: Wallgreeens Posted at: 2017-04-07T04:12:50.652Z Reads: 57

```
That's what I'm thinking.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2017-04-07T04:17:11.007Z Reads: 54

```
[quote="Wallgreeens, post:20, topic:20456"]
It did that twice, but now it's just working fine.
[/quote]

you have a coughing motor, I would stop using it before it causes any more damage. either repair it or replace it. don't leave it as is
```

---
## \#22 Posted by: Wallgreeens Posted at: 2017-04-07T04:26:49.823Z Reads: 50

```
Can I use the enertion motor on 1 side and another brand on the other side?  or would I have to swap both for equilibrium.
```

---
## \#23 Posted by: Blasto Posted at: 2017-04-07T04:29:18.967Z Reads: 50

```
[quote="Wallgreeens, post:22, topic:20456, full:true"]
Can I use the enertion motor on 1 side and another brand on the other side?  or would I have to swap both for equilibrium.
[/quote]

Use motors with the same kv rating, so you can use LHB's red motor.
```

---
## \#24 Posted by: Wallgreeens Posted at: 2017-04-07T07:58:55.947Z Reads: 46

```
I have an  R-SPEC MOTOR and it seems to not function properly.  Originally it was very twitchy as seen in the video below.  I have no disasembled my board and now the motor in question seems to work properly most the time using the blcd tool.  However, when I turn it a little bit, the motor will shoot a spark and stop.  Any idea if the motor is salvageable?  it is an older model moto.  I had read a post from onloop that said there could be extra coil in the motor that I could heat shrink.  

https://www.youtube.com/watch?v=zTGIlZ-kTDc
```

---
## \#30 Posted by: laurnts Posted at: 2017-04-07T07:59:40.154Z Reads: 43

```
@Wallgreeens I've just merged both of your post, please don't double post. Thnx @JLabs.
```

---
## \#31 Posted by: Jebe Posted at: 2017-04-07T08:58:30.438Z Reads: 42

```
try the hobbyking sk3's
```

---
## \#32 Posted by: Wallgreeens Posted at: 2017-04-07T17:45:39.253Z Reads: 28

```
LHB comes through with the awesome customer service.  He is going to swap out the motor for free.  What a guy!  I would never hesitate to order another board from him.
```

---
## \#33 Posted by: Wallgreeens Posted at: 2017-04-27T13:48:58.120Z Reads: 24

```
Put the new motor in and it's been running great so far.
```

---

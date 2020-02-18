# Rode up a 1&rdquo; kerb, motor died. Flipsky 6355 and dual Flipsky 4.2

### Replies: 23 Views: 597

## \#1 Posted by: ervinelin Posted at: 2019-03-31T11:56:39.925Z Reads: 211

```
Hi guys,

This is my dual drive 6" mini AT. Running flipsky 6355 190kvs and dual 4.2. Rode it for 12km in the morning without any issues.

As I was about to ride home after work. In the first few minutes I rode up a tiny kerb (1" or so). Once I cleared the kerb my drive started to cog and sputter.

I had a Bluetooth adapter so I went in and try to see what's wrong. One of the motors just refused to turn properly any more. FOC detection was wonky, hall sensor would not even detect. Wires were intact and didn't pop out. Almost certain the motor itself wouldn't have been impacted because of the clearance with 6" wheels.

Now even with the motor running sensor less it won't spin properly.

Anyone knows what might be the root cause?

Will try to disect it further on the bench but would be good to know where I should be looking.

Thanks!
Ervine
```

---
## \#2 Posted by: Schtekarsten Posted at: 2019-03-31T12:00:46.582Z Reads: 206

```
I would take the motor appart and have a look inside. sounds like your magnets are the source of the problems, or at least could be.
```

---
## \#3 Posted by: ervinelin Posted at: 2019-03-31T12:03:36.194Z Reads: 200

```
If this is the case will the motor spin by hand freely?
```

---
## \#4 Posted by: Schtekarsten Posted at: 2019-03-31T12:17:03.138Z Reads: 197

```
well I guess it depends on alot of factors. if the magnets shattered or not and if they damaged anything else inside or not. when you open it don't try to force a screwdriver into the motor to pry it open. because that can damage the windings when it slips... been there done that. just get rid of the sir clip and open it carefully.
have a look and see if there is a retaining ring for the magnets or not, glue them down if not.
```

---
## \#5 Posted by: ervinelin Posted at: 2019-03-31T13:08:01.166Z Reads: 176

```
Ok this is weird... So on the bench I removed the wheel gear so the motor is free to turn unobstructed.

FOC and Hall sensor detection now seem to work, but the motor just clicks when firing up and doesn't turn at all.
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2019-03-31T13:53:00.856Z Reads: 161

```
Try removing the can and checking out the inside if anything seems off
```

---
## \#7 Posted by: deucesdown Posted at: 2019-03-31T14:12:58.978Z Reads: 156

```
Also try another motor on that esc. Careful though about trying the motor on another esc in case the motor's bad, could kill the esc.

Hmm also try swapping ppm cable.
```

---
## \#8 Posted by: KaramQ Posted at: 2019-03-31T20:34:55.716Z Reads: 135

```
Maybe the wires are loose, same thing happened to me with this one prebuilt with a kicktail
```

---
## \#9 Posted by: ervinelin Posted at: 2019-04-01T07:56:30.451Z Reads: 126

```
So i ran a few more tests.

For some odd reason, motor detection no longer works, neither BLDC or FOC. Either bad detection (BLDC) or R is 0 (FOC).

The red light on the ESC also blinks when I try to run the detection.

Swapping to another motor results in the same problem.

Now I suspect the DRV is blown, how exactly this would happen is beyond me. My only idea is that it was something to do with traction control (it was turned on). 

Anyone else has any ideas before I swap out the ESC for a new one?

Erv.
```

---
## \#10 Posted by: ervinelin Posted at: 2019-04-01T07:56:54.838Z Reads: 120

```
checked, and re-checked... wires were solid...
```

---
## \#11 Posted by: ervinelin Posted at: 2019-04-01T08:06:08.783Z Reads: 120

```
Oh and terminal says FAULT_CODE_DRV

![IMG20190401160605|281x500](upload://7FNIZZ4g5VWCArFbeQLMcIwwVbv.jpeg)
```

---
## \#12 Posted by: mishrasubhransu Posted at: 2019-04-01T09:32:01.626Z Reads: 105

```
So motor didn't die? But the VESC?
```

---
## \#13 Posted by: ervinelin Posted at: 2019-04-01T10:10:35.217Z Reads: 102

```
Seems to be the case... Yes
```

---
## \#14 Posted by: deucesdown Posted at: 2019-04-01T14:03:32.164Z Reads: 96

```
Check for motor short before trying another esc!

https://m.youtube.com/results?search_query=Brushless+Motor+short
```

---
## \#15 Posted by: ervinelin Posted at: 2019-04-01T14:32:43.575Z Reads: 95

```
Nope.. I swapped the motors around (known good motor to bad half of esc first)... Same problem...

Swapped motor on bad side to good esc side. Motor detects and works just fine...

So it's basically a dead DVR or something else on the vesc. What I don't understand is how this would even happen considering how slow I was going and the tiny obstacle I rode over.

I am certain my ERPM limit was set to 60k. Traction control was on if I remember correctly.

The moment I cleared the 1" kerb, the motor started to cog... Then the more I tested the worse it got until now where I can't even get the motor to detect...

I don't even know how I managed to get it to detect on the bench last night.

Do DRVs fail slowly like this?
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-04-01T15:55:44.171Z Reads: 85

```
Drv error does not alawys mean a dead drv, failed detection will cause drv error in the terminal

But don't get your hopes up
```

---
## \#17 Posted by: Battosaii Posted at: 2019-04-01T16:12:47.663Z Reads: 83

```
I've blown a random drv chip like this on a focbox I just had the drv wizzard fix them.up :)
```

---
## \#18 Posted by: threebysix Posted at: 2019-04-01T16:30:42.490Z Reads: 80

```
Is it possible that maybe clearing the 1in curb was enough of a jostle to cause something in the vesc's pcba to fail?
```

---
## \#19 Posted by: ervinelin Posted at: 2019-04-01T16:35:01.955Z Reads: 76

```
What else can cause failed detection?
```

---
## \#20 Posted by: ervinelin Posted at: 2019-04-01T22:58:39.120Z Reads: 65

```
No idea to be honest... Every thing looks intact visually
```

---
## \#21 Posted by: mishrasubhransu Posted at: 2019-04-01T23:06:08.309Z Reads: 64

```
I guess the wheel would have stopped suddenly when you hit the curb and I wonder if that led to something involving high voltage/current causing the DRV failure. I don't know about motors enough so this might be BS.
```

---
## \#22 Posted by: ervinelin Posted at: 2019-04-02T04:48:37.518Z Reads: 53

```
This is along what I suspect as well. But why it would over current or over RPM I have no idea.. I set all the limits up to prevent this.

One other suspicion is traction control was on. Which caused one motor to spin harder than it should have...

Again speculation only...
```

---
## \#23 Posted by: ervinelin Posted at: 2019-04-11T18:54:12.004Z Reads: 41

```
Just an update...

I replaced the faulty Flipsky Dual 4.2 with a new one. Everything works as it should again.

One thing I noticed was that my faulty Flipsky was one of the first generation models, it didn't have the hot glue that held the capacitors in place. Maybe something jolted out of place because of this.
```

---

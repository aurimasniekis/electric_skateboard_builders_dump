# FOCbox Current Spikes (ABS Over current)

### Replies: 9 Views: 265

## \#1 Posted by: bf01 Posted at: 2018-08-30T05:39:33.947Z Reads: 100

```
Hello all,

I'm working on a robotics project that uses two 36v 750w hub motors, and I am (was?) using a pair of FOCBoxes to control them. The battery is 10s7p li ion.

When test driving the robot, I repeatedly ran into ABS over current errors, and when I checked the debug terminal it showed that current was spiking up to 130A.

Is this a problem with the FOCBox or with the motors? The settings on the FOCBox? I've found a lot of threads asking similar questions but I haven't found any with satisfactory answers.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-30T05:43:46.703Z Reads: 98

```
If you read all the threads about that fault you probably already know that. But if not, than
in some cases here that fault appeared when there were bad solder joints or components came lose on the PCB.
```

---
## \#3 Posted by: bf01 Posted at: 2018-08-30T07:14:16.078Z Reads: 84

```
Yeah I found some people say that. I think both of my focboxes have had the problem occur though, which makes me think it could be something else.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-08-30T07:19:11.331Z Reads: 82

```
You have one battery for both focboxes?
If yes check the split plugs.
If no than it’s probably really something else as you say it’s from both focboxes🤔
I once got that faults when driving with connected motor sensor wires.
Was driving two days without sensors than reconnect and never had any problems again
```

---
## \#5 Posted by: bf01 Posted at: 2018-08-30T07:45:23.561Z Reads: 79

```
I do have one battery for both focboxes.

By split plug do you mean the Y cable?

I'm thinking about giving the ODrive a try if it really is a problem with the FOCBox. However I'd have to switch to 48 or 24v motors for that and so I'd rather not, as of now.
```

---
## \#6 Posted by: Silverline Posted at: 2018-08-30T07:47:56.058Z Reads: 76

```
Check the two big caps.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-08-30T08:03:37.002Z Reads: 78

```
yes the xt90 or what ever you use, which make out of one battery connection two plugs for your focboxes.
```

---
## \#8 Posted by: Deckoz Posted at: 2018-08-30T16:48:26.371Z Reads: 59

```
Was it while braking or acceleration?

If it's during acceleration, it is likely the fault of the motor, or a bad motor detection. 

If it's during braking, either your main caps are bad, you have a cold solder in the power lines from the battery, you're using discharge on a bms instead of bypass, or you have a weak series connection in your battery. This would also show a overvoltage fault.
```

---
## \#9 Posted by: strattos Posted at: 2018-08-30T17:02:44.803Z Reads: 50

```
Tagging onto this my experience/question.

If you do your motor detection/sensor detection for foc and decide to rotate the phase plugs (move each one over once) abs over current faults out the whazoo and what sounded like a cogging motor running with no load yet ran fine with load.

This behaviour continued in sensorless mode yet went completly back to normal when I corrected the phase wire orientation to what it was during original motor detection.


Now roughly 250 or so km on the board and there has never been an abs current fault in its "default" (motor config setup) however when I rotated the phase wires I could easily trigger them by just giving a little throttle. 


So I guess something with the motor detection is at play here that dependant on the phase wire orientation. Maybe slightly different lengths of wire? Honestly still doesn't make much sense to me.
```

---

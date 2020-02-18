# Fault code ABS OVER CURRENT

### Replies: 8 Views: 708

## \#1 Posted by: Andy87 Posted at: 2018-06-28T09:40:44.445Z Reads: 123

```
Hey together!
After my yesterday’s ride I charged my battery.
Fully charged I switched on my board and got the fault code ABS OVER CURRENT.
Both motors running without problems. Just always get the code when I switch on my board.
I have seen a lot of other people had the same problem.
So I started my trouble shooting.
I found out, if to disconnect the motor sensors from my master VESC I don’t get any faults anymore.
That means that my motor sensors faulty...
To check this I made a sensored Motor detection but didn’t got any fault from the sensors.
There some numbers written, like
Detected hall sensor table:
-1 2 4 3 6 1 5 -1
But I don’t know for what it stands.
The numbers different from the hall sensor of the second motor.
Maybe somebody can explain me for what this numbers, or why I get that failure code?
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-06-28T15:39:10.923Z Reads: 110

```
I'll hop in here and say I get the same thing at odd times as well. Rarely does it happen when giving full throttle or brake like I'd expect. Either turning on my board, switching from BLDC to FOC, occasionally (very rarely, but happens) when hitting cracks... One time I just changed power modes with ackmaniacs app and rolled the board backwards very slowly a tad bit while it was changing up modes and got the fault.

Luckily I've never had it be an issue.... Im thinking it *may* have something to do with all my power cable adapters to go from XT90 --> XT60 --> single to dual + phase wire extensions... 

But now that you mention sensor wires causing your issue, I might have to look into this as well as being another potential source of the issue. 

I'll probably just be lazy for now until it becomes a real issue, as right now it's more just a nuisance error code with no real side effects... Someone correct me if I'm wrong. I think the highest voltage filtered was maybe 138v, usually it's lower than that though.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-06-28T18:04:18.037Z Reads: 97

```
Could be a cold solder point or some connections become lose a bit.
Strange to hear that it’s appear when you change between foc and bldc.
I read that there was an issue with the Mac version for the ackmaniac firmware (maybe also windows).
The max current ramp step field under advanced motor settings was multiplied by ten. That’s why you needet to set it to 0.004 instead of 0.04.
But as you don’t have the fault permanently I don’t think that’s your problem.

For me just now the question, better to run without sensors?🤔
Can I run in dual mode one motor with and the other without sensors?
Shouldn’t be an issue as long as it’s set in the VESC settings right I guess.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-06-30T10:15:04.301Z Reads: 87

```
I made some more research.
Changed the motors from one site to the other.
No changes. Means the motor sensors ok.
Changed the adapter cable between motor sensors and vesc.
No changes. Means the cables also ok.

As result it only can be the vesc port for the sensor cables...🤔
I opened the cover of my vesc but couldn’t find any bad soldering connection or something else...
So in fact, it needs to be the port on the vesc but...I don’t know how to check that
```

---
## \#5 Posted by: CarlCollins Posted at: 2018-06-30T16:37:47.388Z Reads: 79

```
@Andy87

Have you tried checking your motor and battery settings?
Sometime it appears due to bad settings,

Also on which FW you are?
```

---
## \#6 Posted by: Andy87 Posted at: 2018-06-30T18:14:31.604Z Reads: 67

```
Yes i double checked my settings.
They should be fine and they the same for both vescs.
I‘m on firmware 2.54 with 4.12hw. 
I just was out for a ride. 
Can’t explain why but no faults anymore.
If it will appear after some time I guess it’s really a loose connection on the plug for the sensor wires. Let’s see and hope the best
```

---
## \#7 Posted by: CarlCollins Posted at: 2018-07-01T01:19:27.055Z Reads: 65

```
FW 2.54 has some issues with it try using VESC tool with 3.1xx FW
I hope that helps
```

---
## \#8 Posted by: Andy87 Posted at: 2018-07-01T11:59:18.609Z Reads: 57

```
Thought about it too.
As the guy I bought my vesc from said it’s not recommended to update to 3.xx with his 4.12hw i‘ll wait a bit and look if I get the problem again.
For now all is good.
```

---

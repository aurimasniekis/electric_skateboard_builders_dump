# 11s Lipo, duel VESC 6, 6374 190kv Motor

### Replies: 17 Views: 342

## \#1 Posted by: Volts Posted at: 2018-08-16T15:43:15.683Z Reads: 102

```
I can't find the thread at the moment but someone on here said something about 12s being bad for 190kv motors, I did the calculations from his thread and concluded that 11s at 4.1 or 4.15 max charge per cell was the best for this motor.

Has anyone else here run this setup before that can input their experience, would be appreciated.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-16T15:47:33.291Z Reads: 102

```
Where running 11s LiIon on 190kV.
Was very happy with it. A bit more difficult to get charger and bms but besides that perfect.
The issue with 12s and 190kV is that you could hit the max erpm of 60000 when unloaded on full throttle. That could kill your vesc (if it’s 4.12HW). With vesc 6 up it shouldn’t be an issue. Anyhow you always can set your max erpm Limit in the app to 60000
```

---
## \#3 Posted by: E1Allen Posted at: 2018-08-16T15:48:40.946Z Reads: 92

```
Not even close on vesc6 100k limit.

I can't get above 60k erpm on 12s but terminal said my 190kv were 170kv.  Just limit erpm in vesc settings for hw4.x
```

---
## \#4 Posted by: E1Allen Posted at: 2018-08-16T15:51:06.439Z Reads: 84

```
@Andy87 you beat me to it
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-16T15:54:16.720Z Reads: 84

```
😂...I just mentioned one thing I forgot...12s is with 50.4v fully charged more close to the max voltage the components on the vesc can handle (60v max peak). Shouldn’t be an issue but a bit more buffer from limits never bad ☝️
```

---
## \#6 Posted by: Volts Posted at: 2018-08-17T01:05:23.330Z Reads: 59

```
Thanks guys, Going to change back to 12s setup cause speed is more fun
```

---
## \#7 Posted by: b264 Posted at: 2018-08-17T01:43:55.545Z Reads: 55

```
Running electronic components rated for 60V absolute maximum (VESC 4) on 50.4V (12S) through inductive loads (motor windings) is a bad idea and not safe.

Consumer products usually run at about 60% of their rated max, or, in this case, 8S
So even 10S is pushing the hardware over what you should be.  It's your safety...
```

---
## \#8 Posted by: Volts Posted at: 2018-08-17T01:48:52.714Z Reads: 52

```
I know that Jens runs only 12s on all his systems with the vesc6, and claims to not have problems, 6s and 10s are to slow whats the point in all that work, if I wanted to go slow I'd walk.
```

---
## \#9 Posted by: b264 Posted at: 2018-08-17T01:51:43.062Z Reads: 52

```
If you think 28mph is slow, then go ahead

When I leave, I want to know I'm getting to where I'm going without breaking down or falling off and hurting myself.  If you don't, by all means, do whatever you need to do; it's not my ass :wink:

Also never fall for the "person X did Y, so it's safe" trap.  It's never true.  Look up the "scientific method"
```

---
## \#10 Posted by: Volts Posted at: 2018-08-17T01:53:43.734Z Reads: 46

```
Roger on the scientific process, these things can be programmed to work good even at 12s If I'm not mistaken?
```

---
## \#11 Posted by: b264 Posted at: 2018-08-17T01:54:26.127Z Reads: 44

```
Lots of people have done it and they can be, yeah.  I'm saying you're running the hardware over spec doing that.  Hardware that can kill you if it malfunctions.
```

---
## \#12 Posted by: Volts Posted at: 2018-08-17T01:56:05.759Z Reads: 44

```
Practice makes perfect, when it comes of falling of the board my major concern is the controller failing, have you pushed the VESC 6 to its limits before?
```

---
## \#13 Posted by: b264 Posted at: 2018-08-17T02:00:52.264Z Reads: 41

```
I don't push stuff to its limits because then it breaks more often
```

---
## \#14 Posted by: Volts Posted at: 2018-08-17T02:58:39.022Z Reads: 35

```
What if you run it at 12s with low amp settings?
```

---
## \#15 Posted by: E1Allen Posted at: 2018-08-17T05:10:19.412Z Reads: 33

```
12s is fine. Plus lower amps for same watt output.
```

---
## \#16 Posted by: dareno Posted at: 2018-08-17T07:52:54.827Z Reads: 29

```
Voltage is measured in volts, current is measured in amps and resistance is measured in ohms. A neat analogy to help understand these terms is a system of plumbing pipes. The voltage is equivalent to the water pressure, the current is equivalent to the flow rate, and the resistance is like the pipe size.
So the amount of water coming through is the amps,  the speed with which its coming through is the volts.  If you make it more difficult for the water to get through by decreasing the size of the pipe then you get resistance (ohms) 
You can safely run higher voltages by decreasing your amps but if you want to run more amps then make sure your pipework doesn't restrict it.
If you are using 12s make sure that your set up does not create too much resistance by using lower awg (10) wiring etc and suitable connectors (XT90)
```

---
## \#17 Posted by: Volts Posted at: 2018-10-04T10:50:16.800Z Reads: 20

```
Can I Charge my battery through a bms wthout the vesc 6 being turned off?
```

---

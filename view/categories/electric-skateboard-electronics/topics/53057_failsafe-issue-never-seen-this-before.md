# Failsafe issue? Never seen this before

### Replies: 13 Views: 775

## \#1 Posted by: Mikenopolis Posted at: 2018-04-21T20:26:22.248Z Reads: 158

```
So Jerry at CarvOn offered to upgrade me V3 which has been working flawless in sensors FOC for like 8 months. I got it back and it failed sensor detections even after adjusting the values. 

This morning I was checking the voltage across the sensor wires as he instructed, remote was off to begin with, out of nowhere it went full throttle. I had set the fail safe when working on it and if I turn off the remote mid throttle the motors do stop but this was on the bench and remote was never turned on. So is this something that happens when failsafe (rebinding) is done incorrectly? Never seen this happen before. 

https://youtu.be/ASancp9aV5E
```

---
## \#3 Posted by: pakue Posted at: 2018-04-21T22:58:10.936Z Reads: 120

```
Could the receiver have a different neutral PWM without binding, than the one set in the VESC?
```

---
## \#4 Posted by: Sebike Posted at: 2018-04-21T23:07:51.659Z Reads: 118

```
I had this issue when setting the failsafe (to gradual speed decrease) according to the instructions on the ackmaniac thread. 

But, if no signal from the remote, after about 30 seconds motor went full speed. This happened both with remote off from the start, and if remote was switched off while board was on. 

Could never find the cause of this or how to resolve it, so I disabled the failsafe function.
```

---
## \#5 Posted by: b264 Posted at: 2018-04-22T00:06:56.395Z Reads: 107

```
Are you using the @Ackmaniac firmware?  Which version?
```

---
## \#6 Posted by: Sebike Posted at: 2018-04-22T00:12:12.698Z Reads: 103

```
me? him? who?

if me, yes. whatever the latest version was in november '17 when I tried this feature..
```

---
## \#7 Posted by: b264 Posted at: 2018-04-22T00:35:39.698Z Reads: 95

```
Was asking OP @Mikenopolis
```

---
## \#8 Posted by: Mikenopolis Posted at: 2018-04-22T00:40:56.359Z Reads: 95

```
I might be mistaken as I’m working on three boards. I think this is ackmaniac 2.54? Not 3.1 (I forget the numbers after decimal)
```

---
## \#9 Posted by: Exiledd_Top Posted at: 2018-04-22T02:02:00.331Z Reads: 87

```
I've had similar problems,  my fix at first was ackmamiac  firmware was bassicly saving my ass from falling because my remote went bad try a new remote maybe u have same issue .
```

---
## \#10 Posted by: danielz Posted at: 2018-04-22T03:13:10.395Z Reads: 90

```
I posted about this too only yesterday. Exactly the same problem. Goes crazy after 20 seconds powered on with the remote powered off. Im using latest stock firmware, i think this explains why my board when crazy a few months ago too. I think people dont notice the issue as most turn board and controller off together.
```

---
## \#11 Posted by: rich Posted at: 2018-04-22T04:10:22.047Z Reads: 83

```
This sounds like a nightmare and is very dangerous!
Usaually when I enter e.g. a shop I only turn my remote off but not the board. Because it happened once that I  went accidental full throttle and could watch my board flying into shop-window, lucky that noone got a heart attack including me. But that the same thing can happen with switched off remote is scary!

When I turn my steez remote off and rotate the wheels, there are short strange high frequency noises paired with mechanical resistance each 1-2 turn, not good for coasting. When I turn on the remote everything is fine again. But I prefer this problem over the "full throttle error".
```

---
## \#12 Posted by: danielz Posted at: 2018-04-24T00:14:20.169Z Reads: 63

```
Here we go I confirm the gt2b receiver is the cause. Hooked it up to an arduino. If you power up the gt2b receiver without the controller on after 30 seconds it changes from my custom fail-safe timing valuve of 1330ms to 1500ms. Hence the motors go crazy! 

Now thew question is this by design or have we all got faulty receiever units??? Im guessing people without this problem have the failsafe at around 1500ms so it wont effect them.

Parial solution: Adjust your throttle trim to 1500ms by turning the know anti clockwise should fix this, remember to reset the failsafe too this too. however i can only trim mine to 1460ms, im hoping its enough. I dont thing its acceptable for the receiver to ignore the failsafe adter 30 seconds though

https://youtu.be/Sk8cuHxZtyc
```

---
## \#13 Posted by: Mikenopolis Posted at: 2018-04-24T00:48:28.721Z Reads: 58

```
To what would be have to do to prevent this problem? I’ve never experienced a run away board. I always turn off my remote on extended stops so I don’t accidentally throttle. I feel like I did something wrong instead of the receiver since it’s the same motor, vesc and receiver as before just rebuilding/reconfiguring after motor adapter swap
```

---
## \#14 Posted by: danielz Posted at: 2018-04-24T00:55:24.646Z Reads: 58

```
Adjust your throttle trim to 1500ms by turning the know anti clockwise should fix this, remember to reset the failsafe too this too. however i can only trim mine to 1460ms, im hoping its enough. I dont thing its acceptable for the receiver to ignore the failsafe adter 30 seconds though

EDIT: It was enough, no more worying about run aways.
```

---

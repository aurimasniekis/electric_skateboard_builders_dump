# Help to verify BMS bypass circuitry

### Replies: 13 Views: 375

## \#1 Posted by: Spyke Posted at: 2018-10-16T05:09:48.446Z Reads: 104

```
Hi, I would like to seek for help in the circuitry as this will be my final step with my 12s battery setup.

Appreciate kind inputs and thanks!
![Power%20systems%20wiring|690x388](upload://dPVwjWpdFxyZXgUNkoI2rSUqzvB.jpeg)
```

---
## \#2 Posted by: thisguyhere Posted at: 2018-10-16T05:18:26.012Z Reads: 101

```
looks good to me.

12v Reg.  is that a step down?
```

---
## \#3 Posted by: Spyke Posted at: 2018-10-16T05:22:12.076Z Reads: 99

```
Yep thats for leds, thanks!
```

---
## \#4 Posted by: spesh Posted at: 2018-10-16T07:15:15.914Z Reads: 87

```
What regulator are you using?
```

---
## \#5 Posted by: Spyke Posted at: 2018-10-16T08:11:49.290Z Reads: 84

```
![Reg|500x500](upload://7EeO8M1kjoud782e2uEiJFxiKVm.jpeg) 
This regulator
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-10-16T13:10:40.573Z Reads: 71

```
Just keep in mind that you will need to plug in your antispark to charge it, in the current config. That'll also turn on your vesc.

You could hook it up before the antispark, but then your charge port will always be live.

What I did was have a second antispark plug inline with the negative that leads to the BMS, so that the main battery negative was split (one part goes to vesc antispark, other goes to charge antispark)

That worked out pretty nice because I had two ports right next to eachother, and I didn't have a constantly live charge port.
```

---
## \#7 Posted by: Spyke Posted at: 2018-10-16T14:32:07.699Z Reads: 68

```
Thanks for the reminder, since I’m using the Flipsky VESC 6, the VESC will have a secondary power switch. 
I’m wiring it after the key switch just as u mentioned, I don’t want the BMS to be on all the time.
```

---
## \#8 Posted by: Spyke Posted at: 2018-10-16T14:49:22.089Z Reads: 64

```
 VESC’es will be secondarily turned on by 1 switch for both connected BY CAN BUS
```

---
## \#9 Posted by: Namasaki Posted at: 2018-10-19T23:11:00.075Z Reads: 51

```
What about the balance wires.
If you get the balance wires wrong, you will burn up the bms.

Also, what type of battery Li-ion or Lipos?
```

---
## \#10 Posted by: Spyke Posted at: 2018-10-22T08:43:35.576Z Reads: 44

```
Li-ion, balance plug I’m sure about thus I don’t need to put it in the diagram.
```

---
## \#11 Posted by: Slak Posted at: 2018-10-22T11:11:11.943Z Reads: 35

```
No fuse at all ?
```

---
## \#12 Posted by: Spyke Posted at: 2018-10-22T11:45:59.756Z Reads: 32

```
I built it into the loop key
```

---
## \#13 Posted by: Spyke Posted at: 2018-10-22T16:05:04.308Z Reads: 28

```
The bypass circuit is wrong!!! Please take note, it may even be dangerous!!!

The “B-“ cannot be after the Break Loop Swich, since the balancing wires will have the last wire will function as Negative minus 1 cell count. It will feed negative to all electronics after the break swich negative utilizing only the balancing wire.

If happens that I forget to plug in the Break Loop key/switch and throttle the balancing wire will not be able to handle the amp draw and burn.

Phew! Luckily I have the volt meter, when I plug in my positive terminal without the XT90 break loop and I saw the Volt Meter came on and that’s how I discovered.

Anyways, hope I learn something today.
```

---

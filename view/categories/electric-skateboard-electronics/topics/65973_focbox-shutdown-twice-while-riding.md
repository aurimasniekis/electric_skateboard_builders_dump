# Focbox Shutdown Twice While Riding

### Replies: 16 Views: 288

## \#1 Posted by: mikenyc Posted at: 2018-08-24T21:26:01.613Z Reads: 100

```
Not sure what's going on, the board shut down on me while I was riding twice on separate occasions. Could have gotten seriously hurt, but was lucky enough to run it off both times. 

This happened two times in a row. Both times at around the same SOC (40.1v on a 12s4p 30Q pack). 

When I finally made it home, the board still wasn't powering on. I unplugged the battery connector to check the voltage, and when I plugged it back in, it powered up as normal. 

Any ideas?

Logs:

https://metr.at/r/yilq0

https://metr.at/r/p09Wg

Settings:

![09%20PM|690x470](upload://oePabAF5ogKrQpEzXPLV8XnQ4vX.png)![29%20PM|690x467](upload://znlpaSY98lvpfeHQznk3VEx6CO.png)![46%20PM|690x478](upload://bN4UiHrCirl0TJM7xlcK5FtYQBo.png)![08%20PM|690x481](upload://bjYafZrfO8QeHgKWLOdUTIHdUot.png)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-24T21:41:57.352Z Reads: 81

```
To which voltage you set your battery cut off?
In the first log you have a undervoltage fault at the end.
In the second log you got a drv vault in the end.

Now everything running fine again?
Could be a lose or bad plugged xt90 🤔
```

---
## \#3 Posted by: mikenyc Posted at: 2018-08-24T21:43:56.184Z Reads: 81

```
Voltage cutoff starts at 36v. It's the default @Ackmaniac setting for 12s. Don't mind the undervoltage fault, that comes up when the power drops off at the end. 

All that's visible are the blue lights on the focboxes. The remote and the metr module don't get any power.

I'm wondering if it begins to sag and then the vesc shuts down? Is that expected behavior?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-08-24T21:46:45.513Z Reads: 81

```
That’s what I thought about the undervoltage fault too.
But what about the drv fault?
Still actual?
Did you check all your connections and solder joins?
```

---
## \#5 Posted by: mikenyc Posted at: 2018-08-24T21:48:45.102Z Reads: 78

```
Yes, I checked everything. I just did some test runs in my apartment and was able to replicate. 

https://metr.at/r/dnmT0

https://metr.at/r/kIwbA
```

---
## \#6 Posted by: Andy87 Posted at: 2018-08-24T21:49:38.030Z Reads: 71

```
What’s the cut off end?
In the first log you at 35v than it shut down.
Second it’s for sure not because off vesc cut off
```

---
## \#7 Posted by: Battosaii Posted at: 2018-08-24T21:53:02.545Z Reads: 71

```
Maybe there is a problem with your battery. Could have spot welds that have broken off.
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-08-24T21:57:25.440Z Reads: 70

```
if metr and received didn't get power but blue led shines then means somewhere some 5V tracks are fucked in pcb. But if also blue light doesn't shine it means DRV buck converter is dying or something from similar story
```

---
## \#9 Posted by: mikenyc Posted at: 2018-08-24T21:57:46.800Z Reads: 70

```
I think it's the BMS. I checked the voltage directly on the pack, it read 40.1v as expected. I checked the power on the output of the antispark and it reads 4.09v. Weird
```

---
## \#10 Posted by: mikenyc Posted at: 2018-08-24T21:58:30.704Z Reads: 68

```
Problem seems to go away when the battery is charged up.
```

---
## \#11 Posted by: Battosaii Posted at: 2018-08-24T21:59:37.658Z Reads: 61

```
That's very strange. So is the BMS is not producing the proper voltage then it should be pretty cut and dry, new BMS is needed.
```

---
## \#12 Posted by: Kug3lis Posted at: 2018-08-24T21:59:47.988Z Reads: 61

```
Looks like not opened mosfet at 4V, check maybe some resistors on BMS are fcked from vibrations and cracked solder joint or etc stuff
```

---
## \#13 Posted by: mikenyc Posted at: 2018-08-24T22:04:44.981Z Reads: 58

```
It's the bms. Damn. 40.1v goes in, and 4v is coming out :roll_eyes:
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-08-24T22:05:40.368Z Reads: 57

```
Also check if ur BMS has switch if switch wires are okay...
```

---
## \#15 Posted by: mikenyc Posted at: 2018-08-24T22:06:25.885Z Reads: 55

```
It's a battery supports bms. I have an extra. I'll pull it out tomorrow and examine. 

Thanks for the input guys!

Edit: Weird, just checked the output of the bms. It reads 34v +/-. Pack still reads 40.1v
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-08-25T16:15:48.858Z Reads: 24

```
I had the same thing was the BMS was off without Vesc’s plugged in but it was fine once I turned on the BMS or plugged in vescd
```

---

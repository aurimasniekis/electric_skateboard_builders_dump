# LEDs and resistors

### Replies: 19 Views: 302

## \#1 Posted by: MrDGOrman Posted at: 2018-11-05T10:08:41.432Z Reads: 115

```
Hi everyone,

I've got an LED on off switch which has a max of 3v. The battery pack is 37.8v. Could someone talk me through what resistor I need?

This is the switch I've got:
https://www.ebay.co.uk/itm/12V-4-Pin-12mm-LED-Light-Metal-Push-Button-Latching-Power-Switch-Red/282970899769

Do I need more than 1 resistor? I can't imagine there's 1 resistor that will do from 42v to 3v!? Any advice would be really appreciated.

I'd probably want to get a small PCB as well to wire everything in. Recommendations appreciated.

Cheers,
Daniel
```

---
## \#2 Posted by: L3chef Posted at: 2018-11-05T10:12:06.150Z Reads: 107

```
Got a vesc? Or an extra chanel on the reciever? I take my power from the reciever to the led button
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-11-05T10:14:30.330Z Reads: 102

```
I've got a FOCBOX. Would that work?

How would I wire it up?
```

---
## \#4 Posted by: L3chef Posted at: 2018-11-05T10:16:25.018Z Reads: 95

```
Yeah that will work. Take Gnd and 5v+ from uart port
```

---
## \#5 Posted by: MrDGOrman Posted at: 2018-11-05T10:34:25.647Z Reads: 90

```
But the LED is rated to 3v? Wouldn't it blow?
```

---
## \#6 Posted by: b264 Posted at: 2018-11-05T10:36:48.622Z Reads: 85

```
LEDs are rated only for current (Amps) not voltage.  You can drive them with any voltage.  But the bigger voltage will push more amps unless you slow its roll with a bigger resistor.

If an LED does have a forward voltage rating, it's only the voltage at which you don't need a resistor.  Above that, you still do.
```

---
## \#7 Posted by: MrDGOrman Posted at: 2018-11-05T10:40:02.605Z Reads: 84

```
Okay so long story short, the UART positive should be fine because that is designed to only dish out a small amount of Amps, right?
```

---
## \#8 Posted by: b264 Posted at: 2018-11-05T10:41:41.468Z Reads: 81

```
It will likely need a resistor.  Try 1000 ohms to start.  Measure the current.  Compare it to the LED's spec sheet.

If running from the high voltage from the battery, try starting with 10,000 ohms and checking the current.  You'll probably have to decrease it to brighten it up to its specified current rating.
```

---
## \#9 Posted by: MrDGOrman Posted at: 2018-11-05T10:51:03.150Z Reads: 77

```
I haven't done systems like this in ages. Is there a tool online anywhere that will help me know what resistance level I should aim for? It's been about 11 years since I did "systems and control" at school!

Better yet, is someone on here able to make one for me and I'll buy it off them?
```

---
## \#10 Posted by: b264 Posted at: 2018-11-05T10:52:09.182Z Reads: 74

```
You need to know what current the LED is rated for, what the forward voltage drop is, and the voltage you want to run it at.  From those 3 you can calculate all the numbers.  Those first two you must get from the LED manufacturer.
```

---
## \#11 Posted by: MrDGOrman Posted at: 2018-11-05T10:52:50.430Z Reads: 69

```
The only information I've got is on the ebay link. Only states voltage :(
```

---
## \#12 Posted by: b264 Posted at: 2018-11-05T10:54:09.442Z Reads: 70

```
Then I'd run it from the 5V on the VESC and put a 470 ohm or 330 ohm resistor in series and call it a day.  Those are guesses and could burn it up, but I doubt it.
```

---
## \#13 Posted by: MrDGOrman Posted at: 2018-11-05T11:12:57.288Z Reads: 66

```
Honestly I'd rather have it come straight from the battery and then resist down. I plan to have a little "hub" which will have all my extras wired into. The hub will be between the battery and the FOCBOX. Each accessory is going to be wired into the hub and then resisted down to suit. Like this:

![accessories%20hub|690x354](upload://kleM2OmF9WkAeac9sCRgCaUfH1B.png) 

The hexagons are resistors
```

---
## \#14 Posted by: mmaner Posted at: 2018-11-05T16:55:04.019Z Reads: 54

```
![latching%20switch%20-%20how%20to%20wire%20v3%20022718|690x433](upload://zzcMWwwzNcfaQ1PC4ZLLhDp4wMH.jpg)
```

---
## \#15 Posted by: MrDGOrman Posted at: 2018-11-05T21:37:20.032Z Reads: 46

```
I'll do that as a temporary. I'll have to fit a resistor like @b264 said though.

Thanks!
```

---
## \#16 Posted by: b264 Posted at: 2018-11-05T22:01:53.088Z Reads: 42

```
Maybe.  Without spec sheets, it's not possible to tell
```

---
## \#17 Posted by: MrDGOrman Posted at: 2018-11-05T23:22:22.237Z Reads: 38

```
For arguements sake let's say we don't have a spec sheet. How would I test the switch to find out what voltage I require?
```

---
## \#18 Posted by: pat.speed Posted at: 2018-11-05T23:32:26.766Z Reads: 35

```
Start at 3v and increase the voltage a tiny bit using a variable supply until you achieve the desired brightness
```

---
## \#19 Posted by: MrDGOrman Posted at: 2018-11-10T09:17:08.499Z Reads: 28

```
So I've ordered an adjustable resistor box of eBay. Input voltage of up to 45v and minimum output is 1.25v. I'll see how I get on with that!
```

---

# Help&rsquo;s needed on 12s4p, dual 6355 setup

### Replies: 12 Views: 970

## \#1 Posted by: MaxAssist Posted at: 2017-09-05T17:02:38.968Z Reads: 109

```
Hi guys,
This is my second build and  I'm having a hard time to get my build working. List of my electronic parts: 2 x Torqueboard Vesc, 2 x Torqueboard 6355 190kv motors, Torqueboard12s4p battery. I'm using Ackmaniac BLDC tools (firmware: 2.54) both Vescs are connected via canbus.

1.Master Vesc: 
* ID set: 0
* Multiple Vescs over can: ticked
* Enable traction control: ticked

2.Slave Vesc: 
* ID set: 1 
* Send status over can: ticked
* Control mode: disabled 
The other setting values I left them as default. Data communication between two Vesc seems fine.
I'd even tried Y servo cable which I created followed the instructions I found here with no luck.

Here's the problem I encounter:
Once connected with the 12s4p battery I could only get ONE motor runs smoothly. The moment I connected two motors with the battery they were clogging as shown in the video below:

https://youtu.be/POUeorYATFg

Any help would be greatly appreciated.

Best,
Max.
```

---
## \#2 Posted by: dg798 Posted at: 2017-09-05T17:08:03.432Z Reads: 95

```
I would first check ALL the connections to make sure everything is plugged in properly.
Then go onto the bldc toll and go the the terminal tab and type in fault and see if it shows any errors.
```

---
## \#4 Posted by: L3chef Posted at: 2017-09-05T17:13:03.250Z Reads: 98

```
Can you show a pic on your vesc connection wires? I didn't see a canbus wire. Looks like split servo?
```

---
## \#5 Posted by: MaxAssist Posted at: 2017-09-05T17:13:29.378Z Reads: 91

```
In the video, I tried out the Y servo cable for testing purposes.
```

---
## \#6 Posted by: cwazy1 Posted at: 2017-09-05T17:14:13.960Z Reads: 87

```
did you clip the +5v (red wire) when you did split servo?
```

---
## \#7 Posted by: MaxAssist Posted at: 2017-09-05T17:14:20.472Z Reads: 85

```
Thanks for replying, I did that at first. No fault code found.
```

---
## \#8 Posted by: MaxAssist Posted at: 2017-09-05T17:14:52.007Z Reads: 81

```
Yes, I did.
```

---
## \#9 Posted by: L3chef Posted at: 2017-09-05T17:15:20.277Z Reads: 81

```
Ah okay. Re-read your post and missed the y ppm at first sign. Okay, so did you do motor detection?
```

---
## \#10 Posted by: MaxAssist Posted at: 2017-09-05T17:17:43.547Z Reads: 78

```
Yes, both motors ran strong when I did the detection.
```

---
## \#11 Posted by: L3chef Posted at: 2017-09-05T17:19:23.061Z Reads: 77

```
Good. And you are sure you hit apply button and then write.? Could you post some pics of your settings in bldc tool ?
```

---
## \#12 Posted by: MaxAssist Posted at: 2017-09-05T17:24:02.130Z Reads: 71

```
I did hit apply and write buttons multiple times :sweat_smile: I'll definitely do it later as I'm at school right now.
```

---
## \#13 Posted by: MaxAssist Posted at: 2017-09-16T16:10:56.536Z Reads: 54

```
Hi guys, I found the problem. It was the motor mount screws, I changed the original screws to the stainless steel ones. They were about 2mm longer, and short the motors. I was able to fix it by chopping them down to correct length. Thank you all for your help.
```

---

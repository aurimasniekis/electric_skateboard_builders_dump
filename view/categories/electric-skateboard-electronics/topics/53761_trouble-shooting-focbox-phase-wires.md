# Trouble shooting Focbox phase wires

### Replies: 14 Views: 414

## \#1 Posted by: Acklavidian Posted at: 2018-04-28T17:26:25.308Z Reads: 96

```
I'm having trouble getting the motor detection to work on my dual motor + focbox setup. I have tried every combination of focbox and motor and have narrowed it down to a particular focbox unit. I assume that it is due to my shitty soldering skills on the phase wires. I have a multimeter but I don't know any thing about using it. haha. I just need to figure out which phase wire connection is giving me trouble. Any ideas?
```

---
## \#2 Posted by: Namasaki Posted at: 2018-04-28T17:36:33.814Z Reads: 94

```
Set the multimeter to continuity test.
It's in the resistance testing range.
When you touch the probes together the meter should beep.
Then touch one probe to the bullet connector on the end of the phase wire and touch the other to the solder pad on the Vesc where the phase wire is connected.
This will test continuity of both soldered connections.
```

---
## \#3 Posted by: Acklavidian Posted at: 2018-04-28T18:47:47.821Z Reads: 79

```
I tried all 3 wires and they all produce a beep with a reading of 000.
```

---
## \#4 Posted by: Namasaki Posted at: 2018-04-28T18:50:27.890Z Reads: 71

```
Then your soldering skills are not the problem.

It would help to post more info.

Firmware version
Software Vesc Tool or BLDC Tool
Motor mode FOC or BLDC
Settings
Voltage used for motor detect
maybe even post a video
```

---
## \#5 Posted by: barajabali Posted at: 2018-04-28T18:55:12.464Z Reads: 65

```
What’s the issue with your focboxes? They are dialing bldc detection? I can get on a chat with you to trouble shoot if you want on Monday
```

---
## \#6 Posted by: Acklavidian Posted at: 2018-04-28T19:17:07.796Z Reads: 60

```
During bldc sensored motor detection the motor spins up stops and then shakes violently.
```

---
## \#7 Posted by: barajabali Posted at: 2018-04-28T20:09:08.240Z Reads: 58

```
Have you tried it twice in a row? Sometimes the detection fails the first time
```

---
## \#8 Posted by: Acklavidian Posted at: 2018-04-28T20:11:46.609Z Reads: 58

```
https://youtu.be/DNtC0u0ZdSw
```

---
## \#9 Posted by: Acklavidian Posted at: 2018-04-28T20:12:21.640Z Reads: 56

```
I'm afraid to keep trying it... Lol
```

---
## \#10 Posted by: Blasto Posted at: 2018-04-28T20:18:35.731Z Reads: 54

```
Increase the D value in the detection parameters to 0.15

![image|454x500](upload://wClmZ7eb9TcCasbBAIQ8VgGOBAC.jpeg)
```

---
## \#11 Posted by: Acklavidian Posted at: 2018-04-28T20:20:29.948Z Reads: 53

```
okay. Hahahahaha
```

---
## \#12 Posted by: Acklavidian Posted at: 2018-04-28T20:21:42.261Z Reads: 54

```
That worked!!
```

---
## \#13 Posted by: Bjork3n Posted at: 2018-04-28T21:46:08.188Z Reads: 49

```
Had the exact same issue, turned out to be a too long usb cable between the computer and focbox
```

---
## \#14 Posted by: pixelsilva Posted at: 2018-04-28T23:18:56.213Z Reads: 38

```
Way to go @Blasto :+1: :smiley:
```

---

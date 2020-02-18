# My motor is not spinning. Help!

### Replies: 22 Views: 257

## \#1 Posted by: Ryan.tru Posted at: 2018-10-06T14:03:54.684Z Reads: 77

```
Hey guys. Yesterday I set up everything on the vesc tool and my motor was spinning fine, but today when I tested it my motor was not spinning. It moves a little and makes a little buzzing/beeping noise (I am using keyboard input on the Vesc tool). I will attach a video of it here. https://youtu.be/X4MfaO_P5P4 (I have the sk3 6354 260kv with and 8s 2p lipo battery and a flipsky Mini FSESC 4.20.)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-06T14:59:49.941Z Reads: 75

```
Did you run a motor detection?
```

---
## \#3 Posted by: Ryan.tru Posted at: 2018-10-06T15:04:43.568Z Reads: 69

```
Yeah, I did. Same exact thing happened. I'm not sure of it's the ESC or the motor itself.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-06T15:06:56.400Z Reads: 67

```
What’s the result of the motor detection?
Do you get any faults after?
You can check it in the vesc tool.
Typ faults in the console.
```

---
## \#5 Posted by: Ryan.tru Posted at: 2018-10-07T01:10:50.470Z Reads: 52

```
Hey, when I run motor detection it says bad motor detection, but when I type faults in the terminal it says "No faults registered since startup"
```

---
## \#6 Posted by: Eboosted Posted at: 2018-10-07T01:30:14.762Z Reads: 46

```
Is it a sensored motor? If so, one of your sensor wires or hall sensors could be shot, make motor detection unsensored.
```

---
## \#7 Posted by: Ryan.tru Posted at: 2018-10-07T01:30:55.109Z Reads: 48

```
Hey, it's not a sensored motor and I've been running the motor detection sensorless.
```

---
## \#8 Posted by: briman05 Posted at: 2018-10-07T01:33:59.950Z Reads: 47

```
Well if it says bad motor detection that is your issue. You should post the screenshot of the settings you have.
```

---
## \#9 Posted by: psychotiller Posted at: 2018-10-07T02:00:21.462Z Reads: 46

```
Have you set your battery cutoffs?
```

---
## \#10 Posted by: Ryan.tru Posted at: 2018-10-07T02:45:15.536Z Reads: 37

```
Yes, I have.
```

---
## \#11 Posted by: Ryan.tru Posted at: 2018-10-07T06:53:03.596Z Reads: 34

```
Do you guys have any idea why there is a bad motor detection? I'll post the settings soon.
```

---
## \#12 Posted by: Ryan.tru Posted at: 2018-10-07T08:00:35.849Z Reads: 31

```
Also, nothing looks burnt on my esc and my motor looks fine. I'm not sure what the heck is going on.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-10-07T08:57:12.308Z Reads: 24

```
If I got it right your motor is directly mounted to the wheel?
You also made motor detection like this?
If yes, they to do motor detection without load.
I mean no wheel attached.
Could be the reason why you get a bad results.
```

---
## \#14 Posted by: Ryan.tru Posted at: 2018-10-07T09:12:23.058Z Reads: 25

```
Hey, it's not attached on my wheel. It's just resting on there. (I didn't receive my mount yet and I'm impatient) I'm not sure why this happened.
```

---
## \#15 Posted by: Ryan.tru Posted at: 2018-10-07T12:17:37.985Z Reads: 21

```
Guys now my motor isn't even spinning. Wtf.
```

---
## \#16 Posted by: Andy87 Posted at: 2018-10-07T12:21:10.552Z Reads: 21

```
Your phase wires connected properly?
Which battery you use? Is the battery connected properly?
```

---
## \#17 Posted by: Ryan.tru Posted at: 2018-10-07T12:26:34.187Z Reads: 20

```
I soldered the phase wired directly to my esc and my batteries are connected by anti spark xt90 connectors. They're connected correctly.
```

---
## \#18 Posted by: Andy87 Posted at: 2018-10-07T12:30:17.182Z Reads: 19

```
Can you upload a picture how the solder joins look?
```

---
## \#19 Posted by: Ryan.tru Posted at: 2018-10-07T12:32:22.350Z Reads: 18

```
They're heat shrinked
```

---
## \#20 Posted by: Andy87 Posted at: 2018-10-07T12:49:08.727Z Reads: 19

```
How you could solder your phase wires on if it’s heatshrinked?
```

---
## \#21 Posted by: Ryan.tru Posted at: 2018-10-07T13:00:16.996Z Reads: 19

```
I soldered them then I used heat shrink tubing. What do you mean?
```

---
## \#22 Posted by: Andy87 Posted at: 2018-10-07T13:07:27.956Z Reads: 17

```
I mean that maybe one of your solder joins of your phase wires not good.
One phase doesn’t have a good contact, that’s why your motor not spinning
```

---

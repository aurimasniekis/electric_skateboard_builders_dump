# Torqueboard&rsquo;s esc programming card

### Replies: 9 Views: 2894

## \#1 Posted by: cmatson Posted at: 2015-07-31T21:25:16.019Z Reads: 176

```
So I've had this programming card for a while now, but just today my space cell finally came, allowing me to continue my build. So here's the delima, or rather, a situation that I don't want to screw up: there are two receiver wires coming from the esc: a long, and a short. I've already confirmed the long is for the receiver, and the short is for programming; but, for some reason, the esc only worked when I had the short wire for the receiver... this was before I got the programming card so I just decided to wait until it came in. Now that I have it, I got a few questions... there are three ports on the back: two receiver 3 pin connectors on the left, and a USB on the right. So I am assuming the USB is for power, and the 3 pin connectors are for connecting to the esc. But, what I don't know is where I should plug the leads in, or in what orientation: for example, should the negative of the lead face to the left or right? Also, should I take out the red (power) wire from the esc receiver leads to keep them from overpowering the programming card? being that there are two ports, should the longer receiver wire and the short programming wire be plugged in at the same time, and if some which one goes where? I'm sorry if I'm being super overly cautious but I really don't want to screw anything up... thanks!
```

---
## \#2 Posted by: torqueboards Posted at: 2015-08-01T02:30:41.357Z Reads: 172

```
Hey Caden,

 - The TorqueBoards 12S ESC OPTO includes a short wire which is the ESC Programming Wire and the longer wire which is the ESC Signal Wire. The 12S ESC requires a UBEC/BEC to power your receiver and/or ESC Programmer Card.
 - Both wires (ESC Programming Wire & UBEC Wire) with negative facing wire point to the right side.
 - ESC Programming Wire (Shorter wire) is always plugged into the left 3pin port with negative/ground/black wire facing the right side.
 - UBEC is always plugged into the right 3pin port with negative/ground/black wire facing the right side.
 - The USB Port on the left is only needed if you want to program using the computer software. Both the ESC Programming Wire and UBEC wires still need to be plugged in and the Power needs to be on to power on the ESC Programming Card.
 - Each ESC is programmed individually.
 - The ESC Programming Card is powered by the on-board battery of your setup from your UBEC/BEC.
 - The Y connector and/or ESC Signal wires should be disconnected from the receiver and/or will not allow the ESC Programming Card to boot up the ESC Firmware.
 - If everything works, you should see 1: Motor Timing and 5: Very High as the first value/option to adjust/edit.

Let me know if you have any other questions.

<img src='/uploads/db1493/original/1X/40e2905abacf82f3f0322a5c5200217d80c8f491.jpg'>

I recommend the following settings:

 1. Motor Timing: Very Low, Low, **Normal, High, Very High**
 2. Acceleration: Low, **Medium, High, Very High**
 3. Running Mode: **Forward/Brake,** Forward/Reverse/Brake, Forward/Reverse
 4. Brake Force: 10%, 20%, 30%, 40%, **50%, 60%, 70%, 80%, 90%, 100%**
 5. Drag Brake: **0%,** 5%, 10%, 15%, 20%, 25%, 30%, 35%
 6. Cut-Off Voltage: 2.6V/cell, 2.8v/cell, 3.0v/cell, 3.2v/cell, **3.4v/cell**
 7. Max Forward Force: 20%, 40%, **60%, 80%, 100%**
 8. Max Reverse Force: **20%, 40%, 60%,** 80%, 100%
 9. Motor Rotation: **Normal,** Reverse
 10. Neutral Range: **3%,** 5%, 7%, 9%
 11. Battery Type: NiMh, **LiPo**
```

---
## \#3 Posted by: cmatson Posted at: 2015-08-01T02:40:59.291Z Reads: 135

```
Thank you sooo much! This really helps, and I hope to have it all setup tomorrow!
```

---
## \#4 Posted by: onloop Posted at: 2015-08-03T03:01:45.851Z Reads: 135

```
A video on setting this up would be AWESOME!
```

---
## \#5 Posted by: cmatson Posted at: 2015-08-03T03:07:51.589Z Reads: 137

```
I might put one up on youtube to save him the time: the description was super self explanatory, but everyone loves video tutorials now in days... lol
```

---
## \#6 Posted by: torqueboards Posted at: 2015-08-03T04:19:06.199Z Reads: 133

```
I have one here. I'll make a simpler one soon though.
https://www.youtube.com/watch?v=hvljCjOZLUc
```

---
## \#7 Posted by: Skunk Posted at: 2019-03-08T20:19:17.739Z Reads: 35

```
![thread_necromancer_king_card|333x493](upload://99BgroBFGQpQm4XWgOiU3aBItfQ.jpeg)
```

---
## \#8 Posted by: DerelictRobot Posted at: 2019-03-15T18:57:56.428Z Reads: 23

```
[quote="onloop, post:4, topic:83, full:true"]
A video on setting this up would be AWESOME!
[/quote]

Wait. Was this a simpler time when you were friendly to @torqueboards and even asked for his help?

I'm so confused.

Moooooooooom!
```

---
## \#9 Posted by: torqueboards Posted at: 2019-03-15T21:31:18.710Z Reads: 18

```
This was when onloop use to whisper sweet nothings in my ear.
```

---

# Motor Wont Turn On \[ Need Help \]

### Replies: 10 Views: 997

## \#1 Posted by: NathanMC Posted at: 2016-09-09T19:10:16.388Z Reads: 69

```
Hey Esk8,

So I recently been having troubles with my board and have been spending lots of time trying to fix it. 
So right now I have reached an Issue that I can't solve. 

Specs:
120a 6s FVT ESC
5055 280KV motor Torque boards 
2x 3s 5000mah batteries running in series 

So when I was programming my ESC with a programming card everything was going smooth. I was able to change the settings, The motor would twitch whenever I updated something and looked like there was no problem. However when I tried to test out the motor it wouldn't work. Normally I would hear the beep confirmation when the motor would turn on although this time no motor beep. My GT2B is connected, ESC just arrived from the mail, Batteries are all balanced, motor seems totally fine and checked all the wires. I have no clue whats wrong. 

If anyone could help me it would be awesome thanks

-Nathan
```

---
## \#2 Posted by: crameur Posted at: 2016-09-10T07:28:09.246Z Reads: 50

```
Someone can help him ?
bump
```

---
## \#3 Posted by: kaziupir Posted at: 2016-09-10T10:17:11.591Z Reads: 48

```
Did you calibrate the throttle range? It won't start without it.
```

---
## \#4 Posted by: NathanMC Posted at: 2016-09-10T18:50:40.938Z Reads: 42

```
How do I calibrate it? Is it a setting that I can see in the programming card? Or do I need to calibrate it from the GT2B?
```

---
## \#5 Posted by: kaziupir Posted at: 2016-09-10T19:18:52.778Z Reads: 38

```
Something like that: 
https://www.youtube.com/watch?v=eSq284Ehkps
But better read manual
```

---
## \#6 Posted by: NathanMC Posted at: 2016-09-10T19:24:58.386Z Reads: 32

```
Thanks for the quick reply!, I'm at work but ill update you if anything happens when I get home. Thanks again.
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-09-10T19:38:16.192Z Reads: 30

```
Do you run sensor or sensorless ? If youre sensor did you follow the correct color code for the wire (it can change from esc to esc).
```

---
## \#8 Posted by: NathanMC Posted at: 2016-09-11T00:41:37.874Z Reads: 24

```
Alright so I tried calibrating it but once i got to part where i wanted me to pick my forward and brake it wouldn't beep when i pressed the set button.

I tried following this video.
https://www.youtube.com/watch?v=lXBI4L8y1b4
```

---
## \#9 Posted by: NathanMC Posted at: 2016-09-11T00:43:54.665Z Reads: 24

```
Its sensored, how would you connect the A,B,C wires to the torque motor (Yellow,Blue,Black)
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-09-11T00:57:19.020Z Reads: 22

```
From @torqueboards web site in the motor description:   

Red = 5v, White = Temp, Blue = A, Yellow = C, Green = B, Black = GND

Also look in the datasheet of your ESC to find is right pinout
```

---

# Does battery amps get divided?

### Replies: 10 Views: 250

## \#1 Posted by: amms50 Posted at: 2019-06-25T19:15:11.008Z Reads: 91

```
Hey,
I know it is a stupid question but when the battery supplies 80a and the motors need 75a per motor, will the 80a from the battery get divided into 40a per motor or will i be able to supply the full 75a for each motor (I know it’s never advised to give the full amps to a motor but it’s just an example)
```

---
## \#2 Posted by: Flasher Posted at: 2019-06-25T19:18:19.734Z Reads: 92

```
Depends on the esc settings for your battery. You will draw what you programmed it to give but if my memory is good, you'll end with 40/40 even if you set the motors at 75-80 amps. Battery amps and motor amps are different settings altogether
```

---
## \#3 Posted by: Battosaii Posted at: 2019-06-25T19:18:21.827Z Reads: 89

```
Battery amps and motor amps are 2 different things.

If you have a battery that can deliver max 80a then you should not set the vesc to more than 40a each max battery but motor amps can be set to 80 each.
```

---
## \#4 Posted by: meesie Posted at: 2019-06-26T11:23:52.527Z Reads: 57

```
[quote="Battosaii, post:3, topic:97290"]
Battery amps and motor amps are 2 different things.
[/quote]

i don't know the technical explanation for this, but this is indeed how it works.

what you need to do is take your max battery current and divide it by two for each vesc. so 80 batt amps is 40 per vesc (the same goes for batt min!). now, your motor amps are a whole different thing. i usually put em on 40 buth to begin with and adjust accordingly.
```

---
## \#5 Posted by: amms50 Posted at: 2019-06-26T12:27:13.821Z Reads: 46

```
[quote="Battosaii, post:3, topic:97290"]
Battery amps and motor amps are 2 different things.
[/quote]

Then what’s the relation between them? Like if the battery can supply only 40a per vesc and the motor max is 75a will I still get the full power and acceleration or will something be less and if then what will be less?
```

---
## \#6 Posted by: Battosaii Posted at: 2019-06-26T12:42:10.127Z Reads: 45

```
Really no relation lol

The motor amps are more for that low end power and battery amps is that high speed power. 

I run 80a battery amps per Focbox Unity x2 and moving up from 80a motor amps to 90 then 100 to hopefully end up trying 120 motor amps.

I'd start slow with 40 motor anos and move up from there as you get used to it. It makes a huge difference in board power.
```

---
## \#7 Posted by: meesie Posted at: 2019-06-26T15:30:27.517Z Reads: 37

```
there is some relation, though i don't now what kind of relation. this is one of my logs with the METR app:

https://metr.at/r/286xm

you can see the motor amps and battery amps follow somewhat the same line but  have different amparages at all times except when not applying throttlle.
```

---
## \#8 Posted by: professor_shartsis Posted at: 2019-06-26T16:25:02.403Z Reads: 29

```
[quote="amms50, post:1, topic:97290, full:true"]
Hey, I know it is a stupid question but when the battery supplies 80a and the motors need 75a per motor, will the 80a from the battery get divided into 40a per motor or will i be able to supply the full 75a for each motor (I know it’s never advised to give the full amps to a motor but it’s just an example)
[/quote]

[quote="Battosaii, post:3, topic:97290"]
Battery amps and motor amps are 2 different things.
[/quote]

here is a comparison of the motor current (blue line, top left chart) with the battery current (black line, top left chart)

https://i.ibb.co/3pg7w4K/motor-vs-battery4.jpg

^assumptions: 46v, 2x 0.05ohm 190kv motors, 40a battery limit per motor and 80a motor current limit per motor, 2.625:1 gear ratio & 100mm tires

EDIT: re-uploaded chart to fix some errors in the original
```

---
## \#9 Posted by: professor_shartsis Posted at: 2019-06-26T16:42:14.287Z Reads: 22

```
basically if you were to short your battery to the motor (not advisable) you might get some thousands of amps for a short duration, but if you use a vesc to switch between shorting your battery to the motor and then the motor to itself 20,000-30,000 times per second you might get something reasonable like 80a motor current. the difference between the battery current and motor current comes from the fact the motor current continues to flow inductively during the portions of the second that the motor is shorted to itself, and during these same times, the battery current does not flow, leading to a greater amount of current on average in the motor, than in the battery when the duty cycle is less than %100, which is all the time in a vesc since it does max 95%.
```

---
## \#10 Posted by: professor_shartsis Posted at: 2019-06-26T17:02:58.468Z Reads: 22

```


one of the hardest parts to wrap my mind around initially was the significance of the battery current. if you look at left side of the top left chart, notice the battery current is 6.95a, the motor current is 80a, and the duty cycle is 8.69%, which corresponds to full throttle acceleration from standstill. what does this "6.95a battery current" look like to the battery? the battery is actually supplying pulses of roughly 80a battery amps, 8.69% of the time in an on-off cycle frequency of 20-30 kilohertz (20,000-30,000 cycles per second), which is 6.95a from the battery for the whole second on average.
```

---

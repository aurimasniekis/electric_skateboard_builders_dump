# What Voltage and Amperage should one use to get a good smooth brake that isn&rsquo;t too sharp?

### Replies: 20 Views: 448

## \#1 Posted by: ToucanSam Posted at: 2018-08-01T04:58:46.694Z Reads: 159

```
I have a 12s6p battery on my board and the acceleration is great but a little sharp. The breaking is so sharp i can barely pull the trigger before the board slams on the breaks.

What Voltage and amperage should I use to be able to have good accel and top speed but not too sharp accel or breaking?
```

---
## \#2 Posted by: Eboosted Posted at: 2018-08-01T05:02:51.661Z Reads: 158

```
The sensibility of braking and acceleration is not related to maximum current settings but with throttle settings, if you have a mini remote you should have plenty of throttle range.

Have you calibrated your ppm settings? 

Are you using a nano x remote?
```

---
## \#3 Posted by: koralle Posted at: 2018-08-01T05:04:37.860Z Reads: 152

```
Be sure to try different ramping settings!
```

---
## \#4 Posted by: ToucanSam Posted at: 2018-08-01T12:56:06.785Z Reads: 126

```
I am using the nano remote from Torque Boards, I followed their instructions for remote setup, and their instructions for calibrating the vesc's to my motors, but they didn't mention throttle range or ramping settings.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-08-01T13:40:32.451Z Reads: 108

```
what are your vesc settings?
If you simply use the same specs for brakes as for discharge, brakes are too strong usually.
```

---
## \#6 Posted by: Eboosted Posted at: 2018-08-01T14:43:28.065Z Reads: 98

```
AFAIK the nano remote has a really short throttle range that cause the brakes to feel too strong. You might want to talk to @achatham about this he has the exact same issue. This does not happen with the mini remote
```

---
## \#7 Posted by: ToucanSam Posted at: 2018-08-01T14:46:33.042Z Reads: 102

```
If worse comes to worse, what remote is better but not too big?
```

---
## \#8 Posted by: Eboosted Posted at: 2018-08-01T14:48:35.519Z Reads: 100

```
I'm already used to the mini remote. Best remote connection wise, you get used to it and won't use anything else ever
```

---
## \#9 Posted by: ToucanSam Posted at: 2018-08-01T14:49:37.797Z Reads: 98

```
I think I have max accel amperage at 60 and the breaking amperage capped at 40, but I know the boosted board uses a 12s1p battery which would lead me to believe that the amperage they have available is 15A or 20A, but if it's a remote issue I can just find a different one.
```

---
## \#10 Posted by: ToucanSam Posted at: 2018-08-01T17:36:38.649Z Reads: 84

```
Oh haha good to know, I'll just send Torque Boards an email and see I'd they can tell me how to make the acceleration curve smoother.
```

---
## \#11 Posted by: Hummie Posted at: 2018-08-01T17:40:08.572Z Reads: 78

```
theres two settings for acceleration and two for braking in the vesc: motor and battery current and negative motor and battery current.  40 is high for either negative motor or battery i think.
```

---
## \#12 Posted by: b264 Posted at: 2018-08-01T17:42:35.544Z Reads: 75

```
Mini Remote might be big, but it's killing it in every other way.  Highly recommend.
```

---
## \#13 Posted by: Michael319 Posted at: 2018-08-01T18:09:01.273Z Reads: 69

```
The Maytech thumb remote has actually been pretty great. Also highly recommend
```

---
## \#14 Posted by: DAddYE Posted at: 2018-08-01T18:20:26.253Z Reads: 66

```
Mine has a very short range. I almost died lol
```

---
## \#15 Posted by: Michael319 Posted at: 2018-08-01T18:23:55.287Z Reads: 65

```
Your Maytech? Maybe mine works well because I'm running sensored and the range isn't as important, although still nice.
```

---
## \#16 Posted by: DAddYE Posted at: 2018-08-01T21:55:05.486Z Reads: 58

```
Mine loses connection very often often. Seems due to some interferences
```

---
## \#17 Posted by: Hummie Posted at: 2018-08-01T21:56:46.294Z Reads: 58

```
mine sucks
```

---
## \#18 Posted by: achatham Posted at: 2018-08-02T01:09:52.966Z Reads: 46

```
So I noticed that the braking numbers you set, no matter if it’s 8 or 16, it’s always very responsive at the lower speeds but where you notice the big difference in responsiveness is at higher speeds. With braking set to 16 I am able to stop a lot quicker than if set at 8.

Now that number will be different based on your motor, weight, terrain etc.
```

---
## \#19 Posted by: ToucanSam Posted at: 2018-08-02T01:49:22.156Z Reads: 42

```
What do you mean set the brake to 16? Can you send me a link to what you are talking about?
```

---
## \#20 Posted by: Eboosted Posted at: 2018-08-02T02:08:31.124Z Reads: 41

```
Reduce your motor min from -65A to -50A it'll give you less braking a lower speeds
```

---

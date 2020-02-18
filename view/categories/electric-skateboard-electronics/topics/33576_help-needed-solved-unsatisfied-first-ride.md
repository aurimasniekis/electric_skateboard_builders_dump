# Help Needed(solved): Unsatisfied first ride

### Replies: 21 Views: 894

## \#1 Posted by: TunaTee Posted at: 2017-09-20T14:18:46.906Z Reads: 132

```
<img src="/uploads/db1493/original/3X/b/e/bed71b401a1da49d803d5b6e10821e12f757637b.JPG" width="375" height="500">
Hello guys. This is my first build. I just took it out for my first ride this morning. The experience is great and I was happy like a kid. 
Well, the happiness only lasted 25minutes. :frowning: 

I got three 3s1p 5000mah batteies connected in series. My motor is 6355 190kv from torqueboard.
I weigh about 180lb. 

I fully charged my battery so each is 12.6 V when I left the house. I rode for 25minutes. 3.14miles on record and 14.2MPH topspeed.
Isn't that a little bit too short for 15A?

If it is normal with my setup, then how can I increase the ride length of my skateboard? I am planning to get another 3s1p 5000 mah battery and add that to the serie, will that help? Thanks
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-09-20T14:30:23.060Z Reads: 124

```
its not 15AH. its 5Ah. 
and u have to calculate by Whr that would be 4.2 x 9 x 5.
and 100whr is aprox 10km. 
i think u may set the cut off voltage too high
```

---
## \#3 Posted by: rich Posted at: 2017-09-20T14:30:24.659Z Reads: 120

```
[quote="TunaTee, post:1, topic:33576"]
3.14miles on record and 14.2MPH topspeed.
[/quote]

That's strange with 9s and 190kv motor. I would expect about 10 miles range and more top speed.
What's your gear ratio and diameter of your wheels?
```

---
## \#4 Posted by: NickTheDude Posted at: 2017-09-20T14:30:29.954Z Reads: 119

```
[quote="TunaTee, post:1, topic:33576"]
If it is normal with my setup, then how can I increase the ride length of my skateboard? I am planning to get another 3s1p 5000 mah battery and add that to the serie, will that help? Thanks
[/quote]

What are your voltage cutoffs set at? You're around 200Wh so you should be getting a lot more range.
```

---
## \#5 Posted by: Vieo Posted at: 2017-09-20T14:31:35.912Z Reads: 117

```
Did you measure the battery voltage after?
```

---
## \#6 Posted by: TunaTee Posted at: 2017-09-20T14:32:09.280Z Reads: 112

```
hello onepunchboard, thanks for the correction.
I do not have a cut off voltage. I just plug-in and started riding.
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-09-20T14:32:55.725Z Reads: 114

```
thats why u hav to go to computer connect vesc with usb and set the correct parametet
```

---
## \#8 Posted by: TunaTee Posted at: 2017-09-20T14:33:33.075Z Reads: 110

```
Hello rich,
My gear ratio is 16T to 36T. My wheels are 83 mm. I do not think it should be a problem because it came with a set from TorqueBrand.
```

---
## \#9 Posted by: rich Posted at: 2017-09-20T14:34:14.386Z Reads: 103

```
[quote="TunaTee, post:6, topic:33576"]
I just plug-in and started riding
[/quote]

Without doing motor detection before?
```

---
## \#10 Posted by: TunaTee Posted at: 2017-09-20T14:35:00.102Z Reads: 100

```
Hi nickthedude. I don't have a voltage cutoffs. 
It should be the problem, I could not find a mini usb cable to configure the VESC. I thought it would not be such a big issue and went out lol.
```

---
## \#11 Posted by: TunaTee Posted at: 2017-09-20T14:35:47.664Z Reads: 100

```
Guess that is the problem. lol, thanks.
```

---
## \#12 Posted by: TunaTee Posted at: 2017-09-20T14:36:11.408Z Reads: 96

```
Got it. Thanks man!
```

---
## \#13 Posted by: NickTheDude Posted at: 2017-09-20T14:38:16.009Z Reads: 93

```
You need to program your VESC. You DEFINITELY should not ride it without doing so.

Run motor detection, set motor and battery amp limits as well as voltage cutoffs.

The VESC is ABSOLUTELY NOT plug and play.

Your problem is that you do have the default voltage cutoffs.
```

---
## \#14 Posted by: rich Posted at: 2017-09-20T14:39:18.285Z Reads: 91

```
:joy: I thought I'm impatient but you are the man! Going for a ride without setting it up :laughing: I hope your Lipos are alright. Why you knew that your range is 3.14 miles?
```

---
## \#15 Posted by: TunaTee Posted at: 2017-09-20T14:49:24.250Z Reads: 91

```
Thanks man. Appreciate it.
Guess I am too savage lol.
```

---
## \#16 Posted by: TunaTee Posted at: 2017-09-20T14:50:55.102Z Reads: 91

```
Lol man...haha. I recommend you an app called Speedometer. It uses for trip record on cars but I figure I can use it for my eboard. It costs 3.99 usd. It shows your top speed, trip distance and other stuff.
```

---
## \#17 Posted by: TunaTee Posted at: 2017-09-21T01:57:51.618Z Reads: 66

```
<img src="/uploads/db1493/original/3X/2/6/2617035aba8328e8994dd15ea3fc54edea23d294.png" width="690" height="399"><img src="/uploads/db1493/original/3X/e/a/ea651d94ced56f8b1d3d3771a30d2fc75e9bcd72.png" width="690" height="373">
Hello NickTheDude
Will this be a good setup? I watch the youtube tutorial just want to make sure lol.
```

---
## \#18 Posted by: NickTheDude Posted at: 2017-09-21T02:01:35.444Z Reads: 63

```
Yep, looks good too me.
```

---
## \#19 Posted by: TunaTee Posted at: 2017-09-21T02:10:03.136Z Reads: 63

```
Thanks man~
```

---
## \#20 Posted by: deucesdown Posted at: 2017-09-21T20:00:30.062Z Reads: 43

```
Looks too low to me!
31v/9 = 3.44v/cell
29v/9 = 3.22v/cell

Teh internets tells me for lipo, there's not much energy below 3.7v/cell (33.3v for 9s pack).

As the individual cells in your pack will not discharge perfectly evenly, your risk of overdischarging a cell (going below 3.0v) goes up the lower your total pack voltage.

As for range, your nominal watt hours is 3.7v*9*5000mah == 162wh, and 20wh/mile seems common, with some getting like 10wh/mile (low weight, flat ground, strong batteries). so 8-16miles depending on conditions.


This is all from reading, not practical experience, so I'll defer to people who've actually done it, but I'd set the cutoff start to 34.2v (3.8v per cell ) and cutoff end to 33.3v
```

---
## \#21 Posted by: TunaTee Posted at: 2017-09-25T14:12:09.915Z Reads: 21

```
Thank you, I will change it. Appreciate.
```

---

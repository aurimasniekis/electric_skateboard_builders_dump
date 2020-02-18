# Motor current, battery current, 100km/h

### Replies: 12 Views: 1679

## \#1 Posted by: Fetteperson Posted at: 2017-10-30T13:18:03.873Z Reads: 258

```
Hello everyone,

Last weekend I tried to build my e-skate for 100km/h. 

I changed on my dual setup both cogs on the motor-side from 15T to 30T... so in theory it should go twice as fast. With the rpm- tool I achieved the 100km/h as expected. So I got all geard up to go on the road... Unfortunatelly I only reached 60km/h. Then I connected my laptop to the focbox while riding to see what the data looks like.

My Setup:

12s, 8000mah 45-90c lipo
2x Focbox
2x 6355motor, max 65A, max 3500W (Maytech)

My data at max speed (~50km/h)
Power ~1000W
Duty cycle: ~45%
Electrical speed: ~15000 rpm
Battery current 25A
Motor current 55A

Now the first thing I don't get is: Why is battery current so much lower than motor current?

Why don't I get those 60A * 50V = 3000W power?

My settings are the regular settings on BLDC. I only changed Battery max to 60A, motor max to 65A.

What is limiting the Power?

Thank oyu in advance for your help.
```

---
## \#2 Posted by: telnoi Posted at: 2017-10-30T13:34:55.134Z Reads: 244

```
Are you using a single or multiple lipos? how are they connected?
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-10-30T13:53:57.226Z Reads: 237

```
Now we have a interesting case. Please post a screenshot of your settings. First of all you have to be aware that at 100 km/h you need 8 times the power than at 50 km/h. So with your motor and so on you won't be able to achieve that. Because it needs about 10000 watts or so to hold you at that speed.
But it should at least be able to output more power. But i guess something is limiting the power. Easiest way to find out would be if you get a bluetooth module and use my app. And make a video of course and share it with us.
```

---
## \#4 Posted by: esk8 Posted at: 2017-10-30T14:45:55.759Z Reads: 220

```
Can you give some information for us.
Battery, Motor and Motor pulley was not enough.
Wich wheel size, witch Wheel pulley and how many KV have your Motor.
The transmission play a very big role.
I have making some calculation with some Setups, that you can ride 100Km/h
and Ackmaniac say it right you need over 10.000 Watt and over 200A that you 
can ride this speed.
I would be really interested in your translation.
```

---
## \#5 Posted by: Fetteperson Posted at: 2017-10-30T15:13:04.222Z Reads: 206

```
2 lipos in series
```

---
## \#6 Posted by: Fetteperson Posted at: 2017-10-30T21:15:11.142Z Reads: 187

```
First of all: thank you for your time and help...

@esk8 My gear ration (for this experiment) 40T/30T (5m 15mm)with 97mm wheels. Motor 190kv.
I hope this is everything you need to know.

@Ackmaniac Could you send me a link about some informations about your app and how to use it. 



<img src="/uploads/db1493/original/3X/d/6/d66a2d14fb2fde71f5f1257a9c6dd88ad748942a.PNG" width="690" height="409"><img src="/uploads/db1493/original/3X/2/9/29fb9afff0ea60be5382f3b006d091cc9723a8c1.PNG" width="690" height="407"><img src="/uploads/db1493/original/3X/c/5/c58cae946c84e1da7b5256e06078866f6a978dfd.PNG" width="690" height="415">
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-10-30T21:44:51.736Z Reads: 160

```
More info here.
https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888

Just lower your battery cutofff start and end.  Set the start to 42V and end to 39,6V.
Charge the battery full and use my app to see what is happening.
And raise your motor min because your brakes must be weak. And check which charge current is allowed for your battery. you can go higher but maybe no more than 50%. Because 2 times 20A (battery min) = 40A for the battery can be a bit high.
And you can raise the motor max to 80 or so. (i know it's not rated for that but you won't use it constantly) 
If the motors get so hot that you can't touch them anymore then lower it again. but otherwise you will be fine with 80A.

And most important. Don't kill yourself.
```

---
## \#8 Posted by: esk8 Posted at: 2017-10-31T06:55:49.060Z Reads: 136

```
Hi thanks for the information about your Setup.
I have calculated with your wheels and translation what you can ride.
The maximum was 65Km/h,
by this speed your setup using 2990W and 59,8A 
When you want ride with your Setup 100Km/h you need over 10.000W and over 200A
You can take the Motor setting to 80A but the controller can continues 60A
The danger by this was that your fet´s overheat and kill your controller.
And yes your Battery cut of start and end was to high.
You must looking on your battery wit how many charging rate you can charging
2 ore 4 ore 6 C
You must multiplier the C with your 8Ah and so you know with how many A you
can charged your battery.
When there are standing 4C so you can charging with max. 24A 
then you can leave the 20A by batt min.
But by mot min you must going up to 50-60A
I made the best experiences when the parameter by mot. max mot min. and batt max.
was identical.
```

---
## \#9 Posted by: Fetteperson Posted at: 2017-10-31T13:45:36.743Z Reads: 104

```
Thanks for your help. 

@esk8 How did you calculate that? Did you consider the dual setup? 

Motor min. I just left it where I had it for the 40T/15T pulleys. And the battery min current I also left it for my regular batteries with low C rating...
Concerning the battery cutoff... I had the problem, that not each cell discharged at a same speed. So for security reason i set the cutoff higher.

An other question. How come that battery current and motor current are not identical?
```

---
## \#10 Posted by: Fetteperson Posted at: 2017-10-31T13:55:03.744Z Reads: 102

```
Thank you very much. Just bought the Bluetooth module...
```

---
## \#11 Posted by: Hummie Posted at: 2017-10-31T15:32:59.842Z Reads: 98

```
are your motor and battery current results from one focbox or two?   someone will tell you that you will melt but I put my motor amps to 120 and battery amps you can increase a lot too.  there is a temp sensor to protect the esc from overheating but maybe it's a bit too slow to register the heat there but I wouldn't worry about it as whatever huge current you're trying to do will be done quickly and back to cooling.  
I bet you can do that speed with less than 10,000 watts in a good aero tuck or maybe ud have to lay down
```

---
## \#12 Posted by: Fetteperson Posted at: 2017-11-01T06:14:33.077Z Reads: 66

```
those are the results from 1 focbox
```

---

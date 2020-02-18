# My first board (help with values vesc)

### Replies: 10 Views: 459

## \#1 Posted by: edgar.s Posted at: 2019-01-06T22:03:35.403Z Reads: 121

```
Hello, I'm new to electric longboard

After reading too much in this forum remains confused with 

What do Motor Current Max and Battery Current Max, and what is the ideal value and how to calculate.
Any help is welcome

My setup is dual connected Y-SPLIT 

Specs:
@egzplicit
motor:dual KEDA 63-64 190KV Brushless Outrunner 10S 2000W
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html

dual vesc Turnigy SK8-ESC V4.12
https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html

battery: Lipo 2* ZIPPY Flightmax 5000mAh 5S1P 20C
in serie 10s 5000mah 20c
Max Charge Rate(C) 2
https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html

Vesc tool PrintScreen 
![Capturar|690x353](upload://3uigXTOroFxiHazC7fNNprkAy6l.png) 

Any changes I can make for the better?
I feel like I do not have much braking power
Is it possible faster?
Can someone explain better what it is Motor Current Max and Battery Current Max,
and if I can increase more than 50a, my vesc is 50a current.
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-01-07T05:03:36.905Z Reads: 90

```
Well first for braking Power you can increase it to -60 if you want even stronger braking, second what do you mean by faster, aclearation or speed, if you want aclearation you can increase your motor amps, also you can go over the 50a continuous on the vesc if you have aduqite cooling.

Battery amps is how many amps you vesc will draw max from the battery, since you have 2x 5s 5000mah 20c lipos you will have 10s1p, so basically capacity times c rating (your battery can do 5x 20c = 100 battery amps but take that with a grain of salt as manufacturers overestimate their ratings)

Motors amps is how many amps your vesc will push to the motors of course, and that if you have a decent vesc you can push 80a  through if everything is cooled of course, for the turnigy vesc I wouldn't try your luck with foc on it
```

---
## \#3 Posted by: AlexBE Posted at: 2019-01-07T06:08:47.366Z Reads: 88

```
I would increase your battery charge amps. at -4 you are going to have weak brakes at high speed. At least test the strength of your brakes. I would be comfortable regeneratively charging those batteries at 2C, so -10A.
```

---
## \#4 Posted by: edgar.s Posted at: 2019-01-07T09:50:59.969Z Reads: 75

```
i use bldc mode, can i change motor current max brake for -60A It will not burn my vesc ?

I do not understand if the limit of my vesc 50a is on Motor Current Max or Battery Current Max

which burns vesc

i use dual system (-4) +(-4)= -8
I can by -10 but I do not know if it's going to change a lot
```

---
## \#5 Posted by: Jalapeno Posted at: 2019-01-07T11:38:36.612Z Reads: 65

```
The limiting factor here seems to be the "battery current max regen".
Typically lipos are rated for charge at 1C, which in your case is 5A (5000mA) so that is your very safe braking current.
If you want stronger brakes you can increase it from there, you can run 10A braking current which is 5A per vesc and you are charging at 2C. And so on an so forth.
Some people here use high braking currents like 5C (in your case 25A, 12.5A per vesc) or even higher, some argue that it is only for a small period of time and hence it doesn't negatively affect the lipos. I would say to pick a sweet spot that you're confortable (with respect to braking force) between 1C and 5C.
And just beware that you are charging your batteries above their rated specs.
```

---
## \#6 Posted by: Noob-at-building Posted at: 2019-01-07T11:53:26.879Z Reads: 59

```
Hay i wouldn't recommend going with the zippy if you are having a long term board, and keep in mind 5s will make your board stick out a bit further than you will probably like
```

---
## \#7 Posted by: egzplicit Posted at: 2019-01-07T18:25:17.511Z Reads: 56

```
Like @AlanZhou said, according to specs you can pull at most 100A from your pack. I would recommend 40A battery max per vesc, it's 10A below the limit and 20A below max rating of that battery. For motor amps you can go as high as 80A, It will help with starting from a stand still but at some point the bat max limits motor max so even stupid values won't hurt anything. Do incremental values, try 40A bat max and 60A motor max and see how it feels.

For brakes I'm not sure how many amps those lipos take but in general battery Min should not be more than 120% of the rating of the pack otherwise you'll damage the battery. If it's only 2C charging that gives you only 10A (2c * 5) so that's only -5A battery Min per vesc. If it takes more you can "increase" the value (it's actually decreasing as it's a negative one but whatever).

Edited: bat max Vs motor max was explained here but basically at lower duty cycle you can push more amps into a motor compared with how many you pull from your pack. When setting motor max keep in mind the vesc limits, a focboxes does 80A motor max easily but others I don't know.
```

---
## \#8 Posted by: edgar.s Posted at: 2019-01-09T11:03:41.836Z Reads: 42

```
Hello thanks i put baterry regen max 5A in each vesc and brake better 

I feel comfortable with it so it has a lot of torque power but my question is max battery is the strength of the board correct? and max motor is the speed of the board? Correct or I'll confuse everything.
I would also like to know which is the max engine of my vesc suport without burning
```

---
## \#9 Posted by: egzplicit Posted at: 2019-01-09T16:55:16.929Z Reads: 38

```
[quote="edgar.s, post:8, topic:80123"]
max battery is the strength of the board correct? and max motor is the speed of the board?
[/quote]

Top speed doesn't change when these values are changed, only the time to get to top speed changes.

Battery max dictates how many amps you can pull from your battery. Motor amps are how many amps can be pushed into the motors. The reason motor max can and should be higher is because at lower speeds you don't use all the volts your battery provides. It's to do with duty cycle, there are a few good explanations around here so I won't repeat them... but put it this way: having higher motor max values will help with the power for low to mid speeds. Having higher battery amps will help power when going mid to high speeds (but will also affect low to mid speed).

Just make sure your battery max is below the vesc & battery rating. As for motor max, i don't think anyone quotes limits on their vesc for that value, it's mostly safe to go even to 100A (but again, you won't reach that because after a certain speed the battery max will limit what motors can receive).
```

---
## \#10 Posted by: briman05 Posted at: 2019-01-09T17:56:44.228Z Reads: 33

```
Cant get a better answer right there from @egzplicit. Cut and dry answer
```

---

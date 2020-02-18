# First Build - math problems

### Replies: 22 Views: 2037

## \#1 Posted by: joaosoprano Posted at: 2017-03-17T11:20:55.380Z Reads: 134

```
Hi guys! I'm trying to plan my first build and I am having trouble figuring out the math to be confident that the components that I choose are correct. I already have a deck, trucks and bought some 80mm orangatang wheels. I also bought a VESC. My only problem trying to dimension my esk8 is that I don't see calculations that facture the weight of the rider. How can I account for that? I was trying to work out the math and the theoretical torque that for 100kg (85kg (my weight) + 10kg of the skateboard =~ 100kg) and my 80mm wheels would be T=100*g*0.04=39.24Nm and i can't get nowhere near that value using the motors that i have found to be recommended. for a motor lets say with 60mm with 2200W, 190Kv with a 10s battery (37V) saying that P=T*w, T=2200/((190*37*2*pi)/60) = 2.99N.m that's a 13 times the torque required. gearing this would be a lot higher than a 1:3 ratio. could you help me out figuring out my error? Thanks in advance
```

---
## \#2 Posted by: kampfhahn Posted at: 2017-03-17T11:38:34.476Z Reads: 128

```
Try [this](http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii) calculator. 2200 Watts are way more than you need.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-03-17T11:38:51.288Z Reads: 129

```
we don´t usually make it that complicated. We calculate round about motor, battery, gearing.
Use this calculator for example: http://calc.esk8.it/
Use a motor according to your battery: http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

A good working standard for you would be:
10s battery, 190 kV 6374 motor, 15/36 gearing 15mm and your 80mm wheels.
If you have some hills in your area, go with dual 6355 motors
;)
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-03-17T11:41:08.328Z Reads: 116

```
Also just post here when you want to buy some new things and I´m sure people will try to check that you don´t buy stupid stuff :slight_smile:
```

---
## \#5 Posted by: joaosoprano Posted at: 2017-03-17T11:44:54.829Z Reads: 103

```
Now that's a calculator that seems complete! thanks!
```

---
## \#6 Posted by: joaosoprano Posted at: 2017-03-17T11:52:49.225Z Reads: 96

```
I'm saving for the dual motor setup, so as a first iteration i was thinking on initially going with one 6355 and when I'm able buy the second one. 
That's my problem, I tend to over complicate what seems simple, but as an engineer student, math is the first thing that I turn to facing a problem :p I'm sure that if empirically something works my math should show it, that's what's baffling me x) 

Thanks for the suggestion and quick reply! From my research I was going to go with something along the lines of what you suggested, but wanted to make my math work, just to be sure.
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2017-03-17T12:30:07.819Z Reads: 87

```
[quote="TarzanHBK, post:3, topic:19214"]
we don´t usually make it that complicated
[/quote]

I got to the second sentence and all of a sudden my eyes 👀 it got all blurry
```

---
## \#8 Posted by: TarzanHBK Posted at: 2017-03-17T12:41:41.896Z Reads: 93

```
yah i don´t wanna throw every new guy in our deeeeeeep and coooooold water :smiley:

keep it simple at first
and after bit of reading
they´ll find threads with peops like @devin (all humor here bro ;))
to make it more complicated :stuck_out_tongue_winking_eye:
```

---
## \#9 Posted by: joaosoprano Posted at: 2017-03-17T14:23:15.687Z Reads: 77

```
ahah :p but I figured my problem. Basically I was mixing a stactic problem and a dynamic one. Your weight will only influence going up hill, otherwise it's only influence is on how fast you can accelerate.
```

---
## \#10 Posted by: joaosoprano Posted at: 2017-03-17T16:05:33.787Z Reads: 69

```
between these three motors do you have any opinions?

http://alienpowersystem.com/shop/brushless-motors/alien-6355-outrunner-brushless-motor-190kv-2200w/
diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html 
(was hoping to find a sk3 motor with 190kv (6354) but they seem to have gone extinct)
```

---
## \#11 Posted by: GIP_longboard Posted at: 2017-03-17T18:56:56.786Z Reads: 57

```
You used g wrong, this calculation means you would accelerate at 9.81 m/s^2 in the horizontal direction (neglecting forces such as air resistance (~v^2) and drivetrain resistance), which is accelerating at 1G. This would me the torque required to counter actgravity and drive up a 90° wall for example (impossible in reality, but you know what i mean :wink: )
```

---
## \#12 Posted by: joaosoprano Posted at: 2017-03-17T19:26:30.844Z Reads: 54

```
I know x) after posting I just drew a FBD and realized how stupid I was beeing x) still haven't realized how to calculate the minimum torque needed to move the inertial load tho
```

---
## \#13 Posted by: GIP_longboard Posted at: 2017-03-17T19:31:41.498Z Reads: 50

```
In theory, even the smallest torque would suffice if you just want to move horizontally. Your acceleration would just be very low. In practice, you cant neglect friction resistances, so you would have to know the static resistance in your drivetrain (bearings etc.), which you have to overcome before you can start moving. Air resistance can be neglected at low speeds unless you try to ride it "against" the wind. id say: choose a desired acceleration (like 5m/s^2 or whatever) en then calculate the torque from there and just add a little safety factor. Determining all resistances is way overkill in my opinion :slight_smile:
```

---
## \#14 Posted by: saul Posted at: 2017-03-17T19:33:22.334Z Reads: 46

```
It's not a simple problem. You need to account for rotational energy. And some other things I can't remember from physics class....

Just keep in mind that these motors make plenty of torque! It's more a matter of balancing torque/Speed/range. With battery voltage, motor kv, wheel size and gearing.
```

---
## \#15 Posted by: joaosoprano Posted at: 2017-03-17T20:36:09.084Z Reads: 48

```
after dweling on the subject a little more I began to notice that all the problems in my head trying to start the math were all solved by simply adding a higher safety factor (to account for all the losses). My problem was realy trying to determine a torque that could always start the ride without having to push. Thanks a lot for your answers!
```

---
## \#16 Posted by: joaosoprano Posted at: 2017-03-17T20:39:55.611Z Reads: 49

```
Yeah I know, but since I don't have a lot of money to spend on my build I was trying to understand what and why I was buying some things, and it smeed like no one really accounts for the weight of the rider. And that was really bugging me. Now I realize the error in my thought process. Thanks for your answer!
```

---
## \#17 Posted by: e-Octo Posted at: 2017-03-17T21:28:41.852Z Reads: 49

```
Especially if you plan to go dual motor later - i would get the DIYes motor listed (190kv) but the 6355 vs 6374 - the shorter length will allow you to do dual rear later.  if you go the 6374 motor length - you'll have to dual diagonal if later you want to add a second motor.

I would suggest 10s, 190kv, 14/36 (motor/wheel teeth).  with your 80mm wheels this would be a good setup with top speed around 24mph/40kph.  Plenty fast IMO.

If you try to go up a steep hill - you might walk... but on the flats - plenty of speed and power.
```

---
## \#18 Posted by: joaosoprano Posted at: 2017-03-17T21:46:07.264Z Reads: 48

```
my only problem with DIYes is that the listing price is 90€ but they charge 40€ of shipping to Portugal. that's why I was looking into Alien Power System, but honestly don't want to buy a crappy motor. I got kinda cold feet after reading a thread where Jason trashed their motors
```

---
## \#19 Posted by: e-Octo Posted at: 2017-03-17T21:50:48.669Z Reads: 49

```
they are mostly the same motors. Are there issues and failures?  Yes.  But considering it's likely only a handful of companies in China who make the motors and then re-badge them as 100's of other companies...  If the APS one is closer or cheaper, or easier - i'd suggest you get it.

Jason boasts all of his products are "the best" - it's part marketing and part his passion.  Which i appreciate, but take with a grain of salt.  He likely did spec some better tolerances or parts or bearings...  but that doesn't necessarily mean the others are crap.  diminishing returns and you can always get a spare motor from Hobbyking when they pop-up and are available...
```

---
## \#20 Posted by: joaosoprano Posted at: 2017-03-17T22:01:57.775Z Reads: 43

```
I think I'll take your advice. On the setup in general I am going to do what people are recommending and go with a 10s, 190kv, 14/36. This is always going to be a work in progress (I have big plans: want to eventually use sensors and make an app to control it and read data from the skate), I just wanted to make sure that my first step would allow me to have a nice board that wouldn't be a disappointment - ever since I discovered this all I wanted was to get one for myself. 

Thanks everyone! You've all been most helpfull.

Greetings from Portugal
```

---
## \#21 Posted by: sl33py Posted at: 2017-03-17T22:53:03.505Z Reads: 41

```
don't forget to use 12mm or 15mm wide belts/gears.  A single motor setup on 9mm will skip...  When accelerating or braking hard for sure.
```

---
## \#22 Posted by: Michaelinvegas Posted at: 2017-03-18T01:37:53.754Z Reads: 35

```
Man you guys make me feel dumb 🤡
```

---

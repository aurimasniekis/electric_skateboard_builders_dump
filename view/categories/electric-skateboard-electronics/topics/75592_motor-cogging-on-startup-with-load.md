# Motor cogging on startup with load

### Replies: 28 Views: 720

## \#1 Posted by: legend27 Posted at: 2018-11-22T17:04:01.017Z Reads: 160

```
Hello everyone!

I've seen quite a few people having the same issue as me, but I couldn't find a solution that worked for me so here I am.

When accerlerating without any load there is no problems, but with load the motor dosen't accelerate that well. The motor starts cogging and the VESC makes some sounds. Here is a video I made that shows the issue.

https://www.youtube.com/watch?v=RtoqqC2JDHs

And here is my VESC settings.

https://www.youtube.com/watch?v=9r7ovni2wDc

Realtime stats when accelerating

![Realtime|690x370](upload://ahjBN9OhiFbj4VbGTzy2kdQYEc7.png) 

Any input will be appreciated :slight_smile:
```

---
## \#2 Posted by: amazingdave Posted at: 2018-11-22T17:09:36.853Z Reads: 147

```
What KV, battery and gearing are you on?
```

---
## \#3 Posted by: legend27 Posted at: 2018-11-22T17:11:23.079Z Reads: 146

```
My motor is the 6355 190KV from TB. Vesc is from TB. Battery is 10S6P 30Q. Gearing is 36 on wheel pulley and 16 on motor pulley. So gearing is 2.25 if im right?
```

---
## \#4 Posted by: amazingdave Posted at: 2018-11-22T17:13:59.830Z Reads: 145

```
I was thinking maybe the gearing was steep but that sounds ok to me... it’s acting like sensorless but your settings look ok. 

maybe someone else can offer sage words.
```

---
## \#5 Posted by: legend27 Posted at: 2018-11-22T17:24:29.481Z Reads: 139

```
![Realtime|690x370](upload://ahjBN9OhiFbj4VbGTzy2kdQYEc7.png)
```

---
## \#6 Posted by: legend27 Posted at: 2018-11-28T18:42:53.192Z Reads: 128

```
bump

10char
```

---
## \#7 Posted by: torqueboards Posted at: 2018-11-28T19:32:09.724Z Reads: 125

```
You should just give it more throttle and it should give you more power.
```

---
## \#8 Posted by: bevilacqua Posted at: 2018-11-28T19:51:01.932Z Reads: 126

```
Are you sure that you performed that sensor detection well?

Mind sharing the hall sensor values (I see the same value on your video)
```

---
## \#9 Posted by: Hummie Posted at: 2018-11-28T20:20:18.919Z Reads: 124

```
Maybe increase the amp settings. Always works for me.  Looks like 20 max motor amps on the graph.
```

---
## \#10 Posted by: legend27 Posted at: 2018-11-29T19:57:01.865Z Reads: 117

```
You're right. It looks like the max amps is 20 on the graph. I've set the max amps in general settings to 70 and 40 though?

![vesc|690x124](upload://h6p7XDCupBumpY9TYJG03OwcS9v.png)
```

---
## \#11 Posted by: legend27 Posted at: 2018-11-29T20:06:27.422Z Reads: 114

```
Think I do perform the sensor detection correct. Here is a video of it.

https://www.youtube.com/watch?v=_6YyvbaqepY&feature=youtu.be
```

---
## \#12 Posted by: bevilacqua Posted at: 2018-11-29T20:11:43.020Z Reads: 111

```
![image|551x309](upload://muY8Uj6xwGmUQ8LPkbcjVl5BVcP.png) 

these are my values, yours are much lower. 

Can anyone confirm that the values from the video seem ok?
```

---
## \#13 Posted by: legend27 Posted at: 2018-11-29T20:15:11.447Z Reads: 106

```
wow. there is a big difference.
```

---
## \#14 Posted by: Fiori Posted at: 2018-11-29T20:32:22.074Z Reads: 102

```
Are you sure you are actually writing the config to the vesc? Seems like its on the default config.
```

---
## \#15 Posted by: linsus Posted at: 2018-11-29T20:35:28.841Z Reads: 101

```
There will always be some cogging if you're using an unsensored motor. As someone mentioned above applying bit more throttle usually does the trick. When standstil the vesc has no reference of motor position so it attempts to make it spin very slightly.. Ones it traveled abit youll take off. As you mentioned theres no problem starting with a little speed. Since the motor is already spinning the vesc gets feedback right away.
Youll notice starting from standstil with some incline is even worse. 
If this is brothering you i sudgest using a sensored motor.
```

---
## \#16 Posted by: legend27 Posted at: 2018-11-29T20:39:27.114Z Reads: 103

```
Just tried running my motor in FOC mode. Off topic: WOW IT'S QUIET!

Still same issue.
https://www.youtube.com/watch?v=fk7NkSbBB9g

![FOC%20mode|690x364](upload://so7w5Ro0plC0mrpIZOiFPnRqBz0.png) 

@bevilacqua Are you running FOC? Tried to run the detection under FOC mode and get some results close to yours. I normally run BLDC

![FOC%20detection|690x387](upload://uDyJ95qjW7VL3xREzuq9fYBI2Bl.png) 

@Fiori
Im pretty sure I am. It's says in the buttom right "MC CONFIGURATION  UPLOADED"

@linsus
The motor is sensored. That's the issue. If it was unsensored I know it would be completely normal, but since it isn't, I don't want that issue to be happening. 

![sensored|521x298](upload://adktD7jp6Iu0wZS0J1TD5FDmEMU.png)
```

---
## \#17 Posted by: bevilacqua Posted at: 2018-11-29T20:43:03.408Z Reads: 97

```
yes FOC, maybe thats why. 

Sensored FOC should be much smoother on startup than Sensored BLDC. 

What vesc HW/Vendor are you running? 10? or 12S?
```

---
## \#18 Posted by: legend27 Posted at: 2018-11-29T20:44:36.546Z Reads: 96

```
HW= 4.12
FW= 3.38
Vendor: DIYELECTRICSKATEBOARD
Battery: 10S
```

---
## \#19 Posted by: bevilacqua Posted at: 2018-11-29T20:47:46.111Z Reads: 94

```
try to run FOC, apparently TB-Vescs can run FOC @ 10S. Other than that it appears that everything was fine after all. Just BLDC on a single setup
```

---
## \#20 Posted by: torqueboards Posted at: 2018-11-29T20:55:45.864Z Reads: 90

```
@legend27 I'm still not sure what you're issue is? Is it just cogging at start-up?
```

---
## \#21 Posted by: legend27 Posted at: 2018-11-30T06:53:54.457Z Reads: 85

```
@torqueboards It was hard to see in the video, but when accelerating, I could feel the motor trying to move. It couldn't move because I put some pressure on the wheel.
Don't know if that's just how it has to be and there is no problems in foc.
I will try later to run it in foc and stand on to see if it actually works (should probably had done that instead of just grabbing the wheel). Just don't know how good I feel about running in foc mode if it turns out it works.

And yes, the motor is cogging at start-up in BLDC mode.
```

---
## \#22 Posted by: meesie Posted at: 2018-11-30T09:44:42.012Z Reads: 82

```
BLDC always has cogging if you’re trying from a standstill. Try sensored FOC. It gives the best standstill-startup.

Your gearing is also very steep. Are you going for very high topspeed? If not you could try to reduce it by at least 1 tooth, maybe two.

I’ve had 12S 190KV and my gearing was 15/36. I’ve reduced it to 12/36 to match the stopspeed i wanted. It gave me so much more torque, really a big difference.
```

---
## \#23 Posted by: legend27 Posted at: 2018-11-30T10:43:13.470Z Reads: 79

```
Also when you're running BLDC Sensored? I will try FOC but I don't feel that safe using it. I've heard a lot of people having trouble with FOC mode on the TB vesc and then on the other hand, I have heard a lot of people using FOC mode on the TB vesc without any problems. 

There is two things I don't understand in the esk8 and sk8 world. 1. Bushings 2. Gearing
Why would it help on the cogging if I got more torque? Which gear should I reduce (wheel or motor pulley)?
```

---
## \#24 Posted by: dareno Posted at: 2018-11-30T11:05:24.246Z Reads: 76

```
Sensors are for non skating pussies.  All you need is a little hip flick to go smooth.  From a complete standstill to crazy with just a small movement.  Crack on!
```

---
## \#25 Posted by: meesie Posted at: 2018-11-30T11:36:27.487Z Reads: 72

```
Sensors are for people that like good startup, more efficient motors, and better low speed braking :unamused:

If you lower your motor gear it will make it easier for your motor to propell you. 
Fill in all your specs on this website and see what it does for you http://calc.esk8.it/
It doesnt show torque, but if your max speed is close to what you’d want it to be, your torque will be fine.

Remember this rule:
Torque and speed are related. More topspeed = less torque, less topspeed = more torque.

For your startup issues you’d want more torque
```

---
## \#26 Posted by: torqueboards Posted at: 2018-11-30T13:30:56.679Z Reads: 70

```
I think you're probably just not use to it or not giving it enough throttle. You get a bit of cogging but it's pretty minimal. You can always set it up in FOC if that's something that you prefer. Just make sure to watch a few videos on how to setup in FOC.
```

---
## \#27 Posted by: BruSkater Posted at: 2018-12-03T15:52:27.970Z Reads: 61

```
Were you able to fix it @legend27?
```

---
## \#28 Posted by: legend27 Posted at: 2018-12-03T18:26:59.312Z Reads: 50

```
Unfortunately no. But I have neither not tried the last recommend solutions. I will try again when I get done with my board. Right now it's completely disassembled. Will update when I try again :slight_smile:
```

---

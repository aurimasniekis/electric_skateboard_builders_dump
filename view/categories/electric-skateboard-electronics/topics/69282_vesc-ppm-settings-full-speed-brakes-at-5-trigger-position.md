# VESC PPM Settings Full Speed/Brakes at 5% Trigger Position

### Replies: 16 Views: 275

## \#1 Posted by: Marsl187 Posted at: 2018-09-26T17:31:30.628Z Reads: 101

```
I build a dual setup Boosted Board Clone.
10S2P
2x6355 190Kv Flipsky Motors
2xVESC 4.12 Flipsky
Orangatang Caguama 80A
Caliber Trucks
13/36 gearing

So the problem I have is by configurating the remote and the PPM settings. It works as I did it like in the VESC Tool instructions but in my opinion it works like shit.

So the thing is that you give maybe 5-10% of full throttle. The board starts and then accelerates to its maximum speed by still holding 5-10% trottle position. Even worse with braking, you want to brake smooth but after like 1 or 2 seconds it applies full brakes. 

My aim is that 50% throttle means 50% of fullspeed. 
My remote also has a second speed mode where the value (ms) is limited to 70%. As it works now this is completly useless. 

In the VESC Tool it looks like this:
https://www.youtube.com/watch?v=rlUYQzfyI5I

Can someone help me with configurating the PPM settings correctly?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-26T18:02:28.569Z Reads: 98

```
In the video you just give 20% throttle, right?
Do i only hear it wrong or first one motor spin and after 2-3seconds second motor spins?
```

---
## \#3 Posted by: luv2sk8te17 Posted at: 2018-09-26T18:12:30.372Z Reads: 97

```
Go to "wattage" tab which is under "general" in the motor section and change the positive/negative wattage to the same as what your motors can handle.
```

---
## \#4 Posted by: Marsl187 Posted at: 2018-09-26T18:53:49.934Z Reads: 90

```
yes, sometimes one motor starts later, also under very low throttle one stops to spin already while the other still spins slowly... connected over canbus
```

---
## \#5 Posted by: luv2sk8te17 Posted at: 2018-09-26T19:24:15.030Z Reads: 87

```
Did you name one a slave and one a master?
```

---
## \#6 Posted by: Marsl187 Posted at: 2018-09-26T19:25:25.291Z Reads: 85

```
sure! Did everything like in the Vesc Tool tutorial...
```

---
## \#7 Posted by: Jmding Posted at: 2018-09-26T20:04:45.499Z Reads: 80

```
Are you using Watt or Current control?  These behave like a car gas pedal: more trigger = more force.  That means that if you are traveling on a flat, smooth surface, even 5% trigger will eventually accelerate you to full speed (ignoring rolling resistance and air resistance), just slowly.  It sounds like you want PID Speed control, where 5% trigger will be 5% top speed regardless of whether you are climbing up a hill or going down it.  Its easy to make the switch, it's just one of the drop down options under control mode.
```

---
## \#8 Posted by: strattos Posted at: 2018-09-26T20:19:47.024Z Reads: 71

```
Yeah this is exactly how current control works and the safest most intuitive way to control a board. On the bench it seems dangerous and unsafe but when loaded it behaves properly.

Just imagine lifting a car up and giving it a little amount of throttle. The wheels will keep accelerating until they reach an equilibrium.
```

---
## \#9 Posted by: Marsl187 Posted at: 2018-09-26T20:26:49.272Z Reads: 63

```
Current Control...
I tried PID and Duty Control already, the behaviour of the motors is just wierd. Especially in PID... they start spinning when you hit full brake and release then. Duty control did not work as well...
Do I have to set the parameters of the remote different then? (max,min,center)
```

---
## \#10 Posted by: Marsl187 Posted at: 2018-09-26T20:28:28.555Z Reads: 61

```
I rode it yesterday, the behavior was the same while running... braking almost unpossible. Maybe my limits for breaking were to high? motor min was -30A each
```

---
## \#11 Posted by: luv2sk8te17 Posted at: 2018-09-26T22:06:46.368Z Reads: 61

```
Whats your motor braking regen. Posting your settings will help people see your problem and therfore help you more.
```

---
## \#12 Posted by: luv2sk8te17 Posted at: 2018-09-26T22:22:49.901Z Reads: 60

```
Did you try going to the wattage tab like I suggested earlier? Doing so fixed my 5% full throttle issue. When you set his value to let's say 2500w because your motor is capable of 2500w, this makes full throttle the 2500w and 0 throttle 0w. Total proportions in between so you can be more precise.
```

---
## \#13 Posted by: strattos Posted at: 2018-09-26T23:11:04.532Z Reads: 59

```
Hmmm duty cycle is exactly the mode you are describing eg. 50% trigger throttle=50% of motor throttle. But this weirdness you describe is the reason why current control came to be.

Are you using a custom throttle curve or are you just using a linear throttle control with that remote? 

What do you mean by braking being almost impossible? Just to sensitive or no braking force? 

I run 60/-60 motor max so that really shouldn't be the issue. 

My best guess is low travel remote combined with a linear throttle curve=one twitchy ass remote/board that's sketchy to ride.

That is unless your remote has issues/isn't configured correctly. But I'm guessing you verified your ppm settings and made sure that 100% on the remote matches 100% on vesc.

As well you are supposed to calibrate these remotes everytime you powering them on by giving full throttle and brake, however again I don't think this is it.
```

---
## \#14 Posted by: ksfacinelli Posted at: 2018-09-26T23:34:27.516Z Reads: 54

```
What is your dead band set at if it is 15 drop it down to 3 or 4%
```

---
## \#15 Posted by: luv2sk8te17 Posted at: 2018-09-26T23:55:42.407Z Reads: 53

```
Try adding negative expo for softer throttle
```

---
## \#16 Posted by: Marsl187 Posted at: 2018-10-18T19:24:47.408Z Reads: 39

```
Thanks for all the answers. 
I could not test all these things because I had to wait for new parts.
The problem was that my current limits for the battery were too high in comparision to the max speed.
Now with different gearing it works quite well.
A little bit of throttle curve with neg expo work fine
```

---

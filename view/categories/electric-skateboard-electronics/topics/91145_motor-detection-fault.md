# Motor detection fault

### Replies: 22 Views: 326

## \#1 Posted by: Domj42 Posted at: 2019-04-19T18:59:35.178Z Reads: 70

```
Hi all I’m quite new to electric skateboards and have a basic understanding mostly due to others hard work.
I have an issue with my board which I can’t solve 
Today I took the board out running slow as my daughter was following on bike, as I was slowly braking it just died !! 
I have fully charged batteries 2 x 6s 22.2v 3300mah lipos they read at the moment 49v
Flipsky fsesc v4.12 lights on receiving power all connecting to laptop 
Torque boards 6355 190kv motor, tested resistance 0ohms 
So when I pull trigger green light on esc 
I cannot find any visible issues anywhere I have checked and double checked connections all are good 
But nothing happens to motor 

I redone the set up wizard just in case and it just says motor detection fault 
Real-time data shows nothing 

A little history for those still reading 😂

Recently I added a flipsky smart anti spark switch this seemed to work when installed but little did I know that power was still running to board so completely drain 2 6s 22.2v 5200 mah batteries killing them..
So I removed the not so smart switch and replaced batteries and went back to an xt90 anti spark loop key
I used the board twice and then just died. 

So any ideas or help on testing if power is being sent out of esc would be helpful
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-19T19:37:58.918Z Reads: 59

```
If you have a multimeter you can check the resistance of all combinations of phase wires (a to b, a to c and c to a). The resistance should be very low but the same in all combinations. Also check if no any of the phase wires have a short to the motor mount or ground as well.

Make that before you do another motor detection. If you have a short in your phase wires you can broke your vesc by doing a motor detection.

When you did the motor detection, the motor was as min turning or rattling, or didn’t do anything at all?

Just to double check, there also no red lights in the vesc after you did the motor detection, right?
```

---
## \#3 Posted by: Domj42 Posted at: 2019-04-19T20:00:33.751Z Reads: 53

```
Hi Andy thanks for replying.

I’ve checked with multi meter the 3 phase wires on the motor and I get 0 in all combinations
I’ve now checked the 3 phase wires from the Vesc and I get around 81.0 on all combinations although slight differences.
There is no red light there is a constant blue and green 
And when running detection I get brighter green which comes on assuming that’s it sending power to motor 
Which is same as when I pull trigger on controller.
```

---
## \#4 Posted by: Domj42 Posted at: 2019-04-19T20:07:50.485Z Reads: 39

```
I did just check resistance on the terminals ( solder points )on the Vesc and I got 0 resistance !
Does this mean I could have a break in connection on wire between solder point on board and connector?
```

---
## \#5 Posted by: Andy87 Posted at: 2019-04-19T20:10:34.066Z Reads: 39

```
If it would be a break your multimeter would show open end and not 0 ohm.
```

---
## \#6 Posted by: Domj42 Posted at: 2019-04-19T20:11:17.171Z Reads: 36

```
Scrap that last just checked reactance on each and get 0 so wire ok grrrr 🤔
```

---
## \#7 Posted by: Andy87 Posted at: 2019-04-19T20:13:59.971Z Reads: 36

```
And you say that after you get the message „bad motor detection“ there are no any faults written in the terminal right?
```

---
## \#8 Posted by: Domj42 Posted at: 2019-04-19T20:15:00.344Z Reads: 36

```
![image|374x500](upload://hpIQ64197TzDjPW20AnimZmjZ10.jpeg)
```

---
## \#9 Posted by: Domj42 Posted at: 2019-04-19T20:15:36.573Z Reads: 32

```
Yes that’s what I get
```

---
## \#10 Posted by: Andy87 Posted at: 2019-04-19T20:16:22.439Z Reads: 34

```


Did you do motor detection with belt and wheels on or without?
```

---
## \#11 Posted by: Domj42 Posted at: 2019-04-19T20:18:53.436Z Reads: 31

```
I tried both, the annoying thing is that is was working fine, did a couple of miles I’ve 2 days just short run to shops, and it just stopped working so settings were ok for it to run 
But it’s not even attempting to spin up motor not a flinch
```

---
## \#12 Posted by: Andy87 Posted at: 2019-04-19T20:21:38.366Z Reads: 30

```
Did you also try bldc as well as foc. Maybe one of the both get the motor detection running.
```

---
## \#13 Posted by: Domj42 Posted at: 2019-04-19T20:23:30.292Z Reads: 26

```
I tried both Foc detected motor but didn’t run motor 
I’ll try again now
```

---
## \#14 Posted by: Domj42 Posted at: 2019-04-19T20:27:14.318Z Reads: 31

```
![image|374x500](upload://iU1lPBkUL8U2zbJiHCwnXxRGmBB.jpeg) 
It said motor would make noise and then motor would spin but motor did nothing 
But I got green so assuming it detected motor?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-04-19T20:30:50.439Z Reads: 30

```
If it’s green it should be good. Can’t you apply that settings and continue with the wizard?
```

---
## \#16 Posted by: Domj42 Posted at: 2019-04-19T20:31:14.813Z Reads: 32

```
![image|374x500](upload://77QZCpaVfqGtqWLWPl3VSpEqpvB.jpeg) 

Sorry missed one step and this is what I got
```

---
## \#17 Posted by: Andy87 Posted at: 2019-04-19T20:33:15.365Z Reads: 30

```
Disconnect the sensors and try to set your motor up sensorless.
```

---
## \#18 Posted by: Domj42 Posted at: 2019-04-19T20:36:24.045Z Reads: 28

```
Unfortunately I’ve tried that already as well
```

---
## \#19 Posted by: Andy87 Posted at: 2019-04-19T20:39:44.267Z Reads: 28

```
You also can’t spin up the motor with the arrow taps on your pc?
```

---
## \#20 Posted by: Domj42 Posted at: 2019-04-20T19:25:07.669Z Reads: 23

```
Sorry couldn’t answer as wrote maximum replies as new use lol

No arrow tabs do nothing either.
Unfortunately I don’t have spares or I could swap out either motor or fsesc and eliminate that way. 
I really don’t want to buy the wrong bit. 
Any other ideas to find which is at fault?
Is there a way to spin up the motor without an esc? 
I noticed slick revolutions are close to me might pop in there in the week and see how helpful they are.
```

---
## \#21 Posted by: Andy87 Posted at: 2019-04-20T20:11:10.850Z Reads: 20

```
Maybe you have somebody around you who could borrow you some esc to check what’s the issue?

What’s your settings for battery cut off? Maybe those are too low? Really not so easy case 😅
```

---
## \#22 Posted by: Domj42 Posted at: 2019-04-20T20:43:11.662Z Reads: 19

```
I’ve asked on fb so maybe someone will be close hopefully.
I’ve checked battery settings and all above so no I guess I need hardware to check 

Thanks for you help 
The mission continues lol
```

---

# Abs over current fault while full throttle, 8s, directfet VESC

### Replies: 6 Views: 166

## \#1 Posted by: Szosiem Posted at: 2019-06-23T14:37:37.070Z Reads: 43

```
Hi there! Here is my first post about my board. I have been browsing the forum for 3 years. Now I've decided to create an account, cause I cannot find answer to my problem. Recently I've finished build of my mountain like longboard (well... some Polish roads are terrible :wink: ). This is my second attempt - first one was almost the same (one year ago), but with smaller wheels. 

**TL;DR:** ABS OVER CURRENT error at full throttle, asymmetrical power cables from batteries - is that a problem?

**Long story:**
Yesterday I made a test drive. I was slowly spinning up longboard and when I was at full throttle, the engine stopped (and I fell off the skateboard). It happened only once, since I was afraid of falling again :worried: I had something around 24 kmph (15mph).

I connected the VESC to the computer and in the terminal I had only one error:

    Fault            : FAULT_CODE_ABS_OVER_CURRENT
    Current          : 148.0
    Current filtered : 132.6
    Voltage          : 29.44
    Duty             : 0.005
    RPM              : 27178.5
    Tacho            : 1053289
    Cycles running   : 623544
    TIM duty         : 265
    TIM val samp     : 132
    TIM current samp : 26714
    TIM top          : 53164
    Comm step        : 1
    Temperature      : 53.86

I have tested the motor with multimeter, battery connection, VESC (visual contition) etc. and everything seems fine. In the first build I had exactly the same problem, but in Turnigy 4.10 VESC. After switching to directFET VESC problem still occur. Both VESC's were send to manufacturer and they passed their tests.

Today I gave another try and the same problem appeared on around 85% of throttle ... No DRV errors encountered.

**Some ideas:** 
Maybe someone have an idea what is wrong with this build. I suspect the battery problem but I cannot find any information about different lengths of a cables. In my configuration positive one has 38 cm (14.9 inch) AWG10 and negative one has 63 cm (25.6 inch) AWG8. I have spent a lot of time on forum to find similar posts, but most of them were connected with VESC hardware problem.

Another suspect: motor. I tried detection again and at the first time value of BEMF Coupling was around 900, but now measurement is around 760. Problem still occurs. 

**Setup:** 

    5065 Outruner 270KV (measured 240KV) 1665W in BLDC mode
    DirectFET VESC 4.12
    8s8p LiIon battery (LG MH1)
    Gear ratio 15 / 56 HTD-5M

**Pictures of board:**

![IMG_2039|666x500,100%](upload://vwRKl42XGTn2h3jn6JIUdcWiyTF.jpeg) 

![IMG_2041|666x500](upload://ql8p4CG4T0fob84hmUxWfnrdR5X.jpeg) 

**Pictures of VESC Tool:**

![53|690x420](upload://4EJtqGqv3owz6aqDLjqzle6auxC.png) 

![57|690x420](upload://v6Oa3SWmlvXx9yqcHnQmOMCXnA1.png) 

Thank you for reading this post and I'm counting for your help! :smile:
```

---
## \#2 Posted by: Bataleon Posted at: 2019-06-23T16:14:39.920Z Reads: 30

```
[quote="Szosiem, post:1, topic:97162"]
In my configuration positive one has 38 cm (14.9 inch) AWG10 and negative one has 63 cm (25.6 inch) AWG8. I have spent a lot of time on forum to find similar posts, but most of them were connected with VESC hardware problem.
[/quote]

I think your question should become the template for all future questions. Really nice info you provided :D

The long battery leads could very well be the reason for the issue. Longer leads = higher inductance = more for the capacitors to deal with, which could lead to `FAULT_CODE_ABS_OVER_CURRENT`.

I would try and shorten them and see if the problem persists. You could also try bringing your motor max current down a bit (closer inline with battery max current) but that would lower your acceleration.
```

---
## \#3 Posted by: Szosiem Posted at: 2019-06-23T18:41:02.184Z Reads: 29

```
[quote="Bataleon, post:2, topic:97162"]
I think your question should become the template for all future questions. Really nice info you provided :smiley:
[/quote]

Thank you. I wanted to make nice and clear post with all required info and observation ;)

[quote="Bataleon, post:2, topic:97162"]
The long battery leads could very well be the reason for the issue. Longer leads = higher inductance = more for the capacitors to deal with, which could lead to `FAULT_CODE_ABS_OVER_CURRENT` .
[/quote]

Yea, I would like to test it out, but the main problem is configuration of the batteries. Negative cord is at the end of enclosure, and positive is at beginning.

I realized right now, that my friend have some Li-Ion batteries to another project. I will borrow them, connect in 8S1P and check if that fixes a problem. I need to prepare myself to fall down. That's awful thought. 

[quote="Bataleon, post:2, topic:97162"]
You could also try bringing your motor max current down a bit (closer inline with battery max current) but that would lower your acceleration.
[/quote]

Going to try this too, even if present acceleration is very crappy :frowning: For real, this engine make noises like it going to die (or like small electric cars for kids :joy: ). I know it's cause of using BLDC ;)
```

---
## \#4 Posted by: Szosiem Posted at: 2019-06-23T23:31:50.368Z Reads: 25

```
I lowered value for motor down to 40 Amps. I gave it a try and surprisingly no error during test around house. I slowly increased speed to around 20kmph (12.4mph) and then kick throttle to full value for few seconds. Tried dozen times - still no faults and acceleration is smooth. Going to check it at longer trip soon, but now my leg need to rest after falling off a deck :expressionless:
```

---
## \#5 Posted by: Darkie02 Posted at: 2019-06-24T06:46:42.766Z Reads: 17

```
Interesting result I had a dule set up at 35 motor 25 battery had the same issue had a motor issue and reset it up as single drive 55 battery 55 motor not had a fault since. I put it down to a faulty motor but now I’m wondering if it was both.
```

---
## \#6 Posted by: Szosiem Posted at: 2019-06-24T13:06:02.158Z Reads: 13

```
I think the motor is broken. My friend was driving and it cogged while was accelerating slowly to full throttle without throwing any faults ... Need to buy sensored one because I don’t want to make an accident.
```

---

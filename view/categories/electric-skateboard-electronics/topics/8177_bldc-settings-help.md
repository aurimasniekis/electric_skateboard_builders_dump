# BLDC Settings Help

### Replies: 10 Views: 802

## \#1 Posted by: Mikenopolis Posted at: 2016-08-23T16:42:29.983Z Reads: 101

```
I apologize for being a total n00b at this.

I have the Enertion 6374 motor (is it 6372 or 74? is says 74 on Enertion's site) and a Spacecell Pro 4 (10S). Using the Winning remote and receiver.

I have my Motor Max set to 60. From what I read that gives it a smoother acceleration which is what I want. The problem I have is that on the remote, I stop accelerating about 3/4 way on the throttle. What would I have to adjust so that let's say Neutral is 0mph, Middle is 15mph and Full is 30mph. I don't like that the last 1/4 of the throttle does nothing.

Thanks for the help everyone
```

---
## \#2 Posted by: Namasaki Posted at: 2016-08-23T17:15:23.837Z Reads: 91

```
Calibrate your remote and receiver with Vesc. 
https://youtu.be/OtuofrQr3F8
```

---
## \#3 Posted by: Mikenopolis Posted at: 2016-08-23T17:43:55.998Z Reads: 86

```
THANK YOU THANK YOU! Exactly what I needed. I was looking at esk8 support's videos with the screwed up audio to get my current setting. this one make more sense
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-08-23T17:48:06.010Z Reads: 80

```
something else you can do to make your acceleration a little less aggressive is lower your motor max to something like 50 so that it takes a little bit longer to top out, that will also have an affect on where you are on the throttle vs where you are in speed.
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-23T18:30:58.273Z Reads: 75

```
If you're running current control there's unfortunately no way to make various positions of the throttle run at a set speed. You're supplying varying amounts of current to overcome resistance, and once that resistance has been overcome, you will go max speed.
```

---
## \#6 Posted by: ra.rend Posted at: 2016-08-23T18:58:22.292Z Reads: 72

```
how do you make various throttle position run at set speed?
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-23T19:00:51.461Z Reads: 70

```
Use PID speed control or Duty Cycle. However, these options leaves you with the inability to coast. Neutral throttle will result in braking.

This is what I'm hoping for in VESC 6

http://www.electric-skateboard.builders/t/will-the-vesc-6-0-support-duty-cycle-current-control-hybrid/7636/9
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-08-23T19:13:18.578Z Reads: 67

```
The behavior @Jinra describes is definitely not what you want on an esk8. You want a trigger or thumb stick that behaves more like a gas pedal and allows you to decide how much current to throw at the motors in a more organic way based on feel, and you need to be able to coast. Setting it up so that speed mirrors your  thumb/finger position exactly with the neutral being a brake will cause you to street your face. Neutral is a position that the throttle wants to spring back to. If your thumb/finger slips you're eating pavement.
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-23T19:25:58.123Z Reads: 61

```
I agree, though my Evolve gt  uses duty cycle with great current control. Speed is determined by throttle position but neutral still lets you coast.
```

---
## \#10 Posted by: Mikenopolis Posted at: 2016-08-24T15:55:44.491Z Reads: 41

```
I worked on BLDC setting last night and did what the above video showed, but I'm still getting max throttle at about the 3/4 way up. Also the brakes don't work every time, I would pull the lever forward, then back and the wheel would still be going, brake would engage when I push forward and back a second time.

Do I have a faulty remote or is that just the way a DIY board is
```

---

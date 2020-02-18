# Belt crimps up when motor &amp; wheel spin

### Replies: 22 Views: 324

## \#1 Posted by: Anubis Posted at: 2018-11-03T12:42:56.124Z Reads: 85

```
Hey,
So i have a prebuilt drivetrain with belt tentioners, and the belt is crimping and causing extreme resistance. Additionally, the pulley hits the wheel and the motor makes a weird sound.

Belt crimping (main issue) https://youtu.be/VdJ1ZiTJ2q0

Motor noise and wheel issues https://youtu.be/mJwJ3L_OIbA
Note the grinding is not as audible while the motor is powered, but spinning it by hand almost sounds like there is chalk being ground in the motor.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-11-03T12:55:48.770Z Reads: 83

```
Can’t hear the noice as i‘m siting in a coffee place 😅 but how much space on your hanger left? I mean the nut sitting flush with the shaft?
If no you could place a 2mm thick washer on the shaft. First washer than wheel with pulley than nut.
Is it possible to release the tensioner a bit?
Just to get your belt a bit more lose so that you can place the motor more in the back.
```

---
## \#3 Posted by: Linny Posted at: 2018-11-03T12:57:37.648Z Reads: 75

```
If there is space, you can also push the motor pulley in a bit more, maybe around 1~2mm. It'll make the belt go in and align better than hitting the flange of your wheel pulley
```

---
## \#4 Posted by: Anubis Posted at: 2018-11-03T12:59:24.361Z Reads: 70

```
Yes i belive i can adjust tentioning and i can place that washer. Thanks for your help
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-03T13:01:49.696Z Reads: 67

```
If there is any other problem in the motor or so i‘m sorry i can’t hear the voice in your video as i‘m in a public place 😅
```

---
## \#6 Posted by: Anubis Posted at: 2018-11-03T13:04:41.741Z Reads: 64

```
Looks like 3 speedrings added on has solved the issue with the crimping though :smiley:
```

---
## \#7 Posted by: pat.speed Posted at: 2018-11-03T13:08:34.888Z Reads: 64

```
That’s good to hear. I would also recommend slackening the belts off a little by adjusting the idler pulley if it’s moveable. It will give longer life and less rolling resistance.

As for the motor it sounds like something is rubbing. I would just check that the pulley isn’t rubbing too close to the motor mount or on the motor bolts. If that isn’t the case you may need to open the motor. It’s very simple and should be done anyway every once in a while to give the motor a little clean
```

---
## \#8 Posted by: Andy87 Posted at: 2018-11-03T13:10:47.302Z Reads: 58

```
And make sure the mounting screws for the motor not too long 😅 that can end up not good. Don’t ask from where I know 😒
```

---
## \#9 Posted by: pat.speed Posted at: 2018-11-03T13:12:05.501Z Reads: 53

```
Lol, I saw that thread hah.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-11-03T13:15:34.505Z Reads: 51

```
About to fix it. Was not so bad, learn a lot about motors right now because of it.
If I manage to repair everything i‘ll write a small guide how to... think i‘m not the first one who managed to do so 😅
```

---
## \#11 Posted by: pat.speed Posted at: 2018-11-03T13:19:47.784Z Reads: 40

```
Just make sure to insulate from surrounding wires not just cover the shorts, in case two wires are touching. A tutorial sounds like a good idea
```

---
## \#12 Posted by: Andy87 Posted at: 2018-11-03T13:23:34.752Z Reads: 38

```
I‘ll check the motors and show how to find out if there are shorts in the windings etc.
After will try to repair everything that it looks and work like new. Hopefully 😅
If no i‘ll show how best to order two new 6380 motors from @torqueboards 😂😂😂
```

---
## \#13 Posted by: Anubis Posted at: 2018-11-03T14:29:19.904Z Reads: 37

```
Alright had a maiden voyage today. I had to take off a motor because the fsesc dosent fit, so for a single pnumatic board how slow will it go considering im a heavy dude? I think i got up to max 9mph with 12s5p 6374 15t. It could also be tire pressure i suppose

I think the motor is set to 60A peak in the vesc settings
```

---
## \#14 Posted by: Andy87 Posted at: 2018-11-03T14:52:52.600Z Reads: 30

```
The question is to what is your battery max value set.
Maybe it’s set too low that’s why you can’t drive faster.
Which Flipsky esc you have. 4.xx or 6.xx
```

---
## \#15 Posted by: Anubis Posted at: 2018-11-03T15:21:57.865Z Reads: 28

```
their new fsesc 6.6, and i think the battery has an 80A BMS (eskatingeu one)
```

---
## \#16 Posted by: mutantbass Posted at: 2018-11-03T15:32:54.631Z Reads: 24

```
Sorry can't help you but that accent is bloody glorious :)
```

---
## \#17 Posted by: Andy87 Posted at: 2018-11-03T15:42:21.927Z Reads: 23

```
I mean did you change the battery max value after you changed to single drive?
If it’s set to 20-30a I could be that it’s too less if only one motor
```

---
## \#18 Posted by: Anubis Posted at: 2018-11-03T15:57:41.006Z Reads: 23

```
http://prntscr.com/ldyki2 
I think these are higher values? The tires are quite deflated, but i wouldnt expect it to move as slowly as it does even with deflated tires. With no load the board will move quite fast.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-11-03T16:02:02.685Z Reads: 24

```
🤔 no values look good that’s not the reason.
Besides the battery min is very low with -40.
Would set it a bit up like -20/-30.
But it’s not the reason why you drive so slow
```

---
## \#20 Posted by: Jmding Posted at: 2018-11-03T16:22:15.955Z Reads: 25

```
What is your gearing?

Did you set an erpm limit? 

Did you calibrate your remote? 

Does it accelerate quickly up to top speed, or gradually limp up to speed? 

Did you do motor detection with the belt attached or detached?
```

---
## \#21 Posted by: Anubis Posted at: 2018-11-03T18:58:36.109Z Reads: 16

```
So I went to my local bike store and they pumped up the tires. 10000% improvement, they were the problem. It accelerates slowly, but its speedy and I am happy with the performance considering its only got 1 motor and im 200lbs. going to give it another go a little later on but im really happy so far. 

Thanks so much for all the help you've given me! Hopefully I can do the same for others someday
```

---
## \#22 Posted by: Andy87 Posted at: 2018-11-03T19:06:01.702Z Reads: 17

```
I‘m sure so 😉
Always welcome!
```

---

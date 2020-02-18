# SK8 ESC Turningy heating up , please need advice

### Replies: 29 Views: 436

## \#1 Posted by: t3hricardo Posted at: 2018-11-17T10:25:21.504Z Reads: 102

```
Hi guys, 

Sorry for another silly question, this is my first build. I connected my motor to ESC then ESC to batteries 2x 5s 5000mAh . after few seconds ESC got really warm, probably around 50C by feeling. It was just stand by, motor was not running. Is that normal ? I am bit scared as I dont want to blow it and I payed quite a money for it. ESC is SK8 turningy from hobbyking , should be able to do 12s. 

PS : I did not program this ESC even though there is an option, manufacturer says it comes already set up ready to go.
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-11-17T10:30:02.307Z Reads: 97

```
Link the esc you have please
```

---
## \#3 Posted by: t3hricardo Posted at: 2018-11-17T10:37:46.139Z Reads: 97

```
https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html
```

---
## \#4 Posted by: t3hricardo Posted at: 2018-11-17T10:52:02.864Z Reads: 92

```
also after I paired my controller , motor was just doing like clicking sound and sort of turned 1 magnet ( I think)  and I got 3 red flashes error. Could this be due to not setting it up specificaly to my batteries and motor ? still not sure about the temeperature thing though! I be happy for any advice. Thought this would be easier like connect hit remote and ride :smiley:
```

---
## \#5 Posted by: Grozniy Posted at: 2018-11-17T11:04:46.592Z Reads: 93

```
https://youtu.be/v1glLDO-EjA
```

---
## \#6 Posted by: Andy87 Posted at: 2018-11-17T11:43:29.620Z Reads: 84

```
Red lights not a good sign usually.
Make sure your vesc is hooked up with the right polarity.
Make also sure no any of your phase wires touch each other.
Maybe also upload a picture from your set up.

Without motor detection it’s normal that motor not really spin.
Watch the video @Grozniy linked too 😉
```

---
## \#7 Posted by: pat.speed Posted at: 2018-11-17T11:59:41.092Z Reads: 80

```
I think you will be lucky if you haven't fried your vesc
```

---
## \#8 Posted by: ElectricCoast Posted at: 2018-11-17T13:04:38.712Z Reads: 75

```
Sounds like you have a short.
```

---
## \#9 Posted by: t3hricardo Posted at: 2018-11-17T19:31:16.247Z Reads: 70

```
but how is that possible? no naked cables anywhere, ESC light up normally, right polarity, reciever got power too.
```

---
## \#10 Posted by: t3hricardo Posted at: 2018-11-17T20:03:34.715Z Reads: 68

```
![image|514x499](upload://sinuCOoku3plPuqFTScuXM4uI74.jpeg)
```

---
## \#11 Posted by: ElectricCoast Posted at: 2018-11-17T20:05:01.333Z Reads: 66

```
Look at the esc.  It may have a bad solder on it.  It's not out of the rhelm of possibilities that you recieved a bad sk8 esc.
```

---
## \#12 Posted by: dareno Posted at: 2018-11-17T21:28:35.733Z Reads: 61

```
If you have flashing red lights on that vesc its dead.  HK will replace it no problem if you open a fault with them.  They will require the old one back most probably.  And its always best to set it up before you use it if you're running 12s.
```

---
## \#13 Posted by: pat.speed Posted at: 2018-11-17T22:02:37.544Z Reads: 56

```
I agree. Never ever think that they have set it up for you. I could probably guarantee they haven’t set it up for that exact motor. 

You are lucky you bought from them though as they will refund the money or send a new one
```

---
## \#14 Posted by: mynamesmatt Posted at: 2018-11-17T22:06:31.975Z Reads: 53

```
is there any anti spark in there at all?
```

---
## \#15 Posted by: dareno Posted at: 2018-11-17T22:06:56.999Z Reads: 57

```
I've actually found them to be a good vesc tbh.  I only killed one due to a short and it displayed the three consecutive red flashing lights, it was purely my fault but HK replaced it without an issue.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-11-17T22:07:00.228Z Reads: 55

```
No but it’s not needed, for testing a few times
```

---
## \#17 Posted by: t3hricardo Posted at: 2018-11-18T04:43:38.639Z Reads: 50

```
guys red flashing sometimes stops , then I am able to push throttle but motor only vibrates. still dead ? sorry for noob questions , also is antispark necessary ? since I got heaps xt60 allready. I really appreciate guidance and help from u ! 

Cheers Rich
```

---
## \#18 Posted by: dareno Posted at: 2018-11-18T05:12:07.754Z Reads: 46

```

[quote="t3hricardo, post:17, topic:74987"]
guys red flashing sometimes stops , then I am able to push throttle but motor only vibrates. still dead
[/quote]
Its got a bad connection somewhere and needs replacing.  You run the risk of damaging something else if you try to use it.  You really don't want to short a lipo.  Trust me.
You need some kind of switch in there too.  Either make yourself a loop key with an xt90s or buy an antispark switch.  At the very least I would be using an xt antispark on the battery cabling to the vesc.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-11-18T06:38:51.060Z Reads: 40

```
What @dareno ☝️ said
Plus for the future, doesn’t matter what hk wrote, you need to set up your vesc by your own.
Without motor detection on the motor you use it will most likely not spin at all.
If something not working next time you can always look up the faults on the terminal in your vesc tool. If there is a red light, there should be written what’s the fault means.
```

---
## \#20 Posted by: pat.speed Posted at: 2018-11-18T06:41:41.020Z Reads: 39

```
This, you need to connect it to the computer and set it up. Otherwise it will never work. By trying to move it without detection you will just break the vesc. Please just set it up and all problems should go away. Unless it is already broken
```

---
## \#21 Posted by: t3hricardo Posted at: 2018-11-18T08:28:24.551Z Reads: 34

```
thank you guys, I try to do that! Once I figure out how and I let you know the outcome. If you dont mind me asking, I know I would probsbly find info on youtube or google, but I like talking to people, so should I connect Vesc to pc stand alone, or hooked to battery, motor and reciever as well? cheers
```

---
## \#22 Posted by: dareno Posted at: 2018-11-18T08:36:55.888Z Reads: 30

```
Fully assembled with battery connected.
```

---
## \#23 Posted by: pat.speed Posted at: 2018-11-18T08:37:40.928Z Reads: 30

```
It will need to be connected up to the motor and receiver. It is best if you can connect to a 12v power supply other than the batteries in case it is broken and shorts the battery wires
```

---
## \#24 Posted by: t3hricardo Posted at: 2018-11-19T10:32:52.722Z Reads: 28

```
![image|375x500](upload://A5nbWqy60HQSccNnsQDUosRBcK2.jpeg) ![image|375x500](upload://lF1rsgtZDwC9uTeOaLodcIz0aXa.jpeg) 

updare for interested ones. I managed to connect Vesc to pc and set it up , although Vesc was fine for a while, then got error, then fine again, so I examined it and saw this melted protective plastic in specific area, so I assume this bit is overheating for some reason( probably short) , so I did request a return, hopefully they will exchange it. Love to hear your thoughts! cheers
```

---
## \#25 Posted by: t3hricardo Posted at: 2018-11-19T10:33:56.056Z Reads: 27

```
Ps : when my motor spinned for first time, you should see that smile on my face :smile:
```

---
## \#26 Posted by: ElectricCoast Posted at: 2018-11-19T14:06:42.643Z Reads: 24

```
I figured there was a short.  HK is pretty good about returns.
```

---
## \#27 Posted by: briman05 Posted at: 2018-11-19T14:24:36.345Z Reads: 24

```
There is probably a solder bridge around the area of the melted plastic causing a short. You have to connect it to the pc when you get the vesc and motor to set it up properly if you try to use it before setting it up you will most likely kill the vesc.  You may want to invest in a better vesc as you get what you pay for when it comes to vesc generally.
```

---
## \#28 Posted by: pat.speed Posted at: 2018-11-19T19:33:47.063Z Reads: 18

```
The HK vesc is actually very good, this wasn’t a bad vesc it was damaged from not setting it up in the settings or running a motor detection
```

---
## \#29 Posted by: briman05 Posted at: 2018-11-19T19:49:36.442Z Reads: 16

```
I had never seen much talk about hk vesc but do agree it most likely was user error by not doing the motor detection
```

---

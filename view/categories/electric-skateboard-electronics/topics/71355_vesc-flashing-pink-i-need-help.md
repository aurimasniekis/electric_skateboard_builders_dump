# VESC Flashing Pink, I Need Help!

### Replies: 13 Views: 255

## \#1 Posted by: jojamcha Posted at: 2018-10-16T01:35:18.514Z Reads: 73

```
Hello! I am completely new to skateboard building and all the necessary knowledge. I just unboxed my VESC and I plugged it into my batteries, which are a set of three 2s 5000 mAh li-pos. Weirdly, my VESC glowed blue for a moment, then started blinking pink in sets of two blinks. Also, I am using a Torqueboards 6355 190kv motor, which I plugged into the VESC, will not spin when I try to run the motor detection test. I am using the latest firmware for the VESC and I am using the VESC BLDC tool too. I cant find a solution :( please help! Thanks
```

---
## \#2 Posted by: DAddYE Posted at: 2018-10-16T01:45:01.720Z Reads: 68

```
Did you flash the firmware? Are you sure you flashed the one for 4.12 HW?
```

---
## \#3 Posted by: jojamcha Posted at: 2018-10-16T01:50:11.301Z Reads: 68

```
yes, I did (I have no more replies because I am a new user so I have to wait 19 hours before I can talk again :( ) sorry everyone, ill just have to tackle this problem tomorrow sometime, but feel free to post if you have any thoughts :)
```

---
## \#4 Posted by: lrdesigns Posted at: 2018-10-16T02:04:10.644Z Reads: 65

```
Did you leave all the settings at default? If you changed the voltage range that may cause it to do this.

You can check for faults in the terminal. Follow this thread here. 
https://www.electric-skateboard.builders/t/solved-vesc-motor-not-being-detected-or-turning-red-blinking-light/7840?u=lrdesigns

Please upload some photos of your setup and screen caps of your settings and it will help us find the cause of the issue. :+1: :skateboard:
```

---
## \#5 Posted by: jojamcha Posted at: 2018-10-16T21:04:18.981Z Reads: 49

```
here are the pics of my setup (sorry about the glare)
![skate%201|640x480](upload://4QaDbhYET2VIIW0GDpfvcbJCL6Z.jpeg) ![skate%202|640x480](upload://8oHFjcMwo5CjDIRmuBV2lH2jYI4.jpeg) ![skate%203|640x480](upload://eFoswxcCWtHkEbb00f6fus1b5o8.jpeg) ![skate%204|640x480](upload://gX9Q22G5c78eisdohftETNLbmht.jpeg) 
and my settings
![skate%205|690x423](upload://hPzOmTaoq1a591I9FcmymMdueP3.png) ![skate%206|690x416](upload://v80DNWxE9l4SBARoZWFpYmsaYH0.png)
this is the answer I get when I run the motor detection
![skate%207|283x47](upload://tta9MaHHh22tJPQF9GqIwiL1i4Y.png) ![skate%208|690x416](upload://wUZZxmGAQrPt30qho1L65u2EIgv.png) 
and when I type fault in the terminal:![skate%209|318x65](upload://4BxLAQok9RR1fblUP8nwzpd7Zy.png)
```

---
## \#6 Posted by: Holyman92 Posted at: 2018-10-17T04:44:14.540Z Reads: 41

```
First off, on the battery settings, Change the drop down to reflect Lipo, not li-ion
```

---
## \#7 Posted by: b264 Posted at: 2018-10-17T05:06:17.202Z Reads: 38

```
Try raising I from 5A to 10A when you run detection and increase the duty cycle from 0.05 to 0.10, see if that helps.

Also, those current settings are too high to start with.  Try 50A, -40A,  30A, -10A to start with and adjust from there if it's too weak or strong.

"Motor Current Max Brake" is brake strength at lower speeds and "Battery Current Max Regen" is brake strength at higher speeds.
```

---
## \#8 Posted by: jojamcha Posted at: 2018-10-17T22:59:46.373Z Reads: 34

```
![skate%2011|690x495](upload://nd2DhgJyI5es5a19q7STsf96zPb.png) 
Is my motor current supposed to be that low? Also, wtf I have 6.3 volts going in. Thinking I was given 2 flat batteries. Boo Hobbyking USA
```

---
## \#9 Posted by: jojamcha Posted at: 2018-10-17T23:05:22.883Z Reads: 34

```
changing the I and duty cycle do not work. Also, the li-ion drop-down does not work either, when I click on it no drop down drops down. It just highlights in blue
```

---
## \#10 Posted by: lrdesigns Posted at: 2018-10-17T23:38:29.721Z Reads: 34

```
According to your voltage cutoff the vesc won’t do anything under 18v. If your getting only 6v then that’s why. What’s the voltage after fully charged. 

Also if you really had 6v your batteries are damaged. :persevere: 

Can you measure with multi meter just before the vesc? 

Edit. Or you have a parallel harnes instead of series? Can get a photo of the adapter between batteries and vesc?
```

---
## \#11 Posted by: jojamcha Posted at: 2018-10-18T00:26:12.609Z Reads: 32

```
![skate%2013|642x479](upload://asl51ZSi8bZr32mjqxGk9fvJe3O.png) 
The batteries are connected to the VESC via two 4mm series connectors, then to a 4mm bullet to XT90 connecter that runs to the VESC.

The measurement from the multimeter is indeed about 6.5V, same as the VESC tool. :frowning:
```

---
## \#12 Posted by: lrdesigns Posted at: 2018-10-18T01:20:59.280Z Reads: 26

```
What if you measure each battery individually? A B C

If each is 6.5v then you should get 6.5 X 3 = 19.5v

Something is weird though. The storage charge of each cell should be around 3.8v X6 = 22.8v  Your best case scenario is 19.5 / 6 = 3.25v which is quite low for lipo. I think one or more of your batteries is over discharged. Can you check each cell individually with your charger or multi meter on the balance plug?

You have two 2s series harnesses, but I'm a little confused to how you hooked it up, hard to tell like this. Can we see a photo of them hooked up, no need to connect the yellow xt90.

Your wiring should look like this. 
![image|690x323](upload://rHtLUgvw1a3UelLMToNTOCuuypk.png)
```

---
## \#13 Posted by: lrdesigns Posted at: 2018-10-23T02:05:08.649Z Reads: 15

```
Hey @jojamcha did you get anywhere investigating your issue?
```

---

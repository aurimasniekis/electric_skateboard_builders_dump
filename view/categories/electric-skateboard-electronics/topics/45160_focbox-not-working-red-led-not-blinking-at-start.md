# FOCBOX not working - Red led not blinking at start

### Replies: 18 Views: 1098

## \#1 Posted by: Nicoalix Posted at: 2018-01-31T15:20:04.020Z Reads: 167

```
I tell you what happened just before the breakdown of the VESC and then I give you more data.

Goin up an slope, the engine pulley has been released, I have back home very slow to avoid mechanical problems, and halfway, master vesc has stopped working, the one that move the motor that failed.

Reset, and the red light did **not blink 3 times** when starting.
Blue and green lights stay on.
Receive signal from the remote control

No message in the fault code.

I have changed the vesc and motor, and this moves correctly.
I have tried to reinstall firmware.
The master vesc does not detect the motor, the slave vesc does.
The master vesc does not move any motor.
![IMG_20180131_153241|690x388](upload://xzFOFpWHI0v3gKKSCTORoyYYFyd.jpg)

Left one is master (failed)
![IMG_20180131_151303|690x388](upload://ps7dqHk7kSAUkeKSSJvb5i3DLi9.jpg)

Some help?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-01-31T15:24:11.880Z Reads: 155

```
Mostl likely the DRV or one of the mosfet is blown.
```

---
## \#3 Posted by: Nicoalix Posted at: 2018-01-31T15:27:05.635Z Reads: 153

```
Should not send an error in that case?
```

---
## \#4 Posted by: krloz Posted at: 2018-01-31T15:36:13.930Z Reads: 146

```
Drv usually issues fault code (is it at all possible it wouldn't if damaged?)
Do fets even issue fault codes? 
I'm not helping much here but am also curious
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2018-01-31T15:37:20.699Z Reads: 141

```
No necessarily, It always depend on how the DRV as blown.

If you want to double check you can make sure those resistor are at 39kohms

![image|284x500](upload://8rW5nkFzqGI1OL6r58IdCJpLT90.jpeg)
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2018-01-31T15:37:53.070Z Reads: 133

```
[quote="krloz, post:4, topic:45160"]
Drv usually issues fault code (is it at all possible it wouldn’t if damaged?)
[/quote]

As I said it is a false beleive
```

---
## \#7 Posted by: krloz Posted at: 2018-01-31T15:39:32.145Z Reads: 131

```
Look at me. Believing in false Gods.
Can they be measured mounted or do they have to be removed?
```

---
## \#8 Posted by: Ixf Posted at: 2018-01-31T15:39:56.813Z Reads: 132

```
I had the same problem.  No fault.  Visual inspection turned up a bubble on Vesc.  Sent it into DRVWizard who confirmed it was DRV failure and did chip replacement.  Bought it back flashed it with Ackmanic's fw and been happy ever since.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-01-31T15:55:04.254Z Reads: 132

```
Yes they can be mesure mounted
```

---
## \#10 Posted by: Nicoalix Posted at: 2018-01-31T16:31:03.713Z Reads: 122

```
These are the measures

R30: 39.0
R36 39.0
R46(16?); 9.8
R 29: 5.0
R 35: 5.0
R 43: 5.0
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2018-01-31T16:49:45.397Z Reads: 126

```
![image|666x500](upload://5T6UabLiFHX6mM0OB4QIM6XrSEJ.jpg)

As you can see from the picture above R46 is suppose to be 39Kohms, so the low impedance could be cause by the mosfet, the DRV or the resistor. But I can tell from experience, It is alway the DRV. 

Funny thing I’ve just made a video about that problem yesterday, I should upload it this weekend
```

---
## \#12 Posted by: Nicoalix Posted at: 2018-01-31T16:55:39.720Z Reads: 117

```
Thank you @JohnnyMeduse 
What are the options in Europe to repair this problem?
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-01-31T17:03:20.787Z Reads: 114

```
I think @fottaz does repairs?
```

---
## \#15 Posted by: longhairedboy Posted at: 2018-01-31T17:25:37.403Z Reads: 108

```
[quote="krloz, post:7, topic:45160, full:true"]
Look at me. Believing in false Gods.

Can they be measured mounted or do they have to be removed?
[/quote]

The Goa'uld mount false gods all the time. Usually during the conquest and enslavement of a human or unas  planet that they may or may not decide to completely destroy. But typically they remove them as they never measure up to themselves. Goa'uld literally means god in thier language so they think very highly of themselves.
```

---
## \#17 Posted by: krloz Posted at: 2018-01-31T19:20:45.823Z Reads: 91

```
Dude. Stop it or we are going to get this topic off any topic again.  A couple of comments and we are talking about peeing on a weightless planet
```

---
## \#18 Posted by: longhairedboy Posted at: 2018-01-31T19:29:57.806Z Reads: 89

```
[quote="krloz, post:17, topic:45160"]
A couple of comments and we are talking about peeing on a weightless planet
[/quote]

not even half a comment! look what you've done!
```

---
## \#19 Posted by: krloz Posted at: 2018-01-31T19:32:24.925Z Reads: 90

```
Ooii don't pull this on me... you started talking about goulds.    Naa forget it.   I had it coming...



Soo.....peeing on weightless planets... any opinions?
```

---
## \#20 Posted by: fottaz Posted at: 2018-02-01T09:22:50.674Z Reads: 76

```
yeah I can repair Drv, thank you for the tag Johnny!
```

---

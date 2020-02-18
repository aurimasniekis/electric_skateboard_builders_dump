# **VESC** &#124; Help &#124; Remote off = Motor on break \[SOLVED\]

### Replies: 10 Views: 512

## \#1 Posted by: SpartanFrench Posted at: 2018-04-29T12:16:46.972Z Reads: 81

```
Hi guys,

Does someone experience something like that before with his VESC : 

Remote **on** = Vesc send +/- 0,1A to motor = **Motor spin freely**
Remote **off** = Vesc send +/- 0,8A to motor = **Motor on break**

https://media.giphy.com/media/xUPGczofzl3QEh4glW/giphy.gif

I double check my vesc setting and here are my screenshots : 
It immediatly check my _timeout_ and _timeout break_ setting, nothing unusual here.

Remote OFF
![Apps setting|690x388](upload://xn5EPdPdJWnrHeeaoDL0Ar7oav9.PNG)
![PPM curve|690x388](upload://3i69aW6G31cXGF7D7HOTG2ZOwIl.PNG)
![PPM general|690x388](upload://qgxTyF9Ozuef7fCIVNwK24LnmYq.PNG)
![PPM Mapping|690x388](upload://r4XTsNWL2f6WSMkadWO5dv64Qcl.PNG)

Remote ON : (check real time date at the bottom)
![PPM general - Remote ON|690x388](upload://hPgSgrZuuW6QIpenHwGOGOqujjw.PNG)

Any idea ? :sweat_smile:
```

---
## \#2 Posted by: Acido Posted at: 2018-04-29T14:22:46.119Z Reads: 67

```
motor draws power when its connected, even if it does not spin

also make sure you set the ppm settings right(do the detection)
```

---
## \#3 Posted by: SpartanFrench Posted at: 2018-04-29T14:55:08.880Z Reads: 65

```
But why does the motor draw more power when the remote is **off**?
```

---
## \#4 Posted by: Acido Posted at: 2018-04-29T15:18:15.417Z Reads: 63

```
im not sure, check how many amps does it draw when its idling, also there could be a very small chance of the phase wires shorting
but if its spins nicely by hand when the remote is on there is nothing to worry about
```

---
## \#5 Posted by: RedEagle Posted at: 2018-04-29T15:31:04.428Z Reads: 59

```
Tweak your pulselength and deadband. That should rectify the problem.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2018-04-29T15:44:53.347Z Reads: 56

```
@SpartanFrench which remote do you have?
```

---
## \#7 Posted by: Guacamoleface Posted at: 2018-04-29T15:53:35.607Z Reads: 52

```
if its full brake then its most likely your falesafe on remote thats incorrectly set. Depends what remote tho.
```

---
## \#8 Posted by: SpartanFrench Posted at: 2018-04-29T18:00:31.815Z Reads: 48

```
I use the nano remote from aliexpress 

![20180429_134225|281x500](upload://zE9qZRhWWNpo1X8PwqZDFNQjfX4.jpg)
```

---
## \#9 Posted by: SpartanFrench Posted at: 2018-04-29T18:04:10.684Z Reads: 43

```
:white_check_mark: SOLVED :white_check_mark:

I tweaked the little screw in the middle of the blue blox (see photo above) and ....
... Run the detection again from VESC tool.

:fireworks: MAGIC ! :fireworks:
Problem solved.

Thank @Guacamoleface for the hint.
```

---
## \#10 Posted by: Guacamoleface Posted at: 2018-04-29T18:06:06.753Z Reads: 40

```
Glad you didnt discover it while bombing down full speed :) 

I discovered it the hard way. :joy:
```

---

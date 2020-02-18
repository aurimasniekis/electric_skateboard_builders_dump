# Noob Needing Help Connecting BLDC to New VESC

### Replies: 12 Views: 1977

## \#1 Posted by: sakated Posted at: 2017-04-14T04:48:26.774Z Reads: 151

```
I am officially new to this eSkateboard thing. Having issues connecting VESC to both Mac and Windows XP machines (it's old).

Bought the Buffalo Dual Motor on Kickstarter and actually received it - believe it was manufactured by I-wonder.cn if anyone cares. Used it for less than 8 hours and went through one battery (replaced by Buffalo) and burned up the ESC while braking. 

So rather than get another crappy ESC, I bought 2 VESCs (Vedder) and a bunch of supporting cables from . Including the programming USB cable.

I installed BLDC tool on Mac & Windows (XP) and can't get the BLDC to see the VESC. I have connected the VESC to power and getting solid blue and green lights, and red blinking light (2 flashes)

I have searched this board and the web and have tried all sort of things but VESC is not appearing as an option to connect with

Any ideas are appreciated.
```

---
## \#2 Posted by: IsTalo Posted at: 2017-04-14T12:02:39.594Z Reads: 137

```
You've clicked in connect in the BLDC tool? Choose the right port? It should work fine, but I don't know what is going on, can you put some pics?
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-04-14T16:12:47.931Z Reads: 129

```
Try updating drivers as described here: https://www.electric-skateboard.builders/t/vesc-problems-connecting/20471
```

---
## \#4 Posted by: sakated Posted at: 2017-04-15T00:00:14.053Z Reads: 120

```
See the attached on the drop down. It is the same pick list for both Mac and Windows XP. And I have added a pic of my USB Hardware showing from my system report.  Assume it has to be driver issue but I am running OS X Sierra and can't find one for it. 

<img src="/uploads/db1493/original/3X/7/4/74b65f6e04a598d660b40c1d9776d15d46e15e25.png" width="690" height="393">  

<img src="/uploads/db1493/original/3X/b/8/b8a29b82af5d967af60921abbe0841963c1a0e7f.png" width="612" height="500">
```

---
## \#5 Posted by: sakated Posted at: 2017-04-15T00:21:44.286Z Reads: 84

```
I have already tried the drivers.  Interestingly, when I add the card to Windows XP, it is showing up as a Universal Serial Bus, and a Virtual Com port.  Most likely the issue.  I found a virtual COM Port Driver from ST Micros site, but it doesn't work.  Was found here - http://www.st.com/en/development-tools/stsw-stm32102.html

Possible my Windows computers are just too old.
```

---
## \#6 Posted by: sakated Posted at: 2017-04-19T07:23:52.032Z Reads: 79

```
I figured it out and was a total Noob error.  After many hours of trying with multiple laptops and driver installs, it was as simple as me using the programming cable (STM32) to connect to the VESC vs. using the Micro-USB cable.  I thought the programming cable was required to configure.  BLDC-Tool working on Mac OS Sierra and have already started to configure my motors.  Thanks for your help.
```

---
## \#7 Posted by: Nico Posted at: 2017-04-19T08:22:05.652Z Reads: 77

```
Hello,

I don't understand why you have to connect your VESC to your computer ? :s
```

---
## \#8 Posted by: sakated Posted at: 2017-04-19T15:04:14.250Z Reads: 68

```
This was for the BLDC-tool so I can configure the VESC for my specific motors and preferences.  It has to be done in order to operate the board.
```

---
## \#9 Posted by: Nico Posted at: 2017-04-28T08:05:42.061Z Reads: 66

```
Does I have to do it too ?
```

---
## \#10 Posted by: sakated Posted at: 2017-04-28T15:26:53.566Z Reads: 65

```
Being new to this I am not sure you have to do this in all cases.  But my assumption is that every motor is different and the VESC needs to be configured to support each one. There are a lot of videos out there to help that I have found on this forum, and also on the internet. A couple below:

Basic Configuration -  https://www.youtube.com/watch?v=dxDXUrk-7ek

Setting up FOC - https://www.youtube.com/watch?v=dxDXUrk-7ek

And I did get the software/configuration working for my motor using the instructions.  Quite easy once the computer connected to the VESC.
```

---
## \#11 Posted by: Nico Posted at: 2017-05-02T07:27:48.151Z Reads: 56

```
thank you !
```

---
## \#12 Posted by: epruski Posted at: 2019-08-14T00:57:39.807Z Reads: 9

```
I am having the same issue on my macbook where it isnt connecting. You said it is a programming cable issue? I have the flipsky dual vesc6.6 and it came with a little usb cable. Am I missing something?
```

---

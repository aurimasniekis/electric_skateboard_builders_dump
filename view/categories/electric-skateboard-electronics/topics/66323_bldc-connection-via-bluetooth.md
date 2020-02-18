# BLDC connection via Bluetooth

### Replies: 13 Views: 317

## \#1 Posted by: Marksmoura Posted at: 2018-08-28T05:01:20.702Z Reads: 99

```
Hello everyone,

For around 2 hours I have been trying to find if it is possible to configure the Vesc 4.12 via Bluetooth instead USB and I can't seem to find anything concrete.

I plan on buying the HM-10 but I need someone to answer my doubts.
Is it really possible to do it or will I only be able to read data like speed etc. I am running dual 4.12.

I really just want the Bluetooth module for the wireless connection with the BLDC tool so I can adjust parameters and so on. I have Windows and Ubuntu.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-08-28T05:06:33.638Z Reads: 96

```
Yes you can. You might want the metr module as they are the most versatile
```

---
## \#3 Posted by: Marksmoura Posted at: 2018-08-28T19:13:16.881Z Reads: 79

```
So I found the website where they build the original HM-10 but they have 4 versions of this module.
Which one would be the most suitable to connect with BLDC tool ? 

![image|487x500](upload://adO3gZJfm7eshMdgooFyjjPCuEx.jpg)
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-08-28T20:25:42.182Z Reads: 72

```
Not sure what the difference is between them.
```

---
## \#5 Posted by: Marksmoura Posted at: 2018-08-29T01:06:51.403Z Reads: 68

```
I bought the first on the left, both on top have more pins on the bottom, maybe need to use them and the different left and right is that right has one cristal inside the chip. I really don't know if that makes a difference but I opted to buy the first.
```

---
## \#6 Posted by: Nordle Posted at: 2018-08-29T06:24:53.336Z Reads: 62

```
in a dual configuration, does this require 1 module per esc, or is a canbus connection enough?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-08-29T08:00:41.475Z Reads: 58

```
Can is enough
```

---
## \#8 Posted by: Nordle Posted at: 2018-08-29T08:59:39.016Z Reads: 50

```
nice, can someone explain how to set this up?:)
```

---
## \#9 Posted by: Andy87 Posted at: 2018-08-29T09:09:55.233Z Reads: 50

```
what you want to know exactly?
Just connect your VESCs with CAN cable.
Config that one with bluethooth as master and the second one 
as slave.
never ever disconnect the CAN cable when powered on both vesc.
```

---
## \#10 Posted by: Nordle Posted at: 2018-08-29T09:23:18.499Z Reads: 46

```
how connect to bldc tool, my pc has bt, but my vesc doesn’t show up if not connected via usb?
everything is connected like you said above, can is hardwired:p
```

---
## \#11 Posted by: Andy87 Posted at: 2018-08-29T09:39:14.203Z Reads: 45

```
I only connected my Bluetooth to my phone, so I can´t tell you much about how to connect to PC.
Usually you can choose which com port you use for connecting with your vesc. Guess there should pop up your Bluetooth device also as option. If no, than make sure that your Bluetooth modul also working with the laptop you use.
there are different modules, not all support every operating system.
```

---
## \#12 Posted by: Marksmoura Posted at: 2018-08-29T20:09:23.867Z Reads: 33

```
I have heard maybe you need Linux but I am not sure, just read somewhere I don't remember anymore.
```

---
## \#13 Posted by: Nordle Posted at: 2018-08-29T20:21:03.014Z Reads: 30

```
i just realize my pc's bluetooth is broken.. if it's really that simple and it should just show up under com ports would be nice, if there is something else to do and some one knows let me know, will get new bt for my pc soon to try this:) linux is an option however would prefer in windows
```

---

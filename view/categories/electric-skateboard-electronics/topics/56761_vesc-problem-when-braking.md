# VESC Problem when braking

### Replies: 13 Views: 468

## \#1 Posted by: iscle Posted at: 2018-05-25T19:21:44.755Z Reads: 93

```
Hi there, 
today I tried my first VESC build, and I´m starting to get the hang of it except a problem I have when braking. 
I´ve tried everything to solve it, but nothing has worked. The VESC is a MAYTECH VESC v4.12, which has the capacitor mod done to it (the one from the DRV, C18 if i'm not mistaken), but it still throws an error when braking. The error is the following:

    The following faults were registered since start:

    Fault            : FAULT_CODE_DRV
    Current          : 0.8
    Current filtered : -32.3
    Voltage          : 39.36
    Duty             : 0.000
    RPM              : 5603.9
    Tacho            : 151545
    Cycles running   : 6018
    TIM duty         : 0
    TIM val samp     : 2
    TIM current samp : 4200
    TIM top          : 8400
    Comm step        : 0
    Temperature      : 36.05
     
    Fault            : FAULT_CODE_DRV
    Current          : -12.4
    Current filtered : -25.2
    Voltage          : 39.34
    Duty             : 0.000
    RPM              : 4953.0
    Tacho            : 152086
    Cycles running   : 2857

To be more precise, what happens is that it cuts out and then starts braking again, and it usually only happens when braking close to 100%...

If needed I can post all my VESC parameters, I'm also using HUB motors and FOC mode in a 10s setup. I'm also using Current control.

Has anyone else faced this problem? And if so, how did you fix it? 

Thanks, 
Iscle.
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2018-05-25T20:03:01.764Z Reads: 70

```
What do you have for motor current min, battery min, and absolute max?
```

---
## \#3 Posted by: iscle Posted at: 2018-05-25T21:06:11.921Z Reads: 60

```
Hi! Thanks for the fast reply :slight_smile:

This are my motor settings (It's a dual motor setup, and they are the same in both VESC), I forgot to say that I'm also using HALL sensors, however I think that doesn't matter when braking.
![image|260x259](upload://qgOahIYZetz718bVnQSRWxEBK43.png)
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2018-05-29T14:12:26.333Z Reads: 40

```
Hmm that looks alright to me. What kind of battery do you have?
```

---
## \#5 Posted by: iscle Posted at: 2018-05-29T14:25:38.017Z Reads: 34

```
It's made by me, it's a 10s2p LG HE4 pack, cells are brand new from a good reseller, so not fake... I'm not using any BMS at the moment, they are direcly connected to the VESC with an XT60 antispark as a switch. It's a bit strange as both VESC throw the same error. 

v4.12 has the DRV capacitor mod already done to it right?
```

---
## \#6 Posted by: t0m_r1dd1e Posted at: 2018-05-29T14:38:18.519Z Reads: 32

```
I'm not sure if this is the root of the problem, but you should probably lower your battery max regen. Dumping 20 amps into a 2p is not going to be great for the life of the cells. Maybe try lowering it to -6 amps per vesc and see if you still get the error.
```

---
## \#7 Posted by: iscle Posted at: 2018-05-29T14:56:30.744Z Reads: 31

```
Oh, I thought this value was "shared" between the two VESCs in dual motor setup (because I have them connected via the CAN bus)... 

I will also lower the battery current max to 20A/VESC too then...

The battery datasheet says maximum 5A per cell, so i will lower the battery regen to 5A/VESC and see if it gets any better. I will report the results when I try it! 

Thanks
```

---
## \#8 Posted by: t0m_r1dd1e Posted at: 2018-05-29T15:11:06.714Z Reads: 27

```
As far as I know, the battery settings are per vesc. Yeah, that all sounds good. Let me know how it goes.
```

---
## \#9 Posted by: iscle Posted at: 2018-05-29T17:27:27.125Z Reads: 22

```
Okay, I just tried it. It still doesn't work...

This is the error I got now, basically the same with other values:
    The following faults were registered since start:

    Fault            : FAULT_CODE_DRV
    Current          : -7.4
    Current filtered : -22.3
    Voltage          : 39.07
    Duty             : 0.000
    RPM              : 4816.1
    Tacho            : 8762
    Cycles running   : 2910
    TIM duty         : 0
    TIM val samp     : 2
    TIM current samp : 4200
    TIM top          : 8400
    Comm step        : 0
    Temperature      : 24.81
     
    Fault            : FAULT_CODE_DRV
    Current          : -25.6
    Current filtered : -27.5
    Voltage          : 39.03
    Duty             : 0.000
    RPM              : 4964.1
    Tacho            : 9046
    Cycles running   : 108
    TIM duty         : 0
    TIM val samp     : 2
    TIM current samp : 4200
    TIM top          : 8400
    Comm step        : 0

I've uploaded the appconfig and motorconfig xml files with all the values to google drive, for me everything seems right, but maybe i'm in the wrong... 
Here they are: [https://drive.google.com/open?id=1aZ-AsSYcZOyK7XAYs6jY_uDA6wNoFdE3](https://drive.google.com/open?id=1aZ-AsSYcZOyK7XAYs6jY_uDA6wNoFdE3)

Thanks again!
```

---
## \#10 Posted by: t0m_r1dd1e Posted at: 2018-05-29T17:44:50.811Z Reads: 21

```
Ah, bummer. Well this is starting to get beyond the point where I'm able to be helpful. 

Has it always done this or did it work correctly ever? Are you using the stock firmware or Ackmaniac's mod?
```

---
## \#11 Posted by: iscle Posted at: 2018-05-29T17:53:52.145Z Reads: 21

```
Acceleration is very smooth, I haven't got any problems there, and braking has always been like this... This is my first VESC build so I don't have any more background.

I'm using the latest version of stock firmware, with the latest version of VESC Tool. 

I tried Ackmaniac's mod, and it didn't go well. I couldn't get past FOC setup, and if I tried the BLDC version, the motor would start cogging and making really loud noises, I almost thought the VESC was going to die... 

Could it be an issue that I'm using UART to control the VESC and writing Nunchuk values instead of, say, PPM? Maybe it's receiving wrong values and it doesn't like it? However I don't see why that would throw a DRV error...

Thanks for the help.
```

---
## \#12 Posted by: t0m_r1dd1e Posted at: 2018-05-29T18:13:45.954Z Reads: 19

```
I can't imagine it's an issue with the nunchuck. I have no experience with foc, so it could be something weird specific to that mode. 

If you're willing to try anything at this point, try ack's again. I was getting to cogging on motor detection too until someone told me to raise duty from 0.05 to 0.15 and then it worked perfectly for me.
```

---
## \#13 Posted by: iscle Posted at: 2018-05-29T18:19:04.997Z Reads: 18

```
That seems risky hahaha

I will try switching to BLDC and see how that works, in stock fimware (i've never tried it, I went with FOC directly), and if breaking works good there I might try to add another capacitor in parallel in C18 to see if that's the issue as it was a few years ago, and if not then I will cross fingers and try ack's firmware and pray it doesn't blow up the drv hahaha
```

---

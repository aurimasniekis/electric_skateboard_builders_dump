# Flipsky FSESC 4.12 VESC on 12S working? experiences?

### Replies: 13 Views: 1074

## \#1 Posted by: Marsl187 Posted at: 2019-01-04T18:34:55.291Z Reads: 190

```
Hey guys,

I have two Vesc 4.12 from Flipsky running in my build on 10S, works perfectly fine.
Now I want to upgrade to 12S but I heard some rumors that Vesc 4s in general do not work that good with 12S... so they are recommended to run on 10S....

Does anyone have experiences with running a Vesc 4.12 on 12S?
What are the problems which are cause while on 12S running?
Which ohne is recommended to run on 12S?

Thanks!
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-04T18:41:31.475Z Reads: 187

```
Just use the search function and you will find most answers to your questions.
The cheap versions of the 4.12hw design have problems if you run them with 12s and motors over 200kV.
If you ask @b264 he will tell you that it’s not good to run any esc based on the drv chip with 12s.
So far you will be probably good with a focbox/unity and the most hw6 based vescs.
```

---
## \#3 Posted by: b264 Posted at: 2019-01-04T21:25:42.672Z Reads: 173

```
The VESC 6 series also uses the DRV83xx chips.  The VESC7 does not
```

---
## \#4 Posted by: Wilsonliang777 Posted at: 2019-05-01T22:58:52.759Z Reads: 128

```
were you able to get FSesc 4.12 to work with 12s?
```

---
## \#5 Posted by: Andy87 Posted at: 2019-05-02T01:04:21.876Z Reads: 125

```
They will work with 12s in bldc shouldn’t be an issue. 12s FOC should work too but might also just work for a time.
```

---
## \#7 Posted by: Marsl187 Posted at: 2019-05-02T08:06:18.737Z Reads: 115

```
I stayed for 10s in that build. But I think if you limit the erpm to 58k something and don‘t exceed the current limits it should work properly. 
For my mountainboard I went for a Unity because the price difference is not that high anymore. With 4.12 you still need an additional switch and bluetooth module. When adding this stuff up the Unity is like 50€ more. But they raised the price lately..
```

---
## \#8 Posted by: Wilsonliang777 Posted at: 2019-05-02T09:39:38.324Z Reads: 109

```
My issue is currently i have 2 fsesc 4.12 and I am running my board on 3x3s lipo. I want to used 10s lipo but don't want to take the lipo apart to made 10s.    My plan is to buy another 3s lipo and combine the lipos to 12s lipo.   I have 
dual 200kv motor and will set erpm to 55k.
```

---
## \#9 Posted by: visnu777 Posted at: 2019-05-02T09:53:10.363Z Reads: 109

```
For the protocol: I use them occasionally with a 2s booster plus my normal 10s pack without issues.
```

---
## \#10 Posted by: Wilsonliang777 Posted at: 2019-05-10T15:21:59.705Z Reads: 91

```
last night I configured my board to 12s 7000mah lipo With  a fesc 4.12.  the vesc setting is 25 amp, -25amp motor , absolute battery max 120,   battery max 55amp and battery Regen max at -20 and erpm limit to 55000, on bldc mode.       My board is dual drive, 90mm wheels and with 40/15 gears, motor is 200kv. .   I might lower the gears to 40/12 because I don't need to go 29mph.  Let's see what happen when I ride it this weekend.
```

---
## \#11 Posted by: RobbieP Posted at: 2019-05-10T15:35:20.286Z Reads: 91

```
Ive been running 12s and 10s both, on my dual EMTB sk3 192kv motors, vesc 4.12s in FOC with no issues. Tall grass seems to draw the most from the motors but Ive never experienced any issues with cutting out or overcurrent.
```

---
## \#12 Posted by: Wilsonliang777 Posted at: 2019-05-10T15:53:11.837Z Reads: 88

```
What  is your  vesc setting?.  I will slowly increase to 40/-40 motor but will keep erpm limit to 55000.    O yea. I did add diy heat sink to the fsesc.
```

---
## \#13 Posted by: RobbieP Posted at: 2019-05-10T16:05:15.187Z Reads: 87

```
80/-60 motor and charge settings. E rpm limit was left at whatever is stock
```

---
## \#14 Posted by: ganso.silva Posted at: 2019-07-01T18:56:37.408Z Reads: 57

```
Can you help me?
Is this an esc or is it considered vesc? I'm in doubt
https://pt.aliexpress.com/item/32951134782.html?spm=a2g0s.9042311.0.0.17aeb90aAAmZcf
```

---

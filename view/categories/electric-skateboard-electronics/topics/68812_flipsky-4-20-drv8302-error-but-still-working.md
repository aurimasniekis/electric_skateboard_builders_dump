# Flipsky 4.20 DRV8302 error, but still working?

### Replies: 27 Views: 983

## \#1 Posted by: DAddYE Posted at: 2018-09-22T00:48:38.612Z Reads: 189

```
Hi all,

I'm running [Skullboard hubs](https://www.skullboardvip.com/products/dual-hub-motor), 11s3p 30q with a [flipsky dual esc](https://flipsky.net/collections/electronic-products/products/dual-fsesc4-12-100a).

Im running in **Sensored FOC** with these settings:

motor current max: **30**
motor current max brake: **-30**
battery current max: **30**
battery current max regen: **-6**

Sometimes especially uphill I get _DRV8302_ error, see for example: 
![08%20PM|434x500](upload://sikk9j6jtOnMLEek7fjitj9zWrb.png) 

But after that, it works without issues. What could it be? Any idea?

Thanks!
```

---
## \#2 Posted by: Winfly Posted at: 2018-09-22T01:09:08.215Z Reads: 182

```
It has hardware issue running 12s FOC during hard acceleration and braking,  but no problem at 10s FOC. I guess you have shown that it also doesn't work at 11S.
```

---
## \#3 Posted by: DAddYE Posted at: 2018-09-22T02:08:07.057Z Reads: 174

```
Yeah, I read about it and I was hoping was only on 12s. Is there any workaround?
```

---
## \#4 Posted by: threebysix Posted at: 2018-09-22T02:42:07.378Z Reads: 167

```
I think one work around that I remember reading was to not throttle/brake too hard/quick/sudden.
```

---
## \#5 Posted by: Eboosted Posted at: 2018-09-22T06:23:04.475Z Reads: 155

```
Too bad it does not work on 12s, seems to be a subpar product even though I had high hopes for them
```

---
## \#6 Posted by: dareno Posted at: 2018-09-22T06:59:24.597Z Reads: 150

```
Same.  Shame.
10c
```

---
## \#7 Posted by: hoeksame1 Posted at: 2018-09-22T07:03:18.014Z Reads: 149

```
Mm how is the accelerstiob with those hubs with flipsky esc?? I am thinking to make the same setup.
Only 10s. 
How is the torque,top speed, battery consumption???


Gr sam
```

---
## \#8 Posted by: sayekim Posted at: 2018-09-22T12:20:28.821Z Reads: 135

```
Go 10s or try bigger capacitors. Bigger caps have not been proven yet but it would not surprise me that that would solve it. 
The current caps look tiny.
```

---
## \#9 Posted by: Benjamin899 Posted at: 2018-09-22T17:29:36.567Z Reads: 124

```
i am guessing the smaller size of the vesc took its toll on overall performance. But you can also read people having faults with other vesc at 12s foc. I would rather play with gearing/hubs than change my battery to a higher S.
```

---
## \#10 Posted by: brenternet Posted at: 2018-09-22T18:51:50.861Z Reads: 129

```
I didn't really ever expect this esc to run 12s foc. I can't be the only one. You wouldn't really expect a HK sk8 to run it, hell people even dispute focboxes should do it even though it's been proven a thousand times that they can.

It's a cheap component esc made for 10s.
```

---
## \#11 Posted by: mtuan293 Posted at: 2018-09-23T03:53:21.138Z Reads: 113

```
I noticed this...both their dual 4.20 and single 6.6 use the same 220μF 100V caps. People have been saying good things about the 6.6, while the 4.20 has cutout issues. Why is this? @Kug3lis any explanations? 

single 6.6 on their website
![image|686x500](upload://pjFRH2qPApQQNGQC62ijANlbcIM.jpeg) 

dual 4.20
![image|686x500](upload://hPRy0POFLToReZoSIlavHWCitzt.jpeg)
```

---
## \#12 Posted by: sayekim Posted at: 2018-09-23T09:10:38.940Z Reads: 104

```
Good find. It might be a mistake on their site. @moon Can you confirm that the 6 has these caps?
```

---
## \#13 Posted by: Riako Posted at: 2018-09-23T11:11:39.780Z Reads: 97

```
They're same on my dual or FSESC4.20 and FSESC6.6
I heard that caps. will be changed on next 4.20 ...
Kugelis or Pimousse already advise me to change them on my 4.20s...
For same as 4.12 maybe ? (on the right of the pic)
https://cdn.shopify.com/s/files/1/0011/4039/1996/files/V4_2_2048x2048.jpg?v=1530689341

Also seeing many people trying they're 4.20 under FOCk without issue... Maybe I will give it a try too
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-09-23T12:50:54.553Z Reads: 92

```
Not only those big capacitors, small ceramics and etc :) Until @BarbaraZ release schematics which she must I can't tell nothing much :)
```

---
## \#15 Posted by: DAddYE Posted at: 2018-09-23T19:01:49.354Z Reads: 84

```
Is it going to work without issues on BLDC?
```

---
## \#16 Posted by: Riako Posted at: 2018-09-23T20:55:09.349Z Reads: 82

```
Your too lucky :sweat: ... can say the same for me ...
```

---
## \#17 Posted by: DAddYE Posted at: 2018-09-23T22:06:42.148Z Reads: 78

```
Sorry it was a question :)
```

---
## \#18 Posted by: Riako Posted at: 2018-09-23T22:49:26.815Z Reads: 75

```
:blush: got over current and over intensity on 10s bldc ... I ride during fiew days all good under 20A motor and batt max, then I got faults during downhill braking...
I will make more test with higher batt max see if it change the game ...
some test here
https://youtu.be/1OouVAyi_4I

**Edit** 
1st ride : 40A motor max and min / 30A batt max -15 batt min
2nd : 30A // 25A batt max
3th and good but not that powerful : 20A batt and motor max

I made more change 5Amps by 5A itch time, I change setting with Metr.Pro, I just let you know on the main lines
```

---
## \#19 Posted by: pat.speed Posted at: 2018-09-23T22:49:28.270Z Reads: 74

```
Have you tried setting it below 30a I remember some people have cut outs with maytech vescs when they were set higher than 30a. I can’t remember if that was batt or motor though
```

---
## \#20 Posted by: brenternet Posted at: 2018-09-23T22:53:38.137Z Reads: 73

```
Check out @mmaner Mike's settings he's having success with here:

https://www.electric-skateboard.builders/t/poll-flipsky-information-in-one-place/68940/10
```

---
## \#21 Posted by: Riako Posted at: 2018-09-23T22:54:52.463Z Reads: 71

```
Yes, I will try that tomorrow if it's no more raining here :blush:
```

---
## \#22 Posted by: DAddYE Posted at: 2018-09-23T23:30:49.974Z Reads: 69

```
He’s on 10S. I’m on 11s :( So far I just got 1 fault on foc
```

---
## \#23 Posted by: DAddYE Posted at: 2018-09-25T01:08:03.888Z Reads: 61

```
Today I rode my same usual commute path and with 25a I got no issues so far ;)
```

---
## \#24 Posted by: DAddYE Posted at: 2018-09-25T02:25:29.122Z Reads: 56

```
Worth mentioning, I’m using stock firmware.
```

---
## \#25 Posted by: Riako Posted at: 2018-09-25T02:40:57.993Z Reads: 54

```
Yeah ! glad you could ride it ! :blush: 

I could ride it without issues too, but when you don't cruise and ask a bit more, be careful! The faults could happen maybe (like it does to me, mostly uphill and downhill when you play full trigger at low speed...).

_(I'm maybe a bit misunderstood, cause because English is not that easy for me.)_
```

---
## \#26 Posted by: DAddYE Posted at: 2018-09-25T02:49:46.160Z Reads: 54

```
Are you running stock firmware or ackmaniac?
```

---
## \#27 Posted by: Riako Posted at: 2018-09-25T02:51:48.816Z Reads: 54

```
Stock too, I will try to reupdate it, try to make work sensor again, higher batt max than motor and foc ...
```

---

# First Build Help

### Replies: 19 Views: 2041

## \#1 Posted by: Vermontstig Posted at: 2016-08-06T08:28:15.103Z Reads: 108

```
Hey guys this will be my first build so I'll give you the list and I'll ask my question in the end. 
2x6s 8000 mah in series
VESC enterion 
Motor TB 6374 230kv
Drive Train is the mono build kit via Enertion 
The last thing is the HV 120a on/off switch.

Now to the build question, the batteries have the xt60 connector which is nice but the on/off switch doesn't only a positive and negative cords that was made for the DIY ESC I think. So should I just cut the cord and put a xt60 and solder it on both ends so it would also fit the VESC? or is there a better way? Other than that anyone know of a good solder to get for this job and good shrink rap.
```

---
## \#2 Posted by: jrpwit Posted at: 2016-08-06T08:50:38.020Z Reads: 103

```
Yup just put the connector on the switch. Any solder is good really just dont buy a ton of it or you will end up like me with tons of soldering wire. 

12s and a 230kv will not work with the vesc tho. The erpm with be higher than 60k ((12*3.7)*230*7=71,484) and this is not even with fully charged 4.2 v cells. I think 9s might be fine but still you may exceed 60k ((9*4.2)*230*7=60,858) and this is will fully charged cells. Exceeding 60k erpm will cause you drv chip to fry disabling your vesc so dont do it! If you wanna go 12s get a 190kv motor.
```

---
## \#3 Posted by: Vermontstig Posted at: 2016-08-06T08:59:32.884Z Reads: 97

```
So the vesc-platinum won't work, I'm lost on the hole erpm. I didn't see that anywhere when I bought the VESC so should I contact enertion and tell them to just refund me than I guess? What esc would work with this setup?
```

---
## \#4 Posted by: lowGuido Posted at: 2016-08-06T09:01:26.932Z Reads: 88

```
230kv with 12S is too much. use a lower kv motor or a smaller battery.
[quote="jrpwit, post:2, topic:7209"]
Also on a single drive setup, the board can get unstable at high speeds compared to a duel drive setup.
[/quote]

I dunno where that came from but its untrue. single drive are fine at high speeds.

as far as your switch is concerned you gonna need to show me some diagrams so that I know what you have got.
a traditional switch only needs to be on one lead (+ve or -ve doesn't really matter which one)
I personally would cut the XT60 off and solder your switch on, maybe keep the xt60 for the battery.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-08-06T09:03:20.463Z Reads: 79

```
its not that it wont work its just that your RPM values are way too high.. you would be crackin 60+km/h
just wack your two 6S in parallel instead of series and you will be fine. and have a board that rides for like 40km.
```

---
## \#6 Posted by: jrpwit Posted at: 2016-08-06T09:05:37.663Z Reads: 77

```
Chaka explains the erpm thing here.
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

If you havent purchased the motor yet I would just get a different one. I think DIY's esc should work fine. The vesc is great but high erpm is an issue. Apparently the newer version of the vesc witch is coming is suppose to fix the erpm issue.

@lowGuido Ill edit my post. I said that just cause people talk about how single drive is "uneven"
```

---
## \#7 Posted by: lowGuido Posted at: 2016-08-06T09:09:25.079Z Reads: 70

```
yeah... people talk a lot on this forum..
its hard to differentiate fact from fiction.
I have ridden every drive, I can tell you none feel uneven at speed.
```

---
## \#8 Posted by: Vermontstig Posted at: 2016-08-06T09:13:55.483Z Reads: 66

```
Well damn I bought the motor from DIY already Dexter is super cool so ill ask him if I can get another one. What motor should I get if I want to do the 12s set up I need powa I'm 6'8 305 so I need to get something that can move me. I know duel would be best but money is tight that college life.
```

---
## \#9 Posted by: Vermontstig Posted at: 2016-08-06T09:17:07.604Z Reads: 66

```
So I won't blow up my vesc-platinum it just will be very fast than right? So in theory this is a workable motor and vesc?
```

---
## \#10 Posted by: jrpwit Posted at: 2016-08-06T09:17:53.227Z Reads: 65

```
I think I remember Jason saying something about it being uneven in one of his vids. But thanks for clearing that up for me! :slight_smile:
```

---
## \#11 Posted by: jrpwit Posted at: 2016-08-06T09:37:02.740Z Reads: 62

```
Nothing wrong with single drive. Also lower kv equals more torque but at the cost of speed. You will not blow your vesc if you go 6s with the 2 batteries in parallel. Dexter was pretty cool about me returning a motor mount for a newer version so he won't mind you returning your motor. Anything 190 kv and below should be fine with the vesc on 12s though. The enertion momo motor is a monster. Yes 12s with the vesc will work but is risky. You could blow it when bench testing your board or anytime there isnt any load on the board. I think the drv chip frying is the most commonly broken part amoung vesc owners. Just type drv error in the search and you will find tons of people reporting damaged drv chips and trying to repair the vesc themselves (which actually isnt that hard if you have proper surface mount soldering equipment).

Also if you are in a dorm, I wouldn't recommend lipos. They are a fire hazard if not cared for properly.
```

---
## \#12 Posted by: willpark16 Posted at: 2016-08-06T09:56:41.820Z Reads: 60

```
or just switch ur esc
```

---
## \#13 Posted by: Vermontstig Posted at: 2016-08-06T22:13:12.526Z Reads: 48

```
Ok I just getting a confirmation from enertion that I might fry my VESC. I think the smartest move is just to get a lower 190kv motor. I don't live in the dorms thank god got into way to much trouble when I lived on campus. Thanks for all your help guys.
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2016-08-06T22:30:24.477Z Reads: 47

```
My tb6355 that's rated at 230kv is actually 190kv. The 6374 might be as well. Still wouldn't use it on 12s but 10s yes. You can check erpm on bldc tool.
```

---
## \#15 Posted by: lowGuido Posted at: 2016-08-07T00:04:42.938Z Reads: 46

```
you will be pushing the limits of the VESC's capability with that motor. as I said.. either lower kv motor or lower voltage. battery.
```

---
## \#16 Posted by: Ulfberht Posted at: 2016-08-07T02:49:41.011Z Reads: 39

```
Dexter sells a 170kv 6355 for you to consider as well@12S. :thumbsup:
diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-170kv/
```

---
## \#17 Posted by: Workaround Posted at: 2016-08-07T03:10:53.701Z Reads: 42

```
VESC are designed for max 10s. I better idea is to ether hook in parallel or swap batteries and just use 6s(depends on how you setup your batteries on the board if it is easy to take them off). I would try that if it does not want to push you you need a different motor or gear ratio(which ever is cheaper).
```

---
## \#19 Posted by: Vermontstig Posted at: 2016-08-07T11:26:14.801Z Reads: 41

```
The VESC Platinum is rated for 3-12S that's what the website says. That's the one I have on order.
```

---
## \#20 Posted by: Workaround Posted at: 2016-08-07T13:14:08.059Z Reads: 35

```
From what I have been talking to other people on here 12s is going to put more strain on the VESC. It is rated for that max usually you don't want to run it at max. Some of the information I have found it that there is 15% less efficiency in the system running at 12s vs 10s. This could just be because wind drag, vesc limiting out(because the VESC design is only for 10s he changed a few things to allow 12s but unless you rebuild the VESC complete desicn efficiency will still be much worse at that voltage).
```

---

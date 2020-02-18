# Possibilities of rewinding motor for better efficiency

### Replies: 20 Views: 975

## \#1 Posted by: jbruce Posted at: 2017-10-28T05:28:02.970Z Reads: 164

```
While riding the other day, my sk3 213kv 6364 motor began making a scraping high pitch noise. I stopped riding and took it apart when I got home, finding one of the magnets had broken and the fragments were scraping while the motor spun. I cleaned out the fragments and put it back together and it works relitivly the same as before (hopefully I can get a replacement from hobbyking). 

While messing with opening my motor and and looking inside I became curious if rewinding the motor would provide better efficiency as the factory job doesn't seem great. With this motor ive been getting a shameful 15-20wh/mi efficiency on a single drive board and I weigh 130. With an older tourque boards motor my efficiency was always under 12wh/mi so it made me think what could be so much less efficient about this motor. If anyone has any thoughts on if rewinding it would help, let me know. I myself haven't ever rewinded a motor but would be very interested to learn and see the effects of it would be.  

<img src="/uploads/db1493/original/3X/3/1/31ca488187f1d845fe09f74fdbe4e2c3dd223b95.jpg" width="281" height="499"><img src="/uploads/db1493/original/3X/d/d/dd302563ec16f70a3051a535ea28010e8f7b17c4.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/1/311a051c8fdd02e818622461337ab0091ccf7903.JPG" width="666" height="500">
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-10-28T05:43:10.017Z Reads: 149

```
It certainly can't hurt. It may also be worth it to replace the magnets with more powerful ones, which will slightly lower the kv and increase the efficiency. 

I've never rewound a motor that large, but I've done a few smaller ones suitable for RC planes. The concept is pretty straightforward and there are quite a few tutorial/documentation videos out there.
```

---
## \#3 Posted by: jbruce Posted at: 2017-10-28T08:19:10.486Z Reads: 133

```
How does replacing the magnets decrease the Kv? Also would I be able to just compensate for that in the numbers of turns I use when rewinding?
```

---
## \#4 Posted by: jmasta Posted at: 2017-10-28T08:27:42.861Z Reads: 131

```
[quote="MysticalDork, post:2, topic:36699"]
It certainly can't hurt.
[/quote]

Sure it could. I don't see how winding it yourself is guaranteed as good or better than a professionally wound motor  

But then again, I've never rewound a motor. And I never intend to. Ain't nobody got time for that!!  :joy:
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-10-28T17:35:37.594Z Reads: 102

```
The stronger the magnetic field, the slower the kv. So if you replace the magnets with stronger ones, the kv will go down. Also if you add more turns of wire, that makes a stronger magnetic field, and the kv goes down. What I'd do is replace the magnets and see what that did to the kv, and then figure out what to do in the rewind to compensate for it. 

@jmasta it's a cheap chinese wound motor, not a high quality one. As long as you're careful and take your time, it's not hard at all to do better. It's not guaranteed, just like everything else in the DIY world.
```

---
## \#6 Posted by: chuttney1 Posted at: 2017-10-30T05:47:28.530Z Reads: 90

```
Check the RC forums for more information. People have rewound their motors and some using a larger gauge wire than what was used.
```

---
## \#7 Posted by: jbruce Posted at: 2017-10-30T05:54:55.395Z Reads: 89

```
What do you guys think about delta vs wye winding concerning optimal efficiency. I know it's a different for of terminating the turn but is one known to work better with the vesc or more efficiently overall?
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-10-30T06:16:28.959Z Reads: 91

```
As far as I know, the efficiency is the same between delta and wye. Assuming the windings are the same, delts will give you more power and wye will give you a lower kv. I've also heard that wye will give you less back-emf, so it can be more difficult for sensorless controllers to get a good signal off them.
```

---
## \#9 Posted by: pat.speed Posted at: 2017-10-30T11:07:23.439Z Reads: 88

```
I would say one reason for the torqueboards motor getting better Wh/mi is because of the quality of parts. The windings of the motor are also probably much better.

As for wye or delta, I've heard that wye is more effecient and will give 1.7 times more torque than delta but delta will give 1.7 times more speed
```

---
## \#10 Posted by: jbruce Posted at: 2017-10-30T17:03:08.420Z Reads: 85

```
So most likely I could increase efficiency significantly by rewinding it. I'll prob try that as soon as I get some free time from school.
```

---
## \#11 Posted by: Hummie Posted at: 2017-10-30T17:29:15.653Z Reads: 73

```
With the missing magnet part u have a problem there. Removing the magnets can be practically impossible if they use some adhesives. I've never been able to remove magnets.  
Does the motor get hot? Your wasted energy has to go somewhere 

U likely would get a much better motor if u rewind , meaning lower wire resistance for same kv, if u do even a half decent job. Commercially machine wound motors most often are high resistance and therefore get hotter.  
If u can replace that magnet it'll likely solve ur problems otherwise seems trash.  U could try sinking it in acetone but it's a mess especially trying to deal w just replacing one.
```

---
## \#12 Posted by: jbruce Posted at: 2017-10-30T19:27:06.988Z Reads: 62

```
You're saying the factory wire they use to wind it is low quality and high resistance? 

My motor gets warm but never super hot, but I attribute that to me being light weight and riding on mostly flat ground. 

I actually have no clue how that magnet shattered like that. How serious do you think having the magnet missing a piece is? The motor still runs.
```

---
## \#13 Posted by: Hummie Posted at: 2017-10-30T19:33:51.476Z Reads: 62

```
The wire is fine its just they use multistrand as its easier and it will have a but more resistance n heat than a single strand, but it sounded like u were getting worse range and if it's due to the motor then the motor would get hotter.  The busted magnet...maybe its not that bad and a lot still there. I was just reading about imbalances in a motor and increased inefficiency but on the winding side..was thinking maybe hr an example of inefficiency crated by imbalance on the mags side. But maybe ur inefficiency is due to something else if it's not getting hot
```

---
## \#14 Posted by: pat.speed Posted at: 2017-10-30T20:35:25.655Z Reads: 58

```
Just a thought but is it possible that maybe you batteries have degraded without you knowing. This would make it seem like you are using more Wh/mi. 

Let's say you have a 300wh pack, and x is the number of mi you ride

300/x would give you how many Wh/mi you get.

So 300Wh/ say 20mi= 15Wh/mi but if your battteries don't hold as much charge as they used to the pack might only be 280Wh but you wouldn't know this in your calculations unless you checked. So let's assume you still think it's a 300Wh pack. Now since the pack is less Wh you will get less range thus

300Wh/~18mi= 16.6Wh/mi

This might have nothing to do with your problem but it's worth a try. And the numbers used were just random
```

---
## \#15 Posted by: MysticalDork Posted at: 2017-10-30T21:21:41.985Z Reads: 51

```
As long as you don't care about destroying the magnets, I've seen people put the motor bell in a pressure cooker and use the hot water to loosen the adhesive. The heat will also destroy the magnet though.
```

---
## \#16 Posted by: jbruce Posted at: 2017-10-30T22:41:34.890Z Reads: 49

```
My battery may be degraded but my numbers come from ackamaniacs app which records wh used and distance and calculates it like that, thus battery capacity should have no effect.
```

---
## \#17 Posted by: jbruce Posted at: 2017-10-30T22:42:39.069Z Reads: 51

```
Interesting idea, I just don't know where I would get magnets that matche the ones I have now.
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-10-30T23:17:06.556Z Reads: 48

```
Amazingmagnets.com, there are several others. As long as the dimensions are the same and they're strong, they'll work. If possible, get N45SH, they're the strongest heat-resistant ones. You can go stronger, but they don't like heat much.
```

---
## \#19 Posted by: jbruce Posted at: 2017-10-31T02:53:01.645Z Reads: 47

```
I can't seem to find the N45SH on amazing magnets.
```

---
## \#20 Posted by: MysticalDork Posted at: 2017-10-31T05:07:51.782Z Reads: 40

```
Try https://www.kjmagnetics.com, they may have some.
```

---

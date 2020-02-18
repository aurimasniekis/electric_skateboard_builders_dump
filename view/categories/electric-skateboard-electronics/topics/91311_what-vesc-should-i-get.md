# What vesc should i get

### Replies: 42 Views: 610

## \#1 Posted by: hornet90 Posted at: 2019-04-21T14:31:46.007Z Reads: 144

```
Hi all 
Just sold my kaly so im starting a new build i lost track of whats going on with vescs . its going to have a 12s5p two 150/190 kv motors im not looking for top speed 30mph is fine. 
Whats new in vesc is what im asking
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-21T14:37:03.141Z Reads: 142

```
Depends. Where is your last stand point? Which time you stopped looking for vescs?
```

---
## \#3 Posted by: hornet90 Posted at: 2019-04-21T14:37:44.849Z Reads: 139

```
Just under two years
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-21T14:41:00.605Z Reads: 139

```
I‘m into this only one year, but vesc6 derivates became pretty cheap. There are now dual vescs which share one pcb for two motors. Integrated anti spark switches and roll to start features. The new vesc firmware allows you to flash firmware from the master to the slave via CAN bus. Integrated Bluetooth modules. A lot of things happened in the last time.
```

---
## \#5 Posted by: Pablo_702 Posted at: 2019-04-21T14:44:21.001Z Reads: 135

```
Im in the same place as @hornet90 just starting my 2nd build after 2 years of absence, who make these double vesc in one pcb with bluetooth?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-04-21T14:46:07.148Z Reads: 133

```
Focbox Unity from enertion. They now on Easter sale for some more hours. If you buy two it’s 199$ US per one. Maybe you guys want to share 😜
```

---
## \#7 Posted by: Andy87 Posted at: 2019-04-21T14:46:50.607Z Reads: 129

```
https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/
```

---
## \#8 Posted by: Pablo_702 Posted at: 2019-04-21T14:47:44.552Z Reads: 134

```
Arghhh Enertion, i refuse to buy from him, no one else sells these? Are they vesc or a different esc?
```

---
## \#9 Posted by: b264 Posted at: 2019-04-21T14:47:52.270Z Reads: 136

```
[quote="Andy87, post:6, topic:91311"]
Focbox Unity from enertion.
[/quote]

I don't recommend units with 2 ESCs conjoined together, like this one above.  If you have a failure, you have to replace two ESCs instead of one, and less chance of the other side still working after a failure.
```

---
## \#10 Posted by: b264 Posted at: 2019-04-21T14:48:28.044Z Reads: 132

```
What about this one?

https://flipsky.net/collections/electronic-products/products/fs-esc-6-6
```

---
## \#11 Posted by: Andy87 Posted at: 2019-04-21T14:49:33.614Z Reads: 127

```
Flipsky sell dual vescs as well. 4.20hw and hw6. But There is no Bluetooth integrated and the anti spark switch is so so. Besides that they work well. Considering the point from @b264 it’s always up to what you want and need and if you ready to take the risk of breaking only one esc or both.
```

---
## \#12 Posted by: Pablo_702 Posted at: 2019-04-21T15:05:05.085Z Reads: 122

```
Ill check this one out,  have a list of parts sellers?
Like 
Evolve
Diy
Ollin
```

---
## \#13 Posted by: hornet90 Posted at: 2019-04-21T15:25:47.515Z Reads: 118

```
One setup i was thinking of was two vescs and a battery on each vesc lets say 10s 4p it would be lsame  way trampa do there set ups
```

---
## \#14 Posted by: hornet90 Posted at: 2019-04-21T15:32:40.611Z Reads: 116

```
Sorry trampa put 12s lipo on each vesc 6
```

---
## \#15 Posted by: Kingdom421 Posted at: 2019-04-21T15:35:31.377Z Reads: 114

```
Bro idk why no one refers Vanda but my vescs are beautiful and they work great. I've put them through some heavy abuse and they keep ticking.
```

---
## \#16 Posted by: hornet90 Posted at: 2019-04-21T15:36:16.223Z Reads: 109

```
Put alink up for them
```

---
## \#17 Posted by: Andy87 Posted at: 2019-04-21T15:38:23.547Z Reads: 110

```
If you run both vescs on a separated power supply you can’t connect them via CAN bus. I wouldn’t do that if you want to use can.
```

---
## \#18 Posted by: brenternet Posted at: 2019-04-21T15:38:50.747Z Reads: 109

```
The dual esc's recently on offer are convenient and are performing well. It could be argued that simplifying them, removing extra wiring, the tighter footprint and less plugged in components  will reduce failure rates in tight enclosures on hobby boards that are being worked on often.

Whether you buy one or not you're still going to have to listen to Brian regurgitate the same fucking "advice" over and over and over again. So you might as well buy one and reap the benefits.
```

---
## \#19 Posted by: Kingdom421 Posted at: 2019-04-21T15:39:19.947Z Reads: 106

```
https://vandaelectronics.myshopify.com
```

---
## \#20 Posted by: b264 Posted at: 2019-04-21T15:39:52.645Z Reads: 101

```
I don't recommend CANBUS or any connection.  Even use 2 separate receivers for the remote.
```

---
## \#21 Posted by: Kingdom421 Posted at: 2019-04-21T15:41:47.636Z Reads: 99

```
I use canbus it works fine. I run one power supply for both vanda's I haven't had any problems with then. Over 50 miles I believe I have on them if not more. 10s4p
```

---
## \#22 Posted by: Pablo_702 Posted at: 2019-04-21T15:42:42.799Z Reads: 98

```
Mmm interesting when i left the sk8 community can was the only way to run 2 motors at least i dont remember this veing an option, can u elaborate on how this would work? Or is the there a threat talking bout this?
```

---
## \#23 Posted by: Andy87 Posted at: 2019-04-21T15:43:08.560Z Reads: 99

```
Don’t say it’s not working but you have different potentials on different vescs. Google about it and you will understand that it is not a good idea to do so 😉
```

---
## \#24 Posted by: Andy87 Posted at: 2019-04-21T15:47:05.026Z Reads: 99

```
I wonder how you can skate without to making pipi in your pans every single time 😜😂

Yes split ppm might have his advantages as well has CAN bus does. It’s always up to the person and which features are important for this person. I wouldn’t want to miss traction control on a mtb. With split ppm thats not possible. 

And what if I say you your receiver can break down as well 😱 💁‍♂️
```

---
## \#25 Posted by: Kingdom421 Posted at: 2019-04-21T15:47:55.048Z Reads: 98

```
You're saying it's not a good idea to run one power supply for two vests. I have both of vesc connected as one. Master runs the left motor slave runs the right. I don't even get overheating problems
```

---
## \#26 Posted by: Andy87 Posted at: 2019-04-21T15:49:51.412Z Reads: 95

```
No I mean it’s not good to use one power supply for every vesc and than connect them via CAN bus. So two power supplies and CAN, bad idea. One power supply and parallel plug and CAN, good idea.

My bad I mixed that up in your comment. All good 😅
```

---
## \#27 Posted by: Kingdom421 Posted at: 2019-04-21T15:51:00.258Z Reads: 92

```
Yes sir I concur.
```

---
## \#28 Posted by: hornet90 Posted at: 2019-04-21T15:53:46.798Z Reads: 89

```
Are you saying dont use two 10s4p packs trampa 
Push for this on there boards well 12s lipo on each motor
```

---
## \#29 Posted by: b264 Posted at: 2019-04-21T15:55:01.020Z Reads: 89

```
Some remotes, like this one

https://forum./t/how-to-bind-the-mini-remote/95

allow you to bind 2 receivers.  Just hook one receiver up to each ESC.  Easy-peasy
```

---
## \#30 Posted by: brenternet Posted at: 2019-04-21T16:00:59.639Z Reads: 87

```
Add loads of excess electrical components to your build with a history of failure unnecessarily in order to make it more robust.
```

---
## \#31 Posted by: Andy87 Posted at: 2019-04-21T16:04:40.950Z Reads: 89

```
You can look up the wiring diagram here. Also trampa use only one power supply for both vescs. Both vescs are connected parallel to the battery.

https://www.trampaboards.com/manuals.php
```

---
## \#32 Posted by: hornet90 Posted at: 2019-04-21T16:08:43.111Z Reads: 88

```
I like the way they do there loop key
```

---
## \#33 Posted by: trampa Posted at: 2019-04-21T16:49:49.348Z Reads: 85

```
Two power supplies, two VESCs and CAN works a treat on VESC 6. We do that all day long.
```

---
## \#34 Posted by: Andy87 Posted at: 2019-04-21T17:27:10.254Z Reads: 85

```
Nice to know!

So what i get wrong on your wiring diagram @trampa ? Looks like i‘m totally stupid, but I don’t see that second battery for the second vesc and that i mean seriously. I don’t get it.

![image|603x499](upload://rVLIbyJwn4esR1j3NR9dIFPZO3s.jpeg) ![image|690x392](upload://bA7Kxg5OfdPZepYqNzvlWx3endf.jpeg)
```

---
## \#35 Posted by: hornet90 Posted at: 2019-04-21T17:45:46.197Z Reads: 83

```
I picked that up wrong but it is 2 12s lipos
```

---
## \#36 Posted by: Dirt_Bag Posted at: 2019-04-21T20:23:14.188Z Reads: 80

```
i fully agree. the only one i have seen that doesnt have severe issues with 2 vescs on 1 PCB is the flipsky 6.6 dual

the dual 6.6+ (antispark) appears to have issues with the switch breaking.

I am just waiting for flipsky to make a single 100a vesc....
```

---
## \#37 Posted by: trampa Posted at: 2019-04-22T10:40:47.821Z Reads: 75

```
In most cases people prefer one big battery, since charging is a lot more convenient. The VESC 6 is happy to run of its own battery while being CAN connected. No worries!
```

---
## \#39 Posted by: taz Posted at: 2019-04-22T11:26:57.034Z Reads: 70

```
They also had this in their website

![image|690x313](upload://kgF9mvILfKBOW0j2Ox1z5aLtUeb.jpeg)
```

---
## \#40 Posted by: hornet90 Posted at: 2019-04-22T11:56:12.258Z Reads: 69

```
So i did see it
```

---
## \#41 Posted by: Andy87 Posted at: 2019-04-22T11:57:22.866Z Reads: 66

```
That now make more sense.

I didn’t see that one. That’s why I was wondering.
```

---
## \#42 Posted by: taz Posted at: 2019-04-22T11:58:48.695Z Reads: 71

```
No you did not. It was just a figment of your imagination. As am I, and @Andy87 :crazy_face:
```

---
## \#43 Posted by: hornet90 Posted at: 2019-04-22T14:46:18.473Z Reads: 63

```
https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-plus-based-on-vesc6
```

---

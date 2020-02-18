# Anybody sporting bigger motor pulleys? 18T? 22T? Why is 15T and 16T so common?

### Replies: 27 Views: 3841

## \#1 Posted by: itsmikeholland Posted at: 2016-06-18T17:38:55.143Z Reads: 341

```
It seems like having as close to 1:1 as possible to increase speed, is it at the expense of torque or motor health or something? I'm running 12s and 149kv 83mm with a 36T drive pulley, what should I consider besides a bigger belt when bumping up the motor pulley size?
```

---
## \#2 Posted by: Pablo_702 Posted at: 2016-06-18T17:44:28.987Z Reads: 346

```
36T on the motor side??? Are you sure is not on the wheel side?
```

---
## \#3 Posted by: itsmikeholland Posted at: 2016-06-18T17:44:56.913Z Reads: 347

```
From the beginners guide:

83mm Wheel Diameter
245Kv Motor 
6S Battery (24v for simplicity)
45km/h

With this information now you can more easily calculate your pulley sizes and determine the final reduction ratio. As we want to achieve a top speed of 45km/h we can define the last variable, the gearing reduction ratio, to get the desired top speed we want.

There are some important constraints in drivetrain design, when using pulleys & belts, that must be carefully considered. Firstly there is a minimum amount of teeth you should have engaged between the pulley & the belt. It is called teeth-in-mesh and you should have 6 teeth or more in mesh if you want to achieve the maximum torque transfer rates specified. Your ability to transfer maximum torque will be diminished if you have less than 6 teeth engaged. So it can still work just not to its full potential, so maybe the belt will skip over some teeth.

15 to 36 teeth is the ideal configuration to achieve maximum torque transfer when using 5mm pitch pulleys
Second constraint is your center distance 'C', it is best to have the shortest possible center distance. A shorter 'C' means less leveraging forces being applied onto the motor mounting hardware, it can help to reduce vibrations and minimizes the span of the belt. Basically the shorter it is the less chance the mount will flex, warp, bend or snap which is important when you are frequently accelerating & braking hard.

However you cannot make it too short because you also need your motor to have some clearance from the truck hanger so you can make a turn. It is also worth noting that the longer your center distance the more the belt will wrap around the pulleys so it can actually result in more teeth in mesh, but it is probably better to keep your center distance short and go with a larger pulley to obtain more teeth in mesh.
```

---
## \#4 Posted by: itsmikeholland Posted at: 2016-06-18T17:45:12.240Z Reads: 325

```
oh shoot, totally meant drive wheel pulley is 36T
```

---
## \#5 Posted by: itsmikeholland Posted at: 2016-06-18T17:49:30.868Z Reads: 320

```
So it seems that there is a better torque transfer when using larger motor pulleys, but it doesn't mention anything about why you wouldn't want to go bigger. Why is 15T the magic number for this kind of set-up?
```

---
## \#6 Posted by: Pablo_702 Posted at: 2016-06-18T17:53:37.103Z Reads: 318

```
I have the same motor as you and same wheel size,  i got 36/16 i will be putting it together in the next few days, theres a calculator where you put the kv, efficiency, pulley sizes and cell count and it will give you all the speeds you can play with that to see what kind of pulleys you want, i couldn't find it im from my cell phobe but just tipe in the forum speed calculator or something like that
```

---
## \#7 Posted by: Pablo_702 Posted at: 2016-06-18T17:57:51.194Z Reads: 313

```
http://toddy616.blogspot.be/2013/07/electric-skateboard-calculator.html?m=1

There you go man
```

---
## \#8 Posted by: itsmikeholland Posted at: 2016-06-18T18:07:46.725Z Reads: 300

```
Thanks, I was using this to see what difference a bigger motor pulley would make and it seems to take my weighted top speed over 40mph. I'm curious as to what that actually translates to with performance, since I'm shooting for just an 18mph top speed but I also don't want to waste any energy from the batteries to the wheels. Is the acceleration massively decreased? Is the ability to get up hills diminished? Does it draw more amps and translate to less range? Stuff like that.
```

---
## \#9 Posted by: Pablo_702 Posted at: 2016-06-18T19:09:58.947Z Reads: 291

```
<img src="/uploads/db1493/original/2X/f/f5f594adcfb52bf370663a0965f76e20cc67440e.png" width="281" height="500">

Thats what u should get, how are you getting 40mph?
```

---
## \#10 Posted by: CSN Posted at: 2016-06-18T19:13:56.069Z Reads: 256

```
as your motor pulley gets larger then it might conflict with the motor mounting bolts which means to tighten the motor for belt tension then the pulley might have to be removed.

It depends on the mount. The newer mounts that use the wider bolt pattern would not be an issue.
```

---
## \#11 Posted by: itsmikeholland Posted at: 2016-06-18T19:28:28.357Z Reads: 247

```
.....by increasing the motor pulley teeth/circumference
```

---
## \#12 Posted by: itsmikeholland Posted at: 2016-06-18T19:31:26.209Z Reads: 243

```
awesome, is there any discernible difference in performance with a larger motor pulley? I'm thinking of playing around with an 18T or a 22T since they're pretty cheap, but there doesn't seem to be anybody else thats really done it and reported any positives or negatives regarding the performance
```

---
## \#13 Posted by: Pablo_702 Posted at: 2016-06-18T19:33:45.305Z Reads: 239

```
I thought we still talking about the 36T,  another thing you could do to achieve higher speeds is increase the size of your wheels l, theres some 107mm that are super nice, it might take a little longer to reach its max speed but i think i would prefer a slowy steady increase in speed rather than going from 0-60 real quick
```

---
## \#14 Posted by: itsmikeholland Posted at: 2016-06-18T19:40:47.805Z Reads: 237

```
Yeah the 107mm wheels are MASSIVE, I got to hold one of them at eglide last weekend and was baffled at how its mass doesn't outweigh the theoretical higher top speed. I've got some 90mm wheels here as well but I've noticed even just from pushing that they take way more effort to go fast, I'm curious as to whether bigger wheels have any negative effect on the motor or amp usage, I'm no mechanical engineer (yet) but I feel like maybe bigger wheels translate to a higher top speed but a lower amps:mph ratio because of the size and effort it takes to get up to speed. With only a 18mph top speed goal, Im basically just seeing what set-ups will use the energy more efficiently. For example, if im not mistaken it requires more amps to get a 90mm wheel to go 18mph than it does to get an 83mm wheel to go 18mph, so I'm wondering if it takes more amps to to get an 18T/36T or a 22T/36T to go 18mph than it does for a 16T/36T. Does any of this make sense?
```

---
## \#15 Posted by: Pablo_702 Posted at: 2016-06-18T19:49:01.301Z Reads: 225

```
If your goal speed is 18 then 36/16 with 83mm should doit, and by the calculator youbeven would have 2mph to spare, also the motor we have from what i read and seen are ideal for torque so i dont think it will put much stress having 90mm,105mm or 107mm
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-06-18T20:19:19.370Z Reads: 223

```
I think you've got the right idea. On 6s, 245kv, I tried running a 20/36 ratio with 97mm wheels to boost top speed and was able to get up to ~28mph, which was really the only positive, I would say. Downsides were that the motor and esc got much hotter, takeoff performance was terrible, significant voltage sag when accelerating, and decreased range due to the much higher amp draw, I assume. Since we are basically running at one speed with the gearing, motor and battery setup we choose, I compare it to picking one of the gears on your car to run the whole time. Higher gearing reduction and smaller wheels, might equate to first or second gear, with great takeoff performance, at the expense of high speed, but lower stress on the propulsion system due to the higher mechanical advantage. Conversely, my 20/36, 97mm wheel setup might be more like 3rd or 4th gear where taking off sucks and puts a huge strain on the system to get things moving, but really shines when you hit top speed. If you could do a flat out high speed run in that configuration, it might not be so bad, but every time you slow down and accelerate again, it strains the system and draws lots of amps = excessive heat & decreased range. There is definitely a science to this stuff and a reason why higher gearing reductions are generally preferred. At least that has been my experience.
```

---
## \#17 Posted by: itsmikeholland Posted at: 2016-06-18T21:59:01.830Z Reads: 218

```
awesome explanation! So basically for absolute minimum strain at the expense of speed, the entirety of the mechanics is a balance between how much clearance you need, getting your wheel pulley as close to the size of the smallest ideal wheel as possible, then getting your motor pulley as small as possible without sacrificing torque transfer via less teeth-in-mesh, and keeping the belt length to a minimum while keeping in mind the necessary clearance for your trucks and the road. Basically you decide where to compromise based on how fast you desire to go, which leaves most people at 12s 83mm 16T/36T and ~200kv. awesome awesome awesome, I'm glad you took the time to explain this all!
```

---
## \#18 Posted by: lox897 Posted at: 2016-06-18T23:23:49.740Z Reads: 202

```
The motor will have to work very hard and will draw a lot of amps. If you are going to try this make sure you have the cash for another motor. Not to discourage, for science right?
```

---
## \#19 Posted by: whitepony Posted at: 2016-06-19T08:18:18.185Z Reads: 197

```
im toying with building a high speed board someday, pretty much just for fun and maybe to break the eboard speed record. :stuck_out_tongue:  i dont trust in hubs for that because all concepts dont convince me from an urethane <-> core coupling point of view which is an issue for really high wheel rpms! for that kind of concept, large motor pulleys would be required too - and the larger they get the more torque transfer you got, allowing 9mm belts! 

long story short: if your motors are made for it (low kv), or you have the torque from multiple motors, a large motor pulley has only benefits!
```

---
## \#20 Posted by: itsmikeholland Posted at: 2016-06-19T16:21:13.006Z Reads: 187

```
Im happily discouraged from wasting time and money! Ive still got plenty of ideas to play around with, especially my blinkers, maybe even a 3 truck system that allows you to easily switch between push and electric? Nuclear battery pack (i wish)? So many things!
```

---
## \#21 Posted by: lox897 Posted at: 2016-06-20T02:01:02.247Z Reads: 166

```
Well, good luck! Hope it works out!
```

---
## \#22 Posted by: Mikeomania12 Posted at: 2016-08-04T18:58:50.034Z Reads: 144

```
I have a 6s dual drive 245kv motors with 22t/36t ratio with 97mm wheels. It works pretty well. 
Start form stop is a little twitchy.
Max speed is 35mph, 
Range on my 20ah battery is 25mi. 
But the components get very hot. Cant even touch my motor sometimes. 
Esc get too hot to touch even with fans. but haven't had one fail in over 1000mi. esc is skyrc toro 120amp. 
I did have a sk3 motor fall apart though. 
I think the most impacted by this gearing is the motor mounts which keep breaking on me. I have tried every motor mount on the market they all snap eventually. This stopped when i had my own mount made out of steel. 
I suspect the other mounts cant handle the increase forces because of this gearing. Or maybe they are just too thin.
This gearing deff takes its toll on the life of the parts because all the acceleration and braking forces are much larger. 
Keep in mind i ride very hard :slight_smile:
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-04T19:02:33.368Z Reads: 140

```
You could try Enertion's mount for caliber trucks, they're made of carbon fiber so they're light weight and durable, thought not very good at spreading heat which sounds like a problem you have. Perhaps upgrade to a higher voltage ESC?
```

---
## \#24 Posted by: Mikeomania12 Posted at: 2016-08-04T19:07:35.681Z Reads: 139

```
I have 2 vescs that i intended to use with 15t/36t ratio. and upgrade to 12s to get me up to 50mph but im very disappointed to hear about this erpm limit on the vesc so i wont even gain any speed with my 245kv motors and i dont even want to use them anymore.
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-04T19:09:55.495Z Reads: 138

```
Yea you'll get VESC errors and probably blow a component if you run that. 50mph is pretty crazy stuff. You can try running dual TB ESCs which might be able to handle the speed. If you do try, please don't ride that speed in areas with any people or animals, and gear up!
```

---
## \#26 Posted by: Mikeomania12 Posted at: 2016-08-04T19:12:02.492Z Reads: 140

```
i doubt ill be getting to that speed before i sell my vescs :frowning: need to recoup my money lol
maybe i can trade them to dexter for that dual hv esc.
```

---
## \#27 Posted by: Russell23 Posted at: 2017-07-11T20:41:38.378Z Reads: 76

```
@Mobutusan hey I planning on using a 20/36 gear ratio with a sk3 192kv motor with 83mm wheels. I'm afraid that it will destroy my maytech vesc as it's a cheap Chinese vesc but the thing is I only weigh 48kg.
```

---

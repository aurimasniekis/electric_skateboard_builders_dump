# Lithium ion battery pack anatomy

### Replies: 36 Views: 2475

## \#1 Posted by: moe_lester Posted at: 2017-03-05T13:10:07.832Z Reads: 227

```
Does the anatomy of this battery pack make sense ? 

Its meant to be 8 in series and 4 in parallel.

I don't think I got the 4 in parallel right ?

Also do you guys know what type of wires I need to buy for this, I have already bought a nickel/battery tab machine and the lithium ions (samsung) but I don't know which wires to pick?

<img src="/uploads/db1493/original/3X/7/1/713a0781b66dc5ecbfe5d83f0b291f626fd8efc5.jpg" width="374" height="500">
```

---
## \#2 Posted by: Sander Posted at: 2017-03-05T14:45:51.010Z Reads: 205

```
looks good.
```

---
## \#3 Posted by: eLDoska Posted at: 2017-03-05T15:08:03.888Z Reads: 197

```
your scheme is not incorrect, but in your case you need to balance 32 cells and in "normal" 8s4p - only 8
```

---
## \#4 Posted by: moe_lester Posted at: 2017-03-05T15:13:51.405Z Reads: 201

```
Not sure what you mean, but I'm gonna have a BMS to balance cells. I have created another one but I do not know which is correct. 

Right now Im just designing the basic anatomy of the battery cells so I do not do anything wrong.

What do you think of this one?

<img src="/uploads/db1493/original/3X/0/2/02703483d205a69cdc41459a424914d3fd4abc2d.jpg" width="375" height="500">
```

---
## \#5 Posted by: Smorto Posted at: 2017-03-05T15:25:11.981Z Reads: 188

```
This gives me an idea for a modular type battery pack. I am very new to building packs and know very little about it so Im not sure if this will work at all but here goes. What if instead of soldering the packs in parallel, you took the positive lead and the negative lead and put them into and XT60/XT90 connector. Then did the same for each pack and connected them. This would be useful if you were flying and needed to break them down into smaller <99 WH packs (8*3.7=29.6) (29.6*3=88.8 WH) I was assuming a 3000mah cell for that last equation. Here is a digram that represents what I am saying.
                        <img src="/uploads/db1493/original/3X/e/2/e23605f7e752c91d284b5ebb98e97e79613846f1.jpg" width="374" height="500">
```

---
## \#6 Posted by: Hummie Posted at: 2017-03-05T15:28:00.597Z Reads: 179

```
U have 4 rows of 8 cells in series.  Each cell is individual in this way. If u putt four in parallel...and then put that four in series with 4 in parallel etc. ..then the parallel four cells will be working together as one and ull only need one balance wire for those 4
```

---
## \#7 Posted by: Smorto Posted at: 2017-03-05T15:34:25.324Z Reads: 180

```
Im curious about these diagrams as well as I am trying to learn as much as possible about building your own pack. Would you point me in the direction of a diagram fro a compact or flat 10s3p 10s4p, or 8s4p? Preferably one that is easy to understand for a beginner in the field like me.
```

---
## \#8 Posted by: eLDoska Posted at: 2017-03-05T15:35:26.604Z Reads: 178

```
your second is the same as the first :slight_smile:
 
"normal" sheme:
<img src="/uploads/db1493/original/3X/8/9/897409379d92627323c0a4e74e7b7a34eaef6166.jpg" width="375" height="500">
```

---
## \#9 Posted by: moe_lester Posted at: 2017-03-05T15:47:17.458Z Reads: 159

```
I am using 18650 samsung 3.7v with 2500mah each. 

So my question is once I add a BMS will the first battery diagram post I made earlier work as a 8s4p battery pack making 8 series = 29.6 volts and 4 parallel = 10,000 mah in total??

Sorry guys I'm bit of an amateur at this, don't know what "normal" sheme means?
```

---
## \#10 Posted by: Hummie Posted at: 2017-03-05T16:10:08.903Z Reads: 154

```
the first you posted will make it very difficult to add a bms as while it's said the cells are in parallel, they really aren't and instead it's 4 strings of cells in parallel.  you want to put them in parallel so they are effectively one battery when in parallel.  yes you'll have 10ah either way but it's about being able to add a bms.  the last pic above the cells are grouped in parallel so they behave as one cell and you could add a bms volt sensor to one and they willl all show the same..as they're truly in parallel
normal scheme
```

---
## \#11 Posted by: moe_lester Posted at: 2017-03-05T16:28:35.867Z Reads: 160

```
@hummie 

I made a new layout what do you think? 

The green is the nickel strip and I know once I add the BMS i will have to attach each of the 8 wires to each 4 in parallel group?


<img src="/uploads/db1493/original/3X/4/7/47d9dac7ac86e6a9fff6554a5e805a0d9958bc26.jpg" width="374" height="500">
```

---
## \#12 Posted by: Maxid Posted at: 2017-03-05T16:36:28.660Z Reads: 146

```
looks good - just make sure to use multiple layers of nickel on the series connections - or even better reinforce with copper.
```

---
## \#13 Posted by: Hummie Posted at: 2017-03-05T17:04:30.420Z Reads: 135

```
i wouldn't say you have to attach each of the 8 wires to EACH of the 4 in parallel.  you only need to attach to one in the four in parallel  or just the tab and they'll all have the same voltage
```

---
## \#14 Posted by: Smorto Posted at: 2017-03-05T17:11:38.873Z Reads: 135

```
Hello, I am thinking of using a design like this my only question is where on each parallel group would you put the balance wire, and how exactly to make the bottom connection (the one that looks like a U on the very bottom) with nickel strip and a spot welder.
```

---
## \#15 Posted by: Hummie Posted at: 2017-03-05T17:23:19.415Z Reads: 137

```
you can put the balance wires anywhere on the parallel pack and it'll get the same voltage.   maybe do a long strip of nickel for the bottom and spot weld the ends
```

---
## \#16 Posted by: Smorto Posted at: 2017-03-05T17:50:11.884Z Reads: 132

```
Could I well the bottom + and the - by having the cells vertical then bending them flat after welding?
```

---
## \#17 Posted by: Hummie Posted at: 2017-03-05T17:55:23.299Z Reads: 136

```
dont know how much bending the tabs can do. likely.  but if you just spot weld the two tabs at the bottom..no bending necessary.  you'll need longer tabs in that instance
```

---
## \#18 Posted by: Smorto Posted at: 2017-03-05T17:57:17.287Z Reads: 132

```
Im sorry but I need a visual or something to understand exactly what you are saying as I am having a hard time understanding it. I am very new to building packs which is why.
```

---
## \#19 Posted by: Hummie Posted at: 2017-03-05T18:07:22.232Z Reads: 132

```
cant understand u either.  If u do a drawing we will know
```

---
## \#20 Posted by: Smorto Posted at: 2017-03-05T18:26:16.181Z Reads: 136

```
I am saying something like this. This is a mockup with AA and AAA batteries and only a pack of 2.

Weld them like this
<img src="/uploads/db1493/original/3X/c/1/c1043f6721460e89bcedafb8b8a3a44145cb61e8.jpg" width="690" height="459">

Then bend them flat
<img src="/uploads/db1493/original/3X/0/2/0211cc40aff9fcc72b67ef30a1b9ff9bea758638.jpg" width="690" height="459">
```

---
## \#21 Posted by: Hummie Posted at: 2017-03-05T18:29:10.866Z Reads: 124

```
Sure.  If it doesn't break.
```

---
## \#22 Posted by: Smorto Posted at: 2017-03-05T18:40:32.923Z Reads: 121

```
Awesome. We'll see how it goes if I try it.
```

---
## \#23 Posted by: moe_lester Posted at: 2017-03-06T00:01:15.992Z Reads: 115

```
Also does anyone know what charger to use for the battery, Im using samsung 25r batteries (3.6v at 2500Mah) in the 8s4p structure I have mentioned and I'll be adding a Bms later. 

Does anyone know a charger that i can use for the batteries I have selected? 

What sort of charger rating do I need because I have no idea :/ 

thanks for your help
```

---
## \#24 Posted by: Hummie Posted at: 2017-03-06T00:19:53.815Z Reads: 114

```
If ur adding the bms later, and ur responsible, despite being new to it, and u can follow basic stuff, you could bulk charge!!  But I'm not going to further help u with it and don't blow up ur neighbor.
Get a multimeter immediately.
```

---
## \#25 Posted by: Jammeslu Posted at: 2017-04-11T10:08:29.980Z Reads: 93

```
Is it possible to use silicone wire at the U bend?
```

---
## \#26 Posted by: moe_lester Posted at: 2017-04-11T11:58:28.377Z Reads: 92

```
Very good question, it'll make shit a whole lot easier.

I actually don't know, anybody know if you can use a silicone wire to connect cell 4 to 5 instead of bending the nickel strip???
```

---
## \#27 Posted by: Stefan Posted at: 2017-04-11T12:20:01.903Z Reads: 91

```
I did that but i haven't tested the battery yet.
```

---
## \#28 Posted by: jujet Posted at: 2017-04-11T15:16:48.694Z Reads: 87

```
You should do some more reading on this forum before rushing into anything stupid.
```

---
## \#29 Posted by: t0m_r1dd1e Posted at: 2017-04-11T15:41:41.747Z Reads: 87

```
You can absolutely do this. Use 10 gauge silicone wire though. And make sure your soldered connections are really good. Tin the wire ends making sure the wire is saturated all the way through with solder and of course make sure the wire is protected and won't get cut or kinked.
```

---
## \#30 Posted by: Maxid Posted at: 2017-04-11T15:42:18.968Z Reads: 88

```
sure - just make sure to use thick wire (like 8AWG).
I do the same thing on my build where I connect two 5S batteries together via a bullet connector.
```

---
## \#31 Posted by: moe_lester Posted at: 2017-04-11T18:31:34.991Z Reads: 83

```
Guys Im having problems with this pack so I'm gonna take it all apart and take off the nickel strips. Recharge the cells individually. then put it back together using new nickel strips and reattaching the BMS, also use a 10AWG wire for connecting cells 4-5.   

Im doing this because my voltage on my battery pack changes as the pack moves, which indicates faulty connections somewhere. Also using a bms is making me suspicious, coz my pack only charges to around 32v when it should be 33.6v (8s - 8 x 4.2v = 33.6v). 

Does anyone know what else this could be??

Also whats the best way to remove nickel from 18650 cells??
```

---
## \#32 Posted by: Pantologist Posted at: 2017-04-11T19:33:16.246Z Reads: 80

```
Have you tried testing each parallel pack with a multimeter? 

You have to carefully pull them off with pliers.

That's really amounting so best to find the source of the issue and fix that.
```

---
## \#33 Posted by: moe_lester Posted at: 2017-04-11T19:47:46.306Z Reads: 77

```
yes cell number two is usually lower and cell number 7 / 8 are always about 0.8 volts above the rest. It so strange. 

Thats why I'm gonna recharge each cell individually before putting it back together. I gonna use a higher amp setting on my spot welder to make sure they don't come lose again. I think they came lose from the insane vibrations while i was riding...to give u an idea the vibrations where so intense if I was a girl i'd be leaving a trail. This is why Im gonna eventually use all terrain wheels which makes the vibrations less due to larger wheel base. 

If you guys have any other ideas about improving diy battery builds for eks8 feel free to shout them out. DIY battery packs are insane when you know what your doing because you can customise your packs to be more powerful/less or have more/less capacity and you can make the battery pack the shape you desire for your enclosure.
```

---
## \#34 Posted by: Jammeslu Posted at: 2017-04-11T22:23:10.918Z Reads: 63

```
So to get A shorter pack you could put silicone wire then in the middle and fold over? And i stenad of 8 awg would two 12 awg work?
```

---
## \#35 Posted by: moe_lester Posted at: 2017-04-12T21:55:19.133Z Reads: 61

```
I can't think of any reason why that wouldn't work. Just make sure you solder properly and protect the soldering with heat resistant tape or adhesive card etc.  

From my experience the pack needs to handle vibrations. Just make sure their will be no direct pressure on all your solder or joints from the vibrations inside the battery enclosure. I gonna make an update in the next few weeks hopefully about how I remade the pack.
```

---
## \#36 Posted by: Jammeslu Posted at: 2017-04-12T22:28:41.245Z Reads: 59

```
Thanks, going to cover the pack in foam
```

---

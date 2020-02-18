# Need help validating wiring diagram for a 2-battery e-skate setup

### Replies: 9 Views: 1376

## \#1 Posted by: louwii Posted at: 2017-11-14T01:31:16.875Z Reads: 159

```
Hi there,

After spending days looking at posts about every topic possible, I have a better idea of how to build my first esk8. The only subject I need help on is the wiring.

So in order to get my head around that topic, I first created a simple wiring diagram:
https://docs.google.com/drawings/d/1uPZMhwGIea7Dl05Mq1R6ijs3ZflVSmlJACBvxkrA0_8/edit?usp=sharing
Nothing complex. I'm planning on using 2 5S batteries with a VESC.

Then, I looked at how to charge batteries, and that's where it became a bit more complex. If I understand correctly, I either need to buy a battery charger like that thing (https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html) or go the hardest way and setup a BMS and buy a cheap 37V charger to plug-in.
Why not ? Let's try and do that.


So I looked around and tried to build the next 2 diagrams.

First one is with a BMS for charge and discharge:
https://docs.google.com/drawings/d/1rbgXgp2UWZn-bDWz9UDOltWFuaFqIwo-AvzLW_csUqQ/edit?usp=sharing

The second one is for charge only:
https://docs.google.com/drawings/d/1iVFi9Qhvsu4i0A5HA5kjhf4KGsKHbtk0neIcVBMBFxA/edit?usp=sharing

**Are those even OK ? Have I made any mistake ?**
It's actually quite hard to find proper information as there's a ton out there, but I think I got it right.

I'd be happy to fix those diagrams if I made any mistake. As there's no post about wiring in the FAQ, I was thinking that maybe my post could go in there if it's any good. My first goal is to learn how to properly wire my setup, but I'm also happy to help any beginners out there. I can also create other diagrams for popular setup if you think it could be of any use (like a dual motor setup for instance).

Thanks !
```

---
## \#2 Posted by: PredatorBoards Posted at: 2017-11-14T06:12:19.043Z Reads: 112

```
Assuming you are running off this BMS

http://www.electric-skateboard.builders/uploads/db1493/original/2X/6/65d7443e0ae741e1d89e4e9e9fa571e432b63cbf.JPG

Then yes the battery is wired properly. However, for your charge only diagram, there's tons of excess splicing which makes the diagram hard to follow. You should directly connect a dedicated charge port wire to the battery positive, a dedicated ESC positive wire to the battery, a dedicated -P charge port wire, etc. 

Also I would eliminate the extra set of balance wire connectors, that's just another point for potential failure. Here's my LiPo battery pack and how I wired the balance leads to the BMS:

<img src="/uploads/db1493/original/3X/7/8/78cff2b2a7c15f5223ca1e9b9c3af79cd83524db.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/e/1eaf949d84573c1a7db3a7c7d8eed2e348616389.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/1/610709b040ab8e7f6c17c03583a484a91303dad0.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/c/5/c5c954debfc80ba0bc67af836c66cb1f9a2fb6c6.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/d/2d5508d64bdb03caac3c8e52b445027ab56c8268.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/3/8397b5625ea7cbea82b3d38a0a05c10968f557a0.JPG" width="666" height="500">
```

---
## \#3 Posted by: louwii Posted at: 2017-11-14T06:42:14.435Z Reads: 97

```
Thanks !

I think I got my charge only diagram right then, I'll try to make it more readable. Not easy to draw lines in every directions and keep things clear at the same time.

And thanks for the pictures. For coupling your balancing ports all together, it seems that you just removed the pins from each white connector and inserted them all into one connector, right ? Not even soldering required ?
```

---
## \#4 Posted by: PredatorBoards Posted at: 2017-11-14T06:51:27.079Z Reads: 93

```
Yep. Keep it simple stupid. Words to live by
```

---
## \#5 Posted by: PredatorBoards Posted at: 2017-11-14T06:53:47.886Z Reads: 90

```
It's not just the drawing of the diagram, but the actual principle of making every wire 'dedicated' and minimizing splicing. Electrically everything works, however future maintenance and upgrades will quickly become a pain in the ass. Everything should be self contained to avoid confusion and easy replacement.
```

---
## \#6 Posted by: PredatorBoards Posted at: 2017-11-14T06:57:20.043Z Reads: 86

```
Also note how the black balance wires are ignored. Even the first one.
```

---
## \#7 Posted by: louwii Posted at: 2017-11-15T03:36:44.929Z Reads: 63

```
I'm not sure I follow you here.
I tried to make everything modular, so everything can be remove or disabled easily, that's why I use connectors almost everywhere.
What you say is that I should use less connectors and just solder everything together ?
```

---
## \#8 Posted by: PredatorBoards Posted at: 2017-11-15T07:08:17.401Z Reads: 60

```
No I'm saying you should make sure that every connector/wire is connected to the positive/negative terminals of the battery/BMS. Your current diagram shows a ton of splicing off a single battery positive wire.
```

---
## \#9 Posted by: louwii Posted at: 2017-11-15T07:26:27.510Z Reads: 59

```
Oh, yep, got it. Thanks
```

---

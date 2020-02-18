# 3D printed direct drive gears

### Replies: 11 Views: 2570

## \#1 Posted by: esk8guy Posted at: 2017-10-03T01:45:55.572Z Reads: 273

```
has anyone had experience or heard of someone experimenting with 3d printing direct drive spur gears? i imagine these would hold up the same as the pulley gears that are 3d printed? or would they possibly have more wear on them since it is a gear on gear contact?
```

---
## \#2 Posted by: MrHappy Posted at: 2017-10-03T01:47:58.842Z Reads: 274

```
Wayyy more wear. With a belt drive, at least the belt takes some of the beating. With direct drive, youll crack em apart the first time you break hard, depending on what type of filament you use.
```

---
## \#3 Posted by: esk8guy Posted at: 2017-10-03T01:49:43.126Z Reads: 274

```
so it wouldnt really even be worth experimenting 3d prints? i might take the laser cut route as that might give me a better result. but to my understanding abs with a heavy infill is much stronger
```

---
## \#4 Posted by: MrHappy Posted at: 2017-10-03T01:51:54.105Z Reads: 264

```
Expirimenting with printing for testing the size and how they will fit is a great idea, but dont expect much life out of it, unless you do an extremely heavy infil. At that point, having a company cnc might be cheaper, and last longer.
```

---
## \#5 Posted by: gogomrrobot Posted at: 2017-10-03T01:58:28.134Z Reads: 252

```
Look @Nowind direct drive system.  He uses a nylon gear (drive wheel gear) and then the motor spur gear is aluminum.  Nylon is incredibly strong for drive gears. This works out very well it seems. I have the setup myself. The nylon is somewhat self-lubricating but grease helps.  I think he has some wear and tire pictures on the site... he has very little to no degradation.

http://www.electric-skateboard.builders/uploads/db1493/original/3X/c/3/c31665971c14106bfb65829c755befdbfe1fb52a.JPG
```

---
## \#6 Posted by: chidi21 Posted at: 2017-10-16T07:52:54.531Z Reads: 223

```
Hey esk8guy, I am currently working on exactly what you are talking about;
<img src="/uploads/db1493/original/3X/c/c/cca627637b7475af67ab1b8de11a02611ac5825d.jpg" width="690" height="387">
<img src="/uploads/db1493/original/3X/f/f/ff761eb9eddc1a50427b0d6efb26bb0ce99e694d.jpg" width="690" height="387">

What I have learned about making my own "Geared Drive" (direct drive is technically not correct) is that the only material that will hold up is Nylon, MatX ASA or a Polycarbonate filament. Even if you use these filaments they are not that easy to print with but once you get them right you will find that they are really strong. More important than just getting the right material is the alignment of the gears. You will notice that @Nowind had to mill flats on his trucks in order to get the gear alignment perfect and that is really the key to the longevity of the gears.

You might get some decent ride time out of the nylon to nylon gears but a metal to nylon combo will give you the best results with the motor gears made of metal. If you do decide to try the 3D printed route like me I suggest you get the gears made by [shapeways.com](http://www.shapeways.com). They use industrial SLS machines and the quality of the parts are superior to anything we could print at home (I own a few 3D printers myself so trust me on that ;-)).
```

---
## \#7 Posted by: Sippahodge Posted at: 2017-10-17T23:21:59.407Z Reads: 194

```
What about glass filled nylon?
```

---
## \#8 Posted by: wafflejock Posted at: 2017-10-17T23:25:36.568Z Reads: 194

```
There are printers that can add Kevlar reinforcement to parts but haven't heard of any that add glass fiber reinforcement and not really sure how that would work (honestly not sure how the Kevlar one works either).  I used plain Nylon (Taulman 645) to print some pulleys on a belt drive setup and so far so good, but only a few days into testing these in place of a metal one I've been running for a while.  Planning to use a nylon printed one with an ebike setup too but need to wait a week or so for the belt to ship.

---

As mentioned in the previous post printing with Nylon can be challenging.  I found using a chamber around my printer to manage the temperature and therefore warping (keeping it above 50C is ideal so it doesn't go through its glass transition and warp as much while printing) and using PVA glue (Elmer's brand white glue mixed with some water) on the bed works well.  Still hard to print anything big but works great for pulleys or gears.  I also print extraordinarily slow with it and it requires precooking to get all the moisture out since it sucks up water from the air (boils while printing putting steam pockets in the printed part).

https://photos.app.goo.gl/OIWyPw0BGzFVCkEy1

---

Since I started with a reprap prusa i3 based (first version, clone DIY kit), I had to upgrade to an all metal hot end (e3d v6) so I could get the filament up to temperature without cooking anything in the hot end (needs to be at least 260C basically).
```

---
## \#9 Posted by: Sippahodge Posted at: 2017-10-18T00:28:40.598Z Reads: 184

```
Glass filled nylon is a filament offered by the commercial 3d printers here in brisbane, says it has properties comparable to aluminium.
```

---
## \#10 Posted by: gogomrrobot Posted at: 2017-10-18T01:17:14.122Z Reads: 185

```
Wow that's a near close to identical copy of the original work. I mean you don't have the stainless steel and aluminum pieces but it's damn close!!!

I love the direct drive tech... my only peeve is that when the system isn't engaged like on a push start or standing still you feel the gears "click" which doesn't happen on belt drive.

How many iterations did you take to get it right?

Did you have to mill the trucks?
```

---
## \#11 Posted by: chidi21 Posted at: 2017-10-18T12:58:41.335Z Reads: 172

```
Hey Goldie, yes @Nowind did a good job showing how he put everything together in his original post on Direct Drive. I am just testing to see if 3D printing could replicate the experience. I am not a machinist like Jenso so I can only do what I am good at which is additive manufacturing. This is just my first iteration and my objective was just to test the concept. I have decided not to mill my trucks, instead I think I will use different trucks like the MBS Matrix 2's since they have a uniform extrusion. It would be cool if people could just print our the parts at home but I am far away from that. Once I nail down a decent design I will get them printed all in Nylon and Polycarbonate and do some long-term testing. I would still advise people to just get Jenso's Direct Drive if they want something that has been tested.

I completely agree with you regarding the issues with a geared system, I actually have Jenso's chain drive which I love but I think it's worth pushing the technology to see what else is possible.
```

---

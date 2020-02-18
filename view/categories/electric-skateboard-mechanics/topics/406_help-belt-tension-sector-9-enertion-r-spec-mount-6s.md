# \[Help\] Belt tension &#124; Sector 9 &#124; Enertion R Spec &amp; Mount &#124; 6s &#124;

### Replies: 36 Views: 5736

## \#1 Posted by: lilracerboi Posted at: 2015-11-03T17:55:47.591Z Reads: 296

```
I have an issue with my belts going bad so quickly. I remember reading somewhere here that someone had a belt go for over a year without malfunctioning.

I've already gone through 3 belts and it's only been 2 months since I got my board running. I feel like it's the tension of the belt.

I don't what kind of tension is suitable for it to not break. My motor mount is Enertion's mount.

I would post a photo, but I'm not home at the moment.
Anyone have suggestions?
```

---
## \#2 Posted by: cmatson Posted at: 2015-11-03T17:57:47.924Z Reads: 291

```
enertion has a video on his youtube channel about setting up his motor mount, and it includes belt tension.

I ran one of enertion's belts for over a year before it broke, so it's definitely not the quality of the belt.
```

---
## \#3 Posted by: torqueboards Posted at: 2015-11-03T18:18:15.284Z Reads: 286

```
You can use a cheap belt and they would even last. It's the angle or alignment of your setup. Your belts being too loose that the teeth get pulled off and/or similar.
```

---
## \#4 Posted by: longhairedboy Posted at: 2015-11-03T18:36:28.467Z Reads: 287

```
all of my belt breaks have been due to misalignment or bad tensioning as well.
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2015-11-03T18:52:28.260Z Reads: 284

```
Having the belt too tight will create friction and heat and ruin the belt as well. I made all 3 mistakes...too loose, too tight, not aligned.
```

---
## \#6 Posted by: lilracerboi Posted at: 2015-11-03T19:20:00.719Z Reads: 316

```
Is there a rule of thumb when putting the belt on? I just put a new belt on last night and it's pretty tight. If I try to loosen it, it'll just get too loose.

Also, Enertion's video didn't really help.
```

---
## \#7 Posted by: Jeff Posted at: 2015-11-04T00:34:07.278Z Reads: 370

```
Also, check to make sure you don't have any anything stuck in the pulleys. I once had a tiny rock that wedged itself in there and broke two belts because I didn't notice it.
```

---
## \#8 Posted by: onloop Posted at: 2015-11-04T01:44:53.158Z Reads: 376

```
1. Pull the belt as tight as possible so that you can feel the resistance increase in the wheel when you try to rotate it.... (rotating the motor should also feel more restricted)

2. Now... Loosen the belt fully so that there is zero resistance felt when rotating the wheel.
Now you have experienced both extremes, too tight & too loose.

3. NOW... Slowly increase the tension until you start to feel the rotation of the wheel become very- slightly-restricted by the tension.... STOP.

The aim is to get the belt tight, but not put unnessecary force into the bearings.

With the correct belt tension the wheel will feel loose and free and the belt will feel firm without slack.
```

---
## \#9 Posted by: lowGuido Posted at: 2015-11-04T05:13:48.025Z Reads: 372

```
I just broke my first belt the other day.
It had done just over 400km and had 3 holes in it from small rocks.
```

---
## \#10 Posted by: CSN Posted at: 2015-11-04T05:55:15.498Z Reads: 373

```
Check out how Metroboard uses a guitar string app to measure belt tension. https://www.youtube.com/watch?v=on_L6wAo5yA
```

---
## \#11 Posted by: lowGuido Posted at: 2015-11-04T07:39:07.198Z Reads: 358

```
What are peoples thoughts on idler pulleys to tension belts?
I have always left it because its more effort than just moving the motor. 

But I can see benefits in meshing more teeth..
```

---
## \#12 Posted by: onloop Posted at: 2015-11-04T10:19:40.642Z Reads: 354

```
i think idler belts will be a huge benefit... i just haven't spent much time working out exactly how to integrate that into my mounts.

More teeth in mesh is always better... can use much smaller motor pulleys and achieve greater reduction... this could help with efficiency as you could have the motor spinning at higher RPM - around the 8500 mark.
```

---
## \#13 Posted by: psychotiller Posted at: 2015-11-04T12:39:28.915Z Reads: 348

```
Read this build thread.  I made one for a couple of builds. I called it a tensioner, but it's doing the idler job as well. And works amazingly.
https://endless-sphere.com/forums/viewtopic.php?f=35&t=59259
```

---
## \#14 Posted by: lilracerboi Posted at: 2015-11-05T01:52:17.517Z Reads: 341

```
Can anyone show a visual representation, if possible, of how much tension you have? This is what my board looks like.
Just before I took the photos, I loosened the belt a bit from what it was at previously. Not sure if this helps.

<img src="/uploads/db1493/original/1X/b00e3f19fbe2469ee5de8aa8a2beed5e7d0d2651.jpg" width="666" height="500">

<img src="/uploads/db1493/original/1X/6e6070660f06f743b2250ad7f454dd16864805d8.jpg" width="666" height="500">

<img src="/uploads/db1493/original/1X/a0855cf5ea58c4e0930bbeacd9c0d9a021534511.jpg" width="666" height="500">

<img src="/uploads/db1493/original/1X/a3f25464c94b35a7844e3c9df79c38f8192f527a.jpg" width="666" height="500">

I also have a video of me turning the wheel with the same amount of tension. Not sure if you can hear the noise.
https://youtu.be/zriBHWoRFao
```

---
## \#15 Posted by: onloop Posted at: 2015-11-05T02:15:00.664Z Reads: 319

```
Apart from the obvious "mechanical" reasons of belts wearing out due to bad alignment OR being too tight/loose.

There can also be "electro-mechanical" reasons for the belt to wear out prematurely that are related to the ESC? What ESC are you using? 

There are two ways the belt can be damaged by the ESC.

1. Acceleration Curve, If the ESC tries to accelerate the motor faster than what the torque load rating of the belt can handle the belt will skip. Load on the belt decreases as momentum increases. If you try to spin up too fast, before load has the chance to decrease you could exceed the torque rating of the belt. You will know because the belt will be skipping teeth during starting. 

2. Brake force progressiveness, If the ESC brake is very abrupt and comes on really strong & early the same problem happens. The momentum load is too great for the belt to slow you down without skipping...

both these things will damage a belt quickly.

If you are a heavy guy 90+kg you might need two motors! this will double the torque load rating of your drive train. You can also modify your throttle control technique to try and become smoother.

You may also consider upgrading to a wider belt, ill have a 12mm wide belt system available soon that is designed for single drive boards that need to have better performance.

Also, you might consider going a larger motor pulley to increase the "teeth in-mesh" the more teeth in mesh the greater the torque load transfer.
```

---
## \#16 Posted by: lilracerboi Posted at: 2015-11-05T03:40:18.212Z Reads: 301

```
I weigh roughly 180lb. (~81kg) and I'm using the Hobbywing EZ Run 150amp ESC. I also use the Wiiceiver by Austin David.

I also noticed the acceleration curve, so I usually kick off pretty good, then gradually increase speed. It takes me a bit of time to get up to speed, but I don't really mind it.

With the brakes, I know the Wiiceiver abruptly breaks at whatever position I put it in, but whenever I need to stop I plan ahead and just coast, then use the brakes when needed by going down on the joystick very slowly so that it doesn't stutter.

That 12mm wide belt system sounds very promising, though since I just got my board finished, I don't have money to spend on upgrades in the near future. 

What amount of teeth in the pulley is enough? My pulley has 40 teeth on it.
```

---
## \#17 Posted by: onloop Posted at: 2015-11-05T04:30:37.881Z Reads: 287

```
What pulley has 40 teeth? i assume you mean the wheel pulley?
```

---
## \#18 Posted by: treenutter Posted at: 2015-11-05T14:15:57.443Z Reads: 289

```
@csn I really like metroboard's mount design; a single screw to tension the belt would take a lot of the guesswork out of it!
```

---
## \#19 Posted by: psychotiller Posted at: 2015-11-05T14:39:57.084Z Reads: 293

```
if you read their feedback you'll see some complaints. People still have the same issue with the addition of bending braking the tool
```

---
## \#20 Posted by: lilracerboi Posted at: 2015-11-05T21:41:42.580Z Reads: 284

```
Oh shoot, I didn't read correctly. That was the wheel pulley I was referring to. I have a 14 tooth motor pulley.
```

---
## \#21 Posted by: onloop Posted at: 2015-11-05T22:08:43.016Z Reads: 276

```
Does your wheel pulley have 40 Teeth? If its one of my kits it is 36T, this is important because the larger the diameter of the wheel pulley the less teeth in mesh unless you increase center distance.
```

---
## \#22 Posted by: lilracerboi Posted at: 2015-11-05T22:15:59.802Z Reads: 263

```
Yes, my wheel pulley has 40 teeth. Should I get a 36 teeth pulley?
```

---
## \#23 Posted by: onloop Posted at: 2015-11-05T23:24:43.983Z Reads: 264

```
a-ha! now we are getting to the bottom of this!

if you are interested to learn more about this please read;

http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53
```

---
## \#24 Posted by: onloop Posted at: 2015-11-05T23:34:20.221Z Reads: 254

```
if you keep the 40t wheel pulley you need a 16t motor pulley.
```

---
## \#25 Posted by: lilracerboi Posted at: 2015-11-06T03:32:25.117Z Reads: 251

```
Okay....I noticed something and I needed to confirm it. I just went back and counted the teeth on my wheel pulley and it's 36 teeth, not 40. I don't know where I got 40 from. Motor pulley is 14 teeth.
```

---
## \#26 Posted by: longhairedboy Posted at: 2015-11-06T15:09:32.221Z Reads: 249

```
14/36 is what i'm running too. Have you triple checked for wheel pulley wobble? I had this one situation where I couldn't figure out why my belts were wearing oddly then breaking. Every time i flipped it over and slowly turned the wheels everything looked like it was lining up perfectly. Turned out my wheel pulley wasn't exactly centered and flat with the wheel and i wasn't able to see it until i was looking for it while running the motors flat out on the bench.
```

---
## \#27 Posted by: lilracerboi Posted at: 2015-11-06T22:52:46.839Z Reads: 245

```
I think that may be my issue. I've look at it a dozen times and I can't seem to get it right.

Just now though, I loosened the belt a lot then spun the wheel and it still makes the creaking noise. No matter what tension I have right now, it'll make that noise.

Also note, I did rotate the wheels around recently, so it;ll be a bit different than a couple weeks ago.
```

---
## \#28 Posted by: lowGuido Posted at: 2015-11-06T23:10:19.541Z Reads: 239

```
@psychotiller yeah actually I have seen your thread on ES with the bearing tensioner. how did you mount it?
```

---
## \#29 Posted by: psychotiller Posted at: 2015-11-07T01:36:44.003Z Reads: 244

```
I drilled and tapped an 8mm hole in my mount. Then it was just a matter if putting a screw through the bearings.
```

---
## \#30 Posted by: lowGuido Posted at: 2015-12-19T11:02:54.676Z Reads: 240

```
well I just finished my belt tension idler pulley.
Its pretty simple, just like you described @psychotiller. I drilled a 8mm hole and put a bolt with a bearing on it.
My theory is that it will force more teeth in mesh on the small pulley.
the traditional method of tension by moving the  2 pulleys apart doesn't give optimal amount of teeth in mesh on the small pulley. sure making the pulley bigger will give you more teeth in mesh, but then you lose your gear reduction, and acceleration/torque/hill climbing etc..

<img src="/uploads/db1493/original/2X/9/98e8ea84ba5f7170f28b30fd384cde482deed888.JPG" width="307" height="316">
inserting an idler in the middle of the 2 pulleys should help more teeth mesh in the smaller pulley.

I'll give it a test ride and give some feedback tomorrow.
```

---
## \#31 Posted by: trbt555 Posted at: 2015-12-19T13:54:48.640Z Reads: 226

```
This makes a lot of sense. I'm looking forward to your feedback.
Please post pictures too.
I put this on my todo list.
```

---
## \#32 Posted by: psychotiller Posted at: 2015-12-19T15:46:05.917Z Reads: 227

```
Nice! You should find that you lost the skip entirely. Also, since you now don't have to tension the crap out of your belt your board will roll easier.
```

---
## \#33 Posted by: lowGuido Posted at: 2015-12-19T21:13:18.513Z Reads: 228

```
Wow what a ride!  Acceleration is improved.  Braking is improved. Hill climbing is improved. Under all normal riding belit slip is eliminated. 
And it seems to be quieter as well.
I tried to make it slip by accelerating hard up a hill and i did manage to make it slip a little. But i had to really try to make it slip. And this in on a well worn belt as well.
I will be making this simple mod to all my mounts now.
<img src="/uploads/db1493/original/2X/9/9c27515d81385703aed54790900f87845d48899c.jpg" width="690" height="388">
```

---
## \#34 Posted by: kai Posted at: 2015-12-19T22:08:24.747Z Reads: 220

```
Cool man. Is it a slot so you can adjust it?
```

---
## \#35 Posted by: lowGuido Posted at: 2015-12-20T10:16:04.882Z Reads: 221

```
no the idler itself isn't slotted but the motor slides in and out in the traditional manner, so you adjust the tension that way.
```

---
## \#36 Posted by: Iceni Posted at: 2015-12-20T12:40:36.445Z Reads: 221

```
Simple and effective, the way it should be.
Might be something to keep in mind for the future if needed.
```

---

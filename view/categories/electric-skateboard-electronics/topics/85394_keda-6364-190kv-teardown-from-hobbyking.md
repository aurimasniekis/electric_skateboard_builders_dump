# KEDA 6364 190kV Teardown (from Hobbyking)

### Replies: 38 Views: 1313

## \#1 Posted by: Shaun Posted at: 2019-02-25T20:34:55.009Z Reads: 291

```
So I’ve ordered a couple of these motors from Hobbyking for my first DIY build and thought I would open one up to have a look inside. Build quality doesn’t appear too bad to be honest. There’s loads of room inside the casing so I will be installing hall sensors and some longer flexible wires. Stator is 30mm in length, 52mm OD. NDE stator bearing feels a bit notchy so will change the bearings for SKF. I can’t separate the stator from DE casing so will need to stick it in the press sometime this week.![image|375x500](upload://u3PxGlHFvaJWWLbj4NxUnMOTNpA.jpeg) ![image|375x500](upload://dpeVu2p1syLTfr1xJQDz0zGprMH.jpeg) ![image|375x500](upload://5P8JYum58H1IFFXQH3KYNAEim4p.jpeg) ![image|375x500](upload://8uDbN5JiK93RWY1tX9QqtvhC1wg.jpeg) ![image|375x500](upload://qvvPQed7J7NzS0zTcKMxntzSlLx.jpeg) ![image|375x500](upload://gfVLD7mwiExqCSlZZGZcyCkyK68.jpeg) ![image|375x500](upload://48UouHZLVEwKVIC6Itunp9WrnlN.jpeg)
```

---
## \#2 Posted by: PatRocks Posted at: 2019-02-25T20:57:50.022Z Reads: 270

```
Interesting that there's no space between the magnets 🤔, i guess I assumed that was a requirement... hch bearings are amazing for the price, i have them in all my motors as replacements

Also, how you plan to strip the phase leads?
```

---
## \#3 Posted by: Shaun Posted at: 2019-02-25T21:16:50.701Z Reads: 257

```
Cool, I will take a look at those bearings.

I need to press the front casing out of the stator first so I can get to them and then slice the cable sheath and peel it off.
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-02-25T22:06:55.472Z Reads: 237

```
Great thread. I have a pair of these and have ordered a couple of sensor boards...what great timing

Please keep sharing the excellent pics and details. I don’t think I’m brave enough to try anything but an aspirin to strip the enamel
```

---
## \#5 Posted by: PatRocks Posted at: 2019-02-25T22:18:39.514Z Reads: 224

```
Those phase leads are likely laminated wire, is what I meant. You probably know that already though lol. Major pain in the ass to strip
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-02-25T22:23:08.587Z Reads: 215

```
Lye’r!

10 chars
```

---
## \#7 Posted by: PatRocks Posted at: 2019-02-25T22:23:56.915Z Reads: 205

```
Lol, it's like you've known me my whole life
```

---
## \#8 Posted by: Grozniy Posted at: 2019-02-25T22:44:27.345Z Reads: 196

```
I changed the wires to silicone ones and to remove the coating, I just heated them with 100w soldering iron
```

---
## \#9 Posted by: Shaun Posted at: 2019-02-25T23:04:39.708Z Reads: 185

```
Will do. What sensor boards have you ordered?
```

---
## \#10 Posted by: Shaun Posted at: 2019-02-25T23:09:25.222Z Reads: 187

```
I’ll be trying the heat and Stanley blade trick first. If that fails (or I loose my patience with them) we’ve got a motor rewind shop at work so they will be getting it as a priority job, ha!
```

---
## \#11 Posted by: Shaun Posted at: 2019-02-25T23:10:31.299Z Reads: 186

```
Did you press the stator off the casing or do it in situ?
```

---
## \#12 Posted by: leroy Posted at: 2019-02-25T23:11:50.206Z Reads: 183

```
I bought one of these about six months ago from hobbyking for $21. 
I use it on a board with a hobbywing 150amp 6s esc and  a 6s4p  battery pack, 
and I love it.
```

---
## \#13 Posted by: Grozniy Posted at: 2019-02-25T23:17:15.538Z Reads: 173

```
I didn't open the motor, I just cut the leads as close to the can as possible and soldered silicone ones
```

---
## \#14 Posted by: PatRocks Posted at: 2019-02-25T23:26:59.575Z Reads: 172

```
That's pretty convenient @Shaun !!
The problem with the burning off insulation is the thermal conductivity of the copper. As in, if it burns off the leads, it may burn off the windings too!! That's what I was worried about when I resorted to the "do not attempt " method. Worked for you though @Grozniy ?
```

---
## \#15 Posted by: Grozniy Posted at: 2019-02-25T23:28:04.977Z Reads: 166

```
Worked no problems
```

---
## \#16 Posted by: banjaxxed Posted at: 2019-02-26T08:21:08.226Z Reads: 161

```
these ones
https://alienpowersystem.com/shop/brushless-motors/50mm/internal-pcb-with-hall-effect-sensors-120-degree/
```

---
## \#17 Posted by: Shaun Posted at: 2019-02-26T09:20:13.551Z Reads: 159

```
Thanks. I did see them actually and it appears Alien are the only company that make this design. Which end of the motor did you fit it to and how did you mount it?
```

---
## \#18 Posted by: banjaxxed Posted at: 2019-02-26T10:59:46.857Z Reads: 165

```
they are in the post still
```

---
## \#19 Posted by: Tinp123 Posted at: 2019-02-27T07:08:33.659Z Reads: 160

```
you can make your own sensors under 3$ 
you don't even need pcb
I wired my own sensors yesterday, hall sensor test passed from first try. on bench, motor spins really nice and smooth from start. today, I will test it on street. here is wiring diagram:
![LARGE|690x364](upload://ntMdD2aedSTBNj71DcX73R3VXIM.jpeg) 
just wire them like shown here, but put them between stator poles, 120 degrees apart, just like on APS pcb.

you will need:
-sensors- https://www.aliexpress.com/item/5pcs-lot-SS441A-41A-member-Unipolar-Hall-Switch-Sensor-new-original-In-Stock/32925711838.html?spm=a2g0s.12269583.0.0.58366591jph5uA
-5 or 6 pin jst connector (depends which vesc you use)
-some wires
-soldering iron
-hot glue

![IMG_20190226_205802|375x500](upload://hayFawQWBChuezEFngszbN3nkZ8.jpeg)
```

---
## \#20 Posted by: Shaun Posted at: 2019-02-27T08:38:21.558Z Reads: 150

```
Ideal, thanks for the info.
```

---
## \#21 Posted by: spork Posted at: 2019-05-28T02:19:19.481Z Reads: 129

```
>> I can’t separate the stator from DE casing so will need to stick it in the press sometime this week.

I've got a couple of these on my off-road board.  They've been working great until a few days ago.  One of them has an intermittent short when I move the leads around.  I'd like to get in there and fix it properly.  Were you able to press the stator off the casing?
```

---
## \#22 Posted by: Shaun Posted at: 2019-05-29T15:51:38.416Z Reads: 118

```
Yes, removed the grub screws and pressed it out.
```

---
## \#23 Posted by: spork Posted at: 2019-05-30T07:05:44.436Z Reads: 110

```
Thanks for the response.  But I'm not sure if we're talking about the same thing.  I was able to remove two grub screws and remove the can with the magnets in it (part C), but I can't figure out how to separate the stator (part A) from the front of the case (part B).  It looks like the stator is pressed onto a center hub/cylinder that's part of the case-front, and probably bonded.  But I don't see any grub screws that would be holding it in place.  Can you confirm that you were able to separate A and B?

Thanks.

![IMG_20190529_235434088|690x495](upload://davZTIrkYecfVEoRmf43QpfN34Y.jpeg)
```

---
## \#24 Posted by: Superflim Posted at: 2019-05-30T07:23:26.971Z Reads: 102

```
I tried to tear down some other motor and those parts A and B were epoxied together. I think might be the case here too. Maybe try to a heat gun?
```

---
## \#25 Posted by: spork Posted at: 2019-05-30T07:25:53.731Z Reads: 100

```
Thanks Superflim.  I could put it in an arbor press - if I can figure out a good way to hold it by the stator.  I could also use heat if necessary.  But I figured it would be great to hear from someone that's done it.
```

---
## \#26 Posted by: spork Posted at: 2019-06-02T23:11:33.064Z Reads: 80

```
I made a wooden fixture to hold the stator and heated it with my hot air rework station at 480-F.  Tried pressing it out on my drill press.  No luck yet. :frowning:
```

---
## \#27 Posted by: spork Posted at: 2019-06-03T23:54:48.909Z Reads: 73

```
I gave up on trying to remove the stator, but instead managed to get in there very carefully with a dental pick and separated the leads from the coils where they were shorting.  I got some epoxy in there to keep them separated.  I then used hot-melt where the leads exit the case so that external motion of the leads can't cause further fatigue or abrasion.

I was nervous from the start about the lack of strain relief, but I decided to ignore it.  Now I know better.  I've got both motors strain-relieved with hot-melt glue, and I'll be replacing the leads downstream with the much more supple silicone wire.  I think I would highly recommend the same to others using these motors.
```

---
## \#28 Posted by: Shaun Posted at: 2019-06-04T17:47:19.311Z Reads: 60

```
Fitted some hall sensors and temp sensors to mine last night. Just need to finish the wiring and give them a go. ![image|375x500](upload://xkjyLBJDtNndO4L7VLYxleM7GQl.jpeg) ![image|375x500](upload://lnBp2fYH0XJtYXR3oAV82sA33OZ.jpeg) ![image|375x500](upload://uaxw7IuKBV0YhZpO6SO6pOzAenz.jpeg)
```

---
## \#29 Posted by: Tinp123 Posted at: 2019-06-04T18:22:26.653Z Reads: 56

```
Looks much cleaner then mine! :ok_hand::ok_hand::ok_hand:

Let us know if they work!
```

---
## \#30 Posted by: Shaun Posted at: 2019-06-04T18:26:36.429Z Reads: 56

```
Yeah, will do. It was quite hard to get them in there neatly. Some of the windings on mine are pretty shabby to be honest. Did you put yours 120 degrees out from each other? I also dropped one of mine and damaged one of the windings. Going to give it a zap with the insulation tester later.
```

---
## \#31 Posted by: Shaun Posted at: 2019-06-04T18:28:13.641Z Reads: 57

```
Ignore last comment. I forgot you mentioned it above 🙈😂
```

---
## \#32 Posted by: Tinp123 Posted at: 2019-06-04T18:41:27.666Z Reads: 57

```
Haha no problem! Yeah I installed them on the beginning of this hole between poles. I didn't go so deep, I thought there is not enough space
```

---
## \#33 Posted by: banjaxxed Posted at: 2019-06-04T19:13:09.833Z Reads: 57

```
Probably press fitted on as well as expoxied, dunno never separated those two bits @Riako @Andy87 you guys tried? Curious
```

---
## \#34 Posted by: Riako Posted at: 2019-06-04T21:41:43.773Z Reads: 48

```
Yes press fit on the APS I have open once... it was not easy ^^
```

---
## \#35 Posted by: banjaxxed Posted at: 2019-06-04T21:43:08.421Z Reads: 49

```
Maybe putting it in a freezer bag and in the freezer followed by the heat gun/hot air on the outer part would help
```

---
## \#36 Posted by: spork Posted at: 2019-06-05T02:31:47.616Z Reads: 48

```
[quote="Shaun, post:30, topic:85394"]
Going to give it a zap with the insulation tester later.
[/quote]

Interesting.  What's an insulation tester?

Also, what sensors did you use.  I used SS41F's and it was a very tight fit.  I had to file the sides of the sensors down until I hit metal.  After wedging them in between the stators (at 120 deg) I used hot-melt to hold them in place.  They've been working great.
```

---
## \#37 Posted by: Shaun Posted at: 2019-06-05T21:40:31.891Z Reads: 43

```
Finished the wiring tonight.![image|375x500](upload://fUaDQc8FOqivzOqqx24VmNCquyX.jpeg) ![image|375x500](upload://1NDDbO0JLwrhI3ltrpI95dThtnl.jpeg)
```

---
## \#38 Posted by: Shaun Posted at: 2019-06-18T21:32:20.255Z Reads: 31

```
First test was a success. Hall and temp sensors working well. Now to sort an enclosure!![image|548x499](upload://erFxZKGtGno5e1XQch8bCLrOMiK.jpeg)
```

---

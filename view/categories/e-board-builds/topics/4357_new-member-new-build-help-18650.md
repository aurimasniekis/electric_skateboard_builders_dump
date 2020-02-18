# New member, new build help (18650)

### Replies: 36 Views: 2718

## \#1 Posted by: Pablo_702 Posted at: 2016-06-06T18:12:50.588Z Reads: 185

```
hi guys im trying to put an electric skateboard together, and im getting ready to start ordering parts but before i do that i have a few questions
1. im 200 lbs and i was wondering if 1 single SK3 -6364-245kv will be enough to push me and a 36inch long board to 20mph?

2.if that single motor doesnt, using 2 motors means 2 vesc???

3. and 3rd and last one (for now) i own a Vape Shop and i have acces to a lot of different 18650 batteries
the ones i use for my vapes are 3.7V 30A 3000mAh, how many of them and how would i have to use them (series, parallel) in order to get a range of 20 miles
```

---
## \#2 Posted by: Rob.Endless Posted at: 2016-06-06T18:23:55.567Z Reads: 179

```
I vape and use green samsung 25r's, i've seen people here use those in their packs with good results.
```

---
## \#3 Posted by: treenutter Posted at: 2016-06-06T18:29:14.998Z Reads: 175

```
Welcome @Pablo_702 !

[quote="Pablo_702, post:1, topic:4357"]
1. im 200 lbs and i was wondering if 1 single SK3 -6364-245kv will be enough to push me and a 36inch long board to 20mph?
[/quote]

Probably yes, the top speed depends on your gearing, wheel size, and riding conditions. I don't recommend aiming for a high top speed. Instead focus on good torque and quality components. If you get anywhere near this speed you should wear full protective gear including a helmet,  pads and maybe leathers. 

[quote="Pablo_702, post:1, topic:4357"]
if that single motor doesnt, using 2 motors means 2 vesc???
[/quote]
-yes, 2 motors means you need 2 ESCs, or VESCs.

[quote="Pablo_702, post:1, topic:4357"]
how many of them and how would i have to use them (series, parallel) in order to get a range of 20 miles
[/quote]
-Read through some of the battery build threads on this forum, search for 18650, 10s3p or 10s4p. You'd need between 30-40 to get that kind of range. That said, 20 mile range is somewhat impractical since you'll likely exhaust your body before you can comfortably skate 20 miles :slight_smile:
```

---
## \#4 Posted by: Jinra Posted at: 2016-06-06T18:30:01.142Z Reads: 150

```
You have to make sure the discharge rate can handle what the motor and ESC draw. A good target is 50A continuous total. A single 6364 should be able to get you around, though it may have some trouble up steeper hills, especially at 245kv. You may want to go sub 200kv (@10s) to get additional torque. Two motors does mean 2 ESC/VESCs and should help a lot with torque, though you'll probably still want to go a bit lower than 245kv. Hitting 20mph should be no problem given adequate voltage and gearing.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-06-06T18:31:51.839Z Reads: 143

```
Noticed your 702 ...you wouldn't be in Vegas would you?
```

---
## \#6 Posted by: Ulfberht Posted at: 2016-06-06T18:39:04.427Z Reads: 138

```
@Rob.Endless is right. The most common battery used right now is the Samsung 25R 18650. It has an internal fuse and a pressure vent, just in case. The gold standard.right now. You should check out some of the build threads. Search "18650" and check it out. 
Single motor could be fine, but you have to think about the gearing that you will be using as well as the terrain you will be using it on. Also, 2 motors will need 2 ESC or VESC. On the ESK8 calculator you can get a decent idea of how your build specs out. 
Here's the ESK8 calculator that everyone loves. 
http://toddy616.blogspot.de/2013/07/electric-skateboard-calculator.html
```

---
## \#7 Posted by: delta_19 Posted at: 2016-06-06T18:40:27.716Z Reads: 135

```
What are you using that gets 3000mah and 30A
```

---
## \#8 Posted by: Jinra Posted at: 2016-06-06T18:40:54.926Z Reads: 132

```
I don't think he was talking about discharge rate, just saying 3000mah = 30A
```

---
## \#9 Posted by: delta_19 Posted at: 2016-06-06T18:41:39.466Z Reads: 125

```
But 3000mah=3A
```

---
## \#10 Posted by: Jinra Posted at: 2016-06-06T18:41:55.579Z Reads: 122

```
derp you're right, perhaps typo then?
```

---
## \#11 Posted by: lox897 Posted at: 2016-06-06T20:26:02.415Z Reads: 117

```
@delta_19 @Jinra It is probably a Sony VTC cell.
```

---
## \#12 Posted by: delta_19 Posted at: 2016-06-06T20:30:19.038Z Reads: 118

```
vtc5 cells are only 2600mah
```

---
## \#13 Posted by: lox897 Posted at: 2016-06-06T20:32:32.290Z Reads: 117

```
I saw a samsung cell with 30amp discharge the other day. Could it be that? EDIT: Looks like it could be. It is called the ICR18650-30A and it has 3ah.
```

---
## \#14 Posted by: c4Lvin Posted at: 2016-06-06T20:34:29.715Z Reads: 114

```
I don't mean to interrupt, but how is that Continuous 30-50A discharge calculated in a pack such as the Space Cell's (10S3P) design? I don't even want to get into C-ratings and all that as it's more than my old brain can handle at the moment :(
```

---
## \#15 Posted by: lox897 Posted at: 2016-06-06T20:36:08.679Z Reads: 119

```
Each cell has 20amp continuous discharge and it is 3p which is 3 in parallel. 3x20amp = 60amp continuous. But I think they have a 50amp fuse so you can't go above 50 amps which is kind of stupid since the cells can easily handle 60amp continuous.
```

---
## \#16 Posted by: delta_19 Posted at: 2016-06-06T20:37:56.523Z Reads: 113

```
a lot of cells get warm at their max and will die faster if they are discharged at max current all the time. thats why people will at most run a battery at 75% of its max current. it doesnt get as hot and can last longer.
```

---
## \#17 Posted by: Jinra Posted at: 2016-06-06T20:38:16.360Z Reads: 113

```
40A fuse actually. Fuses don't actually blow at their rated ampere. It would have to exceed it for an amount of time to blow.

Also, the VESC is designed for 50a continuous, probably best to work before that for longevity
```

---
## \#18 Posted by: lox897 Posted at: 2016-06-06T20:39:29.954Z Reads: 113

```
I learnt something new. Thanks for the additions guys.
```

---
## \#19 Posted by: c4Lvin Posted at: 2016-06-06T20:43:52.709Z Reads: 110

```
my Space Cell has a 30A fuse. Can I just swap it out for a 40-50A fuse? It's just running a R-Spec 6355 at the moment but eventually I will run dual VESC and R-Spec 6355 motors. I have yet to blow the 30A fuse so just wondering. I have some LGABD or DBD pink 3000mAH cells, do you think it can handle my current single setup or even the dual? I don't have any other specs on those cells but they all have about 90-100% of their capacity. I'm also planning on doing my first 18650 cheap cell pack if those cells can handle my load. I'm 170lb rider and my first e-board.
```

---
## \#20 Posted by: Randyc1 Posted at: 2016-06-06T20:44:20.930Z Reads: 108

```
For a single maybe be better off with a 6374 192 kv and a 10s4p.
```

---
## \#21 Posted by: c4Lvin Posted at: 2016-06-06T20:46:57.693Z Reads: 98

```
I hear ya Randyc1 but I don't prefer another 10cells if I'm not going to ride for 20miles like others stated, I get tired quite easily. So 10S3P is good for me now unless I get heavier of course! My board came with the 6355 preinstalled and I was already extremely impressed with it's torque and high speed (no gear yet). It felt like the first time I rode my YZF-R1!
```

---
## \#22 Posted by: Maxid Posted at: 2016-06-06T20:51:25.704Z Reads: 98

```
[quote="lox897, post:13, topic:4357, full:true"]
ICR18650-30A and it has 3ah.
[/quote]
At first I thought the same thing but that name is pretty misleading. The ICR only has a max discharge rate of 6A according to the [data sheet](http://www.meircell.co.il/files/Samsung%20ICR18650-30A.pdf)
```

---
## \#23 Posted by: Jinra Posted at: 2016-06-06T21:02:55.992Z Reads: 92

```
keep the 30a fuse and bring spares as needed 40a/50a should be okay.

I looked up the LGBAD11865 (which I'm assuming is the one you have) and it has a 1.5A discharge rate.. Definitely won't work for eskate.
```

---
## \#24 Posted by: lox897 Posted at: 2016-06-06T21:06:24.310Z Reads: 89

```
I think you are right. What cell are you talking about then @Pablo_702 ?
```

---
## \#25 Posted by: c4Lvin Posted at: 2016-06-06T21:52:12.974Z Reads: 84

```
1.4A???  What the heck? How could it be so low?  So the assembled pack would be 5.2A ? I think I got burned.
```

---
## \#26 Posted by: Jinra Posted at: 2016-06-06T21:53:42.470Z Reads: 87

```
It's according to this site http://www.enova18650.com/lg-lgabd11865-3000mah-flat#.V1XwuZErIvg I'm not sure if it's reliable, but if it's true, it won't be suitable.

.5C * 3A = 1.5A discharge
```

---
## \#28 Posted by: Pablo_702 Posted at: 2016-06-07T01:59:33.951Z Reads: 74

```
Yes sir i am from vegas, are you from here too?
```

---
## \#29 Posted by: Michaelinvegas Posted at: 2016-06-07T02:00:28.028Z Reads: 80

```
<img src="/uploads/db1493/original/2X/b/bada37255ee9c8b15c930b05e7d72a7b295ed038.jpeg" width="511" height="500">



Yeah pretty close to you
```

---
## \#30 Posted by: Pablo_702 Posted at: 2016-06-07T02:11:17.642Z Reads: 78

```
I dont know how to upload pics to this forum im from my phone but right now im running brillipower IMR18650 3100mAh max 40A
```

---
## \#31 Posted by: delta_19 Posted at: 2016-06-07T02:17:10.241Z Reads: 77

```
[quote="Pablo_702, post:30, topic:4357"]
brillipower IMR18650 3100mAh max 40A
[/quote]

https://www.e-cigarette-forum.com/forum/threads/brillipower-40a-3100mah-18650-bench-test-results-only-a-15a-3000mah-battery.702075/#post-16538400

toss it, its shite.
```

---
## \#32 Posted by: Pablo_702 Posted at: 2016-06-07T02:19:48.696Z Reads: 72

```
Thats what i have right niw at this momento in my mod but like i said i have acces to mxjo, brillipowers,lg , panasonic, samsung, sony
```

---
## \#33 Posted by: Pablo_702 Posted at: 2016-06-07T02:24:33.319Z Reads: 74

```
Ok im not giving up i hhave to admit theres a lot more that what i thought at first, but i have to start somewhere and i dont want to realize down the road that my motor is not powerfull enough or upgrade other parts so ill start by buying the deck and the motor, considering what i weight and what i want 20 mph max, whats the best motor i can buy links plssssss, also i forgot to mention that im going yo have this 1 motor working on both rear wheels but i wont bother on that i have that all figured out already
```

---
## \#34 Posted by: Michaelinvegas Posted at: 2016-06-07T02:28:35.046Z Reads: 73

```
Take a look at this Sir @evoheyax busted his butt to make this... And he's working on a data base of some sort 

 http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas
```

---
## \#35 Posted by: Pablo_702 Posted at: 2016-06-07T04:57:51.958Z Reads: 76

```
thats a lot of work @evoheyax thanks for all the time you took to put this list together, that means lets go back to drawing hahahahaha, @Michaelinvegas thank you for your help too
```

---
## \#36 Posted by: Michaelinvegas Posted at: 2016-06-07T05:04:06.896Z Reads: 78

```
Yeah man take ur time if u can..take a read on the fourm...there probably isn't a question you can ask that hasn't been already answered...but if u need help just hit us up
```

---
## \#37 Posted by: Northlake Posted at: 2017-03-29T02:16:24.699Z Reads: 35

```
I'd recommend going with the sk3 190kv motor for the same price or even lower kv at 145kv or something. the lower kv motor the more torque it has and less top speed. the 245kv motor will make your motor work too hard going up hills at 200 lbs. i weigh 190 and i find the 190kv great even with a single motor.
```

---

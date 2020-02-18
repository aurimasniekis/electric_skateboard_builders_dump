# Dual Drive E-board with Single Motor

### Replies: 34 Views: 8901

## \#1 Posted by: emotiva Posted at: 2015-11-01T03:56:40.573Z Reads: 480

```
@onloop, Def good idea for build titles. 

I mocked up another nylon bracket and an axle to enable dual wheel drive with a single motor. I've got two sk3s and might end mounting both, but wanted to play with this idea. I'll see how it performs first, anyway. 

<img src="/uploads/db1493/original/1X/b608f22cf79c84705c56362ab826b8a48cb70c6e.png" width="690" height="388"> 
<img src="/uploads/db1493/original/1X/3893f8411f918d1429db566eb54729b7bde2606b.jpg" width="690" height="388">

I've bored out the axle bracket to fit a 608 bearing, and used 5/16" zinc coated steel rod for the axle (no aluminum in 5/16"). I thought I was going to have to order some 8mm rod, but the 5/16" fits the bearing with no slop. The difference in the two nominal sizes is only 2.5 thousandths after all, though I don't know what the tolerances are on these pieces. 

On the motor side, I cut the bolt end off of the included aluminum coupler, then bored it out and threaded it with an M8 tap. I also threaded the axle to fit. I intend to machine a longer coupler in the end so I can get more axle in there / maybe a lock nut on both sides. 

Like I said before, I'll make some changes to the final mounts. I want to include a bash plate of some sort among other things. Now just have to order some aluminum and pulleys and wait for the electronics to arrive. Wish I'd just ordered the existing pulley non-anodized. Ah well, maybe I'll replace it when I buy the second one.
```

---
## \#2 Posted by: lowGuido Posted at: 2015-11-01T04:11:09.145Z Reads: 453

```
I don't want to burst your bubble but that dual wheel drive wont work.
see our discussion about differentials here:
http://www.electric-skateboard.builders/t/dual-drive-vs-diagonal-drive/85/17
```

---
## \#3 Posted by: psychotiller Posted at: 2015-11-01T04:14:08.146Z Reads: 437

```
I'm definitely curious to see what's going to happen. Pneumatic may be the straw that causes the chatter and skipping.
```

---
## \#4 Posted by: lowGuido Posted at: 2015-11-01T04:23:27.625Z Reads: 423

```
my prediction is broken belts...
```

---
## \#5 Posted by: emotiva Posted at: 2015-11-01T04:24:14.200Z Reads: 417

```
@lowGuido, of course, thanks. I have actually read that thread and just forgot about the issue entirely while playing with things today :neutral_face: . Hmm. at this point, I might continue on just to witness what the failure point is (belt slip, I'd guess) and how severe.
```

---
## \#6 Posted by: psychotiller Posted at: 2015-11-01T04:29:11.901Z Reads: 416

```
You'll be the first to actually do it. We've definitely written and read a lot of theory. Let's see it in action! You're already there anyway right?
```

---
## \#7 Posted by: lowGuido Posted at: 2015-11-01T04:59:40.229Z Reads: 413

```
yeah do it for science.

I have always had this theory that when RedRock designed their La Grange truck they had intended 2 wheel drive, and then after the production run realised it wouldn't work so they replaced one side with bearings..
<img src='/uploads/db1493/original/1X/41eefb56d700e52a0b55457e3fa62dd3a0519ebd.jpg'>
```

---
## \#8 Posted by: cmatson Posted at: 2015-11-01T05:00:07.509Z Reads: 405

```
[quote="psychotiller, post:30, topic:356"]
We've definitely written and read a lot of theory. Let's see it in action!
[/quote]

yes, this should be interesting!

my guess is that because of the pneumatics (high amount of hookup/traction) it will cause some differential problems...

if it were normal skate wheels, I'd say that there would be enough room for one wheel to go slightly faster (the truck isn't that wide, so the difference in speed when turning should be small anyways) and you wouldn't see much of a difference; unless it was on a crazy smooth road with a low durometer wheel...
```

---
## \#9 Posted by: psychotiller Posted at: 2015-11-01T05:18:47.691Z Reads: 400

```
My thoughts EXACTLY! As far as the LaGrange L1 truck, it was designed around a floating axle merely because that was the easiest way to allow any wheel to be used. Because they made a "glue in" hub that had no bearing, the easiest solution was to secure the hub to a floating axle.
```

---
## \#10 Posted by: onloop Posted at: 2015-11-02T00:11:34.639Z Reads: 381

```
i've been thinking about this alot lately....  also now i have the 6372 R-SPEC i was probably going to try just for fun...

you cannot ignore the huge savings this setup offers. 1. minus one motor cost. 2.minus one vesc cost! BUT you still have the braking force of a dual setup and better handling without torque steering. these are some legitimate reasons to at least test this configuration.

However i think you need some kind of **coupling** to minimize the differential and reduce the force on the belt.

My gut feeling is that with pneumatics they might not want to slip on the ground as much as a urethane wheel would, so you might have *more* problems.

I was going to install something like this, I'm thinking this will allow for some slight variations in rotation.

it's a torque coupling, design to stop things breaking when motors spin up, i also think it might help reduce stress on the belts

<img src='/uploads/db1493/original/1X/8e54cdecca008c47ff095aa9f8fd3afb058553d3.jpg'>
```

---
## \#11 Posted by: psychotiller Posted at: 2015-11-02T00:23:22.409Z Reads: 362

```
That'll probably work!!! It's going to be make or break with pneumatic. I cant wait to see the results.
```

---
## \#12 Posted by: emotiva Posted at: 2015-11-02T03:18:00.294Z Reads: 361

```
Definitely worth thinking about. I've got some ideas along those lines to try to overcome the issue. I've found some couplers like that allowing up to 15 deg axial misalignment, which probably isn't enough to mitigate the issue entirely (though I haven't calculated the range of turning it would allow and would also largely mitigate the benefit as it would wind up upon initial acceleration). You could definitely put a one way bearing or similar in and only do left turns like zoolander :grin:. There are also options of mechanical or electrically actuated clutches, etc that I've been looking at. At this stage it will probably be an exercise in the space of proof-of-concept as opposed to something elegant / simple enough to be worthwhile, but that's half the fun.

I'm thinking I might try to kludge a pass-through ratchet mechanism between the axles as proof-of-concept, though it would undoubtedly fail under real riding conditions. A tooth or roller clutch made for high torque / rpm might be feasible [Link][1]. The nice part is that once you come out of the turn, the two wheels are travelling at the same angular speed, so re-engaging shouldn't be too hard on the clutch. An active, arduino controlled clutch isn't hard to imagine, but also not quite trivial.A passive, mechanical engagement would be much more satisfactory. 


  [1]: http://www.tinyclutch.com/a-series-roller-clutches/
```

---
## \#13 Posted by: onloop Posted at: 2015-11-02T03:23:51.782Z Reads: 353

```
just slide through every corner! PROBLEM SOLVED!

https://www.youtube.com/watch?v=pt5zABPTllc
```

---
## \#14 Posted by: emotiva Posted at: 2015-11-02T03:26:31.791Z Reads: 344

```
Ha! but on pneumatics!? :neutral_face: I've never skateboarded before, so I'll leave that challenge for someone else!
```

---
## \#15 Posted by: trbt555 Posted at: 2015-11-02T06:27:23.779Z Reads: 346

```
Large scale rc cars use axial differentials that might be modified to suit your needs.
I as thinking something like this : [Chinese axial differential][1] but you'd need to modify the outer gear to take a pulley somehow.

Dunno, just thinking out loud.


  [1]: http://www.aliexpress.com/item/60045-HSP-1-8-RC-Car-Differential-Gear-Set-Model-Car-AUSSIE-SELLER/1749149990.html?spm=2114.01020208.3.10.bdYy5X&ws_ab_test=searchweb201556_2_71_72_73_74_75,searchweb0_0,searchweb201560_9
```

---
## \#16 Posted by: cmatson Posted at: 2015-11-02T06:38:58.466Z Reads: 333

```
I have an axial yeti xl (uses the same diff you linked) and I doubt it would last one acceleration with body weight...

the spider gears on the inside are pretty small, and people strip them with just rc motors on asphalt.

The concept is good, it just needs to be blown up to scale for an eboard!
```

---
## \#17 Posted by: treenutter Posted at: 2015-12-16T16:44:28.974Z Reads: 325

```
@emotiva did you ever get this dual-drive-single-motor concept to work?
```

---
## \#18 Posted by: emotiva Posted at: 2015-12-22T01:11:06.924Z Reads: 311

```
I actually suffered a fairly serious head injury (and brain hemorrhaged) a month ago and haven't done much of anything since. I'm getting mostly back to normal now and hope to revisit possible solutions at some point when my mental drive (hopefully) returns! I probably can't ride for a few months, but if I can gather the motivation, it might make a nice project in the meantime.
```

---
## \#19 Posted by: Jack Posted at: 2015-12-22T01:26:38.058Z Reads: 315

```
@emotiva Awww that sounds nasty, hope you are okay and recovering well. Was that injury from an e-skate related incident? This concept looks great from a simple setup with great torque for steep hills. Thats the only reason I'm looking to go duel motors for better traction.
```

---
## \#20 Posted by: psychotiller Posted at: 2015-12-22T01:31:48.430Z Reads: 316

```
Here's to a speedy recovery brother!
```

---
## \#21 Posted by: emotiva Posted at: 2015-12-22T02:47:23.859Z Reads: 299

```
Thanks! Yeah, it was e-skate related. I was using a soldered nunchuck setup and when I went over a utilities cover on the sidewalk, the board went full acceleration and stayed there longer than I could stay on the board. I was just testing some things out, so I stupidly did not put my helmet on (I generally always use one, cycling or whatever).  Worked great up to that point! I know many people have used the soldered nunchuck setup extensively without issue, so perhaps it was unstable wire routing, or a poor solder joint, or something else rather than interference / loss of signal. I should try reproducing the issue one day (standing off the board, maybe). Wear your helmets kids!
```

---
## \#22 Posted by: treenutter Posted at: 2015-12-22T03:31:28.488Z Reads: 306

```
@emotiva sorry to hear it! I hope you have a speedy recovery!
```

---
## \#23 Posted by: mostwanted Posted at: 2016-02-24T11:19:14.045Z Reads: 304

```
i've been thinking about ~

1)  hub motors                    since november 2015 (my own inside~my~head thinking , but doing nothing physically) :sweat_smile:
2)  trucks with suspensions since i saw bajaboard and that youtube kickstarter 
3)  longboard  footbrakes     since december 2015
4)  single motor dual belt     since viewing eboard pics in google images about an eboarder who made one using a GIGANTIC motor Turnigy 8085 (i think)  in endless sphere .


https://youtu.be/QWM6ALGxaD0


https://youtu.be/aV4_q7GXuvU


what else did we miss ?
```

---
## \#24 Posted by: NIK Posted at: 2016-02-24T12:16:10.071Z Reads: 297

```
I think if they use super flex deck like loaded or etc, plus the suspension truck. That would be toooootallyy flexationn and scary. haha
```

---
## \#25 Posted by: Pablo_702 Posted at: 2016-07-14T07:12:24.796Z Reads: 249

```
Were you able to finish this build?
```

---
## \#26 Posted by: Zoomy Posted at: 2017-05-30T07:40:49.688Z Reads: 185

```
Has anyone done this yet? I am interested in finding some results.
```

---
## \#27 Posted by: lowGuido Posted at: 2017-05-30T17:35:13.857Z Reads: 173

```
I think that the only person who has done this with any success is carvon, they has some sort of one way bearing for differential if I recall?
```

---
## \#28 Posted by: Skitzor Posted at: 2017-05-30T17:47:54.108Z Reads: 173

```
I am very close to a working prototype. The biggest problem I'm running into is that most RC parts are plastic. If someone could craft me the same parts in decent iron, I'm sure I've got the solution
```

---
## \#29 Posted by: BigBoyToys Posted at: 2017-10-13T00:42:44.957Z Reads: 144

```
Anyone seen this?

https://youtu.be/OfPCWTYlGdI
```

---
## \#30 Posted by: Riako Posted at: 2017-10-24T00:50:33.860Z Reads: 137

```
huuum... look cool for lighweight setup !
See once on esk8fr groupe today (he made many build like this)
https://scontent-cdt1-1.xx.fbcdn.net/v/t31.0-8/22550410_1930388660310982_9115740638356980718_o.jpg?oh=5a569f7ac96e30614ea0fb825fc82b2d&oe=5A7AB381
:blush:
```

---
## \#31 Posted by: AgileCow Posted at: 2017-10-26T12:24:47.891Z Reads: 126

```
@Riako any chance for a link to the post?
```

---
## \#32 Posted by: Riako Posted at: 2017-10-26T13:27:32.007Z Reads: 125

```
he didn't post on esk8fr forum .. just the FB groupe ...
But here an other zoom in pic : 
https://scontent-cdt1-1.xx.fbcdn.net/v/t31.0-8/21741264_1891207870895728_3529500367419860885_o.jpg?oh=19a42ba004c2130786cf7fb0361e30b4&oe=5A78DA5B
I think I need to try it :blush:
```

---
## \#33 Posted by: AgileCow Posted at: 2017-10-26T13:37:24.112Z Reads: 119

```
Oh yeah, that seems like it's, at minimum, worth a go :slight_smile:
```

---
## \#34 Posted by: Okami Posted at: 2017-12-11T13:11:12.462Z Reads: 100

```
https://www.banggood.com/REMO-P6952-Differential-Gear-Assembly-116-RC-Car-Parts-For-Truggy-Buggy-Short-Course-1631-1651-1621-p-1101814.html?rmmds=detail-top-buytogether-auto&cur_warehouse=CN

Recently found this, so has anyone else tried it and succeeded ?

--
```

---

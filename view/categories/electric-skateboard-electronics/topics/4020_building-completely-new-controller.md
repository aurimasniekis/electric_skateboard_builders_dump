# Building completely new controller?

### Replies: 14 Views: 2311

## \#1 Posted by: OskarCastrone Posted at: 2016-05-30T18:26:50.151Z Reads: 183

```
Hi there

Has anyone tried to build there own controller/transmitter?
I am not talking about modifying a controller like the Bad Wolf enclosure, but instead building a totally new controller build from the ground up. I am certainly no expert at electronics therefore I am going to need some help, but I really like the idea of making a controller that fits our needs completely. 

Another approach would be to buy a cheap circuit board kit like [this](http://www.aliexpress.com/item/4channel-remote-control-40-27MHZ-remote-control-toy-car-remote-control-transmitter-board-receives-board-antenna/32218289018.html?spm=2114.01010208.3.181.MUqGrI&ws_ab_test=searchweb201556_10,searchweb201602_4_10017_10021_507_10022_10020_10009_10008_10018_10019_101,searchweb201603_2&btsid=7cb54904-cf4d-4a1b-814d-427d26405689) or [this](http://www.aliexpress.com/item/6CH-27-40Mhz-RC-Remote-control-module-transmitting-receiver-for-car-tank-model/32577428330.html?spm=2114.10010108.100009.2.U7s2v7) and modify it. I have no idea how that would work though...
Please share your thoughts and ideas. Any help from experts and future buyers will be much appreciated!
```

---
## \#2 Posted by: Lukas Posted at: 2016-05-30T18:46:52.964Z Reads: 179

```
See this:

http://www.electric-skateboard.builders/t/vesc-connect-beta-program/2427

You can read the thread but I also recommend watching some of jacobs videos that he linked and some others on his channel.

there is also this:

https://endless-sphere.com/forums/viewtopic.php?t=73812


But i encourage everybody to try to make their own stuff! If <ou can make something better than anything we have now, the community profits! :slight_smile:
```

---
## \#3 Posted by: g4tv4life Posted at: 2016-05-30T18:54:07.462Z Reads: 168

```
I'm going to do what this guy is doing for my controller.
https://www.youtube.com/watch?v=zaTskMjpXtA
His instructables is more detailed.
http://www.instructables.com/id/Make-Your-Own-Electric-Motorized-Longboard/

It uses a wii nunchuck, but instead of the expensive wireless one, he modifys a regular one (which you can get on ebay for around 3 dollars. i paid 3.58 for a black one) using a arduino chip and a 433mhz transmitter-reciever. I got all the parts for under 15 dollars. the 433mhz is a pretty reliable spectrum and there shouldnt be any issues with dropouts if wired correctly.
```

---
## \#4 Posted by: OskarCastrone Posted at: 2016-05-30T19:32:43.214Z Reads: 158

```
I would still call this a modification and not a totally new remote.. But thanks for the links guys! :)
```

---
## \#5 Posted by: chipoi84 Posted at: 2016-05-30T19:35:47.544Z Reads: 156

```
Here is a completely new remote design: https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812&start=75
```

---
## \#6 Posted by: OskarCastrone Posted at: 2016-05-30T19:44:39.898Z Reads: 153

```
Looks good! It may be over my level of knowledge but I will  definitely give it a try! :muscle:
```

---
## \#7 Posted by: g4tv4life Posted at: 2016-05-30T20:02:16.248Z Reads: 144

```
the only difference between the nunchuck being a new controller and being a mod is pretty much the case and potentiometer (aka thumbstick). You could get a potentiometer, 3d print a custom case and put the components in it for a fully custom setup. I thought about, but between the 3d modeling i'd have to do and the wasted plastic in prints + cost of a potentiometer and buttons it would be more expensive and less refined than a nunchuck. plus, the nunchuck is a great shape for this. Can't be confused for a weapon either which can cause problems.
```

---
## \#8 Posted by: OskarCastrone Posted at: 2016-05-31T20:52:02.977Z Reads: 115

```
You can't argue with that! You may have convinced me :smiley:.
```

---
## \#9 Posted by: DougM Posted at: 2016-06-01T02:39:41.582Z Reads: 105

```
I built my own controller - it uses an ADAFruit 9DOF module, an XBee and a Teensy.  The idea is that holding it in your hand parallel to the ground is neutral, tilt up for acceleration and tilt down for braking.  It works pretty well, but there are some gotchas.

Originally I wanted to control the board with my phone, and I had a working version, but the more I worked with it the worse an idea it became, for 3 reasons - 1) I can't shoot vid when I'm boarding, 2) if I crash I might break the phone and 3) I now have several boards, so letting friends use the other boards would be a challenge.

The upside of the controller is that it is very intuitive, requires no buttons (except an enable/disable button) or levers to drive it.

The downside is if things go wrong people tend to throw their hands up and that just makes it worse, and sometimes people forget to disable the board when we aren't riding and they flip the thing up and the board runs away.  I will fix this with a deadman sensor on the board but I haven't gotten around to it yet. 

The next rev will have a nice 3D printed case and some additional controls (like cruise control).

The other mistake I made was putting the power button right next to the enable button.  This confuses people for a while.  Next time I'll have a buried power switch - probably a slider or rocker.

DougM
```

---
## \#10 Posted by: g4tv4life Posted at: 2016-06-01T17:31:04.284Z Reads: 73

```
my opinion with tilt controls is that they are far to finicky. I'll admit they are intuitive, however when you are relying on something to act predictably (which considering your standing on a board with a powerful motor on, I want it to do exactly what I want), relying on a accelerator is just not reliable enough. Anyone who's ever used some sort of motion control and can tell you that it has been finicky and not worked on occasion. I'd much rather have a solid, mechanical system where the weakness link is the wireless connection, which on spectrum like 433 and 2.4ghz are very reliable.

Plus, that sounds like carpel tunnel in the making there XD
```

---
## \#11 Posted by: DougM Posted at: 2016-06-01T18:46:17.823Z Reads: 75

```
I haven't really found that to be the case but, ironically, I've never used a mechanical controller.  It isn't that finicky, depending on how you write the software, but even if it was you could easily add an averaging filter to take that out.

I also found that after about the first two times you use it you stop holding in firmly in your hand and begin to hold it between your thumb and forefinger, using your lower fingers to tilt it up and down.  The 3D printed case will be designed specifically for this hand position.

DougM
```

---
## \#12 Posted by: OskarCastrone Posted at: 2016-06-01T21:30:04.047Z Reads: 68

```
This sounds very interesting! Have you made a thread about it, because you should! Be sure to include pictures and/or videos! :D
```

---
## \#13 Posted by: DougM Posted at: 2016-06-02T14:34:10.911Z Reads: 60

```
Thanks, I'm hoping to put together a full build log but I'm having trouble deciding which platform (blogspot? etc.) to setup on.  Suggestions welcome, but it needs to be a more generic platform since not all my projects are esk8 related.

I'm also thinking of maybe selling these as a kit, but right now the BOM is pretty high.

this is looking like a thread hijack, if so please pm me any suggestions.

DougM
```

---
## \#14 Posted by: OskarCastrone Posted at: 2016-06-02T20:58:08.321Z Reads: 54

```
Seem very nice! I will look forward to it! According to your choice of platform I would suggest either Squarespace (a bit expensive but worth it!!) or wordpress (can also work great with the right choice of "skin". Can also be a pain in the ass though). I am actually considering setting up a webshop in EU, so if/when I do, I will gladly sell your remote on my website!

Your posts is not a hijack at all - you simply gave the answer which the thread was asking for ;-)
```

---

# Benchwheel Power Delivery

### Replies: 19 Views: 3565

## \#1 Posted by: thisguyhere Posted at: 2016-09-01T16:48:14.897Z Reads: 210

```
Got a Benchwheel about a month ago, it's been working great up until now but I'm running into some issues, mainly going uphill.

For the most part, it's great on a flat surface.

I'm using the board to travel the last mile to work, which includes a pretty steep incline.

Originally, this board hit that hill with no issues.  Now, after putting roughly 30 miles on the board, it's failing up the hill.

So, the question is, what part is failing?

* Has the battery capacity diminished?
* One or both motors faulty?
* Does the ESC somehow lose their capability after some use?

When I test the board flipped upside down, both wheels turn but the left one is slightly "slower?"  As in, when I give it full throttle and let go, the left wheel / motor comes to a stop first and the right wheel / motor seems to coast a bit longer.

Any insight would be appreciated.

-----------

edit:

Already referenced these posts:
http://www.electric-skateboard.builders/t/new-benchwheel-board-broke-need-help-with-repair/8165/28
http://www.electric-skateboard.builders/t/benchwheel-surgery/867
http://www.electric-skateboard.builders/t/modifying-a-benchwheel-electric-skateboard/7238

I should note, I know building a custom board with legit parts is the best way to go.  I get that.  I just needed a board right away and didn't have the luxury of building-failing-redesigning-rebuilding a board.
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-09-01T16:54:50.153Z Reads: 172

```
Need to check if the wheel is spinning free on the slower wheel... Is it the belt rubbing? Is there resistance from the motor? 

Re check if the motor phase wires are all connected...

Start there
```

---
## \#3 Posted by: Karmannghiagirl Posted at: 2016-09-01T17:01:06.716Z Reads: 165

```
I would also verify that there are no shorts in the motor wires. that can wreak all sorts of havoc
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-09-01T17:05:16.308Z Reads: 162

```
[quote="thisguyhere, post:1, topic:8771"]
I should note, I know building a custom board with legit parts is the best way to go.  I get that.  I just needed a board right away and didn't have the luxury of building-failing-redesigning-rebuilding a board.
[/quote]

Lol.... Ok nobody give him crap 

He already fessed up lol
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-09-01T17:12:03.546Z Reads: 152

```
[quote="thisguyhere, post:1, topic:8771"]
So, the question is, what part is failing?


Has the battery capacity diminished?
One or both motors faulty?
Does the ESC somehow loose their capability after some use?
[/quote]

It's most likey one motor...

The board has two individual ESCs running each motor...

If it was the battery...you would see it effect both motors...

ESCs either work or don't work usually ...

So, in this case could be the belt rubbing the wheel...could be a loose phase wire, it could be an internal motor short ....

The first two can be easily identified .... The motor short...well..you can flip it over and observe if you see any type of spark inside the motor while it's running or feel it is harder to turn compared to the other motor..
```

---
## \#6 Posted by: thisguyhere Posted at: 2016-09-01T17:45:12.915Z Reads: 137

```
[quote="Michaelinvegas, post:5, topic:8771"]
It's most likey one motor...

The board has two individual ESCs running each motor...

If it was the battery...you would see it effect both motors...

ESCs either work or don't work usually ...

So, in this case could be the belt rubbing the wheel...could be a loose phase wire, it could be an internal motor short ....

The first two can be easily identified .... The motor short...well..you can flip it over and observe if you see any type of spark inside the motor while it's running or feel it is harder to turn compared to the other motor..
[/quote]

so awesome...thanks for the info.

i did take the drive wheels and belts off last night just to prod around in there a bit.

one weird thing i noticed is the one of the two belt is slightly different in stiffness.  same length and all, but one feels slightly "thicker" than the other.

anyhow, i basically rotated the wheel and belt, left-to-right, right-to-left, and it's still exhibiting the same "out of sync" speed.

so i'll remove the wires tonight and reconnect, makes sure they're on right.

i can't tell if there's a spark in the motor because they are encased.

either way, more to follow...
```

---
## \#8 Posted by: thisguyhere Posted at: 2016-09-01T17:47:53.904Z Reads: 115

```
[quote="Michaelinvegas, post:4, topic:8771"]

[quote="thisguyhere, post:1, topic:8771"]
I should note, I know building a custom board with legit parts is the best way to go.  I get that.  I just needed a board right away and didn't have the luxury of building-failing-redesigning-rebuilding a board.
[/quote]

Lol.... Ok nobody give him crap 

He already fessed up lol
[/quote]

now that i have a board for communiting, i'm going to start collecting parts to build a custom one, just to see how all this comes together.

sadly, this is a hobby that's not exactly cheap...
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-09-01T18:22:38.409Z Reads: 110

```
Yup need to budget .... Good thing sometimes it take time to get things 

Look here first 

http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-09-01T18:24:45.486Z Reads: 104

```
[quote="thisguyhere, post:6, topic:8771"]
anyhow, i basically rotated the wheel and belt, left-to-right, right-to-left, and it's still exhibiting the same "out of sync" speed.
[/quote]

These should run independent of each other basically
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-09-01T20:28:39.560Z Reads: 96

```
Also ... Video would be helpful 

Upload to YouTube and past link
```

---
## \#12 Posted by: thisguyhere Posted at: 2016-09-02T00:15:35.825Z Reads: 96

```
Fosho, it's OK the way.

Im going to try tonite. 

So, on the ride back I noticed there's resistance when standing still. While stopped I was just kicking the board forward and backwards and it felt like the brakes were on. Definitely feels like some kind of short. 

Gonna troubleshoot the hell out of this tonite. 

Details to follow.
```

---
## \#13 Posted by: Mobutusan Posted at: 2016-09-02T05:13:24.454Z Reads: 93

```
@thisguyhere is there any way to swap the motor phase wires to the opposite motors? if the weird motor Behavior switches sides when you do that it's probably an ESC issue. otherwise, if it stays the same then it's probably a motor / drivetrain issue.
```

---
## \#14 Posted by: thisguyhere Posted at: 2016-09-02T06:28:12.021Z Reads: 103

```
ok, got some stuff for you.

Benchwheel Motor Test - 1/4 - Original Configuration
https://youtu.be/iVqhW2Wxtzc

Benchwheel Motor Test - 2/4 - Original Configuration - No Wheels
https://youtu.be/qITy_bHpCn4

Benchwheel Motor Test - 3/4 - Outside of Case - Original Wiring 
https://youtu.be/2uaq5-b3IEw

Benchwheel Motor Test - 4/4 - Outside of Case - Wiring swapped sides 
https://youtu.be/MWSSOPTDyW4

Had the courage to take it apart after seeing the [surgery](http://www.electric-skateboard.builders/t/benchwheel-surgery/867) post.

Some photos: http://imgur.com/a/UtWZJ

As far as I can tell, all of the wires seems well connected, can't really see any shorts happening.  Took everything out of the case to see if there's anything obvious with the electronics, but nothing.

As @Mobutusan suggested, I'll try swapping the phase wires and see if that has any impact.

More to follow...
```

---
## \#15 Posted by: Smithster Posted at: 2016-11-15T23:57:45.793Z Reads: 65

```
any update @thisguyhere did you manage to resolve the issue?
```

---
## \#16 Posted by: thisguyhere Posted at: 2016-11-17T17:29:02.322Z Reads: 58

```
sorry about the delay.

no real solution, but it seems the battery pack is unable to deliver enough voltage when the motor requires it (going up hill).

board still works fine on flat ground so it's technically still working, but i think the battery pack's degraded since coming out of box.

i'm in the process of building a new battery pack, upgrading to vescs, but attempting to scavenge a lot of the parts from the existing board (motors, mounts, trucks, remote, etc).
```

---
## \#17 Posted by: Smithster Posted at: 2016-11-17T18:39:25.887Z Reads: 55

```
Hope you get the battery sorted out would be interesting to see how the board performs with uprated battery and vescs.

Having read up on the Benchwheel Motor/Mount it seems to be a solid piece of kit.
```

---
## \#18 Posted by: konstantin Posted at: 2017-01-19T07:18:08.330Z Reads: 40

```
have you tried top notch ceramic bearings as well ,i assume you keep your bearings in top notch condition .like i do ,7 of course ABEC 9 PLUS I USE 11 BUT I DONT THINK CERAMICS HAVE A ABEC NUMBER SO,,
seriously my benchwheel has the best ceramic bearings and it make such a difference ,what are you using to modify the battery pack ,
DID YOU SORT IT ?
```

---
## \#19 Posted by: thisguyhere Posted at: 2017-01-19T07:39:01.130Z Reads: 41

```
abandoned the benchwheel altogether.  eventually one of the two motor burned out and the controller isn't working either.  i think i properly burned out the electronics.

instead i'm about 95% done with a fresh building using vescs, a 10s4p battery pack using samsung 25r cells, a proper deck, psychotiller's mounts, jlab's motors, etc.

will put up a build post once complete.
```

---
## \#20 Posted by: konstantin Posted at: 2017-01-19T07:46:39.368Z Reads: 38

```
HI CAN'T WAIT TO SEE IT ,
MAYBE YOU COULD MAKE A VID TOO ,
GIVE ME THE SPECS HOW IT DOES ,
WAS YOUR BENCHWHEEL A "C BOARD  OR A "B BOARD ? 
MAYBE YOU SHOULD PUT THE PARTS ON EBAY 
GET SOME CASH BACK
[quote="thisguyhere, post:19, topic:8771, full:true"]
abandoned the benchwheel altogether.  eventually one of the two motor burned out and the controller isn't working either.  i think i properly burned out the electronics.

instead i'm about 95% done with a fresh building using vescs, a 10s4p battery pack using samsung 25r cells, a proper deck, psychotiller's mounts, jlab's motors, etc.

will put up a build post once complete.
[/quote]
```

---

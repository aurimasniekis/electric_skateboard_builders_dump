# Big dumb cutoff switch

### Replies: 10 Views: 1437

## \#1 Posted by: DougM Posted at: 2016-07-08T04:05:09.105Z Reads: 161

```
Ok, after my runaway board incident here:


[Runaway Longboard!](http://www.electric-skateboard.builders/t/runaway-elongboard/4812)

I decided that a big dumb almost mechanical cutoff switch was in order.

So I modified Vedder's anti-spark switch to add a bigger (60A) fuse and some form factor changes and ordered some emergency cutoff switches from Amazon here:

https://smile.amazon.com/gp/product/B0094GM004/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1

Tonight I wired it all up and tested it - and it works great.  Twist the switch to pop it up and turn on the board and mash it to shut it all down.  

<img src="/uploads/db1493/original/2X/5/5b66258895734a1d18d5f6b0ea7ab7db3a4b1d15.jpg" width="690" height="388">

I'm going to mount this on the rear riser so it is easily accessible while riding.  I'll post some piccies when it's mounted on the board.

DougM
```

---
## \#2 Posted by: Blasto Posted at: 2016-07-08T04:15:12.387Z Reads: 148

```
I'm pretty sure you won't have time to hit that switch if your board fucks off.

Very nice though
```

---
## \#3 Posted by: DougM Posted at: 2016-07-08T04:19:10.630Z Reads: 142

```
During the runaway I had plenty of time - probably 2 seconds - to weigh all my options.  But I get what you're saying - if the motor windings short it won't help.  But then nothing will help that, except a helmet.
```

---
## \#4 Posted by: DougM Posted at: 2016-07-08T04:19:20.532Z Reads: 138

```
Since I know I'm going to get this question, the fuse is a Digi-Key F5097-ND and the fuse holder is a 3555-2K-ND
```

---
## \#5 Posted by: Kaly Posted at: 2016-07-09T02:55:50.347Z Reads: 105

```
[quote="DougM, post:3, topic:5751"]
During the runaway I had plenty of time - probably 2 seconds
[/quote]

Practice high speed runs (30+) once in a while in case you need 2 more extra seconds to use the switch. Good luck :slight_smile:
```

---
## \#6 Posted by: DougM Posted at: 2016-07-09T04:13:10.753Z Reads: 102

```
That's probably a good idea - though I geared it down a bit so now I don't think it can do 30 anymore.  But I need to practice moving around on the board at speed so I can routinely get to the button.

Currently I don't have enough space on the back riser for the button and the anti-spark circuit without interfering with the motor and wiring, so I"m going to have to re-arrange things a bit.

Also, I need to get a full face helmet if I'm going to do 30.
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-07-09T04:26:12.034Z Reads: 97

```
Moving around the board is a recipe of disaster at those speeds
```

---
## \#8 Posted by: baxter Posted at: 2016-07-09T08:59:26.566Z Reads: 82

```
@DougM,

I would recommend using a dead man's kill switch.  Its commonplace in the recreational boating world. Just like a leash a driver of a jet ski or a powerboat, it cuts the power if you fall overboard.  Probably easier than having to remember to mash down on a big E-stop button.  

I am sure that some smart people could even program their esc to apply the brakes as well if the circuit to the switch was broken.

<img src='http://www.easyacdc.com/wp-content/uploads/2011/03/Kill-switch.jpg'>  

This is the idea:

https://www.youtube.com/watch?v=eo5ZFvb2aAk
```

---
## \#9 Posted by: Tarzan Posted at: 2016-07-09T15:09:54.694Z Reads: 68

```
what do you think about switching of the remote instead?
The board should stop accelerating and roll out. Just an idea.
```

---
## \#10 Posted by: DougM Posted at: 2016-07-09T15:38:38.881Z Reads: 63

```
Well, keep in mind that the root of the problem is that the controller fried and stopped sending serial messages and the VESC did not correctly respond to this event and continued to execute the last received command, which was something like "set current 40" so any solution that involves the controller shutting things down won't work.

I agree that the better solution is the leash but the dork factor is just a little bit too high for me (yes, you could argue that a big red mushroom button is equally if not more dorky)

@Michaelinvegas - this is my biggest concern.  I won't be going 30 anymore, but even at 22 I'd rather not have to leap off the board - I'm going to mess around with getting at the button at lower speeds and see how it goes.

I'm fairly confident that the static shielding I added is the solution to the problem but time will tell.
```

---

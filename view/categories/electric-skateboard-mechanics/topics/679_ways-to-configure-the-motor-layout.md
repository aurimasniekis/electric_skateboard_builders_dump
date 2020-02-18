# Ways to configure the motor layout

### Replies: 5 Views: 1719

## \#1 Posted by: Sharkface Posted at: 2015-12-07T22:31:12.407Z Reads: 126

```
Hello All, I was curious about this and if we are at a dead end on developing other ways to mount motors onto the board. Of course I am strictly referring to ways that are easy for us to manufacture and build on our own. I would prefer not to have to start a whole company, get angel investors and all that jazz, just so I can have a fancy way of mounting motors to the board.

The ways I know of mounting motors on our boards as it stands now:

 1. truck mount single motor (front or back, left or right)
 2. Truck mount dual drive (both back, both front)
 3. truck mount diagnol drive (only two diagnols on the board)
 4. hub mount (1 wheel up to all 4 wheels)

has anybody put thought into doing a diagnol loadout, but each of the motors have a different gearing to them? One motor would be geared for high torque, while the other for high speed..... it would be up to us programmers to get the VESC to handle the motors together properly... but in theory you could have a boat load of torque and a boat load of speed, whilst only using 1 motor at a time?

Are there any other mounting strategies that yall have thought of??
```

---
## \#2 Posted by: lowGuido Posted at: 2015-12-07T23:16:06.576Z Reads: 125

```
I have never done an uneven diagonal, but I have built an uneven dual rear drive.
its a bit like a sequential twin turbo in that one motor has the torque off the line, and helps the other get moving, and one has the top end speed.

works well, however hill climbing is limited to that of maybe slightly better than a single drive rather than a equal torque dual drive hill eating machine.
```

---
## \#3 Posted by: onloop Posted at: 2015-12-08T01:04:35.340Z Reads: 119

```
One big motor & a diff would be cool... one guy made it... 
http://www.electric-skateboard.builders/uploads/db1493/optimized/1X/39dd5e66786d618995215dffa167bd1cf5e8d5c8_1_690x388.jpg

Or just a solid axle joining two wheels to one motor probably will work too.

Here is a similar thread about this topic

http://www.electric-skateboard.builders/t/two-wheel-drive-with-one-motor/116/5
```

---
## \#4 Posted by: Sharkface Posted at: 2015-12-08T03:14:40.223Z Reads: 109

```
@lowGuido : wouldnt that mean that you are getting some odd average of the two motors and not really getting the advantage of an uneven dual drive? Good label for it BTW

@onloop : i saw that thread the other day and totally forgot about it. Thanks for adding that into the mix!
```

---
## \#5 Posted by: lowGuido Posted at: 2015-12-08T04:04:11.910Z Reads: 108

```
[quote="Sharkface, post:4, topic:679"]
lowGuido : wouldnt that mean that you are getting some odd average of the two motors and not really getting the advantage of an uneven dual drive? Good label for it BTW
[/quote]

I'm not sure what you mean there, I'm going to say no.
I have ridden single drive, dual drive, and uneven dual drive back to back and I can tell you this:
UDR accelerates harder than DD and top speed is higher than DD.

here's a thread:
http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---

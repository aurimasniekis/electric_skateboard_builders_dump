# Info about ESC X-Car Beast 120A

### Replies: 17 Views: 1474

## \#1 Posted by: edoardo Posted at: 2017-10-05T23:08:44.089Z Reads: 121

```
Hi, is it possibile to join another switch to power on the ESC?
With this mod I would like to turn on and off the system by pressing the "new" button out of the container.

<img src="/uploads/db1493/original/3X/5/9/5973121edb193517dcab4ec5074aa2b8601a3be7.jpg" width="565" height="414">

Thanks.
```

---
## \#2 Posted by: MrHappy Posted at: 2017-10-05T23:39:17.325Z Reads: 115

```
maybe, you'd have to look how its wired up on the inside. of the switch. (ive done this with an external switch on one esc, not 2 at the same time)
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-10-06T02:13:57.416Z Reads: 101

```
First of all don't use that switch to turn your board on and off it's not meant to do that. If your looking for a way to turn your entire board on and off you need to use either a MOSFET Switch, a BMS  with a built in switch or a XT90 loop key.
```

---
## \#4 Posted by: edoardo Posted at: 2017-10-06T05:56:52.975Z Reads: 89

```
Currently I've a XT90s loop key, but it's uneasy to switch on and off the system. 

Can you explain what is a MOSFET switch? How can I implement that on my board? 
( you can also link me a useful topic )

Thanks! :slight_smile:
```

---
## \#5 Posted by: telnoi Posted at: 2017-10-06T06:03:01.892Z Reads: 88

```
MOSFET switch is sold under the name of Vedder anti Spark Switch. It just has +- in and out and goes in between your battery and other equipment.

Also comes with a 40/50a fuse. Some people replace these with an 80a, others solder bridge it and get rid of it and then there are those who use two Vedder switches to circumvent the low A rating.
```

---
## \#6 Posted by: jga Posted at: 2017-10-06T07:38:31.449Z Reads: 76

```
I can direct you to this site for anti-spark as described by @telnoi  I have no commercial interest there, and have not tested yet but it's handy for EU people

https://www.electric-skateboard.builders/t/launch-of-antisparkheaven-com-bulletproof-antispark-switches-nice-prices/31872?u=jga
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-10-06T07:53:03.520Z Reads: 73

```
be carefull with switches on a 6s system!
You´re pulling much more juice than others with 10 or 12s.
Most mosfet switches are rated up to 60A continous and will fail under a bit of riding on 6s.

Good thing with our friend @goldenHusky and his side antisparkheaven.com is, that he has some high power switches, which are able to withstand currents up to 160A cont.
```

---
## \#8 Posted by: edoardo Posted at: 2017-10-06T10:40:01.310Z Reads: 67

```
Hi! So do I have to buy [this](http://www.antisparkheaven.com/product/vedder-fechter-antispark-switch) ?
It's suitable for two motors but my ( single ) 5055-280kv needs 60A cont , and lower Vedder of that "product line" can deliver up to 30A.
```

---
## \#9 Posted by: jga Posted at: 2017-10-06T10:54:02.305Z Reads: 70

```
As it is an anti-spark between the battery and the VESC, I would say that what counts is what the battery can deliver, not really what the motors can take. But maybe that makes no sense. @TarzanHBK can correct me as necessary
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-10-06T11:25:02.298Z Reads: 65

```
i've got both bare bones 
https://longhairedboy.com/collections/all/products/12s-bare-bones-eswitch

and kits
https://longhairedboy.com/collections/all/products/12s-eswitch-complete-diy-kit

if you don't mind soldering.
```

---
## \#11 Posted by: edoardo Posted at: 2017-10-06T11:25:27.023Z Reads: 60

```
My battery is 4.5Ah 35C , so the max cont amp draw is about 160A ( approximated by excess )
Eventually my max cont amp draw is 60A ( limited by motor ) .

Am I right?
```

---
## \#12 Posted by: edoardo Posted at: 2017-10-06T11:34:33.367Z Reads: 58

```
This solution is too expensive... And my battery is a 6s1p, that eSwitch is designed for 12s, can it work with my system?
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-10-06T11:45:35.727Z Reads: 54

```
yes. yes it can. I used these with my 6S boards as well.
```

---
## \#14 Posted by: JdogAwesome Posted at: 2017-10-06T12:22:14.265Z Reads: 49

```
@TarzanHBK well my single FET switch that I built has been working just fine for me in 6S for a very long time. What I think a lot of people don't understand is that normally your only drawing around 15A continuously and you only draw upwards of 60A when accelerating or hill climbing. A 2x FET design like the standard Vedder switch will be fine for you and most people.
```

---
## \#15 Posted by: edoardo Posted at: 2017-10-06T12:30:50.210Z Reads: 48

```
You mean the Vedder linked from this post?
http://www.electric-skateboard.builders/t/info-about-esc-x-car-beast-120a/34893/8?u=edoardo

Or it's enough te switch for 30A cont?
```

---
## \#16 Posted by: TarzanHBK Posted at: 2017-10-07T08:30:42.207Z Reads: 42

```
Of course its enought for most of the time.
But i blow switches and destroy chains, made to be ok for most people..
I like to over engineer things, so it will last guaranteed!

It costs just a little bit more and therefore lasts forever!
```

---
## \#17 Posted by: JdogAwesome Posted at: 2017-10-08T23:25:18.797Z Reads: 28

```
Yeah exactly like for a mountain board or whatever your gonna be drawing a lot more current. And yeah over compensating on these types of things is a good idea.
```

---

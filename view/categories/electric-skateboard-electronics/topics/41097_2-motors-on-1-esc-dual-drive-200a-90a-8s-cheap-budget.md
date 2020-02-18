# 2 motors on 1 esc &#124; dual drive &#124; 200a 90a &#124; 8s &#124; cheap budget

### Replies: 26 Views: 1992

## \#1 Posted by: Dirt_Bag Posted at: 2017-12-15T04:00:59.612Z Reads: 231

```
I have an acceptable understanding of how an ESC's work but I would greatly appreciate others opinions. I have 2 motors that require a 90a esc each, could I use a single 200A if I do the following: 

I would join the motors together on a single shaft with all magnetic poles lined up with each other. This way the phases would be working together perfectly to create 1 really long motor. Everyone has said this would indeed work if I were to get it absolutely perfect.  (This makes sense considering that at this point it is more or less a single motor)
The problem comes with the fact that I need to mirror the motors join both back ends. If they were using the same exact phase signals, they would be counter rotating. Could I just switch 2 phase wires on 1 motor and still have those working together? The poles would still be lined up and the motors should receive power exactly the same. 


EDIT: the major reason people are saying it hasn't worked for them is because they have not joined the motors to share a single load. without this, inevitably the phases will fall out of sync.


I would love to hear from someone who knows more about this.
```

---
## \#2 Posted by: E1Allen Posted at: 2017-12-15T05:16:40.999Z Reads: 220

```
What kind of motors and kV?

Yes, swapping two phase wires changes the direction.
```

---
## \#3 Posted by: E1Allen Posted at: 2017-12-15T05:23:43.171Z Reads: 212

```
https://www.rcgroups.com/forums/showthread.php?1357604-Two-Brushless-motors-on-One-ESC%C2%85-YES%21
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2017-12-15T05:33:19.468Z Reads: 205

```
they are propdrive 5060 270 kv. i made a mistake when i said they require a 90a esc, they actually require a 100a. they will both be ran at 7-8s
```

---
## \#5 Posted by: Dirt_Bag Posted at: 2017-12-15T05:36:51.558Z Reads: 196

```
thanks for the link, a few of his cited sources i have never seen before. the problem is still the fact that none of the tests included a shared shaft to keep them in sync. this is really just a test on a novelty board.
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-12-15T05:39:33.595Z Reads: 190

```
generally speeking it is not wise to do 2 motor 1 esc. cuz of different turning radius for the wheels. 1 motor can get loss in sync. but because of low speed application in esk8 it may not be a big problem in smooth road. in real world tho u gatta test yourself
```

---
## \#7 Posted by: E1Allen Posted at: 2017-12-15T05:39:38.779Z Reads: 178

```
Well. No point not trying.
```

---
## \#8 Posted by: E1Allen Posted at: 2017-12-15T05:43:43.151Z Reads: 184

```
[quote="onepunchboard, post:6, topic:41097, full:true"]
generally speeking it is not wise to do 2 motor 1 esc. cuz of different turning radius for the wheels. 1 motor can get loss in sync. but because of low speed application in esk8 it may not be a big problem in smooth road. in real world tho u gatta test yourself
[/quote]

He will be connecting the motors physically together.  So it might get weird in slow speed turns.
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-12-15T05:47:45.656Z Reads: 177

```
yeap, i get it. still turning is problem either way. someone please invent magnetic differential!!!!
```

---
## \#10 Posted by: pennyboard Posted at: 2017-12-15T06:08:04.247Z Reads: 177

```
Honestly the much easier way to solve this problem of wanting more power but only using 1 esc is to just buy a bigger motor. It'll be much less hassle and you can buy motors for under $100 that are powerful enough that the ESC will be the limiting factor in power, not the motor. But if you're set on doing this "for science" then by all means. It'll be interesting to see.
```

---
## \#11 Posted by: Grozniy Posted at: 2017-12-15T09:11:31.982Z Reads: 168

```
like this one?
http://alienpowersystem.com/shop/brushless-motors/c8085-outrunner-brushless-motor-170kv-6000w/
```

---
## \#12 Posted by: Okami Posted at: 2017-12-16T14:32:27.827Z Reads: 159

```
Do u plan to run a mountainboard? Otherwise i think single motor should offer plenty of power. Or 2nd guess, huge hills is your target.

Anyways, I would look into **differentials**, if u were up to power everything with 1esc and 1 or 2 motors and save on electronics but hassle a bit with mechanics
```

---
## \#13 Posted by: gogomrrobot Posted at: 2017-12-16T15:16:36.756Z Reads: 152

```
I have been talking to Bruno @ APS.

The plan is to get this motor -- to be a smooth 8mm bore shaft on both sides:

http://alienpowersystem.com/shop/brushless-motors/c80100-sensored-outrunner-brushless-motor-130kv-7000w/

It's friggin 7000watts!  I think a single VESC6 clone (maybe even FOCBOX?) with about 80-100A of current to this motor could be used to create a dual drive from a single motor / single VESC.

The setup would play out like below (except the motor below is tiny in comparison to a 80100):

https://www.youtube.com/watch?v=OfPCWTYlGdI

I wish anybody could tell me they tried.  I have ordered (2) motor mounts from @marcmt88 so I want to test it out but it's an expensive for science test. Well i guess mostly I would be out the cost for the motor ~ $240 shipped roughly (includes shaft modification).
```

---
## \#14 Posted by: mmaner Posted at: 2017-12-16T16:59:11.503Z Reads: 137

```
[quote="Okami, post:12, topic:41097"]
Anyways, I would look into differentials
[/quote]

I've been thinking about a 6374 on the front running with wheels with 1 way bearings and x2 5054s on the back.  A total of 3 VESCs with a 10s or 12s 5p pack. I'm.wondering if the torque on the front with, a single motor, is equal on both wheels?
```

---
## \#15 Posted by: E1Allen Posted at: 2017-12-16T17:20:02.523Z Reads: 130

```
https://metr.at/r/T6UPp  
As far as your amps for a FOCBOX I think you will run into a temp issue @80-100a.  I did some testing with my dual 6374 setup on 12s pulled 53a on each box. But temps were on their way up as well fairly quick which any vesc will start to limit based on temp if you set it up.
[quote="gogomrrobot, post:13, topic:41097"]
It's friggin 7000watts!  I think a single VESC6 clone (maybe even FOCBOX?) with about 80-100A of current to this motor could be used to create a dual drive from a single motor / single VESC.
[/quote]

145a @48v to get to 7000w.  No reason you couldn't try this setup however you will probably be limited by something other than the motor is all.  Still going to be plenty powerful with less than 80a
```

---
## \#16 Posted by: pennyboard Posted at: 2017-12-17T07:19:11.894Z Reads: 122

```
You’d have to go VESC 6, or some other high amp Esc, to be able to use all the power that motor has. Have you looked at sk3 motors? They make some that have shafts on both sides and are under $100. Also driving both wheels with the same motor is gonna require a 1 way bearing or something otherwise you won’t be able to turn.
```

---
## \#17 Posted by: gogomrrobot Posted at: 2017-12-17T11:51:26.971Z Reads: 114

```
Turnigy SK3? I saw their 63mm and 50mm widths on hobbyking but nothing with a dual shaft
```

---
## \#18 Posted by: pennyboard Posted at: 2017-12-17T15:12:01.401Z Reads: 106

```
Most of them come with an attachment to attach a second shaft to the other side of the motor, I’ll post a picture of mine when I get home, either today or tomorrow.
```

---
## \#19 Posted by: pennyboard Posted at: 2017-12-18T16:32:41.875Z Reads: 102

```
<img src="/uploads/db1493/original/3X/3/b/3b2ac99b3297a3e7a00a3b58761598394d86f6e0.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/8/3/83abd0f9e3a12571995a2008ee76bf1566c7292c.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/b/bb7c883e6864503014330404ef53c4a250b5a66b.jpeg" width="374" height="500">
```

---
## \#21 Posted by: Homer900 Posted at: 2017-12-20T01:43:07.965Z Reads: 92

```
Your Sk3 is going to fall apart soon. 

Tighten the 3 black screws in the front quick!
```

---
## \#22 Posted by: pennyboard Posted at: 2017-12-20T02:20:02.894Z Reads: 83

```
Are you referring to the screws on the front mounting plate? They are tight. Well 2 are, that's all that's left. The head sheared off the third one a while back lol.
```

---
## \#23 Posted by: Homer900 Posted at: 2017-12-20T03:07:01.113Z Reads: 81

```
Yeah. I tap them out to M4 and put red lock tight. They never fail after that ;)
```

---
## \#25 Posted by: pennyboard Posted at: 2017-12-25T03:59:35.987Z Reads: 68

```
Dude before you rudely tell a long time member here to "pay attention" maybe look at the thread you're posting this in. This is literally a thread about "2 motors on 1 esc", which is exactly what he was talking about. You should be the one "paying attention" cause you're posting this in the wrong thread!
```

---
## \#26 Posted by: Sirshaunsta Posted at: 2017-12-25T07:15:13.784Z Reads: 57

```
Wooops my bad lol
```

---
## \#27 Posted by: banjaxxed Posted at: 2017-12-25T15:48:06.260Z Reads: 48

```
I've been looking into this exact scenario as well minus shaft work, imo you'll want to run a bearing on the motor can end inside the mount plate otherwise you're going to shake you shiz apart
```

---
## \#28 Posted by: gogomrrobot Posted at: 2017-12-25T15:59:51.128Z Reads: 50

```
It's the only option we have... to avoid dual vesc. And one motor one axle drive isn't good for braking or traction unless u are super lightweight person. Carvon and all these dual drive options are coming out but nobody is creating a dual vesc or dual motor capability vesc on one board from a hw or sw perspective.
```

---

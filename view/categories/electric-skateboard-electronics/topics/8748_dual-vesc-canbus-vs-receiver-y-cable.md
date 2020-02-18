# Dual VESC: CANBUS vs receiver Y cable?

### Replies: 12 Views: 1549

## \#1 Posted by: michaelcpg Posted at: 2016-09-01T04:13:18.586Z Reads: 280

```
I'm in the process of upgrading from a single to dual motor system and one thing I've been thinking about is how best to connect my VESCs.
I understand that having a master/slave VESC gives you the advantage of traction control however it also means that if the master VESC fails then you'll lose connection to both VESCs, something that won't occur if you've got the receiver connected to both VESCs via a Y cable.

How much of a difference do you guys find having traction control makes? Is there any other advantages/disadvantages to either option?

Cheers
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-01T04:23:13.419Z Reads: 276

```
Traction control caused me problems and made my motors jitter for apparently no reason. It can also cause problems if you turn hard and lift up your board or lose traction. I wouldn't use it on my builds for this reason. I used to use CAN, but it kept falling out, so I soldered it. Then the vibration made the pins break off. I'm using split PWM now and it's been great!
```

---
## \#3 Posted by: susplus Posted at: 2016-09-01T08:11:01.185Z Reads: 254

```
how reliable is that though ? i mean the Y cable....does the RX receive 5v from both esc???? in this case you might just bow the RX sooner or later....from my point of view ( i am no electrical engineer) the Y cable should be done only for the Signal Wire and the RX should receive it's 5V from only one VESC....correct me if I am wrong. ( have been also thinking of adding a second motor to my skateboard :) )
```

---
## \#4 Posted by: PB1 Posted at: 2016-09-01T09:37:38.574Z Reads: 238

```
Correct, the receiver should only be connected to one 5V source so you have to cut the 5V wire (normally the red one) on one of the cables going to the VESC. 

I've been using an Y-cable successfully on my double board, no issues. 
Think you can by them or solder your own.
```

---
## \#5 Posted by: dinodave Posted at: 2016-09-01T09:50:53.927Z Reads: 236

```
I think I'm seeing similar issues with the traction control. Sounds great in theory, but it seems off, like maybe it's too slow to respond? It sort of hesitantly tries to react, but then gets confused by the response, or something. Anyway, I'm going to try turning it off, and without it there does seem little benefit to going with the canbus link.
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-01T11:57:59.913Z Reads: 216

```
only problem turning off is that if your wheels lift off ground it'll free spin at max speed until it regains traction, not really a big deal though
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-01T15:37:53.111Z Reads: 210

```
I'm using split wpm instead of canbus. Just seemed like the most simple solution. And it works fine. 
I used zip ties to secure and prevent the wpm cables from working loose. 
<img src="/uploads/db1493/original/2X/b/b6d1014fa1d7175c62acad678cc5b5e9db19c6f1.png" width="281" height="500">
```

---
## \#8 Posted by: evoheyax Posted at: 2016-09-01T16:13:58.781Z Reads: 199

```
IMO, I'd rather have a cable than a port. Eventually, small plugs like the canbus will fail, if they are even reliably in the first place. I'd prefer to just has vescs come with wires soldered to the board instead of a port. I desoldered my canbus ports on my 4 vescs, soldered a wire between the front two vescs, a wire between the back two vescs, and a wire running the length between the two pairs. I fell like it's a reliable connection that I can't see failing. Traction control can be good, because it can help prevent a slipping wheel (I experienced this on a bad road with the dual carvons). But ideally, your wheels would never slip so it's probably mostly useless. The servo seems more redundant, and I'm going to try it with my next build.
```

---
## \#9 Posted by: Chris604 Posted at: 2016-11-16T16:47:02.372Z Reads: 158

```
Just did this,  hopefully it doesn't give me issues!  Anybody having problems?
```

---
## \#10 Posted by: laurnts Posted at: 2018-04-10T02:43:02.507Z Reads: 85

```
Yea I was just reading about this, I guess I also have similar issues with traction control having counterintuitive action when one of the wheels is lifting off. Causing random brake, jittering, sudden actions when wheels are bouncing or riding on 2 different surface. Interesting and noted!
```

---
## \#11 Posted by: lazerusrm Posted at: 2018-04-10T05:26:05.447Z Reads: 83

```
I'm using canbus with traction control and no problems. I'm pretty sure my board is one of the most ludicrous, though i never encounter a situation where i am going at speed and lift a wheel (e-MTB)
```

---
## \#12 Posted by: banjaxxed Posted at: 2018-05-19T17:21:19.687Z Reads: 58

```
I've encountered a jitter from my slave motor connected via canbus on a 4.12 vesc. I enabled traction control, which afaik requires a current 'control type'.

The solution was to disable 'send can status' on the master, I also increased 'can status rate' to 500Hz.

Maybe this will help someone with the jitters
```

---

# Jittery dual Car ESC - cause?

### Replies: 22 Views: 1621

## \#1 Posted by: Maxid Posted at: 2017-02-06T16:24:25.067Z Reads: 111

```
I recently finished my pneumatics build.
<img src="/uploads/db1493/original/3X/3/a/3a6703b59cb7d10745126692dd1b8da87856dabe.jpeg" width="375" height="500">

I am using two HK Car ESCs connected to a GT2B receiver via a y-cable. One of the ESCs however (the one with the cut red wire) is very sensitive causing the motor to jitter when in neutral. I increased the deadband to the maximum value in software but that made no change. Any ideas what I can try?

Also if anybody is wondering:
I am using a 6S Lipo and 6S Liions in parallel. Works fine so far
```

---
## \#2 Posted by: saul Posted at: 2017-02-06T17:12:05.891Z Reads: 97

```
try swaping motors/wires to see if its the esc or connection.

[quote="Maxid, post:1, topic:17299"]
Also if anybody is wondering:I am using a 6S Lipo and 6S Liions in parallel. Works fine so far
[/quote]

this is not a good idea. cells should be identical and balanced.
but the super asym motor setup looks interesting...
```

---
## \#3 Posted by: Maxid Posted at: 2017-02-06T17:19:32.384Z Reads: 99

```
[quote="saul, post:2, topic:17299, full:true"]
try swaping motors/wires to see if its the esc or connection.
[/quote]
can't swap receiver cables since I bought the ESC used from a forum member and unfortunately he cut the wire on the ESC side and not on the y-cable. Will swap motors though and get back to you.

[quote="saul, post:2, topic:17299, full:true"]
[quote="Maxid, post:1, topic:17299"]
Also if anybody is wondering:I am using a 6S Lipo and 6S Liions in parallel. Works fine so far
[/quote]

this is not a good idea. cells should be identical and balanced.
[/quote]

They are balanced - I charge them separately outside the enclosure. Also according to this:
https://jacklithium.wordpress.com/2013/12/22/mixing-battery-chemistry-li-ion-and-li-po/
it works fine. In parallel I don't see the issue as long as you take care of them.

The motors are actually set up to result in equal speed via different gearing.
The SK3 has a 20/50 ratio and the smaller 140kv Evolve clone has a 15/36 ratio.
```

---
## \#4 Posted by: lowGuido Posted at: 2017-02-06T17:40:22.812Z Reads: 85

```
im using the dual HK Xcar ESC's and I dont cut any red wire. no jitters here.
```

---
## \#5 Posted by: Maxid Posted at: 2017-02-06T17:51:25.063Z Reads: 84

```
I'll try to reconnect the wire then. Would be an easy fix :)
```

---
## \#6 Posted by: Maxid Posted at: 2017-02-06T20:37:11.053Z Reads: 73

```
Ok so I connected the red wire again. First thing I noticed is that now both ESCs turn on and off when I use the switch on one of them - even when the other is turned off. I also connected just the jittery one to the receiver directly and the jitter is also there - so it is not just a problem of the dual config but the actual ESC. 
Any other ideas? Since it was from a forum member I can't just send it back.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-02-07T12:20:33.530Z Reads: 64

```
[quote="Maxid, post:6, topic:17299"]
First thing I noticed is that now both ESCs turn on and off when I use the switch on one of them
[/quote]
this is normal.

[quote="Maxid, post:6, topic:17299"]
I also connected just the jittery one to the receiver directly and the jitter is also there
[/quote]
sounds like an ESC problem then.
does it work when throttle is applied?
```

---
## \#8 Posted by: Maxid Posted at: 2017-02-07T12:35:40.030Z Reads: 58

```
[quote="lowGuido, post:7, topic:17299, full:true"]
sounds like an ESC problem then.
does it work when throttle is applied?
[/quote]
Everything works but the neutral position (even after numerous throttle range recalibrations).
A small tap on the trigger sometimes makes the jitter stop but returning from like full throttle and releasing the trigger makes the motor jitter then.
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-02-07T12:39:16.995Z Reads: 61

```
Did you try to use only one esc and one motor to test the jittering?
Someone had a jittery esc before with a dual setup an Y cable. It was gone when he only used one esc for testing.
Couldn´t find the thread anymore.
```

---
## \#10 Posted by: Maxid Posted at: 2017-02-07T12:41:21.902Z Reads: 60

```
[quote="Maxid, post:6, topic:17299"]
I also connected just the jittery one to the receiver directly and the jitter is also there
[/quote]
Yeah I have tried and used only the jittery ESC (even with differing motors)
```

---
## \#11 Posted by: TarzanHBK Posted at: 2017-02-07T12:45:53.878Z Reads: 55

```
okok.. so the last test i would do is using an other remote to check.
If its still jittery, I´d replace that esc with a new one.
```

---
## \#12 Posted by: Maxid Posted at: 2017-02-07T12:53:59.320Z Reads: 52

```
bad thing is this is a new one I just got from a forum member :cry:
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-02-07T13:39:23.614Z Reads: 51

```
hmm thats always bad if you got something and it doesn´t work the way expected. 
And the forum member didn´t have the same issue with it?
```

---
## \#14 Posted by: Maxid Posted at: 2017-02-07T13:40:50.561Z Reads: 51

```
I asked him but so far no response
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-02-07T13:41:33.905Z Reads: 51

```
So do you have a second remote to check?
```

---
## \#16 Posted by: Maxid Posted at: 2017-02-07T13:42:28.039Z Reads: 52

```
No - and how can my original ESC work perfectly fine with the same remote when it would have something to do with it?
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-02-07T13:50:56.147Z Reads: 54

```
there are sometimes weird problems with some setups and if you change one part, everything works again flawlessly.
Sometimes it´s just a marginal different current or different resistance in a part..
```

---
## \#18 Posted by: mccloed Posted at: 2017-02-08T01:02:34.057Z Reads: 43

```
Might be a stupid question but, Did you do the throttle calibration on both ESC's?
```

---
## \#19 Posted by: Maxid Posted at: 2017-02-08T07:16:40.183Z Reads: 41

```
Yeah - several times.
```

---
## \#20 Posted by: saul Posted at: 2017-02-09T02:23:42.775Z Reads: 34

```
well if you swap the esc's motors your should be able to make sure that its just the one esc that has some issues.

fixing that issue is another question.. :thinking:

I have a spare hk120a xcar esc if thats what you are using..
```

---
## \#21 Posted by: Maxid Posted at: 2017-02-09T08:44:07.949Z Reads: 33

```
Yeah I tried it on both motors and without the second ESC - always the same thing. Seems like the neutral position is not detected properly and changing the deadband via the programming card has no effect as well. Don't know how to fix this now :cry:
I am using 150A XCar beast ESCs - my first one worked perfectly fine (I had to cut off the fan though - that thing is just annoyingly loud) and onle the "new" one gives me headaches.
```

---
## \#22 Posted by: Maxid Posted at: 2017-02-20T11:32:45.664Z Reads: 28

```
Ok I might have figured it out. After reconnecting the red wire the second ESC also turned on whenever I switched just one of the ESCs on. However this way the problem persisted. When I turn on both at the same time however the jittery ESC works fine (at least it did on the weekend :D ). Thanks everyone for helping me out here.
```

---

# Torqueboards 6355&rsquo;s are kind of locking up

### Replies: 12 Views: 342

## \#1 Posted by: plasteroid Posted at: 2018-10-19T17:39:17.844Z Reads: 153

```
Just started today - when I release the trigger on the remote - the board quickly grinds to a stop. 

Flipping it over, and manually trying to move the wheels, they are very very stiff.
If I turn of power, and spin them manually, they spin as normally expected - a little resistance due to the motor/pulley... but completely different than when power is on. 
Again this Just Started today - I can no longer coast downhill due to motor resistance slowing the board down.  
Any ideas?

![image|458x222](upload://lSTZlU8AMzwCxwSJrsj9MiLjgsj.jpeg)
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-10-19T17:41:29.673Z Reads: 142

```
[quote="plasteroid, post:1, topic:71737"]
over, and manually trying to move the wheels, they are very very stiff.
If I turn of power, and spin them manually, they spin as normally expected - a little resistance due to the motor/pulley… but completely different than when power is on.
[/quote]

What happens if you disconnect the motors from the ESC?
```

---
## \#3 Posted by: plasteroid Posted at: 2018-10-19T17:42:36.085Z Reads: 134

```
[quote="Pedrodemio, post:2, topic:71737"]
What happens if you disconnect the motors from the ESC?
[/quote]

Same as with power off - they rotate freely.
```

---
## \#4 Posted by: b264 Posted at: 2018-10-19T17:49:53.467Z Reads: 127

```
Sounds like your ESC has a closed FET (is broken)

Seriously, disconnect all wires from your motor and test it

It's probably your ESC
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-10-19T18:10:20.394Z Reads: 118

```
It can even be the DRV that is shorting a FET when on
```

---
## \#6 Posted by: torqueboards Posted at: 2018-10-19T18:18:28.350Z Reads: 110

```
@plasteroid - Can you send us an email? I'll PM you.
```

---
## \#7 Posted by: bigben Posted at: 2018-10-19T21:38:59.616Z Reads: 93

```
Sounds daft but is there any chance you have adjusted the trim on the remote a little so the deadzone has changed?
```

---
## \#8 Posted by: dg798 Posted at: 2018-10-19T21:40:39.348Z Reads: 90

```
Are the phases wires touching each other?
```

---
## \#9 Posted by: Namasaki Posted at: 2018-10-19T22:15:31.677Z Reads: 89

```
It could be the Esc as some stated or it could be the remote as @bigben stated.
I would start with the remote because that is the easiest to check out.
If your using the Mini RC remote, the white knobs can get moved accidentally and could cause this problem.
 If you are using the Mini remote, check that the knobs are aligned properly then check the calibration of the remote in the Vesc or BLDC tool.
 
![39%20PM|627x468](upload://m5nSgnKReLVF2dYbFpXplx6LLKl.png)
```

---
## \#10 Posted by: dareno Posted at: 2018-10-19T23:40:44.262Z Reads: 76

```
[quote="bigben, post:7, topic:71737, full:true"]
Sounds daft but is there any chance you have adjusted the trim on the remote a little so the deadzone has changed?
[/quote]

Not daft at all.  I had the same thing happen on my flysky.  took me ages to work it out too.
```

---
## \#11 Posted by: plasteroid Posted at: 2018-11-23T03:47:00.037Z Reads: 51

```
I just wanted to close out this thread.  No further issues.  At this point the issue seems to resolved itself.  
Thanks @torqueboards for the PM and support.
```

---
## \#12 Posted by: vjsharpeyes Posted at: 2018-11-24T08:39:15.087Z Reads: 31

```
For anyone else finding this with similar faults, my enertion motor experienced something similar and it turned out to be the phase wires shorting just inside the motor. Only happened when I got the vibrations just right. Took me a week to find the culprit.
```

---

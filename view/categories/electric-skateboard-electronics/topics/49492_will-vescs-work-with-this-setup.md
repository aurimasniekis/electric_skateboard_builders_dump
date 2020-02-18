# Will VESC&rsquo;s work with this setup?

### Replies: 14 Views: 512

## \#1 Posted by: spork Posted at: 2018-03-19T05:57:27.109Z Reads: 95

```
I just finished building a mountain board (10" pneumatic knobby tires) with this electronic setup.  It works great, but it starts terrible.  The motors just chatter like crazy on startup.  But once I get it going it runs great.  

I'm thinking I need to swap out the Jeti Spin Pro ESC's for ESC's that are designed for electric skateboards.  I like the VESC in theory, but I've heard a lot of folks are smoking them.  Will this config work with the VESC?  Any tips to avoid smoking them?

Thanks very much.

![Electric diagram|690x328](upload://mUsPfz7kAM3GUPlh9Tfgb8CKhuS.jpg)
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-03-19T06:08:10.029Z Reads: 89

```
I think the reason your having problems is your using  
6s on a 190kv motor according to your diagram  there not in series
```

---
## \#3 Posted by: E1Allen Posted at: 2018-03-19T06:14:14.524Z Reads: 80

```
Those are $500 ESC!  Crazy.  Yeah you really need to run those batteries in series not parallel.  Also of you're running a uncensored setup the motors will jitter if you start from a standstill.  What's your current gearing for motor and wheels?
```

---
## \#4 Posted by: E1Allen Posted at: 2018-03-19T06:26:22.332Z Reads: 71

```
I'd recommend focbox. They are around$150. They work good for most setups
```

---
## \#5 Posted by: spork Posted at: 2018-03-19T06:28:27.630Z Reads: 63

```
You guys are right that I'm running 6S on 190 KV motors.  I based that on the top speed I was planning on.    I'm running a 4.8:1 belt reduction.  With 10" diameter wheels, 190 KV motors, 6S, and 4.8:1 reduction I calculated a top speed of about 25 mph if I recall correctly.  I would think running 12S would give me an insane top speed.

>> Those are $500 ESC! Crazy.

It is kind of crazy.  They were left-over from another project, but still new-in-box.  I don't think they're ideally suited for an electric skateboard because they don't have proportional braking, and I don't think they're great for a start from a dead stop.  But maybe that can be fixed.  You mentioned unsensored motors.  I'm not familiar with sensored motors.  Can I add sensors?

Thanks again.
```

---
## \#6 Posted by: E1Allen Posted at: 2018-03-19T06:32:49.522Z Reads: 53

```
Unless someone says the sensors won't fit keda motors you would be able to use them in combination with a vesc for better low speed startup
```

---
## \#7 Posted by: spork Posted at: 2018-03-19T06:41:42.776Z Reads: 48

```
Thanks.  Can you point me at the sensors?  Not sure if they're magnetic, optical, etc.  But I bet I could make them fit.

Also, with the FocBox I notice they say it's based on the VESC open-source design.  I'm guessing based on the name that it specializes in field-oriented control.  From what I've read here it seems people are a little nervous about running FOC.  I don't think I'll have any need to since I'm not worried about noise - or are there other benefits?

Also, what advantages does the FocBox have over the standard VESC?

Thanks.
```

---
## \#8 Posted by: E1Allen Posted at: 2018-03-19T06:55:17.506Z Reads: 47

```
Focbox has direct fets for better cooling.

http://www.electric-skateboard.builders/t/installing-hall-sensors/18378/2
```

---
## \#9 Posted by: b264 Posted at: 2018-03-19T07:53:59.287Z Reads: 36

```
I don't know if those ESCs will have regenerative brakes, or brakes at all, and if they do, if they will be smooth enough to not toss you off the board.
```

---
## \#10 Posted by: spork Posted at: 2018-03-19T08:06:02.006Z Reads: 35

```
Are you referring to the ESC's I have now, the Spin Pro's?  If so, they do have some braking function, but they're not proportional.  You just set a braking profile.  But I think I need to replace them with something that will give me a better startup from stand-still.  I'm looking for advice on which ESC's to use.
```

---
## \#11 Posted by: b264 Posted at: 2018-03-19T08:07:43.138Z Reads: 32

```
[quote="spork, post:10, topic:49492"]
Are you referring to the ESC’s I have now, the Spin Pro’s?
[/quote]

Yes, I was
```

---
## \#12 Posted by: spork Posted at: 2018-03-19T08:08:30.422Z Reads: 32

```
Do you have a recommendation for an ESC that would work well with my setup?
```

---
## \#13 Posted by: b264 Posted at: 2018-03-19T08:10:41.483Z Reads: 32

```
Right now you're kind-of limited to FOCBOX or ESCape, and FOCBOX aren't available at the moment.  The ESC market is in a transition at this point in time.
```

---
## \#14 Posted by: spork Posted at: 2018-03-19T14:02:03.219Z Reads: 21

```
Is the VESC no good for this setup?
```

---

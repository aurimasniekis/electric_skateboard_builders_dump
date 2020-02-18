# R-Spec - given up the ghost? \[FIXED\]

### Replies: 25 Views: 1603

## \#1 Posted by: DanSkates Posted at: 2017-07-27T13:17:46.970Z Reads: 246

```
Forgive the play on words!  

I've had a hunt around but can't find a similar issue though it must be a fairly common I'd imagine.

Any ideas what might have given my motor the jitters?  It would be fair to say I'm not the most gentle lover and she really does need a good clean but today my motor slowly ground to a halt (the accelerator started breaking rather than accelerating) and now I get the following horrific cogging.  

https://www.youtube.com/watch?v=sPKT48tUfBA

Did I break it?  I can't see any broken wires etc, could this just be an ingress of dirt issue is is it likely something more serious?  OR could it be an electrical issue?  I have another FOCBOX to try but it would need different connectors soldering on so I thought I'd ask you awesome folk before I got my tip warm!  

Any help HUGELY appreciated :flushed:
```

---
## \#2 Posted by: Okami Posted at: 2017-07-27T13:27:46.148Z Reads: 223

```
hah.. actually nice play with the words considering the new motor name ;)

Well.. I have only 2 'guesses'·.

1) Something with your settings is not alright

2) Something has stuck into the stator and with motion your motor (the can) needs to skip over this obstacle, so it might as well cause the 'jitter'·.

To be honest I once caught up metal shavings when i placed motor on the table.. it was so bad that when turning the motor by hand it stuck at one point.. and onwards rotated smoothly in only one direction, otherwise it got stuck (stopped) completely again (if turned opposite direction)..

I would advise to check whenever it is 'easy' to turn the motor by hand.. or do you feel some sort of 'shakes' or 'rubbles' when turning it (not smooth) ?
```

---
## \#3 Posted by: DanSkates Posted at: 2017-07-27T13:34:21.396Z Reads: 201

```
Hey thanks for the quick reply!  So turning the wheel by hand (and rolling it along my forearm) feels exactly the same as it usually would - it doesn't feel gritty or obstructed in any way.  It actually happened when riding from a smooth cycle path to more bumpy paving and literally started decelerating at that moment.  I guess the jolt could have interfered with my electronics somehow?  Could that provide this result?
```

---
## \#4 Posted by: rpn314 Posted at: 2017-07-27T13:41:54.531Z Reads: 182

```
[quote="DanSkates, post:3, topic:28758, full:true"]
Hey thanks for the quick reply!  So turning the wheel by hand (and rolling it along my forearm) feels exactly the same as it usually would - it doesn't feel gritty or obstructed in any way.  It actually happened when riding from a smooth cycle path to more bumpy paving and literally started decelerating at that moment.  I guess the jolt could have interfered with my electronics somehow?  Could that provide this result?
[/quote]

Since turning it manually by hand is normal, I agree with @Okami; looks like something odd with your settings. I'd re-run motor detection and see if that fixes it. I'd be curious if and how much your values change. Just don't forget that you need to remove the load from the motor (belt and ideally the pulley as well) to run detection.
```

---
## \#5 Posted by: DanSkates Posted at: 2017-07-27T13:53:10.414Z Reads: 167

```
Thanks @rpn314 - so I just ran motor detection and the result was similar to the controller:

https://www.youtube.com/watch?v=ZqLQlyL8NGE

Cogging hell :scream:
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-07-27T14:12:30.886Z Reads: 156

```
you may have a short either in your phase leads or in the windings. Continuing to run motor detection with a short in the phase leads could potentially kill your VESC. 

Its also possible that you have a connection break, meaning the power isn't going through one of the phases as it should. If you feel comfortable removing the motor and can you might want to do that to look for tiny breaks in the windings.
```

---
## \#7 Posted by: rpn314 Posted at: 2017-07-27T14:17:39.984Z Reads: 156

```
I would have run detection after taking off the wheel and belt (and ideally pulley as well, so it's just the shaft left), but @longhairedboy speaks the truth.
```

---
## \#8 Posted by: TranxFu Posted at: 2017-07-27T14:21:15.068Z Reads: 153

```
Hey man, had the exact same problem. I figured that one of the phase wires coming from my motor were mangled and it disturbed with motor detection. I resoldered the wires and it was fine afterwards.
```

---
## \#9 Posted by: DanSkates Posted at: 2017-07-27T14:21:27.555Z Reads: 149

```
D'oh!  

Thanks man - appreciate the guidance.  I'll strip it down at the weekend and report back.  Sorry @rpn314 I see what you mean now by reducing the load!  Whoops, that would have made sense!
```

---
## \#10 Posted by: DanSkates Posted at: 2017-07-27T14:27:18.320Z Reads: 146

```
AHA!  That'd make sense...and pretty resuring that it might be salvageable.  I guess the proof is in the pudding.  I'll do a bit of research on how to get her clothes off and report back :wink:
```

---
## \#11 Posted by: trancejunkiexxl Posted at: 2017-07-27T14:32:17.777Z Reads: 137

```
id like to say i found the same issue with bent phase wires.. just had to snip and redo them..
```

---
## \#12 Posted by: Bazingazunga Posted at: 2017-07-27T14:42:32.135Z Reads: 136

```
Quick question always wondered - what real world difference would you see if motor detection had been done with/without a pulley+belt? Or is it just a case of 'nothing-really-but-its-best-practice'?
```

---
## \#13 Posted by: rpn314 Posted at: 2017-07-27T17:11:54.708Z Reads: 136

```
[quote="Bazingazunga, post:12, topic:28758, full:true"]
Quick question always wondered - what real world difference would you see if motor detection had been done with/without a pulley+belt? Or is it just a case of 'nothing-really-but-its-best-practice'?
[/quote]

I'll run a test tonight and tell you :)
Vauge recollection of other's experiences tells me that even just the pulley makes a difference of about 100 BEMF.
```

---
## \#14 Posted by: DanSkates Posted at: 2017-07-31T15:17:39.603Z Reads: 127

```
Hey folks!

So I tried the motor with a fresh vesc and had the same result so it has to be the motor.  

I've managed to disassemble it right to the final stages but it looks as though it's glued together???  I've been through [this thread](https://www.electric-skateboard.builders/t/rewinding-the-r-spec/1884) and can see it can be a bit of a beast to get apart but this is ridiculous!  Before I try to go any further can anyone see anything obvious that might be causing the issue??

<img src="/uploads/db1493/original/3X/1/c/1c9bc56292476eddc2b058a1720947ffe199c2c4.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/4/8/48d383b9fc30cff2e3d39d8acd44dc4ee82f14cd.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/6/b/6b3ea6bb804d5bfc5fd90fdb81820d9cdc3d6dbf.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/1/7/17d30c1fca53daa23de05827535ee151ccbb3a96.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/b/b/bb9a4a5787ffe4166e09c3fc4e8744e305dbb0e8.JPG" width="375" height="500">

Any help hugely appreciated.
```

---
## \#15 Posted by: DanSkates Posted at: 2017-08-01T02:29:06.683Z Reads: 116

```
So, I just had a closer look this morning and I think I've found the issue - a couple of wires have broken and look to have shorted against another phase wire - can this just happen if they touch?  The shrink wrap isn't long enough currently to prevent this. It's tricky to photograph but...

<img src="/uploads/db1493/original/3X/7/e/7ea21397eb88dae14d349660e7d1b53c7beb01e6.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/d/3/d38e850e738a33d1d2e75ec22aaf5443a4f17489.JPG" width="375" height="500">

Tried to remove the stator again but it's completely glued on so gonna try and just solder the broken wires and add longer shrink tubing to ensure they don't touch again and give it a whirl.  Hopefuly this will cure the issue?

Thanks,

Dan
```

---
## \#16 Posted by: DanSkates Posted at: 2017-08-01T03:15:36.938Z Reads: 116

```
HALLALUYAH!!!  Praise be to the esk8 gods SHE'S ALIIIIIIIIIIIIIIIIIIVE!!

<img src="/uploads/db1493/original/3X/a/0/a02cc6155e5173b99938e0f1e75353b1fa5717cc.jpg" width="500" height="280">

https://www.youtube.com/watch?v=YW7oZRH-nhE

Guess the phase wires touching is bad juju!  She does sound a little gruff but then I have been man handling the crap out of her - maybe a bit of lube will sweeten things up?  This is starting to sound a little bit to much like a blue movie!  :stuck_out_tongue_winking_eye:

Thank you everyone so much for your help - you my friends are legends :kissing_heart:
```

---
## \#17 Posted by: Mikenopolis Posted at: 2017-09-28T17:48:49.702Z Reads: 95

```
just got here because of your other post. I'm not looking forward to the day I would have to do this...interestingly, this thread looks just like you talking to yourself. Glad you shared
```

---
## \#18 Posted by: DanSkates Posted at: 2017-09-29T03:21:32.273Z Reads: 87

```
Ha thanks.  Yeah it was a bit of a tricky job, but I learnt quite a lot and the sense of achievement in reviving it from the dead was well worth it - plus it saved me $$$!  I reckon if I have to do it again it'll actually be quite a quick job, it's just having the balls to do it - I wouldn't do it for fun though! :laughing:
```

---
## \#19 Posted by: PDXroses Posted at: 2018-01-25T09:50:56.419Z Reads: 66

```
LHB, i have a similar problem with the motor cogging at acceleration (after the board in motion). It cogs randomly and seems to go away for minutes only to come back again.  Is likely that I traumatized my dear motor by riding it with loose screws over rough roads for a few miles?  It was working just fine prior to this abusive episode.
```

---
## \#20 Posted by: PDXroses Posted at: 2018-01-25T09:57:14.904Z Reads: 63

```
Very helpful thread. Thanks for sharing.
```

---
## \#21 Posted by: DanSkates Posted at: 2018-01-25T10:01:37.445Z Reads: 58

```
My pleasure. If it's intermittent it could be that the vibration of riding makes them touch giving you the confused signal aka cogging! It only takes for the wires to become exposed (the heat shrink could have moved over time) and for them to touch to cause that issue. I'm no expert though and this is just a theory from my own experience/meddling! 😉
```

---
## \#22 Posted by: PDXroses Posted at: 2018-01-25T10:44:41.797Z Reads: 62

```
I think you’re right. It doesn’t cog when I just spin the motors, but only when the road is rough. 

Oh that sinking feeling when something’s not working right. :confused:

And that feeling when you think you know why! :smile:
```

---
## \#23 Posted by: longhairedboy Posted at: 2018-01-25T12:54:59.859Z Reads: 58

```
you could have an intermittent short, that can happen when the winding wires start to break and then rub against things.
```

---
## \#24 Posted by: PDXroses Posted at: 2018-01-25T13:13:24.204Z Reads: 58

```
Interesting. Would heavy road vibration cause that?
```

---
## \#25 Posted by: longhairedboy Posted at: 2018-01-25T17:10:59.932Z Reads: 53

```
Yes. Road vibration can definitely lead to things like motor shorts. R-SPECs had a bit of an issue with motor shorts back when.
```

---

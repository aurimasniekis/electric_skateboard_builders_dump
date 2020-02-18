# Fast help, please

### Replies: 12 Views: 536

## \#1 Posted by: Samuele00 Posted at: 2017-12-11T16:40:40.487Z Reads: 154

```

when I have to connect vesc  to the motor  I have to do it with all the lipo batteries or just one? i use 9s with three lipo
```

---
## \#2 Posted by: Youssless Posted at: 2017-12-11T16:42:12.154Z Reads: 153

```
I used 3 3s lipos and connected them all when I put it together. If yours already has a firmware on it jump in.
```

---
## \#3 Posted by: Samuele00 Posted at: 2017-12-11T17:17:54.976Z Reads: 136

```
I did not understand, do I have to or should not put them?
```

---
## \#4 Posted by: mmaner Posted at: 2017-12-11T17:22:23.455Z Reads: 128

```
connect all 3, you need at least 6s to reliably run detections.  You would do better to run detections with the battery you are actually going to use.
```

---
## \#5 Posted by: saul Posted at: 2017-12-11T17:48:42.516Z Reads: 105

```
[quote="Samuele00, post:1, topic:40689"]
when I have to connect vesc  to the motor  I have to do it with all the lipo batteries or just one?
[/quote]

you don't have to use any batteries to connect the vesc and the motor.
but you could then connect batteries to the vesc if you want the motor to move and stuff...

your question makes no sense, i don't know why anyone even replied...
```

---
## \#6 Posted by: Samuele00 Posted at: 2017-12-11T18:09:28.772Z Reads: 81

```
I have to detect and set the parameters so it is obvious that I have to move the motor
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-12-11T18:38:57.240Z Reads: 78

```
The best thing to do, like @mmaner said, is to set up the battery packs like you plan to use them in your completed board, then run BLDC-Tool or VESC-Tool and do motor detection then. 

When  i build my custom completes, i build the whole board first. That includes installing the vescs and everything. I don't run motor detection and load settings until its all built and powering on. 

@saul What about his question didn't make sense, and why would noone answer him? Its a simple question, easily answered, and not really deserving of that reply.
```

---
## \#8 Posted by: saul Posted at: 2017-12-11T19:17:45.295Z Reads: 66

```
[quote="longhairedboy, post:7, topic:40689"]
not really deserving of that reply.
[/quote]

shit, if i'm getting an attitude check from you then I must have really been in a bad mood. 
the question has no context to me, i just gave up on answering the same questions over and over and over and over and ....
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-12-11T20:04:09.346Z Reads: 56

```
[quote="mmaner, post:4, topic:40689"]
you need at least 6s to reliably run detections.
[/quote]

I've had VESC-Xs reliably detect at 4S but yeah, i wouldn't do anything under 6S anyway because you can't really build a board with 4S and expect it to do anything but hold all that 8 gauge wire for all the current you'll need to overcome that lame ass voltage.
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-12-11T20:14:44.443Z Reads: 52

```
LOL I deserve that. I'm a wrench throwing hot head and tyrannically passionate at times. Ask @chaka. Sometimes i have to call him and tell him "fuck this fucking fuck-boy bro he's being a fucker" and then he calms me down and we talk about esk8 racing and stuff for four of five hours and then our wives get mad and give us the "get the fuck off the phone and build some money" eyeball. 

Never to noobs.We have to welcome them, let them settle into themselves, and then if they're jerks we tear into them then later when they're ready for it. 

And yes, when somebody walks into my house (this forum) and kicks my dog then demands a milk bone, i'm going to fuck them all up, you better believe it. I love this community. Probably more than is healthy.
```

---
## \#11 Posted by: chrisongtj Posted at: 2017-12-11T23:41:01.633Z Reads: 30

```
I use a small battery like 3 or 4s first time i power up. This ensures it's less dangerous if there are any wiring faults. I also connect the USB to the vesc to make sure it's working. 

I use full battery power (the actual pack, in your case 9s) before doing detections as the voltage will affect your motor speed.
```

---
## \#12 Posted by: Samuele00 Posted at: 2017-12-12T16:33:14.884Z Reads: 13

```
     thaks you  :)
```

---

# Lunch runner single 6374 build

### Replies: 14 Views: 829

## \#1 Posted by: Idle Posted at: 2018-03-09T19:23:53.906Z Reads: 179

```
I need direction.

Currently:
40" double kick deck (Shorty later) 
10s3p 25r with charge only bms
Focbox
6374 170kv sensored from es8 .de (10mm shaft)
Marcmt mount with idlers
Caliber 44°
1/4" risers
15/36 15mm belt
Was 97mm abec 11,, not enough torque
Now 83mm...meh.
Gt2b mad monkey complete

I'm a little underwhelmed with the performance.
I know I don't have a lot to go on, but I do know it's slow.

**Slow to accelerate, and lacking torque for even small short hills.

As is, it seems it's not going to work well for its intended purpose, the lunch runner...i.e. Leave my truck at the job site, go find food, eat and return in 30-40 min.

It's usually only around 2-3 miles or so to wherever sounds good.

I was hoping (on the 97 abec')..for around 25mph/40km cruise speed with 28-30 mph top.

The basic calculator says 25mph max speed unweighted on 83mm, and it feels like it might do that on a full charge.


Issues:
The mount, motor, belt and 36t pulley are way too close to the ground on 83mm wheels and will no doubt scrape often.
I really want to use the 97's that I have, but could buy some 90mm wheels I guess.
Smallest motor pulley I can find is a 14t pulley with 10mm bore from beltingonlinedotcom



Direction, I need some.

Any positive experiences with single drives in regards to bunny hills, i.e. 8-10% or 5-6°? 

In other news, 
I've got 107's and a Hummie's maplecarbonbamboo deck, and need to start collecting parts for it as well.










![IMG_4835|342x500](upload://oxqJTCK6f8YaGKXF74VIJaggskB.JPG)


![IMG_20180131_200415|666x500](upload://rz0G4Wi1XEcpWfSQMmgmto2XxjH.jpg)

![IMG_20180131_200400|666x500](upload://a0VP5lkIECRDAjlk7qNopvFv1x3.jpg)
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-03-09T19:34:36.864Z Reads: 151

```
I think you`re asking for help, no?
```

---
## \#3 Posted by: Idle Posted at: 2018-03-09T19:39:49.765Z Reads: 152

```
Yes.

I have no idea what I'm doing.
```

---
## \#4 Posted by: Blasto Posted at: 2018-03-09T19:42:37.236Z Reads: 150

```
did you do a BLDC motor detection? 

you can up your motor max to 60A.

you Maximum pulse width seems very high, I would expect a value around 2.00 ms (this is probably the root cause of your underwhelming performance)
![image|690x454](upload://xnCriK8uwzoMQaAkFSeEDZqNv3C.jpg)
```

---
## \#5 Posted by: Idle Posted at: 2018-03-09T19:51:02.403Z Reads: 142

```
1) Yes.
2) okay, thanks.
3) thanks again.

I'll try to get to a computer.

[quote="Idle, post:3, topic:48631"]
I have no idea what I’m doing.
[/quote]
```

---
## \#6 Posted by: Idle Posted at: 2018-03-16T22:54:58.067Z Reads: 117

```
Well, my FocBox popped and the magic smoke came out.

Idk what happened. Using vesc tool.  Sean, @squishy654 was setting it up. Going through motor detection when it happened I think. I don't really know more than that. 


 ![IMG_4899|375x500](upload://h5q1OWP46zp0sdLFn9vcr6jnwWR.JPG)


![IMG_4896|375x500](upload://gy2pCVBDfplYghrQ59fdHy4QFbR.JPG) 

It's a $150 paperweight now I guess.


Sean had a spare vesc in a drawer but didn't have the  correct bullets to hook it up to the original motor, so he hooked me up with a 125kv motor and set it up on foc.

 ![IMG_4902|375x500](upload://aMO3uky6OdFf3XVxsL5Ta8EQrk8.JPG)

And up and running. It was unbelievably quick on 83's and even on 97's it gets it. I'm at 210# and it pushes me up the hills well, even accelerating up the mild ones.

Calc says 20mph, plenty fast for now. Depending on how It gets on with longer hills, I may go to a 18t (25mph top)

Still haven't got a valid enclosure. I need to make one.
I tried, but not hard enough 😂 

![image|375x500](upload://9PvcSSTIlJ8egdHkPNX9Nzeom0e.jpg)


Need to pick up a few things, then I think the pvc or 3/32 abs might do what I want without vacuum.
```

---
## \#7 Posted by: Deckoz Posted at: 2018-03-17T15:23:46.771Z Reads: 100

```
@squishy654 what happened with the focbox man?

Looks like a fet burned... Make me think his old motor was shorted... Have you checked the resistance between phases of the old motor to verify if it's shorted or not?
```

---
## \#8 Posted by: squishy654 Posted at: 2018-03-17T15:53:56.431Z Reads: 90

```
It appeared to me like something metallic had fallen in the holes near the phase wires and shorted out between 2 connectors on a fet.  It powered up just fine but when we went to do the wizard and the tests it immediately smoked
```

---
## \#9 Posted by: Deckoz Posted at: 2018-03-17T16:22:34.987Z Reads: 89

```
Shame. Should still be under the 60 day warranty no?
```

---
## \#10 Posted by: Idle Posted at: 2018-03-17T16:37:31.934Z Reads: 87

```
Got it in sept, from a reseller.
```

---
## \#11 Posted by: barajabali Posted at: 2018-03-17T16:43:05.052Z Reads: 82

```
Hey man,

Send that focbox to me and I’ll have it repaired/replaced. We want to have you riding with some quality components
```

---
## \#12 Posted by: Idle Posted at: 2018-04-19T18:48:43.440Z Reads: 60

```
Thanks for the offer @barajabali ...I'll get it in the post if you're still game.

Board is working well, have made 3 lunch runs so far, and a few cruises around town. 

Had a get-off a few min ago...at full throttle, heading to lunch. the power cut off with no warning. Idk what it was, but it's happened a few times. 

I think I just gave up and jumped off, honestly, as tame as it is, I should be able to stay on it with a chopped throttle, gonna try and practice that. 


The PG&E guys saw it and were impressed that I ran it out.
It was many quick steps and I scrubbed enough speed to fall safely, not a scratch..




![IMG_5261|666x500](upload://iX7llqiXXKxNMiCpfEiJoWlYFHw.JPG)





![IMG_5014|375x500](upload://fTInchQ8E3IqR6FxgLWXshACqnn.JPG)![IMG_5146|375x500](upload://kzFGmBQ7U1DEiMdq2ZkObIRlgMK.JPG)![IMG_5141|666x500](upload://fK08wVryAyl5aktU1WLShHADP6w.JPG)![IMG_5181|374x500](upload://blrCKG6WAnkkqKHXkPAOGybK8kP.JPG)
```

---
## \#13 Posted by: Idle Posted at: 2018-04-19T19:36:37.847Z Reads: 55

```
[quote="Deckoz, post:7, topic:48631"]
Have you checked the resistance between phases of the old motor to verify if it’s shorted or not?
[/quote]

Yes, but it was a month ago.

I don't remember what the values were, but they were about the same. 

I'll check again..but not sure what I'm looking for..

In addition to the phase wires, ammirite that It should have no continuity between any phase wire and ground, i.e. motor housing, correct?
```

---
## \#14 Posted by: Deckoz Posted at: 2018-04-19T19:48:35.496Z Reads: 52

```
[quote="Idle, post:13, topic:48631"]
no continuity between any phase wire and ground, i.e. motor housing, correct
[/quote]

Yes no continuity. If there is then the epoxy on the stator or enamel on windings has broken an allowed a short.
```

---

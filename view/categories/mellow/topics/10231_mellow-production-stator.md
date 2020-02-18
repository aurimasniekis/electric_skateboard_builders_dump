# Mellow production stator

### Replies: 22 Views: 3602

## \#1 Posted by: Mellow Posted at: 2016-09-27T15:46:57.456Z Reads: 247

```
Hi guys, here's a slightly different photo than the prototype one for the update. @Hummie, despite the transparent plastic (which serves another purpose), that was actually a fully functioning stator. 

Kilian didn't just say "it's a hub motor, so it spins better than belt drives" like cogging isn't a thing. He went one step further and reduced the gap between the stator teeth ends to almost nothing. So how did he get those fat energy efficient windings onto the armature? Look closely, and you'll find the answer.

<img src="/uploads/db1493/original/3X/0/7/0720fe0433047f9c522fe3e3d1800c6ea251c36f.jpg" width="666" height="500">
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2016-09-27T16:57:32.823Z Reads: 235

```
Are you referring to the lock/end ring plate on the stator? And by removing it all the stator teeth would come loose?

I'm still thinking that how did they wound it up... Because it would have to retain the same geometry while winding it, or it might else have some loose wire if the stator teeth are far apart while winding them and them bringing them together and locking them with the end plate.
```

---
## \#3 Posted by: Blasto Posted at: 2016-09-27T17:01:43.878Z Reads: 230

```
very nice design!

i'm guessing they wound each phase individually on a jig, then disassemble from the jig, keeping the windings in place and reassemble all 3 phases together to get the tightest assembly possible.
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2016-09-27T17:10:09.554Z Reads: 221

```
Something like that very possibly, because the strip-able stator doesn't really make sense otherwise. Maybe those little bends seen on every second winding are what is left of the "slack", so they can actually put the winding in place. Would be interesting see the other end of the stator.

But all in all this method get more copper on the stator, increasing the motor's Km value.
```

---
## \#5 Posted by: Blasto Posted at: 2016-09-27T17:16:01.990Z Reads: 216

```
[quote="SimosMCmuffin, post:4, topic:10231"]
Would be interesting see the other end of the stator
[/quote]

I agree, @Mellow :)
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2016-09-27T17:26:22.373Z Reads: 214

```
It also makes sense for the ends of the stator teeth to have that plastic end bit, because it spaces them out correctly, so that the teeth are in a straight line in relation to the center and not all wonky, if they didn't have the end cap.
```

---
## \#7 Posted by: Mikenopolis Posted at: 2016-09-27T18:10:44.651Z Reads: 209

```
(post withdrawn by author, will be automatically deleted in 24 hours unless flagged)
```

---
## \#13 Posted by: onloop Posted at: 2016-09-28T06:52:34.272Z Reads: 169

```
Off topic guys. Create another thread. This one is about a stator
```

---
## \#8 Posted by: onloop Posted at: 2016-09-28T06:55:24.685Z Reads: 128

```
5 posts were split to a new topic: [Mellow kit prices](/t/mellow-kit-prices/10271)
```

---
## \#14 Posted by: Mellow Posted at: 2016-09-28T23:09:31.701Z Reads: 139

```
It's also about the little stator tooth that could...

<img src="/uploads/db1493/original/3X/e/6/e6d904b8075af4521c8a6608895c769fbf88935b.jpg" width="588" height="500">
```

---
## \#15 Posted by: Hummie Posted at: 2016-09-29T00:31:08.071Z Reads: 132

```
Ooo.   Neat.  Different.   So the stator is partially plastic or is the plastic removed at the end?  
 

It seems like a really nice board.  The motor.  The esc.  The stator especially is radically different than anything I've seen in the hobby or skate world. 

  This being a DIY forum a lot of us are used to a lot more power and speed than any of the production boards and it's still a question.   The max speed surely is a lot slower than DIY and that's cool and there's a lot of people who don't want to go fast but power is always wanted.  How do you limit the power?  Especially with hub motors they will get hot if enough amps are put in.  Do you have a temp sensor that will decrease amps when the motor gets hot or is it set in the esc as a continuous max amp limit?  What happens if you try to go up a mountain?
```

---
## \#16 Posted by: Mrmoonlight Posted at: 2016-09-29T01:23:32.844Z Reads: 128

```
Nice!!! That's impressive.
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-09-29T06:23:13.436Z Reads: 120

```
@Mellow
Thank you for being  so honest and informative! You have developed a really nice board and you are willing to share R&D information with us! Not many companies are that kind!

Thank you very much!
```

---
## \#18 Posted by: Sharkface Posted at: 2016-09-29T06:37:11.730Z Reads: 121

```
[quote="Mellow, post:14, topic:10231"]
It's also about the little commutator segment that could...
[/quote]



Is that a hill climbing reference?

No seriously, is that commutator segment bigger than your average segment? More electromagnetism generated than an average motor?
```

---
## \#19 Posted by: HTownBomber Posted at: 2016-09-29T17:47:50.502Z Reads: 109

```
I don't see any commutator segments.  I just see stator teeth.  Commutator segments are part of brushed motors. In a brushless motor, commutation is done in the ESC.

@Mellow is bragging that they were able to minimize the gap between stator teeth, which should reduce cogging torque and motor noise, and allow for more efficient windings.
```

---
## \#20 Posted by: Mellow Posted at: 2016-09-29T18:01:54.633Z Reads: 111

```
Thanks. Correcting. Kilian left the non-tech guy the keyboard and look what happened (don't trust online translation).
```

---
## \#21 Posted by: Mellow Posted at: 2016-09-29T18:09:22.813Z Reads: 113

```
@Hummie The plastic stays - locking in windings snugly **and** protecting against abrasion, vibration, voltage surges and possible damage from the sharp edges of the laminated plates. Skateboards have to be built to take abuse, and we knew a few squirts of waterproofing spray wasn't going to cut it.

Temperature and overload situations are monitored closely. We've used extensive modeling, real world testing and hours and hours on the dyno to simulate all types of use cases climbing long hills, multiple hard acceleration with overload, high amp boost scenarios. 

@DeathCookies Nice try, China. We know you are taking notes. 

@Sharkface Not sure what you are asking, but size is just a single parameter among many that all influence each other.
```

---
## \#22 Posted by: DeathCookies Posted at: 2016-09-29T18:11:57.153Z Reads: 109

```
Ofcourse China will copy good designs :D they did not Come over here to e. G. Photograph our car motors :smiley:
Btw, i am not from China, actually from germany too ;)
```

---
## \#23 Posted by: Mellow Posted at: 2016-09-29T18:21:28.910Z Reads: 105

```
Where exactly?
```

---
## \#24 Posted by: DeathCookies Posted at: 2016-09-29T18:39:53.588Z Reads: 104

```
Münster.
I would be glad to meet your team but i dont know when i will get to Hamburg :(
```

---
## \#25 Posted by: HTownBomber Posted at: 2016-09-29T19:07:52.864Z Reads: 101

```
Nice response. I gotta say I'm really impressed with all the R&D going into this. German engineering is no joke. I love the idea of a really solid, tightly wound motor with minimal cogging and dynamic temp/load monitoring. Using thicker wire makes sense as a way of minimizing resistance but it also raises the Kv. Curious about how you guys are managing that.
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2016-09-29T21:31:09.748Z Reads: 97

```
After looking closer at the first post stator picture, I estimate a single tooth winding to have ~21-22 turns.  
My SK3 has 18 turns and a kV of 149.

I'm throwing an uneducated guess about the kV being around 150. Based on the winding turns, guessing the wire gauge, and a diameter  around 65 mm.
```

---

# Landwheel VESC swap

### Replies: 3 Views: 591

## \#1 Posted by: jaysleezzyy Posted at: 2017-07-27T16:29:03.077Z Reads: 67

```
Has anyone attempted to swap the entire electrical board on the LandWheel with a  VESC?

I assume its possible and would like to try it my self when i get some extra cash.
```

---
## \#2 Posted by: Mikenopolis Posted at: 2017-07-27T16:44:34.568Z Reads: 61

```
I think PK did it and blew something. Read it in the private chat, it's there somewhere
```

---
## \#3 Posted by: Mikenopolis Posted at: 2017-07-27T17:28:17.375Z Reads: 58

```
Went to look for the post and realized you were not invited to that old private thread. PK started a new one which you are part of now. Anyway, I'll repost what he played with below:


----
@pkasanda 
Thanks for the update. FYI my VESC experiments failed six different ways:
1) Sensor detection failed
2) 36 volt Dual VESC BLDC V4 Hubs took off like a drag racer complete with wheely. The power was completely unmanageable off the start. It was an un-ridable board.
3) 36 volt FOC blue my vescs. Wheels up the motors alternated between forward and reverse without changing remote directions...then one or both of my VESCS blew.
4) All experiments resulted in stuttering starts. Not one of them produced acceleration as smooth and predictable as what I experienced with the V4 Landwheels

So, the $200 lessons learned are as follows:

1) VESC does not seem to be a viable solution.
2) The Existing Landwheel ESC seems to be much closer to good product than any of the VESC experiments. Hence focusing on programming an eloquent braking strategy for the L4 Circuit board seems to be way to go. Simultanelusly Landwheel needs to figure out why three of the L4 circuit boards have stopped working within just a few days of use. 
2) Higher Voltage seems to be a big factor in sudden braking. Lower voltage applied to braking may be a viable strategy.
3) Large hub motors seem to grab hard at low RPM. Hence, the solution to unpredictable braking may be voltage curve that tracks to wheel speed.
4) Simple braking strategies are not likely to work. For example a sudden transition from one braking strategy to another seems unlikely to succeed at keeping the rider safely on the board.
5) Two large hub wheels seem to land on a locking point and this may be due to both hubs simultaneously aligning with the sweet spot on the magnets. Part of a successful braking strategy may be to enforce a small phase shift in the braking force to both wheels. If this could be accomplished well, the outcome would be two wheels worth of braking force with half the pulsation and perhaps without the sudden locking problem.
6) Looking from the outside in, it seems like the Landwheel programers spent a long time developing a sine wave algorythm for smooth acceleration but very little time developing a square wave algorythm for braking. Square wave braking seems like the wrong approach to solve a problem of sudden wheel lock.

pk
---
```

---

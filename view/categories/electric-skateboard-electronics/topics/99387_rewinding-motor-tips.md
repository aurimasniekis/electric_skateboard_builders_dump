# Rewinding motor tips

### Replies: 26 Views: 392

## \#1 Posted by: whaddys Posted at: 2019-07-30T07:39:19.837Z Reads: 94

```
I wanna try my hand at rewinding a fried motor.  It's a maytech 6355.  I've read a handful of articles and watched videos but have a couple questions here.  One: how do I remove this PCB top?  

![IMG_5277|375x500](upload://isUC7ZoorxcSijuFaJQaBMoXx9o.jpeg) 

Two: Theres some glue/adhesive around some of the coils, is there something I can soak this in to remove the glue and keep everything in tact?  Acetone?  

![IMG_5276|375x500](upload://dzKup3gTs9hnoJklyNcjVfZNIvQ.jpeg) 

I read on an old thread that someone put it in the freezer with penetrating oil to get the stator out but I'm still not sure how to remove that PCB board on top or how that functions exactly with the motor as a whole unit.  Any tips welcome, thanks.

@MysticalDork I feel like you may have some knowledge...:sweat_smile::sweat_smile:
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-07-30T07:59:12.965Z Reads: 87

```
@whaddys  I'd guess the PCB is held in by that aluminum piece with flats on it. Looks like it's threaded on.

As for removing the windings, I've seen people use solvents, heat, brute force or a combination. It's not easy to do when they've been glued in securely like that.
```

---
## \#3 Posted by: whaddys Posted at: 2019-07-30T08:02:39.287Z Reads: 86

```
Is there any particular consideration/danger in soaking it in acetone?  Also do you know what purpose that PCB serves?  It seems to be in all the 63xx motors I've seen but not in smaller ones.
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-07-30T08:18:15.507Z Reads: 78

```
The PCB holds the hall sensors and usually a thermistor too. 

Acetone will probably be okay, it might take the epoxy off the steel laminations, or not. Might not even soften the epoxy on the windings, for all I know. Be careful with solvents, they're usually flammable and volatile. Really easy to have a fire.
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-07-30T08:32:47.756Z Reads: 76

```
I know when I was rewinding a transformer, it had been dipped in some resin or other that made it impossible, so I resorted to cutting off the protruding windings, then pounding out the remainder in the grooves with a punch and a hammer. It was a slow, labor intensive but very satisfying process. :smiling_imp: 

If the acetone does remove the epoxy on the windings, it will probably remove the epoxy on the laminations as well, and it may turn back into a pile of individual laminations that need to be assembled again. If so, remember to insulate them before reassembly - ideally you want no electrical continuity between each lamination and its neighbors. They usually are coated wit ha thin layer of lacquer before being assembled.
```

---
## \#6 Posted by: whaddys Posted at: 2019-07-30T08:36:32.337Z Reads: 73

```
Do you mean the lamination on the stator, so there's no continuity between the stator and the phases?  I read an article saying to coat the stator with liquid paper.
```

---
## \#7 Posted by: MiniChopper4Me Posted at: 2019-07-30T11:52:58.124Z Reads: 57

```
The material the motor is dipped in is an epoxy. I don’t think it will respond well to acetone, but more importantly like @MysticalDork said, you’re likely to take more apart than you really need to. You’ll want to know the number of turns and gauge of the wire used to wind the motor before you rewind it in order to have the right material for the job, and the pattern used to wind and terminate the wire is key as well.
```

---
## \#8 Posted by: MiniChopper4Me Posted at: 2019-07-30T12:03:04.895Z Reads: 60

```
If you look at your second pic, each layer of metal making up the stator is a separate piece of metal.  Those are the laminations. The whole thing usually doesn’t separate into laminations unless you do something to unglue them, like use a solvent.

What you read, about using liquid paper, is to avoid creating a short between the wire you are winding with and the laminations/stator.  This is common at the corners where you bend the wire around, as these edges can be sharp and cut the wires coating.  The whole stator is usually coated with a baked on powder coating that makes the surface less sharp at those edges.  Again, you might find that acetone removes this material.
```

---
## \#9 Posted by: Hummie Posted at: 2019-07-30T16:09:21.758Z Reads: 53

```
heat works well for softening the winding epoxy and then unwind if you can or cut.  
don't pull so hard that you pull up the stator laminations at the top and bottom of the stator. 

if you do end up with a bare edge that the rewind will have to go over its difficult to get a good coating of a resin that will stay on and might be easier to use tyvex paper or something.  usps has the envelopes for free and glue it over the bare spot.  you have to get all spots the wire goes over covered or its easy to short and you will be pisssssed.

if the lrk winding will fit that is an awesome easy winding.  and if terminated wye a hair better

its a nightmare trying to figure how many turns and wires are in parallel and easier to get it all off without thinking about it in my experience, carefully, and just rewind first with a super thin wire that will be easy to put on and you can test the kv, figuring how many turns you really want, and then rewind with the thickest wire that will do it for you.  maybe you know this already.   and youre going to want to put another layer of resin back on after winding and fix down all wires 

its hard to tell if your motor rewind is wound without shorting either to other phases or within the phase or to the stator (which isn't a complete short but a half short and not too bad).    a resistance test with a multimeter will tell only so much and a good inductance meter is the easiest way to see it all and you can get them for like 20 bucks.  L/C meter

im pretty obsessed with winding motors. if you want to talk about it you can message me..or I could clutter the site up for days
```

---
## \#10 Posted by: whaddys Posted at: 2019-07-30T18:42:08.483Z Reads: 45

```
hell yeah thanks @Hummie, you will most certainly get a PM from me over the next week I'm sure!  I was going to count the windings and pay attention to the pattern when unwinding but I may just arbitrarily cut off the wire and do a whichever winding is easiest, lrk you say?  I haven't read about that winding pattern yet only delta and wye.

I think I'll pass on the acetone as to not potentially fuck up the laminations.
```

---
## \#11 Posted by: Hummie Posted at: 2019-07-30T18:53:03.446Z Reads: 45

```
lrk is the winding and wye is the termination.  lrk is failproof as youre winding every other tooth only, strangely, and you just wrap the tooth, filling the two slots beside, with as much as you can and you don't need to make considerations for the windings beside.
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-07-30T20:51:23.748Z Reads: 41

```
[quote="whaddys, post:6, topic:99387"]
Do you mean the lamination on the stator, so there’s no continuity between the stator and the phases?
[/quote]

That, and if the individual laminations come apart, you should insulate every one of them from their neighbors If it were me, I'd probably use some insulating epoxy spray I discovered at my previous job. You want no electrical continuity between your wires and the stator, and if you put one multimeter probe on say the top layer and the other on the next layer down, you should get no continuity there as well. (Some continuity is usually unavoidable due to friction and scraping as you reassemble the layers, but you want to absolutely minimize it.)
```

---
## \#13 Posted by: whaddys Posted at: 2019-07-30T20:56:22.694Z Reads: 35

```
Ideally I don't want these individual laminations to come apart though I'm guessing, correct?  Seems like that would save me quite a headache (or learning experience depending how you wanna look at it =/)
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-07-30T21:12:37.628Z Reads: 35

```
That is correct. if they come apart it's not the end of the world, but it can be a bit of a pain.
```

---
## \#15 Posted by: whaddys Posted at: 2019-07-31T22:35:34.328Z Reads: 29

```
Is 18awg acceptable for rewinding?
![image|375x500](upload://dO4RSClMBQQVqqVG3FG85al8MV7.jpeg)
```

---
## \#16 Posted by: MysticalDork Posted at: 2019-07-31T22:48:57.746Z Reads: 28

```
@whaddys  You have to calculate the space you have and the number of windings you want and pick the wire size that fills as much space as possible without being too much.

Don't use that wire at all though - it's not insulated, it's bare copper.

Also, it's usually easier to use multiple thinner strands than one fat one, because it's less of a pain to bend.

I thought you watched a bunch of rewinding videos? This is all basic stuff that should have been covered from the get-go!
```

---
## \#17 Posted by: whaddys Posted at: 2019-07-31T22:52:30.912Z Reads: 28

```
Hahah no I did not read anything other than thicker wire for higher KV.  Clearly I need to do more HW.  THANKS @MysticalDork if you have any essential literature you  can send my way I’d love the reading material.
```

---
## \#18 Posted by: whaddys Posted at: 2019-07-31T23:07:22.467Z Reads: 28

```
I guess I’ve read more about specific winding types and terminations, and how they affect motor performance. Nothing about the electrical physics behind it though, that would obviously be good stuff to know. Essential stuff to know
```

---
## \#19 Posted by: MysticalDork Posted at: 2019-07-31T23:11:21.797Z Reads: 26

```
https://www.bavaria-direct.co.za/ and [https://www.emetor.com](https://www.emetor.com/) both have some pretty in-depth information about winding schemes.
 This instructable https://www.instructables.com/id/Make-Your-Own-Miniature-Electric-Hub-Motor/ also has loooots of very detailed information and links and equations and and and.
```

---
## \#20 Posted by: Hummie Posted at: 2019-08-01T00:37:04.951Z Reads: 25

```



you strip it yet?

I would skip calculations based on your measuring of space as its hard to really measure accurately and the difference between wire sizes is small.  Easiest is just do the lrk winding with any thin insulated wire (magnet wire being best) quickly and give it a spin on the bldc tool to make sure you got the winding done right and you can see what the kv is.  Then when you figure how many turns of wire you want, for your desired kv, find a wire that you can wind that will be thick enough that it just fits in and does that.   

you can put a very thick wire on by tying the end to a hook and pulling it on from the other end. I find doing multistrand a pain and its unlikely to yield as much copper fill or give as nicely made coils that produce as good a field.  count how many turns are on a tooth from the opposite side the wire ends and starts are.  the goal is of course least electrical resistance for most inductance, so fat wire in nice coils.

with the amount of space in that motor case you have lots of room for the endturns, or copper sticking out the top and bottom of the stator, and I'll bet you can jam the can with a huge amount of wire.  it will be bulging so much I bet the sensor board maybe would be a limitation.  id forget putting it back on if so but to each their own.  

you cant see what the electrical resistance of the motor is now, or maybe someone else has one and you could find out (wouldn't trust the manu number) and you could compare it to what you end up with as shown also on the bldc tool.   or weigh the motor now and weigh it after you strip it and weigh it after you rewind.
and you'll want some thin high heat epoxy to fix the windings down.  Id get omega brand unfilled stuff in the envelope as its easy, heat it up to make it thinner, and try to get it all in there as best you can. and make sure where the wires come out of the motor is well protected.
```

---
## \#21 Posted by: MiniChopper4Me Posted at: 2019-08-01T14:32:21.728Z Reads: 19

```
[My thread on rewinding a motor](https://www.electric-skateboard.builders/t/rewinding-90mm-hub-motor/80491).

The motors I rewound are on my esk8 still running with no issues.  I never dipped mine in epoxy, in case I wanted to rewind them again.  I'm *really happy* with the results.
```

---
## \#22 Posted by: whaddys Posted at: 2019-08-01T18:37:50.946Z Reads: 18

```
wow, thanks a ton @MysticalDork @Hummie @MiniChopper4Me.  I haven't started unwinding yet the motors just been in the freezer with penetrating oil for a couple days now because I've been busy working.  @Hummie are you saying you would just rip the PCB off and run it sensorless?  Because if so that is probs what I'll do!  Will start on this probobly tomorrow since I'm working again all night.
```

---
## \#23 Posted by: MiniChopper4Me Posted at: 2019-08-01T19:58:31.918Z Reads: 16

```
Thicker wire does not yield more kv,  fewer turns does.  Make sure to read the stuff @MysticalDork linked, I'm sure your chances of succeeding will be much greater the more informed you are before you start.
```

---
## \#24 Posted by: Hummie Posted at: 2019-08-01T20:13:47.120Z Reads: 16

```
I would just rip it off.  easier and I find the vesc works well without a sensor and one less thing to break
```

---
## \#25 Posted by: MysticalDork Posted at: 2019-08-01T20:45:43.176Z Reads: 14

```
If you can get the sensor board off without breaking it, might as well put it back on and use it until it breaks. Most people run in sensored hybrid mode anyway, so the sensors are only used at low speed anyway. While it's true that a sensor failure can cause the vesc to brake, it shouldn't occur at high speed. (I haven't tested this, so take it with a grain of salt.) I like sensors because it improves performance starting on hills etc.

Like MiniChopper said, wire size has no direct effect on KV - only the number of turns. More turns makes the KV lower because it increases the strength of the magnetic field. 

But more turns do take up more space, so there ends up being an indirect effect on wire size, because you physically can't fit a bunch of turns of fat wire.

This is also the reason that, all other things being equal, a higher-KV motor will have a higher peak power output - the resistance of the fatter, lower turn coils is lower, so you can shove more power through them before they overheat. The downside is that you reach the ERPM limit of your controller sooner, and depending on the controller that can do bad things.
```

---
## \#26 Posted by: whaddys Posted at: 2019-08-01T20:51:17.506Z Reads: 14

```
Oh yeah, I said that backwards woops I knew that I swear!  Definitely gonna read up on all that literature tho thanks again
```

---

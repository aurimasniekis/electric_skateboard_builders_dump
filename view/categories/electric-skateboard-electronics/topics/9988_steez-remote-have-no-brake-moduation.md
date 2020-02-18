# Steez remote have no brake moduation?

### Replies: 26 Views: 1749

## \#1 Posted by: Hummie Posted at: 2016-09-22T17:02:28.774Z Reads: 127

```
maybe something can be done in the settings but I cant get the brakes to decrease when going downhill.  once I reach a harder level of braking I cant scale it back but have to release the brakes and then apply them lightly.  very annoying.  is this solvable?  it's a good remote otherwise.
```

---
## \#2 Posted by: chinzw Posted at: 2016-09-22T17:14:56.210Z Reads: 125

```
Thats probably your ESC/VESC throttle response. You will need to do a throttle range calibration.
```

---
## \#3 Posted by: Hummie Posted at: 2016-09-22T17:16:55.992Z Reads: 123

```
I did .  it's centered.
```

---
## \#4 Posted by: chinzw Posted at: 2016-09-22T17:18:13.108Z Reads: 119

```
So if the remote range is fine then its something in your VESC
```

---
## \#5 Posted by: Hummie Posted at: 2016-09-22T17:18:56.156Z Reads: 111

```
the vesc works fine on many other remotes.  I know of one other person who said that's just how the steez works.  do you have a steez you've used?
```

---
## \#6 Posted by: flatsp0t Posted at: 2016-09-22T18:00:03.693Z Reads: 97

```
I have this too on my raptor, i played around a bit, but i was not able to solve it.
```

---
## \#7 Posted by: Hummie Posted at: 2016-09-22T18:01:31.675Z Reads: 97

```
it sucks if youre going downhill .  I don't use it anymore
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-09-22T18:08:44.810Z Reads: 95

```
how is this a function of the remote? Does it do this when the VESC is set to brake and reverse? or does it only do it when set to reverse and no brake? 

The reason i ask is because it doesn't go in reverse in any sort of odd way. So why would it apply brakes in an odd way if the signal being sent is basically just reverse? Is braking a separate (third) signal and not just a reverse signal being treated differently by the ESC while moving forward?
```

---
## \#9 Posted by: flatsp0t Posted at: 2016-09-22T18:39:04.805Z Reads: 88

```
I use it just in current, no reverse.
But doing exactly the same with another remote (gt2b for reference), the board acts completely different.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-09-22T18:42:18.234Z Reads: 83

```
now i'm just even more confused about how remotes/receivers work in relation to the ESC. I swear as soon as i think i understand something this forum comes along and slaps me in the face.
```

---
## \#11 Posted by: chinzw Posted at: 2016-09-22T18:53:46.436Z Reads: 76

```
The remote should just send packets to the receiver with the throttle/steering position, and the receiver translates that into PPM, thats how most 2.4ghz remotes work, if there's something funky happening you can check with bldc tool and see how the ppm data is being read.
Another thing that comes to mind is that when braking, back EMF is generated, which could interfere with the signal somehow, and the steez receiver might be more susceptible than others.
```

---
## \#12 Posted by: Hummie Posted at: 2016-09-22T19:03:18.407Z Reads: 75

```
to clarify what's happening, I'm doing current and no reverse, when I'm going downhill i cant lessen the brakes.  once I make them engage strongly there's no coming back to just a little and I have to completely release the brakes and then apply them again to get slighter braking
i know evohyax has the same issue and accepts it as just how the steez works.  we've both done as much adjusting as possible on the bldc tool but I havent seen what's going on in real time with real loads while riding or seen the ppm response
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-09-22T19:59:57.446Z Reads: 71

```
you know what's weird about this is that what your describing.. i do that anyway. That's probably why i never noticed this. When riding the brakes down a hill i tend to hold and release, hold and release, rinse and repeat. 

I did notice that there is some sort of threshold though. If you gradually increase the brake by easing into the reverse throttle position, there is a point where it acutely begins to brake harder after it has already started to ease into the brake.
```

---
## \#14 Posted by: Hummie Posted at: 2016-09-22T20:31:07.212Z Reads: 70

```
its notchy on the steez when braking as you say.  maybe even accelerating but that's not as noticeable.  the brakes have like three possible degrees, mild, medium, and hard, and that's it.  the mini trigger has a smooth transition from seemingly many more possible degrees.  this is besides the afore mentioned issue.  really bummed on it and back to the trigger.  have you tried other remotes like the mini trigger?  maybe you never knew the control you were missing.
```

---
## \#15 Posted by: michaelcpg Posted at: 2016-09-22T21:56:49.314Z Reads: 70

```
I had the exact same issue with my Enertion (Steez) remote, even after calibrating the remote in the VESC settings. Ended up replacing it with a GT2B and I've never had an issue since.
```

---
## \#16 Posted by: longhairedboy Posted at: 2016-09-23T01:25:55.252Z Reads: 66

```
ugh this sucks. i love my steezes so much! guess i need to figure out how to work in some gt2b mods after all. god knows there are enough of them now. ive gott two case mods on my bench i havent even tried out yet. 

im just not a fan of anything even vaguely resembling a gun at all in any way around here. kids get shot here. cops are racist and gun happy in this part of the country.
```

---
## \#17 Posted by: michaelcpg Posted at: 2016-09-23T01:48:20.683Z Reads: 68

```
Can't imagine what having to be wary of something like that all the time must be like :/

I'm sure you would've seen the Baby Buffalo mod? 
http://www.electric-skateboard.builders/t/gt2b-baby-buffalo-mod-case-3d-printable-thumb-throttle-case/4694
```

---
## \#18 Posted by: michaeld33 Posted at: 2016-09-23T01:50:37.485Z Reads: 65

```
Benchwheel remote is still my favorite. Found it to be VERY reliable and comfortable.
```

---
## \#19 Posted by: longhairedboy Posted at: 2016-09-23T11:25:07.434Z Reads: 61

```
i thought i had seen these on aliexpress but now i can't find them. Where did you get yours?
```

---
## \#20 Posted by: Skitzor Posted at: 2016-09-23T11:47:11.088Z Reads: 60

```
Been using the Steez for 4 months now. Maybe it's a production issue but my brakes are as smooth as I could Imagine. I also have tested this with the winning remote. Exacty the same gradual and smooth braking.
Something must be off here...
```

---
## \#21 Posted by: lox897 Posted at: 2016-09-23T11:53:24.545Z Reads: 57

```
I think Miami Boards or Amazon has them
```

---
## \#22 Posted by: Luke Posted at: 2016-09-23T12:28:53.801Z Reads: 54

```
https://m.aliexpress.com/item/32731985084.html?trace=wwwdetail2mobilesitedetail&productId=32731985084&productSubject=Electric-skateboard-refitting-parts-remote-control-bench-technology&spm=2114.01010208.3.1.Qy30XB&ws_ab_test=searchweb201556_10#autostay
I emailed benchwheel and they sent me here
```

---
## \#23 Posted by: michaeld33 Posted at: 2016-09-23T12:45:20.282Z Reads: 52

```
Straight from benchwheel, through taobao. I can send you a link where you can get them thru an agent so you can get them to USA. Only like $3 extra for the agent than taobao.
```

---
## \#24 Posted by: longhairedboy Posted at: 2016-09-23T13:02:34.463Z Reads: 49

```
@oriol360 get these remotes back in stock and I'll buy a few from you. I like buying things from you and supporting your shop. 

especially your flier type e-switches, for some reason they don't seem to fail at 12S the way some other ones seem to lately.
```

---
## \#25 Posted by: Hummie Posted at: 2016-09-23T14:49:46.236Z Reads: 50

```
Skitzor you can go down hill braking hard and then easy off the brakes to a light braking?
```

---
## \#26 Posted by: Skitzor Posted at: 2016-09-24T09:25:03.383Z Reads: 38

```
Yes, without any problems
```

---

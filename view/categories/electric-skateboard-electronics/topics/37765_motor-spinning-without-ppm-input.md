# Motor Spinning Without PPM Input

### Replies: 25 Views: 665

## \#1 Posted by: GrecoMan Posted at: 2017-11-08T20:02:07.044Z Reads: 95

```
Hey guys, I started having a weird problem with my board yesterday after riding about 20 miles.  With my remote and board both turned on (failsafe set up on both correctly) the motor will now randomly spin and brake without my input.  It only happens after I ride for a bit which makes it even weirder...
https://youtu.be/R58pr5_2oAg
```

---
## \#2 Posted by: caustin Posted at: 2017-11-08T20:08:10.683Z Reads: 88

```
What happens when you cutoff the remote and leave deck on and everything else same?
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-11-08T20:08:56.123Z Reads: 86

```
same thing.  the part that weirds me out the most is that it only happens after ive been riding for a while
```

---
## \#4 Posted by: Blasto Posted at: 2017-11-08T20:14:15.175Z Reads: 83

```
two option's here

1- increase you deadband a bit, to let's say 20ms (default is 15ms)
<img src="/uploads/db1493/original/3X/d/e/de0dd5a9ae948717cf0a219a0d72e75d7ddfd9b5.png" width="689" height="175">

2- use Ack's bldctool 2.54, recenter your signal with the "center pulsewidth". Can't do that with 2.18, can only input max and min.

<img src="/uploads/db1493/original/3X/0/f/0f92aa2a0e65fa144e2b55934ca0f4637633bfca.png" width="616" height="84">

3rd not recommended: play around with your trim. (should actually put a bit on a hotglue on that)
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-11-08T20:15:03.389Z Reads: 77

```
ive got ack's tool right now lol.  used the wizard and got it perfectly at 50%

ill try adjusting deadband though, thanks
```

---
## \#6 Posted by: Blasto Posted at: 2017-11-08T20:16:28.491Z Reads: 72

```
[quote="GrecoMan, post:5, topic:37765"]
ive got ack's tool right now lol.  used the wizard and got it perfectly at 50%
[/quote]

how does your signal look when you tick the "display"?

is it bouncing all over the place or is it fairly stable (+-1ms)
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-11-08T20:20:18.634Z Reads: 72

```
its jumping from 50 to 52 every so often
```

---
## \#8 Posted by: Blasto Posted at: 2017-11-08T20:22:15.639Z Reads: 72

```
[quote="GrecoMan, post:7, topic:37765, full:true"]
its jumping from 50 to 52 every so often
[/quote]

that should be fine... motor is still twitching? hit write?
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-11-08T20:26:54.669Z Reads: 69

```
I think I may have been an idiot.  The motor pulley was rubbing against the mount... It created a pocket for itself.  I took the pulley off and no more twitching or random braking
but...
I forgot to take my key out and spun the motor so my key is probably somewhere in Narnia right now...
```

---
## \#10 Posted by: ShutterShock Posted at: 2017-11-09T00:50:49.491Z Reads: 59

```
Yeah, well, that should only affect resistance while riding?  I think there may be a different underlying issue.  Sounds like a wire is bouncing off itself or you've got interference to me.
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-11-09T01:08:08.606Z Reads: 55

```
yea not sure... I cant seem to replicate the issue anymore.  Interference isn't what I think it is, I'm using the jlabs mini and my receiver is mounted outside the enclosure.  All my connectors are fully seated and zip tied togethervso really confused lol
```

---
## \#12 Posted by: guyguy Posted at: 2017-11-09T01:44:10.644Z Reads: 52

```
Did you check your wardrobe?
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-11-09T01:45:05.411Z Reads: 53

```
yea man, went through and I was in this wintery place.  decided that I probably wasn’t gonna find it in all the snow so I turned around
```

---
## \#14 Posted by: guyguy Posted at: 2017-11-09T01:45:59.756Z Reads: 53

```
Aslan would be disappointed you gave up so early.
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-11-09T01:47:46.205Z Reads: 48

```
yea man I already had a chat with him.  he convinced @Titoxd10001 to send me a new key
```

---
## \#16 Posted by: GrecoMan Posted at: 2017-11-09T12:38:30.232Z Reads: 39

```
uuuggg still having the problem 😢
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-11-09T12:44:40.828Z Reads: 39

```
@Jinra has probably had this problem lol...
```

---
## \#18 Posted by: mccloed Posted at: 2017-11-09T16:15:30.298Z Reads: 36

```
I would suggest hooking up a different controller, if you have one. I had a similar problem with the "winning" remote that would only happen after riding for a bit. Very surprised to see this on the Mini.
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-11-09T22:19:47.772Z Reads: 31

```
rebound the controller and the weird jittering is gone!
but...
now I get Over Voltage faults if I brake to hard :cry:
```

---
## \#20 Posted by: Jinra Posted at: 2017-11-10T00:55:46.483Z Reads: 26

```
what's your max input voltage set to?
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-11-10T00:56:34.603Z Reads: 26

```
just the default 58v
```

---
## \#22 Posted by: Jinra Posted at: 2017-11-10T00:57:32.956Z Reads: 25

```
Have you checked for shorts and/or water damage?
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-11-10T00:59:51.706Z Reads: 25

```
yea never ridden through puddles or rain or anything of the sort. shorts are pretty much impossible at this point, insulated everything with kapton, hot glue, and foam.  think it’s because I was braking on a full battery
```

---
## \#24 Posted by: L3chef Posted at: 2017-11-10T09:06:20.167Z Reads: 23

```
I had similar issues back in spring. It was the positive power wire to the vesc that was loose
```

---
## \#25 Posted by: TarzanHBK Posted at: 2017-11-10T11:20:29.706Z Reads: 18

```
Still be careful with electronic mounted outside of your enclosure.
After a bit of riding time you may have debris and dirt inside everything, which also could lead to shorts or random stuff like your stuttering
```

---

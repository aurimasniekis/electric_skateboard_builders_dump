# Motor cogging after acceleration

### Replies: 11 Views: 730

## \#1 Posted by: PDXroses Posted at: 2018-01-25T08:12:46.882Z Reads: 127

```
Hey all, I’d appreciate some advice from the pros here.  I searched and searched, but gave up.  I have a dual motor VESC DIY that’s been working fine for 100+ miles. Then I rode over some really rough surfaces with loose motor mounts jiggling for a few miles. 

Now my left motor cogs on acceleration. I push start (unsensored) and throttle it gently. Right motor does fine as expected. The left motor stutters. I release the throttle and reapply acceleration and it works. It happens randomly. Could it be that I damaged the motor?  Connection issue?  The Vesc?

Any help would be very appreciated!
```

---
## \#2 Posted by: scepterr Posted at: 2018-01-25T08:15:23.245Z Reads: 126

```
Did you check your connections? Phase leads at motor exit?
```

---
## \#3 Posted by: PDXroses Posted at: 2018-01-25T09:33:18.552Z Reads: 109

```
Do you know how I could check them for problems?
```

---
## \#4 Posted by: scepterr Posted at: 2018-01-25T09:34:21.564Z Reads: 107

```
Make sure no tears in insulation, no cold solder joints, stuff like that
```

---
## \#5 Posted by: DanSkates Posted at: 2018-01-25T09:42:59.053Z Reads: 99

```
I had a very similar issue after to many cobbled paths and found the issue to be 2 phase wires crossing. Have a read of my thread to see if it might help:

http://www.electric-skateboard.builders/t/r-spec-given-up-the-ghost-fixed/28758
```

---
## \#6 Posted by: Lumaci Posted at: 2018-01-25T10:33:27.053Z Reads: 92

```
I had the same issue, turned out to be a shorted motor.
```

---
## \#7 Posted by: PDXroses Posted at: 2018-01-25T10:45:58.843Z Reads: 86

```
Thanks dude glad to know I’m not the only one :slight_smile:
```

---
## \#8 Posted by: JonathanLau1983 Posted at: 2018-01-25T12:17:55.146Z Reads: 80

```
I had a similar thing, turns out two of my phase wires had sheared where the cable was soldered onto the bullet connector. I've since added a clamp of sorts to stop movement at this part and no issues since.
```

---
## \#9 Posted by: SeanHacker Posted at: 2018-01-25T14:13:49.757Z Reads: 74

```
@PDXroses I had the same problem a few months back with some R-spec motors just like mentioned above. I had to open them up and put some shrink tube on the phase wires and I haven't seen the problem since. Should hopefully be an easy fix for you. ;)

If your screename is a hint at the city you live in, let me know if you ever wanna meet up for a group ride with a few others here in Portland. That is when this rain stops!
```

---
## \#10 Posted by: PDXroses Posted at: 2018-01-27T09:46:42.123Z Reads: 48

```
Guys, I found the problem. I think. I recorded the motor turning in slow motion and saw that it and half the motor mount was bending towards the wheel on start up.  Cheap/thin mounts. After realigning the mounts, the low speed, “random” cogging vanished. I suspect the slight bend on start up caused the motor to  commutate improperly and cog. If this is indeed what was happening, then it makes sense that it only happened during heavy acceleration and not when I was well in motion.

If this theory is shit and the motor cogs again, I’m throwing it in the nearest lake. Haha.
```

---
## \#11 Posted by: PDXroses Posted at: 2018-01-27T09:52:56.508Z Reads: 44

```
Awesome. Counting down until the rainy season ends.
```

---

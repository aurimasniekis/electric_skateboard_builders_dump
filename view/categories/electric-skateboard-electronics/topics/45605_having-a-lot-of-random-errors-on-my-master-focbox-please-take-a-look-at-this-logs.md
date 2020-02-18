# Having a lot of random errors on my master FocBox, please take a look at this logs

### Replies: 16 Views: 725

## \#1 Posted by: Eboosted Posted at: 2018-02-05T06:22:21.522Z Reads: 168

```
Can someone tell me if this behavior points to a dead mosfet or an almost dead DRV?

![image|351x500](upload://85HEogDy7CRtn32NAvaZPurLZv7.png)

As you can see from the logs, all current and power goes to zero but the duty cycle keeps staying constant, that means the cutouts ocurr while I'm keeping the throttle pressed, of vourse the cutouts are more noticeable on hard acceleration or hard braking.

@JohnnyMeduse any input?

BTW the problem is way more frequent  in FOC, I've been runing flawlessly FOC for months before this issues started
```

---
## \#2 Posted by: dg798 Posted at: 2018-02-05T14:12:17.394Z Reads: 131

```
Check the led when you push throttle. Does it blink red while pushing throttle?
Whatever you do do not run motor detection while this problem is occurring, if you do there is a high chance you will short your motor!
```

---
## \#3 Posted by: Eboosted Posted at: 2018-02-05T17:10:16.512Z Reads: 116

```
The led on the remote does not blink, I have a solid RC conexion, this issue is beyond that.
```

---
## \#4 Posted by: dg798 Posted at: 2018-02-05T17:15:32.521Z Reads: 115

```
No I mean the led on the focbox. Usually if you push the throttle and there’s a drv error the led on the vesc will stay solid red when the throttle is being pushed. If there was no drv the led on the focbox would be a solid greenish color.
```

---
## \#5 Posted by: Eboosted Posted at: 2018-02-05T17:33:18.096Z Reads: 114

```
[quote="dg798, post:4, topic:45605"]
the led on the focbox. Usually if you push the throttle and there’s a drv error the led on the vesc will stay solid red when the throttle is being pushed. If there was no drv the led on the focbox would be a solid greenish color.
[/quote]

Unfortunatelly the errors do not ocurr on the bench, only under load when the board is being riden.

Here is a sreenshot of the errors I got from the VESC Monitor:

[img]https://i.imgur.com/Kgmjm9O.png[/img]
```

---
## \#6 Posted by: dg798 Posted at: 2018-02-05T17:34:04.990Z Reads: 108

```
Can’t see pic
```

---
## \#7 Posted by: dg798 Posted at: 2018-02-05T17:37:22.478Z Reads: 109

```
Also if it occurs only under load then the chance of it being a drv error are a little lower as usually it won’t work at all even under no load. Also if you type in “faults” to terminal in the bldc tool, it will tell you your errors as well.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2018-02-05T17:46:59.879Z Reads: 108

```
These are not errors. It is the acceleration measurement which get's recorded when you press on the speed box.
When you start the app you can see the errors of all vesc if they are connected by CAN while reading the data of the master. If you don't see errors at startup  then there are no none. So it is best to restart the app after you experienced the cutouts.
If you can't find any then it is very likely that your remote has cutouts.
```

---
## \#9 Posted by: Eboosted Posted at: 2018-02-05T18:27:25.642Z Reads: 95

```
I was able to get this error logged:

[img]https://i.imgur.com/wR4mZqx.png[/img]
```

---
## \#10 Posted by: Eboosted Posted at: 2018-02-07T06:12:53.238Z Reads: 70

```
I found the problem:

[img]https://i.imgur.com/h1SMgQg.jpg[/img]

@JohnnyMeduse is this repairable?

I installed a new FocBox and the board is a fucking rocket again!
```

---
## \#11 Posted by: PXSS Posted at: 2018-02-07T06:21:11.615Z Reads: 68

```
Clean it up forst with some denatured alcohol. It's hard to see if the trace survived under the burn. Half of C49 is gone... Wonder what did that...
```

---
## \#12 Posted by: Eboosted Posted at: 2018-02-07T06:26:18.761Z Reads: 68

```
Here is a closed up picture

[img]https://i.imgur.com/PPiyNCV.jpg[/img]
```

---
## \#13 Posted by: b264 Posted at: 2018-02-07T07:22:24.974Z Reads: 62

```
[quote="Eboosted, post:5, topic:45605"]
Unfortunatelly the errors do not ocurr on the bench, only under load when the board is being riden.
[/quote]

Bolt a 25lb [gym weight](https://www.youtube.com/watch?v=QHRPaDwCfzw) to a skateboard drive wheel for testing as-if a rider was present


C49 is only a 50V cap, are you running this at 12S?
```

---
## \#14 Posted by: Pedrodemio Posted at: 2018-02-07T12:30:48.904Z Reads: 56

```
In the spread sheet the highest voltage is above 45V, so is likely that during braking it got up to 50v lots of times and eventually blow the cap

A 63V is that much more expensive to enertion not use them?
```

---
## \#15 Posted by: Blasto Posted at: 2018-02-07T13:44:41.631Z Reads: 49

```
They are 100V caps
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2018-02-07T13:51:18.640Z Reads: 48

```
@Eboosted, yes It could be repaired Just sent it back. 

@Pedrodemio as @Blasto said they are 100V caps, the problem is somewhere else. 

Regards
JF
```

---

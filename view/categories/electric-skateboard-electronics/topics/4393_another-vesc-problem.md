# Another VESC problem

### Replies: 17 Views: 2081

## \#1 Posted by: DeathCookies Posted at: 2016-06-07T14:05:46.969Z Reads: 170

```
Hey there,
unfortunately my VESC is broken somehow... When i pull the trigger there is a difference in the plot but the motor won't spin and it does not show any error at all... It just does not do anything. Someone an idea?
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/2/22d19240138daa2b87a8d6a04c59dfd666a6757f_1_666x500.JPG
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/c/cc1f4c061ebd183054525eb491f0525f5a687ce9_1_666x500.JPG
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-06-07T14:11:48.669Z Reads: 165

```
the drv chip looks a little bit burned.
<img src="/uploads/db1493/original/2X/9/973c34abc45fafd23bc908c66431b0215abf7b3e.png" width="197" height="287">
```

---
## \#3 Posted by: treenutter Posted at: 2016-06-07T14:21:03.473Z Reads: 158

```
@flatsp0t @DeathCookies I was just about to comment on the DRV8302 chip, looks like a hole burnt in it. Can you get an error from BLDC Tool when it's plugged in? 

Also, the soldered connections to the motor and to the caps look like they could use some improvement, probably not the cause of the major error though.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-06-07T14:26:33.370Z Reads: 155

```
[quote="flatsp0t, post:2, topic:4393, full:true"]
the drv chip looks a little bit burned.
[/quote]

That was my thought too... I am just curious that it does not show any error at all.
```

---
## \#5 Posted by: flatsp0t Posted at: 2016-06-07T14:27:53.297Z Reads: 151

```
That is why i think there is another fault somwhere else.
```

---
## \#6 Posted by: treenutter Posted at: 2016-06-07T14:28:25.676Z Reads: 148

```
The DRV error would show up in the realtime data feed in BLDC Tool, just verifying that this is where you are looking, and that you have realtime turned on?
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-06-07T14:29:33.166Z Reads: 142

```
[quote="treenutter, post:3, topic:4393"]
Can you get an error from BLDC Tool when it's plugged in?
[/quote]

Well, maybe i was not specific. 
[quote="DeathCookies, post:1, topic:4393"]
it does not show any error at all
[/quote]

Well, i mean when i have connected it to the bldc-tool it does not show any error at all. The plot of the battery usage shows a difference but it does not turn anything[quote="treenutter, post:3, topic:4393"]
Also, the soldered connections to the motor and to the caps look like they could use some improvement, probably not the cause of the major error though.
[/quote]

I got it like this from enertion. I just swapped out the motor wires. Next time it looks cleaner ;)
```

---
## \#8 Posted by: DeathCookies Posted at: 2016-06-07T14:29:56.418Z Reads: 137

```
[quote="treenutter, post:6, topic:4393, full:true"]
The DRV error would show up in the realtime data feed in BLDC Tool, just verifying that this is where you are looking, and that you have realtime turned on?
[/quote]

Yes,
 that is why i am so curious....
```

---
## \#9 Posted by: chaka Posted at: 2016-06-07T14:33:31.776Z Reads: 133

```
No doubt about it, the drv is toast.  Make sure the gate pins on the mosfets are not bridged if you get the drv replaced.
```

---
## \#10 Posted by: Maxid Posted at: 2016-06-07T15:15:46.701Z Reads: 118

```
any idea what the cause might have been? I don't want to experience the same...
```

---
## \#11 Posted by: DeathCookies Posted at: 2016-06-07T18:19:22.369Z Reads: 107

```
I dont know exactly. I have 12S BLDC mode and it was a bit rainy... Maybe a drop hit my DRV and caused this burning...
```

---
## \#12 Posted by: KMeyerson Posted at: 2016-06-07T23:49:45.374Z Reads: 89

```
That would certainly do it.
```

---
## \#13 Posted by: chaka Posted at: 2016-06-08T13:12:45.049Z Reads: 70

```
What motor are you using?
```

---
## \#14 Posted by: DeathCookies Posted at: 2016-06-08T13:26:46.829Z Reads: 70

```
Turnigy SK3 6374 149kv. Why?
```

---
## \#15 Posted by: chaka Posted at: 2016-06-08T13:43:32.737Z Reads: 70

```
Trying to rule out a high ERPM failure. Hard to really tell from the photos but it does look like you have a possible bridge on the mosfet gates.
```

---
## \#16 Posted by: DeathCookies Posted at: 2016-06-08T13:57:00.640Z Reads: 67

```
[quote="chaka, post:15, topic:4393"]
Trying to rule out a high ERPM failure
[/quote]

[quote="chaka, post:1, topic:3125"]
8570 RPM/50v = 170kv - 12s
[/quote]

I am safe under the 170kv ^^
```

---
## \#17 Posted by: chaka Posted at: 2016-06-08T13:58:01.119Z Reads: 65

```
Yeah those 149kv sk3's work beautifully @ 12s
```

---

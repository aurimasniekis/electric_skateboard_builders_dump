# Remote error stopping sent board into traffic (HELP)

### Replies: 17 Views: 498

## \#1 Posted by: denton Posted at: 2018-06-26T14:40:13.311Z Reads: 119

```
I was stopping at an intersection and hit my breaks then suddenly my board went FULL throttle in reverse, and my board shot out into traffic and I had no control. (the curb on the other side of the road saved my board. It shot a foot and a half in the air off of it and was kinda amazing)

When I hit the top or bottom of the throttle it just holds full power in either direction. Then the remote disconnects. I have a full charge on the remote, but it won't stay on. Is the remote just dead?

Really don't want this to happen when I am on it again.

https://youtu.be/oNaLUy83dtU
```

---
## \#2 Posted by: Acido Posted at: 2018-06-26T14:57:28.733Z Reads: 107

```
use ackmaniac firmware and then use the mode with no reverse
and did you setup the fail safe properly?
```

---
## \#3 Posted by: denton Posted at: 2018-06-26T15:07:40.132Z Reads: 103

```
I like having reverse. But it also does it with forward as well.
It was plug and play out of the box. I haven't had to set up much other than the VESC.
It has been operating for several months just fine then it just did this yesterday.

What is ackmaniac firmware?
```

---
## \#4 Posted by: Sender Posted at: 2018-06-26T15:47:01.676Z Reads: 94

```
Does it do it consistently or is it kind of intermittent?
```

---
## \#5 Posted by: denton Posted at: 2018-06-26T15:50:11.442Z Reads: 93

```
it is now very intermittent. I was thinking of just getting a new controller. 
But I would like to know the cause just for ease of mind when riding it again.
```

---
## \#6 Posted by: JamesNothing Posted at: 2018-06-26T16:52:41.713Z Reads: 87

```
I had kinda the same problem with my firs board. I didn't have reverse, but it did it in fwd mode. Basically I discovered that the receiver was making intermittent contact with the servo cable going to the vesc. I smashed the 3pin connector into the vesc and the receiver and secured the two connections with hot glue (lots of it).
it may be this, it may be a broken wire in the servo cable or it may be an entirely different problem, but it's worth trying to check the connection/change the cable.
```

---
## \#7 Posted by: Sender Posted at: 2018-06-26T16:58:34.186Z Reads: 86

```
I had a similar thing with a nano x, replaced it, problem solved.
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-06-26T17:16:23.629Z Reads: 86

```
[quote="denton, post:3, topic:60107"]
What is ackmaniac firmware?
[/quote]

@Ackmaniac is a user here on the forum. He modded the vesc firmware and BLDC tool to have added functionality. You can check out the thread here http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/3
```

---
## \#9 Posted by: denton Posted at: 2018-06-26T17:18:56.412Z Reads: 85

```
I have done the same thing. I already have it all hot glued, it looks ugly but it’s locked in good. I have been debating on just soldering the cable on. 

I might just get a new controller and hard connecting it in. 

Thanks!
```

---
## \#10 Posted by: JamesNothing Posted at: 2018-06-26T18:03:42.787Z Reads: 76

```
A bit of solder  didn't ever kill anyone. BUT try the glued version for a bit and if the problem is still there try to change the servo wire entirely. Then, if this did the trick you can solder it on "permanently"
```

---
## \#11 Posted by: denton Posted at: 2018-06-27T14:37:08.857Z Reads: 66

```
I’ll get the new one in and work it out and let you know what I find out. 

I played with the connections as I hit the throttle and couldn’t get the wiring to duplicate the problem. It just does it sitting on my desk. So. That’s encouraging.
```

---
## \#12 Posted by: Sender Posted at: 2018-06-27T14:43:29.153Z Reads: 64

```
Man it sounds eerily similar to my nano x that was unpredictable like that.  It was remote, jot the reciever in my case
```

---
## \#13 Posted by: denton Posted at: 2018-07-06T21:45:46.667Z Reads: 45

```
So after some time I asked Dexter at Tourque Boards about the remote and he said it sounded like the battery, so I took it apart and the battery was all swollen. I had some small 3.7v Lipos here and swapped it out and BOOM works like new!
```

---
## \#14 Posted by: Sender Posted at: 2018-07-06T22:35:57.859Z Reads: 42

```
Glad you got it sorted!
```

---
## \#15 Posted by: mmaner Posted at: 2018-07-06T22:58:32.744Z Reads: 39

```
I need a replacement battery for a Maytech remote, would mind linking the small 3.7v lipos you have?
```

---
## \#16 Posted by: denton Posted at: 2018-07-06T23:01:46.783Z Reads: 38

```
This isn't the exact one, but it should do.
http://a.co/4UxQZku
```

---
## \#17 Posted by: mmaner Posted at: 2018-07-06T23:03:09.286Z Reads: 36

```
Thank you sir.
```

---

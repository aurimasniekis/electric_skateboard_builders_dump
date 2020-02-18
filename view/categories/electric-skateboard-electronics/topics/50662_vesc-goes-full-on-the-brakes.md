# Vesc goes full on the brakes

### Replies: 10 Views: 576

## \#1 Posted by: Grolletje Posted at: 2018-03-30T16:01:51.081Z Reads: 89

```
so I got a problem, my board sometimes goes all out of knowwhere 100% on the brakes. this usually happens in intersections. when approaching the intersection I let smootly go the throttle, most of the times halfway past the intersection I (super carefully) go back on throttle. and then shit happens, sometimes with the absolute over current faultcode.

I already did a few motor detections.
some build info:
190 KV motor
vesc 4.10 running ackmaniac

And some BLDC screenshots:
![2018-03-30 (4)|690x387](upload://hTiIgeV1HhLZcCuVcSo5utBuLsH.png)![2018-03-30 (1)|690x387](upload://7Kw85yF3xiWQ0AIYMZBedKvQmwd.png)![2018-03-30 (2)|690x387](upload://v414a7WFoCZR7CeCNb8AeaNH2w1.png)![2018-03-30 (3)|690x387](upload://qDFhQeX53oJgHH027A7ckwmPvx5.png)![2018-03-30|690x387](upload://61zmGHSWfoPTlQawM5vcKhdbUfM.png)
```

---
## \#2 Posted by: Skitzor Posted at: 2018-03-30T18:00:52.530Z Reads: 69

```
In most cases, I would suspect interference in your remote signal. Try changing channels at the mentioned intersection and see if it gets better. Try holding it close to the board.

Edit: The interference coming from ground loops magnetic fields, Radars watching traffic or even wifi when it's very modern
```

---
## \#3 Posted by: Grolletje Posted at: 2018-03-30T18:46:22.135Z Reads: 65

```
thx for the input! I am using a winning remote.

[quote="Skitzor, post:2, topic:50662"]
Try changing channels
[/quote]
how can I do this? I don't really know what you mean with it.

I got a spare remote, I am going to try use that and see if things change!
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2018-03-30T18:48:10.407Z Reads: 60

```
did you calibrate the remote again yet.. i just had one spaz on me.. so i recalibrated.. seems like it worked :thinking:
```

---
## \#5 Posted by: Skitzor Posted at: 2018-03-30T18:57:03.564Z Reads: 55

```
[quote="Grolletje, post:3, topic:50662"]
winning remote.
[/quote]

Careful with those. Where are you at ? Your name seems dutch

Why I say careful : http://www.electric-skateboard.builders/t/has-anyone-not-had-issues-with-the-winning-remote/8524 

Binding procedure: 

vesc on CH1, bind loop key in bind, start everything with the binding button pushed in on the remote! let the button go and remove binding loop.
```

---
## \#6 Posted by: Grolletje Posted at: 2018-03-30T18:59:57.765Z Reads: 48

```
ppm frequencies are about as good as it gets, I don't think it thats the problem...
```

---
## \#7 Posted by: Grolletje Posted at: 2018-03-30T19:01:06.914Z Reads: 49

```
yes I am dutch, I will do the binding procedure.

thx for the help!
```

---
## \#8 Posted by: Skitzor Posted at: 2018-03-30T19:35:28.953Z Reads: 44

```
Yeah, I'm Belgian, so if you're not to far away and want to get to the bottom of this, we could figure something out. Got some winnings laying around
```

---
## \#9 Posted by: RedEagle Posted at: 2018-03-30T20:08:12.407Z Reads: 38

```
Not sure if you know this or it helps but you have to recalibrate the remote everytime you turn the board on. One flick up and down and you're good to go.
```

---
## \#10 Posted by: Grolletje Posted at: 2018-11-07T12:18:23.536Z Reads: 19

```
just to close the topic, the problem was an external motorwire short. The wire protection was rubbed off the cables partially and therefore two wires were able to short.
```

---

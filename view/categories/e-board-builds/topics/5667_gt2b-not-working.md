# Gt2b not working

### Replies: 15 Views: 1741

## \#1 Posted by: gaetjen Posted at: 2016-07-06T18:51:49.286Z Reads: 154

```
Hey guys,

I need some help concerning my g2tb. I setup up everything. Motor detection worked. The red light on my gt2b reciever indicates that it is connected, but when I go to settings and select ppm, current no reverse with brake and tick display it stays at 50 %. It doesn't do anything when I push full throttle or reverse.
I hope somebody can help

greetz
```

---
## \#2 Posted by: cmatson Posted at: 2016-07-07T03:17:27.582Z Reads: 139

```
do you have the PPM cable from the VESC plugged into the receiver in the correct spot and orientation? 

it needs to be in channel 2, with the negative wire on the 3 pin cable furthest to the edge of the receiver.

Even if you have it in channel 1 or 3 (or if the 3 pin connector is in backwards) the receiver will still turn on and connect, it just won't be able to transmit the information to the VESC.
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-07-07T07:48:33.779Z Reads: 127

```
Did you already bind the TX with the RX?
```

---
## \#4 Posted by: gaetjen Posted at: 2016-07-07T08:39:11.599Z Reads: 119

```
Did both. Still doesn't work.
```

---
## \#5 Posted by: gaetjen Posted at: 2016-07-07T15:16:07.371Z Reads: 110

```
I have to bind everythime I turn the board on. Does this have to do with anything?
```

---
## \#6 Posted by: treenutter Posted at: 2016-07-07T16:18:28.173Z Reads: 111

```
[quote="gaetjen, post:5, topic:5667"]
I have to bind everythime I turn the board on.
[/quote]

That's definitely not normal. Do you mean you have to use a binding jumper every time, and go through the whole process? If so, that sounds like a hardware issue to me.
```

---
## \#7 Posted by: gaetjen Posted at: 2016-07-07T16:45:26.155Z Reads: 104

```
It works. Thanks for the help
```

---
## \#8 Posted by: cmatson Posted at: 2016-07-07T22:58:17.058Z Reads: 101

```
What's you end up doing?

Glad it's solved!
```

---
## \#9 Posted by: gaetjen Posted at: 2016-07-09T22:10:44.811Z Reads: 96

```
The order in which you set up your rx und TX is very important. I missed one step and so I didn't get any connection
```

---
## \#10 Posted by: Pablo_702 Posted at: 2016-07-20T02:33:00.757Z Reads: 90

```
can you explain this a little better im going trhu tha same thing right now
```

---
## \#11 Posted by: Jebe Posted at: 2016-07-30T04:11:21.337Z Reads: 84

```
Hey bud, glad you got yours to work. Would you mind sharing with the forum what you ended up doing to fix it ?
Forums only work if its give and take
```

---
## \#12 Posted by: gaetjen Posted at: 2016-07-30T21:31:54.666Z Reads: 79

```
Hey, sorry I was on vacations. Will upload the whole deck soon. @Pablo_702. Just follow the steps from this video step by step https://www.youtube.com/watch?v=W-1CZ5wXC4g
```

---
## \#13 Posted by: Pablo_702 Posted at: 2016-07-30T23:02:48.947Z Reads: 77

```
Hahaha thats the same video i watched to get it goin
```

---
## \#14 Posted by: Poseidon Posted at: 2016-12-17T11:16:33.794Z Reads: 42

```
I followed that video, but when I restart the vesc, the reciever starts blinking again. Anyone could help me? I don't know what else I can try. Thanks
```

---
## \#15 Posted by: gaetjen Posted at: 2016-12-17T11:33:28.863Z Reads: 39

```
Did you configure the ppm settings?
```

---

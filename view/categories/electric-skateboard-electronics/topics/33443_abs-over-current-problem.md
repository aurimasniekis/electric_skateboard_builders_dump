# ABS_OVER_CURRENT problem

### Replies: 16 Views: 962

## \#1 Posted by: rolexbene Posted at: 2017-09-18T20:08:46.991Z Reads: 126

```
So my new setup is running almost sweet. My problem is that I keep getting ABS_OVER_CURRENT Fault. This seems to be when I am going down hill for some time before I start riding. The brake cut out for a few seconds, no ideal down hill...

Can anyone tell me what could be causing this?

<img src="/uploads/db1493/original/3X/a/9/a9bcd9e667faf3ab2b846f792934d7347874ccbf.jpeg" width="281" height="500">
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-18T20:18:15.049Z Reads: 115

```
What connectors are using between motor and vesc?
```

---
## \#3 Posted by: rolexbene Posted at: 2017-09-18T20:20:01.669Z Reads: 114

```
[quote="scepterr, post:2, topic:33443"]
vesc
[/quote]

4mm bullets.

http://www.ebay.co.uk/itm/10-Pairs-4mm-Male-Female-Bullet-Connector-Banana-Plugs-Adapter-For-RC-Battery/331950529236?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-18T20:21:19.841Z Reads: 110

```
Those springy spinny bullets are at fault I'm 99% sure, replace them with solid bullets. Had the same thing happening, 1 out of 6 of those bullets were bad and caused over current fault
```

---
## \#5 Posted by: rolexbene Posted at: 2017-09-18T20:27:00.652Z Reads: 108

```
[quote="scepterr, post:4, topic:33443"]
over current fault
[/quote]

Thanks for the heads up. Do you happen to know what the over current fault means? Why would poor conductivity cause over current? Where is the best place to buy decent connectors.
```

---
## \#6 Posted by: Bloop Posted at: 2017-09-18T20:28:12.901Z Reads: 102

```
wait so you are getting the error when you are breaking downhill when the battery is full ?
```

---
## \#7 Posted by: scepterr Posted at: 2017-09-18T20:33:23.331Z Reads: 98

```
The bullets lose connection, voltage drops and current spikes to try to keep up
```

---
## \#8 Posted by: rolexbene Posted at: 2017-09-18T20:43:36.842Z Reads: 97

```
[quote="scepterr, post:7, topic:33443"]
current
[/quote]

I have heard it is quite a common fault, do you know if it can cause a meltdown, or am I safe until I get some new connectors.
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-18T20:46:46.054Z Reads: 96

```
Could be risky. 
I would still inspect the vesc pcb to make sure its fine, check the shunts, etc
```

---
## \#10 Posted by: rolexbene Posted at: 2017-09-18T20:56:19.620Z Reads: 98

```
[quote="scepterr, post:9, topic:33443"]
etc
[/quote]

Its a FOCBOX but will take it apart soon and have a look, what am I looking for? Bad solder?
```

---
## \#11 Posted by: scepterr Posted at: 2017-09-18T20:58:29.651Z Reads: 95

```
Yeah, not under warranty with the focbox?
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-09-18T21:16:33.194Z Reads: 93

```
Before taking it apart, make sure to contact Enertion support... Or you could void your warranty, If you didn't bought it from Enertion, make sure to contact the person who sold it to you, since he is the warranty holder. I don't think your problem is related to the connector you use...
```

---
## \#13 Posted by: rolexbene Posted at: 2017-09-18T22:03:19.484Z Reads: 91

```
Have just contacted enertionboards to see what they have to say. @JohnnyMeduse can you shed any light on what this fault code actually means?
```

---
## \#14 Posted by: kptheinventor Posted at: 2017-09-19T04:40:52.912Z Reads: 80

```
I had a similar issue to you. The problem for me was the jumper wires between the vesc and receiver had fatigued and the connection jumped in and out while riding. I had the board apply brakes and speed up randomly, sometimes would lose braking ability (can be pretty scary).

I got new connector and changed the way the vesc was layed out in my enclosure so the jumper wires weren't rubbing as much.
```

---
## \#15 Posted by: Jebe Posted at: 2017-09-29T09:38:37.409Z Reads: 66

```
I've had this issue with a vesc -x for a while. It's fine in BLDC (apart from belt cogging and the whine :angry: ) but in foc I am having this issue generally at higher rpm's but not always.
Am running @Ackmaniac 's  awesome firmware in watt mode. Dual sk3 260kv's connected by canbus.
Have changed out the receiver cable, checked all terminations - all seem ok.

Is there a kV limit for foc? I am using the max erpm limit setting at 60000
```

---
## \#16 Posted by: Jebe Posted at: 2017-10-06T02:05:42.107Z Reads: 57

```
found it
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/1162?u=jebe
```

---

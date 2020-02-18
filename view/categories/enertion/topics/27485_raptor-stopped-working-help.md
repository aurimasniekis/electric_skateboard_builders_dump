# Raptor stopped working. Help?

### Replies: 18 Views: 1293

## \#1 Posted by: bucksd Posted at: 2017-07-13T02:39:48.107Z Reads: 207

```
One motor just stutters when you give it throttle. I installed the Nano-X a few days ago, maybe used it on a couple rides since. Stopped working today. Checked that all the connections are snug. Didn't see any visible charring or anything unusual.

[Here's a video showing what I'm talking about.](https://photos.app.goo.gl/fQsesvEDFAeXAAOt2) 

Couldn't even coast the board home because it turns on (when switched off) when you get enough speed and then it brakes with full force...
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-13T02:52:20.672Z Reads: 205

```
plug the VESCs into your computer and check for faults in BLDC tool (terminal > type "faults"). Keep in mind faults reset to nothing through restarts.
```

---
## \#3 Posted by: psychotiller Posted at: 2017-07-13T02:57:49.841Z Reads: 199

```
Sounds like burned mosfets to me
```

---
## \#4 Posted by: Battosaii Posted at: 2017-07-13T03:33:17.838Z Reads: 194

```
My raptor did the same thing, one of my vesc burned the drv chip, working vesc is going slow because the other wheel is not turning i believe its a traction control feature, if you ride it the working motor will operate normally.
Im riding my Raptor with one motor till my Focbox's come in.

Like @Jinra says plug in the BLDC tool and check for faults as you try to spin the wheels with the remote.
```

---
## \#5 Posted by: Skitzor Posted at: 2017-07-13T11:57:56.023Z Reads: 159

```
When it happened. Did it feel like the motor was braking on your left back side?
Anyway. **Stop riding it with the motor connected to your vesc** as the drag could damage more, like your canbus connection going into your other Vesc. You VESC DRV is 9/10 fried. 
You will probably get the DRV-error when you type faults in the BDLC-tool terminal.
Check your motor for shorts before replacing another VESC or you'll go down the same issue.
```

---
## \#6 Posted by: Blasto Posted at: 2017-07-13T15:02:25.228Z Reads: 146

```
The vesc does not seem to be throwing an error, it's hard to see because the signal led is red. But we don't seem to see 3 flashes from the master vesc.

Looks to me it's just a break on one of the phases to the vesc.
```

---
## \#7 Posted by: bucksd Posted at: 2017-07-14T03:48:52.693Z Reads: 127

```
WIsh I had time to try using the BLDC tool you guys are suggesting, but I just don't at the moment. I've contacted Enertion support since it's within a year of purchase. 

I think what some of you were saying is that if I disconnect one of the VESCs, assuming one is fault, then the other VESC and motor should function normally? It'd be nice to ride it on one motor until a replacement part arrives (unless I have to ship the board somewhere). Stopped riding it when this happened because it doesn't move at all.

Also, I LOOKED for shorts but didn't see anything...what exactly should I be looking for and where? I didn't notice any burnt stuff and everything was connected as usual. I'll have to double check.
```

---
## \#8 Posted by: Eboosted Posted at: 2017-07-14T05:53:41.464Z Reads: 114

```
Just plug the vesc to you computer with a regular mini USB cable, download the BLDC tool go to the terminal tab and write faults. 

Another option is to switch the vescs and see if the problem follows the vesc or the motor. 

Another option is a bad connection on the sensor wires on one of the motors
```

---
## \#9 Posted by: Skitzor Posted at: 2017-07-14T11:47:36.171Z Reads: 102

```
This is not enough. Disconnect the CAN between both VESCS to prevent damage to the one that's possibly 'safe'.
There's no sensors in the R-specs
```

---
## \#10 Posted by: bucksd Posted at: 2017-07-27T18:57:41.438Z Reads: 95

```
How do I swap the VESCs? Are they glued in or do they just pull out?
```

---
## \#11 Posted by: Skitzor Posted at: 2017-07-27T19:20:23.659Z Reads: 95

```
All glue. Remove it slowly with a knife and lots of patience. Glue the new ones watertight again. Lovely job. Done it trice already on mine. Focboxes are holding up so far
```

---
## \#12 Posted by: bucksd Posted at: 2017-07-27T19:29:27.746Z Reads: 91

```
Thanks! Suggestion on glue to use?
```

---
## \#13 Posted by: Skitzor Posted at: 2017-07-27T19:32:00.603Z Reads: 92

```
A regular glue gun with sticks will do.
```

---
## \#14 Posted by: bucksd Posted at: 2017-07-28T18:31:09.442Z Reads: 90

```
The middle wire from the VESC to one of the motors broke where it's soldered to the VESC. I tried adding solder but it broke again. 

Should I remove all the solder on that connection and completely redo it? I'm having a hard time getting the wire to reach the VESC, so when I'm trying to connect the two it's basically just solder that's connecting them, rather than the wire being soldered directly to the VESC it is more like solder 'strung' between the two and it keeps breaking.
```

---
## \#15 Posted by: Skitzor Posted at: 2017-07-30T12:53:48.139Z Reads: 91

```
You could lengthen your bullet connectors with some wire up front. Like most are delivered 
You should redo the soldering totally. You probably have a different type of solder.

Example:
wp-content/uploads/2016/02/vesc-electronic-speed-controller.jpg
```

---
## \#16 Posted by: psychotiller Posted at: 2017-11-05T00:08:08.135Z Reads: 73

```
Why not address the issue of the wire being pulled too tight?
```

---
## \#17 Posted by: kisum95 Posted at: 2019-04-17T14:57:58.065Z Reads: 20

```
Have you found a solution? I am currently experiencing the same issue right now ..
```

---
## \#18 Posted by: never4getf150forums Posted at: 2019-04-17T15:02:54.771Z Reads: 19

```
you went 2 years into the past my friend, consider starting a new topic with more details with your issue.
```

---

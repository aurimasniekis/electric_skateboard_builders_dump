# Faulty Board- possible bad connection between VESC and Motor. Requesting help!

### Replies: 11 Views: 267

## \#1 Posted by: nmp160430 Posted at: 2018-07-06T16:18:08.924Z Reads: 73

```
(Hey all! First time making a thread, so feel free to tell me if I need to change anything!)

I made an electronic skateboard last year and it was working great until a few months ago. All of a sudden, whenever I hit a bump in the road, the power temporarily cuts out (and usually comes back on in a few seconds- but by that point I have been knocked off the board). I thought it was just a loose wire initially, but I've re-secured all connections and the power cut-offs are still happening. Now I think there may be something wrong with one of the connections between the VESC and the motor. When I move one (the middle) of those 3 connections when the board is on, sometimes sparks shoot from that connection and the motor halts, even though the wires are still connected. Is there a reason for this, and is there a way to fix this? 

(I have a video showing the problem, but I am not sure how to post it yet. I will try to get that up tonight if it helps)
```

---
## \#2 Posted by: banjaxxed Posted at: 2018-07-06T21:19:40.250Z Reads: 55

```
The three wires, do you mean the phase wires from the esc to the motor?

Is the connection a bullet connection? If so sounds like a bad bullet connection - cold solder, corrosion or the male bullet is not making good contact
```

---
## \#3 Posted by: rich Posted at: 2018-07-06T22:45:54.879Z Reads: 46

```
Could be a loose solder joint on one connector. I had the same thing after several weeks of abuse on one bullet connector of a phase wire extension. After removing the wire mesh the cable just fell off. 

You can upload your video on youtube and just paste the link here, in your post is then the player
```

---
## \#4 Posted by: nmp160430 Posted at: 2018-07-08T21:03:39.851Z Reads: 35

```
Sorry for delay in uploading the video to Youtube (used a family member's account). Here it is: https://youtu.be/OReAjjnANCU.

There are gold/bullet connectors for each of the 3 connections, and I guess they are the phase wires? Is there a better way to connect them than bullet connectors?
```

---
## \#5 Posted by: pat.speed Posted at: 2018-07-08T21:19:22.239Z Reads: 30

```
Hmm ok, what were you using to move them in the video? Was it metal and was shorting the leads?

Btw I wouldn’t do that as it might fry the Vesc I’m actually surprised it hasn’t already
```

---
## \#6 Posted by: nmp160430 Posted at: 2018-07-09T17:09:18.733Z Reads: 24

```
It was the end of the screwdriver, but the first time it happened I was just moving it with my hand.

 I have the BLDC tool- is there a way I could test that the VESC is okay? As long as I am not hitting any bumps, the board still runs fine.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-07-09T22:12:39.105Z Reads: 24

```
Yeah, try typing into the terminal “faults” after sparks happen
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2018-07-10T01:39:14.594Z Reads: 22

```
Sounds like you just fried your DRV
```

---
## \#9 Posted by: banjaxxed Posted at: 2018-07-10T12:04:00.925Z Reads: 16

```
It’s hard to see what you’re grounding out there or even where the screwdriver is placed. If the phases are grounding then this will kill the drv.

If you don’t have the knowledge to work this one out and can’t take a clearer closer video and give the community more help to help you, then I would say take my the vesc out and putting it in some heat shrink and also inspect the phase wires for damage and insulate them where the bullets join
![image|281x500](upload://epRcO46Xqo0mvfh6EPpT64vAC0r.png)
```

---
## \#10 Posted by: briman05 Posted at: 2018-07-10T12:47:29.313Z Reads: 13

```
 You never touch metal on metal when there is electricity running through it that creates a short.  Your body also conducts electricity if you are going to move them around use some sort of rubber glove or plastic fuse pullers.  To me it looks like you hit the solder joint or where the bullet connectors come together.  What Vesc are you using? And could take a picture of the connection
```

---
## \#11 Posted by: nmp160430 Posted at: 2018-09-15T22:52:33.686Z Reads: 10

```
I think I have finally got it! I velcroed the VESC to the bottom of the box closer to the motor so it couldn't move around as much when I hit the bumps. My board seems to be working without any hiccups now! Thanks for all the help!
```

---

# Genesis/Koowheel adding aftermarket esc

### Replies: 11 Views: 262

## \#1 Posted by: DangerSk8 Posted at: 2019-09-08T22:42:38.418Z Reads: 45

```
I have a genesis hellfire - same as a koowheel board.
Mine has the 1st gen electronics on it and the motherboard experienced some water damage resulting in a dead board.  I found replacement parts on the Koowheel website but they are all the 2nd Gen stuff.
What I am hoping someone can answer for me is can I take the gen 2 motherboard and use it with my gen remote and hub motors?  I noticed that the wiring is slightly different (gen 1 has 3 wires per hub while gen 2 has the 3 wires spliced into a single plug) but I think that can be fixed pretty easily, it's the programming that I am clueless about and would love some advice.  
I already have read the other threads with the usual "ditch it and build from scratch" type advice, I get that it might not be the most cost effective way to go but I also don't want to let this beat me and want to see if I can fix it.

TIA
```

---
## \#2 Posted by: Flasher Posted at: 2019-09-08T23:46:16.310Z Reads: 40

```
If you're willing to redo the wiring of the connectors on your motors, itll work. As for the remote, you have to buy the 2nd gen remote with the esc. 1st gen remotes dont pair to the 2nd gen escs. I have a 1st gen koowheel (green wheels) that I brought back to life a while back by getting a meepo v1.5 esc. All I had to do was make a new connector for hall sensors and change the connector on the battery.
![15679862463785681201616559263001|243x500](upload://q0JgEPcnwy8mfg71ST1TywodyPg.jpeg) ![15679862788308206708123992289745|243x500](upload://knM81rujXKYRK0QXFFBe1CndXU7.jpeg) ![15679863033217986109000057806941|690x335](upload://hJdCWqZujzin2JdbswVaabFTaPA.jpeg) ![15679863591644119724949540919951|243x500](upload://5HlvFbNAdrA9Pvt8xf4Xre9p5tZ.jpeg)
```

---
## \#3 Posted by: DangerSk8 Posted at: 2019-09-10T17:02:17.614Z Reads: 24

```
Thanks for the info - that's a pretty simple fix looking at your board.  
I am thinking that I will 3D print a new housing for the esc and wire up the battery like you have, the wires running to the battery make more sense for avoiding lost connections on large bumps with the flush fitted original setup.
I am a novice at the electronics part of this so any info is very much welcome!  Can you suggest a brand or supplier for the parts?
```

---
## \#4 Posted by: DangerSk8 Posted at: 2019-09-10T17:21:40.055Z Reads: 24

```
I found this ESC and remote and was thinking of using it with my existing 36V 5500mAh battery and dual hub motors.
https://www.mboards.co/collections/escs/products/dual-hub-motor-esc
```

---
## \#5 Posted by: DangerSk8 Posted at: 2019-09-10T17:23:30.787Z Reads: 25

```
What I am unsure about is how to connect to the battery for charging?
```

---
## \#6 Posted by: Flasher Posted at: 2019-09-10T18:39:18.338Z Reads: 24

```
I connect to my battery through the xt90 directly. Koowheel battery has a bms so it is still protected. I had a 3d print at the start, but vibrations killed the print and you can't allow for this when connections rely on perfect fits.
![received_338019616903209|281x500](upload://hUsgHtlD3RZalztObOk7Tb1BFut.jpeg) ![received_808621536179326|281x500](upload://yfNyGJasZM3QJNQBbHFByK4sfFr.jpeg) ![received_1001159910274674|690x388](upload://4mfhA3aMnAmvU9IGI35gOOSflgj.jpeg) ![received_278177796464727|690x484](upload://emMqv0pWbuvb1wGixqd9IemLpci.png) ![received_349966288991176|281x500](upload://SajMiYYxIha94ry0xCCAVheN0m.jpeg) ![received_2305545506372478|690x388](upload://tpS0EaD9xwJUDZa5mz0B5qrQXKF.jpeg) 
![USER_SCOPED_TEMP_DATA_orca-image--1840109956|348x500](upload://clZtgtQO8EzoJRr1iAbt7mBNipw.jpeg)
```

---
## \#7 Posted by: DangerSk8 Posted at: 2019-10-15T05:13:09.702Z Reads: 17

```
I have gone the aftermarket esc route and now have a new series of questions.
```

---
## \#8 Posted by: DangerSk8 Posted at: 2019-10-15T05:14:35.002Z Reads: 17

```
What type of plug is the small one coming out of the hub motors? Are these for the smoothness of stops and starts? My board has 6-wire plugs per hub, the new esc has 5 prong plug holes… it this the wrong esc? I went with the Mboards 10s. @MBoards
![image|375x500](upload://moEEIwbjH0sNuvKSNO81QjChgH0.jpeg) ![image|666x500](upload://haVX8i4nm0qa5BrVwZ8oU4yKQiq.jpeg) 

Do I need a loop key with the existing Koowheel battery pack?
What is the plug type on the Koowheel battery?
![image|666x500](upload://imW0UXg9dY6nyDQbHAKsIB94gVE.jpeg)
```

---
## \#9 Posted by: DangerSk8 Posted at: 2019-10-15T05:17:17.641Z Reads: 16

```

There is a reasonable difference in the gage of wires used for the esc and hubs, is this going to be an issue?

![image|375x500](upload://w9IjXRWfHIRVeHGoFEY4makFvxG.jpeg)
```

---
## \#10 Posted by: DangerSk8 Posted at: 2019-10-15T05:18:38.542Z Reads: 17

```
The MBoard esc 10s if anyone is interested in a close up look at it.
![image|666x500](upload://ilgS9tXrbx1Sd5i4oj4IpchqvYm.jpeg)
```

---
## \#11 Posted by: DangerSk8 Posted at: 2019-11-08T17:55:05.496Z Reads: 9

```
For anyone who has been following this thread, here's where this one ended up:
![eSk8%201|666x500](upload://5cUel7lSNB2T3UDGMUdCVFiGplk.jpeg) ![eSk8%202|666x500](upload://ibTHZUZsE5vnqN8eueTzZyzn1VQ.jpeg) ![eSk8%203|666x500](upload://2P9j3fGyOLjChWKpHnhWr0crMTr.jpeg) ![eSk8%204|666x500](upload://ybpp9yy7fbHVRLZAXTSbo6XIYFM.jpeg)
```

---

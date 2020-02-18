# ABS_OVER_CURRENT Error

### Replies: 28 Views: 1306

## \#1 Posted by: Monstercrunch Posted at: 2016-08-25T17:22:31.561Z Reads: 143

```
(copied from my post on vedder.se forums)

Hi guys, 

I managed to get everything working (homemade vesc), the board was moving with the remote (nothing on it), but when I put my foot on it and applied a small pressure, I found some lag in (that's what I thought) the command transmission. And then nothing, even with my foot off. The red led was blinking and the board not moving anymore.

I connected it back to the computer and I had a ABS_OVER_CURRENT (-136amps something like that). I rebooted the VESC, seemed to be ok (no error showing up and correct current values), but now the motor doesn't move anymore  :( 

It's like the VESC "see" it moving (the pikes is when I hit the gaz but the motor doesn't move):

http://i35.servimg.com/u/f35/13/84/06/30/curren10.png
http://i35.servimg.com/u/f35/13/84/06/30/rpm10.png

My motor conf:

http://i35.servimg.com/u/f35/13/84/06/30/motor10.png
http://i35.servimg.com/u/f35/13/84/06/30/bldc10.png

When I run a motor detection it doesn't move the motor and I get bad detection but no error in the real time data.
So close to ride it...  :cry: 

Is it bad doctor ?
```

---
## \#2 Posted by: Monstercrunch Posted at: 2016-08-26T18:33:10.381Z Reads: 116

```
Some news : I saw that there were a possibility that the phases could be shorted, so I disassembled the motor but everything looked fine.

I tried again and now I can get the motor moving a little bit. It just clicks and raises immediately an ABS_OVER_CURRENT.

I checked my shunt they seem fine (added some tin to be sure). Also today (I don't remember changing anything) the real time data look like crap:

http://i35.servimg.com/u/f35/13/84/06/30/shitty10.jpg

My DRV is brand new, the motor worked few minutes perfectly (but with no load). I guess the problem came when it started to draw more amps.

Don't know where to look, I'm desperate... :disappointed:
```

---
## \#3 Posted by: chaka Posted at: 2016-08-26T18:56:56.080Z Reads: 103

```
Post some high res photos and we can take a look to see if something is out of order and can be cleaned up or resoldered.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-08-26T18:59:18.082Z Reads: 105

```
Do you have some picture? Maybe it the Ground plane of the DRV that is not correctly solder.
```

---
## \#5 Posted by: Blasto Posted at: 2016-08-26T19:44:39.778Z Reads: 98

```
Make sure you didn't short out the shunts on themselves, or check if the shunts sense are well soldered
```

---
## \#6 Posted by: Monstercrunch Posted at: 2016-08-26T20:23:37.159Z Reads: 99

```
I checked the shunt and added more tin, don't know how it could come from it. I'll check the shunt line to the drv.

And the DRV pad is good, I made sure to solder it correctly (it's my second DRV, I blew the first one either because I soldered a diode the way around or because the pad wasn't correctly connected).

Here are the pics:

http://i35.servimg.com/u/f35/13/84/06/30/img_5514.jpg

http://i35.servimg.com/u/f35/13/84/06/30/img_5518.jpg

http://i35.servimg.com/u/f35/13/84/06/30/img_5515.jpg

http://i35.servimg.com/u/f35/13/84/06/30/img_5516.jpg

http://i35.servimg.com/u/f35/13/84/06/30/img_5517.jpg



Could it come from the big caps ? I'm not sure the soldering is perfect (I'll fix it tomorrow).

Thanks a lot for your help :relaxed:
```

---
## \#7 Posted by: Blasto Posted at: 2016-08-26T20:57:10.959Z Reads: 90

```
Other thing you can do is check the continuity of the drain-source of the fet to see if you have one that is blown. Same thing for gate-drain, must be high impedance.
```

---
## \#8 Posted by: Monstercrunch Posted at: 2016-08-27T13:12:27.513Z Reads: 88

```
@Blasto : I checked the shunt and they seem to be "shorted on themselves" as you said. I think my multimeter is no accurate enough and see it as a continuous line (here in red). Is it normal or should it see a resistance between the red dots ?

http://i35.servimg.com/u/f35/13/84/06/30/shortc11.jpg

I don't know what you mean by the drain-source and gate-drain. Could you please be more specific ?

Thanks :)
```

---
## \#9 Posted by: Blasto Posted at: 2016-08-27T13:33:33.106Z Reads: 87

```
Thats normal, accros the shunt there's 5mOhm of resistance, you won't be able to measure that with any multimeter. What i mean when i say short themselves, is the small leg is short with the big leg. But i dont think this is the case.
```

---
## \#10 Posted by: Monstercrunch Posted at: 2016-08-27T13:38:19.591Z Reads: 84

```
Ok, but what about drain-source and gate-drain ?
```

---
## \#11 Posted by: Blasto Posted at: 2016-08-27T13:58:35.384Z Reads: 85

```
Need to look in my old threads, i explained this already w some fancy ms paint pictures. Hold on
```

---
## \#12 Posted by: Monstercrunch Posted at: 2016-08-28T16:18:53.835Z Reads: 77

```
Do you have the title of the topic ? I looked to your old posts but didn't find your piece of art :/
```

---
## \#13 Posted by: racidon Posted at: 2016-08-28T16:37:23.922Z Reads: 75

```
I had this issue when I had bad connections from the FETs to the Motor. It was evident when I inspected the plugs and they had burn marks from the arcing electricity. Perhaps ensure that you have a solid connection that can pass high amperage/voltage through?
```

---
## \#14 Posted by: kaziupir Posted at: 2016-08-28T17:08:21.822Z Reads: 74

```
Are these pins soldered together?<img src="/uploads/db1493/original/2X/6/6d9aae532229b7efa1b5fc48c8f3f7a3a1a3cc00.jpg" width="690" height="460">
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2016-08-28T17:12:20.114Z Reads: 72

```
Yes, these are normal
```

---
## \#16 Posted by: Monstercrunch Posted at: 2016-08-28T18:22:10.380Z Reads: 71

```
Well, I checked my soldering and didn't see any burnt marks :confused:
And yes, the two pins are connected together
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2016-08-28T18:26:18.230Z Reads: 71

```
Maybe those will help you for checking the mosfet (Like @Blasto suggest)

<img src="/uploads/db1493/original/2X/c/c27843c7d94b73e97f8483ab3d482181dc7240b7.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/9/93c58b75eed6482ba80d123af1605d6ee2e19cff.jpg" width="375" height="500">
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2016-08-28T18:27:15.189Z Reads: 69

```
You should get the same respond from the multimeter as testing a regular diode
```

---
## \#19 Posted by: Monstercrunch Posted at: 2016-08-28T18:59:41.755Z Reads: 66

```
I tested as you showed. Here are the results:
-in position 1 (picture 1) I have 0.431v value
-in position 2 (picture 2) I have 0.572v value

If I put the probes in the opposte way, I do have OL but not instantly, it "slowly" raise up until it displays OL.

However, in resistor mode, I can read the same value in both position (reversing the probes) :/ Not good right ?
Values:
-in position 1: 41kOhms for the for the two fets of the right, 5MOhms for the third one (the one tested on the picture).
-in position 2: 38kOhms for all fets.

Those values are the same for the fets on the other side of the PCB.
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2016-08-28T19:05:24.015Z Reads: 65

```
these value seem ok, the most important is you don't have any short.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2016-08-28T19:13:39.159Z Reads: 59

```
Where are you located
```

---
## \#22 Posted by: Monstercrunch Posted at: 2016-08-28T20:23:24.595Z Reads: 61

```
Referring to [this](http://en-us.fluke.com/training/training-library/test-tools/digital-multimeters/how-to-test-diodes-using-a-digital-multimeter.html), in resistance mode, "The reverse-biased resistance of a good diode displays OL on a multimeter. **The diode is bad if readings are the same in both directions.**" which is my case.

I live in south of France, but I'm going to SF in september for two weeks :)
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-08-28T21:31:37.589Z Reads: 59

```
Don't forget there is two diode inside a mosfet, also you can get bad reading from charging capacitor, the best way of testing component is to remove them from the circuit. 

South Of France, well... On parle la même langue, mais on est pas sur le même continent :stuck_out_tongue_winking_eye:
```

---
## \#24 Posted by: Monstercrunch Posted at: 2016-08-29T06:29:43.743Z Reads: 58

```
Je me disais bien que ton nom était assez frenchy :stuck_out_tongue:

T'es d'où ?
```

---
## \#25 Posted by: Monstercrunch Posted at: 2016-08-29T18:40:19.208Z Reads: 54

```
Well, I've tested the board with a tiny motor, didn't work :confused:

I've also tested my motor with a standard ESC and it worked well.

Conclusion, now I'm sure it comes from the VESC :'(
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2016-08-29T19:03:06.394Z Reads: 54

```
I think your problem might come from bad soldering over the ground pads of the DVR, it don't take much to burn them, I've just burn one yesterday with a home made VESC, because a forgot to solder one pads of the mosfet. Just changing the DRV may solve the problem .

Montréal, Québec
```

---
## \#27 Posted by: Monstercrunch Posted at: 2016-08-29T19:11:34.606Z Reads: 52

```
Do you think the DRV is dead ? Or should I try to resolder it ?
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2016-08-29T19:23:56.131Z Reads: 52

```
It is most likely dead, but if you can resoldering you should try it just to be sure.
```

---

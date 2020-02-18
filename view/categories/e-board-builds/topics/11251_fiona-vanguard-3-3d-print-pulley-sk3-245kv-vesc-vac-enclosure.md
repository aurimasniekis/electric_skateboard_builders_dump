# Fiona &#124; Vanguard 3 &#124; 3d print pulley &#124; SK3 245kv &#124; VESC&#124; Vac Enclosure

### Replies: 24 Views: 2837

## \#1 Posted by: whatthejess Posted at: 2016-10-16T19:35:42.423Z Reads: 244

```
Meet Fiona an Ogre of a board. The name befits her, based on the rough appearance tied together with the nimble feel of the flex board. Each scar is a battle fought and a lesson learned. I’m from Milwaukee and the roads are atrocious, seriously, this sink hole was two blocks from my house at North and Oakland ave.<img src="/uploads/db1493/original/3X/5/2/5233dffe7b1a94cf8fbb96e68c11a8ce044b978c.gif" width="690" height="450">  The trucks are a mix of a DIY brand Caliber and Gullwings (the blue calibers had some slop in the kingpin and the bushings squeaked). Originally, the board had a DIY brand motor mount but after the second adapter plate cracking I made one myself.  3mm thick ABS Vacuum formed enclosure formed to the contour of the board. 
-VESC in FOC
-245kv Sk3 motors
-15/36 gearing
-NYKO KAMA for controller
- blah. blah.. blah…
<img src="/uploads/db1493/original/3X/4/1/41311ee7d502d5769bbf0898952ce77969e8daa3.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/b/8/b87516c808127a741dc1d45884677cd0602647d5.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/e/b/eb7147a5065f913642b04a861e05d9999ded934d.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/1/9/19756c989c6e557269b05ea82f16ad9bf318b9b1.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/1/d192f277800223afdad52316f6a8208659d54a32.jpg" width="690" height="388">
My informal and evolving plan for this board is a short distance, 10-15 mph cruiser, water resistant and an overall simple design to alleviate points of failure. As you see it now I have completed my objective (water proof seal could use redoing though). The next phase for this board is tuning. I have had numerous little problems:
-momentary acceleration cut out (1/4 second) at the beginning of a hard acceleration 
 - random half second delays
 -at the top end of speed, the vesc will stop accelerating and not accept input for several seconds.
 
Any help on this would be greatly appreciated. I was thinking of moving the Wii receiver outside of the big case. Maybe a ferrite ring too? What do you think?
```

---
## \#2 Posted by: Goombaacez84 Posted at: 2016-10-16T19:46:18.753Z Reads: 230

```
Hey there! I'm from Minnesota. I think you might be the closest esk8 person I've talked to aside from someone who moved out of MN to go to college.

Build looks nice, definitely jealous of the vanguard. I haven't sourced one that I'd be willing to spend on yet but am keeping an eye out for one. Your acceleration cut outs are happening because of the EMI that the phase wires are creating once you go under hard acceleration. It happens to me on high acceleration and when I'm hill climbing with my Kama. I've tried a ferrite ring to no success - I'm at the point that I've ordered several new remotes to replace the Kama. I just couldn't get a smooth acceleration curve or climb hills effectively because of the dropouts.

For the VESC, have you checked the faults to see if you're getting any sort of errors? I had my VESC on FOC and the same thing would happen. I'd have to manually resync my Kama when this happened. Turns out, I was slowly killing my VESC and the DRV went.
```

---
## \#3 Posted by: whatthejess Posted at: 2016-10-16T20:52:16.375Z Reads: 211

```
Have you tried or looked into shielding the phase wires, esc...? 3m Makes EMI Shielding Tapes http://multimedia.3m.com/mws/media/825271O/3m-emi-shielding-tape.pdf. I have aluminum tape on hand now. I could give that a try. Just not sure on what exactly to apply it to, maybe multiple layers of it.
```

---
## \#4 Posted by: Goombaacez84 Posted at: 2016-10-16T21:09:21.502Z Reads: 214

```
I'm not sure about the tape. Someone else here might be able to chime in on if they've tried that. Another way to reduce the noise is to shorten your phase wires as much as possible. My phase wires are a little long and are bunched in my enclosure so that's something I could do to try and mitigate my Kama problems. My VESC is under repair right now though so I haven't touched the board very much since the DRV on that went.

Another thing that might potentially contribute to the interference is just the current coming through your wires from the battery. I don't know how much the batteries actually affect the signal, but like everyone else that had issues, I decided to just get a new remote. Give the ferrite a try and maybe shorten your phase wires if you can. Make sure your receiver wires aren't intertwined in between the phase wires too.
```

---
## \#5 Posted by: whatthejess Posted at: 2016-10-17T01:37:27.419Z Reads: 207

```
Wrapped VESC and phase wires up to block the EMI. <img src="/uploads/db1493/original/3X/1/6/168faaf2b0dda1dbbb1c9084bc329b116f645172.jpg" width="690" height="388"><img 

Works like a charm 
No more problems except now I made a hot potato out of my esc. Im going to wrap it up nice later in the week. Also going to see if i can avoid wrapping the esc.

also here are my screen shots.
<img src="/uploads/db1493/original/3X/2/9/295afc814924254d17de65dc163c70cfb8081dd9.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/d/2dc8666041ed03cbbda43307c02e411812383095.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/3/8/3801f66831aec5432a64690ec3f40bfb839f38c0.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/7/47117b7cb2e2a092ce549cd623884a4125449989.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/5/b5c34c9c5391b1cd9b270b3a948fc94cced7ca66.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/f/8/f8a3fa23a0196244f006b3d6f3f9519b87a7803c.jpg" width="690" height="388">

thanks for the help GoomBaacez84
```

---
## \#6 Posted by: Goombaacez84 Posted at: 2016-10-17T01:44:41.359Z Reads: 159

```
The EMI tape worked, huh? That's really intriguing. I might give that a shot when I get my VESC back and the board running again. Thanks for the suggestion, and glad it worked!
```

---
## \#7 Posted by: Mox Posted at: 2016-10-17T07:06:01.836Z Reads: 149

```
I am currently in the process of ordering items (newby - first orders). Please post updates if this fix actually worked because I was counting on the kama mod. Thanks!
```

---
## \#8 Posted by: whatthejess Posted at: 2016-10-18T16:28:04.464Z Reads: 139

```
Update: This morning I completed some tests on the EMI issue with the wii receiver. The receiver functioned great after the tape was applied (see picture above in previous post) over the past few days. So it removed all of the tape to see if I could duplicate the problem and as expected the negative behaviors came back. I reapplied the Al tape neatly over the same areas as before, this is where it gets weird, the negative behavior was still there. The momentary dropouts and delays in throttle/brake inputs where lessened by the Al tape this time but still apparent. I then turned my attention to the wii receiver to rule out faulty equipment by replacing with a new receiver I had laying around and no change in behavior. So at this point the only difference in the two applications was the way the Al tape was applied. I reapplied the tape in a wrinkled mess and the behavior went away. So my conclusion at this point in EMI issue is Al tape is not thick enough to bock the interference but the wrinkles or gaps, not really sure, do have a positive impact. Need to do some research.
```

---
## \#9 Posted by: Goombaacez84 Posted at: 2016-10-20T17:44:46.019Z Reads: 120

```
@whatthejess - Was your testing done with just aluminum tape? Or did you go out and find some EMI shielding tape?
```

---
## \#10 Posted by: whatthejess Posted at: 2016-10-20T22:42:27.577Z Reads: 124

```
Yeah it was just with the aluminum tape. From what I have researched the aluminum tape is the lowest form of shielding though. 3m makes other types of copper shielding that would probably work even better, but they cost more. Ive been doing upgrades on the 3d printer so I haven't given it much thought. I also want to try moving the receiver really far away, like opposite side of the board at the far end, and see if that makes a difference. It does work with the aluminum tape completely wrapping the esc and phase wires several times. But im not sure of this solution because it looks ghetto and may overheat the esc.

Ive been designing a pulley like the enertion one that doesn't have any hardware. the difference is mine has the 3rd bearing extended out to the center of the pulley. Currently waiting for some Nylon to be delivered <img src="/uploads/db1493/original/3X/9/f/9ff60975dd533e8622d4d382c5180bceabcfb7cd.png" width="471" height="500">
```

---
## \#11 Posted by: Goombaacez84 Posted at: 2016-10-20T22:45:24.894Z Reads: 113

```
Hmm, I've wrapped just the phase wires in a layer of aluminum tape and still got the drops. I'm not sure I feel comfortable making my VESC a hot potato by wrapping the entire thing up either. Maybe I'll give the wires another wrapping of the aluminum tape.

I guess I never considered making the receiver wires super long and just having the wires be on the other side of the board in the other enclosure where my battery is. I wonder if that would cause any sort of delay or latency.
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-10-20T22:47:22.198Z Reads: 108

```
Not worth it just get a mini remote and stay safe
```

---
## \#13 Posted by: whatthejess Posted at: 2016-10-20T22:56:31.076Z Reads: 108

```
My phase wires are wrapped twice. When I just wrapped the phase wires and left the esc alone I it also didn't solve the issue. Ive put about 20 miles total on the board since and I haven't had any overheating issues.  My enclosure is completely sealed and there isn't any air flow to cool.  Maybe wrap it up as a test to pinpoint the issue.
```

---
## \#14 Posted by: Goombaacez84 Posted at: 2016-10-20T23:05:17.249Z Reads: 102

```
I ordered a mini remote from @JLabs on the market on Oct 1st and still don't have any tracking information... just trying to make do with what I have and what's left of the season. There's not much skating time left here in Minnesota.
```

---
## \#15 Posted by: Goombaacez84 Posted at: 2016-10-20T23:06:01.888Z Reads: 100

```
I'll give the VESC a shot too, just as a test. :wink:
```

---
## \#16 Posted by: JLabs Posted at: 2016-10-20T23:21:00.220Z Reads: 100

```
I sent out an update email with all the info you needed. Remotes should ship this weekend. It clearly stated that the remotes ware for pre-order on the website, I am doing my best to get them to you asap. I do not want anyone to get the wrong idea, that they won't receive the product.
```

---
## \#17 Posted by: Goombaacez84 Posted at: 2016-10-20T23:45:53.489Z Reads: 106

```
@JLabs - Sorry, I didn't mean to come off in the way that I'm not getting what I paid for. I'm still patiently waiting for the remote and am still crossing my fingers that it gets here before the snow drops. I wanted to emphasize to @Michaelinvegas that I'm just trying to make do with what I've got and everything I can. I'm aware it says pre-order, but your listed shipping dates on the post have been getting pushed out more and more every time I see it, so at this point I'm just on the "it'll get here when it gets here" boat. Until then, I'm trying to get the Kama going. :wink:

@whatthejess -  I just got back from a ride with an aluminum taped VESC. I experienced almost no drop outs... couple on the hard acceleration pulls, but it was a pretty smooth ride actually. Can't believe it works lol perhaps I'll make little cut outs where the MOSFETs are to let them breath since I'd still feel a little guilty about riding it like this.
```

---
## \#18 Posted by: Michaelinvegas Posted at: 2016-10-20T23:46:49.678Z Reads: 106

```
Waiting is part of the game
```

---
## \#19 Posted by: JLabs Posted at: 2016-10-21T00:02:45.831Z Reads: 108

```
The date was only changed **one** time! It was pushed back 7 days due to the Chinese holiday I was not aware of. These remotes are being provided at an incredible value, and I am doing my *best* to get them to you asap, again the ship date is planned for this weekend.
```

---
## \#20 Posted by: whatthejess Posted at: 2016-10-21T01:58:08.118Z Reads: 103

```
That is good news! I was hoping it would work for you so I didn't seem like a crazy person with tin foil on my head.
```

---
## \#21 Posted by: Goombaacez84 Posted at: 2016-10-21T04:29:48.781Z Reads: 87

```
@JLabs can't wait for the remote :slight_smile:

@whatthejess I'm going to try and put another layer on and then drill holes into my enclosure to let some of the heat dissipate... I couldn't tell if the VESC was hot or if my hands were just that cold after my ride though.
```

---
## \#22 Posted by: Mox Posted at: 2016-10-22T15:50:59.847Z Reads: 84

```
You could try to put the receiver into the battery enclosuer after all. It might make a difference. If I had one I would try myself...
```

---
## \#23 Posted by: XIII Posted at: 2016-10-22T19:47:51.831Z Reads: 89

```
I wrapped the vesc ( entire pcb, half the caps) with kitchen aluminium foil. and I placed the receiver 30 cm backwards with the 4 cables from the receiver completely wrapped in foil aswell.

Phase wires are not wrapped. This solved the entire problem. 
Make sure to wrap the vesc first in electrical tape before applying the foil. 
you should create a new thread of how to fix the nyko kama dropouts!
```

---
## \#24 Posted by: Mox Posted at: 2016-10-23T16:41:43.017Z Reads: 76

```
I found this video.
I figured it might be somewhat helpfull

https://www.youtube.com/watch?v=q04xrNYUa3E
```

---

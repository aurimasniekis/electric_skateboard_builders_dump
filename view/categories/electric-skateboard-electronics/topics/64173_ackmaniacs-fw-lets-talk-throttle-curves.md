# Ackmaniacs FW; Let&rsquo;s talk throttle curves!

### Replies: 26 Views: 1461

## \#1 Posted by: Lionpuncher Posted at: 2018-08-07T20:52:46.525Z Reads: 333

```
Recently finished my second build with Ackmaniacs FW. This little guy is SQUIRRELY. Wanting to adjust my throttle curve to make it a bit more relaxed on the low end and more aggressive on the high end.
Got me to thinking; there must be a buttload of you guys using acks FW, and at least some of you must have messed with the curves and really got the feel you were looking for.
I created this post to have people upload pics of their curves and explain why they went with what they went with.
SHOW US YOUR CURVES!!
```

---
## \#2 Posted by: brenternet Posted at: 2018-08-07T20:59:08.209Z Reads: 325

```
Oh you ;) Let me get a tan first
```

---
## \#3 Posted by: mmaner Posted at: 2018-08-07T21:05:26.083Z Reads: 321

```
![gear%20drive%2012s%20v1%20throttle%20curve|690x412](upload://90sAkhBAEPpdKM5DT3CwYWNPZo1.JPG)
```

---
## \#4 Posted by: Lionpuncher Posted at: 2018-08-07T21:20:43.923Z Reads: 307

```
Sweet! Ok Mike, tell me what I'm looking at here. What does this curve feel like?
```

---
## \#5 Posted by: Mikenopolis Posted at: 2018-08-07T21:27:41.020Z Reads: 305

```
I've actually never messed with these tabs on my own builds since I never had a problem with the acceleration. But after trying out two different CarvOn EVO SDR builds, I plan try it out when I rebuild the current two boards I ride. The difference is very apparent. @caustin what did you do to it? 

What does one do here? just mess with the numbers or is this a click and drag situation?
```

---
## \#6 Posted by: Deckoz Posted at: 2018-08-07T21:28:41.442Z Reads: 300

```
Do Mike's but change edge sharpness to 0...that way it's a smooth curve..

Think of the curve as how much actual throttle the speed loop is receiving. It's basically exponential for the throttle. The horizontal represent your physical throttle. The vertical represent the speed loop throttle

Since Mike's picture has sharpness and isnt smooth I'll use the middle edge upper right quadrant as an example.

Finger 50% throttle
Speedloop 27% throttle

I use:(I think)

standard on X
Y 14.5, 35, 60
Edgeshapness 0


Edit: Also make sure your lines are always shaped like Mike's. Lower left quadrant arching up, upper right quadrant arching down. If you do the opposite, your brakes get stronger (to the point of lock up). And the throttle gets strong and looses umph up top and is very hard to manipulate speed.
```

---
## \#7 Posted by: mmaner Posted at: 2018-08-07T21:54:32.966Z Reads: 277

```
[quote="Lionpuncher, post:4, topic:64173, full:true"]
Sweet! Ok Mike, tell me what I’m looking at here. What does this curve feel like?
[/quote]

It took me awhile to figure out but its pretty simple once you understand it.

Look at the right side of the pic, just the acceleration curve (brakes will come later).  At the bottom you can see the values, power is how much juice the VESC's are pushing and throttle is how far you have pulled the trigger.  

![image|430x99](upload://laiFybYW6Ubahz18lUebcBnAdKA.jpg)

In my example you are getting 12.5% of the available power at 25% trigger pull, 25% of the available power at 50% of the trigger pull, and so on and so on.  

You feel the power more at low speeds than you do at high speeds so it makes sense to have the control more spread out at low speeds than at high speeds.

The brake curve is exactly the same.  At 25% of the throttle push you are getting 12.5% of the available braking, at 50% of the trigger push you are getting 25% of the available braking.

![image|425x91](upload://gaWzvEsmuFGjghVL9HvtY6HWk80.jpg)

I find that at high speeds it takes more braking to actually stop so I want light brakes at the top and hard brakes at the bottom, that way I can choose how much braking is applied progressively.
```

---
## \#8 Posted by: skatardude10 Posted at: 2018-08-07T22:47:57.935Z Reads: 251

```
Someone convince me to mess with my throttle curves a bit... What I've read so far still isn't too convincing. Maybe I should just give it a try next ride and see, maybe it's my gearing tending to be high usually... But I feel like I get punch all the way through for acceleration and braking with a standard linear progression.
```

---
## \#9 Posted by: philvanzu Posted at: 2018-08-07T23:08:01.121Z Reads: 254

```
On my leiftech with winning v2 remote I set the same curve as Mmaner otherwise I don't have enough control at low speeds because the acceleration is pretty brutal, on my Lacroix with GT2B I don't feel the need to change it at all, it all really depends on your setup / remote. If you feel good don't mess with it.
```

---
## \#10 Posted by: b264 Posted at: 2018-08-07T23:15:53.746Z Reads: 251

```
Messing with your acceleration throttle curve isn't too dangerous.  Be careful with the brake part (the left side)
```

---
## \#11 Posted by: strattos Posted at: 2018-08-07T23:29:32.521Z Reads: 243

```
Hmm interesting there doesnt seem to be as much customizability in ack's vesc tool. I can only find preconfigured throttle curves, that being said I'm running a +40% - 40% throttle/break Expo natural curves which gives really easy low end while still being able to zoom.
```

---
## \#12 Posted by: mmaner Posted at: 2018-08-08T00:10:14.365Z Reads: 236

```
You may not be looking at it right because there is a vast amount if customization available in @Ackmaniac 's firmware that isn't in any other variant.
```

---
## \#13 Posted by: DeathCookies Posted at: 2018-08-08T02:13:26.330Z Reads: 227

```
[quote="philvanzu, post:9, topic:64173"]
On my leiftech with winning v2 remote I set the same curve as Mmaner otherwise I don’t have enough control at low speeds because the acceleration is pretty brutal, on my Lacroix with GT2B I don’t feel the need to change it at all
[/quote]

I made the same experience and it is the Best example. In my case i tried it with a r2 and the nanox as Well as a gt2b mod. Because of the wide and sensitive Index finger control of the gt2b i dont need to change the throttle curve. At Low speed i can Start very well.
But if i use the nanox i get knocked off. I am not so used to the thumb Control and the Board launches like a missle. Therefor i change the throttle curve that i dont get Full Power at Low speed. Then i can press Full throttle but the Board will just Power it with for eg 50% which results in a smooth Start up. 

I recommend to try a throttle curve that is proven to be good and that makes sense. (we dont need 200% Power at 10% throttle at Low speed). Then you should fine tune it to your Needs. Everyone rides differently and has a different setup!
```

---
## \#14 Posted by: Lionpuncher Posted at: 2018-08-08T02:29:35.116Z Reads: 210

```
Would you care to screen shot your throttle curve? I think that would add a lot of value to those in the same boat.. (like me)... :sweat_smile:
```

---
## \#15 Posted by: DeathCookies Posted at: 2018-08-08T02:34:37.375Z Reads: 202

```
I am using a gt2b mod and therefore i have no throttle curve to share. I just made the same curve as manner just smoothed out instead of the sharp edges
```

---
## \#16 Posted by: strattos Posted at: 2018-08-08T06:57:55.597Z Reads: 204

```
![1533711358555183135326|690x388](upload://s6WaMwORDxp70rtGSsqof4Oi3W6.jpg)

@mmaner there doesn't seem to be the same customization here unless I'm blind just preset curves and percentage amounts.

This is with a thumb wheel remote and a 10% deadzone
```

---
## \#17 Posted by: Ackmaniac Posted at: 2018-08-08T07:39:22.834Z Reads: 198

```
I can recommend this settings

![image|500x500](upload://dJLouX7igFU6c0IyKkp5I1kpzhE.png)
```

---
## \#18 Posted by: dareno Posted at: 2018-08-08T07:41:29.967Z Reads: 191

```
That is actually the best explanation of throttle curves I've read so far.  I'm using the suck it and see method at the moment which is painfully slow.  Got my board feeling good now but just about to stick 12s in it and so it begins again lol
```

---
## \#19 Posted by: Lionpuncher Posted at: 2018-08-08T14:38:46.238Z Reads: 179

```
So this is a linear brake and an acceleration that starts smooth and becomes more aggressive the faster you go? Trying to understand the graphic. Pretend I'm really slow... :drooling_face:
```

---
## \#20 Posted by: mmaner Posted at: 2018-08-08T15:44:10.321Z Reads: 174

```
[quote="strattos, post:16, topic:64173"]
@mmaner there doesn’t seem to be the same customization here unless I’m blind just preset curves and percentage amounts.
[/quote]

I guess my confusion is that I thought you meant against other firmwares.  It seems there is less configurability between Acks 2.54 and 3.1 tools, but the same effect is achieved in actual use of the throttle curve.
```

---
## \#21 Posted by: mmaner Posted at: 2018-08-08T15:46:59.951Z Reads: 173

```
[quote="Lionpuncher, post:19, topic:64173"]
starts smooth and becomes more aggressive the faster you go?
[/quote]

That is correct.  Acceleration or brakes at lower speed are more dramatic without the curve, meaning 25% throttle = 25% power.  With the throttle curve lower speeds become more controllable and comfortable when 25% throttle = 12.5% power, or whatever is most comfortable to you

At higher speeds the throttle increase/decrease is far less dramatic so you make up the difference there.

Does that make sense?  I'm not sure it does but it's the best I can come up with :slight_smile:.
```

---
## \#23 Posted by: llreinzll Posted at: 2018-08-15T04:06:44.901Z Reads: 147

```
Wow. I just changed both throttle expo and throttle brake to -25%. I can't believe I didn't try this sooner. I also changed my battery regen to -15 from -10. (12S single drive 6374) 

With the 2.4ghz Nano remote and very short ride it already seems 100x better. With the thumb wheel it is now so much easier to modulate the throttle. 

Feels like I'm finally finished with this board. Well not exactly, still need bluetooth module and would like to upgrade to a focbox. Lol I guess we never stop tinkering right. It needs to stop raining up here in the northeast so i can just go out and ride.
```

---
## \#24 Posted by: Mikenopolis Posted at: 2018-08-15T04:09:54.813Z Reads: 146

```
[quote="llreinzll, post:23, topic:64173"]
Feels like I’m finally finished with this board
[/quote]

Yeah. I think I said that like 100 times per board
```

---
## \#25 Posted by: Lionpuncher Posted at: 2018-08-15T04:54:41.397Z Reads: 142

```
 Ya i found that out the hard way HAHA. Been playing a bit with the curve to mellow out. I'm getting close. I'll post once it's there.
```

---
## \#26 Posted by: DanielJohn Posted at: 2019-11-21T13:59:32.287Z Reads: 25

```
Would someone mind providing me some guidance?

When I release the thumb wheel, causing it to return to centre, the board rapidly decreases in speed almost throwing me off the front.

What setting do I need to tweak to make this a more gradual, smooth transition? Cheers
```

---
## \#27 Posted by: Tinp123 Posted at: 2019-11-21T14:02:06.035Z Reads: 25

```
positive and negative ramping time. try positive with 0.6s and negative with 0.5s. adjust accordingly.
```

---

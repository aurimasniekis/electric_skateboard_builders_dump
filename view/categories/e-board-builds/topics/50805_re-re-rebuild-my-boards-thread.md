# Re-Re-Rebuild my boards thread

### Replies: 40 Views: 2401

## \#1 Posted by: pat.speed Posted at: 2018-03-31T21:24:34.285Z Reads: 437

```
I currently have 2 esk8s one is a longboard and the other is  a short board (20”). They are both currently out of commission and waiting for parts to arrive so I can do some transplants and upgrades. 

**Build 1** 

This is going to be my high speed adrenaline board. I want it to have lots of torque as well as lots of speed (I know that’s what most want) here’s the plan

12s1p lipo
2x 190kv 6356
97mm clones
10:27 chain drive
2x Tb vescs 
Extra 19800uf cap bank
Hk trucks
2x Custom motor mounts
Custom styrene enclosure 

With those parts I’m looking at just over 50km/h top speed and 15-20km range.

So far I have the motors, batteries, vescs (thanks @Funktapus), capacitor bank, trucks and wheels, 1 motor mount and the chain drive. I’m only waiting on some plastic to make an enclosure from and some bits and bobs. Now onto some pics

This is the capacitor bank, it’s only about 25mm think you it can be laid on it’s side
![image|375x500](upload://ygcgyV5pztkGIAmI96UMkg6lOrg.jpeg)![image|375x500](upload://gHfMZgdyzKSWlGWYImcS4NBL1wG.jpeg)


And here’s a quick mock up of how it will fit, I also need to fit in a small charge only bms and a Bluetooth module for 1 Vesc 
![image|375x500](upload://7U5umDCqmAV7VUW9N9y8ZGxpz7p.jpeg)

Most of the parts will be here Monday/ Tuesday for a final mock up


Build 2 coming soon!
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-31T21:28:27.065Z Reads: 401

```
What's the extra capacitor bank for? (roast me if necessary :grin:)
```

---
## \#3 Posted by: pat.speed Posted at: 2018-03-31T21:30:55.619Z Reads: 396

```
No roast needed. It’s just for smoothing out extra voltage spikes. I’m kinda paranoid about running 12s on tb vescs so I want to try and do everything to stop them from frying
```

---
## \#4 Posted by: Acido Posted at: 2018-03-31T22:47:35.972Z Reads: 378

```
Dont risk it... Not worth it
```

---
## \#5 Posted by: pat.speed Posted at: 2018-03-31T22:54:47.481Z Reads: 378

```
Running 12s on tb vescs? I’ve seen lots of threads of people having no issues with 12s so I’m just going to give it a shot
```

---
## \#6 Posted by: mmaner Posted at: 2018-04-01T00:49:44.077Z Reads: 350

```
I'm running a 12s3p on the VESC's, 6 months not and no worries. One of the things I've found that helps is using a liberal throttle cirve so as to not throw too many amps in an instant at them.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-04-01T01:23:49.571Z Reads: 344

```
Thanks I’ll take it into account, can I change throttle curves with acmaniacs bldc tool?
```

---
## \#8 Posted by: mmaner Posted at: 2018-04-01T01:34:29.296Z Reads: 335

```
Yep, you can set brake and throttle curves. I'm out if town right now but I'll send you a screen shot when I get back home.
```

---
## \#9 Posted by: ervinelin Posted at: 2018-04-01T01:58:07.355Z Reads: 324

```
Confused how adding a curve will prevent this. Please share your screenshot when you are back.
```

---
## \#10 Posted by: mmaner Posted at: 2018-04-01T02:09:58.250Z Reads: 312

```
It prevents the delivery if a lot of amps quickly, as in it controls the ramp up.
```

---
## \#11 Posted by: ervinelin Posted at: 2018-04-01T02:32:51.136Z Reads: 298

```
Won't the curve just push this ramp up to a higher throttle level?
```

---
## \#12 Posted by: mmaner Posted at: 2018-04-01T02:44:12.310Z Reads: 293

```
No, it slows the range up hence the delivery of amperage
```

---
## \#13 Posted by: Apolo Posted at: 2018-04-01T03:34:56.554Z Reads: 294

```
Id do atleast 12s2p. More current = more torque. More torque = more speed available
```

---
## \#14 Posted by: Mobutusan Posted at: 2018-04-01T04:59:36.187Z Reads: 293

```
Keep in mind this is Lipo at 12s1p, so realistic, conservative output, depending an capacity and C rating should easily be at least 50-60+ amps. That threw me for a loop as well. I saw "speed board" and 12s1p and was like whaaat? :thinking: Oh, Lipos. NVM. :nerd_face:
```

---
## \#15 Posted by: Apolo Posted at: 2018-04-01T05:44:46.648Z Reads: 281

```
Aha

10char
```

---
## \#16 Posted by: pat.speed Posted at: 2018-04-01T07:54:42.714Z Reads: 281

```
Haha yeah, I love lipos, super easy to use and can be just as easy to charge as liion by adding a bms. And they are pretty much just as safe. 

From personal experience shorting a lipo does not cause it to catch fire, I shorted my first lipo multiple times and all that happened was the nickel strips split and burnt out. I see this as a great safety feature since it stops the short immediately
```

---
## \#17 Posted by: pat.speed Posted at: 2018-04-01T07:55:18.897Z Reads: 269

```
Thanks this is my first time using vescs and would rather not need to repair them
```

---
## \#18 Posted by: Blacksheep Posted at: 2018-04-01T10:35:12.097Z Reads: 269

```
me two please
```

---
## \#19 Posted by: pat.speed Posted at: 2018-04-05T11:41:52.976Z Reads: 278

```
**Build 2**

I have received most of the parts for the second build so I thought I’d start putting that together while I wait for the parts for the other build. This is more of a left over parts build with a few small upgrades.

Parts list:
Keda 6364 190kV
5x 2s zippy 5000mah 20c
Dual eBay esc (I broke 1 phase lead inside the esc so I’ll be running it in single drive)
10s bms (charge only)
Old longboard deck painted matte black
Enertion power wheels 83mm
China pulley kit (will get welded to the trucks)
Paris clone trucks

I think that is most of the parts so it’s time to get building

**Pics**

![image|374x500](upload://g0asgGmHRSuLE1myUoIPCccodCk.jpeg)![image|375x500](upload://cPEkqhs3UtjNX71ZXPq7z3dkmbN.jpeg)

Please mind the mess, having two board being built at the same time creates so much stuff. I’ll get some more pictures up as I build and should have some pics of the other board tomorrow
```

---
## \#20 Posted by: pat.speed Posted at: 2018-04-06T01:38:38.589Z Reads: 267

```
Finished the battery and connecting the bms. The esc is connected up and so is the motor. It’s time to build the enclosure.

![image|375x500](upload://19nVnpTi8bB79l9nSto9euFdq6b.jpeg)![image|375x500](upload://39lWdAOREghoObXa1ZOzgxsBKDf.jpeg)![image|375x500](upload://kSLyHLzCmTqapACAQlx3J98y8HS.jpeg)
```

---
## \#21 Posted by: pat.speed Posted at: 2018-04-06T02:29:40.981Z Reads: 255

```
It’s alive, it is now rideable. Well it’s ridebale around my house. This think is so smooth on start up, I’m pretty sure the esc runs foc because I don’t get a single stutter and I’m running sensorless

![image|374x499](upload://fjAsUupTXKgomlSgSU1Ltd4c7BW.jpeg)
```

---
## \#22 Posted by: pat.speed Posted at: 2018-04-10T04:29:55.272Z Reads: 243

```
Well shit, the seller who I ordered the 12s bms from has forgotten to actually put the bms in the packet. So I only received a 12s jst, just want I wanted. Let’s wait even longer now 👍🏻👍🏻👍🏻 Or maybe I’ll get them to ship express.

Anyway I tried making the case for build 2 today and it didn’t quite go to plan. I don’t think I ended up getting the plastic hot enough the first few times so I couldn’t pull it down over the buck. So instead, I just got the heat guns and heated each side then held it down with a ruler. It turned out subpar at best but it will do for now. 

I’ll get some pics up soon
```

---
## \#23 Posted by: pat.speed Posted at: 2018-04-10T05:15:44.202Z Reads: 246

```
![image|375x500](upload://ptGtktfbANH6LP9XkZ1cr8PoqQS.jpeg)![image|374x499](upload://9ARrH42nY5welCEAlVPT4FKNRon.jpeg)![image|666x500](upload://xYvYnV4CzMa0UJyJxGJYqklNkEE.jpeg)![image|374x500](upload://u3YXudYBnChh7jWjFQEjsHPGLWL.jpeg)![image|374x500](upload://721wzVftJomTxyh9altM6VolK3n.jpeg)

I will soon paint the enclosure black as I couldn’t get black plastic since it was out of stock. I will also get one of my mates to weld the motor mount onto the truck as I’m sick of this stupid thing, once that’s all done and I get the bms I’ll go and get some grip from my local skate shop.

As for build 1, well it’s gonna be a while. Stupid bloody seller, damn it. Anyway the Vescs are setup, the mounts a pretty much done just need some M6 nuts, the caps are finished and I’m only waiting on a bms, antispark from HobbyKing, and some more heatshrink for those phase leads, oh and risers cos this thing gets mad wheel bite with 97s

More picks. And yes that is a burn mark in the middle of the deck, don’t ask how!
![image|374x499](upload://5grnKo5xrJS07K7G1HXOGBbJ3jg.jpeg)![image|374x499](upload://9lZKqhKOMGlYic3OQARDtjpxOO2.jpeg)![image|375x500](upload://HtAYLtVeTP9kG3JSle4jFCixk4.jpeg)![image|375x500](upload://1uWqqZWaCooHBl5OnDzN7JeLRPK.jpeg)![image|374x500](upload://uVNjkEZcyqEhBL2xHE1QyftUn7k.jpeg)
```

---
## \#24 Posted by: pat.speed Posted at: 2018-04-11T03:19:05.739Z Reads: 224

```
Board 2 is now rideable, it just needs a bms so I don’t have to use balancers and I might weld the mount on still. Apart from that I’m quite happy, just need some grip tape.



![image|374x500](upload://hER2KNJ3KGlOHxLCg1Ec61rLGVD.jpeg)![image|374x500](upload://eDq8oIhWD81rzoM6OucgBNt6bhw.jpeg)![image|374x500](upload://odlg3BjsIlKLSDN3d7sb5s9evaT.jpeg)
```

---
## \#25 Posted by: Apolo Posted at: 2018-04-11T03:24:33.231Z Reads: 203

```
So he sent you a bms without the bms?
```

---
## \#26 Posted by: pat.speed Posted at: 2018-04-11T04:28:01.465Z Reads: 208

```
Yep... he replied once now he isn't. I might have to file a claim. 

It was a packet with 1 cable in it and that's it, IDK how you forget something like that

Edit: He has offered to send me a new one, at least he wasn’t trying to actually rip me off
```

---
## \#27 Posted by: pat.speed Posted at: 2018-04-14T08:17:51.489Z Reads: 211

```
Little update, I made the front panel that houses a voltage meter and power switch. I can’t decide if I should leave it white or paint it black, atm I like white.

![image|374x500](upload://eaqDEUGTTi6OBuiKD1cHP7En8U1.jpeg)![image|374x500](upload://48cmOHO6aVIGyDGxhPgXHbG41bo.jpeg)



Thanks @Deckoz for the idea of using an as150 bullet
```

---
## \#28 Posted by: pat.speed Posted at: 2018-04-30T09:25:27.668Z Reads: 198

```
It’s been a while since the last update and I have finally pretty much finished the drive train. The clamps and mounts I made are actually really sturdy and they sit a lot higher from the ground than the old ones, although they do sit a bit lower than I would like. I am going to try and wedge the rear truck slightly to try and gain a bit more height. I’m not sure what this will mean in terms of stability though, I guess I’ll just have to wait and see.

![image|375x500](upload://tMVWXvts433rIv8Pr4no9wLK3Yh.jpeg)
```

---
## \#29 Posted by: pat.speed Posted at: 2018-06-05T09:22:58.697Z Reads: 179

```
Ok so I haven’t updated this in a while and I’ve jusg made a few minor modifications that should be the last ones (except I still need to grip the board)

After my mate welding the mount it managed to vibrate loose probably due to only a small bead. This time I got him to weld all the way around and I think this thing is definitely not coming off now, we also glossed the board while we were at it.

![image|375x500](upload://imoFDpykG8nWhYaQWY1IidoE3cF.jpeg)![image|375x500](upload://rUnLBc25Nc7JgOKnXqAqgS4ytME.jpeg)

I also got a new battle scar to the case from coming up the edge of the driveway to sharply ☹️ Oh well scars make you look cooler I guess 😉
```

---
## \#30 Posted by: githigh Posted at: 2018-06-26T07:20:25.173Z Reads: 159

```
What BMS did you use on the 5 lipo build? You have a wiring diagram for it? Dimensions of the batts? Looking to duplicate this setup for a short board.
```

---
## \#31 Posted by: githigh Posted at: 2018-06-26T07:21:07.861Z Reads: 157

```
I might go 3x2S for 6s on that build, but still considering all options at the moment.
```

---
## \#32 Posted by: pat.speed Posted at: 2018-06-26T07:30:16.875Z Reads: 156

```
I think the pack is about 40-50mm long and the bms was one off eBay, although I would recommend a big one that has a higher balancing current.

I highly recommend 10s for a nice cruising board that still has moderate range and power. Another option is 3x 3s for 9s and the pack will be a lot shorter and more compact for a small build
```

---
## \#33 Posted by: Acido Posted at: 2018-06-26T09:24:13.593Z Reads: 146

```
where did you get the sprockets?
```

---
## \#34 Posted by: pat.speed Posted at: 2018-06-26T12:14:07.045Z Reads: 143

```
I got them off ebay, they were $15 AUD, but I ended up also ordering new motor sprockets as the original ones made the gear ratio 1:1.9, the new gear ratio is 1:2.7. It has plenty of torque
```

---
## \#35 Posted by: Acido Posted at: 2018-06-26T12:36:40.988Z Reads: 136

```
the one with the 4 holes already drilled?
```

---
## \#36 Posted by: pat.speed Posted at: 2018-06-26T21:08:15.254Z Reads: 134

```
Yes, I re-drilled the holes out to 7mm and it works fine, but I eventually going to 3D print a pulley holder for flywheels
```

---
## \#37 Posted by: pat.speed Posted at: 2018-07-04T04:19:37.173Z Reads: 130

```
Build 2 is finally finished and working fine for the time being, although I might change trucks and mounts in the future for aesthetic purposes, I finally got around to gripping the top. 

 ![IMG_1649|375x500](upload://aTs5YDQub6X0CUe86ORVjwppOVA.JPG)![IMG_1650|375x500](upload://nYOKrLRHeYEnWQoofYpKb7END8P.JPG)![IMG_1648|374x500](upload://bwS2oA5AAghaXcVEF4arceNJOVL.jpg)

Board 1 is also almost finished, I just need to attach the enclosure and possibly paint it. If you guys see anything potentially problematic let me know, 2 sets of eyes is better than one! 

![IMG_1654|375x500](upload://o1fGk7VqPQGQNkj3V8LjsephkSD.JPG)![IMG_1651|375x500](upload://2AmkgXIkVCtYhl7iFXBE8pMaZCa.JPG)![IMG_1652|375x500](upload://ApDpgaXLswQYjS9a6OjfeNlMwXC.JPG)![IMG_1653|375x500](upload://ozAJdhOLfA5R10n8HZzR09vM3ab.JPG)

What colour should I paint the enclosure? what do you guys think will look good? Let me know
```

---
## \#38 Posted by: Superflim Posted at: 2018-08-08T12:18:13.581Z Reads: 98

```
Broo that's so clean. :star_struck:
```

---
## \#39 Posted by: Skunk Posted at: 2018-08-08T12:20:37.488Z Reads: 95

```
Damn that Awol deck.... do want

Did you ever paint the enclosure?
```

---
## \#40 Posted by: pat.speed Posted at: 2018-08-08T22:02:12.741Z Reads: 88

```
@Superflim Thanks man

@Skunk Nah, I never ended up painting it, I have come to actually quite like the plain alu look
```

---

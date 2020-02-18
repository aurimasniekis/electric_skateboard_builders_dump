# \[Help\] &#124; 27&rdquo; Deck &#124; Caliber Trucks &#124; Single R-SPEC 190kv Motor &#124; Enertion Mount &#124; 6S &#124; VESC

### Replies: 18 Views: 2859

## \#1 Posted by: loganrhyne Posted at: 2015-12-24T17:57:32.782Z Reads: 205

```
Hi guys,

Just got bitten by this bug yesterday after helping my brother with the first steps of his build and have been reading through the forum here and at ES making a parts list for my own build.

Looking to put together something compact and relatively light; will be using it to commute ~2-3 miles over flat roads.

I've put together a detailed parts list here: https://docs.google.com/spreadsheets/d/1RNYZZSbDeuusBSgbq1e1CRSRdVisJzE7fKbwjH5OkD8/edit?usp=sharing but the gist of it is 6s2p (if I have the nomenclature right) with VESC and the beefier of the enertion motors.

I'd love general feedback on the compatibility of this setup; it seems roughly similar to some of the smaller builds on the forum. I don't need to scrape the bottom of the barrel in terms of cost and would like to build something that I could expand (mostly in terms of adding cells for longer range) if this turns out to be a viable form of transportation for me. Also verification that the charging setup (charging the two 3s1p in series with the listed charger) makes sense would be reassuring.

I also have a few specific questions; I'm largely new to the world of DIY electronics so these stem mostly from the lack of experience/understanding with the wiring for the battery/esc/motor circuit.

1. The Enertion R-Spec has 5.5mm connectors and the Zippy batteries have 4mm connectors. It's unclear what the connectors on the VESC will be. What's the best way to handle these size differences? I'm not adverse to stripping the connectors and soldering the connections, but maintaining modularity seems valuable. Do people just make their own adapters to go from one size to another?

2. *How necessary is the anti-spark board? I've been able to dig through details for lots of the other aspects of the circuit, but I'm still unclear on the purpose and necessity of the anti-spark, as well as where I would get one and how it is incorporated into the circuit? Even just a pointer another discussion that lays it out for an electronics neophyte  would be awesome.* **Read a bit more and just purchased the Ollin VESC with the integrated anti-spark.** 

3. I'm totally entranced by the cleanliness of this build: DIY Electro-Trampa and boosted inspired electric longboard (https://endless-sphere.com/forums/viewtopic.php?f=35&t=73230) and am curious if anyone has insights into the connections he used as the charger and balance ports? I also posted a reply in his build thread so if I find out from there I'll include it here in my thread.

4. What are the kinds of little bits and pieces that are often overlooked when getting together a build from scratch? Anything in terms of major components or bits and pieces that I'm missing from my list?

I wanted to get feedback on parts and the general idea for the build before buying parts. I'll keep posting updates as I learn more and add pictures once I start ordering stuff and assembling.

Thanks in advance for help and advice; looking forward to sharing as I go!
```

---
## \#2 Posted by: cmatson Posted at: 2015-12-24T20:53:38.807Z Reads: 197

```
Looks awesome so far, and is very similar to my first build! 

as for the connections, I know if you message @chaka (who owns ollinboards) you can get some level of customization as for which connections you want on your VESC. 

**A couple things to keep in mind:**
-I don't think the deck you picked comes with griptape, so you'll either need to add that or choose another deck.

-what are your plans for that power switch? it won't carry the volts/amps necessary to just put in line between the batteries and the VESC, so I'm not to sure where it would go.

A couple deck related things to consider though: does it have flex? is it long enough?  with flex, you run the risk of breaking components (like batteries) that don't flex; and sense your board is so short, you probably won't be able to make two enclosures like the diy boosted board has. The reason he did that was to allow flex in the middle.

so I'd suggest possibly choosing either a longer deck, or one where you know for sure it's stiff. 

Then for enclures, I highly recommend the ones @psychotiller makes. They are clean, and you can get whatever size you want- he also does custom shapes by request. You can check out a pic of some of them here: <img src="/uploads/db1493/original/2X/e/ea73683fe9e00883d35e9b6bffa628bd8dce03d0.png" width="690" height="386">

After that, the only MISC things I can see you needing are screws to mount down the enclosure. Alot of people use a bolt/wingnut setup to allow easy removal of the case, but that's all up to you!

for balancing/charging you can either have the batteries be removable, or simply allow for the balancing leads to be accessed through the side of the enclure. Maybe @lowGuido can post a pic of his charging setup on this thread so you can see a good example of that.  

You definitely have a  really great start as far as picking out the right stuff :smile:

looking forward to seeing more!


----------


**EDIT:** I'd actually change your motor to a higher KV than 190. with a 6s lipo and 190kv, you are probably looking at less than 15mph with the included gearing from your mounting setup. I'd try something in the 210-245 range if you can. I know @torqueboards has one (it is also sensored for smoother startup!) here that is 230kv: 
product/electric-skateboard-motor-6355-230kv-2650w/

it'd also bring your overall cost down, and you could order a mounting setup from diyelectricskateboard too if you wanted everything to be shipped from the US (i.e. I'd be cheaper again)

edit again.. haha just keep thinking of possible helpful things to add! Here's a thread where some people have shared their builds and specs:

http://www.electric-skateboard.builders/t/diy-eboard-builds-and-specs/33/37
In addition there are a ton of good build logs here on the forum both complete and in progress. I recommend you just take a look around, and it should help alot!
```

---
## \#3 Posted by: cmatson Posted at: 2015-12-24T20:54:50.767Z Reads: 167

```
also one more thing for the charger: I highly recommend this little guy (just a couple more bucks on amazon) as I have been using it for a while now with no issues:

http://www.amazon.com/Combo-Special-Tenergy-Balance-Charger/dp/B00466PKE0/ref=sr_1_3?ie=UTF8&qid=1450990441&sr=8-3&keywords=lipo+charger
```

---
## \#4 Posted by: NNGG Posted at: 2015-12-24T22:00:33.577Z Reads: 161

```
Do you think a 149kv motor on 8S at a 16/36 gearing is too slow?
```

---
## \#5 Posted by: cmatson Posted at: 2015-12-24T23:06:13.894Z Reads: 155

```
I think the perfect combos are:
230-245 -6s
190 -8s
149-170 -10s/12s

I've tried 6s, 8s, and 10s, and both 245 and 190 motors.
```

---
## \#6 Posted by: NNGG Posted at: 2015-12-24T23:07:59.643Z Reads: 149

```
K thanks, wondering how a vesc would handle 10-12s tho
```

---
## \#7 Posted by: cmatson Posted at: 2015-12-24T23:17:00.547Z Reads: 145

```
The VESC will handle all the way up to 12s- A lot of people also run it with the space cell which is 10s.

But let's not hijack this thread :smile:
```

---
## \#8 Posted by: loganrhyne Posted at: 2015-12-25T03:56:23.874Z Reads: 154

```
@cmatson Thanks so much for all your thoughts! Much appreciated.

I've switched out the parts list to grab the DIYes adjustable mount kit and 230kv motor as well as the recommended charger.

Was thinking that the 14/36 gearing is a nice, middle-of-the-road option?

My plan is actually to build up and get the electrics all working (or at least have it in hand) to have an in-person feel of the scale and then pick out a board. I really like the dual enclosure look and the practicality of allowing a bit more flex. There's a skate shop in Palo Alto and I might demo some different boards to get a feel for what works for me.

As for the enclosures, @psychotiller's look amazing; my first hope is that someone at work has a 3d printer and will help me design and print a simple dual-enclosure setup, but if not I'll definitely get in touch to get something made up.

Lastly, wrt to the power switch, I'm trying to get a setup that looks like this: http://i.imgur.com/nfCSnhJ.jpg. I don't (clearly) know enough about circuit design to understand how to find the right kind of switch, but that's what I was going for. Any directional guidance there would be super helpful.

Thanks for the link to the builds & specs topic; I'm definitely still working my way through the mountain of awesome, detailed content in the forum.
```

---
## \#9 Posted by: barajabali Posted at: 2015-12-25T05:28:59.597Z Reads: 149

```
I have that motor and i cant get it to reverse. Do you know how to reverse it? im running it sensored on the fvt 120 amp esc. Thanks
```

---
## \#10 Posted by: cmatson Posted at: 2015-12-25T17:15:32.363Z Reads: 155

```
haha first off, Merry Christmas! 

As for the deck idea, I love it. Try before you buy! whether or not you like a deck all boils down to how it rides, regardless of the looks.

gearing sounds good too. And for the switch, It's just a matter of finding something that can handle more power. I totally get the look you are going for- haha that diy boosted board is absolutely sweet!  I know DIYes has one, but it's $60... 

Have you thought about a simple loop switch that doubles as a key? there is a helpful thread about making one here: 
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

I haven't seen many 3D printed enclosures, but I can't wait to see what you bring to the table! I think the hardest thing is making a casing thick enough, but not having it be overly bulky. Do you know if there is a somewhat flexible filament that would handle road vibrations better? I've only 3D printed small things like go pro mounts, but I'm not sure how well hard plastic will handle road vibrations over time- an interesting experiment none the less! 

As for switching the direction of the motor @barajabali, I'm not sure... You'll have to consult @torqueboards for that.
```

---
## \#11 Posted by: lox897 Posted at: 2015-12-25T22:41:09.362Z Reads: 126

```
NinjaFlex can flex pretty well. I'm not sure how expensive it is though.
```

---
## \#12 Posted by: loganrhyne Posted at: 2015-12-26T04:30:52.973Z Reads: 130

```
Merry Christmas to you too!

Thanks for the link to the anti-spark loop key; will keep that in mind as I go forward. Thinking at this point I'll just order the basics of the circuit and attempt to get that working and can then fancy it up on the connectors and on/off switch/key.

Saw the 3D printed enclosures on this build: https://endless-sphere.com/forums/viewtopic.php?f=35&t=74882&p=1130345&hilit=3d+printed#p1130345. Thought they looked nice and clean and simple. I might also experiment with vacuforming ABS as that seems within the range of my experimenting abilities.
```

---
## \#13 Posted by: mccloed Posted at: 2015-12-27T04:58:25.392Z Reads: 126

```
Hey @barajabali,You may want to change the motor wires around until it works. If the hall sensors are not arranged correctly you mat only be able to do forward.
```

---
## \#14 Posted by: barajabali Posted at: 2015-12-27T06:57:19.711Z Reads: 124

```
im just assuming that the hall sensors are arranged correctly because thats how they came, they came prewired into a plug which fits into the ESC. and i tried some messing around with the 3 phase wires before and fired a brand new 65 dollar esc :( any help would be great. im not getting any resonce from torque boards.
```

---
## \#15 Posted by: barajabali Posted at: 2015-12-27T06:58:49.583Z Reads: 123

```
He told me that id have to program it to reverse (which i did) but when i engaged the throttle the motor engages in breaks.
```

---
## \#16 Posted by: NNGG Posted at: 2015-12-28T00:05:45.596Z Reads: 119

```
Are there any precautions when using a VESC and 12S with a low kv motor, like 149kv?
```

---
## \#17 Posted by: cmatson Posted at: 2015-12-28T01:08:15.539Z Reads: 122

```
I've seen a bunch of people use vesc's on 12s with no problems. 

You just have to use a motor with less than 200kv. Some people put limits on the top speed to keep it at a more manageable level too.
```

---
## \#18 Posted by: NNGG Posted at: 2015-12-28T02:56:12.889Z Reads: 118

```
Thanks, I don't have anywhere I can go faster than 30kph anyway so I think Im good with 149kv at
 8-10S
```

---

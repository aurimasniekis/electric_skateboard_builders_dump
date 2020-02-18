# 10s3p Samsung 30Q Build Check

### Replies: 38 Views: 1070

## \#1 Posted by: boogiewookie Posted at: 2018-11-03T20:59:06.140Z Reads: 203

```
Hey guys I've been lurking on this sub for a while, and finally got the Boss Level Spot welder to spot weld the batteries together. 
Could you guys check if this seems like a safe battery? I only hot-glued the 3 batteries together, and left each parallel group to get some flex. I used separate nickel strips for the balance wire for the BMS besides the last one B10 (36V). 
Did not realize the amount of time and care it takes to build these things before I started lol 
All I need to do is connect the positive and negative to the batteries and connect the charge port. 
I'm thinking of adding some neoprene foam and fish paper before I wrap this in heat shrink. 
Does this look good?
![IMG_20181018_180938|375x500](upload://19GCLqm2UjpVifc3RNdHBCDiDnA.jpeg) ![IMG_20181031_160756|375x500](upload://eC8Nhi11Y698NSrc3PLYCzu7fy7.jpeg) ![IMG_20181102_213435|666x500](upload://7l3tC3zGOyKFW5HeajoYK1YXLFo.jpeg) ![IMG_20181103_010651|375x500](upload://iqyvm2ZRVggOR9lcbPfLDzM5Pee.jpeg) ![IMG_20181103_010701|375x500](upload://2Uw7l3VYRlAGFu5ek2unlE1SSec.jpeg) ![IMG_20181103_010822|375x500](upload://gpZBo8k1OUk9HoVvq62bFQ4pl5P.jpeg) ![IMG_20181103_124110|666x500](upload://8Cr4uIae0FvziG83cv8ZfS81eJa.jpeg)![IMG_20181103_164814|666x500](upload://9IPxQcLERMBGEghZ3jI0CiasBmT.jpeg)
```

---
## \#2 Posted by: JosephShubin Posted at: 2018-11-04T01:31:02.922Z Reads: 171

```
I'll be building a very similar battery, using the same cells when I get to building my electric longboard. Good luck and be careful! :slight_smile:
```

---
## \#3 Posted by: boogiewookie Posted at: 2018-11-04T03:04:23.969Z Reads: 168

```
Yeah I almost burnt my cells when I was careless cutting the nickel strips near the cells hahaha 
thank god I only got away with a burn.
```

---
## \#4 Posted by: kuphjr Posted at: 2018-11-04T03:57:19.273Z Reads: 165

```
I would certainly recommend adding another layer of fish paper where your batteries touch in the middle just to  be safe.  That is an easy place a short could occur.  You can never go wrong by always wrapping all battery terminals in fish paper and using heat shrink tube to keep everything tight.
```

---
## \#5 Posted by: kuphjr Posted at: 2018-11-04T04:00:39.119Z Reads: 159

```
I know fish paper is available on Amazon but I don't think they have any with adhesive backing so you have to tape it around each row of cells.  I bought my adhesive backed fish paper in a in a 5' roll.

I would ship you some for the cost of shipping but I just ran out. :frowning:
```

---
## \#6 Posted by: legend27 Posted at: 2018-11-04T07:48:38.364Z Reads: 145

```
Looks good to me! Only thing I would change was to put fish paper under all the balance wires. And that last balance wire on the other site would I cut a bit shorter.
```

---
## \#7 Posted by: Maxid Posted at: 2018-11-04T09:34:10.016Z Reads: 146

```
Why didn't you put the balance wires on the side with the series wiring? Now you have two sides with protrusions instead of only one and a flat side.
```

---
## \#8 Posted by: boogiewookie Posted at: 2018-11-04T16:24:54.237Z Reads: 129

```
Yeah I was actually worried about that I think that's actually a great idea. I already put fish paper, but I think I'll untape and add another layer just like you said. There's so many cases of DIY batteries going bad and catching fire. 
@legend27  I didn't even think to cut the balance wires instead of bending them great idea! Thanks 
@Maxid I heard that separating the balance wires from the series connections were vital because it heats up and could cause shorts in the circuit. at least that's what @Eboosted said
```

---
## \#9 Posted by: Eboosted Posted at: 2018-11-05T16:03:54.684Z Reads: 121

```
[quote="boogiewookie, post:1, topic:73294"]
et some flex. I used separate nickel strips for the balance wire for the BMS besides the last one B10 (36V).
Did not realize the amount of time and care it takes to build these things before I started lol
All I need to do is connect the positive and negative to the batteries and connect the charge port.
I’m thinking of adding som
[/quote]

Looks reat but you need to use additiona fish paper here:

![image|114x94](upload://9GnZZt8XpIdL2N6rC3noLmXa9oO.jpeg) 

These two strips are too close together, if there's a crash or some accident they could touh each other and start a fire.

Also use fish paper between cells and balance wires.

You also must use fish paper between each P-Group, remember this is the main cause of fire.
```

---
## \#10 Posted by: boogiewookie Posted at: 2018-11-08T01:40:33.705Z Reads: 111

```
Thanks for your input @Eboosted
I did what you said and put some extra fish paper in between the parallel groups so there would be no shorts. 
But I'm having some problem trying to power the VESC using the BMS P- and positive lead straight from the battery. 
![IMG_20181107_202834|375x500](upload://lxbLkmBoMZUzz88jdKNckyiBrJm.jpeg) 
![IMG_20181107_202852|375x500](upload://kgtmS0fY16wHkRcQyvsxNdFxuGX.jpeg) 
I shorted the eswitch and plugged it into my VESC to check if it works, but I don't get any lights. 
I tried to see if there was a problem with the wires so I shorted the pins from the back of the BMS like this, which didn't help the problem. '![IMG_20181107_202900|666x500](upload://q1TZlp5gQ4wuDWvpavVCCJ9l0aQ.jpeg) 
 I also checked the voltage for each cell from the balance wires to see if there were any shorts, but there were no irregularities from cell to cell. 
I'm charging the pack right now to see if a fully charged pack would resolve the issue (it might be triggering nominal voltage, but I doubt that's the case because the voltage of the pack is 37V right now.) , but one thing I notice is the heatsink gets extremely hot when I'm charging it. I can't even touch it for more than a second without pain. Is this normal? 
The only way to get the pack to power the VESC is when it is only charged and as soon as I unplug it it doesn't work. 
I wired everything correctly, but I can't seem to find a solution. 
@kuphjr @legend27 @Maxid @Namasaki I could really use your help. or anyone else.
```

---
## \#11 Posted by: boogiewookie Posted at: 2018-11-08T02:42:00.952Z Reads: 100

```
Okay new update. The charging stopped working for some reason. 
I have no clue what is going on with this.
```

---
## \#12 Posted by: kuphjr Posted at: 2018-11-08T04:07:52.279Z Reads: 94

```
 I’m really out of my depth since I have never used this specific and BMS before, but are you sure the switch is supposed to be shorted? Most buttons I have used for anti spark switches are momentary buttons and do not act like a switch.
```

---
## \#13 Posted by: kuphjr Posted at: 2018-11-08T04:08:56.895Z Reads: 95

```
Honestly, completely disconnect your BMS. You might need a new one.
```

---
## \#14 Posted by: kuphjr Posted at: 2018-11-08T04:13:23.659Z Reads: 94

```
I highly recommend the discharge only BMS. Cheap, small & easy. If you did indeed break this BMS or if you recieved it damaged, you can get one with super fast US shipping from BuildKitBoards.com @JLabs.

Since the VESC is really reliable about cutting off before the battery is over discharged, there isn’t much benefit to a discharge BMS. Just get a $2 50-60A auto fuse to protect your battery in case too much current is drawn for some reason.
```

---
## \#15 Posted by: boogiewookie Posted at: 2018-11-08T04:42:18.972Z Reads: 87

```
I've read a couple of posts saying shorting the E switch would solve their problems of their battery not turning on.
Yeah I think so too it's so annoying to find out I gotta redo everything and it wasn't even my fault.
If ai buy a new one I gotta open the pack up and redo all the balance wires so I might just end up getting the same on I bought I hope I can get some compensation
```

---
## \#16 Posted by: legend27 Posted at: 2018-11-08T05:58:30.194Z Reads: 82

```
Think you wired the bms wrong.
```

---
## \#17 Posted by: lrdesigns Posted at: 2018-11-08T06:26:45.619Z Reads: 86

```
This would have been a great post to put in this thread, I created it to try and get all the battery build info in one area so it could be a more convenient resource for all. 

https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102?u=lrdesigns

I think you did pretty good on your first pack and most of all the extra tips you needed have already been said above. I would just add that the silicone wires you used to connect the p-groups, I would use a two thinner gauge instead of one thick one. As it's easier to solder, more flexible and less thickness. Or braided strap.  

Although already said, insulate between each p-group. If the cell shrink is compromised between two p-groups it can short. It is not really obvious at first. 

![image|649x500](upload://5vmZTo1vlaJemFcgCDuk49zZkq1.jpeg)
```

---
## \#18 Posted by: boogiewookie Posted at: 2018-11-08T13:48:27.808Z Reads: 77

```
Here's how I wired the BMS
1. BMS P- to VESC Out -
2. Battery + to VESC Out +
3. Battery - to BMS B-
4. Battery + to Charger +
5. Charger - to BMS C-
Isn't this correct? 

@Irdesigns Maybe I can post a post on this thread on that thread to find a solution. I mean I already put some fish paper between the p groups and if there was a short, there should be some discrepancy when I measured the voltage of each cell through the balance wire right? it just doesn't add up. All I can say is that it just might be a faulty BMS, but that doesn't seem likely either.
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-11-08T14:08:31.969Z Reads: 77

```
There should be no shorts in the battery at this stage. Pack looks fine.  All the extra precaution / insulation is mostly vibration / crash proofing, an esk8 is a harsh environment for a battery. 

You probably have some BMS issue. :worried: Tricky to solve over forum. Usually need to see the manufactures diagram and really clear photos of where all the balance leads /power wires go. And maybe even hand drawn diagram of how you think you wired it. 

You may have killed it also 😢. Many people have on their first go don’t feel bad. Could have been dead on arrival. 

Im not BMS expert, but if you have the manufacturer diagram and really clear photo of all the wires leading to the BMS maybe someone here can figure it out.
```

---
## \#20 Posted by: lrdesigns Posted at: 2018-11-09T01:38:14.971Z Reads: 53

```
who makes the BMS, model number?
```

---
## \#21 Posted by: boogiewookie Posted at: 2018-11-09T01:44:34.305Z Reads: 46

```
Bestech D596 is the model number. I'm actually trying to solder the switch on if that makes a difference instead of shorting it. 
I will post a wiring diagram soon once I finish my homework. :)
```

---
## \#22 Posted by: lrdesigns Posted at: 2018-11-09T01:50:01.565Z Reads: 52

```
[quote="boogiewookie, post:21, topic:73294"]
Bestech D596
[/quote]

Ok get back to your homework :books: and stop slacking!!! Hahah.

I found a thread on this BMS already with a wire diagram. 

https://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14?u=lrdesigns
```

---
## \#23 Posted by: boogiewookie Posted at: 2018-11-09T01:57:36.564Z Reads: 47

```
hahaha dude this battery has been on my mind this whole day I'm super pissed. 
Yeah I looked at that thread to follow precisely the wiring diagram they provided me. 
Honestly I'm fed up with this BMS it's bullshit the eswitch never even ended up working, and ultimately made the BMS die on me. I got this from @hyperIon2 @hyperIon1 but they don't seem to care enough to email me back a response.  
I think I'm gunna get the D140 charge only BMS or something else if you have any recommendations. 
Just gotta make sure to make a ghetto anti spark plug with an XT90  right?
```

---
## \#24 Posted by: lrdesigns Posted at: 2018-11-09T02:00:12.310Z Reads: 48

```
XT90-S   Its not really getto its proven to be way more reliable and safer than e-switches. It just does not look as nice. Many here prefer them after blowing up many eswitches. 

https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html?___store=en_us
```

---
## \#25 Posted by: boogiewookie Posted at: 2018-11-09T02:05:49.382Z Reads: 46

```
Yeah I ordered a bunch of XT90 just to be on the safe side of things. 
Do you have any recommendations for charge only BMS?
```

---
## \#26 Posted by: hyperIon1 Posted at: 2018-11-09T02:06:48.636Z Reads: 47

```
I did email you a response, and if a d140 will satisfy you I’ll send one tomorrow
```

---
## \#27 Posted by: hyperIon1 Posted at: 2018-11-09T02:12:15.401Z Reads: 49

```
We do care. So much so we will send the D140 for free because the one you have doesn’t work. 
![image|281x499](upload://7dhzceB34ha7XQKaKp8E5ThhgQU.jpeg)
```

---
## \#28 Posted by: lrdesigns Posted at: 2018-11-09T02:12:41.065Z Reads: 46

```
[quote="boogiewookie, post:25, topic:73294"]
Yeah I ordered a bunch of XT90
[/quote]

Maybe a typo but you need the (s) version, XT90-S not the regular XT90.
```

---
## \#29 Posted by: boogiewookie Posted at: 2018-11-09T02:18:52.617Z Reads: 41

```
I'm so sorry I didn't see your email. I was waiting for it all day, but didn't even realize it came when I was asleep. I actually tried shorting the eswitch as soon as I finished soldering all the connectors to the battery.(cause that's how switches work) that was my first instinct, but I still couldn't get it to power my VESC you can see from the pictures I posted. I'm sorry again for my haste comment. 
It'd be amazing if you could send me a D140.
```

---
## \#30 Posted by: hyperIon1 Posted at: 2018-11-09T02:20:24.478Z Reads: 41

```
To be honest. We don’t offer those tanks anymore because they have so many problems. 
I have a d140 with your name on it.
```

---
## \#31 Posted by: hyperIon1 Posted at: 2018-11-09T02:26:03.653Z Reads: 41

```
I’ll mail it  in the morning with tracking
```

---
## \#32 Posted by: boogiewookie Posted at: 2018-11-09T02:31:47.692Z Reads: 37

```
Thank you so much. again I apologize for my foolishness.
```

---
## \#33 Posted by: hyperIon1 Posted at: 2018-11-09T02:32:16.264Z Reads: 37

```
Actually I’m going to send you a new bms unit we are currently using in our builds. It’s self contained and super easy to wire.
```

---
## \#34 Posted by: hyperIon1 Posted at: 2018-11-09T02:34:22.336Z Reads: 43

```
![image|412x499](upload://rKgq7AMTvQsTd2gODCwe1FZACeL.jpeg)
```

---
## \#35 Posted by: hyperIon1 Posted at: 2018-11-09T02:35:07.574Z Reads: 42

```
I’ll send a loop key as well and you can test it out for us. 
Cool?
```

---
## \#36 Posted by: b264 Posted at: 2018-11-09T02:38:37.612Z Reads: 43

```
I would recommend the series connections go across the middle, that reduces the chance it can short in the middle from one side to the other

![connections|610x460](upload://abaq8WOXm5Cc1sQiBRd5nC6sJoz.png)

to elimnate the need for the extra fishpaper @Eboosted suggested
https://www.electric-skateboard.builders/t/10s3p-samsung-30q-build-check/73294/9?u=b264
```

---
## \#37 Posted by: boogiewookie Posted at: 2018-11-09T02:49:00.832Z Reads: 36

```
that sounds awesome. this works for 10s right? cause the specification sheet says 12s
```

---
## \#38 Posted by: hyperIon1 Posted at: 2018-11-09T03:20:00.937Z Reads: 35

```
Yes, the data sheet is for 12s but it comes in 10s.
```

---

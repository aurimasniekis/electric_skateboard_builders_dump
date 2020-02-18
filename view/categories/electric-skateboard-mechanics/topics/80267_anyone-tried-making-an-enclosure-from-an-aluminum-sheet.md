# Anyone tried making an enclosure from an aluminum sheet?

### Replies: 18 Views: 444

## \#1 Posted by: Slydunan Posted at: 2019-01-08T05:37:32.380Z Reads: 182

```
Im thinking about velcro strapping the battery to the board and then bending an aluminum sheet to make a cover. Would that work?

Potential issues i can think of:
Connection interference with the vesc and remote?
Dont know what alloy and thickness would be ideal ...too bendy/malleable or too heavy/unworkable?
```

---
## \#2 Posted by: monsterbuilder Posted at: 2019-01-08T05:43:00.845Z Reads: 182

```
Aluminum will conduct electricity.  So probably not a good idea.
```

---
## \#3 Posted by: JdogAwesome Posted at: 2019-01-08T05:47:52.658Z Reads: 175

```
I guess thats why Tesla's are made of gingerbread right? Lol as long as your board is built well and you dont have a bunch of open connections and batteries flying around inside an aluminum enclosure would be a great idea and offer a lot of protection. 

@Slydunan connection issues should not be a problem because the enclosure would be below you and it would only have to pass through the wood of the board, unless your planning on having it wrap under the components as well?  Also you would probably want to make sure everything inside the board was secured down well and the aluminium just acted as a shield, rather than a bucket probably.
```

---
## \#4 Posted by: Slydunan Posted at: 2019-01-08T05:49:51.774Z Reads: 170

```
If theres no loose connections that wont be a problem no?
```

---
## \#5 Posted by: pixelsilva Posted at: 2019-01-08T07:03:10.265Z Reads: 163

```
Cars been around for almost 130 years now and nobody freaks out because they carry highly inflamable gas fuel inside their thanks! They are running bombs...for lack of a better word. So, some stupid enclosure made out of a stupid material like simple boring aluminum represent no danger for battery cell storage. Like @JdogAwesome  mentioned before, Tesla automobiles are completely made out of aluminum and they carry some of the largest and most powerful battery cells known to men.
```

---
## \#6 Posted by: Gamer43 Posted at: 2019-01-08T07:19:14.239Z Reads: 154

```
I made an enclosure completely out of aluminum. Ran 10S lipo using the SPIM08HPs from alarmhookup on ebay. Used shrouded XT60 connectors for everything, mounted electronics to a piece of plywood that was mounted on standoffs. Used PU packing foam to fill in any gaps between the battery pack and the enclosure. 

Flipped my board over and cracked my skull. Everything inside the enclosure was perfectly fine and works like nothing happened. 

Remote range was reduced since I also had sheet metal covering the top since my board is curved, but for the most part worked fine. Although I did leave one of the ends open, so that might give me more range than a completely sealed enclosure.

My advice is don't bend aluminum sheet, that's a pain. I used 2" and 3/4" aluminum angle (use smaller angle if you don't need the height and want more ground clearance), cut it to length, drilled holes in the sheet metal and angle to bolt everything together using #6 machine screws.
Sheet was .032" thick 5052, angle was 1/16" thick 6061.
I did have to cut pieces out of the angle with a hacksaw in order to close up the ends though.
Enclosure weighs about 3-4 pounds and measures 24" x 7" x 2". The top cover measured 28" x 8.5" was made out of sheet metal.
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-01-08T07:19:29.864Z Reads: 146

```
[quote="JdogAwesome, post:3, topic:80267"]
I guess thats why Tesla’s are made of gingerbread right?
[/quote]

&lrm; plus1
```

---
## \#8 Posted by: ShutterShock Posted at: 2019-01-08T08:16:58.919Z Reads: 139

```
This is along the lines of what I was thinking.  As long as everything is well padded and sheilded from the batteries ever coming in contact with the metal, should be good. 

Keep in mind that with all the vibrations, sometimes the plastic coating and cover on the outside of lipo patches can actually wear completely through, exposing the actual pouch to your enclosure.  Would hate to have that happen on metal.  Just make sure you've got some kind of foam on all sides and secure them well :slight_smile:
```

---
## \#9 Posted by: b264 Posted at: 2019-01-08T08:20:18.714Z Reads: 132

```
A conductive aluminum enclosure doesn't sound like any obstacle some truck bedliner can't fix.  But the remote signal will be blocked by it, so make sure your design takes that into consideration.  If you have a wooden deck, the airwaves will go straight through that anyway.
```

---
## \#10 Posted by: banjaxxed Posted at: 2019-01-08T09:10:03.165Z Reads: 119

```
Have a look at the hard case lipos if you don’t need every mm
```

---
## \#11 Posted by: monsterbuilder Posted at: 2019-01-08T13:36:06.743Z Reads: 101

```
Sorry dude for not thinking things through all the way before blurting out an answer.  Sounds like it's perfectly safe as long as your components are shielded and mounted secure.  Take some pics of your enclosure when you are done.  Should be a really robust solution for protecting the goods.
```

---
## \#12 Posted by: Slydunan Posted at: 2019-01-08T15:13:27.219Z Reads: 91

```
Awesome I would love to see some pictures if you have any!
```

---
## \#13 Posted by: Gamer43 Posted at: 2019-01-08T20:52:09.256Z Reads: 79

```
This is what it looks like with the battery inside. ![20190101_195556|375x500](upload://cuQNcNHmTsCODpDGYCwX7btglhG.jpeg) 
![20180813_183836|375x500](upload://1YV36qfz7Mcau12Kky6YLJf4mNg.jpeg) . This was before I switched to 2" angle, but you get the idea. Sorry I don't have better pictures.
```

---
## \#14 Posted by: Slydunan Posted at: 2019-01-08T21:14:40.597Z Reads: 73

```
Cool thanks! I checked out some sheets today, 0.032" was a lot more heavy duty than I expected. I may go for some thinner sheets that can be bent more easily so I wont have to use multiple pieces.
```

---
## \#15 Posted by: Gamer43 Posted at: 2019-01-08T21:24:40.918Z Reads: 66

```
Oh wow. 0.032" was actually the thinnest sheet metal I could buy cheaply from Industrial Metal Supply. 

What alloy was it? I purchased 5052 galvanized aluminum sheet. 

Good luck on fabricating your enclosure! I don't think you'll run into problems, but it was a pain for me to work with sheet metal, mostly because I didn't have the right tools xD.
```

---
## \#16 Posted by: Slydunan Posted at: 2019-01-08T21:40:09.778Z Reads: 61

```
I think it was 2xxx something, it was just the local ace. They had a few 22-28 gauge ones, which are thinner. I could see 0.032 being very hard to bend. 

I'll have to drive out to a metal sheet supplier and look over some more options, I'll see how it goes!
```

---
## \#17 Posted by: Gamer43 Posted at: 2019-01-08T22:18:40.754Z Reads: 57

```
Oh I see.
Actually, I was wrong, the sheet metal I got was 28 or 32 gauge, not 0.032" lmao. That's my bad.

Good luck!
```

---
## \#18 Posted by: pat.speed Posted at: 2019-01-09T23:03:53.096Z Reads: 39

```
I would recommend a minimum of 0.5mm, that’s the thickest sheet I could get at my hardware store and it’s a little more bendy than I would like however it does work just fine. 

If you buy a full sheet it is very easy to bend it into a case by using the corner of a bench and a long solid wood plank. You put the aluminium on the corner of the bench where you want to bend it the place the wood on top and clamp it down tight, the bend the sheet and move into the next bend, very easy and looks good too. My mate saw mine and thought I must have used a sheet bender
```

---

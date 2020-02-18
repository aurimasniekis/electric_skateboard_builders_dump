# BMS Hunting No More

### Replies: 64 Views: 2029

## \#1 Posted by: scepterr Posted at: 2018-03-14T00:34:26.207Z Reads: 358

```
**Hold onto your brain buckets folks.**
So here's the thing, if you have a dumb BMS(no IC,nothing fancy) like the D122, D140, D190 etc, you can use for instance a 12S BMS on lower S counts. 🤯
They work on a per series basis, the actual total voltage is irrelevant for it to function. So if you take a 12S BMS and wire an 11S battery and charge to 11S voltage. **IT WORKS**

I've tested this on the 12S D122 on my 11S
I'll be testing the 12S D140 tomorrow on a 10S battery

![IMG_20180313_141127|666x500](upload://1mJsL9ydatNBZnH5rZbsGqWHA82.jpg)
![IMG_20180313_202015__01|690x377](upload://6e78DgWjkRCtQ3wxztSRwWXmlCO.jpg)

I wanna buy up as many BMS as I can find to test this functionality on, if you wanna contribute to the effort, my PayPal cyberonu@gmail.com
```

---
## \#2 Posted by: barajabali Posted at: 2018-03-14T00:37:27.522Z Reads: 335

```
Works for supower bms too
```

---
## \#3 Posted by: scepterr Posted at: 2018-03-14T00:39:23.928Z Reads: 335

```
Technically this should work on any that are just discrete component based logic
```

---
## \#4 Posted by: isqueromeroderviz Posted at: 2018-03-14T02:06:43.768Z Reads: 328

```
I already wanted to know about this from the 12s bms to 11s
```

---
## \#5 Posted by: Deckoz Posted at: 2018-03-14T02:07:20.652Z Reads: 323

```
Yep...I've done this a few times before... Even wired dumb 3s & 4s BMS together to make a 12s :P just share some balance leads that need to be shared between the bms and you can. Have a multi part pack... That takes up far less BMS space..
```

---
## \#6 Posted by: scepterr Posted at: 2018-03-14T02:09:10.627Z Reads: 308

```
I've always assumed this was possible just didn't wanna say anything till I did it  and everything was fine. 😋
```

---
## \#7 Posted by: ZackoryCramer Posted at: 2018-03-14T06:42:35.802Z Reads: 281

```
But how exactly does it work? Wouldn’t this mean the bms would output even if one of the cells disconnected resulting in a “type 2” error? 🤔
```

---
## \#8 Posted by: scepterr Posted at: 2018-03-14T06:47:27.190Z Reads: 268

```
I have no idea what you just said lol
```

---
## \#9 Posted by: Deckoz Posted at: 2018-03-14T06:49:22.498Z Reads: 263

```
[quote="ZackoryCramer, post:7, topic:49040"]
But how exactly does it work? Wouldn’t this mean the bms would output even if one of the cells disconnected resulting in a “type 2” error? :thinking:
[/quote]

Forget all you just wrote... Two words


Charge only.

Also @scepterr 11s5p? :D
```

---
## \#10 Posted by: scepterr Posted at: 2018-03-14T06:52:59.541Z Reads: 248

```
Lol yeah 12S fit but with no room for all the extra bits I wanted, 12/5V stepdown, Arduino. 10S left too much room, 11 was the magic number 😋
```

---
## \#11 Posted by: Deckoz Posted at: 2018-03-14T06:54:01.050Z Reads: 239

```
Still... You have 14 more cells then it was designed for. Gonna be awesome.


Where's the build thread?
```

---
## \#12 Posted by: scepterr Posted at: 2018-03-14T06:54:47.024Z Reads: 228

```
Once it's rolling I'll put a build thread up
Got 4 build threads incoming, easier to post when done 😃
```

---
## \#13 Posted by: pat.speed Posted at: 2018-03-14T06:55:29.305Z Reads: 228

```
@Deckoz do you think you could give a little more of an explanation to how you wired multiple small bms together? Pm maybe as not to go off topic
```

---
## \#14 Posted by: Hummie Posted at: 2018-03-14T06:55:29.464Z Reads: 229

```
sounds like a squeeze job.  want to see.
```

---
## \#15 Posted by: scepterr Posted at: 2018-03-14T06:56:37.945Z Reads: 224

```
![IMG_20180314_011637__01|690x307](upload://srRcTKUwknrXQn6mYOPP7XBuwJU.jpg)

@Hummie I'll be mocking up the battery for your deck tomorrow, let's see what happens 😋
The 11S5P is 18.5"x6.5"
```

---
## \#16 Posted by: ZackoryCramer Posted at: 2018-03-14T06:57:58.491Z Reads: 219

```
I meant to ask technically why it works. Shouldn’t the bms block all current flow if one of the cells is faulty/disconnected?
```

---
## \#17 Posted by: scepterr Posted at: 2018-03-14T06:58:18.758Z Reads: 216

```
If it's in the middle yes, if it's at the end no
```

---
## \#18 Posted by: Deckoz Posted at: 2018-03-14T07:09:25.811Z Reads: 212

```
Well every balance lead except B- and B+ is really a ± 

Let's take 3s bms's.  Cell 3 balance lead needs to share b- balance lead of the next group. Which technically happens because of the series connection. B- of each group must be connected.  Ie cells 1-3 group cell 1 connected to b- of BMS 1. Cell 4-6 cell 4 connected to b- of bms2. Etc. B- is the ground and no balance functions will work without it connected on most dumb BMS

To charge -ch on BMS one to charger negative. Charger positive to end of pack b+(not group b+)
```

---
## \#19 Posted by: b264 Posted at: 2018-03-14T08:04:03.569Z Reads: 203

```
@scepterr do you have a schematic for exactly how you've hooked up the 11SxP to the 12S BMS?
```

---
## \#20 Posted by: scepterr Posted at: 2018-03-14T08:08:49.875Z Reads: 212

```
11 wires instead of 12, last one skipped
There's really nothing to it other than pretending it's for whatever S count you have 😉
![IMG_20180314_004213|375x500](upload://3FXCa5U59vXLd8cFkgrb34pyH90.jpg)
```

---
## \#21 Posted by: pat.speed Posted at: 2018-03-14T09:02:15.255Z Reads: 192

```
Uuuuhhhh, I kinda of understand but not quite. Sorry for lots of questions but would you have access to a diagram. I can’t find anything on google about bms modules in series
```

---
## \#22 Posted by: scepterr Posted at: 2018-03-14T09:03:57.796Z Reads: 189

```
It's the same principal as taking 2 5S batteries and combining into 10S

BMS 1
B-, b1+,b2+,b3+,b4+,b5+

BMS 2
b5+ from BMS 1 goes to B- of BMS 2
Then continue, b6+,b7+,b8+,b9+,b10+

Use Charge negative from BMS 2
```

---
## \#23 Posted by: pat.speed Posted at: 2018-03-14T09:18:22.577Z Reads: 183

```
This is going to sound stupid but how are the cells connected to bms 1 charged?
```

---
## \#24 Posted by: scepterr Posted at: 2018-03-14T09:19:04.213Z Reads: 184

```
Because b5+ from BMS 1 is connected to B- of BMS 2, that's the link
You can either run 2 leads from b5+, one to b5+ of BMS 1 and one to B- of BMS 2 or run a lead from b5+ on BMS 1 itself  to BMS 2 B-
```

---
## \#25 Posted by: pat.speed Posted at: 2018-03-14T09:24:43.094Z Reads: 179

```
I understand how they get connected, but what I can’t get my head around is how the charge runs from bms 2 back to 1.


Actually wait I might get this shit. When I get home in 5 I’ll draw a diagram of how I understand it and post it here, could you just tell me if it’s correct?
```

---
## \#26 Posted by: pat.speed Posted at: 2018-03-14T09:36:24.315Z Reads: 178

```
![image|374x499](upload://6ItCkLGS1ei4rjRvGJqnEsyB3AM.jpeg)


I think this is correct
```

---
## \#27 Posted by: scepterr Posted at: 2018-03-14T09:37:39.901Z Reads: 164

```
Almost, that's supposed to be charge negative coming from c- on BMS 2

Charge postive is battery positive, doesn't touch the BMS
C+/B+
```

---
## \#28 Posted by: pat.speed Posted at: 2018-03-14T09:40:01.290Z Reads: 163

```
Lol, yeah I even wrote c- then drew it red
```

---
## \#29 Posted by: pat.speed Posted at: 2018-03-14T10:04:24.266Z Reads: 167

```
Ok so now I’m even more confused. I know that that’s how it must work but I can’t get my head around how those cells circled in red get a positive charge. I understand how the blue cells get charged but not the red. And thank you so much for helping me this far



![image|375x500](upload://bYmcGBWhFi7qNmAAJVHgNa40cWY.jpeg)
```

---
## \#30 Posted by: scepterr Posted at: 2018-03-14T10:07:29.589Z Reads: 151

```
Because your charger is connected to the positive of the **whole** battery and the charge negative of BMS 2 is the total battery negative
```

---
## \#31 Posted by: pat.speed Posted at: 2018-03-14T10:09:02.321Z Reads: 147

```
Wait a moment am I getting confused because I have bms 1 and 2 around the wrong way?
```

---
## \#32 Posted by: scepterr Posted at: 2018-03-14T10:09:20.790Z Reads: 143

```
Probably hahaha
```

---
## \#33 Posted by: pat.speed Posted at: 2018-03-14T10:12:24.514Z Reads: 137

```
Lord Jesus Christ please help me to not be so stupid next time lol. I know exactly why now. I have the two bms modules the wrong way. Which means that it is only charging the first 5 cells and not the others. So if I was to connect the other bms to the charge port that would send voltage through all 10 cells?
```

---
## \#34 Posted by: scepterr Posted at: 2018-03-14T10:13:11.278Z Reads: 138

```
You have it connected correctly just drawn in reverse, regardless, yes
You connect charger negative to the 2nd BMS in the series
```

---
## \#35 Posted by: pat.speed Posted at: 2018-03-14T10:18:22.562Z Reads: 153

```
Ok thanks for all this help, hopefully this helps somebody else to connect their cells with a bms in series. The worst part about all of this is it makes doing it your way with just one less balance lead so much more tempting, haha. 

Here is the final and wrong diagram...lol
![image|375x500](upload://9IZ5RQjmm7JhWbpOsAWbdT8rky6.jpeg)
```

---
## \#36 Posted by: scepterr Posted at: 2018-03-14T10:19:24.873Z Reads: 142

```
WRONG...lol
You do NOT connect charge to BMS 1
```

---
## \#37 Posted by: pat.speed Posted at: 2018-03-14T10:21:40.576Z Reads: 144

```
What the fuggin hell. So was it right before I moved the c- to bms 1? If so I just don’t understand how the positive charge flows into the 4 cells on the right hand side
```

---
## \#38 Posted by: scepterr Posted at: 2018-03-14T10:24:34.517Z Reads: 148

```
![IMG_20180314_062357__01|690x386](upload://e6xVp6ngAqyRlzWUakGP4N0Ypht.jpg)
```

---
## \#39 Posted by: pat.speed Posted at: 2018-03-14T10:30:32.219Z Reads: 146

```
Ok, I kinda get it. So somehow the negative charge from the charger passes through c- on bms 2, then out b- and into b5 on bms 1, and then out of b- on bms 1 and into the battery. I think I might just be over complicating it by trying to picture the flow of electrons
```

---
## \#40 Posted by: scepterr Posted at: 2018-03-14T10:31:18.127Z Reads: 143

```
Dude forget c- on BMS 1, I freaking crossed it out, it doesn't exist
```

---
## \#41 Posted by: pat.speed Posted at: 2018-03-14T10:33:49.292Z Reads: 130

```
Sorry my bad I wrote the bms numbers the wrong way, does it seem right now?
```

---
## \#42 Posted by: scepterr Posted at: 2018-03-14T10:35:20.262Z Reads: 127

```
Lol yes correct numbers help 🤣
Yes everything is in a chain and will function as a whole
```

---
## \#43 Posted by: pat.speed Posted at: 2018-03-14T10:37:08.987Z Reads: 132

```
Ok thank you, jeez I over complicate the crap out of stuff sometimes, you should see me in maths class. My teachers get mad cos I question the workings of every single thing. So this proves you have good patience and I’m grateful for that
```

---
## \#44 Posted by: Scoo_B_SK8 Posted at: 2018-03-14T10:56:41.297Z Reads: 122

```
Awesome napkin diagram :stuck_out_tongue_winking_eye:
```

---
## \#45 Posted by: scepterr Posted at: 2018-03-14T10:58:02.724Z Reads: 126

```
Napkin? What napkin? That's genius paper.
```

---
## \#46 Posted by: Scoo_B_SK8 Posted at: 2018-03-14T11:02:12.365Z Reads: 124

```
LOL... If that's the case should turn the resolution down on camera.

looking forward to your multiple build threads.
```

---
## \#47 Posted by: scepterr Posted at: 2018-03-14T11:07:39.254Z Reads: 120

```
I have a truly first world problem, trying to come up with names for all of them 🤣
```

---
## \#48 Posted by: Scoo_B_SK8 Posted at: 2018-03-14T11:19:51.721Z Reads: 126

```
Once completed and go for a little test spin,  it'll come to you.

on that note tho there aren't a lot of elegant type names out there for boards...
Example
"ZOO Lyn" carver     (combination of Zoo York & Brooklyn) i would expect clean smooth flowing lines maybe even with some lighter/softer shades of running lights, like an angel floating down the street.
or
could be a take from Wu-Tang, shaolin ninja style C.R.E.A.M.

EDIT; the board with the search light on it would represent "follow the light  or Run away from the light" as often described with out of body experiences.
```

---
## \#49 Posted by: Deckoz Posted at: 2018-03-14T13:43:28.043Z Reads: 114

```
I'm confused too because I connected charge negative to BMS 1 in the past...not the last BMS in line...... @scepterr @pat.speed
```

---
## \#50 Posted by: deucesdown Posted at: 2018-03-14T15:59:50.824Z Reads: 113

```
[quote="scepterr, post:12, topic:49040"]
Got 4 build threads
[/quote]

Hm this is to go with the handful of nano-x remotes? One per day of week, charge on weekends?
```

---
## \#51 Posted by: scepterr Posted at: 2018-03-14T18:15:54.418Z Reads: 109

```
I just tried with two 10s BMS wired 5s to each and linked them, and charge negative to BMS 2, charged up fine
```

---
## \#52 Posted by: Deckoz Posted at: 2018-03-14T18:22:08.470Z Reads: 111

```
Then likely either -c will work as the only purpose is to cut off the charge at the end. -c is normally a shared pad of -b with a ic switch to break the shared ground. 

I was under the assumption if you have the charger positive on cell 10 and the -c effectively on 6 negative(2nd -b shared with -c) the charge current would be passing down to the common ground and current only going to half the pack, and the BMS balancing the current to the lower cells.

With -c on the first BMS...the common ground is cell 1 negative. So current goes through the entire pack vs only half way...and no voltage mismatch..

Can you do me a favor and multimeter from your BMS 2 -c and the total pack b+. I would expect to only see 21v~  @scepterr
```

---
## \#53 Posted by: scepterr Posted at: 2018-03-14T18:25:54.622Z Reads: 112

```
Yeah I'll check, gotta put it back together
```

---
## \#54 Posted by: pat.speed Posted at: 2018-03-14T19:37:16.689Z Reads: 109

```
This is exactly what I was thinking, maybe I’m not as stupid as I thought
```

---
## \#55 Posted by: DeathByBacon Posted at: 2018-07-05T19:46:50.441Z Reads: 90

```
if you're using 2 x 6s BMS for a 12s pack, do you still use a 12s charger or does it have to be a 6s charger now?
```

---
## \#56 Posted by: pat.speed Posted at: 2018-07-05T22:26:45.443Z Reads: 85

```
A 12s charger
```

---
## \#57 Posted by: DeathByBacon Posted at: 2018-07-06T07:36:05.801Z Reads: 78

```
Would it also be possible to use 2 x 10s bms for a 12s pack?
```

---
## \#58 Posted by: pat.speed Posted at: 2018-07-06T10:21:39.224Z Reads: 78

```
I suppose so, but it would waste a lot of space
```

---
## \#59 Posted by: DeathByBacon Posted at: 2018-07-06T11:13:10.974Z Reads: 80

```
Yeah but it's been so difficult  to find a cheap 12s bms for charging only
```

---
## \#60 Posted by: pat.speed Posted at: 2018-07-06T12:13:39.996Z Reads: 79

```
Get a 13s one and leave off the last wire, cost me $17 bucks on eBay
```

---
## \#61 Posted by: faithfulpuppy Posted at: 2018-07-06T14:03:56.450Z Reads: 74

```
[quote="DeathByBacon, post:55, topic:49040, full:true"]
if you’re using 2 x 6s BMS for a 12s pack, do you still use a 12s charger or does it have to be a 6s charger now?
[/quote]
you could technically put 2 6s chargers in series but it's easier to just use 12s
```

---
## \#62 Posted by: DeathByBacon Posted at: 2018-07-06T16:36:28.980Z Reads: 69

```
You have a link for that?
```

---
## \#63 Posted by: willpark16 Posted at: 2018-07-06T20:30:29.509Z Reads: 66

```
Do you charge with a 12s or 13s charger?
```

---
## \#64 Posted by: pat.speed Posted at: 2018-07-06T20:45:23.873Z Reads: 63

```
With a 12s one. 

Here’s the link 



https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com.au%2Fulk%2Fitm%2F132601114266
```

---

# Two wheel drive with one motor?

### Replies: 16 Views: 6740

## \#1 Posted by: siggs3000 Posted at: 2015-08-19T20:15:42.009Z Reads: 227

```
I'm about to start building my first board and like everyone at first, am torn about one motor vs two. I'm 140 lbs and live in San Diego with some hills that are mostly pretty mellowish compared to SF but indeed present.  

My goal is to have a light weight board with good range that can get up the hills and down with controlled braking. 

I like the idea of two wheel drive for symmetry in braking and acceleration but would rather stick to one motor for weight, range and cost. (Ideally) 

I'm also planning to add some "smart" features with a raspberry pi after the initial build. More on that later...

For now I'm wondering if anyone has ever put together a gear arrangement to drive both back wheels with a single motor. I think it would be tricky to mount such a thing on the truck but could it be possible?
```

---
## \#2 Posted by: sl33py Posted at: 2015-08-19T20:51:47.108Z Reads: 221

```
If you have access to a CNC and skill to use it, it's doable.  But weight and complexity start to quickly be an issue.  I saw someone on ES who build a differential to drive both wheels...  

I like the simplicity of a single motor setup.  I am nearly two of you and a single 63mm motor w/ a good ESC and higher # series battery moves me along just fine!  At 140 you can use a much smaller motor and less voltage.

Personally i'd keep it simple and save $ w/ a nice motor + ESC.  My GF's board w/ dual 8Ah batteries (8s), VESC, 6354 200kv motor, and Enertion motor bracket is ~15-16lbs w/ a loaded vanguard 41 flex 1 deck.  Some selective weight cutting (smaller batteries especially) and you can get a nice light setup that will push you up any of your local hills!
```

---
## \#3 Posted by: sl33py Posted at: 2015-08-19T20:55:01.295Z Reads: 213

```
light weight is relative.  Do you have a target weight or range?  I personally look at the boosted dual+ as my benchmark (15lbs) and anything lighter than that is "light".  Great board too, minus the range limitation.

Look at the VESC if you can swing it as the best ESC i've tried on a board minus the Boosted (which is sensored and "butter" smooth!).

What are you going to do with RPi?
```

---
## \#4 Posted by: siggs3000 Posted at: 2015-08-19T22:15:25.984Z Reads: 214

```
Thanks for the replies @sl33py. I would be really happy with 15 lbs and it sounds like your gf's setup is pretty close to what I was thinking of too. I was planning  to get the VESC and the Enertion motor bracket. I'm still completely torn about what motor to get though. I already ordered a pair of 8s packs and already have a board with Caliber trucks, ready to go. (31" so it'll be pretty compact) Sounds like a single wheel drive isn't too much of an issue, especially with the VESC. 

I'm not totally sure what I'm going to do with the RPi just yet but I plan to build a companion app (I make apps for a living) and wanted to interface with the board to have some kind of dashboard for battery level, maybe rpm's etc, in addition to speed from gps, etc (from the phone). I figured it might be cool to do some kind of remote kill function (in the event of theft), or even some kind of "find me" so the board can drive itself over to you  or it's charging dock (would need to have some kind of small accessory steerable wheel to extend downward, lifting the front end off the trucks, for self driving)

Possibly even obstacle avoidance, one day

I'm open to other ideas surrounding this too! (Or tips for the actual build, of course!)
```

---
## \#5 Posted by: lowGuido Posted at: 2015-08-19T22:15:49.199Z Reads: 206

```
the only way you are going to get 2 wheel drive with one motor is with something like this:
<img src='/uploads/db1493/original/1X/39dd5e66786d618995215dffa167bd1cf5e8d5c8.jpg'>

(not my image)
although looks like it would be heavier than 2 motors.. certainly alot harder to do.
```

---
## \#6 Posted by: onloop Posted at: 2015-08-19T23:14:02.651Z Reads: 204

```
If you are going to get just one motor make it a big one. 6374 SK3 would be my advice.

Driving two wheels with one motor is not a proven option with eboards.

Actually at your weight 6355 will also be fine.

This one ;)
http://www.enertionboards.com/electric-skateboard-parts/190kv-electric-skateboard-motor/
```

---
## \#7 Posted by: siggs3000 Posted at: 2015-08-19T23:20:26.091Z Reads: 199

```
I'm ordering from you guys right now, @onloop

VESC, motor mount and a motor. This should be fun!

Last question for at least the next 20 minutes: I notice everyone using huge wheels (80mm+) - I would prefer to be a little closer to the ground with familiar 72-ish mm wheels. Any big reason to not use wheels that small?
```

---
## \#8 Posted by: lowGuido Posted at: 2015-08-19T23:31:22.387Z Reads: 188

```
all my boards have 70mm wheels. I was the same I didnt want to ride a monster truck.
I found 70mm was the smallest I could go and still have a drive gear fit on.

I think the bigger wheels is mainly because of drive gear size and also being able to roll over small obstacles easier.
```

---
## \#9 Posted by: onloop Posted at: 2015-08-19T23:42:04.776Z Reads: 185

```
LowGuido got it!

It's mostly due to the size of the wheel pulley & ground clearance. The belt gets very close to rocks if the wheel diameter is too small. Also you need to be able to fit the motor and electronics under a deck. If your motor D is 63mm. And your wheel D is only 70mm it allows just 7mm clearance for motor. So then you need huge truck risers. So just go bigger wheels.
```

---
## \#10 Posted by: siggs3000 Posted at: 2015-08-19T23:45:33.574Z Reads: 174

```
Makes sense. Thanks guys!
```

---
## \#11 Posted by: sl33py Posted at: 2015-08-20T00:28:31.285Z Reads: 172

```
The guys got you squared away on components.

as for RPi - check out the VESC options as you can likely build something that talks with your phone over BTLE.  Quite a bit of development going on for it and might be worth joining vs building something on Pi to do something it does most of already!  (Watch vedder's nightime video w/ logging - tons of data out of VESC).
```

---
## \#12 Posted by: siggs3000 Posted at: 2015-08-20T00:56:01.107Z Reads: 170

```
@sl33py - I'm checking out those videos now. You're right. This thing does way more than I thought! 

I do have another question for you guys: 

Batteries. I think I've settled on an 8s goal. Should I do two 8s packs in parallel? Or two 4s packs in series? The nice thing about the 4s packs is that they are thinner and offer more ground clearance. (plus getting a charger seems to be way easier for smaller voltages)
```

---
## \#13 Posted by: lowGuido Posted at: 2015-08-20T01:03:10.730Z Reads: 167

```
if hills is your goal id go with 2 8S in parallel. or if you are that worried about the thickness why not two 4S in series with two 4S in parallel.

or insert @onloop suggesting you buy a space cell...
```

---
## \#14 Posted by: cmatson Posted at: 2015-08-20T02:20:53.565Z Reads: 170

```
personally, I would do two 4s in series and here's why:
it keeps your build thinner (like you said)
4s packs are easier to charge than 8s, because a lot of chargers top out at 6s (like you said, again)
4s pack are easier to find and cheaper than 8s packs, so if one fails at some point, its way cheaper to replace. 

essentially if you went with two 8s packs, your overall cost on batteries would be higher, due to the price of 8s packs, and you'd need a more expensive charger to charge over 6 cells.

As long as the mah of the combined packs is the same for both the 4s and 8s setups, they will preform roughly the same on hills: its just the layout which will differ.

that being said, here's my two cents:
skip lipos altogether, forget charging two packs or worrying about thickness... just buy a space cell. 
its 10s3p 18650 cells, so it is higher voltage than you want, but it beats lipos in every catagory:
simple charging with a laptop style charger
display with % battery indicator 
built in on off switch
as thin as a 3s lipo

It would probably be around the same cost as the two 8s batteries + charger, and slightly more than the two 4s + charger, but its worth it.

again, just my suggestion- but as for your two options 4s > 8s
```

---
## \#15 Posted by: treenutter Posted at: 2015-09-04T13:28:20.365Z Reads: 157

```
@siggs3000 I'm building a similar setup now, and I'm at about the same phase of the build (lots of reading, everything ordered)... I opted for 2 4s compact lipos to run in series for 8s (25/35C). This will provide 5000mAh. This is to power an SK3 6364 (245Kv) as a single motor. I have a VESC on the way, and I'll run it with 5 inch pneumatic wheels geared at 14T\40T. I'm also a small rider at 145 lbs, so I'm hoping this setup will provide enough power to move me around easily.

I agree w @cmatson about using 2 4s packs; they will be easier to charge and thinner than a single 8S pack. The SpaceCell looks excellent, and I think that's the choice I will make once I have a little more experience with eboards and I understand my needs a little better. 

For now, I've got a box of parts growing in the corner as I track shipments online with unnecessary ferocity!
```

---
## \#16 Posted by: Mikeomania12 Posted at: 2016-08-01T20:12:46.818Z Reads: 104

```
Check this made by CARVON. Interesting design but not practical.
http://www.electric-skateboard.builders/t/has-it-finally-been-figured-out-1-motor-2wd/4567
```

---

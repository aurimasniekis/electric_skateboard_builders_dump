# Onboard Gps locator (Thief catcher)

### Replies: 29 Views: 1073

## \#1 Posted by: amazingdave Posted at: 2018-10-15T18:20:35.771Z Reads: 246

```
Following on from this thread....

https://www.electric-skateboard.builders/t/stolen-evolve-carbon-all-terrain/33979

What would the simplest way to power a gsm gps inside the board? I have one of these..

https://www.ebay.co.uk/itm/Genuine-GPS-Tracker-Magnetic-Car-Vehicle-Spy-Mini-Personal-Tracking-Device-TK102/151857299746?epid=24008060886&hash=item235b668122:g:SZsAAOSwXNNbaCiM

It uses a single cell Lipo like an old school cell phone... Is it possible to pull 5v off the vesc 6.6 (Flipsky dual) to charge it via usb? Or 4v ish to power it directly? My first thought was using the receiver power and charge it so it still transmits when the board is powered off....
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-15T18:28:44.429Z Reads: 237

```
the biggest issue I have run into when looking at GPS tracking as an option is cost and placement.  I just don't wanna spend 30 bucks a month for it, its too much for a passive use item.  If you put it in the enclosure, the only way you get sat acquisition is if the board is upside down.
```

---
## \#3 Posted by: danielz Posted at: 2018-10-15T18:31:23.375Z Reads: 230

```
I have live tracking on my drone, using the tk102 mentioned above. In one year is cost me like £1 with a giffgaff UK sim. I created a youtube tutorial showing how to get it working. It would slide right into my esk8 enclosure, set and forget.

https://youtu.be/7PskGCE_sUc
```

---
## \#4 Posted by: Skunk Posted at: 2018-10-15T18:33:21.172Z Reads: 223

```
So... what no link?
```

---
## \#5 Posted by: mmaner Posted at: 2018-10-15T18:34:35.898Z Reads: 227

```
[quote="danielz, post:3, topic:71319"]
£1 with a giffgaff UK sim
[/quote]

I don't think we have anything similar in the US.  The cheapest I've ever found is $30 a month.
```

---
## \#6 Posted by: danielz Posted at: 2018-10-15T18:35:08.953Z Reads: 226

```
Yes usa hasnt a 2g network i here. Here I can use any non contract sim supporting 2g, Just top it up once, it uses so little data, lasts forever.
```

---
## \#7 Posted by: mmaner Posted at: 2018-10-15T18:43:42.940Z Reads: 242

```
if you have 2G/GSM service available this is a pretty good option...

https://www.ebay.com/itm/Real-Time-GPS-Tracker-GSM-GPRS-Tracking-Device-for-Car-Vehicle-Motorcycle-Bike/153130251877?hash=item23a7463665:g:cT0AAOSw2kNbab9v:rk:18:pf:0
```

---
## \#8 Posted by: JLabs Posted at: 2018-10-15T18:55:37.725Z Reads: 230

```
I have one of these in my AT Evo. 

I used a step down converter and took power from my bypassed BMS. I used a text only plan from US Mobile ($4 a month) but I let it run out, and if I ever need to use it I can just pay the 4 bucks and start tracking it again. Works very well in my rural environment.

I ended up putting a switch on the power line tho as it will drain the battery in 1-2 weeks and it dosnt need to be on 24/7

I got this sim starter kit: 
https://www.usmobile.com/shop/product/Starter-Kit

It looks like they lowered their price for texting only to $1.50 a month plus a couple dollars in fees.

I also took it out of the plastic case and wrapped it in shrink wrap. It is installed right under my BMS and together they are the height of an 18650 so it worked out perfect. If i get the unity beta 2 to test I will take some pics for you guys (and maybe post a build thread, wait who has time for that lol).
```

---
## \#9 Posted by: mmaner Posted at: 2018-10-15T18:56:29.228Z Reads: 212

```
Well, that's good stuff to know.  I will have a look as well.  Thank @JLabs.
```

---
## \#10 Posted by: wolffoxx Posted at: 2018-10-15T20:09:48.966Z Reads: 198

```
Have you looked at Tile?  It's not active tracking like GPS, but it's a low one time cost and a crowdsourced locator.  I have one built into my keyring thing, but I've thought about putting one in my board, just to have a chance at a recovery. 

Here's a story about a stolen bike:

https://www.thetileapp.com/en-us/blog/stolen-bike-recovered-tile-gps
```

---
## \#11 Posted by: mmaner Posted at: 2018-10-15T21:25:22.399Z Reads: 168

```
its decent in large population areas, in rural areas its essentially useless unless the guy that steals your board has the app :slight_smile:
```

---
## \#12 Posted by: wolffoxx Posted at: 2018-10-15T21:31:17.273Z Reads: 164

```
[quote="mmaner, post:11, topic:71319"]
unless the guy that steals your board has the app
[/quote]

:rofl: That would be the best...
```

---
## \#13 Posted by: danielz Posted at: 2018-10-16T02:38:41.848Z Reads: 147

```
Oh I forgot to mention the tk102 can work via the sms text service too. If you text it asking for its location, it will message you back its coordinates. Im not sure what protocol sms uses in the states though.
```

---
## \#14 Posted by: mmaner Posted at: 2018-10-16T03:43:37.625Z Reads: 144

```
I've got one ordered and a US Mobile SIM, gonna give it a try.
```

---
## \#15 Posted by: Eboostin Posted at: 2018-10-16T04:56:32.357Z Reads: 129

```
Interested to see what options arise. If we could also add text to self destruct, that could be fun too
```

---
## \#16 Posted by: b264 Posted at: 2018-10-16T05:06:02.822Z Reads: 126

```
Any option that involves grenades or stun guns hidden in seats has my vote.

I'm not too fond of thieves and I don't care about their wellbeing.  *At all.*  Being a thief is a choice.
```

---
## \#17 Posted by: totalgeek9224 Posted at: 2018-10-16T12:28:42.180Z Reads: 113

```
https://www.ebay.com/itm/GT06-GPS-GSM-GPRS-Car-Tracker-Locator-Anti-theft-SMS-Dial-Remote-Control-Alarm/401309057134?epid=767434076&hash=item5d6fe2406e:g:BmUAAOSwqVxZiTC~:rk:35:pf:0

This could be interesting as it allows for shutoff features, could be modified to turn off power to ESC's or something like that
```

---
## \#18 Posted by: mmaner Posted at: 2018-10-16T13:45:46.055Z Reads: 104

```
I was looking at that as well, it has a SOS cable interface...

![image|465x500](upload://6ANKtUbmKQAt0c3VenUA9eGoDHh.jpeg) 

I assume we could use that as the NO/C connection on an Anti-Spark switch to turn off the board, but I'm not sure you could use it in-line with the existing switch.  

I'm really interested in making these work, I've never had anyone try to take a board from me, would likely be fatal for the other person involved :dagger:. For now I'm just going to work on making the GPS logging and notification work.  After that maybe the cutoff features.
```

---
## \#19 Posted by: Battosaii Posted at: 2018-10-16T13:48:43.785Z Reads: 102

```
I'm not worried about my board being taken away from me when I'm present but when my board is in my car or when I'm not paying attention.
```

---
## \#20 Posted by: mmaner Posted at: 2018-10-16T13:49:46.921Z Reads: 100

```
That too, I'm mostly worried about shipping them.  When I shipped them to Miami this summer I was a nervous wreck for a week :slight_smile:.
```

---
## \#21 Posted by: amazingdave Posted at: 2018-10-16T14:25:37.384Z Reads: 90

```
Here’s one that could be cut down, 5v supply small form factor....

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F253227084373
```

---
## \#22 Posted by: mmaner Posted at: 2018-10-16T14:42:53.913Z Reads: 85

```
I wonder how well its gets sat acquisition...
```

---
## \#23 Posted by: amazingdave Posted at: 2018-10-16T14:59:33.706Z Reads: 77

```
Bought one in the name of science... I’ll let you know.
```

---
## \#24 Posted by: JLabs Posted at: 2018-10-16T15:02:30.595Z Reads: 75

```
Most one the cheap trackers don’t use gps at all. They triangulate the position from nearby cell towers. 

The one I got didn’t even have the gps chip in it (and I’m sure all the other cheap ones don’t either).
```

---
## \#25 Posted by: mmaner Posted at: 2018-10-16T15:03:16.740Z Reads: 74

```
Wow, so much I don't know about these :).  That kind of sucks, I mean GPS isn't all that accurate but it likely more accurate than signal triangulation.
```

---
## \#26 Posted by: amazingdave Posted at: 2018-10-16T15:03:38.547Z Reads: 77

```
The first link I posted at the top is for a tracker I have that works perfectly... cheap nasty functional Gps accurate.
```

---
## \#27 Posted by: JLabs Posted at: 2018-10-16T15:08:12.059Z Reads: 76

```
Mine is dead accurate, like scary accurate..
```

---
## \#28 Posted by: mmaner Posted at: 2018-10-16T15:09:15.179Z Reads: 72

```
Cool, Im gonna try and lay this out in visio with a tutorial for everyone so I may be PM'ing you for info and you too @amazingdave
```

---
## \#29 Posted by: totalgeek9224 Posted at: 2018-10-16T15:14:41.858Z Reads: 72

```
Or with something like the Unity, which has a smart switch build in, run that inline to NO/ O so that when you plug in Xt90 key, all turns on, but you could disable via gps text.. Might be an interesting feature we could try...in the name of science. 
Plus, im sure there are other ways we could integrate it, its size is just slightly large but but seems to be thin.. Could be interesting.

I hope no one had their board taken from them, but is always nice to be safe instead of sorry, plus a cool little party trick and a way to assure S/O that your investment is safe :p ;)
```

---

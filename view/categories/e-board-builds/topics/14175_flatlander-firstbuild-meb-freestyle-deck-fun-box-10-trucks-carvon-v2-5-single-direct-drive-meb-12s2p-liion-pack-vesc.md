# Flatlander Firstbuild &#124; MEB Freestyle Deck &#124; Fun Box 10&rdquo; trucks &#124; Carvon V2.5 Single &#124; Direct Drive &#124; MEB 12S2P LiIon Pack &#124; VESC

### Replies: 8 Views: 1673

## \#1 Posted by: wookiepedia Posted at: 2016-12-04T20:12:42.559Z Reads: 188

```
Hello, everyone!  I am starting the research and planning for my first build.  First, a few things about me and my plans for this build.  I am 180lbs(~81kg) and I live in a very flat area.  My goals for this build are a light and discreet machine to act as last-mile transit on and off of light rail and for cross-downtown trips.  The longest single leg of transit that I plan on going is just under 4 miles.  I would expect to be able to charge at the end of any single leg of the journey, and my expected range out of the system is just over 6 miles.  My top speed requirement is 18mph.  Hopefully I will be able to go faster than that, but for my first board, I think 18mph should be enough.  I am very much decided on using hub motors, as I really like the elegant solution and reduced component count and maintenance.


I have a preliminary parts list from two vendors that I would like feedback on.  I am trying to balance low cost with high quality, durable components that are "community standard" parts that will transfer well into future builds.

Vendor: carvonskates.com
$299.00 - CARVON V2.5 SINGLE HUB MOTOR + FRONT TRUCK + WHEELS SET (RAW EDITION)
$99.00 - VESC FOR CARVON HUB MOTOR


Vendor: miamielectricboards.com
$269.99 - 12S2P Stealth Battery (with power switch and LCD panel)\
$59.99 - Handheld Electric Remote
$49.99 - Freesytle Deck
$19.99 - VESC Bluetooth Adapter
$9.99 - Grip Tape


This brings my build total to just over $800.  I would be sourcing hardware to mount the trucks (and risers, if needed) from a local skate shop.  I have a bunch of kydex left over from making custom holsters and I will be forming my own enclosure for the battery / reciever / vesc.  I would also be going to a hobby shop to pick up XT60 and bullet connectors to finish off the wiring.


Thanks in advance to all reading here, and I look forward to input on this future build.  I will update this thread as parts are ordered / delivered and built.
```

---
## \#2 Posted by: wookiepedia Posted at: 2016-12-05T15:17:41.238Z Reads: 143

```
Because I know it is going to be difficult enough to sit by the mailbox until the orders to come in, I have paid for the above products and now the wait begins.
```

---
## \#3 Posted by: wookiepedia Posted at: 2017-01-03T01:16:37.626Z Reads: 131

```
I've gotten confirmation that my hub motors from Carvon should be shipping next week, so I'm getting this build moving again.  Thus far, I've taken to riding the deck unpowered using some horrendously cheap (but surprisingly decent) 180mm trucks and 90mm wheels from amazon:  https://www.amazon.com/gp/product/B01IBJXW4W/ref=oh_aui_detailpage_o07_s00

I'm really liking the board so far, and have never ridden anything with wheels bigger than 53mm, so it's a very different experience.  Cracks in the sidewalk and gravel no longer are life threatening!  I tried to heat form an enclosure for my MEB battery, which did not go very well.  I need to either build a press, or order an enclosure.  To that end, I have messaged @Dunkirk about an enclosure for the battery/switch and another for the VESC/bluetooth/receiver and shipping across the pond.

I am very excited to get the board mocked up with velcro as soon as the motors arrive and do some testing and tuning!
```

---
## \#4 Posted by: wookiepedia Posted at: 2017-01-09T01:04:12.467Z Reads: 116

```
So, impatience has gotten the better of me, and I've changed direction (again) on the enclosures.  I am having a local shop print out @emancarrillo 's battery box and VESC enclosure found here:  http://www.electric-skateboard.builders/t/vanguard-12s2p-meb-stealth-battery-sk3-149kv-i-vesc-3d-print-pulley-cover/6978/36

The guy doing the printing seems very cool and has been communicating progress as the print goes on (I think my total print time was close to 60 hours) and I managed to run him out of green filament!  The enclosures should be done tomorrow, the same day my hub motor and VESC arrive from Carvon.  Now I need to do some more research on the VESC and see if I'll need to borrow a power supply for the first boot up.
```

---
## \#5 Posted by: wookiepedia Posted at: 2017-01-12T07:29:24.380Z Reads: 108

```
All of my parts are in and I need to go pick up the enclosures from the 3d printer.  I temporarily mounted everything on the board using industrial velcro and some duct tape and took it out for a spin.  I left the house at 94% of the 12s2p pack and traveled 2 miles.  Battery pack was at 77% when I got back.  That's roughly 8.5% of the pack per mile, giving me a back of the napkin usable range of about 10 miles (no way I'm gonna drain the pack completely).  This is very much in line with the orignal goals for this build.

http://i.imgur.com/l0x1sdx.jpg

The acceleration is pretty weak, but once it gets moving, it really goes like crazy.  Hill climbing ability is about what I expected (pretty poor) but I live in a flat area so I'm fine with that.  This thing can get going fast enough that I really need to tighten my trucks more!

As soon as I can get the enclosures prepped and toss all the gear inside, this will be a pretty darn sweet ride.  I'd like to give a shout out to @oriol360 for the awesome battery pack, remote, and deck.  Also, Carvon for the hub motor and vesc.
```

---
## \#6 Posted by: wookiepedia Posted at: 2017-02-20T19:08:16.144Z Reads: 79

```
Quick update for anyone following my build:  I misdiagnosed my battery pack being empty (which shuts off the motor) and went down a rabbit hole of "troubleshooting".  I changed the cutoff voltage on my VESC, setting it WAY too low and killed my MEB stealth pack battery.  I learned a valuable lesson.

I have one of @oriol360 's new 12s3p packs on order and will be putting that in the mix when it arrives.  I expect this will help extend range a bit and also will give me more headroom for current draw.  In the meantime, i have been riding an unpowered longboard and improving my balance and feel for riding.  Some day, I'll probably end up making the beercan boards root beer into an electric board as well.

Once the new battery arrives, I'll relocate the bottom half of the battery box to accomodate the bigger pack and also put the VESC, bluetooth module and receiver inside their enclosure to tidy things up.  I can't wait!
```

---
## \#7 Posted by: rwxr Posted at: 2017-02-20T19:16:54.604Z Reads: 75

```
More pictures!
```

---
## \#8 Posted by: Michael319 Posted at: 2017-02-20T23:28:04.961Z Reads: 70

```
What was your cutoff? and what is your new cutoff?
```

---

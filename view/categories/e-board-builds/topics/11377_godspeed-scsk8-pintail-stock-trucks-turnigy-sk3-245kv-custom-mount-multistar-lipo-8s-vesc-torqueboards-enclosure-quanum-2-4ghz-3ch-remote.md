# Godspeed &#124; SCSK8 Pintail &#124; Stock Trucks &#124; Turnigy SK3 245kv &#124; Custom Mount &#124; Multistar LiPo 8S &#124; VESC &#124; Torqueboards Enclosure &#124; Quanum 2.4GHz 3Ch Remote

### Replies: 9 Views: 1472

## \#1 Posted by: Alanhunt123 Posted at: 2016-10-18T20:12:02.607Z Reads: 265

```
Hi guys!

This is my first build, and I call it Godspeed. It has a top speed around 22MPH, and a range of about 16-18 miles, depending on the conditions. This is really all I could ever need for speed and range, but we'll see what happens. In a few months, I'll probably be wanting to build another one!<img src="/uploads/db1493/original/3X/c/4/c41f37eb4ac5bfeef00fcf0789620c6d72332136.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/8/a/8ab053ce932c83911963a227bbafcf92fbc8becb.jpg" width="500" height="500">

This design uses a cheap SCSK8 Pintail board with the stock trucks. I made the motor mount myself in my school's CNC shop, and welded it to the trucks using a special plate adapter that I made to ensure the mount is welded straight. This is super important, because I have heard from friends that did not weld theirs straight that their belts wore out fast!

I used a 15mm HTD belt with a 14 tooth pinion, and a 40 tooth wheel pulley that a friend 3D printed for me. The wheel pulley is specially designed to fit in the 83mm and 90mm wheels with inner hubs. I'm using 83mm wheels. I chose this wide of a belt as a recommendation from my friend because he said he has never had to replace the belt due to its toughness.

The ESC is a VESC from Enertion, which initially had some issues. I think it may have been the small motor connectors that I had being low quality that led to the demise of the DRV chip. Thankfully, Charles from Enertion offered to replace the DRV free of charge, and I had the board up and running again within a week and a half. After replacing the 3.5mm bullet connectors with 5mm connectors, the VESC has had no issues. For settings, I have battery current limited at 40A out and 18A in (regerative braking). This has proven very good for flat surfaces. I may end up increasing the limit to 45A or even the full 50A if it's not enough once I move back to school where there are lots of hills.

The motor is a Turnigy SK3 245kv motor, and it provides plenty of power! Can climb hills easily, and will easily push the board to ~22MPH where I have the limit set on my VESC. The motor has more left in it, but this is as fast as I want to go at the moment. I may open up the limit just so I have a bit more passing speed on bike paths.

The batteries I am using are Multistar 4S 5,200mAh packs. I'm using 4 of them in this build. They are connected together so that it creates a "8S2P" configuration. I have the balance leads of the packs in parallel connected together so that the cells stay at the same voltage between packs. The motor specs also say it can handle up to 10S, so I may build a second battery pack for this board that uses 3 or 6 3S packs to make 9S, or 2 or 4 5S packs to make 10S. Or I'll go to a 10S setup with 18650s since my friend has a spot welder that I could use. I'm not using a BMS at the moment, but may end up doing so in the future, since I think having to take out the batteries to balance charge every time is going to get old very quickly. The current wiring setup for the batteries can be seen below.

<img src="/uploads/db1493/original/3X/a/1/a10f70f0801300d2e1cce66741ebd229e3a8778e.jpg" width="260" height="500">

All of the electronics are held inside the 2X6S RC LiPo Battery Enclosure from DIY Electric Skateboard. If I had this to do over, I would not have purchased this enclosure, since it is made of some pretty cheap plastic that cracks easily. The included hardware is garbage, as it does not hold it on securely. Within 100 yards of travel, the enclosure would fall out. So, I had to upgrade to some 1/4-20 bolts that I fed straight through the board to some drilled holes in the enclosure. This held for a little bit until one of the bolts tore a clean hole straight through the plastic! Surprisingly, the hole didn't propagate into a crack throughout the enclosure, so it was still usable. I made some aluminum braces to hold it on, but at this point, the case is difficult to take on and off for charging.

For a controller, I am using a cheap Quanum 2.4GHz 3Ch remote from Hobbyking. It's cheap feeling in the hand, but it works well, and has had no drop-outs. For those wondering, it has a little button on the handle for activating the 3rd channel. It simply switches between 2 positions if you hook up a servo to it, and only switches to the 2nd position while pressed.

I just got back from my 2nd test run today. I calculated that the board should go an absolute minimum of 16 miles on flat ground based on some other builds that I have seen on this forum. I rode 8 miles, turned around and headed back down a paved bike path which was almost completely flat. This yielded a total of 16 miles on the board with no problems. When I got back to my car, the batteries were still at 3.79v/cell! The board could have easily gone another 2 or so miles on this charge. This was including having to constantly slow down and speed up to avoid hitting some wide cracks in the road too hard, as well as crossing streets. I could have gone further, but I didn't want to go so far that I couldn't make it back! Also, my feet were very sore after this ride, so I didn't feel like going further.

Well, that's it for this build, feel free to ask questions, I'd be happy to answer them!
```

---
## \#2 Posted by: sl33py Posted at: 2016-10-18T20:27:46.911Z Reads: 218

```
Nice build and looks good!

If you aren't having any issues w/ your batteries i would leave it as is.  I'd spend that $ on another motor/mount/VESC if you want more power next.  This looks like a perfect starter board and i'd go dual diagonal if you want more start and passing power (won't increase top speed, just acceleration and torque).

[quote="Alanhunt123, post:1, topic:11377"]
4S 5,200mAh packs. I'm using 4 of them in this build. They are connected together so that it creates a "2S2P" configuration
[/quote]

That would be 8s2p 10,400mAh!  that's some miles per charge!  What cells are those?  10c multistars?  Any issues w/ this setup?

nice DIY build man.  congrats!
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2016-10-18T20:58:48.113Z Reads: 199

```
Yes, these are the 10C multistars. I've had no problems with them. Before the VESC blew up, I tried 2 of them instead of 4 and they were only a little warm. With the current setup, they are being drawn at 3.84C or less, so they last a long time.
```

---
## \#4 Posted by: willpark16 Posted at: 2016-10-18T21:26:24.472Z Reads: 187

```
bms integration so easier charging
```

---
## \#5 Posted by: torqueboards Posted at: 2016-10-19T05:49:05.381Z Reads: 172

```
@Alanhunt123 - The enclosure was never meant for the actual battery weight to be supported by the enclosure in anyway shape or form. For any ABS enclosure for that matter. If you do that, it will become damaged overtime.

Personally, I would use adhesive velcro + velcro straps (bolted to the deck) to support the weight of the battery pack. The enclosure itself is only meant to be a housing to protect it from the elements.

I also don't use a bolt + nut that way you can easily press down, slide and pop the cover off for changing your packs or charging quickly. Hope that helps.
```

---
## \#6 Posted by: Alanhunt123 Posted at: 2017-01-05T15:13:40.177Z Reads: 124

```
Unfortunately some of the cells are going out of whack on this pack, cutting my range in half and doubling my charge time. This setup really needs 9s or 10s I find, because the motor just doesn't have any umph when the pack is drained to half charge and the voltage has sagged. I'm going to be doing a huge update to this board soon, including 3 3S 8000mAh flightmax batteries in series!
```

---
## \#7 Posted by: sl33py Posted at: 2017-01-05T19:41:11.297Z Reads: 119

```
I think your 10c packs and sag are biting you...  potentially over discharging and unbalancing.  be careful to not damage/puff your cells!

You're doing a re-do so i hope your next setup works better.  I'd recommend a higher C setup regardless of what you go to.  If you are over demanding the Amps that the battery can't provide easily - you'll get huge sag, poor performance, and potential damage to the pack.
```

---
## \#8 Posted by: wmj259 Posted at: 2017-01-05T19:44:24.760Z Reads: 118

```
Multistar batteries are good for drones, the energy hunger is usually low unless its aerobatic/professional photography ones.
```

---
## \#9 Posted by: Alanhunt123 Posted at: 2017-01-06T21:11:45.538Z Reads: 109

```
It's funny, I never exceeded the max draw of these batteries, which would be a calculated 104A (max battery discharge was set to 50A). I also calculated the max charge should be 20.8A (based on the 2C max that hobbyking had on their website), so perhaps my 18A regenerative braking setting was a bit too much for them.

I never discharged the cells past 3.6V/cell, and usually discharged them to 3.75V/cell. So, I don't quite know what gives with these cells, as I balance charged them every time. Oh well!

The flightmax batteries are 30C discharge (240A max) and 5C max charge (40A max), so I think they should be fine. I'll set my regen on the conservative side, probably leave it around 18A, since the higher voltage will give me a little more braking power.

I also plan on using a new deck for the updated build, since this one is a bit large, and is getting pretty ugly with all the holes I drilled in it to experiment with different systems (including a custom CNC milled VESC enclosure to help with heat dissipation). I'm chucking the plastic battery enclosure, and will use an aluminum enclosure that I will make out of sheet metal and CNC machined parts. Should be able to get a much lower profile, which will make the board look sleek!
```

---

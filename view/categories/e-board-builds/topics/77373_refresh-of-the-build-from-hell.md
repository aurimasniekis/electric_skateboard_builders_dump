# Refresh of the build from hell

### Replies: 9 Views: 398

## \#1 Posted by: Livid Posted at: 2018-12-07T20:59:12.178Z Reads: 204

```
Since I've built it I've put about 100 miles on my deathtrap board from hell (only fallen off properly once... oops) 
Old post for reference: https://www.electric-skateboard.builders/t/my-deathtrap-board-100kv-90mm-hub-motors-10s2p-27-deck-maytech-vesc-4-12-modified-firefly-remote/71216

But I kept having issues, for a start the remote kept disconnecting, so I opened both the remote and receiver up and changed the voltage regulation, and it still kept disconnecting, but only by locking the throttle in position. After 3 near death experiences I gave up and ordered a nano x second hand. 

The battery also gave me some pain and suffering. It was not really up to the task of 2400W, any puddle whatsoever and the BMS got water in it and shut off the battery, with no prediction for when it would decide to turn back on. Also, it kept falling off, and it can only happen so many times before you start worrying cells are gonna get punctured

The sandwich box was a good budget friendly idea for an enclosure, but it was pretty cramped, no room for expansion. Connecting the XT60 led to some nice spectacular sparks, and that can only happen so many times before some john doe questions whether or not the board is safe.

The hub motors also have an annoying tendency to loosen the one that rotates contrary to the direction of the thread, so it ends up rattling back and forth on the little indexing square, which aside from making a bloody annoying noise when freewheeling also fatigues the wires which is not a good thing

The nano x was the first to get sorted, I opened it up to reverse the potentiometer because I'm too lazy to hit that bloody button every time I turn the remote on. It does play up with issues connecting on power up, but has been rock solid once I've connected it. No telemetry either unlike the firefly, so I hooked up a bluetooth adapter to read battery levels

New battery was a pair of 5000 30c 5s packs off hobbyking https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack-xt-90.html
I soldered the packs in series, which went fine, rewired the balance port for a charge only bms, which went fine. then after I was just checking the voltages on the balance connector prior to connecting the bms, without removing the xt60 I used as a jig to hold the pins in place aaaand
![20181207_204218|375x500](upload://lYralqdKDgBbsAfBxr8zqrdxDPD.jpeg) 
I accidentally shorted the terminals with the multimeter probe. Made one hell of a bang, the multimeter probe was just gone. Did I mention I did this in my university lab with about a hundred people in the same room? Good news is that didn't damage the pack at all and I've been using it for ages, but it also kept falling off.

Next step was an enclosure and anti spark. I'm using a 100A variant of the fatboy mini sparky switch and the smallest enclosure from eskating.eu
![image|257x500](upload://3LOXSZIBtnQbMuqLuiDldXcupne.jpeg) 
bit of a cramped fit but I got it all in, also uncrossed the motor wires as they were chafing pretty badly with the old setup. PTS doesn't work too well. My suspicion is that because I'm running hub motors they need to go super fast to generate a voltage high enough for the switch to detect it and turn on. 
Quite pleased with how I did the charge port. A bit of filing and epoxy and the XT60 is installed nice and slick. water resistant too, the whole thing is quite well sealed now, held on with 8 m4 screws as opposed to velcro and electrical tape. don't think anythings gonna fall off anymore :stuck_out_tongue:
Other than that it's the same. new pack gives much more consistent power so it really pulls hard now. same backbreaking ride. If only I didn't lose the light at some point when I was going along the route I fell off, then it'd be perfect. maybe some shredlights when I can afford it.
What are your thoughts on how I've polished this turd?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-07T21:44:39.393Z Reads: 143

```
You not afraid to short put the lipos?
The terminals not isolated at all and there are a lot of parts flying around in your enclosure that can easily cause a short.
```

---
## \#3 Posted by: Livid Posted at: 2018-12-07T22:06:41.217Z Reads: 137

```
Everything's secured within the enclosure, i made sure of that. I've shorted this lipo once before and i nearly had a heart attack. I probably should have put some kapton or something on it though that's a good point. I'll do that next time i have reason to open it up
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-07T22:17:09.645Z Reads: 139

```
![image|298x499](upload://59wDvO6gKIGZ3eHbbq2wZrFAwtI.jpeg) 
All this area doesn’t look good in my humble opinion.
This tape looks like it’s falling off when just looking at it.
As you already shorted the battery once, i‘m Sure you don’t want it happen a second time.
It might look good now, but how knows how things move when driving. There not only good vibrations 😜😂
Seriously, get your Terminals isolated, better sooner than later please.
```

---
## \#5 Posted by: Livid Posted at: 2018-12-07T22:30:21.780Z Reads: 120

```
ohh those terminals. the battery came like that. it's fine, I'll insulate that too
```

---
## \#6 Posted by: dareno Posted at: 2018-12-08T01:59:45.312Z Reads: 103

```
After reading that write up I'm not sure you wouldn't be better off with a meepo dude.  :stuck_out_tongue_winking_eye:  Seriously though that was a funny read.  Not having much luck there hey? Looks better now but do get some insulation on those batteries because judging by your run of luck they will go up soon.
```

---
## \#7 Posted by: Livid Posted at: 2018-12-08T10:12:46.569Z Reads: 83

```
Everything i build goes this way, long past the point it would have made more sense just to buy a prebuilt one of whatever it is i'm making at the time :stuck_out_tongue:
```

---
## \#8 Posted by: pat.speed Posted at: 2018-12-08T12:50:14.417Z Reads: 69

```
I think anyone can make anything if they spend enough time learning and put enough effort into it. 

I think that applies here, you really need to open this up take it all apart and put it back together properly, with correct insulation, connections and neat wiring. 

I don’t know if you have kids or anyone who lives with you but would you risk your house for the price of some kapton tape, fishpaper and heat shrink. I know I wouldn’t
```

---
## \#9 Posted by: Livid Posted at: 2018-12-08T17:16:31.349Z Reads: 50

```
Thanks for the concern, i've added some extra electrical tape on the battery terminals on top of the kapton and masking tape hobbyking put on and some VHB to secure the anti spark switch and bms, which had started floating around on the short ride back from the lab i built it in. This board wasn't my first time playing around with EV's, Lipos, this much voltage and definitely not my first time screwing around with this much current, I know the limitations, i wouldn't have bolted the enclosure on if I didn't think it was electrically safe. I'm not denying it's a mess, everything I build is a mess covered in hot glue,  but there's a difference between a mess and unsafe
```

---

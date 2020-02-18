# Splitting/swapping batteries with BMS in the mix

### Replies: 11 Views: 1105

## \#1 Posted by: landonkun Posted at: 2016-11-17T08:53:31.022Z Reads: 105

```
First of all, hey everyone! Been reading for a few weeks, but only recently started posting, and this is my first topic.

I'm about to build my first board, and while I think I've figured out how I want to do it, I have a question that was sparked by the airline regulations thread.

I'm thinking of doing a 10S2P build with the Basen li-ions, but that would put at well over the allowed 160Wh limit of most airlines.

My question is: is there some way to design the battery so that I'm able to "break" it in half (maybe with an XT60) to 2 x 5S2P for airline allowance while still having a BMS attached?
Or is there a way to make the BMS easily detachable as well?

My other thought was to do something like Boosted and simply design a smaller pack for travel, and have an extended pack for when I'm home, but again, I'd run into the issue of swapping out the BMS between battery packs, and don't know if that process can be made any easier.

Any thoughts appreciated. You guys are all awesome! :slight_smile:
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-11-17T08:56:08.279Z Reads: 103

```
Paging Dr. @barajabali  🏥

Is the Doctor in the house lol
```

---
## \#3 Posted by: im-done Posted at: 2016-11-17T13:18:58.477Z Reads: 96

```
Are you running you main power through the bms or only using it to charge? If you are only using it to charge you can use header pins to connect the bms to the battery and swap it around, just make sure you add a way to make sure the bms does not fall off(screws or a lid). For the batterys if you can print out a hard case for the liions than you may be able to make it like legos, where you can snap them together to add a parallel pack. The only thing is that since the cells have not always been used together this may not be the greatest idea. Hope this helps.
```

---
## \#4 Posted by: barajabali Posted at: 2016-11-17T16:00:49.858Z Reads: 81

```
@landonkun  Hey man! 

That is totally possible. Breaking the connection between the 10 cells would be easy as your just going to break the 5th series connection.  The issue is that your balance leads will all still be connected to each pack.  Even if you unplug the balance leads from the BMS, the leads will still be a 'spider web' and  connect the two packs together.  To solve this you could try to get (2) 5pin leads and jam them in the 10pin jst plug that way each one can get unplugged alone.  You would need to modify them to fit though,  Also make sure you never switch their positions or you will ruin your bms.

At the end of the day.  Itll still look 'bomby' so im not sure that it is a feasible solution

EDIT* of the two packs, one will carry the main negative terminal.  The one with the negtive terminal will need a 4pin lead, and the other pack will need a 6pin  lead.
```

---
## \#5 Posted by: chinzw Posted at: 2016-11-17T17:59:30.186Z Reads: 60

```
I have exactly this but instead of 10s i have 6s. Check my build log: http://www.electric-skateboard.builders/t/skelly-bustin-eq-36-hollowcore-diyes-single-kit-sk3-6364-190kv-turnigy-150a-esc-gt2b-baby-buffalo-6s3p-5000mah/8804

What i did was make a Y series for the main leads and a Y series for the balance port. Its pretty simple, but its totally modular, so if i need i can unplug everything, swap batteries, etc.

EDIT: some picks so you don't have to go through the whole thread.

<img src="/uploads/db1493/original/3X/8/c/8c7e1ab26593be481511c282c00b584a34997792.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/6/5693fa294fd9af2bad768e6519000c5479dce484.jpg" width="666" height="500">
```

---
## \#6 Posted by: landonkun Posted at: 2016-11-17T20:28:26.303Z Reads: 44

```
@im-done 

I didn't know it was an option to have it run through main power or only for charging. I'll have to do more research on here to find out how that affects things.

@barajabali 

Awesome. That sounds like a fairly easy solution. Except for the 'bomby' part, haha. I guess there's no way around that.

@chinzw

I suppose that's the advantage to using lipos - it just looks cleaner. And less 'bomby,' haha.

_*sigh*_
Sometimes I feel like going with the new Blink S2 would just make life easier for a travel board, but being 6'7" and 200lbs, I'm worried I wouldn't get anywhere near the top speed/range :frowning:
```

---
## \#7 Posted by: im-done Posted at: 2016-11-17T20:41:11.961Z Reads: 41

```
Running your power through the bms will keep your cells balanced and have a amp limit. A ton of bms's will not handle the amp we require so a lot of people just bypass that part and only use it for charging.
```

---
## \#8 Posted by: im-done Posted at: 2016-11-17T20:47:00.761Z Reads: 41

```
O and i just remebered this.
https://youtu.be/8b9ZYt6MzHc

Dewalt solved the issue of shipping their batters by air by having a series parelle switching circut. So when they mail them its at 20v and blank amps that keeps it below the mailing limit, but when you get it and change it to 60v and blank amps you are now above the mailing limits. You could use a system like dewalts as a loophole in the system but like @barajabali said it looks kinda sketchy.
```

---
## \#9 Posted by: chinzw Posted at: 2016-11-17T22:00:52.159Z Reads: 36

```
You can do exactly what i did with li-ion, there's literally no difference. A battery is just a battery.
```

---
## \#10 Posted by: landonkun Posted at: 2016-11-17T22:41:16.800Z Reads: 30

```
@chinzw 

I was mostly referring to the fact that lipos generally look cleaner when bringing them on airplanes, as opposed to a homemade li-ion pack, which can still look really clean, but who knows what airline agent I might wind up dealing with...

I like your build, by the way! Very nice. I'm in Winnipeg, but next time I find myself in Vancouver, we should totally go for a ride.
```

---
## \#11 Posted by: chinzw Posted at: 2016-11-17T23:19:15.303Z Reads: 23

```
Yeah, thats true. Im guessing a nicely heat shrink wrapped li-ion should look very professional too.

Thanks, and ofc hit me up when you come over.
```

---

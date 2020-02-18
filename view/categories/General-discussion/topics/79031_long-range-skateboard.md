# Long range skateboard

### Replies: 21 Views: 713

## \#1 Posted by: Kempo1 Posted at: 2018-12-26T15:54:41.955Z Reads: 204

```
I’m looking to have a nice long range skateboard. My options are buy  a new board and fix it to my liking or buy a battery pack capable of long distances and put it on my original board. A new board is right around same price as a new battery pack so I’m not sure what’s a better option for me... can anyone stir me in the right path? Thanks!
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-12-26T16:43:35.300Z Reads: 190

```
Ill give you a potentially cheap alternative option, but it will take a tad bit of work. This is definately not for everybody but if you like to tinker, want something fairly cheap and dont mind if its (depending on how you do it) super DIY looking...

1: Keep your current battery. Recycle old laptop cells into a custom battery pack. Check recycling centers, drop off points, remove and test the cells with a capacity testing charger. Most laptop cells even come pre-spot welded making soldering wires to existing nickel strips easy. Need to buy [suggestions]: litokala li-500 charger $20, 1-8S voltage checker/alarm $5, balance leads $5?, shrink wrap or packing tape, soldering iron, wire, shrink tubing and connectors... a lot of times I manage to find old barrel connectors on old power adapters that can be resoldered to fit your needs for free... balance charger or charge only BMS + charging wart for whatever voltage your pack comes out to, doesnt need to be as much as your main pack.

1(alternative): buy some or find some old power tool batteries! Thats it for that... then

2: connect battery pack to a $15 boost converter, set voltage and amps according to your boards specs

3: get creative mounting it on your board and just simply charge while riding. 

Some people don't recommend this since not all BMSs are meant to charge and discharge simultaneously, but i've never heard of anyone having issues. Plus technically there is no such thing as charging and discharging at the sams time. 

Either way, thats an option and if you already have materials, batteries or power tools laying around, it could cost you as little as $15 via prime for a boost converter to extend your range for as far as the batteries you connect to it can charge you.

This way, im able to push my 10S4P board, at full power for as long as I want. I carry around a backpack full of external batteries, and at the end of the day on group rides when everyone else is needing to be pushed because they are at 0%, im still at 98%. My old 10 mile limit is now 20++++++ miles, depending on what I carry with me. Ive never ran out of charge and don't care to try to honestly.
```

---
## \#3 Posted by: Kempo1 Posted at: 2018-12-26T16:50:41.382Z Reads: 139

```
This doesn’t sound like a bad idea and do have a battery pack laying around from my original board. Is there any videos or anything I can use as a guide I’m learning electronics now and just wish I had a better understanding of everything completely. I have a digital battery meter the only thing is the balance charger I don’t have. And I’ve spent months riding my brand new blitzart deck until it stopped working took me months to figure out how to fix it. I fixed it but now having a charging issue and that’s why I’m unsure if I want to fix this or get a new deck. But the option your saying sounds way cheaper just a little confused on the exact set up.
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-12-26T16:58:00.513Z Reads: 126

```
You would need to figure out your charging problem then. Whatever you do, just know that your charging port is connected to your battery, so don't short the charging ports connections if you start poking around to figure it out. 

After you get your board sorted or get a new one, if you are still interested in using your spare packs to charge on the go, check out this thread: https://www.electric-skateboard.builders/t/range-extender-plugged-into-charge-port/64327
```

---
## \#5 Posted by: Kempo1 Posted at: 2018-12-26T17:02:57.367Z Reads: 115

```
That I believe maybe my problem is my charging port. Is there a guaranteed way to tell if it is in fact my charge lead because that’s an easy fix. My board is reading 33 volts on multi meter but saying it’s dead when turned on and in motion. Along with the charge light stays green while charging and won’t turn red? I will definitely give that article a read I’m super interested in extending my range just not sure how or where to start and I appreciate all the help.
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-12-26T17:28:53.138Z Reads: 120

```
No guaranteed way since it could be a number of issues and not just one. But most likely one. You can tell for sure by isolating the component thats giving you the problem.

Where exactly are you reading 33 volts from? Pictures would help. What are your boards specs? Charger voltage? 

Green light staying on could mean bad charger, I've seen that happen but I don't think that's your problem because of the other symptoms. 

Dead/burnt out antispark could mean you read voltage sitting there but get nothing / low voltage when trying to ride. I'm guessing this also isn't your issue, assuming your board only has one issue... But if it turns out there are multiple things failing this is something to keep in mind. 

Are you running VESCs? Are the vescs getting any voltage? 

The most obvious problem I'm thinking is that your BMS is probably dead if the board is not charging and it's dead when trying to ride. If it's a battery from a pre-built, it's most likely wired for charge and discharge, and probably not the highest quality? Just to make sure it's not a P group in your battery, you can test each P group with a multimeter to make sure none of the cells are out of balance or abnormally lower than the rest of the parallel groups before concluding that your BMS is the issue. 

You can also probe your BMS, negative terminal and balance leads to make sure your BMS is reading each P groups increasing voltage correctly (depending on charge level, but for example: 1-3.6v/2-7.2v/3-10.8v/etc). If a balance lead has become disconnected somewhere, the BMS would refuse to charge your pack and might just shut down. 

I'm not a battery expert, but I'm sure some of the experts on here could chime in to help out. If you don't feel comfortable that you 100% know what your doing to not short anything or cause a fire poking around, I'd look into getting professional assistance or just buying a new pack... Just saying this since I don't know exactly how comfortable/experienced you are so I appologize ahead of time, maybe some people if they are completely new and read this should be cautious at least. Regardless, this is a DIY forum, so if you do feel adventurous, do some reading on battery safety, have a plan for if things go wrong as batteries can get explosive if you don't know exactly what you are doing. Get educated if you start poking around basically, or live and learn by your mistakes and try to not make deadly ones.
```

---
## \#7 Posted by: Kempo1 Posted at: 2018-12-26T18:28:54.035Z Reads: 99

```
Yes I’m not super educated in electronics but I have a general understanding. Not super comfortable poking around to be honest and was hoping there’s a simple way of doing it but if not I’m gonna have to get a new pack. It’s a generic vesc I believe.![image|375x500](upload://bUMc6lTimJTfMKz6ASVS0XNtuu2.jpeg) and here’s my battery pack ![image|375x500](upload://mbeozFMogrfKDIeP6Dg72ItphsZ.jpeg) and I think it’s either the bms the charger or the charging port. Or possibly a bad connection 3/4 down the row of battery’s but don’t want to just start poking and having something blow up or short out. And quiet possible that I may have already shorted something. So I’m up in the air on what to do
```

---
## \#8 Posted by: Battosaii Posted at: 2018-12-26T18:54:09.618Z Reads: 89

```
What do you consider long range?

For me my 12s4p gets me from 22-30miles range depending how I ride to me that's not long range as I could drain my battery easily on group rides. 

Now I built my self a 12s8p and I get 45-60miles range on 107s  I now never have to charge or worry about range on most group rides.
```

---
## \#9 Posted by: Kempo1 Posted at: 2018-12-26T20:18:35.485Z Reads: 83

```
How would I go about getting a battery with that range capability? Is there places that sell pre built packs? I’m not savy enough I don’t think to do it myself unless I would.
```

---
## \#10 Posted by: swimmydude Posted at: 2018-12-26T21:17:27.418Z Reads: 76

```
I take it that you're trying to buy a pack rather than make one. You're basically looking for a battery pack that has a higher number of cells in parallel. 6 is a solid number, I'm not sure if they go much higher than 6 though. Depending on what you end up doing, space is a consideration too. So any more than 6 can start getting bulky.
```

---
## \#11 Posted by: directC Posted at: 2018-12-26T21:39:57.860Z Reads: 75

```
With what setup are yiou draining your 12s8p?
```

---
## \#12 Posted by: Battosaii Posted at: 2018-12-26T21:50:09.699Z Reads: 70

```
4wd 6374 with 16/36 pullies and 107mm wheels.

Here's my.build thread.
https://www.electric-skateboard.builders/t/cumulus-nimbus-4wd-12s8p-evo-street-build/57192
```

---
## \#13 Posted by: Kempo1 Posted at: 2018-12-26T22:50:39.129Z Reads: 57

```
How much on the battery and what’s the range on the pack?
```

---
## \#14 Posted by: directC Posted at: 2018-12-26T22:53:17.488Z Reads: 55

```
Nice!
Do you think it's possible to fit a 12s10p battery in this enclosure?
Would a Unity fit into the endpart of the enclosure?

Got the Evo and the DS enclosure but nothing else yet, so i can't test, but dream ;)
```

---
## \#15 Posted by: Battosaii Posted at: 2018-12-26T23:05:04.296Z Reads: 52

```
I really pushed it to fit that battery. You would need some battery making magic to fit a 10p on there even with a dual set up.
```

---
## \#16 Posted by: directC Posted at: 2018-12-27T00:43:16.983Z Reads: 42

```
I guess i need a TS enclosure ^^
Or just mount a battery box on top - did someone do that yet on a evo?
```

---
## \#17 Posted by: Battosaii Posted at: 2018-12-27T00:47:57.188Z Reads: 41

```
It's possible though. 

@deckoz fit a 13s5p in his single stack. I'm sure if you did a similar design to him but 12s and double stack you could squeeze a 10p in there. I thought about it but I wanted 4wd.
```

---
## \#18 Posted by: directC Posted at: 2018-12-27T00:54:02.941Z Reads: 45

```
Mounting the Unitys on the deck would help
Just not sure if it's the best idea as i have no clue how watersafe it is and heard that silicone stops doing it's job over time (at least people say so) if you would just spray it
```

---
## \#19 Posted by: Battosaii Posted at: 2018-12-27T00:59:37.129Z Reads: 47

```
He has the ESC in the enclosure and he's using Focbox, unity is slightly smaller.
```

---
## \#20 Posted by: Kempo1 Posted at: 2018-12-27T18:05:50.058Z Reads: 35

```
Do have any places that are good and reliable to buy prebuilt packs?
```

---
## \#21 Posted by: directC Posted at: 2018-12-27T18:18:44.243Z Reads: 34

```
https://www.electric-skateboard.builders/t/wiki-approved-battery-builders/78661
```

---

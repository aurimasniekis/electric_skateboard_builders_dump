# Adding another battery to the skateboard

### Replies: 15 Views: 1625

## \#1 Posted by: Adelgaard Posted at: 2018-04-27T17:27:08.880Z Reads: 167

```
Hi (sorry for my bad english, also I could not find another topic of this problem)
I recently bought an electric mountainboard for riding on the beach. I love it!
I have imported it from China, so it's not the best quality - but its a joy to ride.
I only have one problem with it... The battery capacity.

It has to be charged for 4 hours after only short period of riding time.
I know that sand is taking a lot of power + my weight of 80kg.

I don't know much (if anything) about batteries, so that's why i'm asking you guys...
"Is it possible to add another battery the to skateboard?

I would love to not having to solder new wires to the componens, so I was wondering if it is possible to add a battery and connect it to the charger input of the existing battery. (as seen on the photos) I know this would mean to charging cables.
![skate bat|580x500](upload://59RcncWKG57GiRhRNrflhsJsI72.jpg)

If this is possible, what kind of battery is needed?

I guess i would need:
* A battery with enough capacity for riding a long time.
* A battery enclosure. 
* A charger.
* A cable that goes from the new battery output to the old battery input. 

Some of the specs of the board.
* 3300W
* 11ah battery
* Samsung Lithium /50cells
* The charger is an 42v/2a.
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-27T17:33:49.642Z Reads: 158

```
You can't just connect another battery to the charge port. You would destroy your house if you did.

Your options are:

Buy a premade battery pack from reputable vendors

http://www.enertionboards.com/on-sale/r2-spare-battery/

OR

collections/electric-skateboard-battery-pack

You can also get a custom battery pack from our vendors here. ( @longhairedboy @psychotiller @barajabali   )
```

---
## \#3 Posted by: barajabali Posted at: 2018-04-27T17:45:03.988Z Reads: 141

```
chibatterysystems.com
```

---
## \#4 Posted by: Adelgaard Posted at: 2018-04-29T14:34:00.267Z Reads: 117

```
Thanks for you help!
Okay, so connecting it to the charger is not possible!

I just opened the board to see how it's wired.
The battery is connected to the boardcontroller via a XT60 cable.
![skat2|666x500](upload://lgXBplMgN235amxk4NJlg6ZtrGF.jpg)![skat1|666x500](upload://whguIDxSqoKywVk2FHdVAzRZ2Lg.jpg)

Is it possible to connect a "XT60 Female to 3 way XT60 Male" cable and connect 2 extra batteries to it? (This one https://ebay.to/2rdyRxp)
![cable|500x500](upload://we7BUR2uQrAeGemRpqspYkm78mp.jpg)

Will that make i parallel, so I get extra range from the batteries?

The battery i've been looking at is an "36v electric scooter battery 36v 16ah 10s5p li-ion" will 2 of those work whith the board though the 3-way wire?  (here it is: https://bit.ly/2r7fXZs)
![36v-electric-scooter-battery-36v-16ah-10s5p|500x500](upload://imauofcFkAmlchRUIjCYnh2uvnr.jpg)
```

---
## \#5 Posted by: RedEagle Posted at: 2018-04-29T15:19:52.952Z Reads: 100

```
That would be overkill. I'm more concerned about _how_ you're going to fit such a large battery in your board.
```

---
## \#6 Posted by: dg798 Posted at: 2018-04-29T15:24:11.742Z Reads: 99

```
If u are wiring them in parallel then u theoretically could but if series then that would be way too much voltage for the esc to handle
```

---
## \#7 Posted by: Adelgaard Posted at: 2018-04-29T16:21:05.997Z Reads: 90

```
I know it sounds overkill - But trust me, the 11Ah battery is drained in no time.
It's an electric mountainboard / offroad, and I use it for riding in the forrest and on the beach. Due to sand and uneven terrain, the board has to push so much more. 

Right now i'm only getting about 5-8km per charge, and then it has to be charged for 4 hours.

The board sould have plenty of space for mounting more batteries (40cm):
![30785165_10156830010038274_216572904_n|666x500](upload://dschGFtf7AeuTvSddlcJIzU1RDw.jpg)

The 3-way wire from ebay is called "Parallel cable" - does that mean that it's as simple as connecting all 3 batteries (the 2 new + the one already installed) to the 3-way XT60 cable and the board-controller - or do I risk destroying the battery or the board by doing that?
```

---
## \#8 Posted by: RedEagle Posted at: 2018-04-29T16:31:56.042Z Reads: 85

```
All three batteries have to be the same type, voltage and capacity.
You will risk damaging more than the battery otherwise.
```

---
## \#9 Posted by: Adelgaard Posted at: 2018-04-29T17:31:47.928Z Reads: 76

```
Ah okay, I see!
So would need 2x of these: https://www.alibaba.com/product-detail/36v-11ah-lithium-ion-ebike-battery_60705602209.html?spm=a2700.7724838.2017115.1.70781630brqLGs.
Since it has 11ah I don't know where to see om many Volts it's running - I guess 36v?
![Manual|375x500](upload://kHYK9KX6voPZnwXpo04Ct8hrp4T.jpg)
Does the battery have to be Samsung as well?

And then it's just hooking it up with the cable from ebay, making a mount and then it should be good to go?
```

---
## \#10 Posted by: RedEagle Posted at: 2018-04-29T17:36:14.099Z Reads: 73

```
Those cells are very low spec. 3a discharge on 1p (so 15a discharge on 5p). I strongly recommend getting a better battery. Samsung 30q is the standard here.
```

---
## \#11 Posted by: rok Posted at: 2018-04-29T17:58:22.900Z Reads: 72

```
You source for these batteries is nkon.nl
```

---
## \#12 Posted by: Adelgaard Posted at: 2018-04-30T10:45:11.708Z Reads: 59

```
The board itself is relatively cheep, so I would prefer to buy some cheap batteries, and the change them out later.

Is it simple as this: 
![batskates|497x500](upload://jfb4rQ2ZYUxhdrQfRCWSN3MAhjP.jpg)

(I know the picture is a bid confusing to look at - but its the board controller --> to the 3-way parallel cable --> to the 3 batteries)
```

---
## \#13 Posted by: pat.speed Posted at: 2018-04-30T11:20:54.331Z Reads: 54

```
Essentially that would work as long as every battery is the same, and I mean almost identical. If connected like that each battery must also have its own bms to protect the cells. The charge port must also be connected to each battery or to the main lead going to each battery
```

---
## \#14 Posted by: Adelgaard Posted at: 2018-05-01T07:41:18.844Z Reads: 45

```
Great! And when you say that they almost had to be identical, you mean both have to be 36v 11ah and what more?

Is a BMS really necessary? I have seen some videos saying it can be a good idea to use, but none says it's a must have.
```

---
## \#15 Posted by: pat.speed Posted at: 2018-05-01T07:45:59.943Z Reads: 45

```
Yes a bms is a must have, if there isn’t one the cells can get out of balance and catch fire due to over charge or over discharge. 

As for the identical batteries you want them to have the same voltage, amps and similar discharge otherwise will drain slightly quicker than the others (why you need a bms). It should basically be the same cells used in each battery
```

---

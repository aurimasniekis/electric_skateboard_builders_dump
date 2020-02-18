# Cells have become unbalanced?

### Replies: 24 Views: 2263

## \#1 Posted by: michaelcpg Posted at: 2016-08-15T21:18:01.555Z Reads: 150

```
This morning I went to plug my charger into my board for a bit before the ride to work and at the point where the battery was showing that it was around 90%, the charger light turned green and the fan turned off as though the board was fully charged.
This had happened to me once in the past after I had ridden over some particularly nasty bumps which had ended up causing several of the fuse wires on my cells to snap due to the fact that my battery wasn't particularly well secured at the time. I pulled the battery out and checked over the fuses wires but there didn't look to be any issues.
Should mention that I've got a 10s4p LG HE4 pack with a BMS and laptop style fast charger. 
I tested the voltage on each 4p pack and found that they were all sitting at around 4.02 - 4.03 volts except for the 4p pack second closest to the battery's positive terminal which was sitting at 4.19 - 4.2 volts so this is likely why the charger stopped running at this stage. Last time I tested the pack, the cells were all pretty much balanced so I'm not sure what would cause a single 4p pack to become so unbalanced.

Is this something I should be concerned about? Is there an easy way to rebalance the cells without pulling the battery apart to charge each cell separately? My understanding is that the BMS only balances the cells at the end of a charge so I'm wondering if plugging the charger back in and leaving it for a while will get the BMS to balance the cells?
```

---
## \#2 Posted by: anorak234 Posted at: 2016-08-15T21:26:26.722Z Reads: 144

```
I've had this problem before with 2x 3s lipo batteries and was able to fix it. First turn off the time limit on the charger. Next, you need to discharge the lowest cell down to around 3.7 (at this point they may still be unbalanced). Finally, charge at a rate of 0.5A or less. It will take around 12 hours, but it worked very well for me. Each cell was within 0.05 volts of each other when I finished.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-08-15T21:36:47.616Z Reads: 135

```
My charger doesn't have anything settings you can change on it unfortunately. Would you mind explaining what the point of discharging the cells down to 3.7V is? I would've thought it'd just be a matter of discharging the 4.2V cell down the the same voltage as the others or vice versa
```

---
## \#4 Posted by: anorak234 Posted at: 2016-08-15T21:46:18.497Z Reads: 124

```
I decided to discharge because although balancing happens at the end, a full length charge will give unbalanced cells more time to catch up.
```

---
## \#5 Posted by: sl33py Posted at: 2016-08-15T21:49:53.353Z Reads: 121

```
What's your setup?  Which charger?  

Sounds like a good way to get them re-balanced.
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-08-15T21:53:33.807Z Reads: 117

```
10S4P LG HE4 18650 pack, 50A BMS and a laptop style fast charger. It was originally one of the original space cells which I later upgraded from a 3p to 4p pack. Other than that, I'm using a single VESC and Enertion 6374 motor.
```

---
## \#7 Posted by: anorak234 Posted at: 2016-08-15T21:53:35.997Z Reads: 114

```
2x 3s lipos in series. I use the IMAX B6
```

---
## \#8 Posted by: michaelcpg Posted at: 2016-08-15T21:55:44.325Z Reads: 115

```
Ah makes sense, would there be any issues discharging the pack by going for a ride or would that be a bad idea with such a difference in voltage between the cells? Not really sure how I'd otherwise discharge them.
```

---
## \#9 Posted by: anorak234 Posted at: 2016-08-15T22:07:15.223Z Reads: 108

```
I don't see how that could cause problems, just make sure you don't discharge them too much
```

---
## \#10 Posted by: michaelcpg Posted at: 2016-08-15T22:18:15.116Z Reads: 104

```
Hmm ok thanks. Any idea what would've caused this in the first place?
```

---
## \#11 Posted by: anorak234 Posted at: 2016-08-15T22:22:06.547Z Reads: 98

```
The damage to mine started with a series charging accident (incorrect wiring with the cell leads), I managed to fry one battery and on the other battery it left the 3rd cell slightly damaged. No puffiness so I decided to keep using it. Next I tried parallel charging, but the damaged cell sent false readings and so the 3rd cell on my new battery became altered. By the time I found a solution to fix the problem, the 3rd cell on both batteries was 0.7 below the other two. No more parallel charging for me. Anyways, this process rebalanced both of my batteries successfully and I've had no problems since.
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-08-16T07:50:52.054Z Reads: 80

```
I took the board for a ride tonight. The 4p pack that had a higher voltage than the rest now has a lower voltage (3.69V) than the rest of the 4p packs (3.75V), not sure if that's to be expected?
Obviously the cells are a lot closer now though which is good. 

I'm going to give the battery a full charge and let the BMS balance the cells at the end. Something I've admittedly never done before as so far it hasn't been necessary, I usually just charge the battery to around 90%.
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-08-16T08:36:17.904Z Reads: 77

```
So my charger just turned off when the battery got up to around 90% again. I'm guessing that the same 4p pack are going to be sitting on a higher voltage than the others again but I haven't had time to take the battery out and check. Any idea why this might be happening?
```

---
## \#14 Posted by: michaelcpg Posted at: 2016-08-16T09:29:41.039Z Reads: 75

```
Ugh so on closer inspection it looks as though a couple of fuse wires had broken again, couldn't even tell till I applied a small amount of force on each wire... 
Looks like I'm going to have to pull the battery apart and come up with a better design as it just doesn't seem to be able to handle some of the more nasty vibrations on really rough roads.
```

---
## \#15 Posted by: lox897 Posted at: 2016-08-16T09:46:56.861Z Reads: 71

```
Fuse wires? Do you mean balance wires?
```

---
## \#16 Posted by: michaelcpg Posted at: 2016-08-16T10:07:01.712Z Reads: 67

```
Nah Tesla style fuse wires
```

---
## \#17 Posted by: lox897 Posted at: 2016-08-16T10:09:01.303Z Reads: 67

```
Oh right. I see what you mean now. Sorry, my bad.
```

---
## \#18 Posted by: metos Posted at: 2016-08-16T11:01:02.533Z Reads: 64

```
Anorak > you can discharge only one cell in a 3s lipo pack with an Imax B6 ?
```

---
## \#19 Posted by: mason Posted at: 2016-08-16T12:04:29.507Z Reads: 59

```
You said you modded a space cell to 4p? If so, what cells did you add?
```

---
## \#20 Posted by: michaelcpg Posted at: 2016-08-16T12:16:09.282Z Reads: 59

```
Same cells, LG HE4. I believe some space cells use Samsung 25R's instead though
```

---
## \#21 Posted by: mason Posted at: 2016-08-16T12:16:31.469Z Reads: 56

```
That could be the issue.
```

---
## \#22 Posted by: michaelcpg Posted at: 2016-08-16T12:17:05.057Z Reads: 56

```
Why would you think that?
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-08-16T12:22:24.932Z Reads: 55

```
Maybe they have different resistance? (The lower the resistance the more output you get and that will drain the battery more)

I can think that your old batteries got a high resistance over the time and the new batteries have a low resistance. The new batteries will drain faster and the pack gets unbalanced.

I am just speculate. Would be nice if somebody could verify my words. :)
```

---
## \#24 Posted by: michaelcpg Posted at: 2016-08-16T12:35:59.349Z Reads: 53

```
When I added the extra cells, I added a new one to each 3p pack so this sorta thing shouldn't really be an issue. As I mentioned though, the issue turned out to be a result of a couple of the fuse wires breaking :p
```

---

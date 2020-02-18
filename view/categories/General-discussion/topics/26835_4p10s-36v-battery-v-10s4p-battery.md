# 4P10S 36V Battery V 10S4P Battery

### Replies: 22 Views: 2381

## \#1 Posted by: Donkeyhotay Posted at: 2017-07-05T11:43:23.284Z Reads: 272

```
Ok here is the problem , I have decided to make my own Batteries out of 18650 cells ( old laptop batteries) totally free so it cuts the cost down on my build. Anyway I am looking at configurations people are using and notice a lot of you are using the 10s Batteries in various Series (36V x whatever) , Im asking if 4P x 10s is better ( 4cells in Parallel x 10S ) . Now the 10s is lots of series batteries put in parallel to make the watt hours up , is easily increased in size but has the problem of balance charging with 10s BMS costing a lot. 

A 4P10S makes the 36v but is only able to be increased by welding in more batteries in parrallel and extra wiring ect. But has the advantage of only using one BMS. 

Whats your thoughts on this.
```

---
## \#2 Posted by: L3chef Posted at: 2017-07-05T11:48:56.408Z Reads: 270

```
4p10s and 10s4p  are the same setup..?
```

---
## \#4 Posted by: karma Posted at: 2017-07-05T11:55:44.767Z Reads: 259

```
You don't want more than one bms! So the way to go is connect 4 cells in parallel and then connect 10 of those groups with balancing wires in between is series connection. Doesn't matter which way 
 (4P X 10 or 10S *4 in) you connect them, they will still end up with the same amount of Wh.
```

---
## \#5 Posted by: TranxFu Posted at: 2017-07-05T12:24:21.898Z Reads: 248

```
Its the same thing you are doing. No matter how you turn around the term "10s 4p" :wink:

I'd not recommend you going for old laptop batteries unless you know that all of them are of the same type and you know their specific data. Make sure they can be used for our purposes. Most / generally all of them are not suited for using on an eBoard.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-07-05T16:43:41.272Z Reads: 223

```
you want to create your P pack first, then string them up in series.  this way each P pack acts as a cell and be balanced by the bms / balance charger.

not sure if anyone's doing a series pack then stringing them up in parallel.  that'd require multiple bms, how silly.

i also second @TranxFu, not only are old laptop cells likely not suitable for esk8s (low continous discharge), but their capacity will differ from one cell to another.  meaning, if you're discharging quickly, one may go below threshold while others are above.  this will lead to all kind of problems, like dead cells in a parallel pack, internal shorts, etc.

this is a common configuration:

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/7/e/7e43c7258f8629d04064bfdf78f80e5644dbd437.png" />
```

---
## \#7 Posted by: rpn314 Posted at: 2017-07-05T16:52:04.576Z Reads: 199

```
The other difficulty with using laptop batteries is that you also need to try and match their individual characteristics as much as possible too. Used cells, especially those that weren't used in the same device together (even though they may be the same cell model), often develop different internal resistances, different cycle counts, and different capacities. Since we push our cells to the edge of what they can handle, having those be as nearly identical as possible is best. If not, then you're likely to have a weaker cell get drained or charged past what it can really handle and then.... :boom:
```

---
## \#8 Posted by: Donkeyhotay Posted at: 2017-07-05T19:48:07.241Z Reads: 177

```
Thanks Thisguyhere. Exactly what i was doing.
 As to the cells they are all processed ( charged to full , voltage over time drop check, and then capacity checked ) and free so don't care to much about under voltage and charging with a BMS will help with the different size packs.

As to the discharging of lion cells on Eboards the load is over 40 cells , so say 30 amps continuous that is riding around, that is .75 amps per cell , the cells can easily handle that. Peaks of sudden take off's ect can be handled with a Capacitor , which i happen to have a 1 farad on my desk at the moment from when i took a microwave apart to make my spot welder for the batteries.  

Only down bit of using the old 18650's is size to Watt hours i only get around 300 Watt hours but its free ( shrugs).
```

---
## \#9 Posted by: rpn314 Posted at: 2017-07-06T19:12:45.947Z Reads: 137

```
[quote="Donkeyhotay, post:8, topic:26835, full:true"]
As to the discharging of lion cells on Eboards the load is over 40 cells , so say 30 amps continuous that is riding around, that is .75 amps per cell , the cells can easily handle that
[/quote]

Not to burst your bubble, but unless you're doing a 1s40p pack, you're not going to get 0.75 amps/cell. At 10s4p, 30 amp discharge means around 7.5 amps each. You can only divide the discharge current by the number of parallel cells (not series). Unless you meant to write 7.5, in which case disregard me :slight_smile:
```

---
## \#10 Posted by: Donkeyhotay Posted at: 2017-07-06T22:30:48.013Z Reads: 120

```
are you sure about that, I think you mean it will be 7.5 amps per group of cells , which has 10 cells in it. Each cell contributes .75 amps to make up the 7.5 amps per group.  I'm pretty sure how this works. If that was the case everyone with a 10s1p would be putting out huge amps per cell..... ? . 

Will Google it but i'm pretty sure it will be ok.
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-06T22:34:25.776Z Reads: 118

```
You can only add discharge potential of parallel cells, not series cells. If you're doing 30 continuous in 4P thats 7.5 amps per cell. Esk8 can easily go much higher than 30 continous, however.
```

---
## \#12 Posted by: Donkeyhotay Posted at: 2017-07-06T22:36:50.897Z Reads: 118

```
crap.... so how is Inertion doing it with their cells ? , which is what i modelled my battery off?
```

---
## \#13 Posted by: Jinra Posted at: 2017-07-06T22:38:48.605Z Reads: 116

```
Well they're not using laptop cells for one. They (as well as a bunch of builders on here) use high discharge 18650 cells capable of 20+ amp discharge per cell.
```

---
## \#14 Posted by: Donkeyhotay Posted at: 2017-07-06T22:41:38.173Z Reads: 116

```
ah bugger, will have to go and check the C rating on the cells , bugger . More work. 

OK thx guys , I really thought i had a cheap way out of the battery cost. Hopefully the cells are at least half decent.
```

---
## \#15 Posted by: Donkeyhotay Posted at: 2017-07-06T23:12:01.605Z Reads: 108

```
https://endless-sphere.com/forums/viewtopic.php?f=14&t=46756

OK now I'm confused
```

---
## \#16 Posted by: rpn314 Posted at: 2017-07-07T15:14:06.725Z Reads: 102

```
Laptop batteries are batteries. They just don't (usually) have the characteristics for skateboard builds. To make the packs small enough, we usually aim for cells that can discharge at least 10A continuous comfortably, so we'll usually aim for cells that are rate for 20A+.

Over on endless-sphere, they're usually building larger things, like electic bicycles, which have more space for larger batteries. So they may actually be doing something like a 10s10p batter, which also gives them longer range.
```

---
## \#17 Posted by: Gordo Posted at: 2019-01-16T22:03:46.024Z Reads: 29

```
If your battery is 4p, and your drawing 30 Amps, then it is 30 A / 4p = 7.5. 30 amps has to pass through each of the the 10 sets of parallel (4) cells.  The number of sets of cells in series gives you your voltage (total).  In the case of 10s you have a nominal voltage of 36 volts.  So, here is the bottom line your power available (Watt hours)  is your voltage 36 times your amp hours for a single parallel set of cells.  In this case it is 4 cells with a capacity of 2500 
(2.5 amp hours) each , so 10 amp hours times 36 volts = 360 Watt hours.
```

---
## \#18 Posted by: J0ker3366 Posted at: 2019-01-16T22:06:46.642Z Reads: 25

```
Pay attention to your dates lol. You just revieve a 2yr old thread lol
```

---
## \#19 Posted by: AlanZhou Posted at: 2019-01-16T22:08:20.743Z Reads: 26

```
Kinda annoyed this thread got resuscitated
```

---
## \#20 Posted by: J0ker3366 Posted at: 2019-01-16T22:10:49.683Z Reads: 24

```
Lmao I feel ya bruv! The nerve of people lol. 

With that said though, I'm going to swap my 8s3p out for a 3p8s. Maybe I can get some more speed if I paint the battery red lol
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-01-16T22:13:38.454Z Reads: 24

```
[quote="J0ker3366, post:20, topic:26835"]
With that said though, I’m going to swap my 8s3p out for a 3p8s. Maybe I can get some more speed if I paint the battery red lol
[/quote]

My day has been abominatied😫
```

---
## \#22 Posted by: AlanZhou Posted at: 2019-01-16T22:16:14.767Z Reads: 22

```
Since this thread is old anyways😈

@moderators1

Shut this madness down, lock it up.
```

---
## \#23 Posted by: Itsmedant Posted at: 2019-01-16T23:03:53.455Z Reads: 21

```
Maybe do a 8s X 3p battery instead. I've heard it has all the torque.


Someone was board and digging through the forum drunk.
```

---

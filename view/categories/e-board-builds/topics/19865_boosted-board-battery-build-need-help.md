# Boosted board battery build. Need help

### Replies: 18 Views: 4435

## \#1 Posted by: ejbares Posted at: 2017-03-28T21:51:13.995Z Reads: 417

```
Hi everyone :) so I'm currently looking at a broken v1 dual+ boosted board that someone is selling. The only thing that is wrong with it is that the battery went bad so the guy took it out. He still has the battery encloser so I thankfully won't have to necessarily worry about that. My question is if it is possible to build a battery so it will work with it. I have never build a battery before but have read quite a bit and understand the basics of it. I'm not sure what battery a boosted board has or the exact specs of it but I would assume maybe a 10S2P? (correct me if I'm wrong). Is there any reason why I wouldn't be able to just hook the red to red and black to black of the battery to the board and have it work? Also does anyone have any suggestions on the cells, bms, and other parts I will need or is there anyone that sells prebuild packs that aren't super expensive? Thank you in advance :)
```

---
## \#2 Posted by: sl33py Posted at: 2017-03-28T21:55:26.468Z Reads: 408

```
I would try to keep the same BMS and charger it shipped with, then simply swap in new cells in the same configuration.  If you look at the extended battery threads for the v1 i'm 99% positive folks identify the stock cells.  I'll do a quick search to see if i can locate that info for you, but you should be able to find it easily.

Don't guess - get the same setup exactly #s#p.  You don't want to mess with a different voltage and fry other components, or starve it of amps.
```

---
## \#3 Posted by: ejbares Posted at: 2017-03-28T21:58:56.448Z Reads: 392

```
Unfortunately I think the battery and bms were trashed :( so I would need to start from scratch
```

---
## \#4 Posted by: saul Posted at: 2017-03-28T22:24:36.744Z Reads: 369

```
the v1 uses 12s1p LiFePO4 cells from a123. but the battery hacks usually use 10s2p 18650.

without the stock bms you loose most of the features like battery meter and I think even the power switch is on there too. 

the deck is worth 300, drive line about 120, if its less than 500 it might be an ok deal but not easy and it won't be as good as new at all. even at that price you end up spending more than a custom.
```

---
## \#5 Posted by: Pantologist Posted at: 2017-03-28T22:52:54.233Z Reads: 353

```
It will not work without the Boosted BMS. There has to be communication between the ESC and BMS. There are data cables between the Battery and ESC. 

Don't buy it for move than $300. 

Also Boosted will probably replace it for you for like $650.
```

---
## \#6 Posted by: ejbares Posted at: 2017-03-29T00:09:05.661Z Reads: 324

```
Yeah. Its priced at $655 or you can make an offer. @Pantologist So it won't work at all unless it has the boosted bms? So ultimately there is easy way of fixing it and it's just not worth it? I'm not really interested in the battery level feature of anything.
```

---
## \#7 Posted by: Pantologist Posted at: 2017-03-29T00:27:21.985Z Reads: 318

```
I didn't work with Boosted on the firmware but from what they've done with the Bluetooth code and the V2s had error codes for even abnormal disconnections in the battery to the ESC connection, you can be sure they will only allow the board to run with a functioning, Boosted programmed BMS sending calculations and data to the ESC. 

It is worth it only for parts. 

Maybe someone will buy a deck for $120, Wheels $50, rear truck and ESC are worth a lot, but not many Boosted owners are in need or want to replace their ESC or motors. 

The best situation would be, build another battery, fit it inside there and buy a pair of VESCs to get the board working again. Sell the old ESC and rep grow the remote and add a Bluetooth chip to the Vescs.
```

---
## \#8 Posted by: ejbares Posted at: 2017-03-29T00:35:29.140Z Reads: 290

```
Ok thank you for your insight :)
```

---
## \#9 Posted by: Pantologist Posted at: 2017-03-30T00:55:51.979Z Reads: 263

```
Did you end up getting it?
```

---
## \#10 Posted by: ejbares Posted at: 2017-03-30T01:04:35.611Z Reads: 254

```
Nah. Unless I was certain that there wasn't a necessary connection between the bms and the esc then I wasn't going to bother with it. If anything maybe this info will help someone that has the same idea because I could find anything on it.
```

---
## \#11 Posted by: Pantologist Posted at: 2017-04-06T00:20:12.840Z Reads: 221

```
Here's another one. Boosted Board owners don't seem to know much about how Lithium batteries work :joy:
```

---
## \#12 Posted by: BoostedBuilder Posted at: 2017-06-19T16:18:28.196Z Reads: 199

```
Hey guys,

Does anyone know the specifications of the boosted battery and the BMS they use? Like what's the peak charge and discharge current of the system? Does the BMS do anything else other then protect from over charge and discharge? And at what V and Amps does the charger charge the battery pack?

I will appreciate any answers!
```

---
## \#13 Posted by: 1930iancook Posted at: 2018-03-31T22:25:26.067Z Reads: 157

```
How much would it cost for you to ship the motors ill pay the shipping fees...
```

---
## \#14 Posted by: danieloath Posted at: 2018-04-14T04:56:08.500Z Reads: 140

```
Where are you located? I have v1 dual+ motors, trucks, mounts and ESC. I'm in Australia.
```

---
## \#15 Posted by: Vin Posted at: 2019-03-04T23:31:58.369Z Reads: 72

```
Hi,

Sorry to bump this old topic but was wondering if I could get some help please? Also if I refer to anything incorrectly please correct me.

Its interesting that you mentioned you worked with Boosted on the Boosted Board what part did you work on? Do you know how the BMS monitors the battery and is it possible to replace the battery pack with an identical pack and is there a chance I end up bricking the board in the process or a way to bypass the system? I ask this as when researching into this issue myself I came across this thread on eSk8 

https://www.electric-skateboard.builders/t/wanted-dead-boosted-board-battery-management-system-v1-preferred-but-i-would-try-v2/57828

One of the commenters mentions something about possibly bricking the BMS and I am a little cautious about this as I don't fully understand the system in place and don't want to end up bricking my board in attempts to replace the battery.

If you dont is it possible you know someone who does that worked along side you?

The reason I am asking this question is because I bought a BB-V1 and the current pack still works but just doesn't hold as much charge as it should and I would like to replace the existing power pack. I also have a company that is willing and capable of building and installing an identical pack of A123 12S pack.

Also is it possible to replace the motors by just soldering in new ones obviously making sure it has all the correct connectors and cables?
```

---
## \#16 Posted by: Vin Posted at: 2019-03-04T23:35:26.595Z Reads: 62

```
Hi,

I know its kind of late to ask but do you still have any of the parts left over?


Thanks
```

---
## \#18 Posted by: danieloath Posted at: 2019-03-05T22:17:59.180Z Reads: 51

```
Sorry, mate. Gave them away many moons ago :slight_smile:
```

---
## \#19 Posted by: Vin Posted at: 2019-03-09T17:24:50.543Z Reads: 43

```
Haha thats okay thanks for the reply
```

---

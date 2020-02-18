# Volt regulator for 24V 5000mAh batteries

### Replies: 66 Views: 1163

## \#1 Posted by: jimmaskell Posted at: 2018-05-27T18:40:11.358Z Reads: 126

```
For my electric longboard I am using 2 3s 5000mAh batteries in series. This was an okay solution because it was affordable. But my biggest problem is that my voltage keeps dropping while riding. Then I heard you could install a voltage regulator to keep the voltage constant. I was wondering if anybody has any recommendations or requirements I need to be looking out for.
```

---
## \#2 Posted by: linsus Posted at: 2018-05-27T18:57:32.032Z Reads: 114

```
Yes the voltage drops. Thats normal. a voltage regulator that withstands 40-60 amps? You'd get better experience and less losses adding another two 3s in parallell. Alot better voltage curve as well.
```

---
## \#3 Posted by: jimmaskell Posted at: 2018-05-27T19:30:38.345Z Reads: 104

```
Sounds great, but how do I connect another two 3s batteries into the circuit? Do you have some kind of special connection parts for that?
```

---
## \#4 Posted by: b264 Posted at: 2018-05-27T19:43:47.706Z Reads: 98

```
A voltage regulator will just burn off the excess power as heat and won't solve many problems without creating more.  So if you feed it 32V and it outputs 24V, and you're drawing 40A through it, then 320 Watts is being wasted -- burnt off as heat from the regulator -- which then has to be cooled with a HUGE heatsink
```

---
## \#5 Posted by: jimmaskell Posted at: 2018-05-27T20:31:46.622Z Reads: 84

```
Oh so it doesn't help with undervoltage but only with overvoltage. Sounds quite useless then.
```

---
## \#6 Posted by: b264 Posted at: 2018-05-27T20:35:30.504Z Reads: 81

```
There are also buck converters and boost converters which don't have that problem but have other problems.  None of those will handle 50A.  They will all waste power as heat.
```

---
## \#7 Posted by: jimmaskell Posted at: 2018-05-27T21:02:57.962Z Reads: 75

```
Then that isn't a good solution. Do you maybe have any info about what @linsus said about adding another two 3s batteries in parallel?
```

---
## \#8 Posted by: linsus Posted at: 2018-05-27T21:23:54.432Z Reads: 70

```
yeah, you'll get less voltage sag and larger capacity, if your cells are bit old i dont recommend mixing tho. They might discharge in an uneven rate. Sure theres many threads you can find to learn more about batteries
```

---
## \#9 Posted by: b264 Posted at: 2018-05-27T21:34:51.564Z Reads: 62

```
Don't mix old and new cells in series.  If you mix them in parallel it's fine.
```

---
## \#10 Posted by: jimmaskell Posted at: 2018-05-27T21:47:44.269Z Reads: 59

```
@linsus @b264 Okay great! Is there some kind of connection part to make like a 5.5mm bullet connector turn into two?
```

---
## \#11 Posted by: b264 Posted at: 2018-05-27T22:06:05.880Z Reads: 56

```
Buy some male and female 5.5mm bullet connectors and some 10AWG super-stranded silicone-insulated tinned wire

Make your own adaptors with a soldering iron and heatshrink and kapton tape
```

---
## \#12 Posted by: petter Posted at: 2018-05-27T22:10:55.063Z Reads: 53

```
There are also sepic regulators that do boost or Buck depending on in vs out voltage. And there are for sure ones that could be used for these high currents.. They probably cost more than a whole board though.
```

---
## \#13 Posted by: jimmaskell Posted at: 2018-05-28T11:48:54.697Z Reads: 50

```
@b264 @linsus  Could this work? And could I also just use regular thick copper wire?
![image|690x388](upload://m82QvjJztw7GMCyqkjyoLwJ7aVw.jpg)
```

---
## \#14 Posted by: linsus Posted at: 2018-05-28T11:53:34.274Z Reads: 49

```
[quote="b264, post:9, topic:56953"]
If you mix them in parallel it’s fine.
[/quote]

Not really. But yes, its the better of the mixes.
```

---
## \#15 Posted by: jimmaskell Posted at: 2018-05-28T11:57:36.009Z Reads: 48

```
@b264 @linsus Oh and I was wondering how I could charge these two extra batteries, because it technically is still a 6s battery, only with more capacity. Right now I have a 6s 12A BMS to charge my two 3s batteries.
```

---
## \#16 Posted by: linsus Posted at: 2018-05-28T12:04:55.635Z Reads: 46

```
if you use a BMS then the BMS will treat the parallell cells as one cell when charging. It will take longer to charge then your previous setup but it'll work. 
Just make sure you buy the same battery when expanding your pack and it should be fine. 

I sudgest doing a few trial runs where you can dissconnect the cells individually to see voltagelevels after a discharge cycle. Then connect the batteries as they're s'posed to be during charging and see if they charge evenly. If they differ alot in internal resistance you might have some missmatch.
```

---
## \#17 Posted by: jimmaskell Posted at: 2018-05-28T12:13:45.503Z Reads: 44

```
@linsus Okay great, but if the BMS treats two cells like one, will the cells charge balanced? And how do I connect the balance wires of the two extra batteries to the BMS? Oh and can you tell if my picture could work, to make a parallel connection?
```

---
## \#18 Posted by: linsus Posted at: 2018-05-28T12:15:22.374Z Reads: 45

```
Make a complete wiring schematic and come back to us :) safest way. 
Essentially, the wires to the BMS should be the same amount. Only more cables on the battery side to connect the parallell poles. (unless you plan to go higher in voltage)
```

---
## \#19 Posted by: jimmaskell Posted at: 2018-05-28T13:14:15.233Z Reads: 45

```
@linsus @b264 This is the wiring scheme for as much as I know now. I didn't know what to do with the balance wires of the batteries, so that's why I left the BMS and the balance wires out.
![image|690x387](upload://zwUiWWJjkLZMSu4liud6v3FIq7I.jpg)
```

---
## \#20 Posted by: linsus Posted at: 2018-05-28T13:21:37.583Z Reads: 41

```
![wire|690x392](upload://hx2FpTXqoa8v6BLYXWv2adObJuC.PNG)
```

---
## \#21 Posted by: jimmaskell Posted at: 2018-05-28T14:03:40.278Z Reads: 40

```
@linsus I don't really understand the bridges, between the batteries. To charge the batteries I have balance wires. This is original wiring diagram for my BMS. ![image|690x388](upload://lVqwGgPYU18i8Ety4LNMuneaJ7p.jpg)
```

---
## \#22 Posted by: linsus Posted at: 2018-05-28T14:08:07.670Z Reads: 37

```
The wiring is the same, either you charge them as two separate packs, 6S1P + 6S1P (separate balance wires). Or you parallell wire pretty much everything so they "share" balance leads. Guessing you want the later since you dont want to open it up everytime you charge.
```

---
## \#23 Posted by: jimmaskell Posted at: 2018-05-28T14:23:22.333Z Reads: 35

```
@linsus Okay great, but will the batteries charge balanced then? And do you approve of the construction I have to make a parallel connection?
```

---
## \#24 Posted by: linsus Posted at: 2018-05-28T14:32:41.366Z Reads: 35

```
Yes, just make sure they share the series terminal on the "3S" line in prev. picture.
Dont know what BMS you have but the chargetime will be minimum doubled with twice the capacity. 

Google around abit on how to build your own lithium packs and you can get a better understanding of how and why things are connected.Youtube is a great source as well as this forum where sevral buildthreads exist.

Can also recommend battery university
```

---
## \#25 Posted by: jimmaskell Posted at: 2018-05-28T14:47:42.222Z Reads: 32

```
@linsus okay great, but the way I connected the batteries was also two serie packs, which are then connected in parallel, right? What is exactly wrong with my connection scheme?
```

---
## \#26 Posted by: linsus Posted at: 2018-05-28T14:52:25.580Z Reads: 29

```
It will probably work with the wiring from your first picture. But you'll have one extra lead to your BMS since they dont share the 3S terminal. Since they'll physically be two separate packs. 
Parallell configuration also helps the cells to balance themselves, meaning they try to maintain the same voltage level when connected in parallell. The stronger one will push voltage into the weaker one simply put.
```

---
## \#27 Posted by: jimmaskell Posted at: 2018-05-28T15:22:58.390Z Reads: 26

```
@linsus won't that overcharge the first battery and undercharge the other battery ruining them in the proces?
```

---
## \#28 Posted by: b264 Posted at: 2018-05-28T16:01:06.763Z Reads: 25

```
[quote="linsus, post:26, topic:56953"]
It will probably work with the wiring from your first picture.
[/quote]

I think it would work anyway because they would end up being connected by the balance wires.  But it's better to have a higher-current connection there
```

---
## \#29 Posted by: linsus Posted at: 2018-05-28T16:41:54.081Z Reads: 24

```
yeah, kind of defeats its purpose to connect them in parallell every 3d cell I guess. My mindset is always in li-on 18650..
```

---
## \#30 Posted by: linsus Posted at: 2018-05-28T16:44:50.573Z Reads: 27

```
Since its segments of 3S I guess it's not that important since the other cells inbetween will still be isolated. Might as well keep them separate as in your picture. The voltage test becomes even more cruicial now tho since they dont balance of eachother. Try to do half a discharge run and see what voltages you have on each.
```

---
## \#31 Posted by: jimmaskell Posted at: 2018-05-28T21:40:10.143Z Reads: 27

```
@linsus @b264 So this would basically be the wiring? Or am I missing wires from the other batteries?
  ![image|690x388](upload://90XmM4uduQsrurcWU6iyt82Bw0Y.jpg)
```

---
## \#32 Posted by: Deodand Posted at: 2018-05-28T22:16:02.418Z Reads: 26

```
You need to join all the balance wires from parallel cells together or havee two seperate bms/chargers.  Remember to only add these connections after a full balance charge, if the packs have significantly different voltage when you parallel them it can be very dangerous.
```

---
## \#33 Posted by: ElectricCoast Posted at: 2018-05-28T23:17:44.540Z Reads: 26

```
Only dangerous if you try to charge them before they all balance with each other.  Best safe practice is to plug all the batteries together including balance leads and then wait a couple of hours to let them all balance out prior to charging.
```

---
## \#34 Posted by: Deodand Posted at: 2018-05-28T23:46:01.436Z Reads: 23

```
If one cell is at 4.2V and the other 3.2V you will probably exceed the max charging amps of the 3.2v cell and most likely start a fire.
```

---
## \#35 Posted by: b264 Posted at: 2018-05-28T23:54:02.558Z Reads: 23

```
No; B3 needs to be connected to both batteries.
```

---
## \#36 Posted by: ElectricCoast Posted at: 2018-05-29T00:00:38.955Z Reads: 23

```
You should never run your battery down to 3.2v lipo or li-ion.  The max percentage that you should run a battery down is about 80% of the capacity.  I found that stopping at 3.50-3.60v per cell is a rough guesstimate on the amount of battery used.  It also helps with battery longevity by not draining your batteries that low.
```

---
## \#37 Posted by: Deodand Posted at: 2018-05-29T00:06:22.037Z Reads: 27

```
Not sure where that information is coming from? Pretty much any device you use lets the battery run down lower than 3.6v. 3.7v is the nominal cell voltage 3.6 is far from dead.
```

---
## \#38 Posted by: ElectricCoast Posted at: 2018-05-29T00:33:12.077Z Reads: 26

```
I have charged a couple thousand batteries over the past few years flying, racing drones.  I use and charge batteries on parallel charging boards on a daily basis.  I always put my batteries on a parallel charging board and let them sit there for a while prior to beginning the charge in order to give all he batteries the chance to balance out.  By doing so I have never had a lipo fire because I utilize go battery management.  The point i was trying to make is by hooking up the batteries together as well as the balance leads that takes the place of the parallel charging board.   I know 3.7volts is nominal I have found over the past years and charging and flying 20-30 packs a day (when I am home).  Running your batteries in particular lipo down past 3.5v on a regular basis will shorten the life span of your battery.  I'll digress because I don't want to ruffle any feathers.  I'm just here trying to give some insight.
```

---
## \#39 Posted by: Deodand Posted at: 2018-05-29T00:40:02.101Z Reads: 26

```
My point is just for an inexperienced user, if you had a fully charged lipo and a fully discharged lipo according to regular values (commonly listed at 2.8-3v industry standard) and connected the two, bad things might happen. It sounds like thats not something you are ever doing. 

A few tenths of a volt is totally fine. Think about with your current limiting charger, it doesn't hit the pack with 4.2v right away most often. If it did battery damage might ensue, and no one wants damaged batteries.
```

---
## \#40 Posted by: b264 Posted at: 2018-05-29T00:42:47.968Z Reads: 24

```
[quote="ElectricCoast, post:36, topic:56953"]
I found that stopping at 3.50-3.60v per cell
[/quote]

Without specifying whether you're referring to li-ion or lipo, this could be slightly misleading.  These look like lipo numbers.
```

---
## \#41 Posted by: ElectricCoast Posted at: 2018-05-29T01:04:29.886Z Reads: 25

```
I made the assumption that he was using a lipo due to the 2 3s 5000mah batteries in series reference but you're both right.  It was an assumption I should have not made.  On the the other hand I monitor my battery mah charged and I have found that my example of 3.5-3.6v worked best and would account for using approximately 80% of the battery capacity thus causing my batteries to get get hundreds of charges out of them before the batteries having issues and having to remove them from service.  Like I said I wasn't trying to ruffle any feathers and I hope I didn't.
```

---
## \#42 Posted by: Deodand Posted at: 2018-05-29T01:13:34.407Z Reads: 24

```
Nope! No ruffling here, just want to make sure new people reading the forum follow safe practices with their batteries :slight_smile:
```

---
## \#43 Posted by: b264 Posted at: 2018-05-29T01:25:09.041Z Reads: 23

```
Yes, me too.  I want to make sure if someone finds this a long time from now it's clear that those numbers are for certain cell chemistries only.

No :fire:
```

---
## \#44 Posted by: jimmaskell Posted at: 2018-05-29T09:47:04.833Z Reads: 22

```
@b264 Could you make a electric scheme? Because right now it isn't very clear to me. The way I drew the balance wires was for my original 6s BMS with two LiPo's. My biggest question is mostly. Do I need to connect any balance wires of the other two batteries to the BMS? It would be very helpful if you could draw an electric scheme.
```

---
## \#45 Posted by: linsus Posted at: 2018-05-29T10:50:42.969Z Reads: 22

```
I can draw something for you after work if you like. The batteries need to share balance leads to the BMS. So there should be a connection point for the two leads from your 2packs of 0-3S(2 balance groups -> into one -> to BMS). And same for 3S-6S balance wires.
```

---
## \#46 Posted by: b264 Posted at: 2018-05-29T14:25:19.087Z Reads: 20

```
There should be a whole thread of electric schematics.
```

---
## \#47 Posted by: jimmaskell Posted at: 2018-05-29T15:00:51.807Z Reads: 19

```
@linsus That would be great. I find it very hard to communicate electric schemes through words and so. Most of the time when I try to draw an electric scheme based of words I'm incorrect.
```

---
## \#48 Posted by: jimmaskell Posted at: 2018-05-29T15:01:24.231Z Reads: 18

```
@b264 What exactly do you mean by that?
```

---
## \#49 Posted by: jimmaskell Posted at: 2018-05-29T15:04:37.922Z Reads: 19

```
@linsus @b264 By the way, these are the parallel pieces I put together. Only need to buy some heat shrink from the store.
![image|281x500](upload://2JC7bawjZnc5Io8rocXJRfSFOPt.jpg)
```

---
## \#50 Posted by: b264 Posted at: 2018-05-29T15:07:23.056Z Reads: 18

```
I mean in this forum the is one entire thread full of schematics already.  You can look around
```

---
## \#51 Posted by: b264 Posted at: 2018-05-29T15:08:12.917Z Reads: 19

```
Those are cold solder joints.  Make sure the wire and the connector are both hot enough to melt the solder and you're not dripping it on like lava.

The connection that I can see on the black one looks good.

Don't strip the wire more than you need to.
```

---
## \#52 Posted by: linsus Posted at: 2018-05-29T15:52:14.161Z Reads: 19

```
![bms|690x388](upload://nZ2MrsY1vnzs7isbv9Zh7sAx5cH.jpg)

Hope this makes sense to you
```

---
## \#53 Posted by: jimmaskell Posted at: 2018-05-29T16:16:26.266Z Reads: 20

```
@b264 I understand. What I do is at first I put a bit of solder on the connector and then saturate the copper wire with solder. Then I just try to fill in the hole that's left with solder. I don't know if that's the best way to do it, but it works.
```

---
## \#54 Posted by: jimmaskell Posted at: 2018-05-29T16:17:30.299Z Reads: 20

```
@linsus I only see two batteries?
```

---
## \#55 Posted by: b264 Posted at: 2018-05-29T16:37:42.610Z Reads: 19

```
It needs to get hotter.  It's not hot enough to weld the metals together.
```

---
## \#56 Posted by: linsus Posted at: 2018-05-29T16:43:05.907Z Reads: 17

```
Look again
```

---
## \#57 Posted by: jimmaskell Posted at: 2018-05-29T21:11:48.959Z Reads: 18

```
@b264 I don't have acces to a welding machine, but this can be soldered just as well right?
```

---
## \#58 Posted by: jimmaskell Posted at: 2018-05-29T21:15:18.550Z Reads: 18

```
@linsus I see it now. My only question is: why does the lower top battery need to be connected to B3 as well?
```

---
## \#59 Posted by: linsus Posted at: 2018-05-29T21:56:37.574Z Reads: 17

```
It doesnt, just showing you that its the same node
```

---
## \#60 Posted by: b264 Posted at: 2018-05-30T00:48:54.327Z Reads: 19

```
LoLz soldering is a form of welding.  I meant soldering.  Sorry :stuck_out_tongue:
```

---
## \#61 Posted by: jimmaskell Posted at: 2018-06-05T16:09:27.086Z Reads: 19

```
@linsus @b264 Hi guys, hadn't had much time to work on my electric longboard, but I just drew an electric schematic. I now linsus already drew something, but this is just to check if we're on the same level. ![image|690x387](upload://tQ8c7L69UgGkqKUtTxljNQCsP2a.jpg)
```

---
## \#62 Posted by: b264 Posted at: 2018-06-05T16:27:02.081Z Reads: 18

```
The balance wires aren't correct, and you don't ever want male connectors on a battery

B+ almost never hooks to the BMS

Also you'd need to draw fat lines and skinny lines for 22AWG and 10AWG
```

---
## \#63 Posted by: linsus Posted at: 2018-06-05T17:58:24.089Z Reads: 16

```
Just draw it up for him then, Im not near a PC atm so cant rly check his picture or do a proper sch
```

---
## \#64 Posted by: b264 Posted at: 2018-06-05T18:03:16.408Z Reads: 18

```
There are already diagrams in the diagrams thread.  If he draws it I will tell him if there are any errors.  I'm not going to spend time drawing him a diagram.  Unless he wants to pay me.  Why don't you draw it?
```

---
## \#65 Posted by: jimmaskell Posted at: 2018-07-13T14:48:29.654Z Reads: 12

```
@b264 Hey, I was wondering about the parallel pieces, because you also form a closed circuit with the parallel pieces. Do the batteries have like diodes to make sure the the circuit only goes one way?
```

---
## \#66 Posted by: b264 Posted at: 2018-07-13T16:42:27.310Z Reads: 10

```
[quote="jimmaskell, post:65, topic:56953"]
Do the batteries have like diodes to make sure the the circuit only goes one way?
[/quote]

No.

[Take a peek at this one](https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/119?u=b264)

Depends on your specific BMS though, and your setup.
```

---

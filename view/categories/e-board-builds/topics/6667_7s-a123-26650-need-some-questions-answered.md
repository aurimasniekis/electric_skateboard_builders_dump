# 7S A123 26650 - Need some questions answered!

### Replies: 28 Views: 2694

## \#1 Posted by: johnny_261 Posted at: 2016-07-27T00:08:37.875Z Reads: 146

```
Hello,

So I have some left over parts and wanted to build my own foldable longboard sort of like the Linky (I think it was called) that was on Kick Starter.

I have two 6s ESCs, two 50mm 245KV motors, and some 3s Lipos.  Anyways, I wanted to get away from Lipos, since I decided the cost savings isn't really worth the risk anymore.  I wanted to build a pack out of Lifepo4 batteries since that is what I gather is the safest to use.  Also I thought it would be good to learn how to build a pack.

For a 6s setup, I believe the only cells that fit the bill are the A123 26650 as they have a high discharge rate.  So here's my questions:

**If the nominal voltage is 3.3V which is lower than a Lipo, can I do 7S and will that still be safe for the 6s car ESC?  It comes to roughly the same voltage as a 6s lipo.  Never heard of anyone doing 7s which is why I ask!**

Also since I have two motors and two escs I thought it would nice to have dual motor.  Would I be able to get away with 6s2p? Or Maybe 6s3p?  Not exactly sure how many amps 6s draws, but I know it's quite a bit.

Lastly, I want to use a BMS for charging only (not discharging because I'm not sure there is even a ESC that could handle the amps for dual drive 6s and if there is I'm sure it costs a lot).  It looks like they do make 7s BMS so I should be okay here.

Thanks guys!
```

---
## \#2 Posted by: anorak234 Posted at: 2016-07-27T00:12:36.102Z Reads: 135

```
1) Never use more cells then your ESC is rated for
2) Link or Barajabali can help you with wiring BMS for charging only
3) I love the idea of making something like Linky, but be careful when figuring it out, Linky used an uncomfortable amount of bolts for my standards... the board itself looks kind of flimsy (Go for reliability, use whatever you can to make sure it won't fall apart)
```

---
## \#3 Posted by: johnny_261 Posted at: 2016-07-27T00:36:40.714Z Reads: 122

```
Thanks for the input. I'm just wondering though since lifepo4 cells have lower voltage than lipo, wouldn't the total voltage for 6s lipo or 7s lifepo4 be about the same?  so lifepo4 is 3.6v x 7 = 25.2 versus 4.2v x 6 = 25.2 for lipo. Just wondering if my math is wack and I'm missing something or if it's okay since I've never heard of anyone doing this before
```

---
## \#4 Posted by: anorak234 Posted at: 2016-07-27T00:43:27.242Z Reads: 115

```
Your math is not wrong at all, however ESCs work off of the amount of cells they detect and use that to determine how much power goes to the motor. If you have 7 cells on a 6s rated ESC 1 of 2 things could/will most likely happen

1) ESC fails and you get that not-so-beautiful smoke because it was drawing what it thought to be 6 cells and ended up taking extra because it didn't detect the 7th

2) it sends too much power to the motor because it thought that it was only sending 6 cells worth of energy vs 7.
 
regardless of your cell energy, an ESC will draw power depending on what it thinks the amount of cells is. It can't account for more than its rating. Its like trying to charge a 10s battery with a 9s rated BMS, it's just not programmed or made to take extra input. Not trying to shut down your idea, but its just not safe.
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-27T00:51:16.638Z Reads: 98

```
I don't see anything wrong with using a 7s LIFEPO setup on a 6s ESC. ESCs dont typically detect how many cells a battery pack has in series. It only reads voltage. 6s li-ion full charge and 7s lifepo4 is the same voltage so they should be fine running it.
```

---
## \#6 Posted by: Jinra Posted at: 2016-07-27T00:55:35.163Z Reads: 96

```
keep in mind that in a dual configuration, each esc is will be drawing half the amps
```

---
## \#7 Posted by: Pantologist Posted at: 2016-07-27T01:26:45.433Z Reads: 95

```
Nah, they don't detect each cell. They will only detect the voltage level. The ESC is going to pull the same amount of current no matter how many cells there are equaling the same voltage. 

A123 cells are rated for 70A continuous, and although you probably wont pull that much, it is nice that their discharge rate is gr8.
```

---
## \#8 Posted by: johnny_261 Posted at: 2016-07-27T01:56:01.485Z Reads: 94

```
Hmm so some conflicting reports....Given how batteries are connected to the ESC, I have a hard time imagining how it would detect the number of cells.  My thinking was that ESC detects total voltage as some of you had mentioned.  

The reason for wanting to add that extra cell is to keep Voltage up.  Since 6s lipo already draws a lot of amps, I figured 6s lifepo4 with lower voltage must draw even more.  Given that it will be dual drive I'm thinking that's even more reason to increase the voltage by that extra cell since the amp draw will be more without it.

So if I do a 6s2p, I would have 140A continuous right? Should be enough for 6s dual drive?  The range would be quite limited though, so maybe 6s3p.
```

---
## \#9 Posted by: Jinra Posted at: 2016-07-27T02:05:16.873Z Reads: 86

```
I'd recommend keeping it 7s. You'll also never draw 140A continuous, you don't have much to worry about for discharge rate. worry more about capacity and range
```

---
## \#10 Posted by: lox897 Posted at: 2016-07-27T03:05:44.418Z Reads: 81

```
I don't know where you got that info from. 7S A123 = 3.6 fully charged x 7 = 25.2 which is the exact same as lipo 6s. The hard part is finding a charger and bms because most lifepo4 charges to 3.65v and that would be too much for your 6s esc. I looked for a charger for ages that charges cells to 3.6v each. Didn't ending up finding one.
```

---
## \#11 Posted by: Jinra Posted at: 2016-07-27T03:07:31.307Z Reads: 76

```
Since s/he's using a BMS he should be fine using a standard 6s lipo/lion charger.
```

---
## \#12 Posted by: anorak234 Posted at: 2016-07-27T03:08:18.502Z Reads: 74

```
(Did some double checking) My bad on the ESC thing, same voltage with 7 cells should be fine. I do know that the ESC detects cells though, mine gives 6 rings when using 2 3s and 3 rings when using 1 3s battery.
```

---
## \#13 Posted by: Jinra Posted at: 2016-07-27T03:09:20.672Z Reads: 68

```
Are you sure it's not just detecting it by voltage? Unless you're plugging in balance wires into your ESC, there's no way for it to know how many cells you have.
```

---
## \#14 Posted by: lox897 Posted at: 2016-07-27T03:10:02.661Z Reads: 67

```
But most 6s chargers don't have a mode for A123 specifically.
```

---
## \#15 Posted by: Jinra Posted at: 2016-07-27T03:11:22.385Z Reads: 66

```
What do you mean "mode for A123", A123 is just a brand. Battery charging is pretty basic and resolves around balancing voltage with a constant current.
```

---
## \#16 Posted by: lox897 Posted at: 2016-07-27T03:13:43.512Z Reads: 67

```
A123 batteries are supposed to be charged to 3.6v. The lifepo4 mode on chargers charge to 3.65v. It will damage the cells a little bit over time and it will also be too much voltage for the esc.
```

---
## \#17 Posted by: Jinra Posted at: 2016-07-27T03:14:54.639Z Reads: 70

```
That's why I said if they're using a BMS it doesn't matter. The BMS will take care of making sure everything gets to the right voltage. You just need a source of 25.2v power which a standard 6s charger provides.

For example, this will be fine for them.

http://www.batterysupports.com/liion-lipo-252v-222v-2a-6s-wall-socket-battery-charger-ac-dc-p-135.html
```

---
## \#18 Posted by: lox897 Posted at: 2016-07-27T03:19:04.718Z Reads: 64

```
I see what you mean now. Have you tried this method?
```

---
## \#19 Posted by: lox897 Posted at: 2016-07-27T03:20:16.216Z Reads: 64

```
I thought you meant using a 7s lifepo4 bms
```

---
## \#20 Posted by: Jinra Posted at: 2016-07-27T03:21:52.636Z Reads: 66

```
Haven't tried it myself, but I'm almost positive it would work. Charger's aren't smart; they just try to bring whatever they're plugged into to the voltage it's rated for. The smart part is the BMS.

I do mean a 7s lifepo4 bms. Basically what I'm saying is a 6s lipo/li-ion laptop style charger is the same thing as a 7s lifepo4 charger.
```

---
## \#21 Posted by: lox897 Posted at: 2016-07-27T03:22:10.519Z Reads: 57

```
Wouldn't the BMS think there was only 6 cells? Also, the balance port would have a 6s connector not 7s.
```

---
## \#22 Posted by: Pantologist Posted at: 2016-07-27T03:24:54.522Z Reads: 56

```
The BMS would be made for 7S though. "7s lifepo4 bms" 

The balance port on the BMS would have a 7S connector. Jinra is talking about laptop style charging though. The BMS will take care of balancing the cells.
```

---
## \#23 Posted by: lox897 Posted at: 2016-07-27T03:27:07.295Z Reads: 59

```
So you are saying a 6s lipo/lithium ion charger + a 7S bms? I'd be interested to know if someone has tried this. Sounds good. Thanks for correcting me guys.
```

---
## \#24 Posted by: johnny_261 Posted at: 2016-07-27T17:22:35.318Z Reads: 54

```
So a BMS like this perhaps?  All though this one might be overkill since I wasn't planning on using it to discharge.
http://www.bestechpower.com/224v7spcmbmspcbforlifepo4batterypack/BMS-D138.html

And then just a normal 6s charger? It does seem harder to find 7s lifepo4 bms, so depending on how expensive they are, might not be worthwhile the hassle in the end...
```

---
## \#25 Posted by: johnny_261 Posted at: 2016-07-27T17:26:59.862Z Reads: 52

```
Actually just found this one:
http://www.batterysupports.com/24v-252v-7s-30a-7x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-258.html

Says it's applicable for 3.6V, so does that mean its good for lifepo4? How does it know to charge to 3.6V vs. 4.2V?
```

---
## \#26 Posted by: Jinra Posted at: 2016-07-27T17:41:01.855Z Reads: 55

```
First one will work, second one will not. The second one balances to 4.2 per cell which will damage your lifepo4 cells.

If you want decent energy density, and safety, why not go for Samsung 25R's? Each cell has a built in safety. I prefer li-ion cells since they're more energy dense than LIFEPO4's.
```

---
## \#27 Posted by: johnny_261 Posted at: 2016-07-27T17:58:17.992Z Reads: 56

```
Thanks I thought the second one wouldn't work.  But just out of curiosity, why does it say:

_Applicable for _
_**25.2V (3.6V * 7S) lithium battery & packs**_
_25.9V (3.7V * 7S) lithium battery & packs_
_29.4V (4.2V * 7S) lithium battery & packs_
_Lithium battery (Li-ion)_
_Prismatic Lithium Polymer battery (Li-Po)_

Would you say there is any difference in safety between Lifepo4 and Samsung 25Rs? The other reason though is because this is only 6s, not sure if the 25R's will have enough amps...
```

---
## \#28 Posted by: Jinra Posted at: 2016-07-27T18:03:57.435Z Reads: 56

```
>25.2V (3.6V * 7S) lithium battery & packs

This is nominal voltage, not full charge. If you read the description below, it says it balance charges to 4.2v per cell which is not good for lifepo's.

Series doesn't have anything to do with discharge rate. If you need the amps you add more cells in parallel. So if you're running 6s4p, you'd have 80A of continous output. 25R's are very widely used in esk8 and other hobbies and are pretty much a gold standard for li-ion. They have higher energy density meaning they pack more punch for the space used.
```

---

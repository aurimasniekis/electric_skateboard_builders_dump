# Inductive charging (wireless) for eboard? Is this possible?

### Replies: 127 Views: 4796

## \#1 Posted by: Okami Posted at: 2017-01-19T17:30:01.767Z Reads: 274

```
Hi there! I recently came up with an idea - how cool would it be to charge your board wirelessy!

Let's say, place the board on a pad and the charging just starts!

It would need a special enclosure / position probably but anyways I think this might be cool.

Balance charging might sometimes suck.. there''s a long cable to my turnigy balance charger.. then there are these 2 wire harnesses, one for main plug, one for balance ports.. and it all has to somewhat stick together..

With wireless charging it would be like - just place it  and go..

--
Video of someone doing a 24v 5w transmission (he claimed that he used 24v 5w bulb)

https://www.youtube.com/watch?v=2ODW-ntPHSU

----
Background found so far from other ''fields'':

Phone ''Qi'' charger pads seems to be rated at 5w, I dont know yet is this actual wattage put out at battery but I will take a look at it!

If 10 of these were combined we would get 50 W or so of power, the only problem still would be to get higher voltage for the charging purposes! 

Unless each cell group were divided seperately, each having its own panel..

But yeah, I still got to take a look at this.. and there would be a need for a lot of panels to charge this way and it might not be the most effiecient way possible!

----
One other guy who has the same idea but about the ebike (video taken from his discussion):

https://endless-sphere.com/forums/viewtopic.php?f=14&t=41064
```

---
## \#2 Posted by: Okami Posted at: 2017-01-19T18:19:16.753Z Reads: 246

```
Some more info:

> Taken from: http://4hv.org/e107_plugins/forum/forum_viewtopic.php?74096


> At the high power end of the scale you will find that the technology exists to fill a room full of enough wireless power to run laptops, light lamps and charge phones etc. 

>The problem is that the required field strength is many many times greater than recommended human exposure levels in safety standards.
 
>**It also causes serious interference problems to equipment that doesn't contain the necessary screening to make it wireless power tolerant! Not to mention induction heating of pretty much anything conductive in the field!**

> -Richie
```

---
## \#3 Posted by: Hummie Posted at: 2017-01-19T18:48:52.460Z Reads: 231

```
Funny they're talking about it in the balancing thread because I think with an inductive charger for each cell i think you could balance the pack!!!

I like this idea. 

I Think someone other than me who knew more wouldn't have difficulty with this and I only understand the basics.   If each cell simply had its own inductive charging coil and rectifier to bring it to 4.2 or whatever.  So simply if you had ten or twelve of those inductive phone chargers with each connected to a different cell and then maybe even just one coil they all sat above.  Maybe it would need two coils per cell or maybe one coil on each cell and one on the garage floor.  And a rectifier for each cell
```

---
## \#4 Posted by: Okami Posted at: 2017-01-19T18:50:16.420Z Reads: 223

```
Yes, that''s the idea! Im trying to find out about how big is the coil power output for ''our sizes''.. since the receiving coil will need to be placed on the board..

BTW, one more great video:

https://www.youtube.com/watch?v=Gw6XtzEOlyI
```

---
## \#5 Posted by: Hummie Posted at: 2017-01-19T18:53:19.617Z Reads: 213

```
What do u think of a coil and rectifier for each cell so that they are balanced?  I bet that's doable.  I really like that. Simplification x2

I'm totally smitten and have an electronics direction. Anything u figure out please add it.   Smitten!
```

---
## \#6 Posted by: Okami Posted at: 2017-01-19T18:59:54.178Z Reads: 204

```
haha for sure! This is as intriguing for me as it is for you, it seems!

I think you saw the other thread and that ''monstrous'' car charger in terms of max output.. 

It did not take up thaat much space, I think, to be able achieve ~7kw output which seems just ridiculous for the size they use.. I hope they dont lie with the numbers.. and the charger really looked comparatively small, especially the ''plug'' / surface point outside of the vehicle's body.

Anyways.. so far it is seems it might be possible to achieve reasonable power output.. the only other part would be to find a smart enough guy to construct the circuit.. I already asked a question to the guy who made that one youtube video  I posted here, I hope he responds and can tell some more numbers concerning these things..

Basically it looks like it is a ''simple'' transformer.. but just with this oscilating frequency adjusted to each other (both coils). But of course, there are a lot of other components (Signal generation) around the coils itself, so it wont be a simple matter of just getting the right coil size and then generating some output power / signal for one of the coils.. 

so yeah, let's see how it goes.. and let's hope someone in the world has already come up with a close enough solution for our needs :slight_smile:
```

---
## \#7 Posted by: IDVert3X Posted at: 2017-01-19T19:01:40.323Z Reads: 168

```
Wireless energy transfer is the most unefficient way you can use... It looks cool, but its really not that great. And in introduces more problems that it solves.

I would not recommend anyone doing it.
If you want to do it anyway, learn something about EMF and resonant circuits in general.
```

---
## \#8 Posted by: Okami Posted at: 2017-01-19T19:02:53.138Z Reads: 161

```
@IDVert3X Do you mean even the ''directed ones''?

There seems like there are 2 types of energy transfer.. one is like in tesla coils.. and the other is the one transformers use.. (close / directed proximity)
```

---
## \#9 Posted by: IDVert3X Posted at: 2017-01-19T19:05:10.642Z Reads: 156

```
Tesla coil was a failed attempt to transfer energy wirelessly.

I mean the one where you use one coil to emit EMF and the second one very close where the voltage is inducted from EMF. There are also heating problems with increased power.
```

---
## \#10 Posted by: Hummie Posted at: 2017-01-19T19:05:19.126Z Reads: 142

```
Strange because I just read it was really efficient.  I really don't know want I'm talking about yet but even if inefficient I don't think it would matter.  Could be done on trickle
```

---
## \#11 Posted by: IDVert3X Posted at: 2017-01-19T19:08:30.654Z Reads: 141

```
One question. WHY you NEED it?
The "cool" effect that is used to sell phones?

Think about how slow its going to be...
Also heat is the no. 1 enemy for the batteries.
```

---
## \#12 Posted by: Okami Posted at: 2017-01-19T19:09:04.904Z Reads: 136

```
Yeah, we need some efficiency numbers for this.. If you place the other coil far away the effiency might be less, I assume. So it will always be somewhat important to keep the coils in the right distance/position

--

5w x 10 = 50w.. does not sound that bad, if that can be outputted.. I charge 7ah battery for about 3hours with 60w, for 5ah these 50w should be quite ok!
```

---
## \#13 Posted by: IDVert3X Posted at: 2017-01-19T19:12:07.445Z Reads: 130

```
Thats not really how it woks, you cant easily stack them. And 50W wireless trasfer would introruce a lot of heat ( besides other problems ).
```

---
## \#14 Posted by: DeathCookies Posted at: 2017-01-19T19:13:16.485Z Reads: 125

```
I think you will only get about 70% into the battery and that is a big loss in energy. If you have the money then do it. It is easier to charge than to plug in a charger ;)
```

---
## \#15 Posted by: Okami Posted at: 2017-01-19T19:13:58.713Z Reads: 124

```
mh, I have to look into that heat thing!

Well, anyways, it seems like these ''phone coils'' are quite small.. For board it still should be possible to make 3-4x the size of the phone's charging coil..

I agree that electronics might need some shielding.. it was mentioned by one user from another forum..
```

---
## \#16 Posted by: Okami Posted at: 2017-01-19T19:15:57.026Z Reads: 114

```
Well. I calculated the power cost and it came to something like 0.02 euro cent per charge.. I wont complain if the ''power amount and its price'' increased to 0.05-0.10 cent..

~80w X 3.25h = 180 wh = 0.180kwh (Cost per electricity ~10cents/1kwh= ~0.02 cents
```

---
## \#17 Posted by: IDVert3X Posted at: 2017-01-19T19:16:52.488Z Reads: 111

```
Magne Charge employs high-frequency induction to deliver high power at an efficiency of 86%.

At 50W, there are 7W lost as heat.
Thats a lot!
```

---
## \#18 Posted by: Okami Posted at: 2017-01-19T19:17:39.593Z Reads: 114

```
Away from batteries perhaps? At the front of back or the board :slight_smile:
```

---
## \#19 Posted by: IDVert3X Posted at: 2017-01-19T19:25:05.535Z Reads: 117

```
Just... WHY?
Why to do it the more complex, more expensive and unefficient way when you can just use cable?

KISS.
```

---
## \#20 Posted by: mountainboardlover69 Posted at: 2017-01-19T19:26:44.591Z Reads: 122

```
i rly like ur ideas guys 
here is a simler but also very cool <img src="/uploads/db1493/original/3X/0/5/0527f089c1d2e969db35c3b89e4d825985f2a319.png" width="690" height="363">
so if u hang it on the wall wit those hooks in the charger 
u board wil charge dont know how to balance charge but okay just somting i had in mind
```

---
## \#21 Posted by: Okami Posted at: 2017-01-19T19:27:37.979Z Reads: 112

```
Yeah, wanted to answer to this:

**Practicallity reasons..**

* No need to carry around wires
* Leave the wires on the ground
* Could be developed as a standalone product

---
If I dont come up with a wireless solution, I might as well try to figure out to make a removable battery or at least a battery contact which is more ''smooth'' / easier to connect.
```

---
## \#22 Posted by: IDVert3X Posted at: 2017-01-19T19:30:55.495Z Reads: 102

```
Your answer in short: no cable
Instead, you have a big plate on a ground / wall.
Congrats.

DO IT.
```

---
## \#23 Posted by: Okami Posted at: 2017-01-19T19:36:39.202Z Reads: 99

```
hah, you actually seem pissed off that someone tries to come up with such a solution.. :D

Im not sure why do you concentrate so much on the efficiency! We use a lot of in-efficient things around us.. and besides ''baking'' some electronics (if the heat is really a problem) what bad can happen?
```

---
## \#24 Posted by: IDVert3X Posted at: 2017-01-19T19:42:59.074Z Reads: 100

```
Im not pissed off.
I try to explain the problems it introduces so you dont have to waste your time doing something pointless. But if you want, do it. At least you will learn something new once you finish it or give it up due to many problems.
```

---
## \#25 Posted by: Hummie Posted at: 2017-01-19T19:48:50.150Z Reads: 96

```
If charging a board slowly is possible by simply putting it somewhere, and it will balance all the cells, seems an obvious plus.  
Even if efficiency isn't that good I wouldn't mind as I don't count the pennies when charging and the heat could be isolated as said.
```

---
## \#26 Posted by: Okami Posted at: 2017-01-19T19:55:34.958Z Reads: 106

```
So far I came up with the numbers = 10-18% and it was a somewhat diy version of these wireless power transmission circuits..

So, taking 18% efficiency, that would mean instead of putting in 200w of power, we would need 1000w .. Ok, at 10% it is a bit worse.. but still - dont you know in how many other ways ppl waste energy? :D 

--

@Hummie at least you are with me on this one.. :D

The reason for inductive (wireless) charging, would be to leave the board for the night.. even if it takes more than 5hours to charge (if the charge rate is slow).. then you would have a charged board next morning without the hassle of plugging in wires, removing them, turning off devices etc..

I dont promise I will build anything in the coming month or so.. but if this topic is ''feasible'' enough I might go and talk with some more ppl who know more about inductiion, electromagnetic fields, transformers and other stuff.. 

I just see this as an opportunity to make something that has not been seen before :)
```

---
## \#27 Posted by: Okami Posted at: 2017-01-19T21:53:16.445Z Reads: 103

```
Ok, latest find:

http://powerbyproxi.com/wp-content/uploads/2012/09/PP150-P012-Datasheet-v1.8-15-mm.pdf

<img src="/uploads/db1493/original/3X/0/6/0603202593e019c9587eef2b9c7df024e06029d9.jpg" width="690" height="145">

<img src="/uploads/db1493/original/3X/c/e/ce14930c867ae003af993fbac87d7902d6541860.png" width="458" height="43">

<img src="/uploads/db1493/original/3X/3/4/3451414062b0ff765ca81cd1a77aa55de9a0deaa.png" width="690" height="449">

<img src="/uploads/db1493/original/3X/9/4/946ce56260c2d35a9b2e7b7e3d81cacfd6c8c3f6.jpg" width="640" height="500">

---

It is bulky, I know, but I think it is made this way to withstand the mechanical shocks and other stuff in the environment it was designed for (forestry for example)..

Maximum distance seems to be 10mm without loosing voltage, still might work ok, if the pad and the receiver box is constructed in a right manner.

I wrote them a message, enquiring about 40mm optimum power transmission distance and capability of 100-200w output, will see if they are nice enough to reply and give out some more details!

~83% efficiency does not sound bad.. 10mm distance is a bit too little, should find out how good it works for about 40-100mm.
```

---
## \#28 Posted by: darkkevind Posted at: 2017-01-19T23:00:10.180Z Reads: 84

```
I like your idea but wouldn't you just use a BMS and feed the power wirelessly to the BMS which will take care of the balancing for you?

Although, when using a BMS you lose all the extra cables and have just one, similar to a laptop charger lead... won't that be sufficient for you as you won't have power + balance cables any more?
```

---
## \#29 Posted by: Okami Posted at: 2017-01-19T23:01:39.934Z Reads: 88

```
Yes, some type of bms circuit would be totally needed to charge effectively the battierys.

I might move onto a bms solution but for now I either have to stick with my current setup or make up how to make the connectors more convenient or the battery removable..

--

This is just an idea of the concept.. If I come up with something that is reasonably affordable and doable, I will also post it here..
```

---
## \#30 Posted by: Hummie Posted at: 2017-01-19T23:21:18.030Z Reads: 85

```
I liked no bms and instead a "receiver" on each battery cell.  Each would take the voltage from the "transmitting" coil separately.  I don't know if that's possible to have the single transformer coil effecting the multiple but think so.  No bms needed
```

---
## \#31 Posted by: darkkevind Posted at: 2017-01-19T23:25:06.132Z Reads: 84

```
But how would you avoid overcharging?
```

---
## \#32 Posted by: Hummie Posted at: 2017-01-19T23:29:13.157Z Reads: 84

```
The voltage coming from the coil would be fixed.  Actually think about it I don't know😥 .   Maybe if the voltage from the main coil is 4 volts when the cell hits four volts no more current would flow.  That's a big assumption.  Anyone know if it would work like that?  It makes sense to me.  Can't have a current when there's no voltage difference
```

---
## \#33 Posted by: captainjez Posted at: 2017-01-20T00:09:10.189Z Reads: 76

```
We've been playing with inductive charging through our battery housing, but the biggest issues we've found is the amount of current we can push without making the coil melt will making charging intolerably slow.
```

---
## \#34 Posted by: Okami Posted at: 2017-01-20T00:09:18.998Z Reads: 80

```
I got your point / idea now..

Instead of one big receiving coil, there would many, smaller coils, each coil could charge its own cell group, This way Voltage would not need to be as high and each cell group / pack, would be almost individually charged..

Not so sure about terminating voltage, but in theory it should work - similar like bulk chargers work, I guess.. depends probably on how that energy transfer works and what dynamics is involved.. perhpaps there could be a little receiver/transmitter, which would let the transmitting coil to shut off completely once cells are charged.. 

The termination of charge probably should not be the hardest part as I think it is not that hard to measure voltage and then make a switch for dismantling the circuit..
```

---
## \#35 Posted by: Okami Posted at: 2017-01-20T00:11:09.175Z Reads: 78

```
Could u give a little insight onto what amperage you achieved? Some clues would be nice :slight_smile:

Ok so from what you are saying.. heat is a problem with higher currents

One more Q - with what distance between the coils you experimented?

This seems to affect the power output/efficiency greatly :slight_smile:
```

---
## \#36 Posted by: captainjez Posted at: 2017-01-20T00:14:07.049Z Reads: 79

```
So far we've been able to push fairly stable just under 1A without causing too much heat through the coil. In our tests with higher amperage we've managed to melt a few coils. Mind you these are fairly compact coils so that we can fit them into our existing electronics housing.

The distance we tested was roughly 9mm between.
```

---
## \#37 Posted by: Okami Posted at: 2017-01-20T00:16:25.670Z Reads: 77

```
@captainjez Did you make custom ones or just experimenting with the current ones made for phone charging?

To me it seems, if using such small coils, that a method of removing heat would be totally necessary.. you should try at least with a fan.. what amps can you get..!

Turnigy chargers (at least mine) also kick in fan, if amps is over 2.0 for 6s voltage.. temp is around 30-40degrees C I think when this happens..
```

---
## \#38 Posted by: darkkevind Posted at: 2017-01-20T00:16:55.110Z Reads: 77

```
You would only lower the amps/current needed if - like you say - you had a coil for each cell, but how would you align them up for charging? You'd need three at least for a 3s battery pack, and 3 transmitting coils in the charger, all three would have to line up like you have to perfectly align your mobile phone on it's charging pad....
```

---
## \#39 Posted by: captainjez Posted at: 2017-01-20T00:18:28.864Z Reads: 77

```
Custom made coils right now. These were left over coils I had from another project we were working on. Can't put a fan as we have no room left in our case :)
```

---
## \#40 Posted by: Okami Posted at: 2017-01-20T00:20:54.809Z Reads: 81

```
Im not at expert on this one yet.. but it looks like there can be ''a bigger transmit pad'' and many, smaller receiving coils.. 

I agree about alignment.. If the coils/circuit is not that effective, the coils will need to be aligned quite precise..

Anyways, take a look at this - his ''field'' is wide enough, that he can charge phone and run the tv at the same time:

https://youtu.be/j4sAzaKfbRc?t=8m42s

You might need to switch a few seconds back or forth.. dont have sound at the moment :)

---

@captainjez hah I see... anyways would be cool to see how high can you go with a cooled coils.. just to know what the amp limits might be with heat removal.. heat removal is practised in a lot of fields in electronics anyways, why not use it here, if it would be beneficial :)
```

---
## \#41 Posted by: Hummie Posted at: 2017-01-20T00:29:36.652Z Reads: 76

```
i thought with a transfomer you could get it to produce a desired voltage with different thickness of wire and the important part was the two coils ratio of windings to each other.  you could bump everything fatter for higher current.  .  
9mm is pretty far considering you could just put them 1mm or closer.  even at 1amp that would be good enough to charge through the night..and maybe heat the room a bit too.

I think it's pretty much just a transformer with a rectifier.  comes out of the wall ac at 120 get that converted to 4 volts.

this would be cutting the voltage way down and the amperage would go way up in the transfomer and just cut it to dc at the right frequency.  this is my huge simplification of what I think is done
```

---
## \#42 Posted by: captainjez Posted at: 2017-01-20T01:58:52.896Z Reads: 70

```
Ours is 9mm because we have to count the wall thickness or our enclosure and the double water seal to ensure that nothing gets in. Trying to get it down a bit.
```

---
## \#43 Posted by: Hummie Posted at: 2017-01-20T08:48:20.368Z Reads: 71

```
http://www.ebay.com/itm/Qi-Wireless-Charger-PCBA-Circuit-Board-With-Coil-Charging-Pad-for-DIY-Arduino-TW-/142013070415?_trksid=p2141725.m3641.l6368

cheap
already built
likely has some safety features.
1 amp  
5 volts  (?which i've often seen being used to power li-ion cells and I don't know why?)


or maybe 12 of these are stackable and could be connected to cells and put on the charging pad:

http://www.ebay.com/itm/Qi-Wireless-Charging-Receiver-Card-Charger-Module-Mat-for-iPhone-6-6s-Plus-5-5s/361740678560?_trksid=p2141725.c100338.m3726&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D20150313114020%26meid%3D456428bcc57f4ea9af053ea7c7a74888%26pid%3D100338%26rk%3D2%26rkt%3D30%26mehot%3Dpp%26sd%3D222251515281
```

---
## \#45 Posted by: darkkevind Posted at: 2017-01-20T10:03:26.661Z Reads: 71

```
It can certainly be done at a distance....

[https://youtu.be/U0Vaw5P8T-o](https://youtu.be/U0Vaw5P8T-o)

If you had 3 of the Qi receivers on each cell and then a big transmitter coil, that might work?
```

---
## \#46 Posted by: Okami Posted at: 2017-01-20T10:27:58.863Z Reads: 70

```
Yes, you should look up these ''3d charging pads'' They are like a bowl and I believe you put multiple devices into them.. the devices of course need to have receiving coils built into them (usually in the case)

https://powerbyproxi.com/proxi-labs/proxi-3d-in-device-charging-system/

https://youtu.be/RWDBPFQQJno

Looks like this could be more mainstream incorporated in the future.. the prices need to go down of course but that idea of just placing multiple devices onto a pad and leaving them there seems very conveniant.. no need to find charger for each device, if it can tuned in such a way that each device receives how much it needs.

---
Btw, it looks like the big guys had beem working on this for a while:

<img src="/uploads/db1493/original/3X/0/9/09de6050ad7dcc70db874ef3eaaa928291cf75d4.png" width="690" height="117">

There was also little statistic, that London bus achieved 60% efficient power transfer between 12cm/4.7in

Source: _Wikipedia Wireless Power article_
```

---
## \#47 Posted by: Hummie Posted at: 2017-01-20T17:18:55.016Z Reads: 64

```
maybe u we're doing something different as these must stop charging at the max charge.  That's how they're designed or people would be blowing up their stuff left and right.  My power supply I set it to a voltage and that's as high as it will charge the cells. No current flows if there's no voltage difference


Seems cheap to me.  Need this at 40$ 
 http://www.bestbuy.com/site/samsung-mini-qi-wireless-charging-pad-black/7250019.p?skuId=7250019
And the little things I posted above at like 2 bucks each!  Maybe u need a pad for each cell with this pad but there's others out there that can do multiple devices at once. As u posted
```

---
## \#48 Posted by: Hummie Posted at: 2017-01-20T17:28:53.742Z Reads: 65

```
Why do u say 3 receivers on each cell?  I'd think one

This is something that can be experimented with for little investment and much is already done.  I'm going to simply get a couple of those receivers and take them to Starbucks or wherever else they have a qi pad with my multimeter and see if I can get them to work stacked.
```

---
## \#49 Posted by: darkkevind Posted at: 2017-01-20T17:30:37.387Z Reads: 64

```
Yeah i meant 3 in total, one on each cell... :slight_smile:
```

---
## \#50 Posted by: Hummie Posted at: 2017-01-20T17:44:06.283Z Reads: 63

```
Your video the tech is much harder to use than simply inductance charging which is simply a transformer.  I'm still unsure how they transfer the energy as typically a transformer has both coils on the same core and the qi is completely flat so no second coil is being looped over a core on the first coil.  But still pretty sure it's the same basic tech as done on toothbrushes and just induction charging.
```

---
## \#51 Posted by: Eboosted Posted at: 2017-01-20T18:08:54.366Z Reads: 64

```
[img]https://gaijinass.files.wordpress.com/2016/03/thats_a_penis_reverse.gif[/img]
```

---
## \#52 Posted by: Okami Posted at: 2017-01-20T18:15:25.498Z Reads: 63

```
@Eboosted  :D you really picked out / chose the best details / picture from this thread! lol :D

Besides.. his idea is not that bad.. will find about one of evolve's guys who made a similar looking thing to charge his board just by ''stacking it'' into place or something..

--

@Hummie I like your idea! Please do so, if you can source them quickly! China is way too far from me and will take too much time to do that + I dont really trust these little coils yet.. I think to achieve some better result there will be a need to make some custom, perhaps different wire and diameter coils for better power output - 

Though - I will agree that these are quite cheap, ready to use.. and for experiment they are totally okay! Just to see, if they can be stacked or what is the minimum distance they need to be from each other not interfere.. -- Fast forward -- I like the idea about the charging mat - it should provide the possibility for multiple receiving coils close to each other 

So basically, just report back once you get some more info about whenever it works or not!

I will try to ask around and contact some more manufacturers or company's who are dealing with wireless technology.. I dont expect that they will give out their intelectual property right away.. but perhaps there can be a deal or some sort of mutual agreement made with them..
```

---
## \#53 Posted by: Hummie Posted at: 2017-01-20T18:55:11.273Z Reads: 61

```
http://www.ti.com/lit/ml/slyt570/slyt570.pdf

http://www.mouser.com/search/refine.aspx?Ntk=P_MarCom&Ntt=145589046

http://www.mouser.com/applications/wireless-charging/

i'm all over this and on hold with texas instruments.  trying to get someone who can dumb it down for me.


I think stacking the standard receivers won't work as they're shielded to get better coupling.  maybe cut the shielding off though.  or another coil.  who knows but texas instruments is going to respond by email to tech questions.
```

---
## \#54 Posted by: IDVert3X Posted at: 2017-01-20T19:12:54.384Z Reads: 60

```
You really should learn basics of electrical engineering, EMF, resonant circuits and other stuff related to this topic before you begin to work on it. Doing something without understanding how it works and which problems / dangers it introduces is just stupid. You will end up having non working device or blow something up ( unless you use a pre made solution ). You should also buy an oscilloscope for debugging those kind of circuits. You will also need a BMS in the board.
```

---
## \#55 Posted by: Hummie Posted at: 2017-01-20T19:17:22.933Z Reads: 63

```
agreed.

easy reading those links are
"Resonance is a property of an oscillating system which drives another system to oscillate with a greater amplitude at a designated frequency. For example, if you have two tuning forks that respond to the same frequency, by playing one fork the other tuning fork will begin to vibrate due to resonance. This same property is achieved in electrical systems through resistor, inductor, and capacitor (RLC) circuits. 
Weakly coupled magnetic resonance, although less energy efficient, reduces the proximity requirements of inductive charging. Nikola Tesla was famous for his experiments using the electromagnetic field (EMF) of the Earth’s ionosphere in an attempt to distribute energy. Similarly, magnetic resonance (non EMF) relies on magnetic fields but allows primary and secondary coils to have fewer magnetic field lines in common. This increases the system’s spatial freedom, allows the coils to differ in shape and size, and allows multiple devices to charge from a single source, establishing a one-to-many relationship."

but not the resonant energy but plain inductive energy transfer and using 12x12 coils, that i think will top the voltage on each cell and put it on simmer
```

---
## \#56 Posted by: mountainboardlover69 Posted at: 2017-01-20T20:42:05.029Z Reads: 51

```
haha 
i dont tink so but it kada looks like it
```

---
## \#57 Posted by: Hummie Posted at: 2017-01-20T21:22:53.836Z Reads: 57

```
add one of these after receiving coil
http://www.ti.com/lit/ds/symlink/bq2000.pdf

what's missing?  
can't find those 2$ receivers anywhere locally, today, and will get it shipped but regardless will likely need the bit linked right above and it's included inside a phone.

or forget most of the complication and get these and then just need to supply 12v dc to primary coil
https://www.adafruit.com/products/1407
very tempting.  but what's the deal with the 5v and does that mean I wouldn't get the cc cv id like for the lithium chemistry? i think so ..so how to add that other part i linked?
```

---
## \#58 Posted by: devin Posted at: 2017-01-21T03:01:44.107Z Reads: 53

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#59 Posted by: Hummie Posted at: 2017-01-21T03:04:49.339Z Reads: 56

```

"This is a basic charger set, and it does work, providing 5V DC output from the output half when the input half is powered with 9V to 12VDC. You can draw as much as ~500mA if the coils are 2 or 3 mm apart. "

so only half an amp is coming out of these at 5 volts, so only maybe 3 watts, times 12 cells with chargers.  40 watt charging.  too slow for me with a 250watt hour pack but if the battery were much bigger these could still be ideal. slow charge a big pack you drained through the day and charge it overnight while you slept. 
if i were to set it up on my board i wouldn't even need a switch to turn it on anymore, just keep the esc in constant ON hard wired and leave the board on it's cradle all the time.   no switch needed.  and definately no bms.  no plug.  !! waterproof to the extreme.  plus a million other plusses.
```

---
## \#60 Posted by: devin Posted at: 2017-01-21T05:32:00.310Z Reads: 60

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#61 Posted by: Okami Posted at: 2017-01-21T09:15:31.460Z Reads: 59

```
@devin I assume you like do calculations and this was one more area to express yourself.. so I assume I should say thanks for throwing in some numbers for this one!

Can you explain the ''Pulsed DC current part''? 

I understand that receiver coils receives AC current, which then needs to be rectified and smoothed out to DC current once again.. but im not sure is this the same thing you mentioned.

---
Your idea about ''inserting a iron / ferrite rod between the coils'' is also not that bad I think!

Perhaps it could be done in a manner similar like this: 

<img src="/uploads/db1493/original/3X/3/e/3e0d2e359a52f7a8b07aaf55d7ab850b69a4dbf0.png" width="359" height="147">

Deck itself contains the coil, perhaps there is some sort of ''hole'' / opening to accomodate the iron core, for increased efficiency. Iron core would be sticking out of the transmit pad..

----

<img src="/uploads/db1493/original/3X/0/1/0102119789c8884d7622aaa956df1f1465a262d1.png" width="349" height="153">

Size minimization for coil and other electronics - embedding in the deck.)
(no iron core through the coil)

----

<img src="/uploads/db1493/original/3X/5/e/5ed405d6c06007169ad2266bab971602d1e05abd.png" width="352" height="102">

Just some kind of little ''lump'' for the sending coil to be able to be closer to the receiving coil. I made this in a somewhat oval shape, but the opening could be something similar like car 12dc jack, - ''barrel style''

(sorry for the rough drawings)

Btw - I actually imagine doing something similar (with barrels / big contacts) if this wireless idea cannot fruit now.. For dc contacts part the only problem would be to secure them / protect from the weather - water, while at the same time making them easy to use.. so no fiddling around them would be needed! But this still would not be as nice solution as the wireless system, where the board just should be put in the right position and left there..
```

---
## \#62 Posted by: Hummie Posted at: 2017-01-21T10:02:07.392Z Reads: 49

```
best bit I've found:
http://www.ti.com/product/BQ51052B/datasheet

this is a cheap receiver and includes all the details needed to charge lithium to 4.2 at 1.5 amps!  simple and tiny at like 3mm x 2mm.   now to figure out how to plug it together.
```

---
## \#63 Posted by: Okami Posted at: 2017-01-21T10:06:15.798Z Reads: 48

```
@Hummie omg I think you are getting closer to this! I hope there are all the required parts.. so we would not need to (you personally, as first tester).. fiddle with coils, wires and capacitors and other stuff!

I read that forum where guys (or seems to be 1-2 of them) made their diy coils.. but ohboyh how many questions they had about the working principles of this tech! They were able to get a somewhat crude model.. working at like 10-18% efficiency..

But you have to understand one thing : These guys are just going after the distance.. not the power..

**We are going after a power.. since we can somewhat adjust what distance we will use to charge our boards!**

----

I can actually show some crude graphs of what others, sometimes in ''laboratory enviroment'' achieves.. and this is without taking into consideration, the New Zealander company, which seems to be working on this for 9yrs already!.. They got 100-150w units working.. some of them are qute bulky for our needs.. but non the less - they work at the required power levels we would need! 

_Im living with 80 charger for 192wh, so with 100-200w there should be enough power to charge decentlhy! When I will be able I will probably make a charging chart for newbeginners! This is somewhat easier than to make .. battery chart with all the finnicky_ details batteries have in common!
```

---
## \#64 Posted by: Hummie Posted at: 2017-01-21T10:20:48.767Z Reads: 45

```
id be happy to use this last chip and charge at 60 watts as long as i add a huge battery.  

 hoping to be spoon fed now what to do with the chip.  This will be much easier than trying to reinvent the wheel though

http://www.ti.com/lit/ds/symlink/bq51050b.pdf

data sheet for it
```

---
## \#65 Posted by: Okami Posted at: 2017-01-21T10:26:05.848Z Reads: 45

```
I took a look at the chip!

I think it just needs a coil as in input.. sort of like that..

Did you check one my documents I sent? There was some shematics info about Qi chargers and how they work.. some answers might be in that document!..

---

1.5Amps per chip did not sound bad at all!

I assume with some extra cooling these chips could be run to their max rating!

Otherwise, for conservative purposes we should be running them at ~1A or so probably.

Plus, we have to look up if all coils are fine for this... some are rated only till 500ma.

----

If, we get 1A per cell group, then depending on how many cells in parallel,  we would probably get around 0.33A per cell (3P pack), If we run 4P then it would be a bit worse..And this is one 1A capable coil per cell group.. now we need to multiply this probably by the count of how many cells in serial we got (6-10S)..

If we had a chance to get 2A from single coil, then we could get the same power for 2 cell groups at once. So half less coils we would need to charge the batteries!

I just imagine how this would look like from charging perspective, if did get that 1A of power, at the receiving coil.
```

---
## \#67 Posted by: Hummie Posted at: 2017-01-21T10:38:24.393Z Reads: 34

```
we're not just connecting coils to cells this is pretty much plug and play stuff.  if you look at the last link i posted if one inductance charger is attached to each cell it will effectively be a balancer.  won't have all the functions of a bms and all that safety but good enough for me.

there/s a chat forum that the texas instruments people have and I should get over there and maybe get it figured but i think it's gunna be easy and there's a matching part intended for this part.  
just need to do the source side and break up the 120ac into...cant find it on the sheet but not a problem
```

---
## \#68 Posted by: Okami Posted at: 2017-01-21T10:38:36.712Z Reads: 35

```
We will get to resonant circuits, dont worry! I think @Hummie is on the way to find everything commerically already made, we just need to put it all together..

I agree that building resonant circuit might not be as easy.. but for some easy tests, it looks like signal generator can also be used! It just need to be able to ouput high enough frequency.. with high enough power, I believe..
```

---
## \#69 Posted by: Hummie Posted at: 2017-01-21T10:41:45.359Z Reads: 43

```
from what i read resonant is kind of a gimmick and it's simply inductive but with better frequency coupling.  nothing really different.  plain old inductive up close for high power is good and this stuff already made by the pros has all the safety and testing needed and cheap i think.  I'm still on the plan
```

---
## \#70 Posted by: IDVert3X Posted at: 2017-01-21T10:44:25.686Z Reads: 46

```
https://youtu.be/ExU32UyGX6w
https://youtu.be/3E5PUnYlaTM

Hope it makes things little bit more clear for you.
```

---
## \#71 Posted by: devin Posted at: 2017-01-21T15:47:31.415Z Reads: 46

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#80 Posted by: IDVert3X Posted at: 2017-01-21T17:34:55.665Z Reads: 45

```
@devin, this went too far from the original topic, for this reason, I deleted my posts, you should do the same and let's talk about this in a PM ( which I sent you btw ).
```

---
## \#81 Posted by: devin Posted at: 2017-01-21T18:54:50.702Z Reads: 46

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#82 Posted by: Hummie Posted at: 2017-01-21T19:15:54.333Z Reads: 39

```
your theory is already on the site many times I think.  how bout leaving it in your thread so we can keep this to the topic
```

---
## \#83 Posted by: devin Posted at: 2017-01-21T19:17:54.900Z Reads: 38

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#84 Posted by: Hummie Posted at: 2017-01-21T19:27:06.102Z Reads: 34

```
you can have induction without a core though.   all the ones I posted don't have one.  I'll give you my theory when I come up with one.
```

---
## \#85 Posted by: devin Posted at: 2017-01-21T19:27:50.349Z Reads: 32

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#86 Posted by: Hummie Posted at: 2017-01-21T19:34:43.245Z Reads: 31

```
i think you could get the 4.2 after the rectifier but lithium charging for safety needs a switch from cc to cv and a shut off of some sort I believe and that's a complication that has to be added.  

they use pure copper or close to it.  the better the conductor the better for an inductor I'd think and it's a layering of the magnetic field.  the core adds more comlexity in the process.  I think you can get much greater permeability and a much stronger magnetic field per amp with mu metal.  it saturates quickly as well but as far as greatest magnetic field build able it's top.  maybe it's chemical structure reveals why but ...how bout what to do to put the parts necessary to get the board charged?
```

---
## \#87 Posted by: devin Posted at: 2017-01-21T19:35:32.401Z Reads: 31

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#88 Posted by: Hummie Posted at: 2017-01-21T19:38:22.331Z Reads: 30

```
yes it would shut off.  but theres more things that lithium needs with the cc cv i believe and going straight to the cell is bad for the batteries.  the cc cv thing they like.  I wish I could omit and simplify...but that chip is an all in one it seems.
```

---
## \#89 Posted by: devin Posted at: 2017-01-21T19:39:21.216Z Reads: 31

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#90 Posted by: Hummie Posted at: 2017-01-21T19:40:58.880Z Reads: 30

```
i'm looking up the cc and cv thing now to see what the hell it's about really but it seems mainly so the current isn't too high,,but dont think that would be a problem to begin with since the induction coils will only transmit 1.5 amps.
but the "transformer" and rectifier need not be bulky or big.    And bms break often.
```

---
## \#91 Posted by: devin Posted at: 2017-01-21T19:42:27.603Z Reads: 25

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#92 Posted by: Hummie Posted at: 2017-01-21T19:53:06.510Z Reads: 21

```
the more i look into cc cv it's purpose is not to add too much current into a cell that's too small by applying a full 4.2 voltage and end up with too high a current.  in our case I don't think it will be important as the battery will be big and have no problem taking the current.  but the  circuit might require it if made from proprietary parts.  

Id like to skip cc cv if possible and think it could be done since the max current would be small coming from the coil.
```

---
## \#93 Posted by: devin Posted at: 2017-01-21T20:05:58.954Z Reads: 25

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#94 Posted by: Okami Posted at: 2017-01-21T20:37:44.995Z Reads: 26

```
This topic seems to answer what happens at 60hz:

http://electronics.stackexchange.com/questions/159170/is-wireless-power-transfer-by-induction-at-60hz-possible-or-does-the-frequency?rq=1

> Inductive power transfer is possible at 60 Hz in fact that's how transformers work BUT you are wanting to transfer over a quarter of an inch so at best you imagine a transformer that is of the double E type and then picture the primary on one E and the secondary on the other now if your imaginary E cores are butted together you have your double E transformer that will operate normally but from experience it will be a buzzy bee SO far so good but here is the problem when you gradually increase the gap the reactive magnetising current increases heating the copper wire So the transformer will have to be huge to support your distance I suspect in the kilowatt ballpark SO possible but at lowpowers not practical

<img src="/uploads/db1493/original/3X/d/e/de2dfc3eb5dc16b2b292612b4a692177fac5b7ec.png" width="180" height="65">



> It's certainly possible, but AFAIK it usually involves high inductances (beefy coils), high powers (multi-ton induction furnace) or both. I think most consumer-level induction power transfer devices (induction chargers, induction cookers etc) work in the high-kilohertz level, making semiconductor power switching an absolute neccessity, but at the same time many other aspects of the device simpler.

<img src="/uploads/db1493/original/3X/5/9/59b17a6ae2e1e91f98c89964727f0e44b158a400.png" width="203" height="82">
```

---
## \#95 Posted by: devin Posted at: 2017-01-21T20:57:41.834Z Reads: 21

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#96 Posted by: Okami Posted at: 2017-01-21T21:00:31.395Z Reads: 21

```
@devin From what you are saying so far I only understand that iron 56 is pretty special material /  substance.. which enables to achieve / do thing u couldnt do with other materials / substances.
```

---
## \#97 Posted by: devin Posted at: 2017-01-21T21:05:33.415Z Reads: 22

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#98 Posted by: devin Posted at: 2017-01-21T21:21:19.085Z Reads: 27

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#99 Posted by: IDVert3X Posted at: 2017-01-21T21:29:56.730Z Reads: 27

```
DEVIN!

You see that domain? electric-skateboard.builders.
I do too. And I can't find iron-56 in it anywhere. Neither I do in this topic title.
This is esk8 builders forum. Not iron-56 fanpage.
It's nice that you fell in love with iron-56, you can marry with it ( well, in some countries ), you can even buy it in the nearest hardware store if you feel alone... but please, try to keep this discussion on topic. Otherwise a supernova may explode and destroy your iron-56 transformer. I recommend taking a short sleep, ideally on a bed which construction is made out of iron-56 just so you have nice iron-56ish dreams :)
```

---
## \#100 Posted by: devin Posted at: 2017-01-21T21:35:10.555Z Reads: 22

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#101 Posted by: IDVert3X Posted at: 2017-01-21T21:36:12.054Z Reads: 21

```
You can do it.
It's just much less efficient.

Take a look at GreatScott!'s channel on youtube.
He explains it in a quite easy-to-understand way if you have at least som electronics knowledge.
```

---
## \#102 Posted by: Hummie Posted at: 2017-01-21T21:37:26.180Z Reads: 22

```
and why inefficient? just like a coreless motor they are more efficient.  not much power but better efficiency possible.
```

---
## \#103 Posted by: devin Posted at: 2017-01-21T21:37:43.553Z Reads: 21

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#104 Posted by: IDVert3X Posted at: 2017-01-21T21:40:51.359Z Reads: 21

```
Geez, DEVIN!
Have you seen the videos above I posted?

It works without feromagnetic core.
The only thing you need is higher frequency.
You can still add some feromagnetic material to concentrate the field better.
```

---
## \#105 Posted by: Hummie Posted at: 2017-01-21T21:41:25.623Z Reads: 22

```
the losses are largely in the core when there is one.  eddy currents and hysteresis at high frequency.  other than that, if you remove the core you only have copper losses I2r.  

it will be less power without a core though.  every inductive power transfer device I posted doesn't use a core.  Qi will have one on some as more of a shielding similar to a flux ring to keep the field in.
```

---
## \#106 Posted by: devin Posted at: 2017-01-21T21:41:38.722Z Reads: 23

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#107 Posted by: IDVert3X Posted at: 2017-01-21T21:43:43.954Z Reads: 22

```
No. Anything under hundred(s) of kHz won't work very well without feromagnetic core.
```

---
## \#108 Posted by: devin Posted at: 2017-01-21T21:44:03.545Z Reads: 21

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#109 Posted by: IDVert3X Posted at: 2017-01-21T21:44:38.914Z Reads: 19

```
When are you finally going to watch the videos I posted?
They explain all of this!
```

---
## \#110 Posted by: devin Posted at: 2017-01-21T21:45:20.036Z Reads: 19

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#111 Posted by: IDVert3X Posted at: 2017-01-21T21:49:26.850Z Reads: 16

```
Coil is always going to be made out of copper, ideally pure copper.
If you have small frequency, you use feromagnetic core.
Higher frequencies works fine without it, it's just less efficient.
If you learned what I recommended to learn, you would know that.

Also, you can not use the transformer core for the board.
You want it wireless, but the core has to be actually connecting the coils so magnetic flux can flow.
You can place a feromagnetic material behind the coil to improve it's efficienty by concentrating the fields in one direction. 

WATCH THE VIDEOS I POSTED! MOSTOF THE STUFF IS EXPLAINED THERE!
```

---
## \#112 Posted by: devin Posted at: 2017-01-21T21:50:27.719Z Reads: 15

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#113 Posted by: IDVert3X Posted at: 2017-01-21T21:52:11.630Z Reads: 15

```
Geeez.
There is a difference between coil and core material.
Coil is always gonna be copper.
Core is feromagnetic material.
```

---
## \#114 Posted by: devin Posted at: 2017-01-21T21:52:58.656Z Reads: 18

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#115 Posted by: IDVert3X Posted at: 2017-01-21T21:53:50.337Z Reads: 20

```
Yes. Because it is **WIRELESS**.
Or you want huge core going through the board from one coil to the other?
I don't think so.
```

---
## \#116 Posted by: devin Posted at: 2017-01-21T21:55:09.251Z Reads: 20

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#117 Posted by: IDVert3X Posted at: 2017-01-21T21:56:49.385Z Reads: 20

```
That's not how it works. You can't use "feromagnetic" coil and think it will serve as a core.
Nope, it won't.

Core is for "magnetic energy flow".
Coil is for "electric energy" flow.
Two different things.

Watch the two videos I posted.
I asked you to do so many times.
He explains this topic really well.
```

---
## \#118 Posted by: devin Posted at: 2017-01-21T21:59:00.778Z Reads: 20

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#119 Posted by: IDVert3X Posted at: 2017-01-21T21:59:21.295Z Reads: 19

```
There will. You need higher frequency.
It's in the videos too.
```

---
## \#120 Posted by: devin Posted at: 2017-01-21T21:59:57.080Z Reads: 17

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#121 Posted by: IDVert3X Posted at: 2017-01-21T22:00:15.585Z Reads: 17

```
Then you cant do it wireless.
```

---
## \#122 Posted by: devin Posted at: 2017-01-21T22:01:29.360Z Reads: 18

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#123 Posted by: IDVert3X Posted at: 2017-01-21T22:03:35.310Z Reads: 19

```
No.
You need a core connecting these two coils and that's even worse than wire going into the board.

Also, mains AC is not stable. With fixed ratio, this can go seriosly wrong.
```

---
## \#124 Posted by: devin Posted at: 2017-01-21T22:04:42.249Z Reads: 20

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#125 Posted by: IDVert3X Posted at: 2017-01-21T22:05:46.805Z Reads: 23

```
Nope.
For "air core", you need to use different circuit providing high frequency signal to the coil.

IT'S IN THE VIDEO!
```

---
## \#126 Posted by: devin Posted at: 2017-01-21T22:06:43.744Z Reads: 22

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#127 Posted by: IDVert3X Posted at: 2017-01-21T22:07:37.558Z Reads: 24

```
[quote="IDVert3X, post:117, topic:16344"]
That's not how it works. 
You can't use "feromagnetic" coil and think it will serve as a core.
Nope, it won't.
[/quote]

I'm giving up, do whatever you want...
```

---
## \#128 Posted by: Hummie Posted at: 2017-01-21T22:10:39.393Z Reads: 24

```
easiest and maybe also cheapest would be stuff off the shelf
https://www.wirelesspowerconsortium.com/technology/magnetic-resonance-and-magnetic-induction-making-the-right-choice-for-your-application.html<img src="/uploads/db1493/original/3X/4/0/400c5d30e80547acc1cd0c1c861a3cdc5a026469.png" width="354" height="193">

products for sale:
https://www.wirelesspowerconsortium.com/products/search
```

---
## \#129 Posted by: Hummie Posted at: 2017-01-21T22:23:35.768Z Reads: 26

```
what'd you make?
```

---
## \#130 Posted by: captainjez Posted at: 2017-01-21T22:58:45.165Z Reads: 26

```
Our enclosure? It's a glass nylon injection moulded housing for our electronics. Has a double water seal. Hopefully should get us an IP6x rating once we've completed testing.
```

---
## \#131 Posted by: Hummie Posted at: 2017-01-22T01:06:04.674Z Reads: 27

```
i mean I thought you tried some induction charging

@Okami with the super find!
http://www.ebay.com/itm/3-Coils-Qi-Wireless-Charger-PCBA-Circuit-Board-Coil-Charger-Micro-USB-Universal-/371814870913?var=&hash=item5691e4af81:m:m89OAwg0jqu1cfyZbPzhgjw

2$ each for the singles is awesome.
```

---
## \#132 Posted by: captainjez Posted at: 2017-01-22T01:18:51.436Z Reads: 27

```
Right. Oops sorry :) we have been experimenting with induction charging using some custom coils we made from another project. The big problem we've found is the coil
heating up too much when we push the limits of what can be achieved in a small space. We're testing a few other changes over the next few weeks. Happy to share results once we have them.
```

---
## \#133 Posted by: Hummie Posted at: 2017-01-22T01:25:31.734Z Reads: 28

```
what power were you doing and how many coils for the induction transfer?  any pics?!  water cooling :mask: underwater charging.  whats the problem with the heat and what is getting hot?
```

---
## \#134 Posted by: captainjez Posted at: 2017-01-22T01:50:31.401Z Reads: 28

```
We've managed to melt a few coils with testing different charging methods. We're pushing 1-1.5A. One coil at the moment connected into our charging system. I'll dig up some pics when i'm back in the shop.
```

---
## \#135 Posted by: devin Posted at: 2017-01-22T02:18:13.481Z Reads: 36

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#136 Posted by: devin Posted at: 2017-01-22T03:36:45.131Z Reads: 38

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#137 Posted by: mostwanted Posted at: 2018-09-04T12:54:49.822Z Reads: 20

```
so.... any one assembled a complete wireless charging for eboards yet ?

also ; have anyone installed a wireless charging for new smartphones docked on board an electric longboard ever ?

tbh . i would do all those . if only i have time . been busy & absent from all the hype since i've driven for Uber & other ride hailing apps .
```

---

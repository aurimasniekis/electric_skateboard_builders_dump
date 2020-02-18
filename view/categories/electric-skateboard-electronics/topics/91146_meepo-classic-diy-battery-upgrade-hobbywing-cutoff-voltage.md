# Meepo Classic DIY battery upgrade? hobbywing cutoff voltage?

### Replies: 22 Views: 916

## \#1 Posted by: blablubb Posted at: 2019-04-19T19:09:22.530Z Reads: 101

```
The Meepo Classic is sold with either a standard 4Ah 10s2p pack (Samsung 20R, 18650) or an upgraded 8Ah pack (Sanyo 20700). I want to see if I can put together a pack myself that is at least as good as the Sanyo pack. Now I need to decide on 

* What cells to use
* 10s2p or 10s3p
* what BMS to use

I find it difficult to decide on a cell type because I know next to nothing about the hobbywing ESC on the board. The motors are rated at a combined 800W. That should mean I need to supply less that 25A under full load with an empty 10s pack. That number already limits my options for 2p builds. However I cannot find any info on the cutoff voltage of the ESC. My main candidates for cells are 

* Sanyo NCR20700B (4250mAh, 15A discharge) (same as upgraded pack from meepo)
* Samsung INR21700-50E (5000mAh, 10A discharge)

If the cutoff voltage is too high, then the Samsung cell would loose most of its capacity advantage. 

So my main question at the moment is: does anyone know at what voltage the meepo hobbywing ESC stops discharging?
Other cells I should consider? BMS suggestions?
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-19T19:12:47.138Z Reads: 96

```
[quote="blablubb, post:1, topic:91146"]
The motors are rated at a combined 800W. That should mean I need to supply less that 25A under full load with an empty 10s pack
[/quote]

please read

but just because it means your battery can output that much current, it does not mean your esc will use all of the current (esc will take as much as it needs)

for ex i can use a 10s10p with that esc
```

---
## \#3 Posted by: blablubb Posted at: 2019-04-19T19:23:46.428Z Reads: 92

```
my point was that a 10s2p configuration with the -50E (10A max discharge per cell) would already stress the cells beyond spec.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-04-19T19:32:31.552Z Reads: 91

```
the meepo esc draws 24a btw

the esc is configured for liion

30v cutoff i believe, do some reading and you'll find this information
```

---
## \#5 Posted by: Dirt_Bag Posted at: 2019-04-19T21:03:14.418Z Reads: 86

```
I can build you a 10s pack if you want. I use sony vtc5 cells, real world specs are 2500-2600 mah and 25-30a
```

---
## \#6 Posted by: blablubb Posted at: 2019-04-21T21:48:23.081Z Reads: 72

```
@Dirt_Bag 
Thanks for the offer. I really want to (learn to) build this pack myself. Arduino spotwelder is on its way. 

@AlanZhou 
I have seen these numbers (24A max, 30V cutoff) mentioned for the other meepo boards with binary ESCs but I still cannot find anything specifically for the hobbywing ESC in the meepo classic. Still, since they use the same motors and batteries for many of their boards, I will go along and assume that my ESC will at least be very similar if not identical. Armed with this information I can compare discharge curves for my cell options:

Nominal rating
* Samsung INR21700-40T:     4000mAh/35A max. discharge
* Sanyo NCR20700B:             4250mAh/15A max. discharge
* Samsung INR21700-50E:    5000mAh/10A max. discharge

Effective capacity@8A discharge with 30V cutoff (=10s3p config)
* Samsung INR21700-40T:      3600mAh
* Sanyo NCR20700B:              3800mAh
* Samsung INR21700-50E:     4000mAh

Effective capacity@10A discharge with 30V cutoff
* Samsung INR21700-40T:     3550mAh
* Sanyo NCR20700B:              3500mAh
* Samsung INR21700-50E:     3800mAh

Based on these numbers the Sanyo NCR20700B is my choice for a 10s3p pack. It should give similar real world range to the other two options, it is at ~50% max. discharge current when the board is under full load and it is also the cheapest option i could find in europe.

Comments, opinions?

I am still reading through the BMS threads but have not decided yet. HCX-D239 or -D124 seem to be decent options for charge only packs but shipping to europe is expensive.
```

---
## \#7 Posted by: Jeram Posted at: 2019-06-30T16:34:58.684Z Reads: 48

```
 hi I wanted to ask if you ever finish this project if you did can you please explain what you did and how I can do it
```

---
## \#8 Posted by: Jeram Posted at: 2019-06-30T16:38:23.514Z Reads: 47

```
Hi I was wondering how much would it cost to make one of those batteries for the meepo classic I should also let you know that I've changed the HobbyKing ESC for the V2 ESC from meepo
```

---
## \#9 Posted by: Jeram Posted at: 2019-06-30T16:40:02.494Z Reads: 49

```
One question if the ESC is not configured for that battery then it won't work it can start a fire
```

---
## \#10 Posted by: Dirt_Bag Posted at: 2019-06-30T16:54:59.676Z Reads: 49

```
I need to know what type of battery it is. 18650, 20700, or 26650?

What amperage minimum? 
What voltage or cell count?
How many parallel groups?
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-06-30T17:26:11.568Z Reads: 45

```
[quote="Jeram, post:9, topic:91146, full:true"]
One question if the ESC is not configured for that battery then it won’t work it can start a fire
[/quote]

???

it wont start a fire as the components on the board are rated for 63v max, and 50v for the updated version
```

---
## \#12 Posted by: Fiori Posted at: 2019-06-30T17:31:29.538Z Reads: 44

```
All you have to do is make the battery 10s and it will work fine.

edit: I suggest a bluetooth bms: http://shorturl.at/xGI06 . I'd bypass the discharge and just get the smaller 20A one.
```

---
## \#13 Posted by: Jeram Posted at: 2019-06-30T20:20:47.139Z Reads: 45

```
I would like a battery that is as good as the (Sanyo 20700) I'm not sure of the specifics as far (What amperage minimum? What voltage or cell count? How many parallel groups?) I needed to fit the meepo enclosure for my meepo classic I would like a range of 25 miles and I'm not sure if speed has anything to do with the battery but if it does I would like to go at least 30rpm
The Sanyo battery from meepo is $255 and I just don't think that it's worth it so I would like to build in myself but I barely understand how batteries work so if I can have someone build it that would be great
```

---
## \#14 Posted by: blablubb Posted at: 2019-06-30T21:25:53.264Z Reads: 44

```
Hi!

yes, by now my build is finally finished. I had to wait forever until my bms arrived. But I used the battery without bms until then and have used it for about 400km so far. I went for 10s3p with sanyo NCR20700B. This means about 410Wh as compared to the 144Wh from the standard (non-sanyo) meepo pack. In the real world this means I can go for ~25km@30km/h or 35km@20km/h.
My pack is split in two in order to a make use of the existing bolt pattern of the old battery pack. It is effectively a 4s3p in series with a 6s3p.
![20190503_174923|374x500](upload://cxJZYrPaIpptvwqMur79lWOV1bX.jpeg) 

The case is mostly 3d printed with a flat plastic sheet underneath for extra protection.![20190620_164353|375x500](upload://nBBlUbIsnxLk2YZkMG7ExVzaZS0.jpeg) 
I also mounted the trucks below the deck to get some extra clearance. My battery is taller than the meepo case from the original battery. My final clearance is half way between original setup with trucks on top and below deck. In practice I would still like more clearance for cornering over curbs but I like the extra range even better :stuck_out_tongue:
The metal ruler is 4cm wide.
![20190518_124652|666x500](upload://6dFLwWkHAsn68Vgvh3t6kLyDKvl.jpeg) 

Total cost for the battery  was ~200€, BMS was another ~100€ but you could go cheaper(~50€). However I also had to buy a spotwelder (~100€) and already own a decent solder iron, multimeters and other standard tools. If I had to by _everything_ I used in my buld the price would be double. 255€ for the 10s2p meepo upgrade is not cheap, but cells and small charge-only bms alone will cost you 150€ with shipping. Add to that fish paper, nickel strips, silicon wire, fuse, charge port... it all adds up. So if you try to save money you will be hard pressed to stay below 255€  total.
I built it myself because I was interested in the process and techniques. And for that I definitely recommend building your own battery pack. I learned a lot :slight_smile: 
![20190630_231309|375x500](upload://ik7eboo7USKdL2Jg2KhwSy9spVL.jpeg) 

And so far it is holding up well to my abuse.
```

---
## \#15 Posted by: Dirt_Bag Posted at: 2019-06-30T21:55:20.417Z Reads: 41

```
i have to know what specs you are looking for before i can quote you on something
```

---
## \#16 Posted by: Jeram Posted at: 2019-06-30T23:19:57.633Z Reads: 42

```
On your battery ⬇️
What amperage minimum? 
What's voltage ?
What's cell count? 
How many parallel groups?
Please also explain what type of batteries you have
Also please explain what is a BMS for
What type of ESC do you have
```

---
## \#17 Posted by: Jeram Posted at: 2019-07-02T14:51:23.140Z Reads: 37

```
Hey I don't know all the specs but is it possible that you can quote me on how much will it be for a 10s3p with sanyo NCR20700B. 


 would it be possible that you can explain what the BMS do
```

---
## \#18 Posted by: Dirt_Bag Posted at: 2019-07-02T15:14:07.246Z Reads: 36

```
the 20700b is a pricey cell at $5 a piece plus shipping. how big is your enclosure? there are cheaper and better options!

the price would be about $300 usd shipped.

the bms is a "battery managment system". it charges all the cells to the exact same level to prevent dangerous consequences of improperly charging cells.
```

---
## \#19 Posted by: Jeram Posted at: 2019-07-02T16:40:24.158Z Reads: 34

```
![Screenshot_20190702-123010_Samsung%20Internet|281x500](upload://8EYQgXtG58UtOtArfjIJGi8Beyh.jpeg)
```

---
## \#20 Posted by: Jeram Posted at: 2019-07-02T16:59:35.737Z Reads: 29

```
This is the meepo board enclosure I don't really like this enclosure it's too bulky if you can recommend something different that would be great😁🤔

What would be your cheaper better options ?

/also I have a switchblade 38 I would like to turn it into a belt drive motor so I would like the battery to fit better on the switchblade best as possible😁

Will the battery work with the belt drive Motors and hub Motors? 🤯

Do you also install bms's on the battery would that make it more efficient or should I  buy it separate🤔
```

---
## \#21 Posted by: Dirt_Bag Posted at: 2019-07-02T17:15:17.916Z Reads: 29

```
I have a 10s4p sony vtc5 pack ready to ship for $310 usd. It is slightly less than an inch tall. Most enclosures that are ling and short are meant to fit a pack of this size just fine. They are 10.4ah and made with tried and tested great quality cells

https://www.electric-skateboard.builders/t/10s4p-batteries-for-sale-300-usa-only/95677/17
```

---
## \#22 Posted by: Dirt_Bag Posted at: 2019-07-02T17:16:35.417Z Reads: 29

```
Read the post i linked and you will understand more. They have plenty of power for either hub or belt.
```

---

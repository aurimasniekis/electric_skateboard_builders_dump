# Bms just for charging?

### Replies: 20 Views: 3183

## \#1 Posted by: Chris_KP Posted at: 2016-08-13T09:25:06.766Z Reads: 324

```
Im upgrading to an 8s Lipo and Vesc setup soon, as its a higher 6s my Lipo charger wont be up for the job and a bms would be plug and play no hassle to mess with the charger,
I was wondering if it was possible to use a lower amp rated bms but just use it to charge the cells but not discharge through the Bms. 
what are the benifits of discharging through a Bms? and where would be a good place to get one preferably in Australia?
```

---
## \#2 Posted by: Skitzor Posted at: 2016-08-13T09:37:53.042Z Reads: 322

```
I guess the most important advantage from discharging trough a bms is the lifespan of the battery.
```

---
## \#3 Posted by: Hillso Posted at: 2016-08-13T09:39:07.181Z Reads: 317

```
@Skitzor 
Why do you get better lifespan when using BMS for discharging?
```

---
## \#4 Posted by: lox897 Posted at: 2016-08-13T09:52:19.588Z Reads: 315

```
SuPower or Bestech have the best BMSs. Just use the vesc for liniting voltage and amp limit, it should work well. Just wire leads from the battery to bms and battery to esc so you can discharge without going through the bms.
```

---
## \#5 Posted by: Hillso Posted at: 2016-08-13T09:53:44.494Z Reads: 306

```
why waste money on expensive BMS for charge only?
for balance charging, I think this is enough: http://www.aliexpress.com/item/New-Battery-Protection-BMS-PCB-Board-for-10-Packs-10s-36V-Li-ion-Cell-max-30A/32574042165.html?spm=2114.10010108.1000014.5.vyeXWy&scm=1007.13338.33346.0&pvid=5478f37e-a0fb-42e0-80e6-41ad6d222028&tpp=1
```

---
## \#6 Posted by: lox897 Posted at: 2016-08-13T10:04:47.948Z Reads: 295

```
He isn't wasting money. He is buying the cheaper one and discharging straight from the battery.

He is also buying from a reliable and well known BMS maker, not from a place that no one has tested
```

---
## \#7 Posted by: Nordle Posted at: 2016-08-13T10:30:20.216Z Reads: 282

```
There are many guys using this white one, if you search for it there are many folks (including me) using it.
If you bypass discharge there is relly no need for a more expensive one.
```

---
## \#8 Posted by: Chris_KP Posted at: 2016-08-13T10:37:59.444Z Reads: 269

```
And what is this supposed white one called? lol
@lox897 thanks for the second opinion, I have never used a vesc or a bms before, will be a good learning experience :sweat_smile:
```

---
## \#9 Posted by: Chris_KP Posted at: 2016-08-13T10:40:46.645Z Reads: 269

```
do you have experience with buying from battsuports, (buying from aus?)
```

---
## \#10 Posted by: Nordle Posted at: 2016-08-13T11:11:00.007Z Reads: 268

```
Its  the one linked from Hillso above... or didn't you click his link or already forgot it.. lol.. this is no gaming chatroom.. rofl.. lol
```

---
## \#11 Posted by: lox897 Posted at: 2016-08-13T11:40:44.982Z Reads: 260

```
Nope. Shipping from China isn't too expensive though. Buy it on their ebay for cheaper shipping
```

---
## \#12 Posted by: Namasaki Posted at: 2016-08-13T12:17:27.374Z Reads: 253

```
[quote="Hillso, post:3, topic:7587"]
Why do you get better lifespan when using BMS for discharging?
[/quote]
Using the Vesc low voltage limit to protect the battery is false security because it monitors the pack as a whole. One cell could fall too low without tripping the protection thus ruining the pack. 
A BMS on the other hand, monitors each cell individually on a 1p Lipo pack protecting against over discharge and over current.
```

---
## \#13 Posted by: chipoi84 Posted at: 2016-08-13T13:50:37.151Z Reads: 240

```
I'm guessing there is no under-voltage protection if we bypass discharge from the bms?
```

---
## \#14 Posted by: Nordle Posted at: 2016-08-13T13:54:21.931Z Reads: 238

```
right, also there is no over current anymore
```

---
## \#15 Posted by: Namasaki Posted at: 2016-08-13T13:55:41.947Z Reads: 234

```
There is a type of protection from the Vesc and some other Esc's. However it is not cell specific and therefore not 100% reliable.
Well, it's over current protection would be reliable but not the under voltage protection
```

---
## \#16 Posted by: Hillso Posted at: 2016-08-13T20:37:58.204Z Reads: 225

```
I have an idea how to specific cell detection cutoff when using charge only BMS, but it's not the most easy solution.
you connect the discharge port of the BMS to an arduino (through resistors), and use the arduino to command the VESC to do cutoff when the BMS cutoffs its discharge. And than you don't need an high amp BMS.

I'm not sure though the cheap white BMS have specific cell detection for cutoff.
```

---
## \#17 Posted by: Kaly Posted at: 2016-08-13T22:06:20.084Z Reads: 215

```
[quote="Namasaki, post:12, topic:7587"]
Using the Vesc low voltage limit to protect the battery is false security because it monitors the pack as a whole. One cell could fall too low without tripping the protection thus ruining the pack. A BMS on the other hand, monitors each cell individually on a 1p Lipo pack protecting against over discharge and over current.
[/quote]

@Namasaki do not full your self with this argument. 
The way we assemble a battery pack is by joining cells in parallel and them joining this pack of cells in series, when we use a BMS the balance lead of the BMS is attach to a pack of cell to monitor the proper discharge and charge of a PACK OF CELLS. 

Here is the point when we fool out self because the BMS is monitoring a pack not a individual cell, if a cell is to breakdown in this parallel pack the BMS we currently use will not notice it or even more let us know that this Happened. 

So the uncertainty factor is always present in a small pack like the ones we use and the probability against the over discharge of a cell are basically the same when the BMS or the VESC are controlling the discharge of the pack. 

IMO is better to buy a less expensive BMS and use the money to get better cells or more cells and building a more robust battery pack.
```

---
## \#18 Posted by: Hillso Posted at: 2016-08-13T22:31:37.131Z Reads: 199

```
@Kaly
The cells that are connected in parallel balance themselves.
And in series the BMS does detect individual cells as Namasaki said.
 
I sort of agree about you conclusion.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-08-13T22:55:01.768Z Reads: 202

```
I think you misunderstood my point. 
I was refuring to a 1p Lipo pack having its cells individually monitored by the BMS. And normally, if you kill 1 cell in a Lipo pack, you trash the whole pack.  I understand the difference when using a BMS with a multiple parallel Lion pack. 
Each cell that is in parallel wether 2,3 or 4p is seen as 1 cell by the BMS. Since every cell in a parallel group will equalize themselves and deplete evenly, the whole parallel group will drop below the limit and trigger the BMS protection saving the entire pack. ( as I stated before, I have proven this theory)
If you rely only on the Vesc low voltage protection, your pack could be damaged before it is tripped seeing that it monitors all groups of cells as 1. 
And from what I've seen, cells in series do not equalize, only the cells in parallel do. 
So imo, it's still better to invest in a good BMS rather than spend all the money on a huge battery pack that you could end up damaging.
```

---
## \#20 Posted by: Kaly Posted at: 2016-08-13T23:45:57.959Z Reads: 198

```
[quote="Namasaki, post:19, topic:7587"]
I think you misunderstood my point. I was refuring to a 1p Lipo pack having its cells individually monitored by the BMS
[/quote]

It look like I misunderstood :-) 
if it is for a 1P Lipo battery pack them the use of BMS is more relevant to discharging. 

To the other point I was referring, even if the parallel pack balance it self if there is a defective cell in this pack it will take that pack down with it and there's not much that the BMS can do.
```

---

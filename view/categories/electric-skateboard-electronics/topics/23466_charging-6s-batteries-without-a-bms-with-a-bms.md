# Charging 6S+ batteries WITHOUT a BMS/ WITH a BMS

### Replies: 10 Views: 1232

## \#1 Posted by: Print3r Posted at: 2017-05-19T13:45:03.658Z Reads: 164

```
I have seen other threads about balance charging 6S+ packs in parallel, but have not seen any that disconnect the positive power from the VESC whilst charging - the motors would still be able to spin?

I have made a diagram of the setup I am thinking of making and was wondering what everyone thinks of it. 

My build is going to be a 10S4P pack (limited to 50A output), split into two 5S4P packs. The balance wires will be connected in parallel when charging, but not whilst riding. My current battery setup diagram idea:<img src="/uploads/db1493/original/3X/2/f/2f781b872855255ea7ffa0bd1fcdc0613d52f314.png" width="665" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2017-05-19T13:51:20.357Z Reads: 146

```
[quote="Print3r, post:1, topic:23466, full:true"]
The balance wires will be connected in parallel when charging, but not whilst riding.
[/quote]

impossible

Edit: or do you mean you only connect them together when you have switched from series to parallel but leave them completely separate as 5S until then?
```

---
## \#3 Posted by: lowGuido Posted at: 2017-05-19T13:55:41.135Z Reads: 139

```
that looks like a very complex solution to a simple problem.
I do apreciate the thought that you have put into it though. very clever.
```

---
## \#4 Posted by: Print3r Posted at: 2017-05-19T14:14:49.916Z Reads: 135

```
I will only connect them in parallel when charging - if connected in series, you get a heater/ fireworks/ magic smoke!
```

---
## \#5 Posted by: PXSS Posted at: 2017-05-19T14:15:52.661Z Reads: 125

```
Plugging the connector to the parallel only charges one battery.
```

---
## \#6 Posted by: Print3r Posted at: 2017-05-19T14:17:44.582Z Reads: 114

```
I don't see how to make it simpler - without loop key 1 it is very similar to a design in a similar thread but the motor would still be able to spin when the batteries are charging as the VESC has a positive and negative connection.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-05-19T14:21:19.476Z Reads: 108

```
just charge through the balance leads.
```

---
## \#8 Posted by: Maxid Posted at: 2017-05-19T14:28:09.598Z Reads: 100

```
Why go for a solution where you have to plug several plugs everytime plus need to make sure the order is correct when you could also just charge them separately one after the other?
```

---
## \#9 Posted by: Print3r Posted at: 2017-05-19T16:20:11.644Z Reads: 94

```
Because the charger I will use has the power to charge at a power of up to 500W, which is the normal charging speed for the A123 cells I will be using. I may just use this BMS  (https://world.taobao.com/item/21608808908.htm?spm=a312a.7700714.0.0.a5w3ik#detail) ... if anyone knows chinese please explain to me what it says as google translate is awful. With the BMS, how do you bypass it for discharging. I am perplexed by connecting balancing wires to a spot - welded battery packs as the point of spot-welding is to not heat the cells too much and soldering wires onto the zinc will pass lots of heat to the cells no?
```

---
## \#10 Posted by: Print3r Posted at: 2017-05-19T18:35:22.428Z Reads: 87

```
Found a bms for lifepo4 batteries (which I will be using) - https://www.aliexpress.com/item/8S-50A-LiFePO4-3S-to-16S-BMS-PCM-PCB-battery-protection-board-for-8-Packs-18650/32711144931.html. What are your thoughts on using that bms, considering I am going to charge it using this buck converter (http://www.ebay.com/itm/131925513356).
```

---

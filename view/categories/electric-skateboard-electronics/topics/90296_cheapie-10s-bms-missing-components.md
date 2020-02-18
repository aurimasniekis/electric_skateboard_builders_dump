# Cheapie 10S BMS missing components

### Replies: 9 Views: 318

## \#1 Posted by: Bataleon Posted at: 2019-04-12T21:26:27.758Z Reads: 96

```
So I cheaped out and bought [this 10S BMS](https://www.aliexpress.com/item/10S-36V-Li-ion-Lithium-Cell-40A-18650-Battery-Protection-BMS-PCB-Board-Balance/32697273276.html) to use for charge-only. I just noticed a few reviews saying that it’s missing a diode, leading to the first cell not being balanced correctly.

Has anybody here used this BMS before and is it known to have issues? Thanks

![10s-bms|539x500](upload://f6z0eTSnFKuyYG4Q9YYchhoVOjh.jpeg)
```

---
## \#2 Posted by: FullMetal_Machinist Posted at: 2019-04-13T06:35:27.187Z Reads: 78

```
I have checked marking codes (thanks for high quality photo) and missing element should be BAW56 dual diode.
From my perspective (proffesional elecronican) it should be there.
Photos on their selling website also have this diode missing.
If several people reported cell 1 not balancing correctly then it is a no-brainer to solder this missing component.
```

---
## \#3 Posted by: Bataleon Posted at: 2019-04-13T07:25:43.690Z Reads: 76

```
Thanks for the info and identifying the component. It's so strange that every place I find the BMS for sale, the photos are missing the dual-diode. Almost as if the factory made 100 000 of them, then only realised their mistake.

I would also expect most BMSes to have a micro-controller of some sort? Maybe that's why it's selling for so cheap. Lesson learned.
```

---
## \#4 Posted by: FullMetal_Machinist Posted at: 2019-04-13T07:49:27.896Z Reads: 75

```
This is the simplest BMS possible, 100% analog circuitry.
In most cases there is some digital MCU, but then it wont sell for $8.
However this is still good enough for simple protection.
Manufacturer mistake is 100% possible - 2 weeks ago i was fixing similar mistake on a 2500 pcs batch of PCBs for one of my customers - he put incorrect value of one component and realized it after batch was done.
If they realized then they should fix it - in some cases it can slip through without noticing.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-15T00:53:33.054Z Reads: 50

```
it actually seems like it might be normal, as in every youtube video and ebay picture that dual diode is missing and 4 of my bms have the missing diode too.
```

---
## \#6 Posted by: b264 Posted at: 2019-04-15T01:04:04.300Z Reads: 46

```
While I don't have any advice or knowledge of this specific cheap BMS -- because I avoid cheap BMSs -- I can say that in electronics design in general, missing components are super-common and almost always benign.  Almost every device has at least one.  But, I don't know anything about this specific unit.

Even FOCBOX 1.7 has a blank.
```

---
## \#7 Posted by: Bataleon Posted at: 2019-04-15T11:36:15.987Z Reads: 36

```
[quote="AlanZhou, post:5, topic:90296, full:true"]
it actually seems like it might be normal, as in every youtube video and ebay picture that dual diode is missing and 4 of my bms have the missing diode too.
[/quote]

I wouldn't have worried but there are quite a few reviews on the AliExpress listing (linked above) which say the first cell doesn't balance correctly because of the missing component :confused:

Which model BMSes of yours are missing similar components? Do they balance all the cells correctly?
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-15T11:49:22.281Z Reads: 32

```
IDK previous attempts have caused failed packs but that might be my fualt
```

---
## \#9 Posted by: gmurad Posted at: 2019-05-27T21:21:10.654Z Reads: 16

```
@Bataleon oh too bad! I was about to buy this BMS because it's available with prime shipping here in Canada.
```

---

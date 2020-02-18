# Do I understand electronics correctly? + questions

### Replies: 6 Views: 393

## \#1 Posted by: karosass1 Posted at: 2017-06-14T11:25:26.480Z Reads: 73

```
I just want to sum up my knowledge and for somebody to confirm/deny it.

**Battery**

* XsYp - X̶ ̶a̶m̶o̶u̶n̶t̶ ̶o̶f̶ ̶c̶e̶l̶l̶s̶ ̶p̶e̶r̶ ̶p̶a̶c̶k̶ ̶Y̶ ̶p̶a̶c̶k̶s̶ ̶i̶n̶ ̶p̶a̶r̶r̶a̶r̶e̶l̶.̶ ̶e̶.̶g̶.̶ ̶1̶0̶s̶3̶p̶ ̶1̶0̶ ̶c̶e̶l̶l̶s̶ ̶i̶n̶ ̶p̶a̶c̶k̶,̶ ̶3̶ ̶p̶a̶c̶k̶s̶,̶ ̶3̶0̶ ̶t̶o̶t̶a̶l̶ ̶c̶e̶l̶l̶s̶.̶
X amount of cells in series (that's what the "s" stands for), Y amount of cells in parallel so 10s3p is 30 cells, 10 in series, 3 in parallel

**BMS**

* Keeps the level of multiple batteries the same.
* Is n̶o̶t̶ involved in battery charging
* Is **not** ok to use multiple ones, e.g. 2x6s bms for 12s battery
* Specific smart bms can use higher one on smaller battery, e.g. 10s bms on 6s battery

**Charger**

* Y̶o̶u̶ ̶n̶e̶e̶d̶ ̶b̶a̶l̶a̶n̶c̶e̶ ̶c̶h̶a̶r̶g̶e̶r̶ ̶f̶o̶r̶ ̶m̶u̶l̶t̶i̶p̶l̶e̶ ̶l̶i̶p̶o̶s̶ ̶i̶n̶ ̶s̶e̶r̶i̶e̶s̶,̶ ̶c̶h̶a̶r̶g̶i̶n̶g̶ ̶t̶h̶e̶m̶ ̶a̶l̶l̶ ̶a̶t̶ ̶o̶n̶c̶e̶.̶ ̶Y̶o̶u̶ ̶n̶e̶e̶d̶ ̶b̶a̶l̶a̶n̶c̶i̶n̶g̶ ̶w̶i̶r̶e̶s̶ ̶c̶o̶n̶n̶e̶c̶t̶e̶d̶ ̶a̶s̶ ̶w̶e̶l̶l̶.̶
You can use bms + power brick to charge lipo batteries. Or lipo alarm and balance charger.

**Misc** 

* You need antispark switch/anti spark loop key to avoid damage on connector And to avoid current rush that can destroy components.

Anything else to add to these? 
Thanks.
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-06-14T11:34:24.238Z Reads: 65

```
**Battery** 

XsYp - X amount of cells in series (thats what the "s" stands for), Y amount of cells in parallel so 10s3p is 30 cells, 10 in series, 3 in parallel

**BMS**

* keeps the level of cells correct
* it is involved in battery charging and discharging but can be bypassed for discharging
* no, there should only be one bms to keep everything leveled
* normaly not, but there are some smart bms out there that are able to use a range of cells like 7s - 13s BMS

**Charger**

You can use a BMS to charge and a laptop style charging brick, or you use a lipo alarm and a balance charger.

**Misc**

Antispark should be used to avoid high inrush currents to destroy your components
```

---
## \#3 Posted by: karosass1 Posted at: 2017-06-14T11:48:04.971Z Reads: 51

```
Edited my post. Can you direct me to some material related to bms charging? Thanks.
```

---
## \#4 Posted by: Smorto Posted at: 2017-06-14T16:48:59.759Z Reads: 39

```
[quote="karosass1, post:1, topic:25359"]
10 in series, 3 in parallel
[/quote]

Just to clarify more, a 10s 3p would normally be 10 packs of 3 cells in parallel, then those 10 sets are connected in series.

Something to add would be what the C rating of a pack means. The C rating is the amperage that the pack is able to deliver and you get to that answer by doing the **Ah** of the pack **times the C rating**. So a 5000mah 20c pack can deliver 100A (5*20=100).
```

---
## \#5 Posted by: Maxid Posted at: 2017-06-14T16:54:10.215Z Reads: 36

```
A BMS with 18650 Liion is not crucial to have.
You can charge without one.

Also I have seen BMSs connected in series - but that is unusual.
```

---
## \#6 Posted by: Davey Posted at: 2017-06-14T17:30:38.653Z Reads: 30

```
The misc part is right, but I use my board without a switch, so plugging and unplugging every time without any problems about half a year now. A loop key/switch is very nice to have, but not really necessary in my experience.
```

---

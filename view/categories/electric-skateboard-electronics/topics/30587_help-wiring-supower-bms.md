# Help wiring supower BMS

### Replies: 11 Views: 886

## \#1 Posted by: cryo Posted at: 2017-08-14T14:50:11.314Z Reads: 89

```
Hey all, my BMS arrived today and I almost have the wiring down but still got a few questions. 
I'm gonna run two lipo packs 5s1p 8000mAh 30c in series. 
Using [this](http://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System/221769582503?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649) BMS.

Gonna take @mmaner's pretty diagram and follow it. 
https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/3/e3796b0f060e303194ee50955916020ecb61ab9c_1_294x500.jpg

1) In the diagram, he has the battery packs positive and negative terminals switched. That is, the right packs positive wire ends up being the negative while the negative wire from the right pack becomes the systems positive wire. Is this correct or should I flip them so that they match accordingly?

2) In @oriol360's setup I understand he uses the left packs balance negative wire as the fourth cell of the other battery, but he also connects both the right batterys balance negative and main negative into the BMS B-. Why does he do this? Do I need to do this too, if I follow my own diagram? 
https://www.electric-skateboard.builders/uploads/db1493/optimized/2X/b/b338e047fd119998805580ce40fefd06ffde0e7c_1_375x500.jpg
```

---
## \#2 Posted by: mmaner Posted at: 2017-08-14T15:21:26.186Z Reads: 79

```
[quote="cryo, post:1, topic:30587"]
I'm gonna run two lipo packs 5s1p 8000mAh 30c in series
[/quote]

This is a diagram for a 6S setup, not a 10s.  Use this one instead as the balance leads will be the same...

<img src="/uploads/db1493/original/3X/0/5/05707bcd45a99ea84365374ea2af659ebd279c76.jpg" width="207" height="500">



[quote="cryo, post:1, topic:30587"]
In the diagram, he has the battery packs positive and negative terminals switched. That is, the right packs positive wire ends up being the negative while the negative wire from the right pack becomes the systems positive wire. Is this correct or should I flip them so that they match accordingly?
[/quote]

I don't understand what you are saying, but the diagram is technically correct, just follow the color codes and yo will be fine.
```

---
## \#3 Posted by: cryo Posted at: 2017-08-14T15:28:52.011Z Reads: 74

```
I know the diagram is for 6s but it should still work right? Only difference is I have 4 extra balance wires to plug in.

And I meant these connections

<img src="/uploads/db1493/original/3X/1/6/1608b67afb46cfd1edeaf76eca9918c3616d1596.jpg" width="294" height="500">

red going into black and vice versa. It looks weird, not sure if its intended or if its a mistake.
```

---
## \#4 Posted by: mmaner Posted at: 2017-08-14T15:48:22.918Z Reads: 67

```
Yes just extra balance leads, you would be better off using the diagram I posted earlier, it has the balance lads in order.  

I don't see red going to black.  I see the POS lead going to the charge port and to the ESC and NEG lead going to the BMS the to the charge port and ESC.
```

---
## \#5 Posted by: cryo Posted at: 2017-08-14T15:52:54.172Z Reads: 65

```
The POS lead is connected to the negative lead from the left battery. 

The NEG lead is connected to the positive from the right battery. 

I circled it in purple. Just want to make sure that is intended.
```

---
## \#6 Posted by: mmaner Posted at: 2017-08-14T15:54:25.443Z Reads: 62

```
Ahhhh, i see that now, right by the battery before the 5.5mm connector.  I dont know how I missed that.  The connector color is what you should pay attention to,
```

---
## \#7 Posted by: cryo Posted at: 2017-08-14T15:59:37.266Z Reads: 64

```
So just to confirm I should connect the left battery POS and right battery NEG to their respective colored connectors right?

Sorry if im being difficult, its my first build and I just want to make sure I get everything correct.
```

---
## \#8 Posted by: mmaner Posted at: 2017-08-14T16:03:05.509Z Reads: 63

```
That is correct.  Here's a corrected diagram.

<img src="/uploads/db1493/original/3X/0/f/0f4242677322586596a6d6761798ba9866de0ef0.jpg" width="294" height="500">
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-14T16:05:20.996Z Reads: 57

```
Make sure you measure the balance header with a multimeter before plugging anything in. Very easy to blow out your BMS with the wrong balance order/voltages.
```

---
## \#10 Posted by: cryo Posted at: 2017-08-14T16:21:11.948Z Reads: 53

```
@mmaner Thanks so much. Feel confident enough that I wont fry anything now :laughing:.

@jinra yup. plan on using a multimeter to check voltages are sequential. If I have the order correct, I can plug in all 10 at once right?
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-14T16:24:53.990Z Reads: 54

```
yep, just triple check everything. These things are sensitive..
```

---

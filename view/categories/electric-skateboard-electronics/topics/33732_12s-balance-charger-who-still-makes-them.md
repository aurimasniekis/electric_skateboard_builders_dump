# 12S balance charger \[who still makes them?\]

### Replies: 14 Views: 4729

## \#1 Posted by: gogomrrobot Posted at: 2017-09-22T20:22:32.974Z Reads: 341

```
I looked around for a while for a 12s balance charger for my 12s4p lithium ion pack I am building and many claimed they are too expensive, etc.  I found one on Amazon for $200. It will be back in stock on 9/26/2017.

https://www.amazon.com/EV-PEAK-Battery-Balance-Charger-connector/dp/B01D4PORJW?SubscriptionId=AKIAJD63CH47PFCH325Q&tag=dronesrc-20&linkCode=xm2&camp=2025&creative=165953&creativeASIN=B01D4PORJW

I have to make a diagram but I guess the way this works is to split the +/- leads coming from the 12s4p battery pack and wire one set of +/- to an XT90 connector and that will serve as the charge port? Then also use a 12S balance leads cable for the balance port on the charger.  The other +/- leads would be connected into an antispark heading to the VESC/motors. Obviously, no BMS.

1) Is that the correct wiring?

2) Are there any other 12S balance chargers out there? I saw some from years ago but they are no longer made. I don't know why it's like that.

The solution doesn't seem more expensive than a BMS ($43) + 12s charger brick ($55) from batterysupports which costs about $65 shipping via UPS/Fedex.  So $200 vs $165 and you don't have an annoying and space consuming BMS to deal with. Also, over time I read articles that the BMS will reduce the life of your batteries anyways.
```

---
## \#2 Posted by: Cobber Posted at: 2017-09-22T22:03:28.716Z Reads: 309

```
I have this [8s icharger 308 duo](http://www.icharger.co.nz/icharger-308-duo)
but they make a [12s version](http://www.icharger.co.nz/icharger-4010-duo)

<img src="/uploads/db1493/original/3X/d/2/d2f701aecec8518bbe4c961816d5e592c3da13fa.png" width="660" height="464">

bit more expensive but has cool features and charges two batteries at once :sunglasses:
```

---
## \#3 Posted by: gogomrrobot Posted at: 2017-09-22T22:48:23.096Z Reads: 286

```
Well that one you linked is $385!

Also, when I click on the link and see the description : "Lithium (LiPo/Lilo/Life) Battery Cell Count: 1-10 series (Per Channel)"

So I think it is only 10S.  There must be a reason why 12S balance chargers aren't around. I just never got into the RC hobby scene enough to know the details.
```

---
## \#4 Posted by: pat.speed Posted at: 2017-09-22T23:21:10.452Z Reads: 264

```
Try having a look for a dual 6s charger then just split the balance leads into to 6s ones and plug them in
```

---
## \#5 Posted by: Cobber Posted at: 2017-09-22T23:23:30.432Z Reads: 258

```
yeah you are right, it can charge 2 x 10s at once though. I do 2 x 7s packs at once with mine. They show you a readout of each cell, you can adjust end of charge voltage and all kinds of stuff... data logging...
```

---
## \#6 Posted by: SilentException Posted at: 2017-09-23T00:18:44.755Z Reads: 255

```
1. Yes

2. They are pretty rare indeed. [Chargery](http://chargery.com/balanceCharger.asp) should have their 12s balance charger ready in some time (shoot them email). 50012B model. Other than that, I don't know of any other.
```

---
## \#7 Posted by: gogomrrobot Posted at: 2017-09-23T00:32:43.459Z Reads: 253

```
@SilentException  Will have to wait until that comes out.

@pat.speed That wont work with the (2) 6S balance leads. Because it will expect in addition to the (2) balance leads... (2) XT-90 or XT-60 connections. But I only have a single xt60/xt90 connection coming out of my pack.  What you are talking about is a more complex split circuit which seems difficult -- at least for my electrically challenged brain..lol, I get series and parallel but there are a complex splits to break a 12s into (2) 6s circuits.

See this thread:  http://www.electric-skateboard.builders/t/series-and-parallel-skateboard-circuits/12618
```

---
## \#8 Posted by: pat.speed Posted at: 2017-09-23T00:36:27.559Z Reads: 236

```
Yes you would need three Xt-60 or 90. If you have a look at @lowGuido YouTube channel he makes a video of how to charge a pack like I am talking about. I will try and find the link for you
```

---
## \#9 Posted by: pat.speed Posted at: 2017-09-23T00:40:26.440Z Reads: 233

```
Here you go, he has lots of useful videos

https://m.youtube.com/watch?list=PLNrR_HHwHVPC8CjfwVUQLDByoNcSyTUa9&v=O5gi35AtPSw
```

---
## \#10 Posted by: gogomrrobot Posted at: 2017-09-23T00:41:35.290Z Reads: 220

```
Thanks will take a look
```

---
## \#11 Posted by: Inwo Posted at: 2017-12-11T06:15:57.408Z Reads: 195

```
C4012b from chargery.
40amp 12s ac charger. Nothing else like it.
I will have the beta model later this week.


C606B/C4012B main spec. is as below,

1.                     Input: 100-265Vac 18A max. and 10-30V DC 25A max.

2.                     Battery type: 1-12S lipo, liFe, Lion, Nimh/NiCd, Pb for C4012B,  1-6S lipo, liFe, Lion, Nimh/NiCd, Pb for C606B

3.                     Charge current: 1-40A for C4012B, 1-60A for C606B,  1500W max. at AC input, and 500W max. at DC input.

4.                     Discharge current:0.1- 40A 100W max.

5.                     Balance current:1.2A per cell

6.                     IR impedance detection,

7.                     USB update

8.                     LCD display

9.                     The size is 278*175*68mm

10.                  Weight is 2.5kg without input cable.

11.                  One knob button and one small key set up parameters

12.                  Two 7 pin balance socket used in two battery connection in series, such as first 3S connect to socket 1, and second 3S connect to socket 2.  One 7pin balance socket for C606B

13.                  Special adapter board prevent two battery from short circuit when reverse connection.

14.                  Protection on output

l  Over voltage protection

l  Over current protection

l  Over temperature protection when AC charge, DC charge and balancing

l  Over temperature protection when battery temperature over setup

l  Over power protection

l  Short circuit protection

l  Anti spark when battery connection

l  Battery Reverse polarity protection

l  Under voltage protection, when pre-charge fail

15.                  Two power leads connect to battery pack when charge and discharge

16.                  One balance wire and adapter board connect to battery balance wire ( similar 9pin wire on BMS)

17.                  Two C4012B charge 24S battery, the output must be isolated.
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-12-11T06:22:18.597Z Reads: 171

```
Thunder power 1430
```

---
## \#13 Posted by: jrpwit Posted at: 2017-12-11T06:44:04.363Z Reads: 168

```
<img src="/uploads/db1493/original/3X/d/a/da25d07358e18c9e1698aa97c5062466edebd5c0.jpg" width="281" height="500">
I have this charger I got for free last week. It is basically two 6s chargers in one. Have only used it to charge two 3s lipos so far so I don't know how good it is but it works and is not too expensive.
https://m.banggood.com/Ultra-Power-UP100AC-DUO-100W-LiPoLiFeNiMH-Battery-Balance-Charger-Discharger-p-1042945.html?gmcCountry=US&currency=USD&createTmp=1&cur_warehouse=CN&utm_source=googleshopping&utm_medium=cpc_ods&utm_content=heath&utm_campaign=pla-heli-us-m&gclid=CjwKCAiA07PRBRBJEiwAS20SIG4xlhJfcIOm6PL3ZPwCr4rWsmzt0QaRpzZFH-SnTAEURwgTe2YZ2xoCHZUQAvD_BwE
```

---
## \#14 Posted by: drone001 Posted at: 2019-07-29T00:25:14.099Z Reads: 28

```
how would you use a 6s charger to charge a 12s battery. the plug has 13 wires on a 12s battery.
```

---

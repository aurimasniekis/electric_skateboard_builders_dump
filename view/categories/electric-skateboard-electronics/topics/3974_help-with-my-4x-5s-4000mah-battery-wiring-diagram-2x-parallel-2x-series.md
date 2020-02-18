# Help With My 4x 5s 4000mah Battery Wiring Diagram (2x parallel + 2x series)

### Replies: 7 Views: 1846

## \#1 Posted by: nfed163 Posted at: 2016-05-29T14:15:08.544Z Reads: 207

```
Let me know if you see any problems with this wiring diagram. I am very new to this but I figured I would try to draw something up as a starting point. Is it correct to run the batteries in parallel first and then series or does this not matter?

Do I need a banana plug in the first diagram or could I just cut it out and plug the top black wire directly from the top xt60 to the bottom xt60?

Sorry its not very pretty.

<img src="/uploads/db1493/original/2X/4/453995b25bf4388cd0f43a5aa0db8fea4ad50860.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/b/bb1965c2523c87a4cf05b2fc5a6e479685795a77.jpg" width="690" height="388">

[The Charger I Plan to Use](http://www.amazon.com/Genuine-SKYRC-Power-6Amps-50Watts/dp/B00ND7J38C/ref=sr_1_1?s=toys-and-games&ie=UTF8&qid=1464529414&sr=1-1&keywords=imax+b6ac)

[The Balance Board I Plan to Use](http://www.amazon.com/WOOCON%C2%AE-Parallel-Balance-Charging-Adaptor/dp/B01BAEFEEQ?ie=UTF8&keywords=lipo%20balance%20board%20xt60&qid=1464529100&ref_=sr_1_4&sr=8-4) (Why is there a male deans plug on top of this the board?)
```

---
## \#2 Posted by: nfed163 Posted at: 2016-05-29T16:26:39.316Z Reads: 174

```
[The 5s2p 4000mah 15C Batteries I Plan to Use](https://www.commonsenserc.com/product_info.php?products_id=101) (I accidentally wrote 4s 4ah on the diagrams)
```

---
## \#3 Posted by: Namasaki Posted at: 2016-05-29T22:38:41.885Z Reads: 157

```
The batteries look cool however, they are only 15c which is low for a 4000mah battery.
Of course running them in parallel will help making them effectively 8000mah and capable of 120a continuous.
The problem with the charging diagram is that you'll be charging in parallel and doing that can be a bloody nightmare.
I would not recommend charging lipos in parallel under any circumstance. It would be safer to charge each pack separately. Every lipo cell will have a different internal resistance so even in a single pack the cells will not discharge and charge at exactly the same rate. This is why they have to be balance charged. Trying to balance charge in parallel just defeats the purpose because the charger you mentioned can only balance up to 6 cells at a time. in order to parallel charge, all cells would need to be perfectly matched in terms of internal resistance and would need to be pre-balanced before charging. This is just not going to happen. your either going to under charge some cells or overcharge some which can be very dangerous.
```

---
## \#4 Posted by: nfed163 Posted at: 2016-05-30T02:30:52.617Z Reads: 137

```
Hmmm, yea that makes sense...

If the charger can only balance 6 cells at a time would it even work to charge one of these batteries? They are 5s2p batteries which means 10 total cells. 

These batteries are also already in parallel so would they charge unevenly for the same reason even if I am only charging one of them at a time?

What if I used a [Battery discharger/balancer](http://www.amazon.com/Tenergy-Intelligent-Capacity-Discharger-Resistance/dp/B0178P8H9U/ref=sr_1_3?s=toys-and-games&ie=UTF8&qid=1464538701&sr=1-3&keywords=battery+medic)? Could this balance out parallel cells?

I'm kinda leaning towards just getting a couple 5s 5000mah 20c Zippy batteries instead...
```

---
## \#5 Posted by: Namasaki Posted at: 2016-05-30T03:20:11.807Z Reads: 130

```
I would highly recommend that you get the 5s/5000/20c zippys instead of those other batteries.
then you can easily hook them up in series for 10s and disconnect them for charging. You can even get a dual bank charger and charge both packs at the same time balancing them individually.
hobby king also has Zippy compacts in 5s/5800/25c and 4s/5000/25c
http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=21382
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idproduct=21371
```

---
## \#6 Posted by: Tijmen Posted at: 2016-09-05T08:57:45.353Z Reads: 99

```
I want to wire 4 3S LiPo's together. 2 in series 2 in parallel. Don't want to have to take the batteries out of the box and plug them into a balance board whenever I need to charge. Anyone have a diagram on how I'd wire that? Including balance leads
```

---
## \#7 Posted by: Waynca Posted at: 2019-01-23T14:48:51.657Z Reads: 24

```
Yeah, rly, make sense.
```

---

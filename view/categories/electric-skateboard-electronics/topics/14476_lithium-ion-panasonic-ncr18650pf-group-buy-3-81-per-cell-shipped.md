# Lithium Ion Panasonic NCR18650PF Group Buy 3.81 per cell shipped

### Replies: 48 Views: 2751

## \#1 Posted by: jbruce Posted at: 2016-12-10T20:15:56.261Z Reads: 172

```
Hey Guys,
So I'm new to E Boards and have lately been using lipos on my board, but wanted a longer range and more reliable battery, so I've decided to make a lithium ion battery pack for my board and am planning on using the Panasonic NCR18650PF cells. My configuration will be 6s6p with a total of 36 cells and about a 390Wh rating. These cells are rated at 2900 mAh and 10A discharge rate. [Here](https://industrial.panasonic.com/cdbs/www-data/pdf2/ACA4000/ACA4000C50.pdf) is the spec sheet. The cheapest place I can find them is from [battery bro](https://batterybro.com/products/panasonic-pf-ncr18650pf-2900mah-10a) for a quote of 3.27 per cells for 50 cells, but with a 95$ shipping fee!!!!<img src="/uploads/db1493/original/3X/3/4/34bbc9085398e762134f8efa0bbde48b9e061ee3.JPG" width="690" height="438"><img src="/uploads/db1493/original/3X/1/8/18064416bb6265d3f110470456a85955ae364818.JPG" width="690" height="280"> So I got to thinking and thought a group buy would be the perfect thing because shipping for 200 cells would be 173$(43$ per 50 cells rather than 95$) and the per cell price would be much cheaper at 2.95 per cell.<img src="/uploads/db1493/original/3X/8/2/82073eb21d19f6d5483b5d28002dfc36dc6e2449.JPG" width="675" height="500"><img src="/uploads/db1493/original/3X/d/2/d2c1c515a98406ad386d7aaf156c1b1f56578690.JPG" width="690" height="273"> This would mean for 50 cells it would cost $147.5(50x2.95) + 43.25(173/4) = $190.75 or just 3.81 per cell with shipping price included. Of course there would be a shiping price from my house to yours(I live in California so that would change depending on where you live), but I don't expect that to be anywhere near what it would be directly from Hong Kong. That's a pretty great deal in my opinion. Earlier I asked the lady who was giving me the quotes if a group buy would be possible where she sent each package of 50 cells to a different address and she said yes it would be possible, but the shipping price would be tremendous at $95 per person. She even recommended one person purchase them and then distribute them. So that is my plan. I want to get the pretty cheap price of 3.81 per cell and need 3 other people that also want 50 cells or 5 others that want 30 etc etc, you guys get the gist. I wouldn't call this a full on group buy because its really limited to 3-5 people, but I guess if enough people want these we could go up to the 500 cell price(I don't even know what it is yet), but that would make it cheaper for everyone. One last thing to address is that I am relatively new to the E skate community and understand nobody knows much about me, thus trust is an issue. I am guaranteeing to be honest with everything and am not planning to make a profit but I completely understand if someones been scammed before and doesn't want to risk it. Thus if this becomes a full fledged group buy with 10+ people in it, I am fine to pass it off to someone more trustworthy in this community who has done this before, I just want to get these cells for cheap. Let me know if this interests any of you. Thanks! :slight_smile:
```

---
## \#2 Posted by: Sander Posted at: 2016-12-12T17:02:21.259Z Reads: 100

```
Cool! But I have one question for you...
Do you know how much I can draw from my batteries?
They are cell 18650. 12s4p.
﻿Max. discharge current: 20A
Nominal capacity: 3000 mAh
Nominal voltage: 3.6 V

So to find out how much ampere I can draw?
Is the formel like this:
Max amp * Parallell
20 * 4 = 80 Amp
So my max is 80 Amp?
```

---
## \#3 Posted by: jbruce Posted at: 2016-12-12T17:11:10.503Z Reads: 93

```
Yes, for battery packs it would be 
(Max amperage per cell) x (number of cells in parallel)= max amperage you can draw
For these cells that are rated at 10A each, a 12s4p pack would be able to deliver 43.2v(3.6 x 12)nominal at 40Amps(10 x 4 cells in parallel). That's should be plenty for most setups.
```

---
## \#4 Posted by: jbruce Posted at: 2016-12-12T17:12:57.635Z Reads: 88

```
If you have batteries that are rated at 20A and are using 12s4p then you are correct that you could draw 80A
```

---
## \#5 Posted by: Sander Posted at: 2016-12-12T17:14:41.668Z Reads: 83

```
[quote="jbruce, post:4, topic:14476"]
u have batteries that are rated at 20A and are using 12s4p then you are correct that yo
[/quote]

Thank you! I thought so :slight_smile:
```

---
## \#6 Posted by: Sander Posted at: 2016-12-12T17:37:32.333Z Reads: 76

```
With the cell batteries you buy from there. Do you need to do capacity testing?
Because that would be a pain in the ass to do... With 48 batteries Im gonna have in my board.
```

---
## \#7 Posted by: jbruce Posted at: 2016-12-12T17:52:16.032Z Reads: 78

```
If they're from a reliable source like battery bro you shouldn't have to test them, just check all thier voltages and make sure they're the same. @Sander
```

---
## \#8 Posted by: Sander Posted at: 2016-12-12T18:08:28.264Z Reads: 73

```
Cool! Hope so :) Im gonna order the LG one because it was one of the best new cells of 2015 and has the most capacity amps(3000mah, 20A). But they cost USD $4.38 per cell. So for 50 it is $219. And I have a trouble of finding trust worthy BMS sites. So if you could provide me with one that would be good :wink:
```

---
## \#9 Posted by: jbruce Posted at: 2016-12-12T18:12:35.356Z Reads: 76

```
Remember that with 80A and about 50v that's about 4000w of power that you most likely will never use (unless you're building a 4wd going up a super steep hill). If it were me I would go with the cheaper cell like the one in this group buy that can deliver less current but still has a high capacity.
```

---
## \#10 Posted by: Sander Posted at: 2016-12-12T18:36:05.493Z Reads: 67

```
I have a limited place inside the board. And if I wanted to get the max distance and max speed I would need to have 12s. 12s is greater power and greater distance then 8s.

The board looks like this inside: <img src="/uploads/db1493/original/3X/6/e/6e0f2453075d175c3ae6bb8b49a933af1f9e3c20.png" width="690" height="361">

Its 8 batteries on the long side. 6 on the short side.

And just to point it out the motors are 2250 Watt Each.
```

---
## \#11 Posted by: jbruce Posted at: 2016-12-12T18:50:29.779Z Reads: 58

```
Damnn thats a nice looking baord :smile: I agree with you about the 12s, im just saying you would be just fine using less expensive cells thats max current was 10A. It would still be the same configuration, 12s4p, and 95% of the capacity(515Wh which should get you over 25 miles and by that time your legs have already fallen off :grin:) but it would be about $100 cheaper for the cells if you bought it from this group buy. Also remember that you motor will most likely never draw 2200 Watts. I have a 2200 watt rated motor and at peak power I draw 1200 Watts, cruising about 250-500.
```

---
## \#12 Posted by: themegak Posted at: 2016-12-12T18:51:49.878Z Reads: 56

```
where did you get that board ?
```

---
## \#13 Posted by: Sander Posted at: 2016-12-12T18:57:36.663Z Reads: 57

```
[quote="themegak, post:12, topic:14476, full:true"]
where did you get that board ?
[/quote]

Haha, no I havent got it yet. I have 3d designed it in Fusion 360. I and my father are gonna make a foam cut of it. And then make a mold of it. Then make it into carbon fiber by laying layers. I can provide you with some schematic I made:<img src="/uploads/db1493/original/3X/b/0/b03d1f3e2b6ed55641af03f329cf0d6987f12bd7.jpg" width="690" height="487"><img src="/uploads/db1493/original/3X/d/5/d5472485045d7e51155d9dcf31f2e61253a21e58.jpg" width="690" height="487"><img src="/uploads/db1493/original/3X/1/1/111c72145614fb8e1eb8d2663f3822d4ef964560.jpg" width="690" height="487">
```

---
## \#14 Posted by: Sander Posted at: 2016-12-12T18:58:33.972Z Reads: 53

```
It will be 3cm thick board that goes 50km/h and goes >50km distance
```

---
## \#15 Posted by: Sander Posted at: 2016-12-12T19:07:48.238Z Reads: 53

```
[quote="jbruce, post:11, topic:14476"]
s, cruising about 250-500
[/quote]

I agree with what you say :slight_smile:. But the specs of the Carvon 2.5V Hub Motor has recommended battery of 10s to 12s. And the wiring in the board will be easier with 12s because then I can wire all the batteries together then having a few extra batteries in 10s. And I saw a man on a youtube video testing out the amps of the motor of the carvon. It took like 10-25 amps straight and up a hill. And that was one motor.. So it would have drawn around >50 amps. And I always likes to be on the safe side :) But I consider going down to cheaper batteries. But I have a budget, and with those batteries it wouldn't matter if I had the expensive ones ;).  And thanks about the comment of the board :blush:.
<img src="/uploads/db1493/original/3X/c/3/c3198aa29d7d5243e360186baaca88aa86f3ab3f.png" width="690" height="361">
```

---
## \#16 Posted by: jbruce Posted at: 2016-12-12T19:19:54.456Z Reads: 54

```
I wasn't saying go down to 10s, 12s is great, and if that's best for you, stick with it! I just thought using the cheaper batteries (with the same setup 12s4p) you could save around $100 and get the same performance. And remember with a single motor going up a hill it has to do all the work, so with two they would each be doing half and I bet you would never be pulling more than 40 amps. Also to be safe if you're using a vesc you can limit the current draw in the programming. I completely understand if you wanna stay on the safe side with the higher amp draw batteries, but if you change your mind and wanna get the Panasonic ones, let me know and we could get them for pretty cheap :slight_smile:  
Also don't forget wherever you're getting your batteries from, they're gonna charge shipping and its normally pretty expensive(from battery bro for 50 cells its $93)
```

---
## \#17 Posted by: Sander Posted at: 2016-12-12T19:22:44.911Z Reads: 52

```
I honestly want the panasonics. Because its cheaper. And I get more and in the VESC settings you can limit the amp draw from the batteries so that will not exactly be a problem :) So How much does it cost for the panasonics for 100 and 200 quanity?
```

---
## \#18 Posted by: Sander Posted at: 2016-12-12T19:27:04.969Z Reads: 54

```
but one problem it has 100mah less... So the distance will be a little differenet.
Calculation with 3000mah cells:
3000 * 4 = 12Ah
12s * 3.7v * 12ah = 53,28km

Calculation with 2900mah cells:
2900 *4 = 11.6Ah
12s * 3.7v * 11.6ah = 51.5km

So it will be 1.78km difference
```

---
## \#19 Posted by: jbruce Posted at: 2016-12-12T19:28:37.622Z Reads: 50

```
for 100 its $3.10 per cell with $132 of shipping and 3% credit card fee so $455.26, and for 200 its $2.95 per cell and $173 of shipping and 3% credit card fee so $785.89.
How many cells would you want?
```

---
## \#20 Posted by: jbruce Posted at: 2016-12-12T19:33:10.591Z Reads: 48

```
You're correct about the distance difference but honestly for me after a 10km ride my legs are sore. I can't imagine what a 50km ride would do :sweat: 
Thus I don't think 2 km will make too much of a difference\ for you because it would be physically very difficult to go on a 50km ride.
```

---
## \#22 Posted by: Sander Posted at: 2016-12-12T19:46:02.098Z Reads: 43

```
[quote="jbruce, post:20, topic:14476"]
You're correct about the distance difference but honestly for me after a 10km ride my legs are sore. I can't imagine what a 50km ride would do :sweat: Thus I don't think 2 km will make too much of a difference\ for you because it would be physically very difficult to go on a 50km ride.
[/quote]

Yes you are totally right! I was gonna mention it in the other reply that you wouldnt exactly need the extra 1km.
Because that extra 1km would be expensive. So I want a 50 cells battery. How much for them and how much for shipping to norway?
```

---
## \#23 Posted by: jbruce Posted at: 2016-12-12T19:51:52.870Z Reads: 42

```
Hmm. Just for the cells if it was just me and you in this buy then just the 50 cells for you would be $227.63. Shipping to Norway is the hard part, I believe it is quite expensive but let me check it out.
```

---
## \#24 Posted by: jbruce Posted at: 2016-12-12T19:54:30.026Z Reads: 41

```
If we could get 2 other people that also wanted 50 cells, the price would go down to $196.47 per 50 cells.
```

---
## \#25 Posted by: Sander Posted at: 2016-12-12T19:57:04.553Z Reads: 42

```
[quote="jbruce, post:24, topic:14476"]
get 2 other people that also wanted 50 cells, the price would go down to $196.47 per
[/quote]

Yeah that would be great... But I think I will stick with the LG Chem 18650 HG2.
Cost $219 for 50. But thanks for your help ;) You have been very helpful :smiley:
```

---
## \#26 Posted by: jbruce Posted at: 2016-12-12T19:58:09.599Z Reads: 42

```
Of course. Just wondering, where are you ordering those from?
```

---
## \#27 Posted by: Sander Posted at: 2016-12-12T19:58:30.843Z Reads: 41

```
[quote="jbruce, post:26, topic:14476, full:true"]
Of course. Just wondering, where are you ordering those from?
[/quote]

https://batterybro.com/products/lg-hg2-inr18650hg2-3000mah-20a
```

---
## \#28 Posted by: jbruce Posted at: 2016-12-12T20:01:26.418Z Reads: 41

```
Ok be weary of thier shipping charges. Your order will most likely come out to over 300$
```

---
## \#29 Posted by: Sander Posted at: 2016-12-12T20:06:20.320Z Reads: 38

```
Will do ;)
```

---
## \#30 Posted by: Sander Posted at: 2016-12-12T20:09:38.486Z Reads: 40

```
But do you know where to buy BMS(Battery Management System) for the batteries?
```

---
## \#31 Posted by: jbruce Posted at: 2016-12-12T20:14:10.813Z Reads: 39

```
Batterysupports.com have reliable bms's
```

---
## \#32 Posted by: lox897 Posted at: 2016-12-12T21:39:54.138Z Reads: 36

```
@Sander wouldn't nkon.nl be way better for you since they are in Europe?
```

---
## \#33 Posted by: jbruce Posted at: 2016-12-12T21:43:59.394Z Reads: 36

```
I've heard of them too. Do you know if they're legit, because there prices are very low, just a little suspicious.
```

---
## \#34 Posted by: lox897 Posted at: 2016-12-12T21:45:27.133Z Reads: 38

```
Yeah I bought with one other person and shipped to Australia and the cells are great. @whitepony buys his from there too and he has made like 4 battery packs
```

---
## \#35 Posted by: jbruce Posted at: 2016-12-12T21:46:06.472Z Reads: 35

```
Ok awesome!! I assume they are grade A cells?
```

---
## \#36 Posted by: Sander Posted at: 2016-12-12T21:46:08.569Z Reads: 38

```
[quote="lox897, post:32, topic:14476"]
wouldn't nkon.nl be way better for you since they are
[/quote]

The batteries are more expensive. But it will add up because the shipping is cheaper there. So it would be more relevant. But I don't know if they're legit. The website is kinda shady :open_mouth:
```

---
## \#37 Posted by: lox897 Posted at: 2016-12-12T21:47:11.242Z Reads: 37

```
I believe they are. As I said, I ordered from there, the cell voltages were all perfect and the cells look legit.
```

---
## \#38 Posted by: jbruce Posted at: 2016-12-12T21:48:35.739Z Reads: 36

```
What types of cell do you use?
```

---
## \#39 Posted by: Sander Posted at: 2016-12-12T21:49:15.267Z Reads: 35

```
The capacity? Was that legit?
```

---
## \#40 Posted by: lox897 Posted at: 2016-12-12T21:49:23.794Z Reads: 35

```
Samsung 25R. The one thing I wouldn't get from nkon is the sony vtc5 because Sony doesn't manufacture the cells anymore.
```

---
## \#41 Posted by: lox897 Posted at: 2016-12-12T21:50:04.524Z Reads: 34

```
Yes it was. @whitepony is known for making awesome packs and he always uses nkon so there is no doubt in my mind that they are fake.
```

---
## \#42 Posted by: Sander Posted at: 2016-12-12T21:51:45.629Z Reads: 31

```
I found a review of the 3000mah LG cell.

"Measured capasity about 2700mAh (discharge at 0,2-0,4A to 3V)"
- Review by Tuborg
```

---
## \#43 Posted by: jbruce Posted at: 2016-12-12T21:54:55.437Z Reads: 29

```
I know this is a weird question but do you by any chance know at what voltage they were when you received them?
```

---
## \#44 Posted by: lox897 Posted at: 2016-12-12T21:55:19.840Z Reads: 27

```
I think they were at 3.5 or 3.7 cant remember
```

---
## \#45 Posted by: lox897 Posted at: 2016-12-12T21:55:55.535Z Reads: 31

```
All I see is 5 star reviews on both pages but the Samsung 25r have got about 6x the amount of reviews
```

---
## \#46 Posted by: lox897 Posted at: 2016-12-12T21:56:58.584Z Reads: 31

```
Plus Tuborg still rated it at 4/5
```

---
## \#47 Posted by: Sander Posted at: 2016-12-12T21:59:19.813Z Reads: 31

```
I think ill go with the Samsung INR18650-30Q 3000mAh - 15A...
It has 7/7 reviews with 5 stars. But none has done capacity test.
```

---
## \#48 Posted by: jbruce Posted at: 2016-12-13T02:10:31.740Z Reads: 29

```
It seems that if you order cells from the Russian nkon that they are maybe 30cents per cell cheaper. Do you think that's a good idea or could they be a different grade cell?
```

---
## \#49 Posted by: lox897 Posted at: 2016-12-13T02:15:17.640Z Reads: 29

```
ru.nkon.nl is for international orders. Normal nkon.nl is for europe only
```

---

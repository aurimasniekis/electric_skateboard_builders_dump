# N00b LiPo Battery Questions

### Replies: 6 Views: 854

## \#1 Posted by: maxhost4 Posted at: 2017-10-07T06:01:53.539Z Reads: 115

```
Hey All,

This is my first build and it is coming along slowly but surely. Just got my motor, wheels, and VESC in the mail so I'm pretty excited. Motor is 6374 190 kv with 83mm wheels (I'll post pictures as soon as I get this whole build on its way). Up next is my battery set-up- I was going to get 4 of [these] (https://hobbyking.com/en_us/zippy-flightmax-3000mah-5s1p-20c.html?___store=en_us) 5S1P zippy's and run them as 10S2P. By my math I'll get a theoretical voltage of 37V, a C-rating of 40, and a total capacity of 6 Ah.

Here's what I'm wondering-
1. 6 Ah seems less than what most people have on their boards. Is there any way to get a rough estimate of range without deriving the formula myself from physics formulas? If need be I can always get 2 more batteries and run a 10S3P setup.
2. I can't seem to find much on charging LiPo battteries. HobbyKing sells [this](https://www.amazon.com/dp/B00L5YBJI2?) charger, but I was wondering if there was a more elegant solution than disconnecting all my batteries and charging them one at a time.

Any and all feedback is always welcome. This has been a work-in-slow-progress but I can't wait to share the finished product with y'all.

-MH
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-10-07T06:11:07.261Z Reads: 112

```
I have 2 graphene lipos  5s 4000mah 45c and run dual 6355 190kv 63 mm motors and get around 9-10ish miles depending on the riding style and hills 11-12 completely kills my lipos I weight 160lb and using currently 90mm clones the math that I came up with in lipos if it's more than 40c for every 4000mah it's a mile for me so 5s 4000mah I get 5 miles per lipo and second for lipos the most you can run is 12s , u can't run 10s3p lipos no esc let alone motor can handle that the most a esc or vesc can handle is 50 volts that would be a 12s lipo configuration I suggest u read more post before asking easy questions u can easily find on the forum ,also 6374 motors do consume a little more power but if u running one motor then I guess it's allmost equivalent to dual 6355,if you want to charge your lipos with out taking them out get a BMS (you can search that up On the forum lipo bms) sometimes the price u pay vs getting 18650 cells is just not worth it , so if you want a plug and play charge solution i suggest going 18650 cells way more exspensive but better in the long run
```

---
## \#3 Posted by: maxhost4 Posted at: 2017-10-07T06:55:59.636Z Reads: 100

```
Thanks for the advice. I would love to get the 18650 cells for my next build but right now I want to keep things relatively simple on the power supply side. I'm not the best at circuits (part of the reason I'm building my own board), so I want to keep it cheap in case I make anything explode. I'll keep you updated as this build takes shape.
```

---
## \#4 Posted by: Youssless Posted at: 2017-10-07T08:32:28.967Z Reads: 93

```
For range you calculate the Wh your batteries provide. 
3.7V (nominal voltage of lipos)  x number of cells in series (10 in your case) x Ah (6 in your case) = 222Wh

10S3P would get you 333Wh

General rule of thumb is 10Wh = 1km so you should see around 22km/13-14 miles (33km/20miles for 10s3p) depending on your riding style and hills.

You can get a BMS for 10S lipos and a charging brick that delivers 37V of DC if you want a plug and play solution.

Additionally, I'd recommend you ensure your lipos are used between 3.7V and 4.1V if you want to maximise their life. You'll see slightly less range (perhaps a mile or two) but they'll have more charge cycles. Some people drive their batteries down to 3.6V or even 3.3V (but motor really struggles to get power at this point if you're heavy like myself). Its up to you at the end of the day.
```

---
## \#5 Posted by: maxhost4 Posted at: 2017-10-07T15:14:08.366Z Reads: 61

```
Thanks for the math man. I didn't realize how important a BMS actually- I don't wanna have to replace my LiPo's every couple months cause I ran them too low. I appreciate the insight.
```

---
## \#6 Posted by: Youssless Posted at: 2017-10-07T22:58:29.396Z Reads: 53

```
All good man, I learned from people on this forum, I hope to contribute what I can. Best of luck and hit me up if you've any other questions.
```

---

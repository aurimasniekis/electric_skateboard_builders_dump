# Helpful 18650 (Nkon.nl) Filtering Tool

### Replies: 43 Views: 1985

## \#1 Posted by: darkkevind Posted at: 2017-08-12T21:59:37.704Z Reads: 260

```
I don't know about you but when looking for my 18650s I found Nkon's website to be a real pain in the arse to filter out which batteries were the best or which ones met my needs.

Because of this, I've created a little handy filtering tool on my website that lets you see **all** of their 18650 products and enables you to filter the results down to meet your criteria. You're viewing **exactly the same results as on their site** as it gets it's data **live**, but you're just able to filter it. Any clicks on the products will take you directly to their secure site.

You can also **enter your pack specifications** such as **8s4p**, and it will give you a total cost (without bulk discount) for your whole pack in order to gauge roughly how much your pack will cost.

Hope this helps.... let me know what you guys think? Try it here: http://kevindark.co.uk/PublicServices/NkonFilter
```

---
## \#2 Posted by: SilentException Posted at: 2017-08-12T22:05:13.177Z Reads: 243

```
Awesome! 2 suggestions: take bulk discount into account and filter ranges. Had to click 15 times to select everything from 2Ah and up :)
```

---
## \#3 Posted by: darkkevind Posted at: 2017-08-12T22:10:38.795Z Reads: 222

```
Hmmm yeah I see what you mean with the clicking....

I thought about taking the multi-buy discounts in to account, but that would mean another call on their site for each product to get that information... Although... it's not all of them that they give a multi-buy discount so I guess I won't be making a call for every single one... Just don't want them to get arsey about me hammering their site to scrape it :confused:
```

---
## \#4 Posted by: SilentException Posted at: 2017-08-12T22:12:08.330Z Reads: 182

```
Yeah, for getting a discounted price you would have to do a request for each one. Probably for the best not to do that, indeed.
```

---
## \#5 Posted by: darkkevind Posted at: 2017-08-12T22:43:30.900Z Reads: 163

```
I think I will do it actually! lol
```

---
## \#6 Posted by: wafflejock Posted at: 2017-08-12T23:01:25.995Z Reads: 142

```
You could always cache the data for a day or whatever it's not like we're looking at stock prices here :) That way it will probably go unnoticed as well.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-08-12T23:03:14.819Z Reads: 134

```
Yeah, that's exactly what I'll be doing, storing for 24 hrs.

My only worry is that they do actually update their site very often so I worry about being out of date some of the time :confused:
```

---
## \#8 Posted by: wafflejock Posted at: 2017-08-12T23:04:05.816Z Reads: 118

```
Yeah could always go like every half a day then or even every 6 hrs but probably best if you don't hit it for every person that loads your page there.
```

---
## \#9 Posted by: SilentException Posted at: 2017-08-12T23:48:02.679Z Reads: 122

```
See if they support ETag, Last-Modified, If-Modified-Since HTTP headers. That way you don't have to reload the page if it has not changed since last cache update.
```

---
## \#10 Posted by: darkkevind Posted at: 2017-08-12T23:49:01.611Z Reads: 117

```
Not a bad idea. I'll check.. cheers :thumbsup:
```

---
## \#11 Posted by: Okami Posted at: 2017-08-13T16:14:48.406Z Reads: 101

```
Havent tried your tool yet but im glad someone has made it and it didnt take that much time either right?

I assume you could somehow sell it off to them since they were.so busy not being able to make one on their own ha, so that others who might not be esk8 related, get to use it too
```

---
## \#12 Posted by: darkkevind Posted at: 2017-08-13T18:42:49.537Z Reads: 90

```
It didn't take that long no, just two evenings.

Yeah I'll have to see if I call sell them my code! Lol
```

---
## \#13 Posted by: SilentException Posted at: 2017-08-13T20:47:14.073Z Reads: 85

```
Not sure if the NKON website has some additional filtering or something but if I filter for LG using your filtering tool I will get 8 results.  If I click on the battery it opens up NKON.nl website but with error:

<img src="/uploads/db1493/original/3X/6/2/62c86e78d2531383004beae8f4289a9454b4ef8f.png" width="567" height="295">

On the NKON.nl I get 0 (zero) LG batteries.
```

---
## \#14 Posted by: darkkevind Posted at: 2017-08-13T20:53:39.911Z Reads: 80

```
That's odd! I get the correct page come up for all of these....

<img src="/uploads/db1493/original/3X/1/f/1ff30c8b68d7ce63648cc77934d55c646da76961.png" width="690" height="350">
```

---
## \#15 Posted by: SilentException Posted at: 2017-08-13T20:54:50.204Z Reads: 78

```
In that case it is probably NKON.nl doing geo-location filtering.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-08-13T20:57:20.153Z Reads: 76

```
You might be right, I'm not sure though because I just used a proxy to be in Turkey and it came up with all 8 of them...

https://eu.nkon.nl/rechargeable/18650-size.html?brand=35

What country are you from and I'll try it...
```

---
## \#17 Posted by: SilentException Posted at: 2017-08-13T21:00:41.179Z Reads: 73

```
Clicking on the link you provided opens up this webpage:
<img src="/uploads/db1493/original/3X/c/3/c3cedc76e3fcb86d627ac7a1697c62a50a05f41f.png" width="690" height="269">

Currently in Croatia but if I recall correctly I haven't seen LG batteries from Slovenia either.
```

---
## \#18 Posted by: darkkevind Posted at: 2017-08-13T21:04:03.705Z Reads: 72

```
That's really weird. Why wouldn't they ship them to you?

I can't change it to Croatia or Slovenia unfortunately, why don't you see if you can use a proxy and pretend you're in the states or the UK to see if that's the case? Perhaps someone could purchase and send them on to you?
```

---
## \#19 Posted by: SilentException Posted at: 2017-08-13T21:16:31.628Z Reads: 71

```
Currently, it is not a problem with purchasing as I'm still deciding on the cells I'm going to use. Was just reporting oddity when using your filter tool.

With France VPN I can see all LG cells on their website so it definitely is geo-location block.
```

---
## \#20 Posted by: darkkevind Posted at: 2017-08-13T21:17:38.182Z Reads: 72

```
Wow, I really didn't think they'd have the know-how to do that... they suck at their product search/filter section! lol
```

---
## \#21 Posted by: SilentException Posted at: 2017-08-13T21:46:55.857Z Reads: 58

```
Yeah, so weird. On 18650 page, only difference between me coming in from here or France are the missing LG cells (8 items missing). Almost unbelievable because HG2 cells were one of my top choices :)
```

---
## \#22 Posted by: darkkevind Posted at: 2017-08-13T21:51:17.164Z Reads: 59

```
They're what I went with and when I bought them they were on offer.. 32 cells £110!! :slight_smile:
```

---
## \#23 Posted by: Jinra Posted at: 2017-08-13T21:56:02.608Z Reads: 59

```
Could you add support for 20700 cells, or other cell types in general? 20700's are also a great alternative to 18650's
```

---
## \#24 Posted by: darkkevind Posted at: 2017-08-13T21:56:34.459Z Reads: 58

```
I'll see what I can do @Jinra
```

---
## \#25 Posted by: darkkevind Posted at: 2017-08-13T23:26:27.333Z Reads: 52

```
OK @Jinra, I've now included 26650. Unfortunately Nkon don't sell 20700s so I can't add that so easily without finding a good, cheap source for them...

I'll add other types soon too... http://localhost:63522/PublicServices/NkonFilter
```

---
## \#26 Posted by: darkkevind Posted at: 2017-08-14T01:25:09.615Z Reads: 44

```
Hey @SilentException, I've added range filters now... :thumbsup:
```

---
## \#27 Posted by: Jinra Posted at: 2017-08-14T01:27:12.490Z Reads: 44

```
are you sure? i saw sanyo ncr20700b earlier
```

---
## \#28 Posted by: darkkevind Posted at: 2017-08-14T01:31:36.255Z Reads: 48

```
Yes, sorry, you're right, they do sell them, albeit only one option :slight_smile:

What I was looking for was a category like the 18650 and the 26650...

Not sure that it's worth adding for just one product...
```

---
## \#29 Posted by: SilentException Posted at: 2017-08-14T08:29:49.706Z Reads: 46

```
Nice, helpful! 

Yesterday I noticed one more reason to take bulk discount into consideration as some comparing cells that are normally cheaper by piece get pricier when bulk discount is applied. If you are going to add bulk discount, it would be superb if you saved the data. Would be useful for price over time graphs, minimum price ever and such :)
```

---
## \#30 Posted by: darkkevind Posted at: 2017-08-14T11:41:00.789Z Reads: 46

```
Seriously!? That doesn't make sense :confused:

OK, I'm working on taking it in to consideration.
```

---
## \#31 Posted by: SilentException Posted at: 2017-08-14T11:53:53.040Z Reads: 49

```
Perhaps I expressed it incorrectly. The cells do not get pricier by piece but when comparing with others, they are no longer cheapest. For example:

CellA = 4€
CellB = 5€

and after bulk discount:
CellA = 3.8€
CellB = 3.5€

So for building a pack, now the B cells would be more affordable. Sorry for the confusion :)
```

---
## \#32 Posted by: darkkevind Posted at: 2017-08-14T11:54:26.638Z Reads: 45

```
Ahhh I getcha! :thumbsup:
```

---
## \#33 Posted by: darkkevind Posted at: 2017-08-15T01:48:35.174Z Reads: 44

```
OK, added multi-buy support for bulk and individual price.

Put your pack details in and it'll show you the total cost and individual cell price based on a multi-buy discount if there's one available...

Let me know what you think guys :thumbsup:
```

---
## \#34 Posted by: darkkevind Posted at: 2017-09-19T14:23:20.826Z Reads: 42

```
I like to think that this addition to Nkon's website for 18650's is down to me....

<img src="/uploads/db1493/original/3X/f/7/f7b0498cde82249f1514fccfd5797531757d415c.png" width="690" height="463">
```

---
## \#35 Posted by: Okami Posted at: 2017-09-19T15:02:27.748Z Reads: 38

```
hah .. looks good.. im glad they added it. Though I think your tool still offers more options to choose from(?)
```

---
## \#36 Posted by: darkkevind Posted at: 2017-09-19T15:03:39.718Z Reads: 43

```
Yeah it does because you can actually price up your pack on the fly and see which one come out the cheapest after multi-buy discounts are applied.

Once they implement that, then it's pretty much the same... lol
```

---
## \#37 Posted by: Okami Posted at: 2017-09-19T15:06:58.958Z Reads: 44

```
well.. it is still a bit funny that they improved the site / filter tool ( a tiny bit) after all this time  lol.. im not sure how much effort / time it required on your end but I still find it silly they hadnt done this earlier.. and that even now it could be more precise / detailed :D
```

---
## \#38 Posted by: SilentException Posted at: 2017-09-19T15:08:26.346Z Reads: 47

```
Haha. Well, TBH ranges were my feature request :stuck_out_tongue:
```

---
## \#39 Posted by: darkkevind Posted at: 2017-09-19T15:11:38.337Z Reads: 50

```
Ranges aren't my favourite user interface control... :confused:
```

---
## \#40 Posted by: SynteX Posted at: 2019-03-06T19:17:53.587Z Reads: 35

```
Hey I made a special site for this as well. You even get 3% discount if you order through my site :smiley:

https://esk8-calculators.com/
```

---
## \#41 Posted by: banjaxxed Posted at: 2019-03-06T22:47:58.612Z Reads: 32

```
Pretty handy thanks, was going to order some cells soon and tried the coupon but..![image|281x500](upload://fWbHeiF1lO2yWCL07ED1lDns9Vu.png)
```

---
## \#42 Posted by: SynteX Posted at: 2019-03-07T06:20:15.193Z Reads: 27

```
Hey benjaxxes you should add the cells first to your shoppingcart.
```

---
## \#43 Posted by: banjaxxed Posted at: 2019-03-07T21:42:09.703Z Reads: 13

```
Yeah thx latexes I got there, the link pre-button was one of my greatest hacking successes 

Nect sql injection with some dom-craft

Thank you for the explanation
```

---

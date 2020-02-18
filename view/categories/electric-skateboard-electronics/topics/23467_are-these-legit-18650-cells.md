# Are These Legit? 18650 Cells

### Replies: 32 Views: 1913

## \#1 Posted by: NerdNinja Posted at: 2017-05-19T14:13:35.016Z Reads: 141

```
http://www.gearbest.com/batteries/pp_383600.html

I wanna jump on this so bad! But I'm always weary of stuff that looks too good to be true. 

Any way I could protect myself?
This thread is very mixed :confused: 
https://www.reddit.com/r/gearbest/comments/3i2ci6/is_gearbest_legit/

(I call dibs on 40 of em if it's legit!! :stuck_out_tongue: )
```

---
## \#2 Posted by: Print3r Posted at: 2017-05-19T14:24:03.485Z Reads: 129

```
Look it up on lygte or look for the datasheet on the internet.
```

---
## \#3 Posted by: NerdNinja Posted at: 2017-05-19T14:40:55.709Z Reads: 125

```
Data sheets wouldn't help? It's a store page....
```

---
## \#4 Posted by: rwxr Posted at: 2017-05-19T14:42:25.412Z Reads: 126

```
http://lygte-info.dk/review/batteries2012/Panasonic%20NCR18650B%203400mAh%20(Green)%20UK.html
```

---
## \#5 Posted by: Maxid Posted at: 2017-05-19T14:46:02.701Z Reads: 122

```
I don't get it. Where is the deal?
33USD for 8 means 4.125USD per cell
At nkon.nl they cost €3.65 per cell and that is including European VAT
At ru.nkon.nl (the site for orders outside of EU) they cost just 2.90€

Plus these are not the best option for usage in esk8s.
```

---
## \#6 Posted by: NerdNinja Posted at: 2017-05-19T14:53:22.605Z Reads: 112

```
What!?! Man there $15 for 2 on Amazon for Panasonic! And why aren't these ideal? I've seen a bunch using the Samsung ones, these are just 900mAh more and .1v more? @Maxid
```

---
## \#7 Posted by: NAF Posted at: 2017-05-19T15:04:15.149Z Reads: 108

```
All cells on GEARBEST are legit...but you need to hunt for good deals.
```

---
## \#8 Posted by: Pedrodemio Posted at: 2017-05-19T15:10:01.273Z Reads: 109

```
i use them, but do not recommend, the internal resistance is too big for high current use, that means that in my 10S3P pack, the max current is 20A, and at that current i have 7V of voltage sagging

Because of that when i have 60% remaining, the VESC already begin to cut off power and the performance just worsens from there

you are batter going with LG HG2, samsung 30Q, etc, even the NCR GA is way better than the B

the only situation they could work is in a gigantic pack (8P or more) and even so the GA would do better for almost the same price
```

---
## \#9 Posted by: Okami Posted at: 2017-05-19T15:12:36.890Z Reads: 105

```
yeh @NerdNinja if you are outside of usa, Nkon might offer a very good deal for you, search for it on google as i dont want to go an type the adress now.
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:13:09.359Z Reads: 103

```
Pretty low discharge current, only 6.7 A...
https://eu.nkon.nl/rechargeable/18650-size/panasonic-ncr18650b-made-in-japan.html

Here's a datasheet:
https://www.math.ubc.ca/~wetton/papers/NCR18650B.pdf

I would suggest Samsung INR18650-35E 3450 mAh, 10 A. With very competitive price at bulk
https://eu.nkon.nl/rechargeable/18650-size/samsung-inr18650-35e.html
```

---
## \#11 Posted by: NerdNinja Posted at: 2017-05-19T15:16:32.074Z Reads: 93

```
I'm in the US 😕 what I'm gathering here is I should try to find the Samsung ones? Is that the best deal you know if @SimosMCmuffin
```

---
## \#12 Posted by: Okami Posted at: 2017-05-19T15:18:31.358Z Reads: 91

```
depends on how big / high range / high power pack you wanna build, then you can build the pack that suits your needs.

If hills are no problem and u dont have dual, u might do well with less powerful pack.

Do u have someone who gonna spot weld them too?

Otherwise u need to look at sleds and / or soldering options.

--

30Q samsungs are generally 'the new trend'' now because they seem to perform better than 25R and offer higher capacity. Dont believe the 15A rating on them, as others report them working at 20A reasonably well (even if both 25r and 30q do get quite a bit hot when operating at 20A constant)

Aim for 60amp discharge, which might be 4P pack in 10s, 8s, 6s or which voltage you might choose..

60amps at 36v ( 10s) is 2160W already, so I would say you can actually go with 3P or even 2P if you want to strain your cells a bit.. choice is  up to you but as u have read around here probably, then people usually recommend 60A discharge or such.

I actually have 1300W pack for mountainboard and for flats and speeds not higher than 22mph, it is more than enough.
```

---
## \#13 Posted by: NerdNinja Posted at: 2017-05-19T15:22:59.311Z Reads: 74

```
I guess I should've mentioned. I'm going for a 10S4P. Although I'm not too knowledgeable in all this... But that's what was mentioned on my build thread.

Hills are a issue​, pretty steep but few and far in-between. I'm going for 1 motor, might upgrade to duals later. Looking for good range with about 20-30 mph speeds.

I think I have a local battery place that can weld for me, but I need to check into that. Might be able to make a spot welder grin an old microwave...
```

---
## \#14 Posted by: Okami Posted at: 2017-05-19T15:25:11.723Z Reads: 76

```
Some say microwave transformers are not best and car batteries perform better but havent tested yet so cannot tell from personal experience.. heck if ultra caps work then in some config microwave transformers should too..

yeh.. well for hills and decent speed you do might need a bit of power.. so yeh, plan ahead and get a pack for 2-3kw of power then. If u gonna use vesc, then this is not a problem, since vesc can also output up to 3kw I believe in 12s because of 50A limit (unless u use VESC X, which has higher rating)

2 - 2.5kw pack might be enough for you.

Take voltage and amps battery can produce and then you get **result**

2500 / 36 (nominal voltage) = ~70A
2000 / 36 = 55.55 A

~19A discharge works here ok.

On flats, i think you barely gonna see more than 500-600w of power being used.

Check VESC telemetry thread where @Ackmaniac and others have posted their data. U will see how much power it actually takes
```

---
## \#15 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:29:08.280Z Reads: 74

```
Can't say what's the best place in US... Google search around for li-ion/18650 wholesale places.

For Europe Nkon is pretty good, just ordered 50 Pcs of Samsung 35E from them and I can also order without the VAT with my company VAT number so it's even cheaper. Capacity tests already show them to be higher in capacity then the LG MJ1s even though they are both rated around 3500 mAh and by a big margin. MJ1s struggled to get 3300 Mah, while the 35Es easily got around 3450 mAh.
<img src="/uploads/db1493/original/3X/c/5/c553c27bbb7e2a6ff1b78eb60ecc90c3a4db5571.jpg" width="689" height="390">
```

---
## \#16 Posted by: Okami Posted at: 2017-05-19T15:30:22.608Z Reads: 69

```
@SimosMCmuffin  yeh, hadnt seen anyone using these cells before, they do look 'brand new'' / like recently released.

Thanks for releasing the results :) they do seem better than LG Mj1 cells.. I think maybe samsung cells in general are a bit better than LG ones(?)
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:32:57.500Z Reads: 64

```
The results were pretty much on par with the ones from lygte when comparing their results for the MJ1s and 35Es.
http://lygte-info.dk/review/batteries2012/Common18650comparator.php

I'm going to check new cells through them first in the future. I was a bit disappointed in the MJ1s' true capacity to be honest.
```

---
## \#18 Posted by: Maxid Posted at: 2017-05-19T15:34:57.802Z Reads: 61

```
35Es seem to be some of the worst cells I have ever seen - lygyte does not even test them at 20A. The voltage sag at 15A is enormous!
Why would anyone want to use them in anything besides a monstrous 8P pack or something?
```

---
## \#19 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:44:17.714Z Reads: 61

```
They are rated for 10 A continuous. I'm building a 10S5P pack. Cruising at 600 Watts would only mean a pull of 15 Amps total at 40 V and you can pull the 2000 W, 50 A, 40 V for hills momentarily. and of course you can always slow down your ascend if you want to use less power. Seem pretty decent for long range pack.

My current pack is 6S4P with the MJ1s and they haven't had any problems so far.
```

---
## \#20 Posted by: Okami Posted at: 2017-05-19T15:45:52.380Z Reads: 58

```
I see where youre going.. u gonna have super long range battery now :D probably wont need to charge the board for 2-3 days straight..

I get 594 Wh for your battery pack, (@3.3Ah * 3.6v nom per cell = ~11.88wh/cell)

So.. going almost 60km with a pack is not bad :D

30km is already decent.. but yeh, u can probably be really laid back now and charge only occasionaly, at fast rate and not till 4.2v
```

---
## \#21 Posted by: Maxid Posted at: 2017-05-19T15:57:36.392Z Reads: 49

```
You did check the discharge curve didn't you? What a cell is rated for is meaningless.
"Pretty decent" would be a 30Q or GA pack compared to the champion VTC6.

If you want a long range pack get GA cells
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2017-05-19T16:00:51.706Z Reads: 51

```
This is my current board:
http://imgur.com/a/Mjodj

I'm going for pneumatics and Trampa trucks on the next iteration to smooth and dampen the vibrations during riding and also give it some off-road capability.
<img src="/uploads/db1493/original/3X/8/7/87c25830106b9b50efd5514d39a6666a6d53bf61.jpg" width="689" height="390">

I'm also developing my own FOC enabled motor controller and once I get the single drive one working nicely I'll make a single board for dual motors.
<img src="/uploads/db1493/original/3X/2/8/28d8968f52c51e3a40a072c3ada2fab4169c0182.jpg" width="282" height="500">
```

---
## \#23 Posted by: Okami Posted at: 2017-05-19T16:04:17.417Z Reads: 51

```
@SimosMCmuffin  Nice! We are probably 'de-railing''the discussion a bit.. but I could shed some details on my build and witnessed power consumtion, if you'ŗe interested. Though data is not as precise and smooth as Vesc App could offer but still..

Ok, then 600wh pack is quite okay for long commute / high power rides.

Would still give you plenty of range probably.
```

---
## \#24 Posted by: SimosMCmuffin Posted at: 2017-05-19T16:09:57.451Z Reads: 50

```
The GA cells are way more expensive compared to the 35Es with pretty much identical performance. Cell current rating is based on it's internal resistance or how much it heats up when you discharge it. They usually test with an upper temperature limit of 60 Celsius.

VTC6s are super expensive and only make sense if you need high capacity AND discharge current.
```

---
## \#25 Posted by: Maxid Posted at: 2017-05-19T16:16:07.178Z Reads: 47

```
[quote="SimosMCmuffin, post:24, topic:23467, full:true"]
pretty much identical performance
[/quote]

Please show me where in this graph you see identical performance:
<img src="/uploads/db1493/original/3X/c/9/c991d6fab3189171a5c1e1fbcfd465399127c5ff.JPG" width="690" height="480">
that voltage drop is real!
30Q still stand as the price/performance winner
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2017-05-19T16:21:58.847Z Reads: 44

```
As I said. They are rated for 10 A and that's what I've been designing my drive around.

That's like saying that "I removed the rev limiter on my car and I drive it around 50% over the limited RPM and it's performance is awful!" Well no duh sherlock.

<img src="/uploads/db1493/original/3X/f/2/f24e3af8a007caea58de824f9023edba78696e7c.jpg" width="690" height="471">

At the more sensible discharge currents they are very similar.
```

---
## \#27 Posted by: Maxid Posted at: 2017-05-19T16:30:36.409Z Reads: 43

```
you always want to overspec- I made that mistake with my 25Rs - they are rated for 20A but don't deliver.
I just don't want you to make the same mistakes.
Good luck with your pack - I hope it works out the way you want it to.
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2017-05-19T16:33:32.851Z Reads: 42

```
Thanks.
I really haven't had a problem with the LG MJ1s, so I'm just building a bigger pack with similiar spec'd cells with a better price point.
```

---
## \#29 Posted by: Okami Posted at: 2017-05-19T16:38:05.010Z Reads: 43

```
@Maxid 

I think a lot of people got 25R cells because they were just 'ŗecommended' at that time on the forum :) Along with LG HG 2 I believe

They do perform poorly for higher load, that's true but yeh unless you really wish to torture cells I think what @SimosMCmuffin will suit him well.. he still has relatively huge pack to compensate for the load / high power demand.
```

---
## \#30 Posted by: NerdNinja Posted at: 2017-05-19T17:46:51.531Z Reads: 42

```
:confounded: My head is spinning!! :dizzy_face: 

How much amperage will I need to draw with 2 motors?? 

I'm thinking on going with the GA's to be safe...?
```

---
## \#31 Posted by: Maxid Posted at: 2017-05-19T17:49:36.697Z Reads: 44

```
get Samsung 30Q and you have the best of both worlds (high capacity and high discharge capabilities). They are the favorites around here at this point.
```

---
## \#32 Posted by: NerdNinja Posted at: 2017-05-19T17:50:59.714Z Reads: 44

```
ok, I'm done thinking for today XD I'll go with those lol. Thanks guys! You saved me a bunch of money and headache!

Found them on ru.nkon.nl. 30EUR shipping for a total of ~ 160USD nice!
```

---

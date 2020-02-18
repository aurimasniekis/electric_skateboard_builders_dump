# Combining parts for the first build

### Replies: 10 Views: 1522

## \#1 Posted by: rafal Posted at: 2016-10-05T20:08:23.296Z Reads: 108

```
Hi, I am learning as much as I can prior to building first electric skateboard with my friend but there are a few question I couldn't find an answer to. I'll give you super quick introduction to our project.

We want to make a build that will let us learn as much as possible and we don't have much money. We learned that crap parts everywhere won't work but I think I found a way to cut the costs at least a bit without making a crap overall effect; mainly by using standard ESC + Arduino instead of VESC and by 3D printing transmission components and the case.
<img src="/uploads/db1493/original/3X/c/a/cad5603e1daf4e34900651101389ea0bcc5d99c7.png" width="690" height="114">

------- TL;DR -------

1. The main question is - how do I know that certain parts fit well with each other? For example - I am able to buy a SK3 5055 430KV engine that has a maximum current of 70 ampers. Does that mean that I have to buy 70A ESC?

2. The battery - [in this video](https://www.youtube.com/watch?v=6yBgsT65UPg) we are advised to buy cheapest 3S 5000mAh battery - I already know the difference between 20C and 30C, but that "S" rating is still not perfectly clear for me. I get that S = 3.7V but does that mean that I'd have to connect two 3S batteries in series to get 6S voltage that's required by most motors?

If someone already answered these questions earlier or I missed something in the basic tutorials, please just direct me to the proper topic/site.

Thanks
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-05T20:24:52.437Z Reads: 96

```
1. As long as both your ESC and Motor current are higher than you need, it doesn't really matter which one is the limit. (as long as you won't go above 50A, a 70A motor on a 50A ESC is totally fine, so is a 50A motor on a 70A ESC).

2. Short answer, you're correct. Slightly longer answer, I think [my post here](http://www.electric-skateboard.builders/t/vesc-and-s-amounts/4737/2?u=rpn314) would be useful for you.

On the rest of your idea, got a few things for you.
1. I would recommend a motor with a much lower KV. 430kv is not ideal for our uses.
2. What's the Arduino going to be doing? I'm just trying to understand, sorry for my ignorance
3. Is your only reason for avoiding the VESC due to cost?
```

---
## \#3 Posted by: rafal Posted at: 2016-10-05T20:54:58.966Z Reads: 81

```
Thank you for linking that post - everything's clearer now.

I don't know if there is a standard of communication between R/C controllers and ESCs. That's why I'm thinking about putting Arduino between them - it would read the signal from R/C receiver, maybe do a little math (smoother start, LED indicators or maybe some of VESC-like functions) and then send proper signal to ESC.

VESC is about $100 (+ shipping to Poland) and ESC will cost about 20% of that and currently it's a huge difference for us (first-year university students). 
Also we want to learn as much as possible - coding Arduino shouldn't be too hard (lots of resources online) and yet would provide a challenge if we wanted to add more features.
```

---
## \#4 Posted by: rpn314 Posted at: 2016-10-05T21:16:16.260Z Reads: 71

```
There is a standard for most RC controllers(PPM I believe). To be honest, most of the benefits of the VESC I don't know how to replicate without a similar system (a specialized ESC), especially the benefits of fantastic unsensored motor controlling (which the SK3 is by stock). I'm not familiar enough with other ESCs to comment too much more on what they can and can't do specifically, but in general, they do what the VESC does, they just don't do it as well
```

---
## \#5 Posted by: TarzanHBK Posted at: 2016-10-06T09:12:27.280Z Reads: 55

```
for EU guys on budget, you should get this kit:
https://electric-skateboard.market/product/esk8-starter-kit-motor-esc-controller/
can´t get cheaper, and all parts are common and well known parts here.
You don´t need an arduino, just stick with a remote and receiver and you´ll be fine ;)
2 x 3s batterys, steel motor pulley (don´t try and print it! It will not last long) and a printed wheel pulley, hdt5 12 or 15mm belt, caliber 2 trucks, a motor mount, printed enclosures.
did i miss something?
```

---
## \#6 Posted by: Bazingazunga Posted at: 2016-10-06T15:03:47.901Z Reads: 49

```
Yo @TarzanHBK where can i get a 12s esc in the UK? do you know any sites? All i seem to find is up to 6s, regardless of whether theyre 60A or 150A :/
```

---
## \#7 Posted by: rafal Posted at: 2016-10-07T21:11:29.724Z Reads: 37

```
I'm not sure about that kit, in EU it costs 140 EUR instead of USD and that suddenly makes HobbyKing offers way more appealing (I was always looking at EU prices at HobbyKing instead of global and somehow global prices are lower).

I'm just not sure if 190 KV isn't too low:

http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=18129

And one of these two ESCs (70A would work with 80A SK3, right?)

http://www.hobbyking.com/hobbyking/store/__80518__Aerostar_70A_Electronic_Speed_Controller_with_5A_BEC_2_6S_.html

http://www.hobbyking.com/hobbyking/store/__24718__HobbyKing_70A_BlueSeries_Brushless_Speed_Controller.html

And the Arduino is out of the equation now, but it looks like an easy way to make a board more useful in the future.
```

---
## \#8 Posted by: TarzanHBK Posted at: 2016-10-10T09:03:51.899Z Reads: 34

```
there you go:
https://eu.electric-skateboard.market/product/12s-120a-esc-hv-opto/
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-10-10T09:08:24.645Z Reads: 36

```
140 euro for that kit is a really good deal to start with.
190kv is indeed a bit low for 6s but a good start for beginners if you don´t want to spend much and keep it low.
later on you just switch your esc to an vesc and upgrade to 10s and you´ll get an awesome board with that 190kv motor.

or just tell @ajaynagra you want a higher kv motor like a 245kv and you´re good to go with 6s.

also don´t use these escs. they are plane escs and don´t have any brakes. also is 70amp too low for an 6s system.
take a good car esc with at least 120amp
```

---
## \#10 Posted by: rafal Posted at: 2016-10-13T20:36:04.459Z Reads: 27

```
So after some more research, here are the components we think are pretty good and won't make us totally broke:

Motor - SK3 192kv
http://www.hobbyking.com/hobbyking/store/__18129__Turnigy_Aerodrive_SK3_6374_192kv_Brushless_Outrunner_Motor.html
Battery - Zippy 5000mAh 3S 25C
http://www.hobbyking.com/hobbyking/store/__8583__ZIPPY_Flightmax_5000mAh_3S1P_25C.html
Charger - Imax B6
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idproduct=76461
R/C - Quanum 2.4 ghz
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idproduct=44693
ESC - FVT 120A
http://www.ebay.pl/itm/FVT-120A-Brushless-Sensored-Sensorless-RC-Car-ESC-2-6S-1-10-USA-SHIP-120-AMP-/391484703658?hash=item5b264e83aa:g:LPQAAOSw8gVX6ObM

Everything including shipping is about 235 usd / 213 eur
We're getting deck, trucks and wheels locally (polish skateboard stores) so rest of the costs shouldn't exceed about 80-100 usd.

ONE LAST QUESTION ABOUT THE MOTOR (192kv SK3)

Using the standard 15/36 gearing ratio the top speed should be around 20-25 km/h according to the calculators. Do you think that motor would be able to withstand 18/36 gearing or similar (we don't need or expect to exceed 30 km/h but of course real life speed is always a bit lower than expected so we'd just like to have a little margin)

Also, thank you guys so much for the replies so far, we're incredibly grateful for them.
```

---

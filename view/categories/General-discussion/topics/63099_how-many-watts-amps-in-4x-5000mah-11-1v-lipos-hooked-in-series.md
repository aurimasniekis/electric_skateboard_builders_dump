# How many Watts &amp; Amps in 4x 5000mah 11.1V Lipos hooked in series?

### Replies: 49 Views: 972

## \#1 Posted by: Toohat Posted at: 2018-07-27T21:44:38.960Z Reads: 121

```
So I have 4 of these https://www.amazon.ca/gp/product/B07594LWWS/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1 

So I have 4 of them hooked in series and I can't figure out how many Amps and Watts they output. Thank you in advance for your help!
```

---
## \#2 Posted by: cryo Posted at: 2018-07-27T21:58:22.691Z Reads: 121

```
4 x 11.1v (3.7v per cell) = 44.4v (3s x 4 = 12s)
5000mah = 5ah 
5ah x 50.4v (4.2v per cell) = 252 Watt hours

5ah * 50c = 250a
5ah * 100c = 500a
250 amps continuous
500 amps burst
```

---
## \#3 Posted by: Toohat Posted at: 2018-07-28T04:06:04.932Z Reads: 108

```
Thank you so much Cryo! And one more thing, so I will be using this vesc https://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

and its rated for 60amps continuous so is my 4xlipos in series too much cuz i will only using one of these motors collections/electric-skateboard-starter-collection/products/electric-skateboard-motor-6374-190kv. And when I hook four of them in series than to a parallel connector it reads about 24v im not sure if it became 10000mah and 6s or its still the same.
```

---
## \#4 Posted by: Namasaki Posted at: 2018-07-28T04:29:04.289Z Reads: 96

```
[quote="cryo, post:2, topic:63099"]
5ah * 50c = 250a
5ah * 100c = 500a
250 amps continuous
500 amps burst
[/quote]

This equation does not give true current capability of Lipo batteries.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-07-28T04:34:07.139Z Reads: 94

```
Take a look at these True Spec Lipos.
They give the true current capability of their Lipos.
https://www.smc-racing.net/index.php?route=product/category&path=67_99

5400/90C is 135a continuous
```

---
## \#6 Posted by: Toohat Posted at: 2018-07-28T04:53:42.211Z Reads: 91

```
anyways ill do my own experiments, thanks alot
```

---
## \#7 Posted by: cryo Posted at: 2018-07-28T06:31:43.318Z Reads: 86

```
I'm just going off of formulas off google search and it seems c rating * ah = amp draw is the consensus. 

I agree manufacturers tend to inflate the c rating a lot but without OPs battery in hand to test, we'll never know

Edit: actually, looking back at it now https://www.smc-racing.net/index.php?route=product/product&path=67_99&product_id=463 
this confuses me. are they saying their 90c batteries are 85 amps continuous? If so, doesn't that just mean they are misrepresenting the C rating of their batteries? Because every website I've visited has agreed that (c rating) * (mah/1000) = (cont. amp draw) so instead of mentioning 90c it would just be 20c...
```

---
## \#8 Posted by: cryo Posted at: 2018-07-28T06:43:51.112Z Reads: 80

```
That depends on the load. A few factors affect how much current you'll draw such as your weight, going up a hill, throttle, etc. 

What I can say for sure is you'll be drawing less amps with the 12s battery setup rather than 6s2p, But if you go 12s, using a 190kv motor might put you over the vescs erpm limit. If going with the 6s, i would maybe recommend a higher kv motor.

See
https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

That being said, 250 amps is just the theoretical max amp draw your battery is capable of, real world usage you will likely never even hit 100...
```

---
## \#9 Posted by: Namasaki Posted at: 2018-07-28T12:03:34.511Z Reads: 70

```
SMC isn’t inflating their C rating. 
They are showing that AH x C does not give true current capability. 
I used to think that my 5ah 60C batteries would handle 300a cont. 
but then I saw how that they have some voltage sag with only 20-30a draw and I realized that the equation was incorrect.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-07-28T15:56:24.379Z Reads: 73

```
Why? How to understand which is right or not?
How about the hobbyking lipos? The rating is there also not right?
```

---
## \#11 Posted by: Namasaki Posted at: 2018-07-28T18:21:23.541Z Reads: 65

```
The formula of AH x C = current is not right. 
It doesn’t give a true answer. 
This is the case with all Lipos. 
That is why SMC states the true current capability of their Lipos.
```

---
## \#12 Posted by: Toohat Posted at: 2018-07-28T19:43:46.156Z Reads: 58

```
I don't understand, I thought that hooking 4 of them in series would equal to 12s and 44.4V but it stays 5000mah so how 6s is more amps and it becomes 10000mah and about 22.2V right?
```

---
## \#13 Posted by: Andy87 Posted at: 2018-07-28T19:56:27.324Z Reads: 60

```
I don’t like this c-rating declaration...
Just wonder why smc just don’t write there max amp???
There c rating totally over the top.
You said the formula ah x c = amp is wrong, but how than all companies define there declared c rating?
What would you recommend is a good point to start with. If to look again to the hobbyking lipos which most common here I guess.
Let’s say 6s 4000mah 65c would be after the old formula 240a constant.
So in real life i can take from this the half, 130a and this would be the real max constant current? 🤔
```

---
## \#14 Posted by: Andy87 Posted at: 2018-07-28T20:02:04.619Z Reads: 58

```
In series the volts add up
In parallel the amps and ah add up
With 6s you still have 5000mah
But if you run 6s2p than it’s 10000mah and 22volts
```

---
## \#15 Posted by: Toohat Posted at: 2018-07-28T20:14:05.826Z Reads: 53

```
what does 2p mean?
```

---
## \#16 Posted by: Andy87 Posted at: 2018-07-28T20:26:58.778Z Reads: 54

```
2p means two in parallel.
Now you made a 12s1p pack with your 4packs
You can make a 6s2p out of this 4packs
Just set up 2packs in series, twice and connect them than parallel
```

---
## \#17 Posted by: Toohat Posted at: 2018-07-28T20:28:03.123Z Reads: 56

```
like this?![IMG_0075|375x500](upload://yIzwh8KsG45xOqVKiuKoSwJSXQ9.JPG)
```

---
## \#18 Posted by: Andy87 Posted at: 2018-07-28T20:36:12.763Z Reads: 54

```
Like this (sorry for the shitty drawing 😜)
![image|374x500](upload://fHn28WMjhj8wqiY1y6RYzqT6Ho3.jpeg)
```

---
## \#19 Posted by: Toohat Posted at: 2018-07-28T20:49:01.369Z Reads: 50

```
just to make sure like this? ![sketch|690x388](upload://z93RkuIXg4RXVdw7HihE2JePby.png) LOL
```

---
## \#20 Posted by: Andy87 Posted at: 2018-07-28T20:59:48.239Z Reads: 45

```
🤔you are the next Picasso 😉 
That’s right. Should work.
```

---
## \#21 Posted by: Toohat Posted at: 2018-07-28T21:04:59.663Z Reads: 41

```
:joy::joy::joy::joy::joy: hahaha
```

---
## \#22 Posted by: Andy87 Posted at: 2018-07-28T21:06:15.732Z Reads: 45

```
I just read again through your post.
Don’t understand right what’s your problem in the end. The batteries you chose for sure able to handle the 60a the focbox can handle.
Doesn’t matter if you run 12s or 6s.
The weak point in this case is your focbox.
If you planed to order the 190kV Motor, than stay with it. 12s 190kv should give you a good speed.
Just don’t forget to set your max battery current to 50a (60a should be fine too if airflow is good around your focbox) and your max erpm to 
+-60 000
```

---
## \#23 Posted by: Toohat Posted at: 2018-07-28T21:09:05.090Z Reads: 45

```
so 12s 44.4V would be more speed and 6s2p would me less speed but longer range?
```

---
## \#24 Posted by: Andy87 Posted at: 2018-07-28T21:11:12.656Z Reads: 46

```
One additional explanation as I think you got it wrong.
Your batteries just give what your focbox and your comand by the remote ask for.
So let’s say your max current of your focbox is 60a and you pull your trigger on the remote and go up a hill with your 130kg 😜(just for example...don’t know your weight) your batteries will need to deliver 60a.
```

---
## \#25 Posted by: Toohat Posted at: 2018-07-28T21:12:33.350Z Reads: 44

```
im 65kg hahahaha
```

---
## \#26 Posted by: Andy87 Posted at: 2018-07-28T21:13:04.007Z Reads: 43

```
It depends on your motor kV, the gearing and the wheel diameter. 
You can calculate everything here:
http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":170,"system-efficiency":85,"motor-pulley-teeth":9,"wheel-pulley-teeth":40,"wheel-size":200}|
```

---
## \#27 Posted by: Toohat Posted at: 2018-07-28T21:19:07.452Z Reads: 41

```
ok so when its 12s top speed is about 40mph and 6s is 20mph is this true?
```

---
## \#28 Posted by: Andy87 Posted at: 2018-07-28T21:24:26.088Z Reads: 40

```
If you used the calculator which I linked you than yes. Just make sure you looked the weighted speed. For my set up it was pretty close to the real values. If you run single motor it can be that you need a bit longer to reach top speed, but in general it’s really good template
```

---
## \#29 Posted by: Toohat Posted at: 2018-07-28T21:27:25.339Z Reads: 38

```
I will try both setups and see whats better long range but slower or faster but short range, Cuz I made the connectors for both setups of 12s and 6s2p
```

---
## \#30 Posted by: Andy87 Posted at: 2018-07-28T21:32:46.675Z Reads: 36

```
Which range you wanna have?
```

---
## \#31 Posted by: Toohat Posted at: 2018-07-28T21:34:45.557Z Reads: 35

```
idk how far can the batteries i got go?
```

---
## \#32 Posted by: Andy87 Posted at: 2018-07-28T21:41:17.747Z Reads: 37

```
Depends on your ride stil.
If I remember right than I had about 11wh per km for one motor on dual, so 22wh per km. 
You have 12*4,2=50,4 *5ah =252wh 
So about 12km with dual motors and flat area.
In your case could be a bit more as it is only single motor
```

---
## \#33 Posted by: Toohat Posted at: 2018-07-28T21:43:15.236Z Reads: 36

```
and what if i run the 6s2p will that be like 24km?
```

---
## \#34 Posted by: Andy87 Posted at: 2018-07-28T21:54:20.145Z Reads: 37

```
There shouldn’t be so much difference.
It’s still the same energy stored in your batteries.
But I think it’s analog to a car.
To drive 200km/h will bring you not the same way like you drive 80km/h but also not the double.
I think it will be not more then 2km more.
If you ride economic with 12s it can even bring you the same.
```

---
## \#35 Posted by: Toohat Posted at: 2018-07-28T21:56:08.373Z Reads: 35

```
gonna have to make an eco switch ahahahahaa. Thanks for your help Andy, thanks a lot.
```

---
## \#36 Posted by: Andy87 Posted at: 2018-07-28T22:10:17.121Z Reads: 35

```
Welcome!
If you interested in your data I can just recommend you to get a Bluetooth module. You can get them very cheap like 2€ on AliExpress and there are some good apps with which you can record your rides. It will show you directly which is the best set up for your needs.
```

---
## \#37 Posted by: Toohat Posted at: 2018-07-28T22:24:19.115Z Reads: 33

```
Good to know, I might give it a try. thanks!
```

---
## \#38 Posted by: Namasaki Posted at: 2018-07-28T23:18:21.169Z Reads: 35

```
[quote="Andy87, post:13, topic:63099"]
I don’t like this c-rating declaration…
Just wonder why smc just don’t write there max amp???
There c rating totally over the top.
You said the formula ah x c = amp is wrong, but how than all companies define there declared c rating?
What would you recommend is a good point to start with. If to look again to the hobbyking lipos which most common here I guess.
Let’s say 6s 4000mah 65c would be after the old formula 240a constant.
So in real life i can take from this the half, 130a and this would be the real max constant current? :thinking:
[/quote]

I run 5ah 60C Lipos. They are adequate for a street board. Voltage sag is only about 1/2 v off total pack voltage when accelerating on flat ground.
For a mountain board or a street board with larger than 90mm wheels, I would try to get some 90C or higher.

You want to have as much headroom as possible to reduce voltage sag and battery heat.
```

---
## \#39 Posted by: Andy87 Posted at: 2018-07-29T06:19:58.738Z Reads: 34

```
I‘m looking for some lipos for my next mountain board at the moment.
Can you recommend a brand or shop which also ship internationally?
```

---
## \#40 Posted by: Namasaki Posted at: 2018-07-29T22:59:32.097Z Reads: 32

```
I would try the SMC Lipos
There is a link posted earlier in the thread.
I think they go up to 150C
```

---
## \#41 Posted by: Andy87 Posted at: 2018-07-30T04:39:53.248Z Reads: 29

```
I already looked it up.
Problem that they don’t ship international.
That’s why I asked if you can recommend some brand which is available also internationally.
Till now I just found the hobbyking lipos which go up to 60-65c only
```

---
## \#42 Posted by: Namasaki Posted at: 2018-07-30T11:54:17.429Z Reads: 29

```
60C is fine for a street board.
I’ve never built a mountain board so I can’t say how they would perform in that scenario
```

---
## \#43 Posted by: Andy87 Posted at: 2018-07-30T17:58:14.537Z Reads: 28

```
What I forgot to say, if you put your lipos in parallel, take care that they mach with the voltage. I don’t have experience yet but as i‘m also planning to buy some I started to look for information.
In series it’s not so big problem but in parallel you can for example over discharge one if they don’t match. It can even blow them up. So better safe than sorry😉
```

---
## \#44 Posted by: Toohat Posted at: 2018-08-04T02:09:20.510Z Reads: 24

```
Will this https://www.amazon.ca/DSD-SH-HC-08-Bluetooth-Transceiver-Compatible/dp/B01N4P7T0H/ref=sr_1_2_sspa?s=electronics&ie=UTF8&qid=1533348277&sr=1-2-spons&keywords=bluetooth+module&psc=1 Bluetooth Module work with the FOCBOX?
```

---
## \#45 Posted by: Andy87 Posted at: 2018-08-04T04:44:50.314Z Reads: 24

```
I have this one
http://s.aliexpress.com/mIviqeUn
Works great with my iPhone and should work with android too.
If you want to use the metr app than you need to buy there Bluetooth module. The standard modules doesn’t work with it.
```

---
## \#46 Posted by: telnoi Posted at: 2018-08-04T07:19:06.044Z Reads: 24

```
[quote="Namasaki, post:38, topic:63099"]
For a mountain board or a street board with larger than 90mm wheels, I would try to get some 90C or higher.
[/quote]

Depends on the capacity. 2s2p 8000mah 30c (16ah 10s) delivers more than enough for a dual set to 60A, even for steep off-road hill climbs (mine last 5 minutes). Never had them overheat or suffer from severe sag.
```

---
## \#47 Posted by: Namasaki Posted at: 2018-08-04T16:47:43.877Z Reads: 22

```
If your using five 2s2p 8ah/30C Lipo packs, 
That’s 10s 8ah not 16ah
A 2s2p 8ah pack will have four 4ah cells, not four 8ah cells. 
A 10s/8ah/30C  is going to have sag even on a street board. 
You might not notice voltage sag while riding. 
You have to monitor your battery with a voltage meter while riding to see it.
My 10s/5a/60C sags about 1V  going up steep hills with 90mm wheels and 15/40 gears. 

Voltage sag will affect performance a little but it will affect range even more.
```

---
## \#48 Posted by: telnoi Posted at: 2018-08-04T19:23:11.216Z Reads: 22

```
Sorry, meant 16ah. 4x5s 8000 mah/10s configuration.
```

---
## \#49 Posted by: Namasaki Posted at: 2018-08-04T23:57:08.634Z Reads: 19

```
[quote="telnoi, post:48, topic:63099, full:true"]
Sorry, meant 16ah. 4x5s 8000 mah/10s configuration.
[/quote]


You said 2s2p packs 8ah/30
```

---

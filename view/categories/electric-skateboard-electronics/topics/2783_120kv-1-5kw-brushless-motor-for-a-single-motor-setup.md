# 120kv, 1.5kW brushless motor for a single motor setup

### Replies: 33 Views: 8374

## \#1 Posted by: Timur Posted at: 2016-05-01T18:05:07.612Z Reads: 237

```
Hello guys, I am a newbie in e-skating and actually also in skating world. Nevertheless I am to building an e-longboard. I need an advice regarding a motor. I am proposed the brushless D-Power BL 6362/120 motor, I guess some kind of German brand, I am located in Berlin. Basically specs are the following: 
- dimensions: 62 x 60 mm
- weight 550g 
- 120 kv
- 1500 W
- battery support up to 12s
- price: 40 euros = 46 USD
<img src="/uploads/db1493/original/2X/6/69031aef07b95407aa89f42577b8d01dd49136c9.png" width="408" height="336">

I wonder if this motor is ok for my setup? I've learnt that the less kv i have, the higher torque and lower max speed I get. However when I make some calcs with a standard variables like 15 teeth pinion and 36 teeth spur, 83 mm wheels and 24V battery I get 19 km/h as a max speed. I wonder if that's acceptable (pls keep in mind I have no clue how fast it means since I tried skate/longboarding 3-4 times).

The items I already have in a setup are:
- 83mm abec wheels
- 27 cm long, 9 mm wide, pitch 5 belt

I also understand that I can theoretically increase max speed by using different spurs and pinions however not sure that the length of my belt (27 cm) allows that.

What would be a difference if I use for example this: http://alienpowersystem.com/shop/brushless-motors/alien-5065-fr-outrunner-brushless-motor-270kv-2000w/ 
or this motor: RC C6364 245kv 
<img src="/uploads/db1493/original/2X/9/93aa02513b6ddd85fa587c08aaf6710f2200028f.png" width="690" height="387">

thanks in advance!
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-05-01T18:51:27.233Z Reads: 222

```
Hey bro...

Let's start here....use a 70-75 efficiency 🤘🏻


http://toddy616.blogspot.ca/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#3 Posted by: Timur Posted at: 2016-05-01T19:16:45.590Z Reads: 219

```
Hi, Michael! Thanks a lot. That's what I get with the most standard numbers and 120kv:

<img src="/uploads/db1493/original/2X/f/fcd842fd7e0324b4a861069ede0789d98000d6b6.png" width="322" height="439">

Does it make sense? I mean I read couple of sources stating "buy the lowest kv motor you can since max speed isn't that important as torque". So I would assume I would get a lot of torque, in other words I would be accelelrating very fast with 120kv motor, however in order to get higher speed (than 17 km/h) I'll have to choose different pulleys or higher voltage battery, right? Is there any other principal advantage of having a high torque motor except getting faster acceleration? E.g. how would this motor behave when it needs to go uphill?
```

---
## \#4 Posted by: makevoid Posted at: 2016-05-01T19:57:14.909Z Reads: 198

```
Yes, more torque = more power to go uphill too.
The problem is that with 17km/h max speed you may get bored too quickly.
Almost everyone will suggest you a motor around 190-200kv or getting a 12S battery if your kvs are that low with that motor.
Also your motor power should be probably > 2000w if you want enough power, also it depends if you're hevvy or not, and how high are the hills you want to go onto, if you're ~60kg and you keep high torque then it will be ok.

If you go with the second instead you will have more power (2kw instead of 1.5kw) but then you'll may need to stick with a 6S setup because a 12S the torque may be a bit too low? Also the motor is small (50x65mm) so it could overheat. 

Many people from this forum will suggest you the SK3 192kv from hobbyking: 
http://www.hobbyking.com/hobbyking/store/__672__663__Electric_Motors-63mm.html or the rspec+ from enertion 6372 if you have the $$

post how much you weigh and if you need to go up big hills
```

---
## \#5 Posted by: mohammedex Posted at: 2016-05-01T20:08:26.590Z Reads: 181

```
How much do you weigh?

I would say that if you weigh less than 150kg then 120kv is waaay too low if you only plan on running 6s. When I started eboarding I had little experience with skate/longboarding in general and my board could do about 25 km/h and after just a few weeks I started gaining more confidence and yearning for more speed. 13km/h will feel like a toy after a very short time.

If you weigh 70-80 kg or less then I'd recommend a motor with around 250-280 kv. It will still give you plenty of torque and a better top speed with those gears.


Of course you could also run your motor in a 12s config for more top speed + more torque. Low kv is generally good, but you shouldn't go too low.
```

---
## \#6 Posted by: makevoid Posted at: 2016-05-01T20:32:58.396Z Reads: 166

```
am I wrong or if you go from 6S to 12S the torque actually decreases because of the RPM increase?

> Power (watts) = Volts * Amps * motor efficiency 
> Torque = (Power*60)/(2*pi*RPM)

The RPM with higher voltage increases so the torque lowers, isn't it?
```

---
## \#7 Posted by: mohammedex Posted at: 2016-05-01T20:44:03.631Z Reads: 153

```
As far as my first hand experience and knowledge goes, going from 6s to 12s theoretically means double up on torque and max speed and it halves the used amps.

I don't know about the fancy mathematical formulas tho :sweat_smile::sweat_smile:
```

---
## \#8 Posted by: makevoid Posted at: 2016-05-01T20:50:43.091Z Reads: 148

```
[quote="mohammedex, post:7, topic:2783"]
I don't know about the fancy mathematical formulas tho :sweat_smile::sweat_smile:
[/quote]

I don't know either :sweat_smile::sweat_smile:, I just found them online and now I'm curious to know if really everything is doubled so there's basically no point of running on low voltage, if somebody can explain :D
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-05-01T20:54:05.374Z Reads: 143

```
The lowest I'm going is 149kv with the Turnigy Sk....but I'll use 12s with a 16/36
```

---
## \#10 Posted by: Timur Posted at: 2016-05-02T02:25:06.746Z Reads: 129

```
Hey guys, thx a lot for all the answers. I am about 72-75 kg, hills would be an exception rather than EV every day practice, but nevertheless good to be able to climb some of them I guess. Generally not steep.
```

---
## \#11 Posted by: Timur Posted at: 2016-05-02T02:34:06.695Z Reads: 132

```
I am located in germany. I asked about this 120 motor only bcoz it's super affordable since it s private sale however motor is new and I can get it quickly.  The next cheapest motor is 62-70 euros. Anyways none of famous hobbyking turnigies are in stock. Another option is probably this: http://m.ebay.de/itm/RC-C6364-245kv-Brushless-Outrunner-Motor-/152069194891?_trkparms=aid%253D222007%2526algo%253DSIC.MBE%2526ao%253D1%2526asc%253D20150519202354%2526meid%253D498325e53a6b4c559ea96df5b8b66b19%2526pid%253D100408%2526rk%253D4%2526rkt%253D21%2526sd%253D161988186137&_trksid=p2056116.c100408.m2460.

Wow sorry for this... I am typing from my mobile! :slight_smile: or motors from aliendrive. They seem to have couple in stock. I found one from aliexpress ad well but I am kinda reluctant to trust Chinese also those customs payments I guess.
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-05-02T02:43:19.327Z Reads: 123

```
Bro...spend your good Euros on something else...it may be a great deal...but it's less than ideal for what you want to use it for....

But move to a kv Range I would say...149 low and at the most 270kv 

There are plenty of diffrent motors and price points
```

---
## \#13 Posted by: Timur Posted at: 2016-05-02T08:56:32.341Z Reads: 116

```
[quote="makevoid, post:6, topic:2783"]
Power (watts) = Volts * Amps * motor efficiency Torque = (Power*60)/(2*pi*RPM)
[/quote]

When I look at these formulas, it seems that torque wont change, bcoz RPM = KV * Voltage and power = current * voltage, if we fit those two equations in the torque formule, the those voltages would just "remove" each other - sorry I don't know the correct English word, hope you get what I mean. 

May be I am wrong, just my opinion.
```

---
## \#14 Posted by: Timur Posted at: 2016-05-02T08:58:09.894Z Reads: 109

```
My problem is that I cant  find the online sources to order those motors... I need delivery to Berlin.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-05-02T09:39:15.643Z Reads: 111

```
I hear you mate...we don't have such problems here in the US...
```

---
## \#16 Posted by: BoardAdmin Posted at: 2016-05-02T12:22:14.132Z Reads: 108

```
Hey im from germany too. 
You could visit the german forum elektro-skateboard.de . There are also a few people from berlin and maybe someone is selling a motor in the market.
```

---
## \#17 Posted by: bigben Posted at: 2016-05-02T14:45:48.359Z Reads: 108

```
Had a recent email conversation with Bruno from alien drive systems and he assures me all his motors are in stock even though it doesn't show this on the website. 
Could be worth dropping him an email?
```

---
## \#18 Posted by: Timur Posted at: 2016-05-05T11:05:09.743Z Reads: 105

```
Thank you for valuable advice!
```

---
## \#19 Posted by: Timur Posted at: 2016-05-05T11:08:09.023Z Reads: 103

```
Thanks, i am familir with this forum as well! :) I actually started the similar topic there and got some good input! Shortly: seems like motor should be ok if I use a high voltage battery like 12s. But I still wanna look at the cost factor. Here is the thread:

http://www.elektro-skateboard.de/forum/szene-talk-63/120kv-1-5kw-motor-ok-fuer-single-motor-setup-5430.php

There is some English at the end - guys were tired of my broken German... :)
```

---
## \#20 Posted by: fraannk Posted at: 2016-05-11T21:15:46.308Z Reads: 92

```
I did a lot of reading and I can't figure out what gearing to use... I would like to have about 30 km/h as top speed, and decent amount of torque, can you help me? Thanks
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-05-11T22:38:56.152Z Reads: 88

```
<img src="/uploads/db1493/original/2X/e/ec07dfb359ffdb439b67c11d4998a29b12867533.png" width="281" height="500">

With stuff u can buy off the internet easy....

This is based on this thread using 12s 120kv
```

---
## \#22 Posted by: DrYou Posted at: 2016-05-13T00:14:25.020Z Reads: 81

```
I'm in the US and having issues finding motors in stock as well. There are some 149kv's last time I checked but don't know if that's too low. I'm larger, 235 lbs.
```

---
## \#23 Posted by: willpark16 Posted at: 2016-05-13T04:14:19.754Z Reads: 78

```
work great for ur weight
```

---
## \#24 Posted by: itsmikeholland Posted at: 2016-05-19T05:43:46.834Z Reads: 71

```
Hows your building coming along? I'm also in the 149kv 12s crowd, we seem to be a daring minority here!
```

---
## \#25 Posted by: Michaelinvegas Posted at: 2016-05-19T06:00:34.764Z Reads: 69

```
Lol oh shit I just picked up one of @chaka's new motor offering... Also picked up an 18t  
Are u home I was gonna ride tonight
```

---
## \#26 Posted by: itsmikeholland Posted at: 2016-05-19T06:38:38.033Z Reads: 64

```
is....is this an e-skate booty call?
```

---
## \#27 Posted by: Michaelinvegas Posted at: 2016-05-19T06:39:09.813Z Reads: 62

```
Haha yeah u down??

202020020
```

---
## \#28 Posted by: itsmikeholland Posted at: 2016-05-19T06:42:30.943Z Reads: 60

```
I would totes be down but I'm still waiting on my VESC to come in the mail! Is you 149kv rig up and running?
```

---
## \#29 Posted by: Mobutusan Posted at: 2016-05-19T06:56:14.386Z Reads: 61

```
You filthy little ESkanks...
```

---
## \#30 Posted by: Michaelinvegas Posted at: 2016-05-19T06:56:58.214Z Reads: 60

```
Lid ur home I'm gonna ride by and drop off the motors
```

---
## \#31 Posted by: itsmikeholland Posted at: 2016-05-19T07:01:03.952Z Reads: 60

```
Yooo I don't think you're talking to who you think you're talking to! I'm a new user in LA! If you're in Vegas thats quite the trip!
```

---
## \#32 Posted by: Michaelinvegas Posted at: 2016-05-19T07:03:08.640Z Reads: 61

```
Oh hahaha I need glasses I thought I was talking to @thisrealhuman haha .... And his name is Mike hahah
```

---
## \#33 Posted by: Michaelinvegas Posted at: 2016-05-19T07:07:38.233Z Reads: 58

```
Yeah I don't have that many lipos lol
```

---

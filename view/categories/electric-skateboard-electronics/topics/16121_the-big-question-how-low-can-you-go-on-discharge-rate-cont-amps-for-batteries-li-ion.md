# The big question - How low can you go on Discharge rate (cont amps) for batteries (li-ion)?

### Replies: 37 Views: 3320

## \#1 Posted by: Okami Posted at: 2017-01-15T02:18:26.007Z Reads: 224

```
Hi! I think this topic has been brought up many times but I have not heard a somewhat ''definitive'' answer to this one..

So - **what would exactly be the ''minimum'' pack size / discharge rate to go with?**

I know there are many variables in this one (wheel size, terrain, weight of rider, hills, voltage etc) but as we have seen, there are these chinese and even some ''american'' commercial boards which use a lot less cells than we do here on the forum..

So my question is - **what Cont Amp rating battery pack to go for**, _if an average user wants only 20-30kph ''regular'' speeds, and, perhaps, only, occasionally push till 40kph (if his board is able to) ?_

This is without hills, I can take some general setup, like 83mm wheels, 2.25(?) - 16/36 ratio, perhaps 90kg total weight (board included), 10s system.. 

So yeah, would like to hear the answers to this one :slight_smile:

---
Otherwise, a poll might be a good idea to collect info about all sorts of battery (especially li-ion) ppl tend to use here :slight_smile:
  
If this discussion does not go well or steer in the right direction, I might consider to just close it.. till someone else comes with the answers..

I know all of this can be proven / tested with a simple vesc telemetry app/data collection but I wanted to hear the opinion, too... besides the reason that I'd need to ask someone to log the data for me and have the right setup to make the test :)
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-01-15T02:38:09.666Z Reads: 203

```
10S3P for cruiser. 2160 watts
10S4P for power.  2880 watts
10S5P for performance. 3600 watts

But with a gearing for 40km/h and your chilled riding style a 10S3P would be enough.
```

---
## \#3 Posted by: Okami Posted at: 2017-01-15T02:50:51.808Z Reads: 203

```
2000w still seem quite a lot.. for ''normal'' cruising, it looks like it is sufficient to have around 300-400w available.. 

Anyways, wont argue, as I understand I should investigate some of these vesc log/monitor videos more closely to look at the data..

Me, included, 800-1200w seems like enough in some scenarious, and at the moment, im having a mountainboard, so for longboard the wattage might be even lower, I think.
```

---
## \#4 Posted by: PXSS Posted at: 2017-01-15T02:54:15.459Z Reads: 199

```
Depends on a lot of factors like you said down to the cell you use. 

For continuous power:
10S3P 25R: 600W
10S4P 25R: 800W
25Rs although they have a high max power output they dont do too well above 7A/cell due to voltage drop. 

Now if you use HG2s, 30Qs or VTC6s. You can do hogher continuous rates.
```

---
## \#5 Posted by: DeathCookies Posted at: 2017-01-15T02:56:41.765Z Reads: 190

```
i would change the verding. power seems to be more aggressive than performance. just change these two words but they describe it very well!
```

---
## \#6 Posted by: Okami Posted at: 2017-01-15T02:57:53.335Z Reads: 182

```
That's something I wanted to see more likely!

@PXSS thanks for pinning out the 7A discharge curve for the samsung's 25r, had not heard/seen before about it :slight_smile:

So, essentially to mitigate (lower) the voltage sag for 25r's, users would essentially use only  less than a half of their rated cont discharge.

Which would translate to 21A/3P and 28A/4P. Will probably look up some more datasheets after you mentioned this :slight_smile:
```

---
## \#7 Posted by: DeathCookies Posted at: 2017-01-15T03:04:53.433Z Reads: 161

```
A boosted board has plenty of power. Not the most power but enough for good riding. It only has a 1000w motor (or two).
```

---
## \#8 Posted by: PXSS Posted at: 2017-01-15T04:16:15.490Z Reads: 157

```
Plenty of discharge curves data on lygte-info.dk
Henrik (the guy that runs the site) is awesome too, He won't mind sharing any of his work. 

I've reached out to him several times to confirm my own tests and discharge models.
```

---
## \#9 Posted by: Okami Posted at: 2017-01-15T04:24:10.875Z Reads: 154

```
Im not sure how but personally I think we would need to develop a model at what criteria/scenarios what cells/conig is best suited.

It somehow seems that ebike builders dont have such a hard time deciding what cells to use as they also usually have quite big capacity packs.
```

---
## \#10 Posted by: PXSS Posted at: 2017-01-15T04:29:05.740Z Reads: 147

```
I started on a calculator but am out of town for the next 2 weeks flight testing. E-bike builders have more space/less power requirement. They mostly use GA cells. Most of their packs also have at least twice as many cells so yeah. Not that big of a deal when they're drawing similar maybe slightly higher amounts of power
```

---
## \#11 Posted by: Okami Posted at: 2017-01-15T04:35:20.161Z Reads: 147

```
Yes, plus they have reliable human power helping the motor of about 200w-300w in power (internet stats).. :D

I think i saw the power demand for bicycles somewhere and it was quite similar to what elongboards consume (10wh/km - 25-30kph avg)

Of course with higher speed wh consumtion goes up

--

@PXSS ok please post / share it once you get back. If it is somewhat completed or something others have not done yet, then it might be really useful
```

---
## \#12 Posted by: DeathCookies Posted at: 2017-01-15T09:40:02.376Z Reads: 137

```
It is hard to tell how low you can go with the continuos discharge... 
I (60kg 1,73m) have a Mini cruiser, 90mm, 15/36 teeth, 149kv FOC, 12S and went up to 30km/h and had only a peak of 10A/500W!
<img src="/uploads/db1493/original/3X/7/9/7971260cc7e5a134e8868bdb7b7b207b14aaad62.png" width="690" height="388">

Maybe i could have reached a higher peak but if i would limit The battery to 10A battery max i still could ride quite normaly
```

---
## \#13 Posted by: Okami Posted at: 2017-01-15T11:20:24.776Z Reads: 137

```
@DeathCookies Cool. Thanks for sharing this! That is one really low peak value!

I hope that more ppl show up who can prove that in some cases it is possible to "live" with such low discharge because their setups just dont consume anymore!

Wind is something we should take tests on! It may not be regular / strong enough for all cities/places but I just remember my times riding underpowered scooter/motorbike against the wind and not being able to achieve the max speed!

So this should be probably planned, that even if there are no hills, that this board will be strong enough against a wind blowing in the face! :)
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-01-15T12:35:26.092Z Reads: 128

```
@DeathCookies your setup is wrong. Great to see a picture of my app because it makes the analysis much easier. You have a higher Max Battery then Max Motor. Your should not do that. So you can switch the values to 100 Max Motor and 70 Max Battery. And in the picture you did not even touch the limits, so if you did a full throttle something must be wrong.
Tell me about your battery, motor and setup. 

@PXSS there is no need to reduce the max amps we draw from a Samsung 25R to 7A. Don't think in continious discharge curves because that doesn't happen when we ride.

To everybody. You can use the Samsung 25R with 20 A each cell when you have a 10S3P (60 A) or 10S4P (80 A). 
There are only a couple of things which limits those values.
1. It's too much power for you
2. You have a fuse that can't take that much current
3. You have a BMS in the discharge cycle  that can't take that much current

And to reduce it to 7A is like buying a Ferrari and reduce it to 100 km/h top speed because it might get a bit warmer when it goes faster. 
When you drive a car you don't push the throttle 100% all the time.
Only people who had problems with their battery are reporting about issues. And in the end they have a terrible gearing ratio, wrong cells, wrong VESC setup or no glue and not even a board.

And when you are worried about your batterys life cycle then ask yourself the question if you will ride more than 10000 km with that battery. If the answer is yes then you can be worried. If no then don't care about it.
```

---
## \#15 Posted by: DeathCookies Posted at: 2017-01-15T12:43:43.590Z Reads: 117

```
[quote="Ackmaniac, post:14, topic:16121"]
You have a higher Max Battery then Max Motor. Your should not do that. So you can switch the values to 100 Max Motor and 70 Max Battery.
[/quote]

Well.... My Motor is rated to 70A so i wont change it to 100A!
Why shouldnt i do that? I know that i should Set up a even acceleration like devin said but these settings are quite old. I wont reach The 100a battery because The 70a Motor preventing it? 

I already told you my setup.... Overread it? 
[quote="DeathCookies, post:12, topic:16121"]
I (60kg 1,73m) have a Mini cruiser, 90mm, 15/36 teeth, 149kv FOC, 12S
[/quote]
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-01-15T12:50:29.061Z Reads: 116

```
What Devin tells about even acceleration is wrong. Really sad to see that he can convince so many people with that stuff and that they believe it. Sadly English is not my first language so i don't sound that intelligent when i explain the stuff.

[quote="DeathCookies, post:15, topic:16121"]
I wont reach The 100a battery because The 70a Motor preventing it?
[/quote]
Correct

Did you do full throttle before the picture above?
```

---
## \#17 Posted by: PXSS Posted at: 2017-01-15T12:55:43.384Z Reads: 110

```
@Ackmaniac. Im sure his question asked what CONTINUOUS amp rating cell to choose. If we talk about continuous then yes 7-10A should be their limit if you want good endurance. 

Look at the discharge curves for 15A and 20A. They sag a lot. Voltage drop is 0.22V from 7-15A and 0.37v from 7-20A per cell.


And you should really think in how many times you ride not total distance as batteries only care about charge cycles but I agree you'll ride the same batteries for 2 years riding every other day
```

---
## \#18 Posted by: PXSS Posted at: 2017-01-15T12:58:18.342Z Reads: 107

```
Your battery limit should always be lower or equal to motor limit. That way theres less that can go wrong if something fails.
```

---
## \#19 Posted by: DeathCookies Posted at: 2017-01-15T13:24:57.678Z Reads: 107

```
Well, honestly i do not know if i had Full throttle. It is a Mini cruiser. The torque with this Setup so much that i did not need to go Full throttle. 
I just wanted to point out that you can achieve a good performance up to 30km/h with only 500W and 10A max battery! 

I will test this setup even more and make tests like Full throttle.

@PXSS yeah, better be Safe than sorry
```

---
## \#20 Posted by: DeathCookies Posted at: 2017-01-15T13:27:29.393Z Reads: 105

```
[quote="Ackmaniac, post:16, topic:16121"]
What Devin tells about even acceleration is wrong.
[/quote]

Why is he wrong? His math does make sense and it explains The boost many people get on a certain RPM!
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-01-15T13:38:20.083Z Reads: 97

```
The boost comes from the current noise on the VESCs sensors for current at around 85% duty cycle. Vedder mentioned that already. And if you have contentiously 2000 Watts from a stand still till close to max speed that would not result in a even acceleration. It would throw you off the board when you start and would be controllable at higher speeds.

To accelerate 80kg from 
 0 km/h to 10 km/h in 1 second needs 308 watts
10 km/h to 20 km/h in 1 second needs 925 watts
20 km/h to 30 km/h in 1 second needs 1542 watts
30 km/h to 40 km/h in 1 second needs 2160 watts
And wind, rolling, belt and bearing resistance is not even involved.
```

---
## \#22 Posted by: Pedrodemio Posted at: 2017-01-15T13:38:51.893Z Reads: 97

```
No it doesn't,

As I explained in one of the topics that he showed the math, we don't want constant power, we want constant acelleration

Torque is directly proportional to current, and power is voltage times current in electrical terms or torque times rpm in mechanical terms, with that and devins math, with a high power in low rpm it equals to off the chart torque that will throw you off the board

That's the beauty of current control, your acceleration remains almost constant, the current remains almost constant and power rises as the board speed up (in an ideal scenario, without drag forces)
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-01-15T13:40:18.511Z Reads: 93

```
@Pedrodemio LOL, we posted in the same second. But you are absolutely right. It's really strange that most of the times the wrong answer gets accepted by the community.

And when we add drag forces then we would need the opposite of Devins theory to have a even acceleration. But to set the Motor max higher then the battery max is quite nice because you have extra power at lower speeds without stressing the battery. And when the battery max sets the limit at higher speeds it is a smooth process instead of a boost. 
Also it would not be a boost, it would be a loss of power.
```

---
## \#24 Posted by: PXSS Posted at: 2017-01-15T15:03:38.453Z Reads: 90

```
I'm glad we all agree. Lol
```

---
## \#25 Posted by: Pedrodemio Posted at: 2017-01-15T15:44:10.311Z Reads: 91

```
Exactly, for constant power we have a decreasing acceleration as speed increase

Another problem that has to be considered is efficiency, if we pump 200A at 37V in our small motors and expects that all of that power is going to be converted in mechanical power we're going to have a bad time, just look at the power/torque/efficiency plots that @Mellowhas been doing of some boards, the efficiency at low rpm is very bad, we are basically cooking the motors
```

---
## \#26 Posted by: Okami Posted at: 2017-01-15T16:51:59.507Z Reads: 89

```
[quote="DeathCookies, post:19, topic:16121"]
I just wanted to point out that you can achieve a good performance up to 30km/h with only 500W and 10A max battery!
[/quote]

To drive the topic back to watts / amps abit more, I think I can remark here that some of these "old eboards" especially with these heavy Pb batteries still achieved 20-30kmh even if their motors were brushed and 400-800w. 

Of course I dont know their gear ratios and other stats but I think it should be left here that even such "seemingly low power" eboards were able to achieve such speed. I dont know their acceleration and sluggishness but I still think this proves the point. 

First evolve boards also did not use top notch motors but I think it once again proves it that if you are not after top stats/performsnce, it is possible to live with less.

Similar like comparing ferrari and perhaps some old 90's car. Both will get till 65mph/90kmh the difference will be in top speed and how fast they will get there + the durability too, probably.
```

---
## \#27 Posted by: Ackmaniac Posted at: 2017-01-16T01:26:08.249Z Reads: 84

```
300 watts is enough to reach 30 km/h on the flat. It only takes long to get there and you have a problem with hills.

If you want to know now how many watts you roughly need for which speed you can use this formula. 
(New speed / 30) * (New speed / 30) * (New speed / 30) * 300= watts at New speed

Please don't stone me to death if this is wrong.
```

---
## \#28 Posted by: Okami Posted at: 2017-04-06T21:57:39.681Z Reads: 74

```
Time to revive this thread!

**So how big battery (in terms of discharge) should someone get for going max 30-40kph with 8s setup and longboard wheels?**

My 'estimate'' is that 40-45A should be plenty already.. this gives a power output of:

~1150W (40A x 28.8v)
~1300w (45A x 28.8v)

~1720w (if 60A x 28.8v)

-----

**What Im still not sure though is, how much power hills might require?**

I tried to go up some very steep hill.. and max power I saw on my wattmeter was 42A with 6s setup, that is ~910w (@21.6v). And I dont have longboard wheels ;)

So I think with 8s, the amps might be in ~30A range? 
(900w / 28.8v = 31.25A)

My speed was not the highest though.. I think I managed to push 15kph instead of regular 25kph that i can do on flats.

--

Maybe @Ackmaniac and @rpasichnyk can share some data? U should have seen plenty of vesc data from the app you use :)
```

---
## \#29 Posted by: Pedrodemio Posted at: 2017-04-07T01:42:44.099Z Reads: 66

```
This is for 80mm wheels

on experience, i use 20A max on 10s and can climb 10% with ease, but no full speed

The problem in estimating the torque in a given moment is that most people use different battery and motor limits, and since the torque on the motor is directly proportional to the motor current, the max torque depends on the duty cycle

I don't know what the duty cycle is proportional to, the guys you mentioned should have a better take on this

<img src="/uploads/db1493/original/3X/3/7/37a9e7e54dc21e8edb793e45ce444601be533884.jpg" width="690" height="339">
```

---
## \#30 Posted by: jmasta Posted at: 2017-04-07T04:15:54.233Z Reads: 61

```
[quote="Okami, post:28, topic:16121, full:true"]
**What Im still not sure though is, how much power hills might require?**

I tried to go up some very steep hill.. and max power I saw on my wattmeter was 42A with 6s setup, that is ~910w (@21.6v). And I dont have longboard wheels ;)

So I think with 8s, the amps might be in ~30A range? 
(900w / 28.8v = 31.25A)[/quote]

I was surprised to find my 12S setup only needed about 1000W  (20-25A) to climb the steepest hill near my place. I go into the hill around 20mph and there is some slowdown. But I bought wider belts/pulleys, and the enhanced torque transfer should allow me to pull enough power to maintain my speed up that steep hill
```

---
## \#31 Posted by: Okami Posted at: 2017-04-07T04:17:54.179Z Reads: 59

```
@jmasta  Thanks for response! This is some solid data I was looking for! 

The speed you mention also sounds pretty good for the amount of power it required for you to go up that hill
```

---
## \#32 Posted by: Maxid Posted at: 2017-04-07T06:10:22.239Z Reads: 60

```
The slow down is probably due to voltage sag not your belts. Or did you have slipping issues?
```

---
## \#33 Posted by: jmasta Posted at: 2017-04-07T06:25:14.170Z Reads: 57

```
Some of it would be to voltage sag, but it's primarily a slipping issue. I had to throttle back my battery amps to limit the current/torque.  The SK3 6374 149kV can produce more power than my belt can transmit.  It's a 3/8" XL belt, which from my memory is only rated for something like 1-1.5 hp.  Replacing them with 15mm GT2-5mm  (improved version of HTD-5mm), which are good for 3 hp

1.34 hp is 1000W, so those charts I stored somewhere in the back of my brain seem to match reality
```

---
## \#34 Posted by: Maxid Posted at: 2017-04-07T06:31:14.460Z Reads: 58

```
ah okay - it sounded like you just went on full throttle and still slowed down. That is why I said voltage sag is the issue here. If you indeed have the belt slipping then you obviously have to take care of that first :smiley:
```

---
## \#35 Posted by: PXSS Posted at: 2017-04-07T11:54:29.930Z Reads: 57

```
[quote="jmasta, post:33, topic:16121"]
Replacing them with 15mm GT2-5mm  (improved version of HTD-5mm), which are good for 3 hp
[/quote]

Cool stuff I wasn't aware of. I might give these a try! Thanks
```

---
## \#36 Posted by: saul Posted at: 2017-04-07T22:08:07.158Z Reads: 50

```
[quote="Okami, post:28, topic:16121"]
My 'estimate'' is that 40-45A
[/quote]

You got that right. My 8s needs 45a battery to get hills.
12s only needed 25-30
```

---
## \#37 Posted by: Okami Posted at: 2017-04-07T22:21:41.607Z Reads: 49

```
@saul  Thanks for the info! The more info we gather, the better!

So the one who builds 8s setup and has some hills to conquer, could go with 60A battery to have some headroom for the hills, even if general riding on flats, probably, wont take more than 20A day to day.

Would you be kind enough to pinpoint in which location / region you reside? 

Or at least pinpoint how steep hills you got, since the geography around the world seems to shift quite dramatically in regards to terrain :)
```

---

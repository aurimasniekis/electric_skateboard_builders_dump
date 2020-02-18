# High C-rating means good quality battery?

### Replies: 14 Views: 1721

## \#1 Posted by: GunnarK Posted at: 2017-08-05T09:52:03.458Z Reads: 166

```
Hi guys I just found this website from a YouTube video from this guy called Dylan Kowalski (https://youtu.be/mj96BjGx1n0). He reviewed this esk8 called Meepo from a builder living in China, seems like an 'ok' esk8 but then I went to check his website and found this li-ion battery 10s2p with Samsung 18650s with a BMS installed already!
Check out this link
https://kieraneboard.myshopify.com/collections/frontpage/products/battery-10s2p-36v-4-4ah-samsung-18650-5c

I'm building my first esk8 at the moment and was almost going to buy 3 3s turnigy 5ah 45c batteries (https://hobbyking.com/nl_nl/turnigy-nano-tech-5000mah-3s-45-90c-lipo-pack.html?wrh_pdp=3).
But this li-ion battery got me hesitating. What do you think?
Should I go for this 10s2p battery?

It seems like a legitimately good option!

Thanks in advance

EDIT: this topic used to be about above mentioned li-ion battery but turned into a discussion/advise topic about what a high c-rating automatically means a good quality battery. And wether or not to invest in a higher c-rated one.
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-08-05T10:13:57.006Z Reads: 156

```
The best solution in this case with those two choices is to use the lipo batteries. I really can't see the 10s2p pack performing well at all. They give you the c rating as well. 4.4ah x 5c is 22amps continuous. This will lead to huge voltage sag and poor performance as well as decreased range. Everything will get hot and struggle to move you along. The lipos are more or less 225amp constant. Even with less volts the lipos will outshine the 10s2p pack.
```

---
## \#3 Posted by: GunnarK Posted at: 2017-08-05T10:17:11.582Z Reads: 152

```
Ah yes you're correct.
Should have read better, thanks!
```

---
## \#4 Posted by: darkkevind Posted at: 2017-08-05T10:20:03.426Z Reads: 150

```
That pack is going to be terrible and have massive voltage sag.
With li-ion the best discharge (c) rate is around 20A, for this you want a minimum of 4p. I'm using 3000mah HG2's that have a 20A discharge rate in an 8s4p configuration which gives me a 12ah battery pack that can discharge at 80A. There's very little voltage sag at all!
```

---
## \#5 Posted by: GunnarK Posted at: 2017-08-05T10:51:02.170Z Reads: 132

```
Sounds great! Costs a lot of money I reckon?

How does one calculate/estimate the voltage sag?

Also, maybe a bit off-topic:
- Is there a ceiling to the discharge rate with lipos? For example 35c is the most cost/performance effective. Buying a battery with higher discharge rate is a waste of money?
- Does the c-rating somewhat resemble quality of a battery? So buying a high c-rated battery could mean longer lifespan and less prone to dead cells? I understand that a c-rating of 35 will get less warm than a 25 rated battery.
```

---
## \#6 Posted by: darkkevind Posted at: 2017-08-05T11:01:16.968Z Reads: 117

```
You need to look at the max amp rating of your motor(s) (combined if dual setup), anything more than that is a waste.
```

---
## \#7 Posted by: GunnarK Posted at: 2017-08-05T11:44:41.075Z Reads: 104

```
Ok so a 20c would be more than sufficient for a single motor setup (80Amps)
5ah x 16c = 80

Why would one still recommend to go for something like a 40c battery if it's a waste?

EDIT: maybe so one is able to get the burst of a 20c at a continuous with a 40c battery?
```

---
## \#8 Posted by: i2oadsweepei2 Posted at: 2017-08-05T11:50:25.537Z Reads: 96

```
There isn't really a way to calculate the sag because of all the variables like components used like wheel size, gearing and others like your weight, uphill/downhill and terrain. I think you could try and estimate it through the advice of others who have experienced it. Or possibly distance travelled until low voltage cutoff to find the watt hours per kilometre or mile. I've used nanotechs for many years and they have proven to me at least to be one of the better lipo cells. 35-70c would be my choice as well. Zippy's are ok too. I have been eyeing up the 4s 8000's for some time.

At the moment I'm not using lipos for either of my rides.
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-08-05T11:51:34.810Z Reads: 89

```
I would say 30c as a safe minimum and anything above that. I would think that higher c rating should give better efficiency and provide longer range with less sag.
```

---
## \#10 Posted by: GunnarK Posted at: 2017-08-05T12:11:59.775Z Reads: 87

```
I guess you're talking about these?
https://hobbyking.com/nl_nl/zippy-flightmax-8000mah-4s1p-30c.html
Looks like the burst is only 33% the continuous discharge is. I thought bursts were almost always twice the continuous rate?  `"30C Constant / 40C Burst"`

> I would say 30c as a safe minimum and anything above that. I would think that higher c rating should give better efficiency and provide longer range with less sag.

Thank you for helping me out. I think I'll go for the 45-90c turnigy nano tech since the cost per battery is only 3 euros higher than the 35-70c version!
Would you recommend this?

Check it out here if you'd like:
35-70c - https://hobbyking.com/nl_nl/turnigy-nano-tech-5000mah-3s-35-70c-lipo-pack.html
45-90c - https://hobbyking.com/nl_nl/turnigy-nano-tech-5000mah-3s-45-90c-lipo-pack.html
```

---
## \#11 Posted by: i2oadsweepei2 Posted at: 2017-08-05T12:18:36.958Z Reads: 77

```
Ya those are sweet. Only 35mm thick. Also at 30c x 8ah that is 240a continuous. It's actually probably less, but still more than enough for esk8 IMO.

Either of those nanotechs should be fine. How do plan to charge them? Will you use 9s now?
```

---
## \#12 Posted by: GunnarK Posted at: 2017-08-05T12:32:48.390Z Reads: 72

```
I want to install a BMS and use a ebike charger or something. I don't want the hassle charging each battery individually

I'm dubbing between 8s and 9s for these reasons:
1. the 2x 4s 8ah-30c; you don't get the speed but a lot more range (top speed: 19.76 mph - 31.8 km/h)
2. the 3x 3s 5ah-45c; gives more speed but less range (top speed: 22.23 mph - 35.78 km/h)

I found this calculator online which gives an estimate about the speed performance of a particular setup
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":9,"motor-kv":190,"system-efficiency":90,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":80}|
The filled-in values are the ones that I'll be having.
I live in Holland so almost everything is flat.

I do wonder if I would want the 5kmph (2.4mph) increase in speed giving a top speed of 35.78 kmph (22.23 mph)
```

---
## \#13 Posted by: i2oadsweepei2 Posted at: 2017-08-05T12:40:50.409Z Reads: 70

```
I should have said those are sweet based on what I am reading. I haven't tried them yet.

Application is everything
My turnigy Nanotech 5s 5000mah 65-130c batteries give me different performance for the different things I use them for. 

In my 43" Aeromarine Challenger Boat I use 2 x 5s in series and get 4 minutes of runtime. The boat pulls over 7000 watts.
In my RC monster truck using one 5s I get 15+ minutes of runtime using a neu motor 1515 1yf
For my electric skateboard 2x 5s in series 230kv 16/36 83mm wheels and me weighing at 216lb I get 45-60min of runtime or 16kms/10miles whichever come first. Depends on terrain.

20+ mph is very fast on a skateboard. Some people love the thrill. I have tried to keep mine in and around 20mph max. Never really cruise that fast. You can always increase your speed by going up a tooth on the motor pulley to 16 later on. 

Check out this thread for using a BMS with Lipos. Namasaki is the man for tips on installing those.
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014

Time to go play hamster on the treadmill. 

BBL
```

---
## \#14 Posted by: GunnarK Posted at: 2017-08-05T13:32:06.051Z Reads: 62

```
Wow those are some comparisons haha

I think I won't even be able to go faster than 20 mph since I plan on using it through the city most of the time.
Also esk8s aren't exactly legal in Holland. But from what I understand the cops won't make a big deal about it as long as you ride safely.

If there was a 4s 8000mah 40c battery I would be all happy

Found that thread already but thanks for reassurance!

Good luck!
```

---

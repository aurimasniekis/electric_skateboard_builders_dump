# DIY Trampa Urban Carver ESK8

### Replies: 21 Views: 1203

## \#1 Posted by: chocol4te Posted at: 2018-03-07T14:19:04.157Z Reads: 211

```
Hello!

If this is the right place for it, I was wondering whether anyone could look over my parts list and check if it's OK? I also have a few questions. I have a background in embedded systems as well as UASs but I am not sure how many rules of thumb translate across.

* Trampa Vertigo Urban Carver - Superstar 7 inch wheels and Yellow DAMPAs
* Trampa Urban Motormount - 15 tooth pulley
* 72 x Samsung INR18650-35E in 12s6p configuration
* FOCBOX
* Eskating PRO motors 6374 190Kv
* Nano-X remote

Is there any real difference between the 3 Urban Carver boards and also between Hypa and Superstar wheels?

Is it true that the pneumatic wheels are significantly less efficient than urethane 90mm wheels? The worst material I will be going on is cracked road, no gravel or dirt, so are 125mm "Gummies" a compromise?

Do I have the right voltage/kV/gear ratio/wheel diameter? I would like to be able to go up fairly steep (25%?) hills and although speed is not a priority, range is.

The motor is rated for 70A, but the FOCBOX says only 60A continuous, and the 6p battery configuration should be 60A max there as well, my assumption being that it is unlikely to be drawing 70A for long. What kinds of current should I expect from the motor?

Will I every need to upgrade to a dual motor system? I weight 75KG, and I want to be able to take my school bag with me (on a bad day 5kg).


Thank you so much for any advice/help! :)
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-03-07T14:24:25.015Z Reads: 200

```
Dual isnt necessarily necessary, but traction and braking will be alot better, compared to the single 

I know you had more questions, but I dont have time to answear them right now.(I’m sure some others will)
Hope this helps :grinning:
```

---
## \#3 Posted by: chocol4te Posted at: 2018-03-07T14:26:06.934Z Reads: 195

```
Thanks! Sorry about all the questions :D
```

---
## \#4 Posted by: cosmicc89 Posted at: 2018-03-07T14:54:00.776Z Reads: 191

```
Hey there @chocol4te I believe I can help as I have a similar setup.

The 3 urban boards have different trucks, one has a solid steel axle, second a hollow steel axle and the third has titanium axle and hardware. The differences are lower weight for more cost. Generally people feel the titanium is unnecessary unless you're riding in salty areas. The solid steel axle is best if you're going to be doing any jumps, and otherwise the weight reduction for the hollow steel is generally a good idea for the small increase in cost. 

Hypa wheels are all plastic, superstars are aluminum. people generally go with superstars even though they cost slightly more. I have superstars. I'm sure hypa wheels are great, but I decided on the added piece of mind of metal.

pneumatic wheels are less efficient, but I've pumped mine up to 60 psi and have noticed at most a 20% reduction in range and a bit less torque. But their vibration dampening outweighs these downsides since my area is primarily crappy pavement with some gravel. If the worst you're experiencing is cracked road, I would go with a big urethane wheel like the gummies, or a 97mm Sticky or clones depending on your budget.

As for your kv/voltage configuration, I recommend you spend some time with this calculator: http://calc.esk8.it/ to find the best ratios. Keep your erpm below 60k (this is a must!) and keep in mind that the higher your top speed, the lower your torque will generally be, so keep a good balance. 12S is great for tons of torque, 10S is a bit easier on the speed controllers due to the lower voltage, though tons of people run 12S with no issues. My single motor urban carver can go up 25% grades, albeit slowly. My area is almost entirely flat, so I'm happy with a single motor. If hills like this are common in your area, I recommend you go with dual drive.

The motor will only draw something like 60A for only a couple seconds at a time, typically people see less than 20 A continuous. Keep in mind that the equipment is rated for spikes of current higher than their continuous ratings.

I weight 85kg, and on flat ground with a single motor I don't have any issues and have plenty of torque. I'm not going 60km/h or anything, I don't really ever go more than 40km/h so my setup works great.

Here is my board if you're interested: 
https://www.electric-skateboard.builders/t/identity-crisis-hybrid-class-trampa-urban-carver-10s-lipo-bms-vesc-200kv-single-motor-motorcycle-lights/41676
```

---
## \#5 Posted by: chocol4te Posted at: 2018-03-07T16:15:53.576Z Reads: 153

```
@cosmicc89 Thank you so much for your detailed reply, it is really helpful! I think the gummies might be the best option for me, and I live right by the coast so the titanium might actually be necessary. Thanks again! I love your build!
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-03-07T16:25:41.255Z Reads: 143

```
If you choose to go with the Ultimate/titanium, you’ll have the benefit of having a 9.25mm axle, which means you can use them with street wheels like 83-107mm superflyes!
```

---
## \#7 Posted by: Lukas Posted at: 2018-03-07T16:55:30.783Z Reads: 135

```
Do you want to mount the 72 cells on top or under your board?

If you want to mount under your board you have to consider that there is very limited space.
I think the biggest battery i have seen underneath a trampa yet was 12s5p.
But maybe i will work if you double stack them but then you would have to be aware of your clearence.
Another option would be to mount the FocBoxes on top :thinking:

Just keep this in mind :smiley:
```

---
## \#8 Posted by: chocol4te Posted at: 2018-03-07T17:01:10.645Z Reads: 135

```
@Lukas  Will do. Since I already have a 6s charger and it would be nice to occasionally use the batteries in my drones, I was thinking of making a 3 4s6p packs then wiring in series, but you're right, it will either have to be a very tight fit underneath, or I'll go the centre box route. I'd certainly like to leave the option of dual motors in the future and another 72 batteries will be cramped. :D
```

---
## \#9 Posted by: Acido Posted at: 2018-03-07T17:40:26.200Z Reads: 115

```
I crashed today because of lack of traction...definitely go dual its much much better, and since you have a huge battery its no biggie
```

---
## \#10 Posted by: FredrikHems Posted at: 2018-03-07T17:50:20.017Z Reads: 108

```
One thing you might wanna change is the battery cells to 30Q/VTC6.. The 35E are only good for 10A each , while the 30Q and VTC6 can do 20A. The 30Q also is just like 0.04£/cell more expensive
```

---
## \#11 Posted by: chocol4te Posted at: 2018-03-07T17:52:42.166Z Reads: 109

```
The data sheet shows that the 35E can do a 12A burst, and with 6 in parallel I though I would have enough? Will I have noticeably less range with the 30Qs?
```

---
## \#12 Posted by: FredrikHems Posted at: 2018-03-07T17:57:19.450Z Reads: 103

```
The range will probably be a little less, nothing extreme though.. The benefit of the 30Q will be less voltage sag and better performance, compared to the 35E
```

---
## \#13 Posted by: Der6FingerJo Posted at: 2018-03-07T18:05:13.554Z Reads: 107

```
Go with lower kv motors unless you want to hit more than 50 km/h which isn't really a thing on trampas as far as i know. Otherwise everything seems to have been said.
I would also recommend dual drive, might not need the power but the individual vesc will run cooler and braking is better as well.
```

---
## \#14 Posted by: chocol4te Posted at: 2018-03-07T18:06:33.088Z Reads: 107

```
Thanks, I'll make that change. (Also on nkon.eu when purchasing more than 10, the 30Q ends up being 0.15€ cheaper :D )
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-03-07T18:37:39.018Z Reads: 100

```
How are you gonna Get your pack build btw?
```

---
## \#16 Posted by: chocol4te Posted at: 2018-03-07T18:50:14.353Z Reads: 107

```
@FredrikHems I'm going to spot weld it myself
```

---
## \#17 Posted by: FredrikHems Posted at: 2018-03-07T18:56:53.519Z Reads: 107

```
Do you have a spot welder already?
```

---
## \#18 Posted by: chocol4te Posted at: 2018-03-07T19:02:19.789Z Reads: 107

```
@FredrikHems I plan on building a [car battery spot welder](https://www.youtube.com/watch?v=o1NFbchHeM8).
```

---
## \#19 Posted by: Sn4pz Posted at: 2019-02-28T19:24:21.066Z Reads: 47

```
How did this ever end up??? Im building something similar :)
```

---
## \#20 Posted by: chocol4te Posted at: 2019-02-28T19:38:59.428Z Reads: 45

```
Well, I ended up going with something pretty different: https://www.electric-skateboard.builders/t/lacroix-prototipo-aps-8072s-12s6p-30q-escape/63318. I like my build a lot, though I really wish I hadn't gone with the APS 8072S, it's a pretty crappy motor and I only found the bad reviews after buying :/
```

---
## \#21 Posted by: Sn4pz Posted at: 2019-02-28T19:42:56.348Z Reads: 45

```
Oh wow I dont know why I didnt recognize your username then :man_facepalming:

I want to see all the carver builds... I cant decide if i Want to keep it or go for a kaly deck o3o
```

---

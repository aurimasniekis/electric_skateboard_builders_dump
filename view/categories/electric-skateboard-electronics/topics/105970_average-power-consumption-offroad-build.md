# Average Power Consumption - Offroad build

### Replies: 10 Views: 102

## \#1 Posted by: pmouraguedes Posted at: 2020-02-13T18:39:04.876Z Reads: 45

```
Hi,

Recently finished a new MTB esk8 build, using 8 inch pneumatic tires and 2 x 2000 W 6354 motors.
I'm pretty chocked by how much it's draining the battery... I did a 6.5 Km ride and I got a 55 Wh/km average consumption and didn't even ride fast.

Can someone share their own numbers with a similar setup? 

Thanks,
Paulo
```

---
## \#2 Posted by: Okami Posted at: 2020-02-13T18:53:09.349Z Reads: 44

```
https://www.youtube.com/watch?v=WIdTK5-xKyg

@rich

There were a couple similar topics.. 

Did u ride off road? On street consumtion should be more like 20-30Wh/km, if you ride till 40kph or so, I think.. Off road it could be up to 55wh/km
```

---
## \#3 Posted by: Halbj613 Posted at: 2020-02-13T18:55:08.293Z Reads: 42

```
Yeah I am getting 25wh/mile on 6 inch and I thought that was bad

Also post this on esk8.news forum
```

---
## \#4 Posted by: Okami Posted at: 2020-02-13T19:02:00.048Z Reads: 42

```
For pneumatics that seems quite ok to me, if I convert to wh/km, you get ~16 wh / km.

With these 6inch airless tires, consumption for my friends board is like 18 - 22wh/km, even when riding below 35kph (below 22mph)
```

---
## \#5 Posted by: pmouraguedes Posted at: 2020-02-14T07:36:11.433Z Reads: 34

```
I do ride offroad but these numbers were taken on a asphalt ride and I was with my dog, so not fast at all :slight_smile:
<br>
I think I should be getting values in the thirties, 55 wh/km is really too high... I don't see any reasons why this is happening, the VESC configuration didn't report any problem, it seems everything ok. How could I troubleshoot this?
```

---
## \#6 Posted by: Okami Posted at: 2020-02-14T07:41:38.897Z Reads: 30

```
From where do u take your wh/km number? 

Do u have phone app using bluetooth or u got different datalogging?

55wh is too much for sure then.
 I would say number is doubled or there is something else going on.

U could also calculate used capacity directly, if u know how many km u rode and your charger has watthour/amp hour meter
```

---
## \#7 Posted by: pmouraguedes Posted at: 2020-02-14T08:09:01.419Z Reads: 28

```
Exactly, I'm calculating it like you do with a car :) <p>
I'm using a watt meter when charging. I just read the Wh and Ah that it took to charge to the same level it was, and before I recorded my ride with a standard app in my phone so I know how many km were done.
```

---
## \#8 Posted by: Okami Posted at: 2020-02-14T12:36:11.480Z Reads: 26

```
Well, in that case I would suggest to do straight road ride, for maybe a couple of Km and then measure the energy consumption.

Also, if the outside weather is cold im sure the battery will drain faster..

I havent really looked into this by much detail, but If im right, when riding out in cold, your battery could have 20% less capacity.. 

So, instead of example 10ah, it would get only 8ah out of battery.

And I guess when charging you would charge more than you actually drained.

But I havent really tested this but this is something worth looking into.

So in that matter, It would be best to measure **consumed** energy not the one you put back while charging.

---

Here's an article I found:

https://www.researchgate.net/post/How_much_energy_is_lost_when_charging_a_battery

But honestly, I would find someone who has better electronics knowledge and who can explain the Coulomb counter principle when charging. I suppose a wattmeter does count how many amps/volts goes to the battery = charged energy, but it might be that not all energy gets stored in the battery directly and some is lost in the process.

So here I dont know if wattmeter/charger can take this into an account or if the losses are bigger than 5%.

In my experience I think charged vs consumed shouldnt be more than 10% difference. But It could be more in cold weather, if what I said earlier is true. (needs more data from scientific sources)
```

---
## \#9 Posted by: itsrow Posted at: 2020-02-15T00:03:18.207Z Reads: 17

```
The losses in temperature, depending on battery chemistry, can be a hell of a lot more than 20% my LiPos get maybe 40-50% of their total capacity when they're taken into -20C for more than an hour or so, but no real degradation from the cold.  LifePO4 is where you want to be if you live more than an hour from the equator.
```

---
## \#10 Posted by: Okami Posted at: 2020-02-15T16:50:10.808Z Reads: 12

```
@itsrow  Hi, thanks for the input.

My 20% was a conservative amount for giving example, taking into consideration the temperature still could be +5 degrees C (~41F).

But yes, Ive heard below 0C degrees (36f) the capacity drops a lot more drastically and it is not advised to charge batteries at all, if temperature is below zero.. or should be done at low c rate at best.

Good point about Lifepo. Havent seen many builds for eboards with them but they are a thing in ebike/motorbike/e-car community for sure.

---
My final conclusion could be that @pmouraguedes rides in cold weather, his consumed energy is less than that charged back in battery or that his gps reading is off for distance he did. 

 So yes @pmouraguedes give more precise data and maybe we can work this out..

Otherwise im not sure the drag / inefficiency could be that big, that you get such high energy consumption.
```

---

# VESC cooling warning

### Replies: 28 Views: 2659

## \#1 Posted by: ThierryGTLTS Posted at: 2017-09-22T15:13:10.355Z Reads: 356

```
Please allow your VESC to cool down!

I'm almost sure that a lot of fried VESC come from bad cooling.

Heatshrink tube is good to protect from water, but doesn't allow Mosfet and DRV cooling.

VESC 6 and FOCBOX are well cooled.

Thierry
```

---
## \#2 Posted by: hexakopter Posted at: 2017-09-22T15:18:52.812Z Reads: 349

```
Normally the VESC decreases the current when a critical (adjustable in GUI) temperature is reached which is measured over a temperature sensor located nearly to the FETs. So it should not be possible to overheat when the temperature limits are set wisely.
Can you back up your "almost sure" with something?
```

---
## \#3 Posted by: ThierryGTLTS Posted at: 2017-09-22T16:51:15.712Z Reads: 344

```
You are right about the protection if the temperature rise is slow, and that's often the case with low to mid current motors.

But if it fast, and with high currents, the temperature of the die of the Mosfets will be much higher than the temperature of the sensor.

If you do a serious thermal analysis and take into account all the thermal resistances in your circuit model, you'll see that I'm right.

That's partly why the VESC 6 has been created.

Have a Nice Day.

Thierry
```

---
## \#4 Posted by: Namasaki Posted at: 2017-09-22T17:00:42.432Z Reads: 317

```
I'm running two builds with dual Vescs 
They are covered with shrink tube and inside a sealed enclosures and I have no over heating issues. 
I'm 195 lbs and I charge steep hills. 
The catch is that they are equipped with heat sinks. 
That is the way to keep your Vescs cool. 
Ollinboards was first to offer Vescs with heat sinks. 
Then came the focbox and then Vesc 6
```

---
## \#5 Posted by: hexakopter Posted at: 2017-09-22T18:45:44.394Z Reads: 305

```
[quote="ThierryGTLTS, post:3, topic:33716"]
You are right about the protection if the temperature rise is slow, and that's often the case with low to mid current motors.

But if it fast, and with high currents, the temperature of the die of the Mosfets will be much higher than the temperature of the sensor.
[/quote]


I dont think we are near the point that the temperature of the MOSFETs is far of the NTCs value. I have done a test with up to 120A motor current shooting the temperature in the temperature limit. You can read more about it here: https://www.electric-skateboard.builders/t/vesc-hw-4-12-temperature-comparison/23230
I dont think the temperature is off that much that it had destroyed a lot of VESCs as you stated. Let it be up to 5-10 °C difference max.
But feel free to make a serious thermal analysis and show us the results. :slight_smile:

@Namasaki 
[quote="Namasaki, post:4, topic:33716"]
The catch is that they are equipped with heat sinks.
[/quote]
Just equip them with heatsinks and then put them in heat shrink and inside a sealed enclosure isn't useful at all. You have a slightly higher thermal capacity, but if your heatsink is hot ones it will also take longer to cool down. Look at the link I posted above.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-09-22T20:09:55.793Z Reads: 263

```
[quote="hexakopter, post:5, topic:33716"]
Just equip them with heatsinks and then put them in heat shrink and inside a sealed enclosure isn't useful at all. You have a slightly higher thermal capacity, but if your heatsink is hot ones it will also take longer to cool down. Look at the link I posted above.
[/quote]
All of my Vescs came with heat sinks and shrink tube. 
I neglected to mention that the shrink tube is cut to expose the heat sinks. 
I put them in a sealed enclosure to keep them dirt and moisture free. I also neglected to mention that they are not stacked or stuffed tightly in with other components but they have a decent amount of space around them to allow for some heat dissipation. 
I apologize for not being more specific and for being a little misleading.
```

---
## \#7 Posted by: hexakopter Posted at: 2017-09-22T23:10:06.683Z Reads: 238

```
[quote="Namasaki, post:6, topic:33716"]
I neglected to mention that the shrink tube is cut to expose the heat sinks.
[/quote]

:grin: That explains a lot. Couldn't believe someone putting a heat sink on his VESC just to but a heat shrink over it afterwards.
What also explains why you don't have a problem with heat is the observation that you are draining relatively low max currents of around 26.3A motor current when referring to this post: [https://www.electric-skateboard.builders/t/6v-sag-too-much/32002/37?](https://www.electric-skateboard.builders/t/6v-sag-too-much/32002/37?)
When you are pulling over 60A you will see how important the airflow gets.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-23T01:29:30.499Z Reads: 223

```
How do you manage to pull 60a?
I've tested 6s going steep uphill with dual motors and only pulled 36a total from the battery.
```

---
## \#9 Posted by: ThierryGTLTS Posted at: 2017-09-23T15:41:28.822Z Reads: 218

```
I will do a more extensive post taking into account ambient temperature, current, voltage, switching frequency, and datashet of the Mosfet, because the problem is very complex.

And when someone  blow-up a VESC, it's often the result of many factors, not only temperature or current.

But it's always better to keep electronic cool.

Have a Nice W-E.

Thierry
```

---
## \#10 Posted by: High-roller Posted at: 2017-09-23T18:31:16.671Z Reads: 205

```
So do FOCboxes need external cooling, like an airscoop, over their heatsinks, or can I just put them in my enclosure and leave them like that?
```

---
## \#11 Posted by: hexakopter Posted at: 2017-09-23T22:09:14.420Z Reads: 209

```
I was talking about motor current, because that current flowing through the FETs is heating the VESC up. As you can see in the link I already posted above  (https://www.electric-skateboard.builders/t/vesc-hw-4-12-temperature-comparison/23230) Im not just pulling 60A but 120A for a short time when accelerating. 60A was just a example where good cooling starts to become more important in my opinion.

[quote="High-roller, post:10, topic:33716, full:true"]
So do FOCboxes need external cooling, like an airscoop, over their heatsinks, or can I just put them in my enclosure and leave them like that?
[/quote]
It depends on the motor currents that you will reach and for how long. If you are pulling just 26A like @Namasaki does you shouldn't have to much problems I think. The easiest way would be just log your temperature with something like the [metr.at](http://metr.at) bluetooth module where you would see when you are hitting critical temperatures.

@ThierryGTLTS Looking forward to your post. Great that you will investigate more on that topic. :+1:
```

---
## \#12 Posted by: Namasaki Posted at: 2017-09-24T00:21:58.326Z Reads: 184

```
I see, your talking about an E-bike pulling those high amps.
My examples are with an E-board.
```

---
## \#13 Posted by: ThierryGTLTS Posted at: 2017-09-26T16:03:07.933Z Reads: 174

```
It may take a few days.

Thierry
```

---
## \#14 Posted by: chaka Posted at: 2017-09-26T16:11:17.013Z Reads: 172

```
I am running one of my first VESC's in heat shrink on a single motor build. I regularly hit the thermal cutoff on a really steep hill just before I reach the top. This VESC has been in service for over two years!  I think you assume too much in regard to why a VESC will fail. 

The biggest cause for failure by far is improper installation followed by poor manufacturing and cheap components. You could run a VESC at 80 degree Celsius all day and it would be fine.
```

---
## \#15 Posted by: ThierryGTLTS Posted at: 2017-09-27T15:07:56.979Z Reads: 166

```
When you wanna have a very long lifetime (especially for electrolyic capacitors and semiconductors), you have to run them cool.

A well known engineering rule in the electronic industry says:

+10°C cut the lifetime by a factor of 2.

So you do what you want, but I don't recommand using the VSC at those elevated temperatures.

Thierry
```

---
## \#16 Posted by: chaka Posted at: 2017-09-27T17:06:41.010Z Reads: 158

```
I thought you were blaming MOSFET failure on heat? Are we talking about capacitors now? I agree cooler is better but you are off the mark on your original assumption. If you are having trouble with heat I suggest you switch to a dual motor drive or a directfet design with heatsinks and actively cool with a fan.
```

---
## \#17 Posted by: ThierryGTLTS Posted at: 2017-09-28T10:16:10.983Z Reads: 148

```
If you read my first post, I also include the DRV.

But I just wanna give advices after what I see here and elsewhere (industry and power electronic).

Some have troubles with Mosfets, others with DRV, others with capacitors.

Most of the resistors and MLCC capacitors are the only components that tolerate to work at high temperatures without premature failures.

As I said you can do what you want, no problem for me.
```

---
## \#18 Posted by: chaka Posted at: 2017-09-28T13:36:00.803Z Reads: 148

```
I know you have no issues with what I do but I do have issues with people spreading assumptions and stating them like facts without field testing on a skateboard. If a board is built with good specs and a proper gear ratio we actually do not see any issues with overheating or hitting the cutoff.

 Some of us have been at this for a long time and have "real world" experience with the current state of eskate. It is disheartening to see new members join only to spread advise based on assumptions. If your VESC is getting as hot as you say you have a problem somewhere else in your build, gear ratio too tall, heavy rider paired with a single drive or something else?

The fact is there are many people still riding on 2 year old VESC's who regularly push them to their limits. Are these people magicians, do the emit some protective force-field around them that protects electronics from failure or maybe it is because we are operating well withing the recommended temps for the components we use?
```

---
## \#19 Posted by: DilatedPupils Posted at: 2017-09-28T14:16:13.240Z Reads: 135

```
My 2 ollin vescs from 2 years ago are still alive and well on my trampa in a UK water proof case. 
I might be a magician.
```

---
## \#20 Posted by: ThierryGTLTS Posted at: 2017-09-28T14:42:40.831Z Reads: 139

```
It seems I'm not welcome altough my advices are also based on more than 30 years of electronic engineering experience.

So I will shut off my mouth.
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-09-28T15:03:38.423Z Reads: 144

```
@chaka @ThierryGTLTS hey guys come on, I think that everyone's had different experiences with VESC's and why they fail and everyone has a different opinion. I don't think anyone wants any hard feelings on here alright. 

Anyways originally my VESC was un shrink-wrapped   just sitting inside my enclosure and I was thermal throttling a lot with my Carvon V2 hub. Eventually I added heatsinks to both top and bottom side MOSFET's and added a small fan and I didn't have any problems after that. Now with my dual Maytech hubs with both my VESC's heatsinked and the fan blowing across both of them my temps don't even go above 40c.
```

---
## \#22 Posted by: GhettoFab.rictation Posted at: 2017-11-09T08:35:57.855Z Reads: 130

```
What fan do you use and do you use from the 5v on vesc? Where is the 5v at on vesc and could a person possibly use a fan along with a step up converter in parallel for light to see at night. Can you help me get a fan and aluminum cooler on mine? I'm a noob to installing them
```

---
## \#23 Posted by: GhettoFab.rictation Posted at: 2017-11-09T08:39:12.047Z Reads: 131

```
<img src="/uploads/db1493/original/3X/3/d/3d0795c390a18375d0bb57be0b496624288e74ea.jpg" width="281" height="500"> is this 5v at bottom?
```

---
## \#24 Posted by: GhettoFab.rictation Posted at: 2017-11-09T08:41:07.803Z Reads: 124

```
Here are my mosfets <img src="/uploads/db1493/original/3X/5/b/5be6bd67eb6f2ad0338f8ae8241e72759b841f03.jpg" width="281" height="500">
```

---
## \#25 Posted by: JdogAwesome Posted at: 2017-11-09T16:02:21.760Z Reads: 115

```
No I use a 12V fan as well as 12V LEDs and anything that needs 5V I buck down from the 12V main converter because it can take the high 50V input voltage of my 12S battery. For the heatsinks I just use some small ones I found in eBay, I'll get you the measurements in a little while if you'd like.
```

---
## \#26 Posted by: GhettoFab.rictation Posted at: 2017-11-26T10:43:37.769Z Reads: 106

```
I have these guys rated at like .02amps <img src="/uploads/db1493/original/3X/2/4/24b0efd2fd7986d8a0769bef55d8bd834c442204.jpg" width="281" height="500">
```

---
## \#27 Posted by: JdogAwesome Posted at: 2017-11-26T13:13:33.764Z Reads: 100

```
Yeah that should work, seems a bit low of a current draw only 20ma so it's not going to blow alot of air, but it will work as long as it's 12V and your bucking it down.

EDIT: Just saw it's 5V so yeah you could connect it to the 5V on the VESC because of how low current draw is.
```

---
## \#28 Posted by: GhettoFab.rictation Posted at: 2017-11-27T04:03:54.219Z Reads: 88

```
Awesome thank you! I tested it out and after a minute they fire up! I'm going to add my heat sinks on both sides then add fans on both sides then shrink wrap it! Going to seal onewhere( motor wires ) then have both sides cut out to where the air flow sucks in through fans and out the battery lead side!
```

---

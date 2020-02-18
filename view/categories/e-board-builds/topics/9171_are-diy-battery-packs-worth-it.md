# Are DIY battery packs worth it?

### Replies: 12 Views: 3426

## \#1 Posted by: cryzies Posted at: 2016-09-07T22:41:37.690Z Reads: 356

```
Weight: 225 lbs

Parts planned so far:

Motor: Turnigy SK3 6374-192kv
ESC: VESC 4.12

Looking to do a DIY battery pack, but I'm not sure if it's worth it. Looking into A123 26650's which satisfy the 80amp burst draw of the motor. Looking to do a 12s back so with 3.3 nominal voltage per cell I'd get a total of around 40volts. Should I be trying to reach the maximum voltage of the motor? How would my expected range be with a 12s pack of A123 26650s.

Battery data sheet: http://www.a123systems.com/Collateral/Documents/English-US/A123%20Systems%20ANR26650%20Data%20Sheet.pdf
```

---
## \#2 Posted by: cryzies Posted at: 2016-09-07T22:43:14.663Z Reads: 345

```
Any comments on my motor and esc choice will be greatly appreciated as well
```

---
## \#3 Posted by: Namasaki Posted at: 2016-09-07T22:53:53.767Z Reads: 337

```
That motor is a bit much for the Vesc at 12s. 
You should do 10s with 192kv
Or 12s with 170kv
For long term dependability. 
A123 is a good option. 
A 10s2p pack should give you around 10 mile range and enough current capability to avoid excessive voltage sag. 
Or get a lower KV motor and build a 12s2p.
Oh, and definitely go with Vesc. They perform like a dream!
```

---
## \#4 Posted by: cryzies Posted at: 2016-09-07T22:58:49.184Z Reads: 316

```
Hey Namasaki! Big fan haha been following some of your builds, I too live in SD and wish to cruise around PB/Mission Bay

Thanks for the advice, 10s2p would make a huge dent in my bank, if I'm not mistaken, the more cells/volts the more instantaneous power correct? So how would a 6s2p or even 8s2p do to my build, the should just be lower voltage but same range correct? Just lower torque and top speed?
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-09-07T23:25:08.099Z Reads: 285

```
If you do go to a 6s the best would be a 6s4p ....6s2p would just cause some major voltage sag towards the end of your short ride
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-07T23:32:31.832Z Reads: 274

```
That motor is actually fine for the VESC since he'll be using lifepo4 cells that run lower voltage. 12s lifepo's are about the equivalent of 10s liion.
```

---
## \#7 Posted by: Titoxd10001 Posted at: 2016-09-07T23:39:06.784Z Reads: 267

```
The voltage seems fine but the range will be bad for the price. Look at boosted some people only get 4-6miles with the 12s1p. 12s2p should be around 10-12miles. If you go  10s4p with 18650 cells you would get more range with similar price. If range isn't much of an issue a123 cells are probably safer
```

---
## \#8 Posted by: treenutter Posted at: 2016-09-07T23:44:15.027Z Reads: 272

```
[quote="cryzies, post:4, topic:9171"]
So how would a 6s2p or even 8s2p do to my build
[/quote]


@cryzies you'd notice more heat and have a higher potential for overheating. 

[quote="cryzies, post:4, topic:9171"]
just be lower voltage but same range correct?
[/quote]

Correct that voltage would be lower. Range would not be the same, you get more range with as you increase cells in serial, but the impact isn't as dramatic as increasing the cells in parallel.

[quote="cryzies, post:4, topic:9171"]
Just lower torque and top speed?
[/quote]

Correct; the most significant impact being reduced torque. You'd have to push to get started with 6S unless you have a really high reduction ratio (4:1 might get you there, but then you're using pneumatic wheels)

I think that for your weight 10S or 12S is the common recommendation. You can save money by reducing the cells in parallel at the expense of range.[quote="cryzies, post:2, topic:9171"]
comments on my motor and esc choice will be greatly appreciated as well
[/quote]

I use VESC 4.12 from Ollinboard with an SK3 6364 and I'm very happy with it! 

http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6364-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292 

@cryzies check out the math that @chaka offers to help determine the right motor kv with VESC. Many folks on the forum are using this advice to select motors with VESC.

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#9 Posted by: cryzies Posted at: 2016-09-07T23:51:40.082Z Reads: 226

```
Thanks for all the help! If I go with A123 26650s, would I need a BMS? How would I go about charging a 10s or 12s pack? Once I can increase my budget, how difficult would it be to make another 10s/12s pack and wire it in parallel. Is as simple as wiring it up?
```

---
## \#10 Posted by: treenutter Posted at: 2016-09-08T00:01:29.122Z Reads: 229

```
[quote="cryzies, post:9, topic:9171"]
If I go with A123 26650s, would I need a BMS?
[/quote]

@cryzies there is debate about this; but I think the general thinking is that you should have a BMS unless you are able to carefully monitor your cells my measuring them at strategic intervals. If you want easy plug-n-play charging (and I think this is the benefit of building a pack like this) you want a BMS.

[quote="cryzies, post:9, topic:9171"]
Once I can increase my budget, how difficult would it be to make another 10s/12s pack and wire it in parallel. Is as simple as wiring it up?
[/quote]

If you wanted to increase your range you would have to dismantle the pack and rebuild it, but it is better to avoid this. You want all the cells in the pack to age together so they remain easily balanced.

To build a pack, you have to solder or spot-weld the cells together with nickel stripping, or copper wire. It would be better to wait and save up enough funds to build the pack you want.

Here's a basic shopping list for a li-ion based pack.
http://www.electric-skateboard.builders/t/18650-10s3p-battery-for-the-village-build/2087
```

---
## \#11 Posted by: sl33py Posted at: 2016-09-08T00:16:24.546Z Reads: 197

```
[quote="cryzies, post:9, topic:9171"]
If I go with A123 26650s, would I need a BMS? How would I go about charging a 10s or 12s pack?
[/quote]


BMS is nice, but option B would be to remove and charge as two 5s or 6s packs w/ a regular charger.  Easy peasy breezy.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-09-08T01:04:09.316Z Reads: 183

```
8s2p will give you more speed, torque and range over a 6s2p
You live in San Diego, that's cool. 
I live in Lakeside but I like to skate all over. Except mission bay park. The sidewalk cracks are ridiculous. 
Constantly chunk chunk chunk. 
The mission beach boardwalk is fun and fairly smooth. A lot of the streets in PB have been repaved so there really smooth. I surf at Tourmaline a lot. 
I've also done the silver strand bike way. 
We'll have to meet up for a cruise. 
So if your wanting to build a battery, I can help. 
I have a spot welder and extra nickel strips
```

---

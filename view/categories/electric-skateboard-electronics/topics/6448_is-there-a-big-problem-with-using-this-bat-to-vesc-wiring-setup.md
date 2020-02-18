# Is there a big problem with using this (Bat to VESC) wiring setup?

### Replies: 11 Views: 1323

## \#1 Posted by: paul775 Posted at: 2016-07-21T21:50:44.882Z Reads: 122

```
<img src="/uploads/db1493/original/2X/d/dd4fbbb73c9bb2e4245c6bf9f83971656ef0b014.jpg" width="590" height="220">

From what I gathered is that I will not have:

* a Power Switch
* no Anti-Spark Protection
* and I might have some heat issues since the XT’s are rated to higher temps than these 5.5mm.

I will use Voltage Buzzers to keep track of the voltage.
Besides that, what do you think of this straightforward series setup?
```

---
## \#2 Posted by: zk8_builder Posted at: 2016-07-21T21:52:17.548Z Reads: 116

```
Seems correct except I would make or get a anti spark
```

---
## \#3 Posted by: paul775 Posted at: 2016-07-21T22:02:44.432Z Reads: 114

```
Okay I will look for some adapters since I really don't want to solder XT-60 connectors to batteries. Seems like a whole different game compared to soldering on PCBs.
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-21T22:03:35.845Z Reads: 108

```
I soldered an XT-60 to my 6s battery with minimal experience and it works fine. I don't think it's that hard :)
```

---
## \#5 Posted by: paul775 Posted at: 2016-07-21T22:06:34.501Z Reads: 99

```
Not hard just worried about blowing up the battery haha
```

---
## \#6 Posted by: Karmannghiagirl Posted at: 2016-07-21T22:07:40.107Z Reads: 95

```
trust me, unless you are a complete idiot, you'll be fine.

If you really dont want to change the battery conenctors, put an xt90s on the vesc connection.
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-21T22:24:40.089Z Reads: 89

```
I think you'll be fine! Most important rules are,

1. Don't snip both wires in 1 go. Snip 1 at a time so you don't short it with your scissors/wire cutters

2. Electrical tape the bare lead on the wire you're not working on to avoid a short.

3. Insulate a soldered lead as soon as your done to avoid a short while working on the next one.
```

---
## \#8 Posted by: paul775 Posted at: 2016-07-21T23:41:23.537Z Reads: 80

```
I am going to skip on changing the batteries but I will change the VESC connectors.

Was figuring it out and thought I post my soon-to-be adapter setup.
VESC > [XT-90S Female](https://www.amazon.com/XT90-S-Female-Connector-Battery-Charge/dp/B00RVM8U5W/ref=sr_1_5?ie=UTF8&qid=1469140936&sr=8-5&keywords=xt90s) > [XT-90 Male to XT-60 Female](http://www.hobbyking.com/hobbyking/store/__62937__XT90_male_to_XT60_female_2pcs_bag.html) > [XT-60 Male to 5.5mm](http://www.3drcparts.com/direct-connect-male-xt60-to-female-5-5mm-lipo-battery-adapter/) > Batteries

Thanks for confirming my current setup will work though!
```

---
## \#9 Posted by: paul1 Posted at: 2016-07-22T15:12:31.360Z Reads: 68

```
Hi, can you explain why its important to have an anti spark thing?
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-22T15:48:47.720Z Reads: 63

```
Sparks cause carbon build up which affects the quality of your connection. Anti spark does exactly as it says and prevents sparks when connecting your circuit.
```

---
## \#11 Posted by: paul775 Posted at: 2016-07-23T05:59:05.759Z Reads: 42

```
Found another adapter! [Jeti AFC Anti-Spark Connectors 5.5mm (150A)](http://www.espritmodel.com/jeti-afc-anti-spark-connectors-5-5mm-150a.aspx)
Would just need to replace one connector from the VESC and done!
```

---

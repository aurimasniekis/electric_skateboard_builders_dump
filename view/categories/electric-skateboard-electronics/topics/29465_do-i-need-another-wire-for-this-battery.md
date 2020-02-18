# Do I need another wire for this battery

### Replies: 8 Views: 656

## \#1 Posted by: Tycho Posted at: 2017-08-02T18:09:28.907Z Reads: 97

```
I going to run a 245kv motor with two of these.

https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html
<img src="/uploads/db1493/original/3X/d/0/d0a2b00408d9d5648e9bd1b6ac97fb498e9e2847.jpg" width="565" height="414">


Is it possible to have them in series?
Is it possible to charge them at the same time. 

The videos I see on youtube does it with an ekstra wire, do I need that?


thank you for the help
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-02T18:12:19.870Z Reads: 87

```
You need a 2 x 3s to 6s balance lead adaptor and a 4mm bullet connection series adaptor.
```

---
## \#3 Posted by: jammin Posted at: 2017-08-02T18:54:02.103Z Reads: 69

```
Regarding your questions, yes and yes. Wire them up in series (plenty of youtube videos / forum posts about it) and you can charge and discharge in series with something like the iMax b6.

The extra wire you're talking about (I'm assuming) is the balance lead, you'll need that whenever you charge your batteries.

Edit: on second thought, you might want to consider choosing batteries with a higher discharge rating ( 'C' rating). What's the setup you're using / planning to use with these lipos?
```

---
## \#4 Posted by: Tycho Posted at: 2017-08-03T09:16:12.575Z Reads: 48

```
[quote="darkkevind, post:2, topic:29465"]
6s balance lead adaptor
[/quote]

Like this? 
https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html

and this?

https://hobbyking.com/en_us/xt60-to-3-x-3-5mm-bullet-multistar-esc-power-breakout-cable.html
```

---
## \#5 Posted by: Tycho Posted at: 2017-08-03T09:50:52.490Z Reads: 38

```
Hi Jammin,
thank you for response.


Desired top speed 
12-18 mp/h (20-30 km/h)
The range should be 9-15 km (6-10 miles)

A light board and great acceleration would be great.
As the range goes I think a batterie with a low range would be fine, (low mAh). Then in the future I could get the same batterie pack so I could change it on the go.

(It is going to be a light city esk8 that i can easely stop and start with in intersections without having to give it a push)
That is why in taking the 245kv
190kv needs a lot a batterie weight
270kv dont have that great acceleration

I have a 15T 36T gear solution with a 83mm wheel
It should be going with a 245kv motor

I've been looking at some batteries with a higher 5800mAh but that is the only thing I need to get higher.
I'm not going faster than 15-24 km in the city, (had a speedometer on my phone while biking in the city)
30 km is when I realy give it all I got :-) 

I've been looking at these two 
https://hobbyking.com/en_us/zippy-flightmax-5800mah-3s1p-30c.html
two of them in series so it became a (5800mAh 6s1p 30c)


Here is some calculations with 5000mAh

<img src="/uploads/db1493/original/3X/3/b/3b76f1967fb0fd27db22f53b16fa39842b0ec8ee.png" width="690" height="335">
```

---
## \#6 Posted by: Tycho Posted at: 2017-08-03T09:58:10.318Z Reads: 31

```
is it so much saying a effeciency on 90% ?
```

---
## \#7 Posted by: darkkevind Posted at: 2017-08-03T12:15:57.731Z Reads: 29

```
The XT60 connector is wrong but the balance adapter is correct.

The batteries have female connectors, you need a lead with male connectors...
Plus, that's a parallel connector not series.
```

---
## \#8 Posted by: jammin Posted at: 2017-08-03T16:19:55.968Z Reads: 22

```
90% is a little optimistic, but it's more dependent on the roads in my experience. Your series cable is wrong (you have a parallel cable); assuming you don't want to solder:
https://hobbyking.com/en_us/hxt-4mm-to-xt-60-battery-adapter-2pcs-bag.html
https://hobbyking.com/en_us/xt60-harness-for-2-packs-in-series-1pc.html

Your battery has 4mm bullets, not 3.5. Depending on your ESC you might need an adapter for that as well. Don't forget an anti-spark switch / power button!
```

---

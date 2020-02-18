# Question about building a modular battery

### Replies: 6 Views: 328

## \#1 Posted by: ssdorsey Posted at: 2018-09-09T01:59:34.025Z Reads: 97

```
I wanted a build an esk8 with a modular battery system but I'm still a little unsure about whether or not it would work. The basic concept is that sometimes I want to have a 10s2p battery and sometimes I want to add in another 10s2p pack for a total of 10s4p. Is it possible to have a BMS tucked in with the rest of my electronics but wired in a way where only half the ports are being used sometimes? Or would I have to use a BMS for each of the packs?

Any recommendations for a reliable BMS that might accommodate this setup?

Sorry for the noob questions
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-09-09T02:06:24.146Z Reads: 95

```
These things are amazing

https://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847/601
```

---
## \#3 Posted by: Andy87 Posted at: 2018-09-09T05:13:09.759Z Reads: 82

```
For lipos there are parallel charging ports.
You could create something like this.
The big problem, the batteries need to be close the same voltage as possible if you start charging them.
In general that’s your problem. You shouldn’t connect two packs with different voltage as they will drain differently and could potentially discharge under the min cell voltage.
If you need a second pack just because of range than just create a plug and play version so that you can swap out one pack of empty and plug in a new fully charged just by connecting the main plus and minus and the balance leads.
```

---
## \#4 Posted by: ssdorsey Posted at: 2018-09-09T21:38:30.080Z Reads: 50

```
Cool that makes sense. Thanks
```

---
## \#5 Posted by: detroitwheelin Posted at: 2018-09-09T23:25:15.239Z Reads: 39

```
http://www.ebikes.ca/product-info/ligo-batteries.html

What we need is an open source BMS to build modular batteries like Grin Technologies LIGO packs
```

---
## \#6 Posted by: ssdorsey Posted at: 2018-09-10T01:23:57.814Z Reads: 29

```
Yes, this is exactly what I'm looking for. I'm going to poke around and see what I can do.
```

---

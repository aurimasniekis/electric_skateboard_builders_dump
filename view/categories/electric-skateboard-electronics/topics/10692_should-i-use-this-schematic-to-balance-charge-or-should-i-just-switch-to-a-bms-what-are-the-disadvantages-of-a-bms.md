# Should i use this schematic to balance charge or should i just switch to a BMS? what are the disadvantages of a BMS?

### Replies: 5 Views: 1450

## \#1 Posted by: itsmikeholland Posted at: 2016-10-05T19:39:00.574Z Reads: 378

```
Hi guys, Im having difficulty deciding between a permanent charging solution for my board. I like that the Turnigy Accucell gives me active cell readings while its charging, but id also like to be able to just walk away and balance charge my 12s setup. With the scheme, id just have to rotate the knob when my charger is finished charging a battery. Is it still safe to just rely on a 12s BMS to balance charge my setup? Im very new to electronics and would appreciate any input!

Thanks guys

 <img src="/uploads/db1493/original/3X/7/f/7f1db1a05053a0150f94cd6eeed0e507dd34eaf9.png" width="690" height="388">
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-05T19:44:46.281Z Reads: 360

```
I have a BMS (not a very good one to be honest) so I monitored my cells a lot towards the beginning, but now I just plug it in and let it do it's thing. I think the BMS choice often turns into more of a space (mounting on the board) and money issue than a functionality one. From what I've seen, even half-way decent BMS's will balance charge without issue. Where it starts to get more expensive is a BMS with a higher discharge rate. I decided to use my BMS just for charging and letting the VESC manage the discharging (ie, I just bypass my BMS for discharge)
```

---
## \#3 Posted by: chazeldine Posted at: 2016-10-27T20:49:23.279Z Reads: 301

```
Can you elaborate on which BMS you use? 

I am hoping to run x2 3S 5200 Mah lipos with a turnigy SK3 motor rated at 90 Amps peak.

Most of the BMS i have seen top out at about 60 Amps. 

How would you wire it to bypass discharge limits?

Thanks for the answers to my newbie questions.
```

---
## \#4 Posted by: mmaner Posted at: 2016-10-27T23:51:55.451Z Reads: 279

```
Here ya go...
<img src="/uploads/db1493/original/3X/e/c/ec0fe412b3e04e1d38dddac0ea8ee17f05b60fbf.jpg" width="670" height="500">

I've ordered a BMS to attempt a Zippy + BMS battery pack.  As soon as I get all the components I'll upload the diagram and pics.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-10-28T01:36:38.681Z Reads: 265

```
I have a very cheap BMS that I got from china on ebay [here](http://r.ebay.com/RLXDz6). I think it tops at 15A discharge, but I don't use it for managing my discharge current so I didn't care.

To bypass the BMS just hook up your positive and negative wires going to your ESC straight to the battery instead of through the BMS (and my recommendation is through a switch or key as well))
```

---

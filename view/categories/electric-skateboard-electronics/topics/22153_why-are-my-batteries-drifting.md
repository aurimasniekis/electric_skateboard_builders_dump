# Why are my batteries drifting?

### Replies: 17 Views: 844

## \#1 Posted by: Norco Posted at: 2017-05-01T17:19:51.250Z Reads: 140

```
So I have 2x 5s4p packs that I connect in series for my build. I did it this way so I could balance charge with my hobby charger. Only problem is that this is happening...
[Uploading...]() 
 I've checked all of the joints and all looks good. Ideas? Solutions?
```

---
## \#2 Posted by: Print3r Posted at: 2017-05-01T17:33:00.359Z Reads: 135

```
[quote="Norco, post:1, topic:22153"]
Uploading...
[/quote]

The picture wasn't uploaded before this was posted I think!
```

---
## \#3 Posted by: Norco Posted at: 2017-05-01T17:38:47.870Z Reads: 128

```
Nightmare. It didn't save either. OK imagine a charger readout charging at 5s with the first 4 cells at 3.75 and the fifth cell flicking between 3.89 and 3.90

😕
```

---
## \#4 Posted by: jujet Posted at: 2017-05-01T17:46:10.299Z Reads: 122

```
Maybe it's time to get a BMS mate
```

---
## \#5 Posted by: Norco Posted at: 2017-05-01T17:55:10.182Z Reads: 119

```
I'm thinking it would be less hassle. Want to get this to work at least first. No reason why it shouldn't. What would bother me is that with a bms, this could be happening and you would never know.
```

---
## \#6 Posted by: Hummie Posted at: 2017-05-01T18:02:59.617Z Reads: 116

```
<img src="/uploads/db1493/original/3X/f/7/f7683e98e7d20d3a8c658d3e08d822fc4eaeb010.png" width="333" height="500"><img src="/uploads/db1493/original/3X/b/7/b70a0230be4d60734b0446cab889e2bb48a37834.jpeg" width="500" height="500"><img src="/uploads/db1493/original/3X/2/1/21a35cdb3bb0a871380d3d248aaa202c6e229f04.jpeg" width="375" height="500">zhave you charged further?  I'll have drifting but when I charge, and the cells get up around 4 volts, everything comes back together again.  I'll have a much greater spread when discharged than fully charged.  
get one of those discharge balancers for like 10 bucks and solve it
```

---
## \#7 Posted by: Norco Posted at: 2017-05-01T18:04:38.191Z Reads: 102

```
I'm thinking this. Have link to a tested one/which do you use? Still charging so will see.
```

---
## \#8 Posted by: Hummie Posted at: 2017-05-01T18:07:26.851Z Reads: 107

```
just posted pics one post back.

this is a typical charge method for rc planes and a lot of diy ebikes.  the bms isnt necessary.  just make sure when you charge you are there and set the bulk charger to the correct voltage and I highly, highly recommend wiring in a watt meter onto the charger so you know whats going on and what the bulk charger is set to.  it's only adjustability is a tiny screw to change the output max voltage.  when it hits that it shuts off.
ive had three of these things and this new one is...new and I cant vouch for it yet but I can say the last one they sent me, when it snapped doing way more wattage than it was supposed to, they sent me this higher 500 watt one for free.  thats pretty cool and was about a 1/3 the price of the meanwell I had a while back.   actually I think so far its been better than the meanwell as the meanwell you had to keep stepping up the voltage if the pack was totally depleted otherwise it would go into a super slow charge mode.  a safety feature..maybe I'd want but so far no snap.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-02T05:08:41.806Z Reads: 77

```
[quote="Norco, post:3, topic:22153, full:true"]
Nightmare. It didn't save either. OK imagine a charger readout charging at 5s with the first 4 cells at 3.75 and the fifth cell flicking between 3.89 and 3.90
[/quote]

It has been my experience with my hobby charger that it is not uncommon for multiple cells to show varying voltages during the charge process. But as cells hit the full 4.2v, they stop and wait for the other lower cells to catch up.
If your cells are going way out of balance during discharge, It's most likely due to  internal resistance varying from cell to cell.
Unless you special order matched cells, they could vary a lot.
```

---
## \#10 Posted by: saul Posted at: 2017-05-02T05:52:17.779Z Reads: 68

```
thats weird that it goes higher than the others, i've had some cell checkers give bad readings on 1 of the pins.

but as long as the cells aren't dropping low while **discharging** I don't  think its much of a problem. 
most likely that group of cells just had a lower internal resistance so it takes in power a bit faster.
```

---
## \#11 Posted by: Norco Posted at: 2017-05-02T06:40:49.038Z Reads: 55

```
All cells ordered on one batch from nkon. Hobby charger stops charging Liion at 4.1 and once the first cell got to 4.1 it was taking forever to bring the others close (hours). Charged both batteries and went for a quick run. Cells where closer after discharge! I'm going to cycle a few times and see what happens.
```

---
## \#12 Posted by: Okami Posted at: 2017-05-02T11:18:41.541Z Reads: 49

```
I cant see your first.post picture anymore but sometimws if there is bad balance port.connection (or.it is.maybe corroded) the voltages might.be way off..

I have had this happen 2 times. Once when the extender balance cable broke I even got 9v for one cell group, zero.for.another and the rest.were also.very messed.up.showing.4.5v or.something

I would just.move the.cable around while it.is.connected.to.see.if.voltages change.
```

---
## \#13 Posted by: Norco Posted at: 2017-05-02T11:21:15.163Z Reads: 47

```
As part of my fault finding I have also soldered a new 5s balance plug - hopefully this will be solid now.
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2017-05-02T11:26:58.095Z Reads: 48

```
My battery pack has one series cell that discharges further than the other ones and at the end of a run I took a picture of the pack with my IR camera and it clearly shows the "bad" series cell being hotter then the other cells, indicating higher internal resistance. I do believe it has gotten damaged when I had before charged the pack without balancing (mistake). Now I always balance charge.

<img src="/uploads/db1493/original/3X/f/d/fd3787404bbc637e348d9e25b0ebe90f1f0e8bcb.png" width="281" height="500">
```

---
## \#15 Posted by: Namasaki Posted at: 2017-05-02T12:27:00.745Z Reads: 41

```
[quote="Norco, post:11, topic:22153"]
All cells ordered on one batch from nkon.
[/quote]
This doesn't guarantee there matched.
```

---
## \#16 Posted by: Norco Posted at: 2017-05-02T15:00:40.293Z Reads: 34

```
Fair point. They all arrived roughly the same voltage before and after making the pack up. Not the full picture I know but worth saying they should be quality.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-05-02T18:15:13.136Z Reads: 27

```
Having the same voltage means they're balanced. 
Having the same internal resistance means they are matched. 
You probably won't get matched cells unless you request it and then you have to find a supplier that will match them.  $$$$
```

---

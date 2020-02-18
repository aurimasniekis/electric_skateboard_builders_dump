# Setup, can it be done?

### Replies: 6 Views: 414

## \#1 Posted by: hunter Posted at: 2017-09-07T20:11:24.084Z Reads: 108

```
Heya guys/girls..

Been running my (prototype) for 6 months runs ok but dosent look good =)
Also I am working on the setup, I made this beautiful drawing. Just want to know if this setup can be done??
<img src="/uploads/db1493/original/3X/e/4/e4457e6721878b9e64875cc95b096a580adecb23.JPG" width="375" height="500">

Wandering if it is possible to charge while it connectet to the Vesc?
```

---
## \#2 Posted by: sl33py Posted at: 2017-09-07T20:20:11.039Z Reads: 93

```
You need to disconnect the batteries in series before charging.  If you plug it in like this it will let the magic smoke out!  You are still in series and will short.

Disconnect series, and charge two 5s batteries.  OR get a 10s charger and charge at 10s voltage w/ split balance leads.  ( I have the http://www.hobbypartz.com/75p-1220-charger.html - which does this).  It's meh.  No real advanced settings like on iCharger (miss the IR measurement in particular).  But does work for this.
```

---
## \#3 Posted by: hunter Posted at: 2017-09-08T15:23:44.386Z Reads: 44

```
So maybe the Best will be to buy a Bms and a Ebike charger for 10s?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-09-08T15:48:39.765Z Reads: 37

```
Actually it is possible to do as you have illustrated because you are in effect isolating each battery with charge leads. 
I have done this with my 5 x 2s in series 10s setup and it worked just fine. 
Just use a hobby balance charger and charge each pack separately. DO NOT charge both packs together in parallel
```

---
## \#5 Posted by: hunter Posted at: 2017-09-08T17:07:39.018Z Reads: 21

```
Ok, its because i have the 6s charger, so my plan is too charge them 1 by 1. I am also doing it now but is not pretty, as I want it in a closed container.<img src="/uploads/db1493/original/3X/3/1/31a5721cd23aed332bff360946361c7705f6c827.JPG" width="375" height="500">
```

---
## \#6 Posted by: Namasaki Posted at: 2017-09-08T17:12:37.543Z Reads: 20

```
Just charge them one at a time wired as illustrated and you will be isolating the pack your charging without disconnecting the series connections.
```

---

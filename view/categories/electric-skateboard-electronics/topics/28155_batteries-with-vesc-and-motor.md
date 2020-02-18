# Batteries with vesc and motor

### Replies: 8 Views: 653

## \#1 Posted by: dg798 Posted at: 2017-07-20T22:41:18.733Z Reads: 62

```
i have this vesc diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/ and this motor diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/.
would this battery work https://hobbyking.com/en_us/turnigy-5000mah-6s-40c-lipo-pack.html.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-20T22:47:23.755Z Reads: 58

```
This can work 6S is pretty low though and this is a bulky battery configuration to strap to the bottom of the board, check the dimensions on it.  I use 2 5S 5Ah batteries like this in series to make a 10S 5Ah total battery but they are pretty brick like so your enclosure will be bulky, you might want to go with a few smaller ones instead (say 2 3S batteries in series or something) or look for ones with flatter configuration.
```

---
## \#3 Posted by: dg798 Posted at: 2017-07-20T22:50:43.780Z Reads: 55

```
how about this one https://hobbyking.com/en_us/turnigy-4000mah-5s-30c-lipo-pack-xt-60.html
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-20T23:07:02.948Z Reads: 48

```
Yeah that's almost the same one I have I went with the 5Ah ones I get about 12 miles on a good day on mostly flat ground with 5Ah 10S configuration so just up to you in terms of the Ah if you want more/less range/weight/bulk.  Just saying good to  keep in mind you're going to wrap some enclosure around the batteries to keep them from getting damaged so need to take the height of them in the way you'll put them on the board and add a few cm for mounting parts and the enclosure thickness itself around the batteries.
```

---
## \#5 Posted by: dg798 Posted at: 2017-07-20T23:20:30.539Z Reads: 40

```
i was thinking of using 4 of these https://hobbyking.com/en_us/turnigy-bolt-v2-lihv-500mah-3s-65c.html in series. do you think that would fit
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-20T23:39:25.127Z Reads: 35

```
Those are super tiny think you sent the wrong link or searched for the wrong thing there though.  First ones were 4Ah or 5Ah last one is .5Ah so it's 1/10 the capacity of the other ones basically.  Think the math is basically 10Wh = 1 km (.6 miles) in ideal conditions (to compute the Watt hours Wh just do the Ah times the voltage, 1Ah = 1000mAh).  My board at 5Ah 10S (3.7V nominal voltage) is basically 5*10*3.7 = 185Wh which means I should get 18.5 km or 11.1 miles, I actually get a little more than that but I'm also a light dude and mostly riding on flat and always do a little kick start so I actually get a little over 12 miles on a good day.

---

Also wiring the batteries in series you add their voltage V (capacity Ah stays the same) wiring the in parallel you add the Ah (capacity but the voltage stays the same)
```

---
## \#7 Posted by: dg798 Posted at: 2017-07-20T23:42:29.960Z Reads: 32

```
i want 2 6s batteries. can you reccomend thinner ones fornot 0ver 60 bucks per
```

---
## \#8 Posted by: wafflejock Posted at: 2017-07-20T23:51:21.904Z Reads: 31

```
Maybe these:

https://hobbyking.com/en_us/zippy-compact-5000mah-3s-40c-lipo-pack.html

You'd need to get 4 and wire them in series to get your 12S if that's what you're going for but they should be pretty compact and will get you up to 5Ah and have the 40C rating so shouldn't get too much voltage sag.

Can see some other competition in the filter here too:

https://hobbyking.com/en_us/lipo.html?config=53&capacity=4000-10000&discharge=40-110&

I filtered to just 3S batteries but can include or just search 6S ones there as well but probably want somewhere around 5Ah total I'd think.
```

---

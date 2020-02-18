# Motor Controllers

### Replies: 8 Views: 557

## \#1 Posted by: FMS Posted at: 2017-07-01T17:48:50.094Z Reads: 98

```
Why is everyone using motor controllers that are rated for 100A or more? I was going to use some that were rated for 60A but was wondering why everyone was using such high amperage ESCs
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-01T17:49:33.737Z Reads: 98

```
Better to have more head room
```

---
## \#3 Posted by: NAF Posted at: 2017-07-01T17:52:14.843Z Reads: 98

```
..in a lot of cases the answer is: HUB MOTORS ...they do eat up lot's of amps.
```

---
## \#4 Posted by: Hummie Posted at: 2017-07-01T18:02:26.432Z Reads: 92

```
how do those hobby kind of escs with just an amp rating work as far as their limit?   I'd think they would be limiting the amps so regardless of what load you put the motor under it would at worst just be low power but I get the feeling with the need for headroom that that's not the case and a big load will blow it up.  But this "blow up" would still be simply too much heat like all the others and if you monitored and kept the heat below a certain unknown level you could get away with using a low amp esc.   No?
```

---
## \#6 Posted by: NAF Posted at: 2017-07-01T18:29:17.792Z Reads: 73

```
There are not many options: you have old JACOB hubs modified by Ralphy, you have upcoming Carvon V3, and you have upcoming @Hummie hubs. All the rest like Maytech hubs and many others seem to be lacking..
```

---
## \#8 Posted by: Smorto Posted at: 2017-07-01T19:02:59.734Z Reads: 62

```
I am wondering this as well since it is recommended to get a 120A or 150A ESC when using hobby ESCs, but the vesc can only handle about 45A continuous right?
```

---
## \#9 Posted by: Hummie Posted at: 2017-07-01T19:16:25.248Z Reads: 60

```
Whatever you could get the continuous power of the VEC to with heat sinks or whatever its got that temp shut down safety vs hobby stuff I bet there's no heat sensor an safety shutdown. It's been said there's "spikes" created when using an esc as we use them on a board.  I don't remember if it's the current or a voltage spike and a voltage spike being a killer makes more sense to me otherwise it'd just be more heat that maybe could be controlled.   I'm waiting for someone to tell why a 6s 50amp hobby king esc would die and if it'd still be workable by watching the temp or heat sinking it really well.  
I have my vescs programmed to pull about 50 amps max from the battery and especially on 12s it's pretty damn powerful.
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-01T19:30:30.489Z Reads: 57

```
VESC is rated for 50A continuous 240A peak, the MOSFETs it depends on to deliver the power are limited to 240A

https://www.infineon.com/dgdl/irfs7530-7ppbf.pdf?fileId=5546d462533600a40153563a9d1e21d8

I used a 120A 6S ESC for a bit while I was waiting on a back-ordered VESC and it ran pretty well given the 6S but had active cooling on it and couldn't deal with higher voltage.  I swapped it out for the VESC since I did want more voltage than that and didn't like that I had to buy other proprietary hardware to configure the car ESCs (also just knew you have more control with software configuration the VESC gives).
```

---

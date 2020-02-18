# DRV8302 errors all bad?

### Replies: 7 Views: 829

## \#1 Posted by: Goombaacez84 Posted at: 2016-10-09T20:53:15.170Z Reads: 92

```
Hey all,

So I just had to give FOC a try. I uploaded a fresh firmware (2.18) and immediately switched to FOC and wrote the configuration. I followed Benjamin's FOC tutorial he has on YouTube and everything configured and detected okay. Got my nunchuck all setup and went out for a ride.

The board feels amazing and is a different sensation than BLDC mode. I rode the board home and immediately plugged it in to see if I had tripped any faults - DRV 8302s errors of course. Should I be concerned? My VESC still functions perfectly and nothing spectacularly wrong happened on the road while riding except for having to reconnect my Kama a couple times. Should I be concerned?

My setup is:

* Ollin 4.12 VESC w/ 2.18 firmware
* 12s MEB stealth battery
* 190kv 6374 r-spec motor

Edit: I should also mention that I can't see anything visibly wrong with the DRV chip... looks in tact to me.
```

---
## \#2 Posted by: laurnts Posted at: 2016-10-09T21:09:39.049Z Reads: 89

```
If your board ride okay, it should be fine. It could be that the connections of your VESC with the computer are not correctly installed. Otherwise feel free to post photo of the VESC as well as the PC and the way you connect the VESC to the PC. It would gave us better perspective in investigating your issue.
```

---
## \#3 Posted by: caustin Posted at: 2016-10-09T21:11:40.266Z Reads: 86

```
Can you post screenshots of your settings?
```

---
## \#4 Posted by: Goombaacez84 Posted at: 2016-10-09T21:29:59.608Z Reads: 78

```
Here's how it's physically connected, nothing out of the ordinary aside from a long USB cable:

<img src="/uploads/db1493/original/3X/b/1/b1fe8b95a2086afba8f258c08c494b859d44f0ea.jpg" width="375" height="500">

Here are the settings pages... I think I got everything necessary, but let me know if I missed one:

<img src="/uploads/db1493/original/3X/b/e/beeacdae77cb87488cb47b34adf5bf108178af4d.png" width="690" height="362">

<img src="/uploads/db1493/original/3X/7/7/77c563032c1f92f42585fe23ebf5c5de7cb09624.png" width="690" height="363">

<img src="/uploads/db1493/original/3X/f/4/f4709fd48eba8c05ceb085891f0a48f669c4d62c.png" width="690" height="363">

<img src="/uploads/db1493/original/3X/b/a/badbb037d415e4e968eed688f36ea3f456af688b.png" width="690" height="163">

Edit: Setting screenshots should be accurate now :slight_smile:
```

---
## \#5 Posted by: chaka Posted at: 2016-10-09T21:57:55.751Z Reads: 75

```
You may have trouble if you try and go back to bldc mode.
```

---
## \#6 Posted by: Goombaacez84 Posted at: 2016-10-09T22:08:59.835Z Reads: 70

```
I just went for another ride down the street, changing the eRPM limit down to 60k just to be safe... I think it's done for. Didn't make it very far this time. Do you see anything wrong with those FOC settings @chaka?

I'll be PM'ing you here shortly about the DRV as well... :sweat:
```

---
## \#7 Posted by: chaka Posted at: 2016-10-10T00:29:50.922Z Reads: 64

```
Yeah it will need to be fixed, this is why I do not recommend using FOC mode it has fried a lot of hardware. Send it in and I will get it back in operation. ;)
```

---

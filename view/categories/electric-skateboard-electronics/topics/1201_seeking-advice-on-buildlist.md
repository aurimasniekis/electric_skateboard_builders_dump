# Seeking Advice on Buildlist

### Replies: 12 Views: 1691

## \#1 Posted by: gamma2 Posted at: 2016-02-02T05:21:51.485Z Reads: 62

```
Hi guys, this is my first post on the forum. I've been doing some research on building my own eboard and was wondering if I could have some input on [url=https://docs.google.com/spreadsheets/d/1fK_vySqIhCLB-rnoNRqwW6gdb5bHKuq_vVj7kkb3Uho/edit#gid=0]my build list[/url]. I have a lot of experience with quad and tricopter builds, so I'm pretty strong on the assembly side; I'm just not sure if I have the right parts chosen. Please give me any input you have. I made a notes column on the right with major questions I have; but feel free to tell me if theres a better part I should be looking at. I played varsity football all through HS so I'm a bigger dude (6'1", 260lbs), so should I be looking at a dual motor setup instead? My daily commute is mostly flat with only one small hill. I'm not trying to build some total speed demon. My main use will be commuting but it would be nice to hit 15 or 20 every once in a while.
I also currently have an [url=http://www.poolkingskateboards.com/images/alva_tri_logo.jpg]Alva Pig[/url]. Any thoughts on using this, a shorter board, versus something like my ThreeSix Downhill, stability, strength, powerwise, etc?


Thanks for the help guys!
```

---
## \#2 Posted by: laurnts Posted at: 2016-02-02T05:44:43.693Z Reads: 62

```
Try to get the 192kv motor as they have more torque on lower speed and I also recommend getting VESC from Enertionboards.com / Ollinboardcompany.com as they are currently one of the best ESC you could get with nice low speed startup. Most ESC out there are not build to pull 60kg weight ++ for long period, hence you might wanna get something more decent for it's purpose.

For the rest you could get opinion from other builders here :)
```

---
## \#3 Posted by: onloop Posted at: 2016-02-02T12:48:48.716Z Reads: 58

```
Everything looks good!... go the 15mm wide belts.

ill never use lipo on a board again personally but they are a good starting point.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-02-02T15:58:44.184Z Reads: 51

```
If your board has not enough power i would try to go 12s. That should fix the missing power.
```

---
## \#5 Posted by: gamma2 Posted at: 2016-02-02T18:15:11.881Z Reads: 47

```
What would u recommend in place of lipo onloop?
```

---
## \#6 Posted by: onloop Posted at: 2016-02-03T00:24:28.818Z Reads: 39

```
more and more people are building boards with 18650 li-ion type batteries & BMS built in to manage charging etc.

the SPACE CELL is the easiest way of making it happen. 

https://www.instagram.com/p/BADzJlggW-f/?taken-by=enertionboards
```

---
## \#7 Posted by: barajabali Posted at: 2016-02-03T01:16:17.441Z Reads: 38

```
Im cheap i use whatever i can get my hands on! If i have spare lipo cells, ill make a pack   
If i have spare 18650's ill make a pack.
```

---
## \#8 Posted by: gamma2 Posted at: 2016-02-03T02:02:18.910Z Reads: 38

```
How would the battery life and performance compare between running 2 6s 8Ah lipos in series vs in parallel? I'm hoping to get at least 5-10 miles a charge. Is that going to be realistic with my motor/VESC combo?
```

---
## \#9 Posted by: laurnts Posted at: 2016-02-03T02:19:03.502Z Reads: 39

```
Im running 6s 10Ah and I could get solid 20km, so it could be around 25km'ish depending on ground level and the way you ride.
```

---
## \#10 Posted by: gamma2 Posted at: 2016-02-03T04:59:34.247Z Reads: 34

```
So 12s 8Ah I can expect somewhere in that region? 15km maybe?
```

---
## \#11 Posted by: laurnts Posted at: 2016-02-03T06:53:15.859Z Reads: 31

```
Yes I really believe so. Just do kick push when starting and try to ride 80% of the throttle and you'll be fine.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-02-03T07:16:16.915Z Reads: 32

```
If you have a VESC and you have the choice of running your batteries in parallel @6S or in series @12S, in my opinion it makes most sense to run them in series @12S because the current draw will be lower and so will heat losses. More efficient. 12S will give you a high top speed but the VESC will allow you to cap this to any speed you wish.

The 192kV motor would be ideal for 12S.

There's a rule of thumb that says approx 1km range for every 10Wh, [I confirmed this on my single motor setup][1], and going through some readings on the forum I'd say it looks pretty accurate.

Series:  12S 8ah = 44.V x 8 = 355Wh.
Parallel: 6S 16Ah = 22.2V x 16 = 355Wh

You should get way more than 15km. Probably more like 30km.


  [1]: http://www.electric-skateboard.builders/t/loaded-dervish-dual-r-spec-6355-dual-vesc-nunchuck-paris-195-90mm-flywheels/524/61?u=trbt555
```

---

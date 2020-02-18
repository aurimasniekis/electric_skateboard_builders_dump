# Battery wiring idea.. is it possible?

### Replies: 37 Views: 2099

## \#1 Posted by: flywithgriff Posted at: 2017-03-13T23:48:07.373Z Reads: 177

```
I am currently running 2x3s 5,000mAh. I am happy with speed but want to extend range. Is there a way to wire my current 2x3s with an additional 2x3s for a total of 10,000mAh for longer range? If I am correct wouldnt this simply be a 6s 10,000mAh setup that can still be charged on a iMax B6AC? Would my VESC still handle this ok?
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-13T23:52:08.748Z Reads: 177

```
Yes there is. We call it parallel. Search for "zippy in parallel" or something similar. You'll just need a "Y" connector essentially.
```

---
## \#3 Posted by: IsTalo Posted at: 2017-03-13T23:52:34.214Z Reads: 174

```
I think It could, It won't modify the Erpm rate, but I don't know if the Imax can support 10A. Why don't you use they together and use separately?
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-03-13T23:55:18.180Z Reads: 173

```
My main goal is to be able to charge without opening the enclosure. I already have a 2x3s setup with a charging port but want to add an additional 2x3s setup for extended range. Because the imax will only charge at 5A it will just twice as long to charge correct?
```

---
## \#5 Posted by: rpn314 Posted at: 2017-03-13T23:56:42.627Z Reads: 152

```
[quote="flywithgriff, post:4, topic:19035"]
Because the imax will only charge at 5A it will just twice as long to charge correct?
[/quote]

Correct. You could also get a parallel charging board off of hobbyking or something.

Here's a good thread to read through.
http://www.electric-skateboard.builders/t/charging-4-3s-batteries-2-series-2-parallel/16129
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-03-13T23:59:16.925Z Reads: 121

```
@rpn314 thank you!
```

---
## \#7 Posted by: rpn314 Posted at: 2017-03-14T00:01:14.346Z Reads: 114

```
If you want a completely integrated solution, you could also add a BMS inside and then you'd just need a single laptop style charger. [quote="flywithgriff, post:6, topic:19035"]
thank you!
[/quote]

Happy to help!
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-03-14T00:18:09.117Z Reads: 104

```
Im not opposed to a BMS i just have absolutely no idea how they work or are installed. Any idea what the charge time with a BMS would be?
```

---
## \#9 Posted by: IsTalo Posted at: 2017-03-14T01:24:25.872Z Reads: 94

```
It depends, the bms simply balance your batteries and cut the voltage when nedded. It is faster because you can use a 5A ,or more,power brick to charge the batteries.

Also try to use reliable Bms because it is better, but if you don't want to spend a lot of money like me, buy one from ebay, bypass the wiring and use the Vesc to cutoff the battery and the power brick to don't overcharge
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-03-14T02:06:57.957Z Reads: 92

```
So basically I need to buy a BMS that supports my battery configuration and then pair a power brick with it that charges near the max amps my batteries can receive. Is this correct?
```

---
## \#11 Posted by: mmaner Posted at: 2017-03-14T02:09:46.676Z Reads: 85

```
You can  at 2a if you want, 5a is about the safe max.  I usually charge at 2a with a BMS and 5a with a balance charger.
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-03-14T02:19:45.128Z Reads: 81

```
Running a bms with 4x3s 5,000 mAh batteries, what kind of charge time will I be looking at?
```

---
## \#13 Posted by: mmaner Posted at: 2017-03-14T02:21:48.492Z Reads: 84

```
Hmmm, prolly 4 hours or so at 5a.  But it's hard to say.  Depends on how low you run the voltage, how out of balance the cells are, the quality of the batteries, etc.

If it were me, I'd make 2 15 pin charge ports, 1 for each series of batteries (each series being 6s) and charge them separately.
```

---
## \#14 Posted by: flywithgriff Posted at: 2017-03-14T02:27:48.456Z Reads: 86

```
My entire reason for considering BMS is for ease of charging. Do you mind if I PM you my current setup and what I want to achieve to get your opinions?
```

---
## \#15 Posted by: mmaner Posted at: 2017-03-14T02:56:02.347Z Reads: 85

```
Sure.  It's just cheaper to use a 5s charger on each pack, if you already have the charger, the buying a BMS. If you are set on a BMS follow the @Namasaki rules of "Zen and the Art of BMS's" 😀 and get the BestTech HCX-D223V1.
```

---
## \#16 Posted by: flywithgriff Posted at: 2017-03-14T03:07:43.195Z Reads: 86

```
I currently have two 3s 5000mAh 30C packs wired together in series for one 6s pack. This setup is connected to an external mount charging port. I charge it with a IMAX B6AC. 

I want to add an additional 2x3s pack and wire it to the current setup for an overall 6s setup with more Amp hours but without losing the external charging port.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-03-14T03:48:48.250Z Reads: 82

```
Personally, I have never been a fan of charging lipos in parallel. Some people say it's ok other say it's not ok.
Since you where planning to buy additional batteries to up your range, I believe there is a much easier way.
Just replace your two 3s 5000 30c packs with two Zippy Flight Max 3s 8000 30c packs. This way you are increasing your range by 63% with a "bolt on" upgrade.  So if you where getting 6 miles with your current batteries, you should see close to 10 miles with the flight max. Also the fact that the flight max support higher amperage draw means less voltage sag which in turn means added range. The ZFM are also only 27mm thick so they are good for low profile installation.
You could recoup some of the cost by selling your used Lipos in the forum market or keep them for backup.
This way you can gain valuable miles using your existing setup and charger.
https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-03-14T03:52:55.742Z Reads: 74

```
Well damn, that's a pretty simple solution!! I believe I will buy the 8000's and then work on using the 5000's as a backup set.
```

---
## \#19 Posted by: Namasaki Posted at: 2017-03-14T03:56:15.839Z Reads: 68

```
Also, to answer your question about the Vesc handling the upgrade.
Since your not changing the voltage, the Vesc won't know the difference.
The Vesc doesn't care about battery capacity, only voltage.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-03-14T03:58:12.905Z Reads: 63

```
oh, one more thing, An important tip about Hobby King.
```

---
## \#21 Posted by: flywithgriff Posted at: 2017-03-14T03:58:33.666Z Reads: 64

```
Please share
```

---
## \#22 Posted by: Namasaki Posted at: 2017-03-14T03:59:36.172Z Reads: 60

```
create an account and log in then sit on the page with the item you want until they pop up a discount offer.
They always do, you just have to wait it out.
It may only be a few bucks but every bit helps
```

---
## \#23 Posted by: Namasaki Posted at: 2017-03-14T04:01:36.501Z Reads: 57

```
I was just there anonymously and as soon as I signed in the price dropped $2 per pack
```

---
## \#24 Posted by: flywithgriff Posted at: 2017-03-14T04:17:48.590Z Reads: 55

```
I read in their accounts tab that after your second order you receive discounted pricing but im currently waiting out an offer while sitting on the listing for the 3s 8000.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-03-14T04:21:22.917Z Reads: 50

```
Some times if takes a bit.
```

---
## \#26 Posted by: Namasaki Posted at: 2017-03-14T04:22:01.793Z Reads: 50

```
what price are you seeing?
```

---
## \#27 Posted by: flywithgriff Posted at: 2017-03-14T04:30:32.491Z Reads: 48

```
Im not getting a pop up and they are displaying for $45.46
```

---
## \#28 Posted by: Namasaki Posted at: 2017-03-14T04:31:27.355Z Reads: 51

```
its been a while since I bought there, they may not be doing that anymore
```

---
## \#29 Posted by: flywithgriff Posted at: 2017-03-14T04:32:39.651Z Reads: 51

```
I was able to get two batteries with 2-7 day FedEx shipping for $100.34.
```

---
## \#30 Posted by: Namasaki Posted at: 2017-03-14T04:36:24.561Z Reads: 53

```
Thats good, They are pretty quick at getting your order out as well.
Be sure to check the voltage of all cells before installing or charging them.
Just in case you get a bad pack. It happens some times.
When it does they are very good at making it right.
I got a couple bad packs once and they just had me email pics of the serial numbers and voltage meter reading and they shipped me out 2 new packs. They told me not to return the bad packs.
Normally, each cell will be at 3.6-3.8 v when shipped.
```

---
## \#31 Posted by: flywithgriff Posted at: 2017-03-14T04:38:00.600Z Reads: 49

```
I ordered the Turnigy 5000 packs I have now from them as well. Best I remember I received them in 4 days and im on the opposite coast from them. I need to read up on how to test the cells with a multi meter.
```

---
## \#32 Posted by: Namasaki Posted at: 2017-03-14T04:43:12.764Z Reads: 48

```
You can do it with a multimeter or one of these:
https://hobbyking.com/en_us/turnigy-cell-diagnostics-meter-2s-6s.html
```

---
## \#33 Posted by: Namasaki Posted at: 2017-03-14T04:57:42.564Z Reads: 47

```
With a multimeter, you just test at the balance leads. start with neg probe on the black wire and pos probe on the wire next to the black wire that's cell 1
then move both probes over one wire thats cell 2
then mover both probes over one wire thats cell 3
the black wire is the neg wire for cell 1
the pos wire of cell 1 is the neg wire for cell 2
the pos wire of cell 2 is the neg wire for cell 3
the red wire is the pos wire for cell 3
```

---
## \#34 Posted by: saul Posted at: 2017-03-14T05:47:40.337Z Reads: 44

```
yea I think they got ride of the pop up when they redid the site.
```

---
## \#35 Posted by: saul Posted at: 2017-03-14T05:49:38.354Z Reads: 46

```
what kind of performance are you getting with 6s? 
speed? range? hills?

i've used 12s and 8s. seems like 6s would be for mostly flat rides.?
```

---
## \#36 Posted by: flywithgriff Posted at: 2017-03-14T18:51:14.141Z Reads: 43

```
I'm in central Florida so any hills here are driveways. I just went for a range test while my car is getting an oil change. I didn't record the first 0.4 miles and I stopped riding when I felt the soft voltage shutdown from my VESC. The fastest I've hit so far in a smooth flat parking lot is 19.6 mph and I'm pretty sure that's about all it's got. These stats are on 83mm wheels and I am a good size guy at 240 lbs
```

---
## \#37 Posted by: flywithgriff Posted at: 2017-03-14T18:55:11.577Z Reads: 44

```
<img src="/uploads/db1493/original/3X/a/3/a3e2748883f26e9d88dda59dff28a2e3e11adc1a.PNG" width="281" height="499"><img src="/uploads/db1493/original/3X/4/4/44988c2963388a18ee64fdbefebfb0355253603e.PNG" width="281" height="499">
```

---

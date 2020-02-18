# Pairing two Chinese escs to one remote?

### Replies: 31 Views: 3676

## \#1 Posted by: Kooli Posted at: 2017-09-15T07:03:22.213Z Reads: 265

```
So I have a meepo and I've been trying to modify it to make a 4x4. I received all my components today and I gave it a test run. The two escs will not pair to one remote. The owner of meepo told me it would. Am I missing something here?
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-15T20:45:58.701Z Reads: 255

```
Great, this forum will soon be the community for fixing chinese eboards and not a builders forum. Sorry, i wil continue. The owner of meepo board is @kieraneboard.
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-15T20:52:16.966Z Reads: 249

```
I think contacting meepo first would be better than posting here, especially since you've talked to the owner
```

---
## \#4 Posted by: Namasaki Posted at: 2017-09-16T01:50:04.934Z Reads: 236

```
Did you try to pair both at the same time or one at a time?
```

---
## \#5 Posted by: Kooli Posted at: 2017-09-16T01:58:21.687Z Reads: 225

```
<img src="/uploads/db1493/original/3X/5/6/568eade35bf09a8c9942ecef59ad45ec44ab5cbe.JPG" width="375" height="500">Both of those. First pairing one then pairing the other. Then setting both in pairing mode and trying to pair at the same time. I attached a pic of the esc.
```

---
## \#6 Posted by: Kooli Posted at: 2017-09-16T01:59:24.427Z Reads: 212

```
I'm building a custom board. Thanks for your input.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-09-16T02:37:54.470Z Reads: 212

```
You can't pair 2 at the same time. 
You have to pair #1 while #2 is off
Then turn #1 off and turn the remote off
Then  #2 on and pair it.
Then turn #2 off and turn the remote off. 

When you complete this procedure, turn the remote on and then turn both ESC's on at the same time and they should both connect with the remote.

It's really easy when using receivers that are separate from the ESC's 
In your case, you have to be able to power each ESC separately
```

---
## \#8 Posted by: Kooli Posted at: 2017-09-16T03:02:53.123Z Reads: 206

```
Hmm didn't seem to work. After completing what you stated above I turn on both and it only pairs to esc #2. unless I have to turn on both at the exact same second, but I tried doing that.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-09-16T03:46:05.676Z Reads: 205

```
Is the remote and receiver Bluetooth or 2.4ghz RF
I don't think it will work if they are Bluetooth
Never mind, I see they are 2.4 g
The board you have shown appears to have one receiver for a dual esc. 
Are you trying to use 2 of these boards?
```

---
## \#10 Posted by: jourm Posted at: 2017-09-16T07:00:53.120Z Reads: 203

```
Cool to se someone trying this as i have been thinking about it myself for a while, seeing as you can get 2 x double escs for the price of one vesc.
```

---
## \#11 Posted by: DK-Odense Posted at: 2017-09-16T18:23:43.085Z Reads: 194

```
Looks just like the backfire gen2 ESC. 

All those china boards are identical 😁
<img src="/uploads/db1493/original/3X/e/d/ed35ece3ce7421e268a61c94f00645819a9dce9a.jpg" width="374" height="499">
```

---
## \#12 Posted by: Kooli Posted at: 2017-09-16T19:46:49.963Z Reads: 177

```
Yeah two of these boards
```

---
## \#13 Posted by: Namasaki Posted at: 2017-09-17T02:00:37.108Z Reads: 170

```
what remote?
```

---
## \#14 Posted by: Kooli Posted at: 2017-09-17T17:45:42.831Z Reads: 163

```
It looks like this https://meepoboard.com/products/remote
```

---
## \#15 Posted by: Namasaki Posted at: 2017-09-17T18:02:05.059Z Reads: 162

```
Maybe that remote can only pair with one receiver. 
I've been able to operate dual receivers with the Mini RC remote. 
<img src="/uploads/db1493/original/3X/8/b/8b81178de61cd75c492c8bb9fbfcfcec6313ade0.JPG" width="375" height="500">
```

---
## \#16 Posted by: Kooli Posted at: 2017-09-18T06:31:41.350Z Reads: 150

```
Interesting. I would try the mini rc remote but I don't think it'll work with the Chinese motherboard. The meepo dude told me to use a jst pH wire to link the two, I ordered one to see if itlll work but I'm not convinced, it sounds like I'd have to screw with something to really get it to work...
```

---
## \#17 Posted by: Namasaki Posted at: 2017-09-18T12:30:11.798Z Reads: 146

```
As you can see by the pic, I'm using Vescs with separate receivers. 
I'm not familiar with those Chinese boards
```

---
## \#18 Posted by: RetroBorg Posted at: 2017-11-27T12:53:16.879Z Reads: 142

```
Did you ever get both escs to link to one remote?
```

---
## \#19 Posted by: ATLesk8 Posted at: 2017-11-27T15:32:28.002Z Reads: 140

```
@diyeboard ?
```

---
## \#20 Posted by: diyeboard Posted at: 2017-11-27T15:36:34.016Z Reads: 145

```
<img src="/uploads/db1493/original/3X/1/2/12fffea00239ac0fe01a5ec78b921a187bb24a17.jpg" width="666" height="500">
we will lauch this four motor esc kit for belt and hubs soon.
keep your attention on our site www.diyeboard.com  
or my thread on esk8 forum.
http://www.electric-skateboard.builders/t/diyeboard-com-china-factory-direct-retail-electric-skateboard-diy-kits-and-parts/32666/674
```

---
## \#21 Posted by: RetroBorg Posted at: 2017-11-28T11:22:53.775Z Reads: 125

```
What's involved in getting two escs to be controlled by one remote?
```

---
## \#22 Posted by: diyeboard Posted at: 2017-11-28T12:11:36.967Z Reads: 121

```
many issues, the four motors speed must be slightly not same, so the remote can control them well without delay and signal mess. i mean the firmware make four engines of differential speed, and conbine the two esc with one receiver, and change the protocals.
```

---
## \#23 Posted by: Kooli Posted at: 2017-11-29T07:12:06.191Z Reads: 113

```
unfortunately no. I was upsold by meepo and under delivered.
```

---
## \#24 Posted by: RetroBorg Posted at: 2017-11-29T10:00:31.302Z Reads: 109

```
What are the performance changes?

I assume quicker acceleration?

Perhaps slightly higher top speed?

Better braking?

Less range?
```

---
## \#25 Posted by: RetroBorg Posted at: 2017-11-29T10:14:46.609Z Reads: 106

```
I don't believe Kieran would deliberately mislead you just for a sale.
```

---
## \#26 Posted by: Okami Posted at: 2017-11-29T11:42:42.602Z Reads: 107

```
Maybe do what this guy did:

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/6/7/67df5f89df7d1f9f92c866834aa3e68ec2387902_1_375x499.jpg

https://www.electric-skateboard.builders/t/4wd-electric-mountainboard-trampa-holypro-2-x-dual-esc-2-x-6355-190kv-2-x-6374-192kv/39610
```

---
## \#27 Posted by: Hariboisawesome Posted at: 2017-12-07T05:39:13.845Z Reads: 92

```
Dude way to think outside the box!!
```

---
## \#28 Posted by: Jebe Posted at: 2018-03-21T03:33:03.497Z Reads: 75

```
And they are rubbish. Dont trust them. Have 2. Not using either. Throttle acts odd at times, delay in response, brakes as well. Had one totally ignore the remote and just accelerated into a curb.
```

---
## \#29 Posted by: Wilsonliang777 Posted at: 2018-04-22T08:55:55.455Z Reads: 61

```
I am in the process of trying to link 2 single esc to make a dual drive.   Diyeboard had a 2.1 esc thst seems to just stack 2 single esc to make a dual drive.  It seems like all tbey did was connect 6 wires and the power cables.
```

---
## \#30 Posted by: TxFlatRoller121 Posted at: 2018-12-10T17:34:00.546Z Reads: 29

```
this guy did exactly this ! the only solution is to 3d print a dual controller holder which are available on thingiverse.com . this guy did the remote and also 3d printed some offroad wheels in TPU seems to work well check it out. 
 https://www.youtube.com/watch?v=B-Gqwqf2An0
```

---
## \#31 Posted by: TxFlatRoller121 Posted at: 2018-12-10T17:35:00.606Z Reads: 31

```
also if you do not have a 3d printer .. www.shapeways.com you can upload your files and have someone print them for you. :sunglasses::sunglasses:
```

---

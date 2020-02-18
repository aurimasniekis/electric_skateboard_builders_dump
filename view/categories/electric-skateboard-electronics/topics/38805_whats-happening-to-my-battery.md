# Whats happening to my battery?

### Replies: 10 Views: 700

## \#1 Posted by: Geddi Posted at: 2017-11-20T11:04:06.123Z Reads: 154

```
I have been using my first board since July now. And I love it and it works great. The thing is I have never drained the battery further down than 50%. I never had any issues with that, because I usually only go small distances and charge it every day. So the other day I forgot to charge it. I started with about 75% charge and went about 8km. I dropped to about 35%. Now when the battery went lower than that the charge would drop instantly. I could not go even close to fullspeed. When I put to much gas on it the motor would not react anymore until pressed the break function. Then I could accelerate again, but only barely. So the battery was at 30%. After 200m I checked the indicator again and it said 2%. And then it would slowly go back up to 30% when I was not riding it. After the next 200m it turned itself off. And after a minute it was turned back on and back to 30%. What is this madness? Does this have something to do with the cutoff voltage you can define in the VESC settings?<img src="/uploads/db1493/original/3X/9/d/9dcbfc99fee9d0bba44a964f8f55494dc5cde287.png" width="690" height="388">

My setup:

5 LiPo 2S 5000mah 40C batteries from Turnigy
10S BMS from Bestech
Maytech VESC from APS ( have not had the best experience with it. Read more about that here)
APS 200kv 6374 Motor (great motor btw.)
a little battery indicator from APS as well

PS: I also have the feeling that my range dropped quite a bit in general.
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-20T11:20:23.152Z Reads: 139

```
You were hitting the battery cutoffs at 36 and 34v
You can lower to 34 and 33
Those percentage based indicators can be weird, because they rely purely on voltage, while under load they can drop significantly and then recover
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-11-20T11:22:48.671Z Reads: 134

```
You´re hitting a BMS or Vesc cutoff. 
Check your cell voltage from time to time, sometimes they drift a bit and the BMS is not able to manage that if your cells are too far from each other.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-11-20T12:22:57.929Z Reads: 123

```
I guess one of your cells in series is already empty so that they collaps the moment you apply load. Check the single voltage of each series pack. Lipo's can drift a lot. 
The BMS doesn't really help because they can't handle the huge drift while the battery is in use. Guess it doesn't balance at all while in use (would be pointless anyway).
```

---
## \#5 Posted by: Geddi Posted at: 2017-11-20T12:35:50.113Z Reads: 106

```
@Namasaki
You have a similar build. Do think it's that or the VESC setting?
```

---
## \#6 Posted by: pat.speed Posted at: 2017-11-20T12:38:10.576Z Reads: 101

```
Voltage sag are my thoughts too. When the batteries are nearly fully drains they tend to sag more
```

---
## \#7 Posted by: Namasaki Posted at: 2017-11-20T16:38:46.570Z Reads: 82

```
First of all you need to have a voltage meter, not a percentage meter. 
Percentage meters are a joke in my opinion. 
You need to be careful about over discharging Lipos. 
They can't go as low as Li-ions. 
And if you take them below 3.4v per cell, they can drop rapidly from their. 
You can easily ruin Lipos by taking them too low.
```

---
## \#8 Posted by: florensvb Posted at: 2017-11-20T18:42:49.243Z Reads: 64

```
Just a side question i wanna throw in here:
Whats your recommended cutoff for lipos and liions?
```

---
## \#9 Posted by: Namasaki Posted at: 2017-11-20T22:08:34.626Z Reads: 55

```
I have my cutoffs set at 34v start and 32v end BUT, I don't depend on the cutoffs to tell me when my battery is done.
I monitor my total pack voltage by a meter mounted through the top of my deck and I don't run it below 36v although most of the time lately I'm  I don't even go that low.
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-11-21T07:22:23.824Z Reads: 45

```
Lipo: 3,5V cutoff
Liion: 2,8V cutoff
```

---

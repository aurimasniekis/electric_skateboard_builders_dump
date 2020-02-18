# Wanted: 10s BMS System (Solved)

### Replies: 14 Views: 977

## \#1 Posted by: nihliphobe Posted at: 2017-06-02T03:17:48.983Z Reads: 164

```
Looking to buy a 10s BMS system, preferably one of the extras from someone who got stuck with the minimum 2 order from bestechpower. If there are other easier to acquire solid bms systems, I would love to hear about them too!

Thanks in advance all :)
```

---
## \#2 Posted by: jormundur Posted at: 2017-06-02T05:28:00.597Z Reads: 149

```
I'm in your same boat. Looking to buy a 10s with a swithc like @Namasaki uses in his builds. I just saw that alien drieve systems has one.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-06-02T05:31:49.782Z Reads: 148

```
Better to buy it direct from Bestech so that you can customize the adjustable parameters Like low voltage detection. And over current detection.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-02T05:37:33.191Z Reads: 143

```
@nihliphobe @jormundur

Are you guys in the USA?
```

---
## \#5 Posted by: nihliphobe Posted at: 2017-06-02T05:38:17.830Z Reads: 133

```
That is a good point, thanks man. I suppose I can always pass along the second one on here! Do you happen to know what I should customize those parameters to for a 10s4p pack?
```

---
## \#6 Posted by: nihliphobe Posted at: 2017-06-02T05:38:30.255Z Reads: 125

```
I am in the US of A :)
```

---
## \#7 Posted by: Namasaki Posted at: 2017-06-02T05:47:56.124Z Reads: 127

```
I have one for Li-ion packs and another for Lipo packs.
You can use the Lipo settings fro Li-ion if you don't want to drain your cells below 3.0v

**Li-ion parameters**
<img src="/uploads/db1493/original/3X/b/c/bc58929c32295d0a9a65852f61f36f14722e91e7.png" width="389" height="500">


**Lipo parameters**
<img src="/uploads/db1493/original/3X/9/d/9d6a90c730691eb35a06cf54cf9eacd2f2b7ac60.png" width="392" height="500">
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-02T06:11:23.897Z Reads: 112

```
Email Lucy Li  
 lucy@bestechpower.com
Request to purchase 2 of these and attach the spec sheet.
It takes about 2-3 weeks for delivery.
They have to set them and test them before they can ship them out.
they will send you an invoice by email and you pay by PayPal
```

---
## \#9 Posted by: jormundur Posted at: 2017-06-02T20:36:19.166Z Reads: 96

```
I'm in California near LA. I'd definitely be down to take one if your ordering. I would be using 2s 5000mah 60C hardcase lipos like @Namasaki has done in his boards. Would the same parameters as above fit that build?
```

---
## \#10 Posted by: nihliphobe Posted at: 2017-06-03T06:18:34.629Z Reads: 87

```
Quick question, what happens if I bought a unit for use with a li-ion system but the over current detection current set to 240A? Would that risk damaging the board? I have an opportunity to buy a bms with those settings and am unsure of the potential damage. Thank you for all the info, it's been extremely helpful!
```

---
## \#11 Posted by: Namasaki Posted at: 2017-06-03T11:58:25.864Z Reads: 74

```
240a over current detection is the default setting because it's the most that the bms can handle. 
If your running a Vesc, that setting will not matter because you will control max current by the Vesc settings.
```

---
## \#12 Posted by: zeno Posted at: 2017-06-03T12:18:20.363Z Reads: 76

```
Lipo temperatures set here (0 ~ +85 degrees) are different then your own build topic (-40 ~ +85 and -20 ~ +125 ) what would be recommended? My guess would be the 0~85 but not sure.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-06-03T13:34:34.177Z Reads: 73

```
The temp range on both where default settings. 
The default settings where changed by Bestech. 
These temp settings are FET temps not battery temps. 
The upper limit is important to prevent overheating of the FET's but the lower is irrelevant when set below zero. 
The reason for storage temp;
The bms, from what I've seen, continues to monitor and balance the battery even when it's turned off. 
So you can fully charge your battery and then turn the bms off and it will continue to balance the cells and prevent voltage swelling making it safe to charge your board up the night before a ride. 
But, if your planning to store your board for extended period of time. You might want to do a storage charge and disconnect the bms from the battery.
```

---
## \#14 Posted by: zeno Posted at: 2017-06-03T13:46:56.084Z Reads: 69

```
Thanks for the info!
```

---

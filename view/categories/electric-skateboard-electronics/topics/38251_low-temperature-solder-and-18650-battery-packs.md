# Low Temperature Solder and 18650 battery packs

### Replies: 32 Views: 1635

## \#1 Posted by: skelstar Posted at: 2017-11-14T02:18:38.242Z Reads: 198

```
I had [what I thought was] an epiphany last night: 

I want to build an 18650 battery pack but I don't have a spot-welder. I don't really want to buy one. I was going to have a go at soldering the packs but I'm aware that it's not a great idea. I was going to try anyway.

I remembered back to when I was an electronics engineer (technician mostly) and we used to use a low-temperature solder. I was wondering why you couldn't use some of this low-temp solder to solder nickel strips to 18650 battery packs. 

Maybe a higher-resistance? 

Solder would melt when battery pack was under load?

Keen to hear thoughts.
```

---
## \#2 Posted by: skelstar Posted at: 2017-11-14T02:20:15.623Z Reads: 194

```
An example from my favourite store: [Aliexpress.com low temperature solder](https://www.aliexpress.com/item/High-Purity-Low-Temperature-Solder-Line-Rosin-Core-Wire-Welding-Soldering-Iron-Accessories-2017-New-Arrival/32817812784.html?
```

---
## \#3 Posted by: skelstar Posted at: 2017-11-14T02:32:37.656Z Reads: 188

```
Also: you seem to be able to buy 18650 batteries that have tabs already welded to them (have been able to for years), but maybe they aren't high-discharge batteries.
```

---
## \#4 Posted by: scepterr Posted at: 2017-11-14T02:34:05.002Z Reads: 184

```
It will break apart under vibrations, low temp solder is used for desoldering, is then removed and proper solder applied
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-11-14T02:41:18.478Z Reads: 172

```
Yeah, lo-temp solder is a bad idea, especially with nickel strips. The heat up during heavy discharge, and that could cause the solder to melt and either come loose, or cause a short. 

If you're going to solder (And it can be done, done well and safely if you are careful and practice) then it's worth going whole hog and using copper wire, strip, or braid.
```

---
## \#6 Posted by: skelstar Posted at: 2017-11-14T02:46:34.691Z Reads: 167

```
AH good point (@scepterr). It's been a few years since I used it (literally for desoldering).

I might get some 18650s (10s1p probably) when I find some at a good price. I live in New Zealand so I generally have to pay freight unless get some good ones from AliExpress.
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-11-14T03:11:40.683Z Reads: 152

```
10s1p won't give you much current. 18650s don't really shine as a battery for esk8 unless you have at least a 3p pack.
```

---
## \#8 Posted by: skelstar Posted at: 2017-11-14T05:58:00.811Z Reads: 135

```
Just want to build a really low profile battery pack so it's really stealth (like everyone does I guess).

Cheers for advice.
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-11-14T06:02:08.545Z Reads: 130

```
If you want stealth and don't mind the range taking a hit, I'd recommend getting some 1s or 2s lipos and stringing them together into a nice flat pack. They'll handle the current much better than a small 18650 pack would.
```

---
## \#10 Posted by: skelstar Posted at: 2017-11-14T06:10:35.290Z Reads: 127

```
I have got two 5S 5000mAH lipo packs coming. It doesn't say how many cells in series, but I guess the 5AH batts suggest that.

Was reading about how someone took packs like that and disassembled them and spread them out. Makes me nervous. Maybe on v2 of my board.
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-14T06:17:46.586Z Reads: 113

```
5S means 5 in Series
```

---
## \#12 Posted by: E1Allen Posted at: 2017-11-14T06:38:57.670Z Reads: 110

```
Yeah, what mystical said. 10s1p of 18650 gives you what? Maybe 15a continuous? 30 peak.   2p gives you 30/60a. 1p won't give you much. Your 5s lipo in series for 10s are probably 20 or more C discharge so 5ahx20=100a. Which is doable, u can make it flat and is cheaper in the short run.  Lipo is more picky than lion though. Not supposed to leave charged and they don't like being punctured.  However opening the package to flatten the cells is acceptable.
```

---
## \#13 Posted by: florensvb Posted at: 2017-11-14T07:14:14.792Z Reads: 97

```
Now this got me kinda curious: What would you guys recommend is the safe-zone melting point for solder? In degrees celcius if possible :D
```

---
## \#14 Posted by: MysticalDork Posted at: 2017-11-14T07:19:45.857Z Reads: 90

```
It depends on the thermal mass of the soldering iron tip. Regular 60/40 leaded solder melts at 183C, and a good soldering temperature is 300C. But if you have a small/low wattage iron and you try to solder large wire, it's going to suck a lot of heat out of the tip and you may need to set the temperature higher to compensate. To solder battery terminals, you want the spend the least amount of time possible, because less time means less heat into the battery. A large, high thermal mass iron is ideal because it can melt the solder really fast.
```

---
## \#15 Posted by: florensvb Posted at: 2017-11-14T07:21:35.577Z Reads: 87

```
aalright thats good to know cause my electrical solder melts at 181 :D i do have a 100w iron that does the job really quick. just wondered if my first pack that i built a few days ago is going to melt away when i burst the throttle hahahah
```

---
## \#16 Posted by: MysticalDork Posted at: 2017-11-14T07:24:26.160Z Reads: 88

```
What sort of connections are they, and how thick? Nickel has 4x the resistance of copper.
```

---
## \#17 Posted by: florensvb Posted at: 2017-11-14T07:25:45.219Z Reads: 88

```
http://www.electric-skateboard.builders/t/new-single-build-for-my-brother/34155/55?u=florensvb
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-11-14T07:27:17.530Z Reads: 87

```
Oh yeah, you'll be fine.
```

---
## \#19 Posted by: florensvb Posted at: 2017-11-14T07:27:41.911Z Reads: 88

```
good to hear :)
```

---
## \#20 Posted by: MysticalDork Posted at: 2017-11-14T07:28:01.370Z Reads: 85

```
If your wires get hot enough to melt solder, that means you have other problems, namely the cells trying to make it into orbit.
```

---
## \#21 Posted by: florensvb Posted at: 2017-11-14T07:28:42.991Z Reads: 81

```
hahhhahhaha got me laughing out loud alone in my room hahha
```

---
## \#22 Posted by: MysticalDork Posted at: 2017-11-14T07:29:52.030Z Reads: 83

```
Then my work here is done for the night. I gotta get some rack time, work in the morning.
```

---
## \#23 Posted by: florensvb Posted at: 2017-11-14T07:30:30.491Z Reads: 85

```
haha my day is just starting: 8.30 am. Sleep well brothaaa
```

---
## \#24 Posted by: rene Posted at: 2017-11-14T07:40:19.414Z Reads: 82

```
Got myself this nice cheap Arduino Spot Welder v3 running with the 5000mAh 3s 130C.

https://www.youtube.com/watch?v=CNmvx2JSCvA
```

---
## \#25 Posted by: skelstar Posted at: 2017-11-14T07:57:50.488Z Reads: 80

```
NICE (@rene). Got me thinking now.
```

---
## \#26 Posted by: scepterr Posted at: 2017-11-14T08:14:55.141Z Reads: 76

```
It's awesome, do .20 nickel all day long
<img src="/uploads/db1493/original/3X/5/8/5844f7598ac0e69561b0dada3fcc4fbf6de39613.jpg" width="666" height="500">
```

---
## \#27 Posted by: skelstar Posted at: 2017-11-14T08:26:46.090Z Reads: 74

```
How cheap? What do you do for power supply?

Also, do you make many battery packs?
```

---
## \#28 Posted by: rojitor Posted at: 2017-11-14T09:31:49.617Z Reads: 69

```
if you don't wanna spot weld you wanna solder them asap so you better use a superfast 100w solder. it's better if you apply max heat for the minimum time possible.
this is the one second solder technique:
[https://www.youtube.com/watch?v=0ZRwMXL-Rvs](https://www.youtube.com/watch?v=0ZRwMXL-Rvs)
nevertheless i prefer spot welding..The damage is always lower.
[https://www.youtube.com/watch?v=byvr-dwwao4&t=1s](https://www.youtube.com/watch?v=byvr-dwwao4&t=1s)
```

---
## \#29 Posted by: skelstar Posted at: 2017-11-14T17:03:39.500Z Reads: 65

```
Thankfully I have a pretty nice Hakko (spelling?) solder station. Might purchase a bigger tip for it though.
```

---
## \#30 Posted by: MysticalDork Posted at: 2017-11-14T17:21:20.424Z Reads: 64

```
Get some good flux. I use "Ruby fluid" liquid flux, it helps the solder wet out and stick to the nickel battery contact with minimal heat. Works way better for that than rosin flux.

I basically go around and tin the contacts of all the batteries in a row, then let them cool while I tin the copper braid. Then I let that cool, and then solder them together. It's very fast that way and you don't get heat buildup.
```

---
## \#31 Posted by: skelstar Posted at: 2017-11-14T17:22:40.064Z Reads: 59

```
Right...  so copper-braid instead of nickel? ... or both?
```

---
## \#32 Posted by: MysticalDork Posted at: 2017-11-14T17:29:03.743Z Reads: 55

```
I'm a proponent of copper and solder over spot welding and nickel. It's just more robust for high current applications.
```

---

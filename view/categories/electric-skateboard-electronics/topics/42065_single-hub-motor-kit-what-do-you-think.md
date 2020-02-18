# Single Hub motor kit, what do you think?

### Replies: 15 Views: 1363

## \#1 Posted by: westonbe Posted at: 2017-12-28T08:04:01.408Z Reads: 159

```
Hi Guys,

I've built a single motor belt drive board. The board worked until I pushed it up a hill and blew out the motor. So I've decided to try out a hub motor build. Do you think this hub motor really has a top speed of only 25 km/h(link below)? It says the max voltage allowed is 36 V but I'm not sure if that really means 42 V at 10S (full charge) or if means 8s at full charge? I was wondering if you guys know or think I could run this kit with a 10s lipo and if you think I could push it faster than 25 km/h? Any help is greatly appreciated. Thank you for your time!

Wes

http://vi.vipr.ebaydesc.com/ws/eBayISAPI.dll?ViewItemDescV4&item=263192451180&t=1509414471000&tid=10&category=165945&seller=fibreskate&excSoj=1&excTrk=1&lsite=0&ittenable=false&domain=ebay.com&descgauge=1&cspheader=1&oneClk=1&secureDesc=0
```

---
## \#2 Posted by: pakue Posted at: 2017-12-28T12:49:49.156Z Reads: 133

```
The 25 km/h may be even too high depending an your weight as this hub motor won’t have as much power output as a belt drive due to thermal limitations. 

36V usually means 10S.
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2017-12-28T14:36:54.737Z Reads: 112

```
That's a *really* small hub motor. I doubt it will get you to 25km/h or be able to climb any hills. What happened with the other motor? Perhaps we can take a look at it, try to fix it or something.
```

---
## \#4 Posted by: ATLesk8 Posted at: 2017-12-28T16:22:57.560Z Reads: 88

```
If you blew up the belt drive going up the hill the this hub will be wayyy worse...just switch to a dual drive or a bigger motor
```

---
## \#5 Posted by: michichopf Posted at: 2017-12-28T16:23:53.420Z Reads: 80

```
Blew up belt drive? how do you mean? belt ripped? mount broken ? motor damage ?
```

---
## \#6 Posted by: westonbe Posted at: 2017-12-28T18:45:12.334Z Reads: 69

```

<img src="/uploads/db1493/original/3X/a/2/a2a312f8712a7b178ba19cddd084809fe7194e66.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/8/8/88fb5778181066b6fce6c3cc15740ebce8464f14.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/8/e8bd740b087ad907eb242c4f27a506bbcc2792f3.jpg" width="374" height="500">
```

---
## \#7 Posted by: westonbe Posted at: 2017-12-28T19:00:04.624Z Reads: 60

```
So I originally designed and used a two piece mount on these square trucks (below) because I heard of a lot of mount slippage issues occurring with rounded trucks. After a lot of jb weld and failure I have redesigned the mount into one piece, but need to find a different cnc shop etc to cut the new mount. My motor stopped working and sticks a little when I try to rotate it by hand. Some people have said it's due to melted wire (I have no idea though. I tried a diagnosis in bldc tool and nothing showed up(motor detection failed, bad results). I am not sure if the drv on my vesc blew, but will be able to test it on my next build(was wondering if any of you guys had similar issues). I tried taking apart my motor but the screw (touched by the screw driver in the pic above) is stripped and I tried drilling it out with a small drill bit but had no luck. If I get this hub motor set up it would allow me to skip over the cncing and getting a new motor, which is a plus, at the sacrifice of speed and better quality of course. My vesc is covered by the 2 year ollin warranty so I'm not too worried about that(if it is the issue). This first board hit 35 mph which was way too fast for me so I'm not mad if the new single hub is slower. What do you guys think? Again, I greatly appreciate any input you guys have and wanted to thank you for replying and reading my post. 

Square trucks: https://www.muirskate.com/longboard/trucks/2194/150mm-bennett-raw-6-0-inch-longboard-skateboard-truck

(board specs: single 12s, 6374 turnigy, 83 mm wheels, 36:16 gear ratio, 290 mm belt)
```

---
## \#8 Posted by: faithfulpuppy Posted at: 2017-12-28T19:03:16.824Z Reads: 59

```
is your motor mount bolted to your deck? oh my.
```

---
## \#9 Posted by: faithfulpuppy Posted at: 2017-12-28T19:03:56.942Z Reads: 61

```
also, what's your motor Kv? i might be interested in buying it (broken)
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2017-12-28T19:06:42.702Z Reads: 61

```
and what part specifically brok?
```

---
## \#12 Posted by: westonbe Posted at: 2017-12-28T19:13:30.727Z Reads: 61

```
A stabilization bracket (used to reduce vibration because the two piece mount, which I copied from a youtuber and enertion, kept loosening) keeps the mount in place. The new mount I've made is a single piece, and will fit onto the square profile of the truck perfectly after filing the axle hole a small amount(designed with slightly more material in the hole to be filed off). It won't vibrate, like the last one did, haha. I have no idea what broke on the motor, but it's in pretty bad shape. It's a turnigy 192 kv sk3. I'd like to fix it if possible, but as you can see below, the screw is stripped, and after trying to drill into it (two broken drill bits later), it's been flattened down. <img src="/uploads/db1493/original/3X/e/b/eb86707c3aa54dc41398662ddfcf0566d6f0b532.jpg" width="374" height="500">
```

---
## \#13 Posted by: westonbe Posted at: 2017-12-28T19:40:11.290Z Reads: 55

```
Yea, I'm just gonna go with caliber trucks and the diyesk8 mount, and get a new motor =/. I'll have a cool story to tell when submitting my resume, I guess.
```

---
## \#14 Posted by: GrecoMan Posted at: 2017-12-28T19:46:17.193Z Reads: 53

```
you tried a stripped screw remover? worked for me when my motor mount set screw got stuck
```

---
## \#15 Posted by: westonbe Posted at: 2017-12-29T03:35:01.103Z Reads: 46

```
Yea I need to get one small enough
```

---
## \#16 Posted by: westonbe Posted at: 2017-12-30T03:13:26.443Z Reads: 35

```
So here's the new mount I made for these trucks: https://www.muirskate.com/longboard/trucks/2194/150mm-bennett-raw-6-0-inch-longboard-skateboard-truck

Ideally it should not require any set screw tightening because of the corner edge grip. It must be filed down after being cut.
The fea looks good and the part won't fail with a static load. I didn't account for motor torque and didn't do fea for frequency analysis because most people on this site have said that a minimum thickness of 9 mm is ideal for the mount. I ended up buying a torque board mount kit to avoid remachining (limited time due to other projects). If anyone wants to actually try machining this mount and putting it on the truck, hit me up. <img src="/uploads/db1493/original/3X/c/6/c619dbfe1a5a088f28c502e26a4a6d70c1fb1579.jpg" width="690" height="232"><img src="/uploads/db1493/original/3X/3/7/3783b9ee381f0b6f9acfe5542538fdc069194291.jpg" width="690" height="232">
```

---

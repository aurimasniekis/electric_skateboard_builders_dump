# Basic Bamboo &#124; SCSK8 Bamboo Kicktail &#124; Yocaher Trucks &#124; Turnigy 6364 245kv &#124; Custom Welded &#124; 6s (3sx2) Zippy &#124; FVT ESC

### Replies: 14 Views: 3584

## \#1 Posted by: jakobnator Posted at: 2016-03-05T05:31:17.586Z Reads: 233

```
Just finished my first build!

I did it relatively cheap but without skimping, don't know the exact total but probably in the low 300$ range. I will post more detailed pictures/ answer questions as requested. 

**Build Process (don't expect award winning writing)**

**Drive Train:**
Designed the mount in 123D (Baby's first CAD software) and got it cnc'd out of aluminum and welded onto el cheapo trucks from amazon. All for free at my universities fabrication lab! I had to do some minor filing for the mount to get as far down the shaft as possible, the truck is a weird tapered, triangle-ish shape. I pretty much eye-balled the levelness of the mount as the professor spot welded it until he did the full weld. After a lot of frustration trying to drill holes in washers and gears perfectly spaced apart I remembered I built a 3d printer last summer and printed a 40t pulley (4 perimeter 35% infill, ABS) and mounted with ease. The wheels are cheap ebay flywheels and came with surprisingly good bearings. Overall I am happy with the setup, I get a decent amount of cogging if I am not careful with the acceleration but I think its mainly due to the acceleration which I will touch on later. I go to university where it is completely flat, so the cogging only happens when you try to start from zero momentum or try to slam the throttle way to fast, its manageable though.

**Electronics**
This is were thing got....unfortunate. 

When putting the two 3s batteries in series I accidentally connected the balancing plugs to they y junction backwards. When I connected the main negative and positive leads (to put them in series) they welded together and I quickly cut the connection. No visible damage to the batteries but I had to resolder some of the wires as the old ones fried. After connecting them they appear to work,except after driving about 1/2 mile it starts not throttling and the ESC indicates that its got a low voltage even though the voltage is fine. To fix it I have to turn it off leave it for a few minutes then its good for another 1/2 mile or so. Anyways I used 10 AWG wire which was probably overkill. Using a FVT ESC had I known the VESC was going on sale I probably would have waited and I am really not fond of the slowest acceleration setting on the FVT ESC. 

**Enclosure & Ports**
Bought generic "Hammond" abs boxes and mounted them on opposite ends to hopefully help with the clearance issues of these gigantic boxes. Looking back I probably could have 3d printed a case and laid the individual cells flat, but I surprisingly haven't scraped the boxes yet coming down a curb. The bigger box has the batteries and wires to a xt90 charging port, and 6s balancing port epoxied into the side of the box for easy access. The Front box has an xt90 "key" used to turn it on and off. 

Overall happy with my build hopefully my batteries aren't busted open for questions, pictures or insight on my problem above. 

EDIT: It appears the ESC is blinking green which actually means overheating. Any good ways to cool this ESC? the box is enclosed because I wanted it somewhat weatherproof. Perhaps drill some holes in the box?

<img src="/uploads/db1493/original/2X/c/c8d45ce7c2af8d75e9239f6705a534397f8f6d4b.jpg" width="282" height="500"><img src="/uploads/db1493/original/2X/9/9538386d1f4f0e50b7e814469f3684d512812634.jpg" width="282" height="500"><img src="/uploads/db1493/original/2X/7/783f3c323de97055b736d91df8c7d704b181f7fa.jpg" width="282" height="500"><img src="/uploads/db1493/original/2X/5/5459431fc2e9fc929e00b91f2be77c2ac52649ad.jpg" width="282" height="500"><img src="/uploads/db1493/original/2X/e/e58261ce86745fe52fb96dc987db892f73494d01.jpg" width="282" height="500"><img src="/uploads/db1493/original/2X/1/11ab884773c46c4eeddacc28992270a81769df43.jpg" width="282" height="500">
```

---
## \#2 Posted by: xalitust Posted at: 2016-03-06T06:47:04.133Z Reads: 205

```
Nice board! 
What motor are you running?
```

---
## \#3 Posted by: mostwanted Posted at: 2016-03-06T10:56:46.821Z Reads: 202

```
looks to me like hobbyking Turnigy SK3 6374 ...
i think ....
```

---
## \#4 Posted by: jakobnator Posted at: 2016-03-06T16:53:07.552Z Reads: 194

```
Turnigy sk3 6364 245kv

Very beefy for a single motor setup. I honestly don't feel the need to go dual motor, still haven't pulled throttle all the way back.
```

---
## \#5 Posted by: Iceni Posted at: 2016-03-06T17:11:03.246Z Reads: 187

```
Regarding the ESC overheating, though I'm not familiar with the FVT, if it's got a cooling fan it would need some ventilation holes to pull air through.
Very few, if any, actively cooled ESCs can be mounted in an enclosed case.

Or go overboard and install a watercooling system in place of the fan and route the pipes to a radiator on the outside of the case ;)
```

---
## \#6 Posted by: jakobnator Posted at: 2016-03-06T18:11:23.669Z Reads: 181

```
I just drilled 3 0.5" holes in the front of the esc box and 2 on the back. Didn't seem to make much of a difference. Strange because I am seeing forum posts about how great the esc is and how they even took the fan off and didn't have any problems. It may be that I am testing it on a huge hill, but I was having problems on flat ground at my university.
```

---
## \#7 Posted by: lowGuido Posted at: 2016-03-09T00:28:01.735Z Reads: 182

```
I have removed the fan from one of my ESC's and run it for about a year and a half now no issues. however I have placed the heatsink in the airflow under the board.
<img src="/uploads/db1493/original/2X/4/4dc3c23eb92b6429c2c8a99619241072b9a008e0.jpg" width="690" height="388">

P.S.
I like the shape of your board.
```

---
## \#8 Posted by: jakobnator Posted at: 2016-03-09T21:49:45.456Z Reads: 171

```
I might try taking the fan off but sticking the heatsink through a hole in the side of my enclosure and create a somewhat weatherproof seal. Just out of curiosity what do you use for ESC settings?
```

---
## \#9 Posted by: lowGuido Posted at: 2016-03-09T22:06:38.240Z Reads: 164

```
I started with: 
forward/brake no reverse
maximum motor timing
minimum punch
50% brake
```

---
## \#10 Posted by: jakobnator Posted at: 2016-03-21T04:02:13.663Z Reads: 151

```
Just re flashed the firmware from apparently some experimental "e board" firmware from FVT. HUGE difference, great acceleration and braking curves and there are only three quick beeps instead of the annoying 8 when its powered on. 

https://endless-sphere.com/forums/viewtopic.php?f=35&t=73851
```

---
## \#11 Posted by: minimorris77 Posted at: 2016-04-28T01:13:44.143Z Reads: 136

```
Did you have to get a usb programmer to update the firmware?
```

---
## \#12 Posted by: jakobnator Posted at: 2016-04-29T04:30:47.624Z Reads: 123

```
Yes I did, looking back buying the ESC and the programmer wasn't much cheaper than a VESC...
```

---
## \#13 Posted by: Pablo_702 Posted at: 2016-06-28T22:43:01.669Z Reads: 93

```
how did you permanently fixed those ports on your enclosure, im having a hard time figuring out that part
```

---
## \#14 Posted by: jakobnator Posted at: 2016-06-28T22:45:42.922Z Reads: 97

```
[quote="Pablo_702, post:13, topic:1669"]
your enclosure, im having a hard time figuring out that part
[/quote]

Drilled holes and filed out to get a tight fit with the xt90 and balance port, then stuck them in and epoxied the back from the inside, only downside is they are permanent. In my new enclosure I hot glued a bracket to the port then used m3 bolt and nut to hold it in place in case I need to replace them.

EDIT: Most recent update on board, swapped for VESC and new 3d printed enclosure:

http://www.electric-skateboard.builders/t/low-profile-3d-printed-6s-enclosure/5625
```

---

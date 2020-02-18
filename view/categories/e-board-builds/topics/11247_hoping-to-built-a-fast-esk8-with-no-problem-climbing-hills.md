# Hoping to built a fast ESK8 with no problem climbing hills

### Replies: 43 Views: 3531

## \#1 Posted by: AHS Posted at: 2016-10-16T17:53:28.534Z Reads: 276

```
Hi Guys! I need help and tips for my built, especially on items. I live in Malaysia so shipping would be very costly for me so I hope to get all things right before all my purchase is done.

My current list:

Motor: Alien 6374 Outrunner brushless motor 240KV 3200W
http://alienpowersystem.com/shop/brushless-motors/alien-6374-outrunner-brushless-motor-240kv-3200w/

Motor mount, wheels, etc: Single Motor Mechanical Kit by diyelectricskateboard

Speed controller: VESC BLDC Speed Controller by diyelectricskateboard

Controller: Alien Power System 2.4Ghz Electric skateboard Remote control
http://alienpowersystem.com/shop/radio-transmitters/alien-power-system-2-4ghz-electric-skateboard-remote-control/

Battery: SPACE Cell pro ( can anyone confirm if this battery is compatible with my motor or not? i couldn't find an answer.)

Do tell if there is any missing parts or things to improve. I'm seriously in doubt with the battery and motor, so some explanation there will be highly appreciated. Thanks Guys!
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-16T18:43:06.283Z Reads: 263

```
KV of your motor is too high for a 10s battery such as the SPACE Cell. Try to get a motor 200kv or less.
```

---
## \#3 Posted by: AHS Posted at: 2016-10-16T19:11:00.226Z Reads: 255

```
But the specs say the max volt is 10s, that's why i opted for the space cell. :sweat_smile:
Though, what Kv motor could you advise me on?
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-10-16T19:21:55.182Z Reads: 245

```
The problem is not the motor itself, it is the VESC.
The Vesc cant handle more than 60000 ERPM(Voltage*kv*7)
In your case, it would be (36*240*7=60480)Slightly above with nominal voltage,
but 70560ERPM on full charge.

I would recommend 190kv
Something like this:
https://electric-skateboard.market/product/190kv-sensored-motor-6354-6374/
```

---
## \#5 Posted by: Jinra Posted at: 2016-10-16T19:32:48.636Z Reads: 230

```
What @flatsp0t said. I use this one myself.

http://www.ollinboardcompany.com/product/om5065-200kv
```

---
## \#6 Posted by: AHS Posted at: 2016-10-16T19:47:45.040Z Reads: 215

```
I get it now! I wasn't aware of the limit the VESC had before this. Totally understand now.
Thanks a lot! @flatsp0t and @Jinra. If there is anything else I need to know, do notify me. Really appreciate it!
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-16T22:46:37.655Z Reads: 189

```
I'm using 190kv with 10s  and Vesc. Dual setup. Plenty of speed and hill climbing power yet very dependable and no overheating.
```

---
## \#8 Posted by: ajaynagra Posted at: 2016-10-16T22:51:57.138Z Reads: 183

```
Are you in Europe or USA.

Europe Parts

https://eu.electric-skateboard.market/store/polar/

USA Parts

https://electric-skateboard.market/store/polar/
```

---
## \#9 Posted by: AHS Posted at: 2016-10-17T04:18:41.630Z Reads: 167

```
@ajaynagra  I'm in Asia 😅
```

---
## \#10 Posted by: AHS Posted at: 2016-10-17T04:20:43.816Z Reads: 164

```
How about for single motor? Will it work as well as dual?
```

---
## \#11 Posted by: Namasaki Posted at: 2016-10-17T04:24:55.752Z Reads: 160

```
dual will always be better even if your just riding on flat ground because your dividing the load between  2 Vescs and 2 motors. So each is caring ½ the load that a single would.  Also acceleration and braking is more  efficient, balanced and stable.
```

---
## \#12 Posted by: AHS Posted at: 2016-10-17T05:28:00.758Z Reads: 153

```
But the cost would also be almost twice. 😂
```

---
## \#13 Posted by: saul Posted at: 2016-10-17T13:22:33.697Z Reads: 149

```
A single 6374 can handle hills but only if you carry enough speed into it.

If you have lots of steep hills you need dual, or to walk....but I use lipo, space cell output is a bit low. Seem fine for a single.

Shipping is an issue I don't see why you want 3 vendors when 1 or two could do.
```

---
## \#14 Posted by: AHS Posted at: 2016-10-17T14:37:10.659Z Reads: 143

```
Well, 2 vendors offer free shipping according to the amount of my purchase. So it's a slight win for me there. 😬
```

---
## \#15 Posted by: Namasaki Posted at: 2016-10-17T15:40:38.606Z Reads: 139

```
I started with Lipos then switched to Li-ions with a BMS and now I'm using Lipos with a BMS. 
Pound for pound, Lipos have more power.
```

---
## \#16 Posted by: IDVert3X Posted at: 2016-10-17T16:25:00.410Z Reads: 139

```
Like @Namasaki said, if you need a lot of current ( which you will need for those hills ), Li-Ions are not an option ( you don't want to pull more than 10A per cell even if they are rated for 20A ).
Well, they might be an option, but you would have to do like 10S8P pack which would be HUUUGE.
It's just so much easier with LiPos for those high-power builds thanks to their small internal resistance and shape. You just have to be more careful working with them and properly balance-charge them.
```

---
## \#17 Posted by: AHS Posted at: 2016-10-17T20:31:33.806Z Reads: 132

```
Thanks @Namasaki and @IDVert3X will bear those things in mind. Though I want something easy to charge and carry around. How much power does a motor take in though? I've read some people say that motors don't even take up to 30A unless really inclined hills. Maybe I'm understanding things wrong here. 😅 Sorry.
```

---
## \#18 Posted by: IDVert3X Posted at: 2016-10-17T21:03:20.140Z Reads: 126

```
Depends on your weight, hill grade, wind, speed...
You can calculate how much power you need using complex physics formulas, but to keep things simple: it can draw much more than 30A climbing steep hills. Prob. max. power you will EVER need is ~3kW ( really steep hill, 95kg rider, high wind resistance ... dont ask me how I calculated it ), which is about 70A at 12S. LiPo can do that without any problems, 4P Li-Ion will have terrible voltage sag and heat up fairly quickly. But that is really the worst case scenario. Most of the time, you should be under 15A on flats. I cant really provide you with exact number coz there are so many factors... Also, I have never built an eskate before, I'm planning my build for early 2017 when VESC 6 and other cool stuff will be out. I have just got quite some experience with electrical engineering, high-current devices, batteries, electric motors in general and so on.

If you want something easy to charge, just use BMS with balancing.
```

---
## \#19 Posted by: AHS Posted at: 2016-10-17T21:12:33.504Z Reads: 120

```
I see. Really nice input man! Thought of stalling my built too, but these things just excite me too much. Anyway, probably need to do a little more reading on LiPo now. Haha. Really appreciate the help. Thanks!
```

---
## \#20 Posted by: Namasaki Posted at: 2016-10-18T01:54:15.674Z Reads: 120

```
If you really want high performance going up hill. 
Consider building a dual beltdrive system with 6355 190kv motors and a 10s Lipo battery system similar to the build I did with 300a continuous capability 
Voltage sag on 12% grade is only 1volt 
That's with a 188lb rider.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-10-18T01:56:04.769Z Reads: 116

```
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#22 Posted by: AHS Posted at: 2016-10-18T08:33:35.460Z Reads: 98

```
Quick question, will the vesc limit the battery discharge up to 50A? Because the specs say up to 240A for a few seconds or 50A continous. However some battery packs have a 40A fuse like the space cell and 80A like the Epower. Just trying to understand 😅. Like if using a Lipo will give you more power, will it damage the vesc?
```

---
## \#23 Posted by: IDVert3X Posted at: 2016-10-18T10:21:42.450Z Reads: 93

```
VESC pulls as much current as it needs, but you can limit it of course to something like 40A per VESC. If you use two of them, the load ( and so current ) will spread between them. Just don't overload it ( you should not be able to fry it with two motors and correct configuration tho ).
Battery pack rated for 50A is just NOT ENOUGH.
You don't want to pull more than 1/2 of the current battery is rated for.
That's why enertion puts 40A fuse on their "80A rated" battery pack. 
They know it's real limits and rate it for 40A, enough for most people. For hill climbing? Not really.
Just get something that can deliver 150A+ continous current, then you should be totally safe.
Most LiPos can do that without any problem.

Multistar batteries are not a good option from experience.
I use one for my high-power LED project which draws about 30A from 5.2Ah battery rated for 52A continous.
It gets hot fairly quickly and voltage sag a lot. I would say it's more like 4-5C than claimed 10C.
```

---
## \#24 Posted by: Namasaki Posted at: 2016-10-18T13:38:19.645Z Reads: 84

```
I agree with everything that @IDVert3X has said. 
That is why after some trial and error, I have ended up using Lipos 5000mah 60c. 
At 10s I'm pulling less than 10% of my battery's continuous current capability.
```

---
## \#25 Posted by: AHS Posted at: 2016-10-18T17:06:28.990Z Reads: 81

```
Thanks guys for the intel. It was really helpful! now i just have to find the right lipos. How much range do you get with a 5000mah anyway @Namasaki ?
```

---
## \#26 Posted by: Namasaki Posted at: 2016-10-18T17:40:46.802Z Reads: 76

```
Actual mileage can depend on many factors but for a ball park idea I  usually got around 12 miles with
12s/5000mah/25c on a dual belt drive. 
I haven't had a chance to do a full range test yet with my 10s/5000/60c battery. But the other day I went 
7 miles on flat ground with some wind and still had 80% battery left.
I have found that higher C ratings can have a very positive effect on range. 
Simply because of reduced voltage sag.
```

---
## \#27 Posted by: AHS Posted at: 2016-10-18T17:48:42.919Z Reads: 77

```
So guys, I've just ask Enertion about the space cell. They said that the 40A fuse could be exchange to a higher Amp fuse. But only if it repeatedly blows (indicating you probably need more power right?). So, I think I can get more juice if needed in the future if I choose to purchase it. On the other hand, I've been doing some research on lipos. I was wondering if it'll be alright for me who lacks the technical background and knowledge ( I'm a medical student :sweat_smile: ). I mean, I've read some threads (correct me if I'm wrong) that there are a few techniques for soldering certain apparatus. Something thats needed to connect the BMS right? Just a little paranoid here. Haha.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-10-18T17:53:52.757Z Reads: 74

```
Connecting a BMS to Lipos is easy and I could walk you through it.
```

---
## \#29 Posted by: AHS Posted at: 2016-10-18T17:54:45.673Z Reads: 74

```
Your lipo set up looks really cool man. Are you still using the same setup? Any chance I can see your housing for the electronics? :grin:
```

---
## \#30 Posted by: AHS Posted at: 2016-10-18T18:03:35.058Z Reads: 72

```
Would really appreciate the help. Thanks to you guys I think I have a clear idea on what to and not to buy now. Will keep you posted if i need help with a Lipo setup. Too bad esk8 isn't a thing in my country yet, still have to bare in mind the shipping costs :confused:
```

---
## \#31 Posted by: IDVert3X Posted at: 2016-10-18T18:24:34.063Z Reads: 73

```
Trust me, space cell is not a good option for hill climbing board.
There is a reason why it has 40A fuse. And you don't want to draw more current through these cells.
If you want to go with Li-Ion, go with 6P or even better 8P ( gonna be huge ). Otherwise there is still a LiPo.
```

---
## \#32 Posted by: AHS Posted at: 2016-10-18T19:02:07.067Z Reads: 75

```
Thanks @IDVert3X. Been exploring some vendors. Should this be okay? Will it have significant difference from a 10s?

http://alienpowersystem.com/shop/alien-power-pack/alien-power-pack-8s-10000mah-25c-lipo/
```

---
## \#33 Posted by: IDVert3X Posted at: 2016-10-18T19:05:07.048Z Reads: 72

```
I don't know this product, but if the numbers are real, aka it's really a 25C pack ( 250A max ), it should be fine.
8S vs 10S? Not a big deal.
I'm personally going to stick with 8S as well. 190kv 16/36 97mm should give me ~ 40kmh^-1
```

---
## \#34 Posted by: AHS Posted at: 2016-10-18T19:14:56.958Z Reads: 75

```
Those are some big wheels you got there bro. Haha. How much would you limit your power on your vesc? And how about heating? Will this cause the motor to heat up a lot?
```

---
## \#35 Posted by: IDVert3X Posted at: 2016-10-18T19:21:01.218Z Reads: 74

```
Roads are terrible where I live, pavements are sometimes even worse...
I would use 107mm flywheels if they were available at a reasonable price.
I'm going dual motor and because I live in really hilly area, I'm going to limit each VESC to 40A.
If you do the math, it's ~ 1200W per motor for total power of 2400W or ~ 3hp.
Probably never gonna use that much power as I'm pretty light person, but why not.
VESC can handle it, motor can handle it, batteries can handle it, no reason to limit it.

And about heating? 
I don't think this is going to be an issue with dual-motor even on really steep hills.
Same goes for the VESC.
```

---
## \#36 Posted by: AHS Posted at: 2016-10-18T19:31:46.792Z Reads: 72

```
How bout a single motor? Because I don't want to go dual just yet due to lack of budget and just to gather more experience and knowledge first before spending even more. I know it won't work as efficient as a dual-motor. But just to get an idea of its limitations. And what settings would you propose for a single motor?
```

---
## \#37 Posted by: IDVert3X Posted at: 2016-10-18T19:34:47.673Z Reads: 72

```
Single motor for hill climbing?
Geez, that will overheat on longer hills man...

But for a single motor drive, 149kv 6374 motor, 15/36 and something like 83mm wheels should be fine.
Won't be super-fast, but should have enough torque to get you up a hill, probably not for very long time tho.
```

---
## \#38 Posted by: AHS Posted at: 2016-10-18T19:46:01.944Z Reads: 73

```
I would just limit to recreational use then, nothing to extreme for now. 😂 So a space cell wouldn't be such bad idea after all. Haha. But seeing the lipo I found with quite a reasonable price, I think I would invest on that and slowly build towards a dual drive in the future. It would be easier with that kind of battery don't you think? Plus, I could hit certain hills occasionally too.
```

---
## \#39 Posted by: IDVert3X Posted at: 2016-10-18T19:50:05.465Z Reads: 72

```
Well, if you won't climb a lot of long/steep hills, Space cell is fine. One motor should be fine then as well.
But if you want to upgrade it later for an awesome hill-climbing ability, buy a LiPo.
```

---
## \#40 Posted by: AHS Posted at: 2016-10-18T19:51:37.866Z Reads: 72

```
Got it man! Thanks for the flood on intel! Appreciate it.
```

---
## \#41 Posted by: IDVert3X Posted at: 2016-10-18T19:52:16.062Z Reads: 71

```
Np, glad I helped!
```

---
## \#42 Posted by: Namasaki Posted at: 2016-10-18T20:05:35.637Z Reads: 76

```
[quote="AHS, post:29, topic:11247, full:true"]
Your lipo set up looks really cool man. Are you still using the same setup? Any chance I can see your housing for the electronics?
[/quote]

Yes, currently using this setup. 
Enclosure by @psychotiller
<img src="/uploads/db1493/original/3X/2/e/2e674975e9930ea8c27d6de82070334c3f93743d.JPG" width="374" height="500">
<img src="/uploads/db1493/original/3X/c/9/c9ead3e1526aea42fbc529980dd1dd8ca3ea47f9.JPG" width="375" height="500">
```

---
## \#43 Posted by: 6gtht6 Posted at: 2018-03-11T06:39:55.537Z Reads: 31

```
Hows ur skateboard build so far?
```

---

# First Build &#124; Loaded Vanguard Deck &#124; 1 Turnigy SK3 6374 192kv &#124; 12S3P Samsung 25r &#124; Vesc-X

### Replies: 77 Views: 6429

## \#1 Posted by: ZachNYC Posted at: 2016-12-06T03:50:56.064Z Reads: 484

```
Hi all, this is my first build and I was wondering what you think and what suggestions you have.

These are the parts that I have/ that are shipping:

Deck: Loaded Vanguard
Trucks: Caliber II
Wheels: 97mm ABEC 11
I bought these 3 from a shop in NY by the name of Uncle Funky's
Motor: [Turnigy SK3 6374 192kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html)
ESC: [VESC-X](http://www.enertionboards.com/electric-skateboard-parts/vesc-x-motor-controller/)
Battery: [36 Samsung 25r cells that I will be connecting in 6S6P](http://www.ebay.com/itm/252644359533)
Remote: Wiiciever from @vitormhenrique
Pulleys and Belt: [36T ABEC Pulley Combo Kit](diy-electric-skateboard-kits-parts/36t-abec-drive-pulley-belt-combo-kit/)
Motor Mount: From @korryh
Charger: ?? I did order a BMS but it isn't coming for over a month (I only saw after I ordered) so I might just not use it. My plan is to be able to take the battery on planes, so I think I will make 2X 2S6P batteries and 2X 1S6P batteries and possibly connect them through XT-60 connectors, but I would like to be able to charge without opening my board at all, does anybody know how I could do this? Also, correct me if I am wrong, but you are allowed to have 2 batteries over 100Wh and as many as you want under that right? If not, how could I make the battery so that I could take it on planes?
```

---
## \#2 Posted by: ThieryB Posted at: 2016-12-06T08:27:59.049Z Reads: 423

```
I would suggest a 12s3p so you can have speed. Otherwise you should be just fine.
```

---
## \#3 Posted by: ZachNYC Posted at: 2016-12-06T12:17:27.594Z Reads: 409

```
Wouldn't my range be cut in half then?
```

---
## \#4 Posted by: ToMiCcc Posted at: 2016-12-06T12:38:50.290Z Reads: 399

```
Nop.. Your total stored energy will give you range.. So volts x amp = total energy... 12s3p is the same as 6s6p... You need same number of cells so its same stored eneregy.. But yet 12s gives u more volts = more rpm on the motor = more speed = less heat due to lower current drawn...
```

---
## \#5 Posted by: ZachNYC Posted at: 2016-12-06T13:02:46.668Z Reads: 389

```
So then would there be any advantages to 6S6P over 12S3P? Also, I can program the vesc to limit the speed right? Because I used a calculator and it had me going at 40mph with a 12s battery.
```

---
## \#6 Posted by: ToMiCcc Posted at: 2016-12-06T13:08:13.902Z Reads: 374

```
There are no adventages of 6p6s...  U can limit the speed with pulleys and gear ratio...
```

---
## \#7 Posted by: ZachNYC Posted at: 2016-12-06T13:49:28.161Z Reads: 365

```
12S it is, thanks!
```

---
## \#8 Posted by: TheImmortalJew Posted at: 2016-12-06T15:01:14.297Z Reads: 372

```
There is actually one advantage to 6S6P....easier charging. You could forego the BMS and balance charge with any 6S balance charger (iMax, Accucel, etc). You can do this in 12S3P too, you just have to wire it more cleverly. 

And yes the range should be near identical between the two. I have a 12S3P LG HG2 pack and do 12-15 miles if I'm not riding crazy fast.
```

---
## \#9 Posted by: ZachNYC Posted at: 2016-12-07T02:03:16.934Z Reads: 353

```
How are you charging the battery at 12S, and is there any way that I could still (I didn't have it completely worked out yetfor 6s anyway, as I didn't have a solution for charging) make it so that I could take it apart to go on planes?
```

---
## \#10 Posted by: saul Posted at: 2016-12-07T02:07:27.423Z Reads: 343

```
if you're going 12s then 192kv will be too high, i dont think vescx solved the 60k+ erpm issue.

for easy charging I would just get a custom pack from @barajabali with a bms and brick charger.
```

---
## \#11 Posted by: ZachNYC Posted at: 2016-12-07T02:08:45.570Z Reads: 335

```
I already have the cells though and I spoke to @barajabali and was told I that I couldn't send cells in to have a battery made for me.
```

---
## \#12 Posted by: saul Posted at: 2016-12-07T02:12:44.733Z Reads: 329

```
yea not worth it to ship them in circles, maybe he can at least help you with a bms and charger to use.
```

---
## \#13 Posted by: ZachNYC Posted at: 2016-12-07T02:15:45.236Z Reads: 322

```
Definitely worth a shot, @barajabali any ideas on what I could use?
```

---
## \#14 Posted by: barajabali Posted at: 2016-12-07T02:19:29.791Z Reads: 323

```
[quote="ZachNYC, post:11, topic:14242"]
and was told I that I couldn't send cells in to have a battery made for me.
[/quote]

yea only for samsung 25R's since I have them in stock, any other cell is fair game send them in. 

the BMS and charger i would just recommend batterysupports.com
```

---
## \#15 Posted by: ZachNYC Posted at: 2016-12-07T02:27:47.177Z Reads: 332

```
Would this charger work: http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html ?
Also, because I want to be able to take it apart into smaller "packs", I don't think I'm going to use a BMS.
```

---
## \#16 Posted by: barajabali Posted at: 2016-12-07T02:29:21.272Z Reads: 336

```
yea that will work for a 12s battery but it will charge your pack super fast and shipping is pretty expensive for that brick ( i use those)
```

---
## \#17 Posted by: ZachNYC Posted at: 2016-12-07T02:55:56.887Z Reads: 337

```
I think I will buy it then, do you have any idea of how i could make it so that the batteries could be disconnected and reconnected to make the 12s3p battery, but then disconnect to make 3 12s1p batteries?
```

---
## \#18 Posted by: barajabali Posted at: 2016-12-07T03:03:38.831Z Reads: 327

```
Yes I do know how. But you won't break it up into 3 12s1p packs. You would break it into 3 4s3p packs
```

---
## \#19 Posted by: Jebe Posted at: 2016-12-07T04:06:36.342Z Reads: 324

```
at least 10s. Love the vanguard decks. look forward to watching you build
```

---
## \#20 Posted by: ZachNYC Posted at: 2016-12-07T05:20:45.621Z Reads: 319

```
@barajabali I'm intrigued, how would that work?
```

---
## \#21 Posted by: ZachNYC Posted at: 2016-12-07T05:23:05.227Z Reads: 284

```
@Jebe thanks!
```

---
## \#22 Posted by: barajabali Posted at: 2016-12-07T05:37:25.892Z Reads: 285

```
It gets more complex when you want to use a bms but that just means you need more plugs. 

Will you be using a bms or no? that matters on how the pack will be split up
```

---
## \#23 Posted by: ZachNYC Posted at: 2016-12-07T05:57:16.142Z Reads: 277

```
if it works and is chargeable without a bms, then no.
```

---
## \#24 Posted by: Tuomalar Posted at: 2016-12-07T06:20:10.015Z Reads: 283

```
I don't see any problem with or without bms, but why you want charge it like this?
```

---
## \#25 Posted by: ZachNYC Posted at: 2016-12-07T12:51:50.519Z Reads: 278

```
It's easier and more convenient.
```

---
## \#26 Posted by: TheImmortalJew Posted at: 2016-12-07T13:35:09.250Z Reads: 282

```
You could also break it into two 6S3P packs. That would give you 21.6V * 7.5Ah = 162 WH which is just over the 160WH limit some airlines have. Run the two packs in series for 12S when riding (discharge), and separate them to charge at 6S. That's how mine is setup, I charge with 2 iMax B6 chargers.
```

---
## \#27 Posted by: Tuomalar Posted at: 2016-12-07T14:08:29.573Z Reads: 273

```
In my opinion it's way more easier to charge one battery rather than three. But if you want take batteries in the airplane or you just don't care about clean look and usability I'll get that.
```

---
## \#28 Posted by: ZachNYC Posted at: 2016-12-07T20:08:14.155Z Reads: 274

```
@TheImmortalJew have you tried this at an airport? If so, did they let you go? 

@Tuomalar I care about all three, and maybe the look of the battery itself will be worse, but in an enclosure it won't make a difference, and I think it would be very easy to use and possibly make for easier charging, but as long as I can take it on a plane it's fine.
```

---
## \#29 Posted by: nmagz3 Posted at: 2016-12-07T20:47:18.302Z Reads: 258

```
Those 97mm wheels on the Vanguard are gunna look dope!  I'm also working on my fist build as wel.  However my expirience with Lipos is more familiar so I went that route.  Good luck and look forward to the completed project 🤘🏽
```

---
## \#30 Posted by: ZachNYC Posted at: 2016-12-07T21:39:59.794Z Reads: 260

```
I already have the board, I'll send pictures when I get home, it looks awesome.
```

---
## \#31 Posted by: ZachNYC Posted at: 2016-12-07T22:11:47.372Z Reads: 284

```
<img src="/uploads/db1493/original/3X/8/6/8601917e270c9b8d0ebacb6669e041c3665d1de8.PNG" width="281" height="500"> just used a calculator and this is what I got. 😱😱
```

---
## \#33 Posted by: nmagz3 Posted at: 2016-12-07T23:40:35.950Z Reads: 250

```
HAHAHA That's nuts man. Hope you have insurance :innocent:
```

---
## \#34 Posted by: Kaly Posted at: 2016-12-08T02:49:30.090Z Reads: 270

```
this number are right check my build
http://www.electric-skateboard.builders/t/emtb-and-vanguard-built/995/25?u=kaly

if you are having issue with the battery let me know i can help i am in the BX
```

---
## \#35 Posted by: ZachNYC Posted at: 2016-12-08T03:27:45.097Z Reads: 280

```
Loved both builds and the idea of easily being able to switch from 6s to 12s. For the battery, to get it to be to fit airline regulations, 6s3p would be to large, Coreect me if I am wrong, but I could just do it like this and charge at 12s right?
<img src="/uploads/db1493/original/3X/b/9/b9058101a76c69e5375b90d023cb168dc3bb232b.JPG" width="375" height="500">
```

---
## \#37 Posted by: Kaly Posted at: 2016-12-08T16:37:48.788Z Reads: 253

```
You can do it like that, it will be annoying to open up the enclosure every time you'll need to charge but will have the option to air travel.
```

---
## \#38 Posted by: Tuomalar Posted at: 2016-12-08T16:43:12.971Z Reads: 255

```
Or you can make few charginport. There's 3 ports in my board. Two for chargin batteries (2x3s) and for one loopkey which connect batteries to esc.
```

---
## \#39 Posted by: Kaly Posted at: 2016-12-08T17:08:45.252Z Reads: 258

```
That sounds good 
Can you share a picture of this ?
```

---
## \#40 Posted by: ZachNYC Posted at: 2016-12-08T23:00:42.710Z Reads: 273

```
Sounds awesome, would love to see some photos 😛😛
```

---
## \#41 Posted by: Tuomalar Posted at: 2016-12-10T15:42:50.010Z Reads: 282

```
Left one is for loopkey and two right ones for charging. Would be awesome if someone here could 3D print this kind of mount for xt90. There is one already in thingverse.

<img src="/uploads/db1493/original/3X/0/6/0677049215a909bc98c2ac31647408538a775093.JPG" width="375" height="500">
```

---
## \#42 Posted by: ZachNYC Posted at: 2016-12-14T13:40:05.013Z Reads: 266

```
Sorry for responding so late, but I think I am going to do 3 4s3p batteries connected by xt60 series connectors, each with its own charging port. I want to just do one fast charger and I will charge each individually, which if I am correct should take an hour, right?
```

---
## \#43 Posted by: Tuomalar Posted at: 2016-12-14T16:33:02.991Z Reads: 240

```
Hard to say how long it take, because charging time depend on your charger and battery's capacity.
```

---
## \#45 Posted by: ZachNYC Posted at: 2016-12-19T05:38:08.691Z Reads: 233

```
Would this charger work?  I don't see why not, and correct me if I'm wrong, but this could be adjusted to have the same charging stats as the fast charger on batterysupports.com.  https://hobbyking.com/en_us/turnigy-reaktor-250w-10a-1-6s-balance-charger.html
```

---
## \#46 Posted by: Tuomalar Posted at: 2016-12-19T06:32:51.501Z Reads: 225

```
Yes, this is fine, if you adjust it correctly. But you need also power supply.
```

---
## \#48 Posted by: ZachNYC Posted at: 2016-12-21T03:12:16.431Z Reads: 218

```
Could I use xt60s for the charging ports and just change the charger to an xt60 as well?
```

---
## \#49 Posted by: Tuomalar Posted at: 2016-12-21T06:34:24.384Z Reads: 219

```
Sure. Just use these for example: https://hobbyking.com/en_us/xt60-charged-discharged-battery-indicator-caps-5-pairs.html
```

---
## \#50 Posted by: ZachNYC Posted at: 2016-12-29T06:47:39.987Z Reads: 216

```
I'm still searching for a cheaper charger that comes with everything, which is the best one of these (or any others) that could do charge a 4s3p pack in under an hour?
 http://alienpowersystem.com/product-category/chargers-power-supply/imax-rc/
```

---
## \#51 Posted by: PXSS Posted at: 2016-12-29T13:09:59.047Z Reads: 235

```
Why do you want to split the pack? Is it so you can take it on flights? Or simply for the charging?

If you want to take it on an airplane, you need to split your pack in at least 4. Reason is a 12s3p pack of samsung 25r has 324Wh of energy, airlines allow a maximum of 2 batteries between 100wh and 160wh. If you split your pack in 2 you'd have 2 packs of 162wh and you'd be at the mercy of the person behind the counter or tsa agent. If you split it in 3, you have 108wh packs which are still just over the limit. Now the kick is that you can take as many batteries under 100wh as you want, so if you split it in 4, now you have 81Wh packs which are not limited at all. 

If you want to simplify charging get a bms and a 42v charger. It really doesn't get any simpler. Both will run you about $70. 

If you want to charge them with an rc charger:
You need a power supply and a 12s rc charger. Rc chargers for 12s run above $100, so it is cheaper to get 2 6s chargers a dual 6s charger or make a wire harness to be able to charge them in parallel with one 6s charger. 

You cannot have the cells connected in series while charging if they share the same charger as you will blow something up. Trust me, I've done that...

I personally went with the BMS as going the rc route only saves a few bucks and over complicates things

I got my bms from batterysupplies and a 42v5A charger from alibaba.
```

---
## \#52 Posted by: mmaner Posted at: 2016-12-29T14:17:57.094Z Reads: 216

```
[quote="ToMiCcc, post:6, topic:14242"]
There are no adventages of 6p6s
[/quote]

Chargers for 6s are cheaper...
```

---
## \#53 Posted by: ZachNYC Posted at: 2016-12-29T16:12:23.742Z Reads: 231

```
I want to split the packs for airplanes. Even though it is over 99wh, the 3 108wh batteries would be fine as I rarely travel alone, in which case I can leave one behind. I wouldn't mind doing the 4 batteries though and being able to take it on a plane. Either way though, how would you suggest I charge it? I wouldn't be happy, but I would be fine with having to separate the batteries for charging. What do you think about having a bms for each pack and charging through there, would that work while connected in series? Also, I could do alibaba for the charger, but I haven't had a great experience with buying from them as everything takes forever to ship, and I've had two things I've ordered not arrive. That was completely different stuff though, so if you had a good experience with them, I'll give it another shot. Thanks, Zach
```

---
## \#54 Posted by: PXSS Posted at: 2016-12-29T19:38:08.393Z Reads: 245

```
I would separate the packs for charging. I'm not sure if you can charge them while they're connected in series but I'm no electrical engineer. I would have a harness made to connect the packs in parallel and charge them that way as it probably is the least expensive.

You could have 4 bms and have 4 loop keys to disconnect the series packs to charge them. That way you could also just remove the loop keys and now you have 4 individual packs without having to open up the board too for traveling. 

The way I would do this is

Master loop key on the most positive terminal between battery and load. Loop key between batteries 1 and 2, 2 and 3, and 3 and 4. You can connect them in any order as long as the master is always last to connect and first to disconnect. Disconnected you have 4 packs you can charge individually and are under 100wh and connected you have a single 12s3p pack.
```

---
## \#55 Posted by: ZachNYC Posted at: 2016-12-30T03:34:11.864Z Reads: 223

```
So I did some reading, and from what I am understanding, it is possible, but not recommended. I would definitely do a harness, but feel like I would mess it up somehow, although I do like the idea of the loop keys but that would get really messy/crowded in my enclosure (if I kept it in the enclosure). If I didn't have it inside the enclosure, there would be too much on the outside of the enclosure. 

Also, do I need a bms/bms's if I buy a balance charger that will stop charging when full? If the charging port is before the series connector, isn't it charging separately and not in series?
```

---
## \#56 Posted by: PXSS Posted at: 2016-12-30T05:07:34.121Z Reads: 208

```
The loop keys would definitely have to be within an enclosure. It would be a big wire mess otherwise. 

You do not need a BMS if you're using a balanced charger, problem is that there are no 10S chargers on the cheap side. The issue with charging separately while still connected in series is that now you have several grounds at different voltages and if the chargers/power supply are not designed to be protected against this, you will smoke them. I've ruined a $400 charger by charging two batteries that shared a ground as two separate packs.

Again, this is all from personal experience and not really technical knowledge as I'm not an electrical engineer.
```

---
## \#57 Posted by: ZachNYC Posted at: 2016-12-30T05:49:05.400Z Reads: 203

```
That's fine then, I'd be willing to open the enclosure, disconnect, and charge separately. Do you have any dual balancing chargers that could charge a 3S3P battery in 3-45 minutes that you would recommend? This to me looks like the least complicated/easiest airplane possible battery to me. Would you suggest you loop key method over series connectors?
```

---
## \#58 Posted by: PXSS Posted at: 2016-12-30T06:42:36.444Z Reads: 212

```
The loop key method allows you to charge without having to open the enclosure, same thing with travel, just take them out and you're good to go. As long as you have enough space for them...

As far as chargers... I use iChargers almost exclusively but do have friends that have reaktor and b6 chargers from hobbyking. 

FYI, you should not charge 25rs in less than an hour. Max charge rate is ~1hour, standard charging is ~2 hours per the spec sheet. 

So with that in mind you need a 400W power supply and a a dual 6s charger or 2 dual 3s chargers.
Hobbyking also has some chargers that have power supplies included, they usually dont have as high wattage though. I would shop around there if I were you. 

Now if you want a really good charger check any of the icharger duos (you need a separate power supply). I charge at a whooping 800W on some of my rc airplanes.
```

---
## \#59 Posted by: ZachNYC Posted at: 2016-12-30T18:36:15.539Z Reads: 196

```
I see what you're saying with the loop keys, and that is genius. As for chargers, I was looking through hobbyking and found this, https://hobbyking.com/en_us/hobbykingtm-quattro-4x6s-lithium-polymer-multi-charger.html which I think would be good because I don't need to worry about switching the battery that is charging when one finishes. Would I still need to buy a power source though? It looks like there is one attached.
```

---
## \#60 Posted by: PXSS Posted at: 2016-12-30T21:26:28.548Z Reads: 201

```
You definitely need a power supply with that charger. 
Look at the ones in the AC/DC section for ones that do not need power supplies, they usually only have ine channel. 

The power supplies are pretty expensive at hobbyking from what I'm seeing. I would get a 350W or 400W one from progressiveRC. They run about $50-70

And you can either run several small chargers in parallel or the one you posted.

E: heres one from hobbyking to match that charger. 
https://hobbyking.com/en_us/turnigy-reaktor-pro-350w-23a-power-supply-100-240v-ac.html
```

---
## \#61 Posted by: ZachNYC Posted at: 2016-12-30T22:19:18.373Z Reads: 190

```
That power source with the charger would be too expensive, I think I'll just do multiple of these, https://hobbyking.com/en_us/imax-b6-ac-dc-charger-5a-50w-with-us-plug-copy.html or the real ones if the it's worth the extra money.
```

---
## \#62 Posted by: PXSS Posted at: 2016-12-31T01:02:33.339Z Reads: 192

```
That looks good. Just beware of the 50W charging limit. If you buy 4, you are looking at charging roughly in an hour and a half
```

---
## \#63 Posted by: ZachNYC Posted at: 2016-12-31T01:24:45.976Z Reads: 197

```
Sounds good! I'll order tonight.
```

---
## \#64 Posted by: wmj259 Posted at: 2016-12-31T01:30:25.510Z Reads: 201

```
Maybe a stupid question,  but is it required to use a power supply to run the charger? Why not plug like landline phone power cord to it?
```

---
## \#65 Posted by: PXSS Posted at: 2016-12-31T03:09:36.859Z Reads: 180

```
Depending on the charger, you need between 12v-24v dc.
If you plug it straight to the wall (110v ac) you will see the magic smoke that makes electric things work leak.
```

---
## \#66 Posted by: wmj259 Posted at: 2016-12-31T03:12:22.851Z Reads: 169

```
So basically any box that can downstep 110-120V to the input Voltage of the charger.
```

---
## \#67 Posted by: PXSS Posted at: 2016-12-31T03:14:16.643Z Reads: 181

```
that plus convert ac to dc, and have enough wattage for the charger
```

---
## \#68 Posted by: ZachNYC Posted at: 2016-12-31T05:04:05.186Z Reads: 191

```
Before buying, I stopped and read through this thread quickly, and realized that in thinking of buying four chargers, I forgot my main goal, to make this airplane/travel possible, and searched some more and found this, which I'm pretty sure I will get as it isn't too big, and is a dual charger. http://m.rcmoment.com/battery-charger-accessories-2128/p-rm2995uk.html?currency=USD&lang=en&aid=rmsmplaus1&gclid=CMDsz4zTndECFUlNfgod62EBuA
```

---
## \#69 Posted by: PXSS Posted at: 2016-12-31T06:58:44.489Z Reads: 187

```
That only gives you 100W total charging power. Not enough in my opinion.
This one?
http://www.banggood.com/Ultra-Power-UP240AC-DUO-240W-LiPo-LiFe-NiMH-Battery-Dual-Balance-Charger-Discharger-p-1094621.html?rmmds=search
```

---
## \#70 Posted by: eblade Posted at: 2017-01-02T04:29:19.764Z Reads: 198

```
Just wanna clarify, if I have 4 3s packs (making it 12s) connected in series with serial connectors.

Can I have 2 3s packs connected in series and charge as 6s on a 6s charger. Or,
4 3s packs connected in series and charge as 12s on a 12s charger.

So it'll be like 2 charger, each charging 2 3s packs and connect them back together to the ESC when I wanna use them.
I guess I would get off cheaper with 2 6s charger maybe?
```

---
## \#71 Posted by: PXSS Posted at: 2017-01-02T05:49:55.616Z Reads: 190

```
You can do 2 6s chargers. Or one of the ones from above that can charge several 6s/3s packs at once
```

---
## \#72 Posted by: willpark16 Posted at: 2017-04-16T07:26:22.748Z Reads: 151

```
Any updates?
```

---
## \#73 Posted by: ZachNYC Posted at: 2017-04-16T18:26:35.609Z Reads: 147

```
Nearly done, I will update photos and videos later today. Only problem is I don't know what best settings to use. I'm probably 110lbs and want the tips speed to be 25mph.
```

---
## \#74 Posted by: ZachNYC Posted at: 2017-04-17T04:48:42.847Z Reads: 140

```
Forgot to take them, but I will upload later today.
```

---
## \#75 Posted by: Eboosted Posted at: 2017-04-17T05:34:07.827Z Reads: 153

```
I don't know if you've seen this, but it might an easier idea for your Vanguard build.

https://www.electric-skateboard.builders/t/travel-safe-battery-design-v2-10s4p-360whr-for-loaded-vanguard/19535
```

---
## \#76 Posted by: ZachNYC Posted at: 2017-04-18T05:06:08.256Z Reads: 157

```
Xt60 loop keys came out great, covered them with sugru. That stuff is amazing. After a long time I got the 10AWG wire into the xt60 for the battery connection. The kydex came out great. I have a lot more, will upload tomorrow. 


<img src="/uploads/db1493/original/3X/7/0/70195bff384e510482f806648b38350204a0adc1.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/a/faef6740deb5283fbdc1a5fd06c83743d4f62397.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/8/1/810b23c1228f7adb95eca0d5cb2d18a5f63169fc.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/5/159b98417387ed96974919172d28c70a27f590af.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/a/7/a73c502c8981f56ec94ce6384a8b0b85d9dc416b.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/3/a33edd24f713396269ab5b75f758fcd2ea01775d.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/f/3f9ac6f303aefb10c0d59335c0c69b4a0b48af9e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/f/6f9e5fcba7f370987801da5dea5d82a26e4cd45d.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/3/93075dc222e312fba8212c587e4a552db83fbaeb.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/7/d79c28f87d0d88eb9336bca7eadbf9056a261183.JPG" width="375" height="500">
```

---
## \#77 Posted by: Maxid Posted at: 2017-04-18T08:23:22.901Z Reads: 141

```
that is very poor soldering on the XT60 connector. The solder looks like to be only applied on the surface - it needs to go all the way through the exposed wire in order to make a good connection. Your joint will fail eventually or/and have high losses (=heat). I recommend redoing that.

that's how it should look (from @whitepony's spud build):
http://www.alternative-4.com/DIY/spud_freeboard_52.jpg

Edit: the red wire actually appears to be broken
```

---
## \#78 Posted by: ZachNYC Posted at: 2017-04-20T02:33:50.359Z Reads: 125

```
Which has red wire?
```

---
## \#79 Posted by: monkey32 Posted at: 2017-04-20T09:10:20.098Z Reads: 117

```
Ugly soldering man...pretty dangerous. The red lead you have in those pictures- Not broken just ugly connection. You need to heat the wires up so you solder "flows" into the strands. Also as they are now be careful because if those pieces of soldered red and black wires touch you will short your circuit. These connections move and friction esspecially on sharp crappy joints, like those in your photos,  wear thru
```

---
## \#80 Posted by: Tuomalar Posted at: 2017-04-20T09:53:13.522Z Reads: 120

```
First solder one and shrink tube it then solder second one and put shrink tube. 

You probably need more powerful solder iron to make solder flow properly.
```

---
## \#81 Posted by: Maxid Posted at: 2017-04-20T10:09:51.680Z Reads: 122

```
[quote="monkey32, post:79, topic:14242, full:true"]
Not broken just ugly connection.
[/quote]
 I am not so sure - isn't this looking like the wood is shining through?
<img src="/uploads/db1493/original/3X/6/0/6002a645929fab5dd0982434bc1e80727c6f7a2b.JPG" width="528" height="500">
```

---

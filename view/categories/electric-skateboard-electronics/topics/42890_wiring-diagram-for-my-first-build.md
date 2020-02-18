# Wiring diagram - For my first build

### Replies: 38 Views: 3520

## \#1 Posted by: Flaco Posted at: 2018-01-05T21:41:02.439Z Reads: 326

```
Hi to everyone, so after reading and researching I came with a diagram for my first build. It will be a 12s4p 30q dual focbox bms for charging and discharging and a e-switch.
Any suggestions advices corrections comments will be appreciated.
So this is it:
<img src="/uploads/db1493/original/3X/1/1/119c1e3610fc3f6d104a0cee327973a6d5773a6a.jpg" width="690" height="470">

If I want to use a fuse, where it should go?

P.S: The battery diagram and balance wires will be another chapter.
```

---
## \#2 Posted by: Sebike Posted at: 2018-01-05T21:44:22.584Z Reads: 293

```
Nice diagram. Fuse should run in series with the anti spark plug.

Edit - Or rather on the positive lead coming off the battery before anti spark, so that it protects from a short even on the charge plug.
```

---
## \#3 Posted by: Genghis_Kuan Posted at: 2018-01-05T21:54:50.843Z Reads: 290

```
Nice man, Im doing the same except with a Supower BMS no e-switch (Antispark Loopkey is my switch). I would also suggest cell level fusing over the series fuse (Just cause thats what im doing on mine).
```

---
## \#4 Posted by: mmaner Posted at: 2018-01-05T22:19:45.167Z Reads: 274

```
You will most likely want the HM-10 bluetooth module on the same VESC (the Primary VESC) as the RX).  If you dont have one PM @GrecoMan, he makes and sells them cheap.  

@Sebike is right.  If you are going to use a XT90s loop key, you want it after the battery but before anything else.  If you have a BMS with an E-Switch its unnecessary.
```

---
## \#5 Posted by: b264 Posted at: 2018-01-05T22:23:53.766Z Reads: 258

```
You've got this wired like it'll run in bypass but then also wired in discharge mode.  You typically want one or the other.

You want either
A) bypass mode
- you need a loop key
- don't run the esc power through the BMS at all
- no power switch needed

B) discharge mode
- you need a power switch
- run the esc power through the BMS (P-)
- no loop key needed

Make sure you understand the pros and cons of each method
```

---
## \#6 Posted by: Sebike Posted at: 2018-01-05T22:34:29.925Z Reads: 238

```
I'm not sure I'm following here... The diagram looks like charge+discharge and is how it should be set up if discharging through BMS. It's either charge only or charge+discharge. At least I haven't seen anyone going discharge only and then charging pack without balance charging..?

Only thing that is not necessary is e-switch, since a loop key is being used.
```

---
## \#7 Posted by: mmaner Posted at: 2018-01-05T22:35:14.596Z Reads: 226

```
[quote="b264, post:5, topic:42890"]
You've got this wired like it'll run in bypass but then also wired in discharge mode
[/quote]

This confused me.  From the image I see the Battery negative connected to the BMS at B- and the BMS negative connected to the VESC' at P- and the charge port negative connected to the BMS at C-.  The E-switch should kill the negative flow of current when in the off position thereby isolating the battery from electronics down the chain.  That's textbook discharge mode right?
```

---
## \#8 Posted by: b264 Posted at: 2018-01-05T22:35:57.687Z Reads: 222

```
pros of running bypassed:

- smaller BMS requirements (charging/balancing only)
- brakes won't cut out if the battery is completely full
- can be safer for humans, at the expense of possibly damaging batteries or electronics
- BMS discharge current rating is irrelevant

pros of running through BMS discharge circuit:

- will shut down if any P group runs down quicker
- safer for electronics

cons of bypass:

- if a parallel cell group gets weak it can get damaged
- you can hit the brakes until your battery is destroyed, if you wanted to and had a big enough hill and had a completely full battery
- need to carry a key for your skateboard and not lose it

cons of discharge:

- you need a BMS rated at >= 50A (one motor) or >= 80A (two motors)
- if you start braking on a full battery it can shut down, killing your braking ability
- more expensive BMS
- bigger BMS
```

---
## \#9 Posted by: b264 Posted at: 2018-01-05T22:36:23.178Z Reads: 198

```
[quote="mmaner, post:7, topic:42890"]
That's textbook discharge mode right?
[/quote]

yes, except with an extra loop key
```

---
## \#10 Posted by: mmaner Posted at: 2018-01-05T22:38:56.175Z Reads: 200

```
[quote="b264, post:9, topic:42890"]
yes, except with an extra loop key
[/quote]

Ahhhhh, I thought you meant the BMS was wired in discharge.  I assume he just wants extra protection by using the XT90s loop key.  Seems needless to me with a quality BMS, but I can understand wanting to protect a few hundred bucks worth of electronics :slight_smile:
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-01-05T22:40:29.669Z Reads: 199

```
looks like eswitch is permanently connected then loop key is master switch. this is exactly how I've got mine wired up right now, same bms and all that. 

only thing, I stopped using xt90s because they're bulky. and once wires are soldered up they're pretty long/tall. and doing the split to dual focbox as in the diagram, you'll be surprised how bulky that loom becomes. I've switched mostly to bullet connectors.
```

---
## \#12 Posted by: b264 Posted at: 2018-01-05T22:41:15.772Z Reads: 202

```
[quote="mmaner, post:10, topic:42890"]
but I can understand wanting to protect a few hundred bucks worth of electronics
[/quote]

I'd prefer to protect the human at all costs, even if it means overcharging the battery while braking hard.  But there are many pros and cons to sort through, all depending on your preferance.  I also like the BMS being physically smaller and not needing heatsinks on it.
```

---
## \#13 Posted by: Flaco Posted at: 2018-01-05T22:41:35.076Z Reads: 196

```
I've put the loop key for extra protection, not sure why
So I moved the bluetooth to the main vesc, put a fuse and removed the loop key

<img src="/uploads/db1493/original/3X/0/a/0addfeeb8e03e51218bf4004ffbb2031a6457a9c.jpg" width="690" height="470">

Now what do you think?
```

---
## \#14 Posted by: Sebike Posted at: 2018-01-05T22:41:47.376Z Reads: 186

```
[quote="b264, post:5, topic:42890"]
B) discharge mode
- you need a power switch
[/quote]


Why would you need a power switch in discharge mode? You mean, in discharge mode you can either use a BMS e-switch or a loop key?
```

---
## \#15 Posted by: Sebike Posted at: 2018-01-05T22:43:13.868Z Reads: 180

```
TBH I think dont use e-switch and use loop key :joy:
```

---
## \#16 Posted by: b264 Posted at: 2018-01-05T22:43:58.704Z Reads: 179

```
[quote="Flaco, post:13, topic:42890"]
Now what do you think?
[/quote]

That's the textbook discharge mode circuit.

[quote="Sebike, post:14, topic:42890"]
Why would you need a power switch in discharge mode? You mean, in discharge mode you can either use a BMS e-switch or a loop key?
[/quote]

I meant the BMS e-switch or a separate antispark e-switch
```

---
## \#17 Posted by: mmaner Posted at: 2018-01-05T22:44:56.610Z Reads: 179

```
[quote="Flaco, post:13, topic:42890"]
put a fuse and removed the loop key
[/quote]

If you want the extra protection, use the loop key.  When a fuse blows you will eat pavement, at least most people do as it will most likely blow under a heavy load meaning fast.

This is how I wire mine, maybe it will simplify the concept a bit...
<img src="/uploads/db1493/original/3X/2/1/2150169f9a8b9f0a6196979bfe69ae02cf4897cf.png" width="409" height="499">
```

---
## \#18 Posted by: Sebike Posted at: 2018-01-05T22:46:34.824Z Reads: 170

```
But at the rate e-switches and separate power switches seems to be failing on peoples builds, and for the sake of better protection (like @mmaner already mentioned) I'd still vote for an XT90s ! :wink:
```

---
## \#19 Posted by: mmaner Posted at: 2018-01-05T22:47:54.385Z Reads: 171

```
I haven't noticed a failure in BMS E-switches, just Anti-Spark switches.  That being said, an XT90's loop key won't hurt anything.
```

---
## \#20 Posted by: b264 Posted at: 2018-01-05T22:48:20.502Z Reads: 177

```
[quote="Sebike, post:15, topic:42890, full:true"]
TBH I think dont use e-switch and use loop key
[/quote]

If you want to use a loop key instead of the eswitch, put the loop key on the BMS P- to XT90 run

[quote="thisguyhere, post:11, topic:42890"]
only thing, I stopped using xt90s because they're bulky. and once wires are soldered up they're pretty long/tall. and doing the split to dual focbox as in the diagram, you'll be surprised how bulky that loom becomes. I've switched mostly to bullet connectors.
[/quote]

Also, this.  Consider soldering them together too, instead of bullet connectors or the XT90/XT60/XT60 harness unless you have tons of space in your enclosure.  I wouldn't solder them together unless you use a loopkey though
```

---
## \#21 Posted by: b264 Posted at: 2018-01-05T22:49:04.311Z Reads: 163

```
[quote="mmaner, post:19, topic:42890"]
an XT90's loop key won't hurt anything.
[/quote]

I beg to differ.  If you're getting ready for work and you have your skateboard and remote but can't find the loopkey, it can most certainly hurt
```

---
## \#22 Posted by: Sebike Posted at: 2018-01-05T22:49:32.624Z Reads: 162

```
No? Maybe Ive got it mixed up with all the e-switches that are DOA then
```

---
## \#23 Posted by: mmaner Posted at: 2018-01-05T22:50:51.547Z Reads: 163

```
LOL, I guess it would.  But that's why I keep an extra at work and another extra in my backpack :).
```

---
## \#24 Posted by: Sebike Posted at: 2018-01-05T22:53:50.571Z Reads: 161

```
or when you have your loopkey but cant find your board ! :smile:
```

---
## \#25 Posted by: Flaco Posted at: 2018-01-05T23:17:57.656Z Reads: 163

```
So the fuse of how many amps it should be?
```

---
## \#26 Posted by: Sebike Posted at: 2018-01-05T23:25:49.795Z Reads: 167

```
There is no consensus on that here, but go through these threads for some thoughts and tips

https://www.electric-skateboard.builders/t/wiring-up-an-in-line-fuse/35304/5?u=sebike
```

---
## \#27 Posted by: Namasaki Posted at: 2018-01-06T03:17:49.445Z Reads: 164

```
[quote="Flaco, post:1, topic:42890"]
If I want to use a fuse, where it should go?
[/quote]


You really don't  need a fuse with that BMS. It has external short circuit protection that works very well.
```

---
## \#28 Posted by: Flaco Posted at: 2018-01-06T14:24:37.022Z Reads: 161

```
So I removed the fuse since it seems to not be necessary and bc it's hard to find a high amp fuse small enough.
I added a xt90 after the battery so it can be separated.

<img src="/uploads/db1493/original/3X/f/b/fb0791121ee6117835923c634d43b89729b1b135.jpg" width="690" height="466">
```

---
## \#29 Posted by: ArnhemAnt Posted at: 2018-01-27T07:00:56.761Z Reads: 155

```
Just gotta say - this thread is very helpful. I'm planning my first build and the wiring has me a little stumped. Reading through this thread has certainly made things easier to understand - thank you.
The Focbox thing still has me a little stumped, but I plan to read up on this over the next week while I wait for the parts to start arriving.

This forum rocks.
```

---
## \#30 Posted by: Flaco Posted at: 2018-01-27T18:15:43.159Z Reads: 152

```
Glad it's useful for you.
I was in your position like 2 months ago. I couldn't find it at the moment so I created expecting that.
```

---
## \#31 Posted by: adilism Posted at: 2018-03-21T12:28:16.603Z Reads: 140

```
Hi guys, a new builder here needs help. I ordered [this](https://ru.aliexpress.com/item/10S-60A-active-bms-2017-new-Li-ion-smart-bms-pcm-with-android-Bluetooth-app-UART/32827750823.html?spm=a2g0s.9042311.0.0.DBpvBC) for a 10s3p 30q battery pack. Will be using it in discharge mode. Can I use a power switch without anti-spark with it? The reason I'm asking is some BMS mention the power switch capability in specs, but I couldn't find the mentioning for this particular BMS. Maybe it's just a conventional wisdom that with BMS you don't need anti-spark? The BMS itself seems like a good quality product, hope it will serve me well.
```

---
## \#32 Posted by: krloz Posted at: 2018-03-21T13:31:37.497Z Reads: 136

```
[quote="adilism, post:31, topic:42890"]
. Can I use a power switch without anti-spark
[/quote]

Nope. You need an anti spark to solve the inrush when connecting caps to lithium power sources. The bms you link doesn't include this
```

---
## \#33 Posted by: adilism Posted at: 2018-03-21T17:03:30.389Z Reads: 129

```
[quote="krloz, post:32, topic:42890"]
Nope. You need an anti spark to solve the inrush when connecting caps to lithium power sources. The bms you link doesn’t include this
[/quote]

Thank you for the answer, although that's a bummer for such pricey BMS. One more question, can I hide it inside the enclosure, or it needs to be disconnected sometimes (e.g. for charging)?
```

---
## \#34 Posted by: krloz Posted at: 2018-03-21T19:47:11.655Z Reads: 118

```
I don't follow. What do you want to know ou'd it had to be disconnected when charging??
```

---
## \#35 Posted by: adilism Posted at: 2018-03-21T20:08:43.456Z Reads: 122

```
I want to keep the anti-spark in connected permanently and hide it under enclosure, so that I only use the power switch to turn the board on/off. Can I do it? I read somewhere, that the anti-spark needs to be disconnected when the board is charging, but not sure right now.
```

---
## \#36 Posted by: krloz Posted at: 2018-03-21T20:42:00.390Z Reads: 123

```
That is not a thing.  The only thing I can imagine you have found is somebody using an xt90s connector with built in antispark, both for connecting batteries to the esc suppressing sparks and for charging the battery. In your case you will have a bms wired to the battery.  A charge connector wired to the bms and the batteries also connected to the esc through the antispark switch. Which is a very very common setup so I'm sure there are diagrams around
```

---
## \#37 Posted by: GUAN1111 Posted at: 2019-04-12T19:45:13.971Z Reads: 39

```
Hi, I have built a electric longboard. I used it one summer but I wanted to upgrade. It was a hazel to unplug the battery's every time and plug them in to the balance charger.

Therefore I decided to add a BMS, 3 pin charge port and a small battery presenting indicator for easy use.. I decided to bypass BMS. I started with wiring the cables like the picture below, but forgot plug in the motor ore the balance wires to the battery's(I did not plug in the XT-90). When I plugged inn my charger the BMS became super hot(to hot to touch). I though it was because my battery balance leads were not plugged inn. Therefore I plugged in my balance leads and tried again. This time the 3 pin charge port and the charger welded together. Then I plugged in the XT-90 to complete the main circuit. This was a bad decision on my behalf, because the battery's started to expand, my cables and connecters started to smoke, and the VESC MOSFETs melted through the heat shrink. This lead to all my electronics getting destroyed. :-(

I believe the wiring is the problem. I did not have the motor plugged inn. Can this have an effect on what happened.

But can anyone just take a quick look at this whirring and tell me if it is right. Do I nead the black whier form battery 2 to B- on the BMS?

Thanks ;-)![Untitled|690x360](upload://t1tQssshfPQ0hdWRDT8g8PXx1yF.jpeg)
```

---
## \#38 Posted by: Jumpman Posted at: 2019-04-12T19:53:08.446Z Reads: 38

```
No, I don’t see why you would need to add the thin black wire to B-.  

Personally, I would double check the polarity of your charger, and your charge port.
```

---

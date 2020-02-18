# Charging questions! Battery questions! HELP!

### Replies: 26 Views: 2503

## \#1 Posted by: emstr Posted at: 2017-04-28T13:16:13.093Z Reads: 145

```
Hi eSk8 community! I'm really new to building a DIY board and I've picked a couple parts already, however I'm not sure if everything will work as I expect. I need this board to ride to school which is 10km(6.2mi) away and back 20km (13mi) I'm not concerned with speed but I'd like the board to go at least 15mph. I live in a pretty hilly place so I'd like torque to be good, I weight 70kg (150lbs.)

I've selected parts (but haven't bought anything) from DIY including:

Motor 5055 190KV diy-electric-skateboard-kits-parts/electric-skateboard-motor-5055-190kv/

VESC diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

And here's my trouble: Batteries. I was thinking of getting 3x 5000mah 3s batteries and connecting them in series. Will this be okay? If I weight 70kg will I be able to go 13 miles? https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html 

My other query is charging difficulty. What charger should I use to charge the board? Since I've got 3x 3s batteries that's 9s. I want a simple charging port that I can stick into the board. I don't care too much about speed, as long as the range will get me 20km.

TL:DR Please help me decide my batteries and charging method! I want to go a long distance, don't really care about speed, need torque, 9s, don't know how to charge easily! THANK YOU!
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-04-28T16:55:05.151Z Reads: 129

```
Have you pulled the plug on the motor yet? I would suggest getting a 6355 sized motor instead. Based on you saying it's pretty hilly place. Also with the batteries it shouldn't be too much more but, I would recommend at least 30c instead of twenty. I don't have too much time to research at the moment cause I'm on lunch. Do you want to remove the batteries for charging or leave them in?
```

---
## \#3 Posted by: OskarCastrone Posted at: 2017-04-28T17:23:56.075Z Reads: 115

```
The easiest way would definetly be to use a BMS for charging. You should use the search function to learn more about that. 
As mentioned above, I would also consider a bigger motor, if you need a lot of tourque. The 5055 is acceptable for a beginner board on flat ground, but not on hills. The motor is most often used in a dual motor setup where it works great. 

When using such a small motor it will probably also get pretty hot when you are going up hills... That will also affect the effectivity which means that you will use more energy and therefore get less range. 

The battery you have chosen looks good. You could choose a higher c-rating, which would give you more tourque, but I am not sure you will feel a differnece using the small 5055 motor... If you need more range you could also hook up some batteries in parallel, which would also double the c-rating. 
The c-rating means how many amps the battery can deliver to the speed controller / motor. 

If you have any other questions, please let me know
```

---
## \#4 Posted by: sl33py Posted at: 2017-04-28T20:17:27.479Z Reads: 96

```
Good suggestions from the group so far.

I'd also suggest a 63mm motor setup.  And if you are going with only one motor - get the larger 6374 or similar instead of a 6355.  I just upgraded my GF's board from a 6355 to 6374 and even on 8s it seemed much more powerful.

If you find you still need more power for hills - then you can add a second motor in dual diagonal setup (on front trucks).

Even though the "rule of thumb" is 10Wh = 1km - it's very much a guess.  If you are riding up hills - you'll get less.  So if you are set on 13 miles - i'd add in some extra capacity to make sure you have enough capacity to do it.  I also would suggest higher C batteries so that voltage sag when riding hard (like uphill) won't cut your range short.

As for a charger - BMS might be simpler to charge, but overall more complicated to wire up.  Getting a decent lipo charger and balance board is simple and only takes a few minutes to connect and charge.  My .02.

GL!
```

---
## \#5 Posted by: emstr Posted at: 2017-04-28T20:53:17.603Z Reads: 86

```
Great thank you guys so much for your help @sl33py @OskarCastrone @i2oadsweepei2 

I'm going to buy the bigger motor from DIY thanks to your advice, I wasn't quite sure the difference between the two, thanks for clarifying.

As for the batteries, I'm just wondering if 15000mAh will even be enough to get me to school, it isn't too hilly but there's the occasional one. You guys also recommended a higher C rating. Would this battery setup work? 3x 8000mAh 30C https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html

Or could you recommend me the batteries you guys are using?

As for charging, no I don't want to remove the batteries for charging (@i2oadsweepei2) and I'd like something that's plug and play. A BMS seems like a very good idea, could someone recommend one and a charger for my setup based on your experience? How do you guys charge your boards?

Thanks again so much to all of you! Really helping me out.
```

---
## \#6 Posted by: SageTX Posted at: 2017-04-28T21:27:13.651Z Reads: 81

```
First, you aren't getting 15000mah. whenever you connect batteries in series, you increase voltage (9s) so you will have only 5000mah.  
And second - the 8000mah will be better for range. I use 9000mah (at 8s with zippys) and get up to 20 miles (Weighing ~65kgs).  Even though i have a _dual_ 6355 setup, I believe 8000mah zippys should get you home with a little to spare. Plus the 30c will keep the voltage sag down, thus increasing your range (so it won't sag under the mins).  
My 2¢
```

---
## \#7 Posted by: OskarCastrone Posted at: 2017-04-28T22:00:09.150Z Reads: 84

```
The battery you have linked to looks good! 

For a BMS, I would loomin ebay for the cheapest BMS for 9s available. You should only use the BMS for charging so the discharge ampere limit is not important. With a BMS yu can install a simple plug and play charging solution. It will be as simple as charging a laptop. Just search for: "BMS for 9s lipo" or something similar. As for the charger you need a "2 fase charger" for 9s. 

I use my own assembled LION battery. It is a bit more expensive but more reliable. For your first build, I would recommend some Lipo batteries though. It is easier and cheaper...
```

---
## \#8 Posted by: sl33py Posted at: 2017-04-28T22:20:17.345Z Reads: 83

```
As @SageTX mentioned - you won't have 15000mAh/15Ah.  Series increases voltage, parallel increases capacity.  So your 3 x 5000mAh 3s = 9s 5000mAh.  In parallel you'd have 3s 15000mAh.

To determine your watt hours (Wh):  V x Ah = Wh.  So take your pack voltage (9 x 4.2v = 37.8v) x 5/8Ah =  189Wh (9s 5Ah) / 302Wh (9s 8Ah).  So simple ballpark of 10Wh = 1km = 19km and 30km range for those two packs to compare.

The batteries i like are typically much more low profile - i think i have two sets of 3s in series.  one of the nano-tech 4500mAh 65c, and zippy compact 5000mAh.

the nano-tech 4500 are *super* thin at just about 20mm:
https://hobbyking.com/en_us/turnigy-nano-tech-a-spec-4500mah-3s-65-130c-lipo-boat-pack-mono1.html

To charge, while slower than some of the nicer iCharger and similar that can do 20/30/40Amps - the iMax B6ACv2 would be a good starter charger IMO.  Integrated power supply, so you don't need an AC->DC power supply.  Limited to 5A charge which can be slow.

HTH - GL!
```

---
## \#9 Posted by: Namasaki Posted at: 2017-04-28T22:24:20.735Z Reads: 81

```
[quote="emstr, post:5, topic:21960"]
Would this battery setup work? 3x 8000mAh 30C https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html
[/quote]
I agree that this battery would do the job for you, they are rather large though.

If you decide to hook a bms up to it, I would advise against getting  the cheapest bms you can find on eBay.
They have been known to be unreliable. 
If you decide to use a bms, spend a few dollars more and get a name brand like Bestech or Battery Supports.
You can use a bms for charge only however, there are some important  benefits to discharging through the bms as well.
And a good bms can save your batteries if a short occurs. Also, the bms will monitor every individual cells voltage and shut down if any cell falls too low. It will also prevent overcharging from regenerative  braking.
You will loose these benefits if you use a bms for charge only.
You will also need some sort of anti-spark switch or loop key unless you use a Bestech bms which has a built in E-switch.
```

---
## \#10 Posted by: emstr Posted at: 2017-04-29T09:41:10.348Z Reads: 77

```
Another round of great advice!

Okay... After looking around I think I've found a solution that could work thanks your post about BMS @Namasaki 
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/43

I think I'll get 5x 2s 5000mah 30C batteries and a BMS. @Namasaki is [this] BMS still applicable for the setup? (couldn't find a purchase button) - Also, would you have done anything differently next time? (http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html)  

Also, I'd love it if someone could explain to me how this whole battery is series vs parallel business. I'm so used to more mAh meaning longer life in phones - how does it work here, in simpleton(ish) terms - is it voltage ie 9s that shows capacity? Surely not.

So I'm thinking:

The big boy motor diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/
(Better torque and power over hills)

5x 2s 5000mAh 30C batteries https://hobbyking.com/en_us/turnigy-5000mah-2s-30c-lipo-pack.html
(Better C rating for less voltage sag on hills, 10s vs 9-9, low profile + higher capacity - right??)

Thanks fellas! Really supportive forum community, love it!!
```

---
## \#11 Posted by: Norco Posted at: 2017-04-29T10:21:01.388Z Reads: 64

```
I'm now wondering why people who use Lipos and want to build a single plug set up don't use hobby chargers and build a parallel charging board into a charging loop on their board? No need for a bms and batteries would be balanced charged each time?
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-29T13:08:08.202Z Reads: 63

```
To order a Bestech bms you need to email them with your request. The whole purchase process is done through email and they accept PayPal. 
Sales Contact is lucy@bestechpower.com
```

---
## \#13 Posted by: Namasaki Posted at: 2017-04-29T14:16:27.228Z Reads: 65

```
[quote="emstr, post:10, topic:21960"]
Also, I'd love it if someone could explain to me how this whole battery is series vs parallel business.
[/quote]

More capacity (mah)= more range and more current capability. 
More voltage = more range and higher rpm capability

More voltage = more range because with higher voltage you draw less amps. 
Less amps drawn means less capacity used.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-04-29T15:45:09.969Z Reads: 63

```
[quote="Norco, post:11, topic:21960"]
I'm now wondering why people who use Lipos and want to build a single plug set up don't use hobby chargers and build a parallel charging board into a charging loop on their board?
[/quote]
There are Bennifits you get with a bms that you don't get with a hobby charger. 
And the charging process is quicker and easier with a bms and simple charger.
```

---
## \#15 Posted by: SageTX Posted at: 2017-04-29T16:31:02.324Z Reads: 65

```
[quote="emstr, post:10, topic:21960"]
Also, I'd love it if someone could explain to me how this whole battery is series vs parallel business. I'm so used to more mAh meaning longer life in phones - how does it work here, in simpleton(ish) terms - is it voltage ie 9s that shows capacity? Surely not.
[/quote]

Well yes, mAh does show that the life is longer, basically it is capicity.

However where you are getting confused is the parallel/series connection.

The last battery choice (5 X 2S x 5000mah) you need to connect all in series to obtain 10S (~40v) voltage.  This series connection does not allow the mah to add up.  

The second battery choice(3 x 3s x 8000mah) you will connect in series as well.  However you will end up with 9S (~36v) voltage and 8000mah.  

NOW  to estimate (remember this is a total estimate) distance you need the WattHours (V x Ah).
So 40x5 = 200 WH.  APPROXIMATELY 10WH/KM = 20KM or 12.43 miles.
OR 36x9 = 324 WH or APPROXIMATELY 32KM or 19.88 miles with your 2nd choice of lipos.

NOW -  in my build **_I_** have 6 (total) X 4s X 3000mah lipos.  2lipos in SERIES make a 8s 3000mah (cell).  Take 3 sets of those and put them in PARALLEL you get a 8s3P 9000mah battery. (8x4x9 = 288 WH)

It gets confusing, especially when looking at lipos.  

Make any more sense??

BTW I am using 4.0v per series cell.  Max is 4.2 and nominal is usually 3.8.  its just easier to use 4.
```

---
## \#16 Posted by: emstr Posted at: 2017-04-29T23:59:11.810Z Reads: 64

```
Okay great, thank you for filling me in on battery in series vs parallel. I get it now.

I'm still quite stuck on what batteries to buy though, as everyone has a different setup.

@SageTX I am thinking about going your route. Is there any downsides to doing series and parallel together? Ie charging times? I know the cost is a lot higher than my 3s 8000mah solution.

 So what should I do? I want to spend no more than $150 on batteries that will get me at least around 250wh. What's the best way to do this right now?
```

---
## \#17 Posted by: mmaner Posted at: 2017-04-30T00:58:50.995Z Reads: 61

```
I just finished building a 10s pack with x5 2s 5000mah 30c Zippy hard case lipos.  @Namasaki did it before anyone.  It works very well.  The batteries and a cheap 10s BMS should be around 150 bucks.

 x5 ZIPPY Flightmax 5000mAh 2S1P 30C hardcase pack
$24.99 e = $124.95 + $9.84 = $134.79
https://hobbyking.com/en_us/zippy-flightmax-5000mah-2s1p-30c-hardcase-pack-roar-approved-de-warehouse.html

60A Lithium-Ion 7S10S13SBleeding BMS(30A-60A)with electronic Switch (BMSOn-Off)
$22.00 + $4
http://www.ebay.com/itm/222373438930

Total = $164.79
```

---
## \#18 Posted by: emstr Posted at: 2017-04-30T02:14:08.132Z Reads: 57

```
Alright team! I've compiled a list of 3 battery options based on all of the suggestions. Feel free to make any new suggestions. Also feel free to tell me if I'm being an idiot.

My required specifications: 

* 250wh battery minimum
* Under $150USD

**wh = V*Ah**

**Option 1**

https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html

3x 8000mAh 3s 30C 11.1V - series

 = 9s 8000mah 34V

34x8 = 272wh for $132

_=$0.49/wh_

169mm*207mm*27mm, 945cm^2, 1.9kg - thicker fatter and cheaper, and slightly lighter - 9s rather than 10

**Option 2** - @SageTX 

https://hobbyking.com/en_us/turnigy-3000mah-4s-30c-lipo-pack.html

6x 3000mah 4s 30C 14.8V - connect 3 lots of 2 in series to create… 

3x 3000mah 8s 30V connect that in parallel…

8s 9Ah 29.6v

9x29.6 = 270wh for $210

= $0.7/wh

137mm*258mm*25mm, 884cm^2, 2kg - slightly thinner, different form factor, bigger area, more cost

**Option 3** - @mmaner, @Namasaki 

 https://hobbyking.com/en_us/zippy-flightmax-5000mah-2s1p-30c-hardcase-pack-roar-approved-de-warehouse.html

5x 5000mAh, 2s, 30c, 7.4v - series

= 10s 5Ah 37V 

5x37 = 185wh for $150

= $0.81/wh

Cheaper (not really), but doesn't hit the mark for range - 10s with more power though.

So now I wanna know some stuff! With the battery that you're using @SageTX it seems to be more expensive and I can't see why I'd go with that one over option 1. Is there more speed? Or since there's 30c x6 is there less voltage sag? Is it better to have 6 batteries than 3? What are the benifets that I'm missing? 

Again thank you all so much, I'm genuinely learnt so much this past 24 hours, way better than physics class!! Haha. I owe you one guys :slight_smile:
```

---
## \#19 Posted by: mmaner Posted at: 2017-04-30T02:34:58.934Z Reads: 54

```
Ok, didn't realize we were competing.  Good luck.
```

---
## \#20 Posted by: emstr Posted at: 2017-04-30T03:01:56.223Z Reads: 53

```
Nah nah nah! I really loved that battery setup, especially for its power. Some of the guys here on the forum said it wouldn't be enough for the range that I wanted. Really appreciate your help though! It was an option I was genuinely considering.
```

---
## \#21 Posted by: mmaner Posted at: 2017-04-30T04:33:24.804Z Reads: 51

```
Some.of the guys here don't understand that when it comes power density there's a difference between x5 2s packs and x2 5s packs. 

My issue was that you asked for help, then scored the help you were freely given. Not very gracious imo.
```

---
## \#22 Posted by: emstr Posted at: 2017-04-30T04:46:06.469Z Reads: 51

```
Sorry man! Could you give a beginner some of your knowledge? 

What's the difference between power density in x5 2s packs and x2 5s packs? What would you recommend to get to my desired range? I need to get up hills and need at least 25-kilometer range if not more. 

I am completely open to suggestions, no need to get tweaked. It just didn't seem like there was any evidence that I would get my range with that setup. Can you understand where I'm coming from?
```

---
## \#23 Posted by: emstr Posted at: 2017-04-30T06:17:25.668Z Reads: 49

```
@Namasaki @mmaner How much range do you guys get on your 10s 5000mah boards? My environment is fairy hilly.

I realise that there is far more current in the 10s 5000mah pack, does this make the packs last longer while not technically having more WH?

@Namasaki if you were to build a board with my specifications, what would you do? Really appreciate your skill.
```

---
## \#24 Posted by: Namasaki Posted at: 2017-04-30T06:30:38.522Z Reads: 49

```
Not only voltage and capacity play a part in range but discharge rate also factors in because higher current capability means more headroom which means less voltage sag.
Less voltage sag mean less current draw which in turn means more range.
example:
My 12s/5000/25C/125a    got me 10-12 miles
My 10s/5000/60C/300a    gets me 12-14 miles
The lower voltage battery should  get less range but instead it gets more because the voltage sag is much less with a 300a battery than it is with a 125a battery.
```

---
## \#25 Posted by: landonkun Posted at: 2017-04-30T17:36:02.982Z Reads: 50

```
[quote="mmaner, post:21, topic:21960"]
My issue was that you asked for help, then scored the help you were freely given. Not very gracious imo.
[/quote]

I see what you're saying, but @emstr is just trying to weigh his options for his first build, understandably. I did the same kind of math when I did my first build. He still seems very appreciative :slight_smile:
```

---
## \#26 Posted by: SageTX Posted at: 2017-05-01T16:03:34.431Z Reads: 47

```
You are on the right track.  You now have to choose what's best for your build abd expectations. 

To  answer your question though, I went with the 6 batteries because I bought from another builder and got a deal.
```

---

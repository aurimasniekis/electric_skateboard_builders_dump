# Loaded tan tien, 6374 mono drive, 3D printed enclosures

### Replies: 12 Views: 1857

## \#1 Posted by: BenTheBarre Posted at: 2017-07-01T01:20:08.182Z Reads: 249

```
Hey all! 

This year, in my high school engineering class, my classmate wrote a grant and $1000 was donated to our class to build an electric longboard. It was fantastic! I emediatly fell in love. Dual drive, 12s, homemade deck- it was raw. 

 I've always wanted to build an E-skate since the boosted hype a few years back, and after building one for school, I put the nail in the coffin. I've been lurking for a while now, and have had some experience with the previous build for school. I'd love some input on my upcoming build! 

Goals: 
*as lightweight as possible
*7-8+ mile range (more the better)
*great for carving 
*solid hill climbing ability
*clean looking
*easy to charge 
*smooth ride (Spokane streets kinda suck)
*as cheap as possible (can splurge depending on how much lawn mowing is done this summer)

Parts list: (ITEMS WITH ! HAVE BEEN BOUGHT)
*Deck- loaded tan tien flex 2 !
*caliber 2 50° 10inch !
*97mm flywheel clones !
*15mm belt, 15:36 ratio gearing (ebay) !
* torque VESC 
*torque 190kv 6374 sensored
*torque motor mount 
*3x series turnigy 3s 5000mah {9 cell} (or 4x? 6000mah? I'm just worried about room, and the flex of the deck)
*some bms for charging (bestech? They're very expensive tho..)
*anti spark xt90 loop key 
*printed enclosure (need to design- have printer) 
*mastercho mod gt2b 
*flat braided copper wire to mate enclosures

There she is! Super excited. Like I've mentioned within the parts list, I do have some questions and would like critique if possible. 

Firstly, at a single 190kv, would 9s be a sufficient power supply? Or should I go 10 or 12? I would go 18650 cells, but they seem expensive and I don't have a spot welder:/ Battery space is an issue as well(need to be close to trucks to prevent bottoming out) 
Has anyone else used the tan tien in a build? Haha am I the first? I could also top mount the drop through deck for more space....

Also, I should aim for the highest c rating output, correct? Higher amp output will reduce voltage sag,  and improve range right?

What BMS should I get? Is there a cheaper option than bestech if I bypass it for discharging?  

Sorry for the barrage of questions. Thanks everyone though! Excited for this build, and will keep this thread updated with the progression. 

-Ben
```

---
## \#2 Posted by: Jammeslu Posted at: 2017-07-02T09:16:17.174Z Reads: 198

```
You can buy a very cheap bms if you are charging only, but if you want to discharge aswell have a look batterysupports bms at least 60A con
```

---
## \#3 Posted by: Jammeslu Posted at: 2017-07-02T09:17:28.258Z Reads: 197

```
And Im building the apx the same build can you show pictures of the final enclosure bc Im looking for one aswell for tan tien thanks!
```

---
## \#4 Posted by: BenTheBarre Posted at: 2017-07-02T17:25:06.765Z Reads: 187

```
Alright, so I'm looking at the zippy compact 6200mah 3s 40c packs(wired 3 in series for 9s). With these batteries, I'd be getting 248a discharge right? (6200*40)/1000

 That seems very high, but will the VESC and motor only draw what they need? I've read that the higher discharge your packs are, the less voltage sag you will get and therefore longer range/longevity. 

Also, how would this bms perform if only set up in a discharge-only format? I'd just rather save some cash and bypass than buying a Bestech and running it on balance discharge..  http://www.ebay.com/itm/Balance-BMS-PCM-21A-w-Temp-Switch-for-9S-33-3V-Li-ion-Li-Po-battery-9S21W001-/221809130907 

Also, it would be much appreciated if someone could direct me to a wiring diagram of a bypassed bms. I've been browsing the forum but there just seems to be a lot of misconstrued information and mis-drawn diagrams...

@Jammeslu Will do! I have yet to design them, but I'll let you know. I will probably upload them to thingaverse as well.
```

---
## \#5 Posted by: Jammeslu Posted at: 2017-07-02T22:42:15.048Z Reads: 160

```
Yes you are correct with the Battery and Vesc theory.
Discharge only ? Do you mean charging only?
```

---
## \#6 Posted by: wmj259 Posted at: 2017-07-03T00:38:38.064Z Reads: 160

```
I'm running a 6374 190kv on 9S (3x3S) and it's enough power for me. I limited my erpm in the vesc setting and can still hit 22mph, which is good enough for. Me.
```

---
## \#7 Posted by: BenTheBarre Posted at: 2017-07-03T05:55:30.229Z Reads: 149

```
@Jammeslu yes, the bms, if bypassed becuase of low amp output, for charging purposes only.
```

---
## \#8 Posted by: Jammeslu Posted at: 2017-07-03T12:31:43.880Z Reads: 143

```
Yes many people here does it and it saves a buck, i have personally not Done it but you can easy use the search function and find a diagram, just make sure the values on the “vesc” are correct since that’s taking over the bms job of overcharge and overdischarge etc
```

---
## \#9 Posted by: BenTheBarre Posted at: 2017-07-04T20:11:50.864Z Reads: 145

```
I think I'm going to go 10s instead of 9s (2 5s turnigy in series) for ease of finding chargers and bms's. 9s is just too strange and there doesn't seem to be many options. 

I am looking at this bms- 
http://m.ebay.com/itm/221769582503?_trksid=p2385738.m2548.l4275&_mwBanner=1

With 60a discharge, would I be safe using the balance discharge feature? And how reliable can these ebay Bms's be? I would definitely go for a bestech, but there "min order 2" policy is a huge turnoff, and I'm on a pretty tight budget at this point. If anyone has a spare 10s bestech bms id definitely buy it though! Haha

https://tinyurl.com/y96kzp89
Also, this^ charger is what I should use, correct? With only 2a charge I do expect it to be slow though. Should I look for a higher ampere charger? I Or does 2a work just fine?
```

---
## \#10 Posted by: WawiKirsinger Posted at: 2017-08-19T17:59:20.200Z Reads: 125

```
@BenTheBarre so how is your build going? any progress? take photos plz! 

thanks! hope you are doing ok!
```

---
## \#11 Posted by: BenTheBarre Posted at: 2017-08-21T22:49:15.942Z Reads: 126

```
Hey all! Sorry for the lack of updates. Board is finished!! Few changes made,  3d printed the enclosures out of wood PLA and opted for 2 5s 35-70c lipos in series at 10s1p. No BMS yet. 

 However, during the first test ride, after braking, the VESC quit! In BLDC I am getting DRV8302 error:( After looking back at my settings, I realized I never set the ERPM limits to 60k (at 100k)... could this have been the issue? I'm also worried that my problem could have been associated with the long battery connection to the VESC. Does having an extension result in damaging the VESC? I know it can be troublesome with normal ESC's. I just want to make sure I don't ruin my next speed controller. Kinda really disappointed, but just bought another replacement from @torqueboards 

<img src="/uploads/db1493/original/3X/a/3/a343b1b8dbd53971e4201ca6c5a82ef75a093494.JPG" width="690" height="459">

<img src="/uploads/db1493/original/3X/3/9/39c325713bc020572c356ff4db4267818538d7ff.JPG" width="690" height="459">

<img src="/uploads/db1493/original/3X/8/7/87c3fd7e7ce0fc1cc5ddc39c2b90d0db5393f379.JPG" width="690" height="459">

<img src="/uploads/db1493/original/3X/3/0/30e36ac7e9457b6b419a45e6240615c0b8e56b3f.JPG" width="" height="500">
```

---
## \#12 Posted by: ivanflo Posted at: 2017-12-03T13:01:31.142Z Reads: 86

```
i'm getting started with a Tan Tein or Dervish build soon, just dimensioning both boards which I already have and will have to decide on either.

Just wondering how you have faired in terms of bottoming out and flex. I would like to keep the flexible feeling of these particular boards and also want to keep my wheels at 72mm with the drop through as well.
```

---

# Is this a good battery pack?

### Replies: 8 Views: 302

## \#1 Posted by: BP1702 Posted at: 2019-02-26T08:38:40.728Z Reads: 134

```
Hi guys,

I was hoping you would be able to tell me if [this](https://www.voltation.net/product-page/alien-power-pack-10s-10000mah) 10s3p is a good battery pack? I am planning on using the [HAGGY DRIVE SYSTEM - 2 IN 1 kit](https://haggyboard.com/products/haggy-drive-system-2-in-1-street-and-all-terrain-version?variant=10625113718899) to build a board. I'll mostly use the Bergmeister All-Terrain wheels (150mm). How much range can I expect to get with this pack assuming I averaged at like 30 - 40kph and will it be able to produce good torque? I'm not very experienced in this stuff and so to me it looks good with the built in BMS, battery indicator, charging port... The cost of the pack is $497 AUD total (355USD). Thanks for the help guys, this is my first build. :slight_smile:
```

---
## \#2 Posted by: Winfly Posted at: 2019-02-26T09:23:49.671Z Reads: 123

```
APS is really reputable is all i can say. no idea what kind of cell is in it. probably the HG2 which is good but no as good as the 30Qs.
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-02-26T09:38:56.549Z Reads: 118

```
Based on the advertised numbers, it suggests a 2900mah cell, and I don't know any of those made by LG that are very high-current. It'd be a little weird to use a 3000mah (HG2) cell and call it 2900. 

@BP1702  Either way, whether it's a HG2 or 30Q, A 10s3p pack is only really good for 60A continuous, not the 80 that's advertised there, so keep that in mind when you're setting up your ESCs.
```

---
## \#4 Posted by: BP1702 Posted at: 2019-02-26T09:57:33.241Z Reads: 105

```
Okay, thanks. What kind of performance do you think I could get with that? Will torque / top speed / range be no good with only 60A continous on 150mm AT wheels? I'm planning on using the focbox unity which I think can take a fair bit more than that. Would you recommend another pack like 10s4p etc.. or even change to LiPo? Sorry, i'm not experienced with this battery stuff.
```

---
## \#5 Posted by: Schulerbible Posted at: 2019-02-26T10:33:41.731Z Reads: 90

```
Just as an example: I am running an oldish 10s3p with Samsung 25R cells (2.5ah ea) and get about 20 km on flat and 15 km on hilly terrain (97 mm wheels and dual drive). If it’s windy the range drops another few km. Def not great. 😪
```

---
## \#6 Posted by: BP1702 Posted at: 2019-02-26T11:51:57.219Z Reads: 79

```
hmm, that sucks. :frowning:  So what do you guys think would be the optimal battery to use if I was looking for a 25km range while averaging about 30-40km that also provides good torque? Would wiring 2x 12000mAh 6S LiPos into series to make a 12s be an alright option? Or should I stay away from LiPos and get something else? What would ya recommend? Thanks
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-02-26T18:15:53.961Z Reads: 53

```
Lipos and cylindrical cells both have their pros and cons, but I personally am a cylindrical guy. In terms of power to weight, lipos win. But in terms of energy to weight, and especially energy to volume, cylindrical cells win by a LARGE margin. 

Lipo cells also don't usually last as many charge/discharge cycles (100-500, compared to 500-2500+ for cylindrical cells) and they're more susceptible to damage by puncture.

60A should give you some decent power, but nothing absolutely mind-blowing. The focbox unity is definitely capable of a lot more.

If you want a ballpark range calculation for different configurations, plug all your information into an esk8 calculator - [https://calc.3dservisas.eu](https://calc.3dservisas.eu) is a pretty good one.
```

---
## \#8 Posted by: BP1702 Posted at: 2019-02-27T02:09:23.589Z Reads: 31

```
Awesome, thanks for the help!
```

---

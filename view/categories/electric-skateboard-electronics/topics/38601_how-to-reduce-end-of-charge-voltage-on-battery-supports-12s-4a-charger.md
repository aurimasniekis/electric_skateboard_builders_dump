# How to reduce end of charge voltage on Battery Supports 12S 4A charger

### Replies: 40 Views: 2318

## \#1 Posted by: Eboosted Posted at: 2017-11-17T05:55:30.638Z Reads: 216

```
I've heard some people were able to adjust the end of charge of these chargers, does anyone knows what components would be needed to get and adjustable end of charge voltage?
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-17T05:57:21.701Z Reads: 217

```
Post a picture please. If it's one of the aluminum chargers, it should be fairly straightforward to get it open. Most of them have a trim pot on the output side for adjusting the output voltage.
```

---
## \#3 Posted by: rojitor Posted at: 2017-11-17T12:38:08.768Z Reads: 204

```
Some can't be changed. Open it. If you see blue pots you can do it. Usually the pot next to output is voltage and the one in the center is amperage. If you increase voltage you must lower amps. If you lower v you can increase amps. If you see 3 pots just ignore the third.

https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/5/5548ae39124490bb826a75cf1866e638b090df8d.jpg
```

---
## \#4 Posted by: Eboosted Posted at: 2017-11-17T18:15:30.090Z Reads: 188

```
I'll open my charger today and upload a picture of the internals.

I don't understand why I'd have to increase the current when decreasing voltage, current is usually lowered automatically when the preset voltage is reached.
```

---
## \#5 Posted by: rojitor Posted at: 2017-11-17T18:33:04.848Z Reads: 186

```
You are right. But afaik some chargers keep the amperage making it risky. So you must be careful on that.
Edit:if you plan to lower the voltage you are safe no matter what. I just recall a guy that increased voltage and kept the amperage. Since the wats were over the límits of the charger it fried in a few minutes.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-11-17T21:47:48.208Z Reads: 178

```
Here is the opened charger:

[img]https://i.imgur.com/awNfDjN.jpg[/img]

Seems to be a very similar one, I'll hook a voltmeter and adjust the voltage al 50.00V, hope it works, I'll report back.
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-11-17T22:22:37.138Z Reads: 174

```
I remember reading somewhere (don't ask me for source) that the bms does its balancing once it's reached full charge.

so if your release voltage is 4.2, but your power supply only reaches, let's say 4.1v, then wouldn't that prevent the balancing function?
```

---
## \#8 Posted by: Ronny_CTS Posted at: 2017-11-17T22:29:45.384Z Reads: 173

```
I'm interested in knowing this as well...i would like to use a bms to charge my cells, but i would also like to undercharge my cells to increase cycle life. So i am also interested in in knowing if the bms will still do its job if the cells are only charged up to 4.1v.
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-11-17T22:40:24.748Z Reads: 171

```
with the bms you're getting from me, I had the modules modified so their upper release voltage is 4.1v. so at 4.1v they'll be balanced
```

---
## \#10 Posted by: jmasta Posted at: 2017-11-17T22:41:25.921Z Reads: 172

```
The SuPower BMS starts balancing at 4.15V

I use a variable voltage 12S charger. Usually I only charge to 4.0~4.1V, but every few cycles I go to 4.20V to ensure that the cells get properly balanced

Permanently modifying your charger to a lower voltage might not be the best course of action. Maybe you could add an external knob for the voltage potentiometer so you can easily adjust output voltage
```

---
## \#11 Posted by: Eboosted Posted at: 2017-11-17T22:49:09.080Z Reads: 170

```
I was able to reduce the voltage from 50.9V (4.241V per pack) to 50.2V (4.183V per pack), so I'm expecting this to avoid the overcharge situation on braking at 100% SOC caused by the BMS shutting down all power to the VESCs.

As I'm unsure which is the other blue pot for current, but I'd like to reduce the charging current to 3A, 2A is too low and 4A is not mandatory for me, for this test I didn't move current, I hope I don't fry anything.

https://www.youtube.com/watch?v=_TZCSqMZVBE
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-11-17T23:41:02.675Z Reads: 159

```
Regarding the BMS issue, I'm using one from AliExpress that has fully adjustable settings, so I've set mine to start balancing at 3.7v. it'll waste a couple percent maybe, but it'll always stay balanced even if I only ever half-charge it.
```

---
## \#13 Posted by: Eboosted Posted at: 2017-11-18T00:01:06.255Z Reads: 159

```
[quote="MysticalDork, post:12, topic:38601"]
I'm using one from AliExpress that has fully adjustable settings, so I've set mine to start balancing at 3.7v. it'll waste a couple percent maybe, but it'll always stay balanced even if I only ever half-charge it.
[/quote]

Can you point us the link of the BMS you got?
```

---
## \#14 Posted by: scepterr Posted at: 2017-11-18T00:05:10.745Z Reads: 156

```
My advice is get one of these, and charge any battery at whatever voltage and current below the max of your current charger
Max output is 50V, which gets you max 4.16v/cell on 12s and you can set it to anything below that
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/2941
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/2945
```

---
## \#15 Posted by: b264 Posted at: 2017-11-18T00:16:27.615Z Reads: 150

```
[quote="scepterr, post:14, topic:38601"]
My advice is get one of these
[/quote]

Those suck for carrying your backpack
```

---
## \#16 Posted by: Eboosted Posted at: 2017-11-18T00:17:09.988Z Reads: 149

```
I already got this one, but you don't want to carry it on your back pack on long trips :grinning:

[img]https://images-na.ssl-images-amazon.com/images/I/61IxN-RPGkL._SL1000_.jpg[/img]

I'll try the SuPower charger today adjusted at 4.18v
```

---
## \#17 Posted by: scepterr Posted at: 2017-11-18T00:26:43.750Z Reads: 149

```
<img src="/uploads/db1493/original/3X/6/4/649ce4b1c0d63e1e9d9c50232022aa7bea5f7d68.jpg" width="422" height="500">
<img src="/uploads/db1493/original/3X/3/0/306a04d3168b46c90767bacc905134d1c8ab2ddb.jpg" width="375" height="499">
<img src="/uploads/db1493/original/3X/a/f/af08d58a496a82a65a1e66ed6d508f85b5933a6a.jpg" width="361" height="500">
```

---
## \#18 Posted by: Eboosted Posted at: 2017-11-18T01:00:07.864Z Reads: 140

```
Can you take a picture with a dollar bill besides it?
```

---
## \#19 Posted by: scepterr Posted at: 2017-11-18T01:05:02.514Z Reads: 147

```
Still need to add tiny fan and mount ports
<img src="/uploads/db1493/original/3X/5/0/50267de92dabc5b71b3dc7f598802b39b5739167.jpg" width="487" height="500">
```

---
## \#20 Posted by: jmasta Posted at: 2017-11-18T01:28:15.002Z Reads: 149

```
Here's my charge setup.  12S 4A CCCV charger with adjustable EOC.  It can be adjusted from about 42V to 50.4V by turning the pot knob on the side.  I only use 12S so this is perfect for me

I added a power meter to monitor voltage and current.  The meter has the same input/outut as my board and the charger, so I can use the charger with or without the meter.  Overall the system is very compact and portable.  It is not much bigger or heavier than my 12S 2A brick charger. 

<img src="/uploads/db1493/original/3X/e/f/effc5530cd59761305b0fbbd9c198ef8d49552c1.jpg" width="690" height="441">
```

---
## \#21 Posted by: deucesdown Posted at: 2017-11-18T03:41:59.899Z Reads: 145

```
This meter reads consistently 0.2v high? Not adjustable. And that recessed button, grrr.. I've been meaning to glue something to it so I can reset the "energy" without grabbing a pen. It's awesome though.
```

---
## \#22 Posted by: Eboosted Posted at: 2017-11-18T05:38:45.075Z Reads: 138

```
Would you mind sharing the part lists and sources?

Where did you get that adjustable EOC voltage charger?
```

---
## \#23 Posted by: b264 Posted at: 2017-11-18T06:11:54.952Z Reads: 135

```
[quote="MysticalDork, post:2, topic:38601"]
If it's one of the aluminum chargers, it should be fairly straightforward to get it open. Most of them have a trim pot on the output side for adjusting the output voltage.
[/quote]

Where does one obtain these chargers?  I have one but I don't know where they are sold to get more :cry:
```

---
## \#24 Posted by: Eboosted Posted at: 2017-11-18T06:19:59.212Z Reads: 131

```
http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#25 Posted by: cwazy1 Posted at: 2017-11-18T06:53:43.244Z Reads: 132

```
is there any available in the USA? I'm also having a hard time finding these locally.
```

---
## \#26 Posted by: b264 Posted at: 2017-11-18T06:58:20.885Z Reads: 128

```
I still can't even find them there.  I'm looking for 10S 1.8A (2A will work but prefer 1.8A) chargers with adjustable voltage and I can't find a single one
```

---
## \#27 Posted by: cwazy1 Posted at: 2017-11-18T07:18:38.388Z Reads: 128

```
https://www.aliexpress.com/item/50-4V-3A-3-5A-4A-4-5A-Lithium-Ion-Battery-Charger-For-Two-Wheel-Chair/32812792872.html?ws_ab_test=searchweb0_0,searchweb201602_1_10152_10065_10151_10344_10068_10130_10345_10324_10342_10547_10325_10343_10546_10340_10341_10548_10545_10541_10562_10084_10083_10307_10178_10060_10155_10154_10539_10312_10059_10313_10314_10534_10533_100031_10103_10073_10594_10557_10558_10596_10595_10142_10107,searchweb201603_25,ppcSwitch_5&btsid=76e48901-86c2-4c05-b2d0-1403184c6440&algo_expid=84776f40-0705-4c3f-956f-152b170e782b-2&algo_pvid=84776f40-0705-4c3f-956f-152b170e782b&rmStoreLevelAB=0

This looks like the cheapest option on aliexpress.
```

---
## \#28 Posted by: cwazy1 Posted at: 2017-11-18T07:19:22.886Z Reads: 123

```
He likely purchased the link I posted, and then added a voltage pot.
```

---
## \#29 Posted by: b264 Posted at: 2017-11-18T07:33:45.642Z Reads: 123

```
"Cheapest" is not what I'm looking for.  I'm looking for a 42V (adjustable voltage) 1.8A (2A if I have to) Li-ion charger.  "Cheaper" only matters if I can find more than one.  That one above is not 42V...
```

---
## \#30 Posted by: Ronny_CTS Posted at: 2017-11-18T08:35:24.447Z Reads: 127

```
@Eboosted there was a group but that when on a while ago and @jmasta 's charger looks very much like the one in the group buy! 

https://www.electric-skateboard.builders/t/10s-and-12s-adjustable-charger-from-china-groupbuy-worldwide/17287/177?u=ronny_cts

Perhaps we could organize a need group buy for similar chargers with adjustable EOC. I would totally jump on a few.
```

---
## \#31 Posted by: Sk8Board Posted at: 2017-11-18T11:23:59.391Z Reads: 114

```
http://vruzend.com/product/52v-lithium-ion-battery-charger-3-amps/
```

---
## \#32 Posted by: Eboosted Posted at: 2017-11-18T17:54:27.031Z Reads: 110

```
Yeah, I know. @jmasta made a group buy a while back, he hasn't disclose who the seller was at the time or where he got those chargers from.
```

---
## \#33 Posted by: jmasta Posted at: 2017-11-18T18:21:49.702Z Reads: 109

```
Yep I got the 12S adjustable charger from @PXSS 's groupbuy awhile back. Maybe you could contact him to track down the source.  I can take a picture of the charger's label if that is helpful

 I haven't modified or opened the charger at all.  It was marketed as 5A but my 12S version is only 4A (which is plenty).  I suspect it is just a 200W charger that they adjust for 10S and 12S ranges.    I honestly don't know why these aren't more common.  I'm not sure how I'd live without mine!

The power meter is just from Amazon.  Get the 20A version for your charger so you don't need to use a shunt resistor.  It has screw terminals for input/output.  If you want to make the charger work with and without the meter, the meter's input needs the same port as your board and the output needs the same plug as your charger

  @Eboosted @cwazy1   

https://www.amazon.com/Digital-Voltmeter-6-5-100V-ChiTronic®-Multimeter/dp/B01GZP743E/ref=sr_1_4?ie=UTF8&qid=1511029022&sr=8-4&keywords=power+meter+dc+20a
```

---
## \#34 Posted by: Eboosted Posted at: 2017-11-18T18:30:30.634Z Reads: 99

```
Yeah the one that didn't disclose the source was @PXSS not sure if the seller can't be found or if he does not know where to get more of them.

@jmasta did you charger come with the adjustable EOC knob? Did you added it?
```

---
## \#35 Posted by: jmasta Posted at: 2017-11-18T18:39:29.692Z Reads: 99

```
The external EOC knob came like that.  I bet you could add one to the voltage pot on yours and modify the case to be able to access it

Or.... drill a hole in the case above the potentiometer and use a screwdriver to change?
```

---
## \#36 Posted by: Eboosted Posted at: 2017-11-18T18:41:19.579Z Reads: 98

```
My Battery Supports charger can only decrease EOC down to 50.2v, if I keep on turning the knob it wouldn't let me go down more
```

---
## \#37 Posted by: Eboosted Posted at: 2017-12-07T05:29:13.215Z Reads: 89

```
Ok, my charger stoped working, I think it's tosted.

So, it seems lowering the EOC voltage causes some issues on the charger
```

---
## \#38 Posted by: cwazy1 Posted at: 2017-12-07T05:32:51.663Z Reads: 87

```
Thats good to know..
```

---
## \#39 Posted by: Ronny_CTS Posted at: 2017-12-10T09:26:18.331Z Reads: 83

```
Stole the source from another thread. Has anyone tried [this charger?](https://www.ebay.com/itm/50-4V-8A-Lithium-Battery-Charger-for-44-4V-8A-Car-Li-ion-Ebike-XLR-Plug/282751644047?hash=item41d54fb18f:g:TM0AAOSw2nNZ6Gu4) Aluminum case, 50.4V, 8Amps, Dual fan cooled! 

Can't really make out if it has pots to adjust the EOC? Can anyone find them in the image they provide?
```

---
## \#40 Posted by: Flaco Posted at: 2018-02-02T17:30:07.352Z Reads: 69

```
Mine is in the mail but this is what I bought  for my 12s.
Input
AC 90 to 305v

Output
Voltage adjustable range: 44.8 to 51.2
Current adjustable range: 2.5 to 5 amps

Another characteristics:
cc/cv
metal housing
ip65
7 year warranty

http://www.meanwell.com/webapp/product/search.aspx?prod=HLG-240H

Also it is FANLESS
```

---

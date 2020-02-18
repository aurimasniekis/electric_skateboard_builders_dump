# What charger to use for 8s4p lithium ion

### Replies: 30 Views: 3267

## \#1 Posted by: moe_lester Posted at: 2017-03-09T12:07:21.931Z Reads: 218

```
HI guys I'm from London, I am having trouble finding a charger for my lithium ion battery pack. 

My pack is 8 in series and 4 in parallel using samsung 25r meaning my pack is = 33.9v max charge

I have a bms and I will charge through the bms. 

My question is what charger/port shall I use. I can't seem to find a 33v charger. Also do I need 1A,  2A, 3A or 4A because I don't know. I don't need a balance charger because the bms does that, so all i need is charging port and a charger. 

Cant I use a 36V charger? and unplug it earlier so my pack doesn't exceed 33v? is that even possible? Will my house blow up?
```

---
## \#2 Posted by: Okami Posted at: 2017-03-09T12:55:54.380Z Reads: 209

```
if u want to charge a bit faster then choose with higher A.. 3-4A should be good.. but you might as well go with 2A and wait about 4-5hours till charging is complete..

u should look for one's with adjustable voltage.. you wil have to search around a bit..

Take a look at what @PXSS offered in his group buy.. it might be possible to downgrade the voltage enough for your system..

keep looking ;)
```

---
## \#3 Posted by: moe_lester Posted at: 2017-03-09T13:35:39.343Z Reads: 194

```
Great thanks man, theoretically what would happen if I used a 36v charger?
```

---
## \#4 Posted by: Okami Posted at: 2017-03-09T15:46:52.612Z Reads: 182

```
10s charges till 41v.. unless u can turn it down to 34 or so.. u.will overcharge.your.cells.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-09T21:08:29.039Z Reads: 168

```
Full charge for an 8s pack is 33.6 not 33.9
4.2v x 8 = 33.6
Using a 36v charger could be dangerous. 
You could get a variable power supply to charge it. 
It would have to have adjustable voltage and current with constant current and constant voltage modes.
Then if you decide to build a bigger battery later, you'll be able to use the same charger up to 12s

SKYTOPPOWER STP6005 Precision Variable DC Power Supply 0 - 60V / 0 - 5A Digital Adjustable Regulated Lab Grade Safe Circuit Design - US Power Cord https://www.amazon.com/dp/B01MQFCFMN/ref=cm_sw_r_cp_api_zuCWyb6VJC6PG
```

---
## \#6 Posted by: Namasaki Posted at: 2017-03-09T23:28:36.553Z Reads: 156

```
[quote="moe_lester, post:3, topic:18800, full:true"]
Great thanks man, theoretically what would happen if I used a 36v charger?
[/quote]


 best case scenario: Your BMS might not work if you use a higher voltage than it was designed for.
worst case scenario: :volcano:
```

---
## \#7 Posted by: Namasaki Posted at: 2017-03-09T23:32:03.551Z Reads: 157

```
I got tired of my cheap  brick chargers cutting off before my battery was fully charged and got a 60v 5a adjustable Linear power supply to charge my batteries.
And it works like a dream!!!
<img src="/uploads/db1493/original/3X/7/9/791cdee632cad64b2e152de0ce22a56a33c032b1.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/3X/f/4/f4e5c69cd3790d7e29c2b1bf63fe76872a464dfb.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/3X/8/d/8d267396d0c867229495367b3e4fbc502b95e24c.jpeg" width="375" height="500">
It starts in constant current mode and slowly brings the voltage up until the battery reaches around 90%
then it switches to constant voltage mode and as the battery fills up the current gradually decreases until it gets to zero at which point the battery is full.
```

---
## \#8 Posted by: sl33py Posted at: 2017-03-09T23:36:02.531Z Reads: 152

```
I got a lab power supply a few years ago too - like @Namasaki has in his pic.

I've thought about building another from components...  Here's a cool option for those who want to make their own variable power supply:
http://www.banggood.com/DP50V15A-DPS5015-Programmable-Supply-Power-Module-With-Integrated-Voltmeter-Ammeter-Color-Display-p-1072236.html
```

---
## \#9 Posted by: mrplaygood Posted at: 2017-03-09T23:36:51.127Z Reads: 148

```
Do you have a special charger between your batteries and the supply? I got myself a bms but the manufacturer told me I have to buy a cv cc charger. I don't really get it 🤔
```

---
## \#10 Posted by: mrplaygood Posted at: 2017-03-09T23:38:40.105Z Reads: 147

```
If you already got yourself a bms maybe this is something for you:
http://www.ebay.com/itm/Intelligent-Smart-33-6V-2A-Charger-for-8S-28-8V-29-6V-Li-ion-Li-Po-Battery-EU-/321471399664?hash=item4ad93046f0:g:YXAAAOSwKIpWBgVj
```

---
## \#11 Posted by: Namasaki Posted at: 2017-03-09T23:40:32.113Z Reads: 143

```
[quote="mrplaygood, post:9, topic:18800"]
Do you have a special charger between your batteries and the supply? I got myself a bms but the manufacturer told me I have to buy a cv cc charger. I don't really get it :thinking:
[/quote]

I am using a BMS installed on the board and my power supply is CC/CV
It has to be Constant Current/ Constant Voltage to work properly
```

---
## \#12 Posted by: mrplaygood Posted at: 2017-03-09T23:42:19.457Z Reads: 137

```
Ah, okay. I thought it just would supply voltage or current and you have to switch manually between the modes.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-03-09T23:42:48.694Z Reads: 136

```
It switches automatically.
All you have to do is set the max voltage and current
like I said, It works like a dream!
```

---
## \#14 Posted by: mrplaygood Posted at: 2017-03-09T23:43:49.073Z Reads: 132

```
Just saw it under your post. I think I over read it...my fault 😕
```

---
## \#15 Posted by: Namasaki Posted at: 2017-03-09T23:47:48.669Z Reads: 133

```
The problem I was having is that my BMS would not start balancing until my 10s pack reached 42v and then the brick charger would turn off. 
At this very moment I'm charging my board. the pack is showing 42v but my power supply is still sending 55ma of current because the bms is balancing. When all the cells reach 4.2 the power supply output should be at zero.
Or I could stop it at 50ma and call it good enough.
```

---
## \#16 Posted by: mrplaygood Posted at: 2017-03-09T23:51:23.781Z Reads: 121

```
Do you have a link to your power supply? I have not bought the brick type charger yet because I'm still building up my board. But I think I could get the same scenario.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-03-09T23:57:58.962Z Reads: 123

```
I have 2 brick chargers. One is 2a the other is 5a both do the same thing. They cut off when my battery gets to 41.8 or 41.9v and never fully charge the battery.
The Power supply I got was a little pricey but not bad it was $179 +tax on Amazon
I posted a link earlier in this thread for one that is only $75 on Amazon
Mine is this one:
https://www.amazon.com/gp/product/B00G0HAY3U/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1
```

---
## \#18 Posted by: Namasaki Posted at: 2017-03-09T23:59:18.876Z Reads: 119

```
Here is the one for $75 Thats a real bargain for a 60v 5a supply.
 they both have CC and CV modes
https://www.amazon.com/dp/B01MQFCFMN/ref=cm_sw_r_cp_api_zuCWyb6VJC6PG
```

---
## \#19 Posted by: mrplaygood Posted at: 2017-03-10T00:01:08.011Z Reads: 116

```
Sorry it's to late here in Germany. I should get some sleep or I will over read even more links :P
```

---
## \#20 Posted by: moe_lester Posted at: 2017-03-10T00:12:48.518Z Reads: 122

```
Great thankz guys, i ended uo buying a 8s brick charger from America specifically for charging 8s lion pack at 4a. 

Thanks getting some real value from you guys
```

---
## \#21 Posted by: Aleximus Posted at: 2017-03-21T14:02:44.770Z Reads: 118

```
Hi guys!
Is it possible to use this regulator:
https://www.amazon.ca/Converter-Transformer-Regulator-Controller-Regulated/dp/B00E8D7XYG/ref=sr_1_6?ie=UTF8&qid=1490102218&sr=8-6&keywords=regulated+power+supply+60v

powered from 210w 19.5v laptop brick like this (I already have one)?
https://www.adapter-chargers.com/product/genuine-dell-19-5v-10-8a-210w-7-45-0mm-ac-adapter-power-supply/
I also have a good 550w PC power supply, but it is limited to 12v...

The thing is now I am working on dual motor build with 8s7p battery (with used laptop cells) for this summer, but for next year I am going to build a solid 12s battery with new high drain cells.
So I don't want to buy a charger to use it only for one summer and then put it on a shelf.
I would prefer to build a good variable power supply/charger to use for various projects...
Looking for your advice.
Thank you!
```

---
## \#22 Posted by: Maxid Posted at: 2017-03-21T15:06:00.977Z Reads: 112

```
Be careful - that is just a step down converter.
It says in the description:
[quote]You must make sure that the input voltage is 1.1 times higher than output voltage[/quote]

This makes this hard to use as you can't use any PSU and when you do have a lab supply you would not need this in the first place.

You should use this for your purpose (that is what I did):
http://www.ebay.com/itm/DC-DC-900W-0-15A-8-60V-To-10-120V-NC-Boost-Power-Supply-Module-CC-CV-LED-Driver-/182029384354?hash=item2a61cbfaa2:g:1gAAAOSwezVWxxrE
```

---
## \#23 Posted by: Maxid Posted at: 2017-03-21T15:18:05.733Z Reads: 107

```
read this thread (especially at the end it gets interesting and describes your plan):
http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902/
```

---
## \#24 Posted by: Aleximus Posted at: 2017-03-22T18:10:21.531Z Reads: 101

```
Thanks, That's exactly what I was looking for!
```

---
## \#25 Posted by: VAEsk8 Posted at: 2017-10-20T07:04:08.299Z Reads: 67

```
Hi man! What BMS do you use, and what charger did you find? :)
```

---
## \#26 Posted by: composites_r_awesome Posted at: 2018-06-22T19:05:44.532Z Reads: 50

```
Do those brick chargers cut off both with BMS and w/o BMS at 41,8v?  What would happen if the chargers do not cut off at 42? Could they just be 'dumb chargers' and idle at 41,8-42 like all night, and letting BMS balance all nice and dandy?  
  
Thanks!

Edit: Could I just use DC-DC 'universal' converter for normal charging to get my 42v charger to 40/41? and some time scer the converter to 42 for balancing?  
  
Like this[ 8.5-50v input - 10-60v output cheap Aliexpress DC-DC converter?](https://www.aliexpress.com/item/400W-DC-DC-Step-up-Boost-Converter-8-5-50V-to-10-60V-15A-Constant-Current/32858186482.html?spm=2114.search0104.3.69.5aa83a2axf7Wk0&ws_ab_test=searchweb0_0,searchweb201602_1_10152_10151_10065_10344_10068_10342_10343_5722611_10340_10341_10696_5722911_5722811_5722711_10084_10083_10618_10307_10820_10821_10303_10302_10059_306_100031_10103_10624_10623_10622_10621_10620_5722511,searchweb201603_12,ppcSwitch_2&algo_expid=140510b6-a928-47cb-8705-f22ce630a21c-10&algo_pvid=140510b6-a928-47cb-8705-f22ce630a21c&priceBeautifyAB=0)

Although they do mention something about for charging  you'd need this and that, in the description    
  
Oor just use a fully adjustable, probably €€€ bms from the start?[BesTech](http://bestechpower.com/communicationbms/BMS-D298V1.html)
```

---
## \#27 Posted by: composites_r_awesome Posted at: 2018-07-06T10:34:21.747Z Reads: 46

```
Namasaki, do you know whether if using a one of those 'dumb', [power supplies with voltage regulator (43-40v) on them](https://www.aliexpress.com/item/S-350-36-Low-noise-350w-dc-36v-output-SMPS-36v-350w-switching-power-supply/32818273743.html?spm=a2g0s.9042311.0.0.27424c4driNREI) and voltage on 41v, when do they cut off? Do they just idle all night at 41v after the battery doesn't take current in anymore? does a SuPower BMS make difference when charging with 41v with it?
Would it be possible to add a cut-off measures?

Thanks!
```

---
## \#28 Posted by: Namasaki Posted at: 2018-07-07T02:05:59.904Z Reads: 41

```
I use a Lab power supply to charge my batteries. 
If you use a power supply it should be a CC/CV power supply
Voltage is like water pressure
Current is like water flow
Current will only flow into the battery as long as the voltage in the battery is lower than the voltage your charging it with.
So when your charger is set to 41v and as your battery reaches 41v, the flow of current drops.
When I charge my batteries, my Vesc's are on so they take a littler current. 
So the current on my charger never drops below 50ma at full charge.
If your Vescs are not on during charge, then it's possible that your charge current would drop to zero at full charge.
So even though the charger stays on, it's not overcharging the battery.

I looked at the power supply your linked. It only outputs 36v
If I'm not mistaken, a regulator will reduce voltage output but not increase it so you'll need a supply with higher output.
```

---
## \#29 Posted by: composites_r_awesome Posted at: 2018-07-07T16:44:26.227Z Reads: 34

```
Yes that's what i wanted to hear, that although I could use timer, there wouldnt be anything bad happening if it would just idle at that 50mA

Haha yo yeah I had looked on too many different 10s/36v/42v chargers that I automatically though "hey that fine!"

Thanks
```

---
## \#30 Posted by: Namasaki Posted at: 2018-07-08T22:16:51.396Z Reads: 29

```
When the charge voltage and battery voltage equalize, current can no longer flow because the pressure being equal will stop the flow. If you do not have any load on the battery, Vescs on for example, the charge current should drop to zero.

Check out this video about charging a Lipo with a power supply:


https://youtu.be/0yhbof6_s64
```

---

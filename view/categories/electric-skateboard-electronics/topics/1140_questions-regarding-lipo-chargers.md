# Questions regarding LiPo chargers

### Replies: 22 Views: 3627

## \#1 Posted by: Andrew Posted at: 2016-01-28T19:03:12.747Z Reads: 245

```
I just bought two turnigy 3s 5000mah 20c lipos and im looking to buy a charger. Im looking to charger them im parallel and im a bit confused on the overall subject. Could anyone recommend a charger and balancing board that will suit my needs?
```

---
## \#2 Posted by: trbt555 Posted at: 2016-01-28T19:19:01.181Z Reads: 252

```
I own two [Imax B6][1] chargers and they have never failed me.
(you can easily find parallel balancing boards on HK too)

Bear in mind that by charging in parallel you'll double the charge time compared to a single pack. And you'll not be balancing individual cells but parallel sets of two. 

That's the reason I decided to start charging in series : it's faster and you're balancing individual cells. But you need to know what you're doing or you'll have fireworks. There are a few threads on series charging.

  [1]: http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=58285
```

---
## \#3 Posted by: laurnts Posted at: 2016-01-28T19:31:47.008Z Reads: 242

```
I agree with @trbt555 the Imax B6 is a good buy. Personally I use Turnigy Accucel series
http://www.hobbyking.com/hobbyking/store/__64345__Turnigy_Accucel_6_80W_10A_Balancer_Charger_LiHV_Capable.html

But it's not recommended because you will need to purchase additional power supply and the connectors to supply power to the balance charger are XT60, so you will need additional rewiring for it. So stick with the Imax B6.

I personally use 4 packs of the same batteries you have, 2 in series and 2 in parallels. Since you've only have 2 batteries, I recommend you to get http://www.hobbyking.com/hobbyking/store/__36290__Twin_pack_charge_lead_2_x_3S_6S_w_XT60_EU_warehouse_.html?strSearch=twin and charge series like @trbt555 said then you could have individual cell being balanced individually. However you will need this if you really really want to charge in parallel http://www.hobbyking.com/hobbyking/store/__27077__JST_XH_Parallel_Balance_Lead_3S_250mm_2xJST_XH_.html
```

---
## \#4 Posted by: Andrew Posted at: 2016-01-28T20:50:48.771Z Reads: 223

```
Does the imax b6 need a seperate power supply?
Also correct me if im wrong but from what it sounds like if i charge the 2 batteries in parallel then the 2 batterys will be balanced but the individual cells will not be balanced. 
So in my scenario it is better to charge them in series and all i would need would be the imax b6 and the harness to attach the two 3s battteries together nothing else correct?
```

---
## \#5 Posted by: torqueboards Posted at: 2016-01-29T01:59:40.193Z Reads: 203

```
I suggest invest in a decent high quality charger. iCharger 208B $120 and an HobbyKing 350W $40. You can charge up to 8S, charge in parallel and charge at up to 20 amps. :smile:
```

---
## \#6 Posted by: laurnts Posted at: 2016-01-29T02:37:03.728Z Reads: 196

```
[quote="Andrew, post:4, topic:1140"]
Does the imax b6 need a seperate power supply?
[/quote]

Well I don't think so. From the photo I could see the AC cable goes to the device, but for sure better wait for @trbt555 reply since I dont own the product.

[quote="torqueboards, post:5, topic:1140"]
I suggest invest in a decent high quality charger. iCharger 208B $120 and an HobbyKing 350W $40. You can charge up to 8S, charge in parallel and charge at up to 20 amps. :smile:
[/quote] 
@torqueboards I really do believe this is suggestion is really good up to one point. For instance, If you're planning to stay with lipo packs, decided to stay with it and experiment with higher charge rating like 4 - 5c then having such great charger and or with the power supply is a really good investment. Super fast charger are expensive and requires also expensive packs that capable of handling the high charging current.

Personally I'd like to improve the safety and the easy side of charging by using Li Ion Cells and a BMS. What does BMS do is to protect your battery from temperature, over charging and shorts. It also do balance charging for you by simply just plug a laptop adapter like to the BMS. Easy, neat and simple practice. But again it's a matter of preferences.
```

---
## \#7 Posted by: torqueboards Posted at: 2016-01-29T03:50:19.359Z Reads: 177

```
We'll you did say LiPo chargers :smile:

Also, you can always charge 6x packs in parallel and you won't need a 4-5c rating for your battery since it will be like 4S 30,000mah (5ah packs *6).
```

---
## \#8 Posted by: laurnts Posted at: 2016-01-29T04:43:03.676Z Reads: 174

```
[quote="Andrew, post:4, topic:1140"]
So in my scenario it is better to charge them in series and all i would need would be the imax b6 and the harness to attach the two 3s battteries together nothing else correct?
[/quote]

Yep, this is by far I belive as the best starter setup. If you have more experience and extra budget later, then going other path such recommended by @torqueboards is an option. But for now if you really aim to charge only those 2 battery packs you have now, imax and twin charging plug is all you need.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-01-29T06:14:48.415Z Reads: 168

```
You don't need a separate power supply if you get the iMax B6ac (ac = mains), the one I linked above.
```

---
## \#10 Posted by: Andrew Posted at: 2016-01-29T07:04:26.740Z Reads: 166

```
Any tips on charging my batteries in series safely?
Also, in order to charge that batteries in series i would use 10 amps correct? How long would it take to charge?
```

---
## \#11 Posted by: trbt555 Posted at: 2016-01-29T10:03:13.721Z Reads: 162

```
Always keep the same packs in series for riding and for charging.
Use the correct harness, refer to my [schematic][1] if you're not sure.
Number them so you don't get them mixed up. Also number the balance leads.

As long as you don't exceed the max charge current for your batteries, you're OK.
I believe the ones you mentioned are 2C = 2 x 5A = 10A max.

The iMax B6 is a 50W charger, so it will be able to charge your 2 x 3S 5000mAh packs in a little over two hours:
Series pack voltage = 2 x 3S = 22.2V
Energy contained in pack = Volts x Capacity = 22.2V x 5Ah = 110 Wh

To charge 110Whs with a 50W charger you'll need 110/50 = 2.2 h.

I suggest you read up intensively on Lipo charging and such.
Here are some useful links:

 - [A guide to understanding lipo batteries][2]
 - [Lithium Polymer Etiquette: A Comprehensive Guide to Working with LiPo][3]
 - [Understanding wattage in relationship to charging][4]


  [1]: http://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734/9?u=trbt555
  [2]: http://www.rogershobbycenter.com/lipoguide/
  [3]: http://www.instructables.com/id/Lithium-Polymer-Etiquette/
  [4]: http://www.tjinguytech.com/charging-how-tos/wattage-for-charging
```

---
## \#12 Posted by: Andrew Posted at: 2016-01-29T16:08:43.975Z Reads: 144

```
That was very helpful thank you! 
Hopefully one last question, according to your schematic it seems like i need a y-type harness to connect to the "charge". Is that correct?
```

---
## \#13 Posted by: Andrew Posted at: 2016-01-29T16:11:25.429Z Reads: 137

```
Something like this?
https://jet.com/product/detail/90d3a13e96f54276b703d2ce3354c321?jcmp=pla:ggl:toys_games_a3:toys_remote_control_toy_accessories_a3_other:na:na:na:na:na:2&code=PLA15&k_clickid=3150aaab-55cb-4ab2-af5f-5dd50478cfcf&abkId=403-82457&gclid=CjwKEAiAuKy1BRCY5bTuvPeopXcSJAAq4OVsDzINxQb8g4GQQAtbEh_9Rufg04OgU7oAZ4b4l_3jkxoCR6Xw_wcB
```

---
## \#14 Posted by: paragon Posted at: 2016-01-29T17:07:04.268Z Reads: 133

```
I've been happy with the accucell 6 which Hobbyking sold for $5 on black friday.
```

---
## \#15 Posted by: trbt555 Posted at: 2016-01-29T18:50:20.901Z Reads: 135

```
A Y-harness is a parallel harness.
You need a [series harness][1].

Series charging is not really advisable for complete newbies, you might want to charge your lipos separately at first, until you get more experience and confidence.



  [1]: http://www.hobbyking.com/hobbyking/store/RC_PRODUCT_SEARCH.asp?strSearch=Series+harness
```

---
## \#16 Posted by: laurnts Posted at: 2016-01-29T22:41:31.975Z Reads: 131

```
[quote="Andrew, post:1, topic:1140, full:true"]
I just bought two turnigy 3s 5000mah 20c lipos and im looking to buy a charger. Im looking to charger them im parallel and im a bit confused on the overall subject. Could anyone recommend a charger and balancing board that will suit my needs?
[/quote]

Since you only have 2 packs of 3s 5000mah lipo, you can connect with the twin charging 6s without danger of shorting. I believe @trbt555 is concern about charging in both series and or parallels with more than 2 battery packs.

---

This harness is what you need
http://www.hobbyking.com/hobbyking/store/__10993__Twin_pack_charge_lead_2_x_3S_6S_w_XT60.html

So you can connect both balance plug from the battery packs into this harness, from 2 3S into 1 single 6s. This harness also provide you with additional XT60 connectors. Easy!
```

---
## \#17 Posted by: Andrew Posted at: 2016-01-31T02:25:43.461Z Reads: 126

```
Thank you. Bit off topic question for you guys with more knowledge of diy skateboards.
Im looking into getting a wireless controller for my first build and ive been looking at the wiiceiver since the beginning of this build. It seems to be a bit harder to find a wii nunchuck type controller than i thought. I dont necessarily need the nunchuck but i want a smaller controller than fits in my hand and is not the traditional gun looking bulky controller. 
I know that diy skateboard.com had the reciever board but not the actual nunchuck.
Please let me know if you guys know where i could buy this smaller type of controller
```

---
## \#18 Posted by: laurnts Posted at: 2016-01-31T02:30:51.674Z Reads: 128

```
There are some you could get I believe best fits for your scenario.

Wii Nunchuck Nyko Kama with VESC. Just need some rewiring and good to go, best way if you already VESC in the first place. Anywhere you could get one of this pretty easy I guess.

If you have budget, contact @onloop for his Enertion Wireless Controller. Looks very promising. Ship from Australia.

If you still like the 2.4GHZ connectivity of a remote but not the bulkyness, you could also contact @chaka for his Ollinboard G2TB badwolf ready use remote. Ship from US.

Or you could also get the small torqueboards remote (the small 2.4GHZ pistol remote), I believe you can contact @torqueboards for it. Ship from US as well.
```

---
## \#19 Posted by: barajabali Posted at: 2016-01-31T03:29:41.006Z Reads: 118

```
I use the prophet pro sport duo. Charges two packs at the same time at up to 6 amps each. Doesn't over charge, has a cooling system and knows when a battery is unsafe to charge and provides an error message on why and how to fix
```

---
## \#20 Posted by: Andrew Posted at: 2016-01-31T07:25:08.260Z Reads: 113

```
What is the benefit to having the additional xt60 cable on that adaptor?
```

---
## \#21 Posted by: laurnts Posted at: 2016-01-31T07:50:42.164Z Reads: 114

```
You can dedicate that twin plug series charging harness especially for charging. So the main power cable that connects the battery with the ESC can stay and doesn't necessarily to be unplugged (though I believe it's best to disconnect everything from the battery while charging). Just added convenience.
```

---
## \#22 Posted by: Conman Posted at: 2017-11-06T19:59:00.113Z Reads: 29

```
So I’m in a similar boat where I don’t quite got a great plan for my setup.  5s 4000mah x 4.
I bought a HTRC 80W B6 V2 RC Balance Charger Discharger with Power Supply 15V 6A AC Adapter
and trying to think my best choice is.  (Fastest/safest/with lipos)
```

---

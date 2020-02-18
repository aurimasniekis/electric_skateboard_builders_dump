# First try eSK8 build

### Replies: 20 Views: 1020

## \#1 Posted by: Markuss Posted at: 2018-03-19T12:48:42.624Z Reads: 228

```
**​**
**Hello everyone,** 
after I informed myselfe a bit I’m finally ready to start my first E-Board build, but frankly am unsure if all parts work together so I am hoping to get help from this awesome community!

**motormount and pullys**: , eskating.eu, electricboardsolutions.com or trampaboards.com any recommendations?
**motor:**
APS 6374S 200KV, APS 6384S 200KV has more power but the price is almost similar, Torque Boards 6370 190KV or simply SK3 6374 192KV. what do u guys say?
**Battery**: 10s3p with Samsung 30Q
What´s the difference between those two? https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html and https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah-button-top.html
**BMS**: http://www.batterysupports.com/36v-3...bms-p-267.html
when building the battery pack is it better to conect the cells via a spotwelder and nickel strips or would it also workout with that https://eu.nkon.nl/accessories/welding-material/vruzend-diy-battery-kit-2759.html
**power Switch**:
https://eskating.eu/product/anti-spark-power-switch/, how much amps do I need?
**VESC**:
I´m thinking of buying the vesc from diy or do you recommend a other one?

_Thanks for helping_
```

---
## \#2 Posted by: dg798 Posted at: 2018-03-19T12:52:13.026Z Reads: 203

```
Ok so before I give recommendations are u looking for speed or torque?
```

---
## \#3 Posted by: dg798 Posted at: 2018-03-19T12:52:28.083Z Reads: 194

```
That’s what’s going to determine what parts would be best suited for u
```

---
## \#4 Posted by: Markuss Posted at: 2018-03-19T15:23:42.516Z Reads: 173

```
I know that you can´t get both but I’m trying to build a board which reaches about 50 kmh and can also go up stepper hills. I know that you can´t get both but I’m trying to build a board which reaches about 50 kmh and can also go up steeper hills.
```

---
## \#5 Posted by: ZackoryCramer Posted at: 2018-03-19T15:48:11.220Z Reads: 159

```
Dual 6374 190kv, you would want to picked a high p for your battery pack though.
```

---
## \#6 Posted by: Acido Posted at: 2018-03-19T16:22:41.535Z Reads: 151

```
I do no think his budget it that high..

I would recommend getting a Focbox and any motor that's 6374 for mono. 220kv tops if you ask me
```

---
## \#7 Posted by: gee Posted at: 2018-03-19T18:52:07.042Z Reads: 128

```
Your weight is a factor into building your first electric longboard. 
I'd say buy [this.](https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html)
Mount and pulley you can find one on amazon for a cheaper price I think. 
VESC from DIY but I'd say enertion. 
To be honest with you. I'd go for HUBs. 
Check this site out tho. They have bunch of good stuff. http://www.diyeboard.com/
```

---
## \#8 Posted by: Markuss Posted at: 2018-03-20T23:25:35.918Z Reads: 113

```
Thanks for all the help
so fist of all my weight is about 75kg and i would prefer Shops in EU cause its cheaper delivery.
I thought that HUBs arent´t as fast and powerfull as the belt and pully system. Any recomondations than?
So i guess a 6374 motor is by best bet than but just for interest why no 6384, they have more power don´t they?

whats with the batteries, BMS and power switch

what is the main difference about the diy vesc and a focbox?
```

---
## \#9 Posted by: ZackoryCramer Posted at: 2018-03-20T23:38:34.622Z Reads: 110

```
[quote="Markuss, post:8, topic:49509"]
why no 6384
[/quote]

You mean this: :smirk: ?
http://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-170kv-4000w/
```

---
## \#10 Posted by: dg798 Posted at: 2018-03-21T00:35:35.802Z Reads: 93

```
Focbox is for fox hence the name focbox. Running a diy vesc on foc is risky. There are many EU group buys for bms. U can use an anti spark xt90 as on off or a vedders anti spark switch.
```

---
## \#11 Posted by: b264 Posted at: 2018-03-21T00:38:19.601Z Reads: 92

```
What is your budget?
```

---
## \#12 Posted by: abenny Posted at: 2018-03-21T00:45:18.347Z Reads: 92

```
those vruzend battery connectors wont work as they wont be able to handle the current you're looking to push... however they recently posted that they're working on a version that will have higher capabilities and to look out for more info in the next few weeks
```

---
## \#13 Posted by: Markuss Posted at: 2018-06-04T17:23:08.068Z Reads: 73

```
thanks for the help guys :smiley:

i do have a nother question and hope u can help

i´m thinking of buying the focbox for a dual setup and i wanted to aks if it it is hard to do all the programming stuff and how the two focboxes workes together. Do i have to conetct 2 remote receivers and 2 bluetooth modules, so one each?  Or would it be easier to wait for the focbox unity?
```

---
## \#14 Posted by: rey8801 Posted at: 2018-06-04T19:11:21.568Z Reads: 60

```
There are plenty of tutorial on how to configure you lr vesc. One even using focbox https://youtu.be/v1glLDO-EjA (it's the same BTW). For the other question you can decide to go for a can bus connection and in this case receiver connect to the master VESC and the slave VESC connected to the master VESC via can. Only one Bluetooth module to the master VESC. Differently you could opt for split the receiver signal. Then servo cable (the one from the receiver) to both of the VESC. On one vesc you cut the 5v wire to the receiver (the receiver needs 5v only from on e esc otherwise it will blow up). In this case you will need two Bluetooth modules if you want to control the vescs setting through the smartphone app. If you want just telemetry data one bluetooth is fine.
```

---
## \#15 Posted by: Markuss Posted at: 2018-07-17T01:01:13.225Z Reads: 53

```

what kind of nickel strips are the best for spot welding  a 12s4p battery? And what kind of wires are most likely to use to connect the battery with the anit spark and what for connecting the bms with the battery or are there already kabels included and what should i use to power up the bms?
By the way what BMS could u guys recommend using a 12s3p or 12s4p ? living in Germany if that matters
And last thing is, at https://eu.nkon.nl/ thy´ve two Q30 batteries with 2€ difference. Whats the difference between those. They´re looking pretty similar to me

thanks for helping
```

---
## \#16 Posted by: rey8801 Posted at: 2018-07-17T03:51:03.945Z Reads: 50

```
Hi, 
10mm x 0.15 nickel strips are the most use. Also nklon sell it usually. Depends on the battery diagram consider to use copper brail or thick silicon wires to make the series connection. 12 awg silicon wire should be fine, 10 awg if you want it more efficient (less heat) since the resistance inside drops. It is less flexible though. 
This is the battery cell you are looking for https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html.
BMS 12s bestech can be discharge as well. I saw someone selling one on the forum a new one now (you need to buy 2 of them each time, it's annoying). Otherwise a smaller one for charge only, depends what you want.
Also buy insulation paper and insulation 0-ring for the cells + side. Kapton tape. Optional shrink tube. XT90 for sure for a 12s or similar high amp connectors.
I think it's all to start. Good luck!

Edit: so now about BMS wiring. Usuay BMS comes with the balance wires. To connect the charging branch to the BMS and battery thinner cable are fine. I think I used 26 awg.
```

---
## \#17 Posted by: Markuss Posted at: 2018-07-17T20:25:33.048Z Reads: 39

```
[quote="rey8801, post:16, topic:49509"]
BMS 12s bestech can be discharge as well. I saw someone selling one on the forum a new one now (you need to buy 2 of them each time, it’s annoying). Otherwise a smaller one for charge only, depends what you want.
[/quote]
So if i want to buy one i have to get two? which one can u recomend, there´re so much and what "Continuous Current" do i need? whats with the BMS´s at http://www.batterysupports.com ?
What do u mean with getting a smaller one for charge only, thought the hole part of a bms is charging the battery?

[quote="rey8801, post:16, topic:49509"]
battery diagram
[/quote]
what battery diagramm do u mean?

thanks
```

---
## \#18 Posted by: rey8801 Posted at: 2018-07-17T20:36:55.587Z Reads: 37

```
Like flat, double stacked pack. Based on that you will have different nickel strips configurations. For instance a 10mm x 0.15 mm nickel strip is rated about 15A, so based on your battery configuration you would need to double or triple the layers, add silicon wire or copper braid (usually in case of flat pack). Differently for double stacked pack you can apply more single layer of nickel strips at the level of the series connections to distribute the load between cells.
```

---
## \#19 Posted by: Markuss Posted at: 2018-07-17T20:45:52.868Z Reads: 37

```
ahh okay :sweat_smile:

and what do u thing with the BMS?
```

---
## \#20 Posted by: rey8801 Posted at: 2018-07-17T21:01:03.066Z Reads: 35

```
I start using both charging discharge BMS. Then I had problem with the discharging part cutting off the board when battery fully charged (regenerative brakes give back current to the battery and BMS shut off momentary to protect the battery). Result I fall at 30Km/h...since then I use it for charging only. So if you want to go for discharge also I advice a nice BMS as Beshtech that you can customize the values, or buy a cheaper charge only BMS rated for your battery size,
```

---

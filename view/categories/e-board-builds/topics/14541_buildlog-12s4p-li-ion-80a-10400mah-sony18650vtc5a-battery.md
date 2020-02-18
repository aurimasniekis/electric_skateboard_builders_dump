# BUILDLOG: 12s4p Li-Ion 80A 10400mAh (Sony18650VTC5A) battery

### Replies: 17 Views: 2183

## \#1 Posted by: 3sly Posted at: 2016-12-12T10:19:47.850Z Reads: 253

```
Hello everyone!

I'm back, and tired of running my Multistar LiPo's to failure. (3*4S 10000mAh 10C)
So I have some cash and am willing to make myself a sweet 12s4p battery pack

Here are the parts thus far:

* 48 x €5,05: US18650VTC5A Sony Cells (35A/2600mAh) (nkon.nl): **Arrived**
* 3m x €3: 10mmx0.15mm Pure nickel strip (nkon.nl): **Arrived**
* €4,60: [50 pcs of battery holders](https://nl.aliexpress.com/item/Consumer-Electronics-Shop-Free-shipping-1-SET-50x-18650-Battery-Spacer-Radiating-Shell-EV-Pack-Plastic/32601474267.html?spm=2114.13010308.0.0.ifv4hD). I'll probably have to file down the tabs to accomodate the 10mm nickel strips: **Arrived**
* €50: [BMS 12S 80A](http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html). Should be plenty right for a single 149kV 6374? **Ordered**
* 10€: 3 antispark chaka/vedder 1.4 boards: **Arrived**
* 5€: Heatshrink aliexpress: **Arrived**
* ~20€: Parts for 3 antispark boards from Farnell + miscellaneous: **Arrived**
* 50€: [CLG-150-48A](https://www.elpro.org/gb/150-w-ip65/35114-clg-150-48a.html): is normally 48V but I found out it can be adjusted up to 56V: **Arrived**

**If anyone wants to go over this list for feedback, let me know! I don't think I forgot anything?**

I'm excited! Hopefully this will help others as well
Dries

<img src="/uploads/db1493/original/3X/4/6/4672d534658f899587ae2465077af991687d0d64.jpg" width="666" height="499">
```

---
## \#2 Posted by: rwxr Posted at: 2016-12-12T14:24:10.791Z Reads: 213

```
What are you going to weld the batteris with?
```

---
## \#3 Posted by: 3sly Posted at: 2016-12-12T17:51:44.845Z Reads: 197

```
probably spotwelding. But I hope I can lend one from someone I know, as I'm not yet isnterested to invest in one :p
```

---
## \#4 Posted by: 3sly Posted at: 2016-12-12T23:17:04.650Z Reads: 189

```
I'm about to order the BMS, is it appropriate for my purpose usage? I'm assuming it is. Some final feedback is welcome ;)

A second question. Do you guys always test the cells? Even if they come from a reputable source? Or just a quick check of the voltage?
```

---
## \#5 Posted by: Sander Posted at: 2016-12-13T17:41:16.103Z Reads: 174

```
If I were  you I would probably take some capacity testing some, like 10 and if they are all the same(But if it was me I would do a test on all of them! Because if one has less capacity like 2500mah and the others 3000mah it can destroy all the batteries in that serie and worst case scenerio fire.).
Because the site you ordered from has a LG battery of 20A with 3000mah. And there were a review about it was actually 2700mah not 3000mah. But maybe, just maybe he didnt charge them before discharging.
```

---
## \#7 Posted by: 3sly Posted at: 2016-12-13T20:04:18.702Z Reads: 161

```
Thanks for the heads up! I'll definately do that then. I'll make sure I charge them to the same voltage first
```

---
## \#8 Posted by: 3sly Posted at: 2016-12-19T16:28:33.607Z Reads: 166

```
Hey guys. Batteries and nickel arrived! About to start some testing. 

Small question though: anyone know of a good charger that I can use to charge the end product?

 <img src="/uploads/db1493/original/3X/4/0/406a16c87dc11f340a1168eca8eb704dddb526ae.jpg" width="375" height="500">
```

---
## \#9 Posted by: lox897 Posted at: 2016-12-19T22:01:45.240Z Reads: 152

```
SuPower or Meanwell are good chargers. Some Meanwell can even change the output voltage which is great if you want to charge to 4.1v per cell to give them a greater life.
```

---
## \#10 Posted by: 3sly Posted at: 2016-12-20T12:12:09.339Z Reads: 146

```
Ah thanks! seems like meanwell is pretty common.
But then I have a second question for which I can't seem to find an answer:
Does the charger voltage dictate the cell voltage (chargerV/12)? Or does the BMS up/downstep the input voltage as to set each cell at a certain voltage?
```

---
## \#11 Posted by: lox897 Posted at: 2016-12-20T12:24:33.764Z Reads: 142

```
Assuming you are using 12S you will want a 50.4v charger. The bms kind of splits that by 12 and charges each parallel set of cells. So yes, the charger dictates the cells voltage.
```

---
## \#12 Posted by: 3sly Posted at: 2016-12-21T13:31:40.417Z Reads: 135

```
Ok, found one!

Anyone an experience with these? http://www.ebay.com/itm/50-4V-2A-Power-Adapter-For-Self-Balanced-Vehicle12S-Li-ion-Battery-Charger-Plug-/291922334252?hash=item43f7ed522c:g:WNsAAOSwo4pYD1ks

The meanwell ones seem decent, but with import taxes they will cost me 50€ more :( , any thoughts if it's worth it?
```

---
## \#13 Posted by: lox897 Posted at: 2016-12-21T20:16:33.087Z Reads: 132

```
Usually, if we aren't getting MeanWells we will be getting BatterySupports. The ones on ebay may be risky. I wouldn't trust it, if you are paying the extra money at least you know your house isn't going to burn down. This is not the kinda product you go cheap on. So I'd say get a battery supports.
```

---
## \#14 Posted by: 3sly Posted at: 2017-01-07T22:45:15.636Z Reads: 118

```
Ok guys. Big update and a lot of pictures coming soon. 

Question though: I have some do but about the testing the capacity of the cells using the imax b6ac (genuine).  The charger indicated the cells voltage at 3.4v! Even though when measuring them with the multimeter they are at 3.65 volts. That difference is a bit too big for me as I'd like to keep them below 4.1v when fully charged. Is this normal?
```

---
## \#15 Posted by: Pedrodemio Posted at: 2017-01-07T23:43:27.813Z Reads: 110

```
This voltage is with the charger doing what? charging or discharging? this is just a single cell?
```

---
## \#16 Posted by: 3sly Posted at: 2017-01-08T15:17:51.563Z Reads: 104

```
yes, charging. But the same voltage is displayed if I use the 'battery meter' mode of the charger (not charging). Yes, one single cell. I don't really dare to charge the cells anymore, because when they had 3.9 according to the charger (while charging), it already had 4.1V when I checked with a mm
```

---
## \#17 Posted by: Pedrodemio Posted at: 2017-01-08T15:37:14.298Z Reads: 99

```
There is a calibration menu, but i think its too far off to be correcteted, if thats not enough you could switch the battery type to Li-Ion(4,1) and see if thats keep under 4,2V on the full charge https://www.rcgroups.com/forums/showthread.php?827821-iMax-B6-service-menu
```

---
## \#18 Posted by: 3sly Posted at: 2017-01-09T18:31:14.745Z Reads: 87

```
Well as promised a big update. Almost everything has arrived and is ready to go. I decided last minute to make a 12s4p battery as I'd like to make this battery future proof, and who knows maybe one day I'd go for a dual carvon setup. For this purpose a 80A BMS should certainly suffice. 

I still have to solve the problem with my imax :( so I can start testing the cells. But I'm about to start on the chaka switch. I have enough for 3 sparkswitches, so I might sell the others as kits.
```

---

# Magnetic Charge Port

### Replies: 19 Views: 2442

## \#1 Posted by: spannepacker Posted at: 2018-01-11T19:41:21.088Z Reads: 444

```
I have been using a 5.5mm barrel jack (the default on the [charger](https://www.ebay.com/itm/50-4V-2A-Power-Adapter-For-Self-Balanced-Vehicle12S-Li-ion-Battery-Charger-Plug/291922334252?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649) I have been using) but am looking for a more reliable and cleaner solution. I am currently running my board at 12s with a 12s SuPower BMS. I have had to replace my 5.5mm port on the board side twice now due to sparking and grit getting in (any ideas why I would get a spark with a BMS?). While my board is out of commission from a fried anti spark (wrong order of operations when installing) and failed charger (no idea), I thought I would start exploring what it would take to build a simple magnetic charger that can withstand a high current.

I have seen a [few people use Apple MagSafe connectors](http://www.electric-skateboard.builders/t/magsafe-as-charge-port/13458/24) with good results, but they are definitely pushing the limit of those small pogo pins. 

One high wattage option are the [RoPD Connectors](http://www.rosenberger.com/en/products/automotive/ropd.php) that are becoming more standard in the ebike community. But between the price and my inability to make things easy for myself, I decided to start ordering the parts to make my own:


High current probes:
https://www.ebay.com/itm/5Pcs-16mm-Lenght-Spring-Loaded-Contact-PCB-Testing-High-Current-Probe-Terminal/322523817883?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2648
<br>


Copper rods as contacts on the board side:
https://www.amazon.com/gp/product/B07125HMM2/ref=oh_aui_detailpage_o09_s00?ie=UTF8&psc=1
<br>
And some little pieces of magic in solid form:
https://hobbyking.com/en_us/n35-2-2-5mm.html

<br>

Goals:
-A nice click when connecting
-Reversible direction (180 degrees)
-Redundant pins for higher currents
-Low profile on both male and female connectors
-Waterproof female (board side) port
-Magnetic board side port cover?


I still have some modeling and printing to do. I will check back with updates...
```

---
## \#2 Posted by: Maxid Posted at: 2018-01-11T20:35:11.386Z Reads: 408

```
How are we pushing the limits of those pins? I use less current than Apple does
```

---
## \#4 Posted by: spannepacker Posted at: 2018-01-11T21:08:54.981Z Reads: 388

```
From what I can tell from your posts (and assuming you are charging at 2A with 41V) your setup is just below the 85W that Apple uses the connector at. Please correct me if I’m wrong. My board needs to charge at 50.4V with the hopes of a 3A or 4A charger in the future. With my current 2A charger, I would be pushing 100W.

You mentioned that the charger got a bit warm at 30V which could be normal operation… but I am interested in building a beefier (definitely overbuilt) version for science.

Your build looks beautiful by the way. I hope I can pull off a subtle charge port like that.
```

---
## \#5 Posted by: Pimousse Posted at: 2018-01-11T21:45:18.216Z Reads: 356

```
I love this idea !!
Thanks for sharing ! I spent a LOT of time trying to find those Apple magsafe spring connectors but I found only very expensive parts.
So I keep a very interested eye on your project ! :slight_smile:
```

---
## \#6 Posted by: Maxid Posted at: 2018-01-11T21:48:33.557Z Reads: 336

```
Only the current matters (at least with those voltages) - so Apple does 4A while we only use 2A - so well below the maximum for that plug. It only gets warm because the control ICs Apple uses burn up at the voltage. Once they are cooked you don't feel anything getting warm anymore.
```

---
## \#7 Posted by: spannepacker Posted at: 2018-01-11T22:35:05.011Z Reads: 312

```
Gotcha. It had crossed my mind that only current matters when considering wire gauge. How has the MagSafe setup been working for you? Does the magnet pick up any particulate over time?
```

---
## \#8 Posted by: bimmer Posted at: 2018-01-11T22:40:30.107Z Reads: 297

```
Say you build this and it gets wet.... your Batteries will drain or if the water is salty  it will spark,
```

---
## \#9 Posted by: Idle Posted at: 2018-01-11T22:50:55.930Z Reads: 306

```
Those magnets are cheap.
Hk is weird...they sell silicone lipo protectors for one penny each.
```

---
## \#10 Posted by: spannepacker Posted at: 2018-01-11T22:56:50.450Z Reads: 302

```
The charge port is not connected directly to the batteries. I am using a BMS so there should not be any hot terminals until its plugged in. That being said, I may have an integrated magnetic cover that will keep it clean.
```

---
## \#11 Posted by: bimmer Posted at: 2018-01-11T22:58:00.702Z Reads: 295

```
You should take a multi meter to your charge  ports and see  if they're "hot".
```

---
## \#12 Posted by: GhettoFab.rictation Posted at: 2018-01-25T19:56:03.775Z Reads: 269

```
I think if he just makes a magnetic cover with an o-ring on it he'll be just fine.
Edit needs to make everything water proof anyway. The charger port needs the seal on it as well. It isn't hard to make?
```

---
## \#13 Posted by: spannepacker Posted at: 2018-01-29T18:35:04.791Z Reads: 249

```
I had in the past, but just did again now that my board is back in working condition. I was totally wrong. The contacts in the barrel connector are live. I think I had previously incorrectly metered the external surface of the barrel connector and not the internal contact.
```

---
## \#14 Posted by: spannepacker Posted at: 2018-01-29T18:37:03.357Z Reads: 249

```
The charge port I'm working on will be plenty water resistant to keep water out of the board, but I will definitely need to come up with a simple solution to cover the charge port itself.
```

---
## \#15 Posted by: spannepacker Posted at: 2018-03-14T21:46:35.122Z Reads: 226

```
Unfortunately my access to prototyping facilities is changing soon and I will be focusing on finishing up my new build in the short amount of time I have. For now I will be testing out the MagSafe solution at 2A but hope to circle back to continue working on the perfect charge port.
```

---
## \#16 Posted by: totalgeek9224 Posted at: 2019-03-26T10:39:39.536Z Reads: 124

```
Have you been able to give some thought to this recently?
```

---
## \#17 Posted by: Winfly Posted at: 2019-03-26T14:33:05.964Z Reads: 108

```
I've found some good stuff from a manufacturer. Advertised 6 A capable but a MOQ sample of 5 pairs runs about $90 to land in the us. Fml.
```

---
## \#18 Posted by: Surfer Posted at: 2019-03-26T14:57:41.514Z Reads: 104

```
I can get a pair to make things going, it will be nice to post some pictures.
```

---
## \#19 Posted by: Chalupa_Batman Posted at: 2019-03-26T22:46:05.813Z Reads: 86

```
has any one seen [These](https://www.alibaba.com/product-detail/Wholesale-Promotional-Waterproof-Usb-Fast-Connector_60769676622.html?spm=a2700.7724857.normalList.51.e1af2cebjT45ps) might work well. only 3A rating but would work for 10s and 12s
```

---
## \#20 Posted by: totalgeek9224 Posted at: 2019-03-27T05:59:25.199Z Reads: 79

```
Yeah, someone (i forget who) was trying to experiment with them but in his trials they kept sparking
```

---

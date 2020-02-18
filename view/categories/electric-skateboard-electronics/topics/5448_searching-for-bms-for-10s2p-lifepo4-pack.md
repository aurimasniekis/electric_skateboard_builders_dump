# Searching for BMS for 10s2p LiFePo4 pack

### Replies: 2 Views: 898

## \#1 Posted by: ndwallick Posted at: 2016-07-02T00:52:39.881Z Reads: 81

```
Hi everybody, I have recently started my second build and one of my goals is to be able to charge it really easily and not have to worry about cell balancing, keeping it at a storage charge, or it lighting on fire. So I have ordered 5 HK Zippy 3600 mAh 2s2p LiFePo4 battery packs (still shipping).

I want to be able to charge it easily with a laptop style charger, so I began searching for a BMS and I am having trouble finding one for 10s LiFe.

**Here are some questions I'm trying to answer:**

Do I need to discharge through the BMS or can I bypass it? (so I can use a BMS rated for a lower discharge rate) (my motor will pull 65 amps max)

can I use a 12s BMS for 10s? (most I've found skip 10s)

Is it easy to make a BMS out of transistors and resistors etc? (I have soldering equipment and have made a few circuit boards before)


**Here are links to the electronic parts I have ordered (still shipping):**
batteries (5): http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=14062
Vesc from Ollin: http://www.ollinboardcompany.com/product/vedder-s-speed-controller
190 KV motor: http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=18181

Thank You!!!

ohh ya and heres a pic of my board so far:
<img src="/uploads/db1493/original/2X/a/ab36444874f5c38649d43b94fe4c3a450b152348.JPG" width="666" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-02T08:03:56.321Z Reads: 63

```
Nice, you had the exact same setup as me with the Arbor Axis and purple kegels, until I found that it was too flexy for my space cell pro.

You can discharge straight from battery, and use the BMS to balance charge, you just won't have the added benefit of the BMS's over current protection, which isn't a huge deal if you're using a fuse. I think you can use a 12S BMS for a 10S setup if you plug it in right, but don't quote me on that. It seems less trouble to just go regular li-ion lipo's if you're cost conscious. Personally I'd go LiFePo4 with 26650 cells.
```

---

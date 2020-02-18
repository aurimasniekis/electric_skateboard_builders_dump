# Battery Monitors how low to go?

### Replies: 3 Views: 909

## \#1 Posted by: dstnceswmer Posted at: 2016-10-25T20:38:22.730Z Reads: 110

```
So random question regarding those LCD battery Monitors people have been putting in their builds. I have see that you never want your lipos to go below a certain voltage level (3V/cell I think it was) My question is these battery monitors, does that save level correspond to 0% on the screen? Or do I have to pay attention and stop riding at say 20%? Also would the board keep function beyond that minimum voltage cutoff? As in could I accidentally ride my board too long until the batteries become unstable and dangerous? If it makes any difference I have a VESC and a 60A BMS in my setup. 

This is the monitor I was reffering to: http://www.ebay.com/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-25T20:51:32.524Z Reads: 111

```
This is an approximation of how voltage level corresponds to meter %. You'll have to check the datasheet of your batteries, but lipos lower voltage limit tends to be higher than li-ion.

<img src="/uploads/db1493/original/3X/c/d/cd28e21a324ca4ab755a2046abf6a5d09f73e086.png" width="586" height="196">
```

---
## \#3 Posted by: mmaner Posted at: 2016-10-25T21:30:11.525Z Reads: 98

```
If you are looking at the [DROK DC8-63V](https://www.amazon.com/gp/product/B00VUUKIMY/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1) Volt Meter, which is what most people use, you can switch it from percentage to voltage on the display.

I usually charge my cells to 4.2v & run them to 3.6v (@ 6s total voltage = 25.3v top to 21.6v bttom).

There are 2 styles (I didn't say model, because the model numbers are the same).  On both styles, you have to solder a [button](https://www.amazon.com/uxcell-6x6x4-3mm-Momentary-Tactile-Through-Hole/dp/B0090VQK7C/ref=sr_1_1?ie=UTF8&qid=1477430676&sr=8-1&keywords=uxcell+50pcs+6x6x4.3mm+Momentary+Tactile) on the front.  On the old style, you have solder points on the back that you bridge for different functions.  On the new style, its all done with the 2 back buttons and the front button.  

Here's a [youtube](https://www.youtube.com/watch?v=py_LKc1Zt7w) video of the old style.
```

---

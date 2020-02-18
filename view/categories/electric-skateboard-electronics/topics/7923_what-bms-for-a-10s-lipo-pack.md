# What BMS for a 10S lipo pack?

### Replies: 5 Views: 1149

## \#1 Posted by: jallart Posted at: 2016-08-19T21:31:44.823Z Reads: 158

```
Hi guys, 
Do you have any BMS to advice for a 10S lipo pack ? 
I had this one : http://www.batterysupports.com/36v-37v-42v-10s-45a-10x-36v-lithium-ion-lipolymer-battery-bms-p-266.html but i got some output voltage issues on the one i received, so i am looking for another one...
Is this one ok for lipo too ? https://fr.aliexpress.com/item/New-Battery-Protection-BMS-PCB-Board-for-10-Packs-10s-36V-Li-ion-Cell-max-30A/32574042165.html?spm=2114.13010608.0.73.86szDe
If you have some other one to suggest,dont hesitate ! :D
Thanks !!
```

---
## \#2 Posted by: makevoid Posted at: 2016-08-20T02:14:34.782Z Reads: 135

```
Those are both for li-ion cells, lipos have a slightly different charging curve so I don't know if they're optimal.... Also the second is not rated very high (45A the first one and less the second 30A) so if you have/get a bms with that low discharging capacity (30A) you should really using it for charging only, bypassing it for discharge. The 45A is probably ok but I would go with one with more capacity maybe (I have the 60A and I'm using it with li ion cells)
```

---
## \#3 Posted by: jrpwit Posted at: 2016-08-20T02:23:10.492Z Reads: 127

```
Get at least a 60 amp. Batterysupport is great!
```

---
## \#4 Posted by: jallart Posted at: 2016-08-20T08:13:53.395Z Reads: 113

```
So for you both could work with lipo cells ? 

Gonna try to find a diagram somewhere to know how to bypass the BMS for discharge coz i dont know how to do it...
```

---
## \#5 Posted by: makevoid Posted at: 2016-08-20T08:23:24.282Z Reads: 107

```
I'm saying that that shop, SuPower, sells lipo BMSes as well if I'm not mistaken, and I guess that they're tuned for a different charge/discharge curve as the chemistry is a bit different, but they may work anyway even if they're li ion. Also yes, just bypass the BMS and use it only for charging if you plan to use the 30A one, connect your battery directly to the esc (maybe add a switch or an anti spark between them ^^). Your charging circuit will have the bms in it instead.
```

---

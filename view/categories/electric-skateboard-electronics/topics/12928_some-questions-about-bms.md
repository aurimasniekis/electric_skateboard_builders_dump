# Some Questions About BMS

### Replies: 8 Views: 918

## \#1 Posted by: Esrapp21 Posted at: 2016-11-12T16:49:45.970Z Reads: 86

```
I am reluctantly going to get a BMS, as I am planning on making a permanent series connection between 2 6s 5000mah lipo batteries. I have a few questions about it though. This is it: http://www.batterysupports.com/44v-48v-504v-12s-30a-12x-36v-lithium-ion-lipolymer-battery-bms-p-268.html . I'm going to charge it with a laptop charging brick, so what Voltage should the brick be? Also, should I be worried about all this talk about how BMS are untrustworthy?
```

---
## \#2 Posted by: rpn314 Posted at: 2016-11-12T19:52:31.160Z Reads: 69

```
I read that as "i'm reluctant to get a BMS" instead of "I"m reluctantly going to get a BMS" and I had this whole long paragraph convincing you to get a BMS or a balance charger, but then I reread it and saw my mistake :slight_smile:

As to your question, the voltage should be what you want to charge your pack to. So if you're making a 12s pack (2 6s in series) you're looking at 4.2*12 = 50.4ish. Now I know some will undercharge their packs by a volt or so to maximize longevity. So maybe a 48v-49V brick. 

As for BMS being untrustworthy, there's some that are and some that aren't. Battery Supports is pretty well respected so you should be okay with that one.
```

---
## \#3 Posted by: Esrapp21 Posted at: 2016-11-12T20:05:26.572Z Reads: 59

```
Ok, perfect. Thank you!
```

---
## \#4 Posted by: Esrapp21 Posted at: 2016-11-12T20:20:49.136Z Reads: 51

```
As for the charger, do you know of one? I can only find chargers for 48v batteries.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-11-12T20:24:11.205Z Reads: 51

```
They're a little harder to find than 10s, but [here's an example on ebay](http://www.ebay.com/itm/Two-wheel-self-balanced-vehicle-12S-43-2V-44-4V-Li-ion-Battery-Charger-50-4V-2A-/222180188366?hash=item33baf8a0ce:g:Nm0AAOSweWVXf1pc). I'm not recommending it, cause it looks like a super cheap chinese brick, but if it puts out the voltage you need consistently and at that amperage, you'll be good.

edit: BatterySupports also sells one that I'm sure is much bettery quality: http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#6 Posted by: Esrapp21 Posted at: 2016-11-12T21:27:50.812Z Reads: 48

```
Ok, cool. Also, just to add to the struggles of 12s batteries :unamused:, is there a 2x 6s to 12s JST XH balance adapter?
```

---
## \#7 Posted by: Namasaki Posted at: 2016-11-13T00:27:31.742Z Reads: 43

```
I agree with @rpn314. Stay with a quality bms from a reputable company and you should be fine. Just be careful not to short anything (mount the bms securely,don't lust leave it loose in the enclosure) and be careful to wire the balance lead correctly before plugging them in and powering up.
A good way to connect the balance leads to the bms is by using 2 6s balance extensions.
Plug each battery into a separate extension cable female end and remove the male end plugs and connect to the bms harness that will come with the bms.
The bms will only have 12 wires so you commit the black ground wire from each pack and just connect the colored wires, one for each cell.
The Red wire will most always be the last cell in the pack. You can use a volt meter to determine which wire goes to which cell in each pack.
You could just hard wire the balance leads to the bms harness but using the extensions makes it easy to swap out in case a pack goes bad.
```

---
## \#8 Posted by: Esrapp21 Posted at: 2017-03-01T02:24:35.784Z Reads: 16

```
I just got the space cell, and I was wondering if it would be ok to charge over night. I have the 2a charger, and I think the BMS will protect to cells, I just want to make sure.
```

---

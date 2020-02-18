# BMS configuration for 12S1P (2x 6S1P)

### Replies: 5 Views: 112

## \#1 Posted by: zenobios Posted at: 2019-07-09T11:21:37.469Z Reads: 39

```
Hi there,

I'm in the endphase of planning my first electric skateboard. I think i will use two of https://hobbyking.com/de_de/zippy-flightmax-5000mah-6s1p-30c-xt90.html and set them in series so I get a 12S1P LiPo.

Furthermore I'd like to use the BMS HCX-D223v1 from BesTech (http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) and I was asking myself which values to use for the adjustable ones:

![image|556x500](upload://kcEYuKUTxMZuwKArSuCdd2nn4iA.png) 

**Over charge detection voltage**: *4.2V*

**Over charge release voltage**: *?* (not sure what this is)

**Over discharge detection voltage**: *3.0* (I'm a bit confused since I read that a good cut-off value is somewhere at 3.2V - 3.4V. Or is this only the cut-off value set in the VESC?)

**Over discharge release voltage**: *?* (not sure what this is)

**Over current detection voltage**: *?* (not sure what this is)

Thanks a lot :slight_smile:
```

---
## \#2 Posted by: zenobios Posted at: 2019-07-10T08:20:51.894Z Reads: 21

```
Can I provide more information to get some help?
```

---
## \#3 Posted by: zenobios Posted at: 2019-07-10T12:14:46.368Z Reads: 19

```
Ok, just learned from BesTech support, that there is a newer version called HCX-D596. BesTech said that I should order it throgh liTechPower: https://www.litechpower.com/product-detail/HCX-D596LI12S80A_08.html. 

If I have a look on the spec, it seems like there is nothing that is adjustable anymore:

![image|618x500](upload://nop8m2xx863rDvufCjMDbaF5KKn.png) 

However, if I download the spec as PDF I can find "Criteria(Adjustable)" as column header:

![image|546x500](upload://ufTs2rN4yu9MPovVTlY33ExWY6p.png)
```

---
## \#4 Posted by: janpom Posted at: 2019-07-10T13:13:39.409Z Reads: 16

```
[quote="zenobios, post:1, topic:98117"]
**Over charge release voltage** : *?* (not sure what this is)
[/quote]

If the highest cell voltage gets above the "Over charge detection voltage", i.e. above 4.2V in your case, the BMS cuts off the charger to prevent over-charge. The voltage then needs to drop below the "Over charge release voltage" until charging is re-enabled.

Example: You set the "Over charge detection voltage" to 4.2V and the "Over charge release voltage" to 4.1V. You charge your battery and the top cell gets to 4.21V. The BMS cuts off the charger. You now have to discharge the battery such that the top cell is at 4.09V or below. Until that happens, you won't be able to charge the battery.

Over discharge release voltage is analogical.
```

---
## \#5 Posted by: zenobios Posted at: 2019-07-10T18:53:12.517Z Reads: 14

```
Thx for the explanation!
```

---

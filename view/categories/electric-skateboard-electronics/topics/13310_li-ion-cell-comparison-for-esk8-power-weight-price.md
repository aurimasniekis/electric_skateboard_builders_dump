# Li-Ion cell comparison for ESK8_Power_Weight_Price

### Replies: 5 Views: 1018

## \#1 Posted by: CRABOLSKY Posted at: 2016-11-19T03:48:51.675Z Reads: 128

```
I've been talking with a local electrical engineer about the best cells to use in an ESK8 scenario. More specifically I've been looking at the A123 26650m1B's.  I want to go about finding the best possible power to weight ratio for a light weight "last mile" build. The one cell that interests me is the Sony VTC5A. In a 10s2p configuration it would have a noticeable drop in output power but would offer double the capacity at the same weight as the A123 cell.

I thought I'd share his rundown as it might be helpful for others evaluating what cells to use. I also provided him with the specs of the VESC 4.12 (referenced as the "controller" below) and the cells used in the space cell for comparison (opt 1. is the space cell). You can ignore the pricing as it represents AUD retail (there are cheaper places to buy from), but he does break it down as a creative cost per 100watt hours. He also comments of the longevity of the cells dependant on discharge rate and drain level which I found interesting....

_"A note on discharges and cycle rates. Discharging at close to the C rate gives the best cycle rate, also partial charges and discharges greatly increase cycle rate. A cell discharged 100% at 20A rate will give you 250 recharges where as a cell discharged from 80% down to 30% at 0.2C rate will give you over 4000 recycles."_

At any rate, here's his breakdown:

I have worked out a range of options for batteries to give you choises in weight, price and energy. Each option provides 36V and 60A nominal, although I've included one at 36V and 45A as the controller you are using is a 50A unit. This battery is capable of the 60A's ( in 3P configuration) with a slight voltage drop of 8% over the true 60A ones but as running at 60A is the upper limit of your requirements and unlikely to be required except for short periods I though it a good option to include as it is a very good battery.

1. Existing cells used: LG18650 HE2  3.6V 2500mAh 20A continuous current capable

10S 3P = 36v (nominal) 60A   total power 270Wh  weight 1380g  

195Wh/Kg

30 cells @ $9 = $279    

$103 per 100 Wh

 

2. Samsung 18650-25R 3.6V 2600mAh 20A continuous current capable: These are very similar to the HE2 but are slightly better.

10S 3P = 36V (nominal) 60A  total power  280.8 Wh  weight 1380g  

203Wh/Kg

30 cells @ $9 = $279  

$100.6 per 100 Wh

 

3. Sony VTC5A 3.6V 2600mAh 30A continuous current capable

10S 2P = 36V (nominal) 60A total power  187.6Wh   Weight 920g  

203Wh/Kg

20 cells @ $11 = $220

$108 per 100Wh

 

4. Samsung INR18650-30Q 15A contiuous current capable

10S 3P = 36v(nominal) 45A  total power 324Wh  Weight 1380g

234.8Wh/Kg

30 cells @ $10 = $300

$92 per 100Wh

 

5. A123 26650m1B 3.3V 2500mAh 70A contiuous current capable

12S 1P = 39.6V(nominal) 70A total power 99Wh weight 912g

108.5Wh/Kg

12 cells @ $13.33 = $160

$161 per Wh

 
I've attached some charts to show how these batteries perform under load. With all batteries the nominal voltage is when being discharged at the 1C rate. C being the capacity of the battery ie the HE2 battery has a capacity of 2500mAh or 2.5Ah so 1C discharge is 2.5Amps. The 20A discharge graph shows that the nominal voltage at 20A is more like 3.2V. Also there is a cycle rate for a 25R at 20A discharge which shows that discharging at 20A shortens the life of Li-ion batteries drastically. The pdf file is a datasheet of the A123 cell and it's discharge cycle chart shows that the cell still has over 80% capacity after 1400 cycles compared to less than 70% after 250 cycles for a typical Li-ion cell. Taking that into account the A123 become a more viable option over the life of the cell. The A123 cell will outlast the Li-ion cells by at least 4 times. Also the voltage curve on a Li-ion cell is much steeper than a LiFePO4 cell which holds 3.2V till about 80% of discharge.

A note on discharges and cycle rates. Discharging at close to the C rate gives the best cycle rate, also partial charges and discharges greatly increase cycle rate. A cell discharged 100% at 20A rate will give you 250 recharges where as a cell discharged from 80% down to 30% at 0.2C rate will give you over 4000 recycles.
```

---
## \#2 Posted by: saul Posted at: 2016-11-19T03:58:21.821Z Reads: 112

```
it really depends on what you want.

a123's are great for high power lightweight packs because you have that crazy 70A cont. and you get really nice fast charging too 
but 18650's have almost 2x the capacity for the same size/cost.

also according a friend who is into the vape scene the sony vtc5's are almost impossible to find.

but i'm still using lipo  because its cheap and easy to setup with just soldering connectors...since we'll pushing these batteries hard I don't expect them to last more than a year or two..but $120 for 2000+ miles of esk8 riding who cares? just ride... :sunglasses:
```

---
## \#3 Posted by: CRABOLSKY Posted at: 2016-11-19T04:07:40.955Z Reads: 103

```
I love that its a vape "scene" :stuck_out_tongue_winking_eye: . There are actually a lot of battery sites that have disclaimers about vaping and safety.  He also mentioned that he vtc5's were actually developed for the high end power tool market.
```

---
## \#4 Posted by: saul Posted at: 2016-11-19T04:13:02.771Z Reads: 94

```
yea i never use the word like that but i don't know what else to call it...
they are high power/quality which is why they are hard to find...cheap atleast...
```

---
## \#5 Posted by: IDVert3X Posted at: 2016-11-19T10:55:04.286Z Reads: 75

```
http://www.electric-skateboard.builders/t/li-ion-cells-comparison-graphs/12595

There I did a comparison of commonly used cells with many graphs recently. Can also be useful to someone.
```

---

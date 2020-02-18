# Do I need BMS with ICharger?

### Replies: 9 Views: 732

## \#1 Posted by: butt_stallion Posted at: 2017-12-15T17:40:20.730Z Reads: 92

```
So I was looking over ICharger's about page and there was a section about balance charging.  It says, "There is no longer a need to have a cell balancer working alongside your charger to balance charge your Lithium batteries."  Does anyone with experience with these chargers know if that means I don't need to purchase a BMS to solder onto my custom battery pack?
```

---
## \#2 Posted by: DEEIF Posted at: 2017-12-15T17:45:21.863Z Reads: 87

```
@scepterr someone needs your help with batteries
```

---
## \#3 Posted by: Grozniy Posted at: 2017-12-15T17:52:53.296Z Reads: 78

```
the chargers we use are balance chargers. Usually they are 6s (it's cheaper).With these chargers you just plug your batteries (up to 6s) and balance charge them. 
A BMS gives you an option of charging them without removing the enclosure and you can charge higher S count(+6). ANd it protects your battery from over charge, discharge, voltage, etc...
difference is in the price. BMS are more expensive
```

---
## \#4 Posted by: butt_stallion Posted at: 2017-12-15T18:06:42.355Z Reads: 73

```
Alright, so I am building a 10s3p battery from 18650s and I already have the icharger 1010B+.  Do you think I need to buy a BMS?  If so, I have seen two recommended on this site.  I know the bestech one is wholesale and you have to buy in bulk and I would rather not do that.  Is the second alright or should I just buy the bestech?

1. http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
2. https://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System/221769582503?epid=1440597425&hash=item33a27f47a7:g:VV0AAOxywCJRa-m2
```

---
## \#5 Posted by: Cobber Posted at: 2017-12-15T18:12:29.601Z Reads: 70

```
i use  a 308 duo, it balance charges 2 x 8s packs at once. lipo, lion... heaps of features, end of charge voltage data logging... as far as chargers go they are the ducks nuts. Nowind uses one too, he has the 2 x 10s model.
An icharger is more advanced than your average BMS, it doesn't go on your board so it saves weight. The disadvantage is no discharge protection and you will have more than one plug to plug in to charge.
if you can work around those points you can save yourself the money and space of a BMS for each build.
```

---
## \#6 Posted by: PXSS Posted at: 2017-12-15T18:19:26.949Z Reads: 63

```
You do not need a balancing BMS. You could simply use a protection board without cell balance
```

---
## \#8 Posted by: butt_stallion Posted at: 2017-12-15T18:34:31.170Z Reads: 55

```
What do you mean by more than one plug to charge?
```

---
## \#9 Posted by: Cobber Posted at: 2017-12-15T18:37:30.161Z Reads: 55

```
charge plug and balance lead for each battery pack on your board... unless you are charging through the balance leads.
example: you might have 2 x 6s packs...
```

---
## \#10 Posted by: Grozniy Posted at: 2017-12-15T22:42:18.629Z Reads: 38

```
Well, if you're investing in good battery pack, why not protect it better? That means adding a BMS.
some Esk8ers liked this one: [supower](https://www.aliexpress.com/item/SuPower-10S-36V-37V-42V-60A-Li-ion-Lithium-LiPo-Battery-BMS-Management-System-Balance-PCB/32801166001.html?spm=2114.search0104.3.68.nkJCEA&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10344_10068_10130_10345_10324_10342_10547_10325_10343_51102_10340_10341_10548_10609_10192_10541_5000012_5130012_10190_10084_10083_10307_10301_5080012_10303_10610_10539_10312_10059_10313_10314_10184_10534_100031_10604_10603_10103_10605_10594_5060012_10596_10142_10107,searchweb201603_1,ppcSwitch_5&algo_expid=918ae807-905d-4d29-abfa-cf6bf07ace98-9&algo_pvid=918ae807-905d-4d29-abfa-cf6bf07ace98&rmStoreLevelAB=0#thf) but i don't have experience with it and i don't know if one could program different values.
And other esk8ers don't use a bms on their 18650 packs and rely on charger.
So if you want to save some :money_with_wings:, don't get a bms, use your charger. If your batteries are high drain, they will not "die" if vesc asks for more power, your vesc will die first. 
Summation: With bms everything is protected. Without bms, only charging is protected and your vesc could be harmed, you spend less, save some space inside enclosure and you'll have far less soldering work.
PS: i'm not an expert, consider my opinion and compare it with others ;)
```

---

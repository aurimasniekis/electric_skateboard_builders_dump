# Charging individual cells while in series question

### Replies: 12 Views: 1814

## \#1 Posted by: Hummie Posted at: 2017-10-21T17:46:22.569Z Reads: 126

```
i forget, can you keep all cells in series and attach an individual 4.2 regulated supply to individual cells if it's a switching supply, or will that be creating shorts?  I imagine if it's a linear supply it will have no true connection similarly to a transformer and therefore there would be no short for sure?
was thinking of using a 13 prong plug and charging cells individually to balance.  so skipping a bms or balance charger and balancing in this way

was thinking of using something like this but a cheaper version
https://www.adafruit.com/product/1904

OR INSANE DEAL ON LINEAR SUPPLY:
https://www.openimpulse.com/blog/products-page/product-category/tp4056-single-cell-lipo-battery-charger/
```

---
## \#2 Posted by: pakue Posted at: 2017-10-21T23:07:35.835Z Reads: 102

```
It‘s a bit tedious, but as long as you only connect the poles of one cell (or multiple ones in parallel) you can charge them one by one.
```

---
## \#3 Posted by: Hummie Posted at: 2017-10-22T01:51:06.413Z Reads: 97

```
I tried to get 100 but it says only for certain countries.

  I don't see it as tedious, once 12 of these are connected to a power supply at one end and their other ends connected to a thirteen prong plug then can balance charge with one plug.   paired w the lvc on the vesc and it's a battery situation solved in my mind.
```

---
## \#4 Posted by: pakue Posted at: 2017-10-22T10:34:24.307Z Reads: 66

```
If you connect them all to the same power supply they have the same ground level and it would short once you connect 2 of them to the battery. This would only work once they are galvanically isolated from each other (e.g. through a transformer).
```

---
## \#5 Posted by: Hummie Posted at: 2017-10-22T14:56:36.045Z Reads: 55

```
A linear power supply is pretty much a transformer and circuit is isolated no?
```

---
## \#6 Posted by: Fatos Posted at: 2017-10-22T18:06:55.520Z Reads: 49

```
@pakue @Hummie

If it balancing the pack on cheap is what you are trying to achieve I can suggest this PCB. Its dirt cheap and does the job. But it won't protect from overcharge and discharge. https://www.ebay.com/itm/3S-13S-Lithium-Battery-Balanced-Function-Board-For-18650-Polymer-Battery/332160632043?ssPageName=STRK%3AMEBIDX%3AIT&var=541192613484&_trksid=p2057872.m2749.l2649
```

---
## \#7 Posted by: pakue Posted at: 2017-10-22T18:54:46.297Z Reads: 45

```
No, normal switch mode power circuits aren't isolated. Something like [this](https://www.digikey.com/product-detail/en/recom-power/REM6-0505S-A/945-2231-ND/5130719) is, but way more expensive than just using a balance charger if you need one for every cell.
```

---
## \#8 Posted by: Hummie Posted at: 2017-10-22T19:38:06.778Z Reads: 39

```
No such thing available as a 12s charger.  
How bout a linear power supply for each cell to be connected to individually instead of a switching supply?
```

---
## \#9 Posted by: Hummie Posted at: 2017-10-22T22:56:43.167Z Reads: 36

```
this is great @Fatos.  I didn't really look at it.  fantastic.  just what I wanted.  and it just connects to the cells.  the missing ingredient in my one-plug high-power bulk charging board.   why is no one else interested in these?  especially considering there are no 12s chargers.  and bms suck!  I feel safe with this..tell me why I shouldn't just run with these and bulk charge with the vesc low voltage shut-down as protection?  its a one sided balancing version vs a bms having two.  what else is the difference!? simple

ok there's a difference and no shut down and probably other things ..which i'd like to hear about.  i'm still all in and got 6 as if they were going to disappear or something.  I've been looking at just such a thing and found it before but at huge cost.  maybe the resistor is small and have to charge slowly?  and when I saw it it was practically custom.  or you can make it but that's a lot of work.  and this is so small.
```

---
## \#10 Posted by: Fatos Posted at: 2017-10-22T23:08:49.727Z Reads: 34

```
@Hummie
First of all glad to help. The balance current on this is not so high, just around 60mAmp I think. But that should not be a problem. BMS has its advantages even though I think I won't use one myself either on the build im doing.A fuse should do it.
There are plenty of 12s (50.4v) chargers also. I own one like this at least:slight_smile:. https://www.aliexpress.com/item/100-240V-DC50-4V-1-6A-polymer-lithium-battery-charger-DC-5-5MM-2-1MM-Portable/32777216768.html?spm=a2g0s.9042311.0.0.eCUbGF
Not the most powerful one but still(dirt cheap). You could connect 2 of them parallel.And I know there are more powerfull ones out there also.
I'm on the making of a fast charger with an Omron PSU https://www.ia.omron.com/products/family/1616/
And a step-up converter something like this https://www.ebay.com/itm/DC-DC-150W-Step-Up-10-32V-to-12V-60V-Boost-Constant-Current-Power-Apply-Module/161506793056?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D2%26asc%3D41375%26meid%3D3a523174c83e4bb49b92daa8d7c5909b%26pid%3D100005%26rk%3D2%26rkt%3D6%26mehot%3Dpp%26sd%3D171827535350&_trksid=p2047675.c100005.m1851.
 To be able to fast charge, my board, in case I'm in a hurry.But also too not charge my batteries to full when I don't need long range. (a good way to prolong battery life is too use them around 85%-30%)
```

---
## \#11 Posted by: Hummie Posted at: 2017-10-22T23:21:10.965Z Reads: 31

```
terminology I call those bulk chargers vs a balance charger, yea I have a bulk switching supply like that, a couple different amperages all at 48v.  or adjustable.  Why bother with the step up voltage instead of getting the supply at the voltage you'd want?  seems more trouble.  that Omron power supply  its list of features is crazy.  Ive got some cheap Chinese ones or meanwell.  what sold you on getthing the Omron?  

glad to hear you like these mini balancers too!  damn I'm excited for these.  just have to confirm they work, and what else you think how they will do?

and how much power will you be charging at!?  get it on video just in case.  just kidding.  the sound of my higher power supply just sounds powerful.
```

---
## \#12 Posted by: Fatos Posted at: 2017-10-22T23:31:51.697Z Reads: 31

```
I see, I'm not in Lipo charges and batteries. I have never owned a lipo battery and most likely never will. 
I have a more than one power supply laying around. But that is too mainstream. :slight_smile:
I have two of these Omron PSU, one at 150W and one at 300W. Ane they are high-quality PSU with high efficiency. I got them for free since some bigger devices went obsolete and I did scavenge them.  
Another reason to use them is they don't need a FAN to make noise and they are still way lighter than a Variable power supply.In case you want to take them with somewhere else.
Chargig current will be : 
150W/24V= 6,25A
 24/50=0,48x6,25=3A
300W/24V= 12.5A
 24/50=0,48x12.5=6A
You wold lose a bitt on the eficcency of the step up conbertor but not much.
```

---

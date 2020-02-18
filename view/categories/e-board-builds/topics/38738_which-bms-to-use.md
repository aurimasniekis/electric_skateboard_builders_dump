# Which BMS to use?

### Replies: 9 Views: 3715

## \#1 Posted by: shong96 Posted at: 2017-11-19T11:24:45.521Z Reads: 321

```
Hey guys, Im currently planning a build with a dual 6374 190kV motor, 2 vesc from torqueboards and a set of Samsung 30Q 18650 Batteries in a 12S4P config. Im currently looking at a BMS from Battery Supports. Will this [BMS](http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html) work? 
Should I go for a BMS with a lower amp or a higher amp? 

Thanks!
```

---
## \#2 Posted by: Bloop Posted at: 2017-11-19T12:25:27.116Z Reads: 310

```
Hey id say the higher amps are only if you want to use the bms to also discharge the batteries like when you are riding or you only want to use it to balance charge your batteries 

Supports Max. Continuing Discharge Current: 60A

 so this will depend on how much current will your motors use. 
I saw some guys are using a lower price bms to only charge the batteries and bypassed it when discharging.
```

---
## \#3 Posted by: Sender Posted at: 2017-11-19T13:24:24.227Z Reads: 283

```
I see this a lot and don't fully understand it. can you clear up the advantages and disadvantages to using a BMS only for charging or charging and discharging ?  Or is it only that you can use a cheaper BMS for charging only?
```

---
## \#4 Posted by: Bloop Posted at: 2017-11-19T14:00:19.730Z Reads: 266

```
Bms will have some protections for overcharge over current etc for charging but it also have protection for under discharge. so if you discharge your batteries under Over-discharged Protection: 2.9 ± 0.05 V in your case then bms will cut the power so your batteries wont get damaged. 
if you bypass the bms it wont know when the batteries are discharged and you might damage them. with bypassed bms it will only balance charge your pack

You can also set some limitations on vesc tho so i think this is why people do bypass on discharge or just be careful not to discharge batteries under 2.9-3V  per cell
```

---
## \#5 Posted by: Acido Posted at: 2017-11-19T16:11:23.395Z Reads: 243

```
Its faster to search than to wait for reply ;)
```

---
## \#6 Posted by: Sender Posted at: 2017-11-19T16:20:26.370Z Reads: 242

```
I've read a descent amount, just curious his summation 😉.
```

---
## \#7 Posted by: willpark16 Posted at: 2017-11-19T20:35:15.737Z Reads: 217

```
https://www.electric-skateboard.builders/t/a-final-word-on-bypassing-bms-for-discharge/18351
```

---
## \#8 Posted by: Namasaki Posted at: 2017-11-19T21:56:10.324Z Reads: 198

```
I wonder if those Vescs can handle 12s
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-11-19T22:00:36.541Z Reads: 193

```
I'm running 12s mono with tb vesc in bldc, hasn't gone bad after 100+ miles. 

wouldn't attempt foc though.
```

---

# Charger For 9s BMS

### Replies: 7 Views: 1257

## \#1 Posted by: dyingmoss Posted at: 2017-08-22T15:29:23.171Z Reads: 85

```
Hello all,

Will this [Charger](http://www.ebay.com/itm/42V-2A-AC-DC-Power-Adapter-Battery-Charger-for-Hoverboard-USA-/311857168225?epid=917511745&hash=item489c22bf61:g:QSIAAOSwmCVZARfU) work with a 9s lipo BMS setup?

The BMS<img src="/uploads/db1493/original/3X/2/b/2b016715c66bfc07d1acd8d197e7f324f1a8ffc8.jpg" width="353" height="500">
```

---
## \#2 Posted by: SilentException Posted at: 2017-08-22T16:09:42.693Z Reads: 74

```
No, you need 37.8V charger.
```

---
## \#3 Posted by: dyingmoss Posted at: 2017-08-22T16:13:11.490Z Reads: 73

```
[quote="SilentException, post:2, topic:31259"]
37.8V charger
[/quote]
https://www.aliexpress.com/store/product/37-8V-3A-lithium-battery-charger-for-9S-lithium-battery-pack/1922288_32491575567.html
So this one would work?
```

---
## \#4 Posted by: rojitor Posted at: 2017-08-24T08:22:02.466Z Reads: 62

```
Yes it will work...... as long as the bms works. If the bms fails your cells will Overcharge and die,so not recommended. The other charger will work better and is also cheap. I'd go for it.
```

---
## \#5 Posted by: Rashid Posted at: 2017-08-25T17:55:50.174Z Reads: 58

```
I think silentexception and rojitor are right.
Your bms has Overcharge protection but you must have blind trust on the bms if you use overvolted charger. In case it fails you battery is finished. 
You should use a 9s charger instead. 
I also think the green light will never be on if you use the 10s charger, charging would be confusing too.
```

---
## \#6 Posted by: SilentException Posted at: 2017-08-25T18:06:02.944Z Reads: 57

```
Using higher voltage charger would result in completely wrong charging curve and the charger would never enter CC mode. BMS would of course cut the charging when any cell go over over charge voltage but this scenario is far from perfect. I've also been told by BesTech themselves to always use proper voltage charger. 10S BMS will work with lower number of cells but when charging use proper   CV charger.
```

---
## \#7 Posted by: vap Posted at: 2017-08-26T12:04:38.054Z Reads: 52

```
Since i didn't find any good chargers (i've got a chinese one that overcharges batteries) i'm going to build my own adjustable charger using 36v power supply, CC/CV dc-dc module, relay and arduino for voltage/capacity cutout. So for a rare 9s setup you might consider something like that.
Parts:
https://www.banggood.com/36V-180W-AC-DC-Switching-Power-Supply-Board-High-Power-Industrial-Power-Supply-Module-p-1111658.html
https://www.banggood.com/600W-Digital-Control-DC-DC-Adjustable-Step-Up-Module-Constant-Voltage-Current-Solar-Charging-p-1082316.html
alternatively:
https://www.banggood.com/400W-DC-8V-80V-10A-Digital-Voltage-Current-Boost-Module-Constant-Converter-p-1141070.html?rmmds=cart_middle_products
```

---

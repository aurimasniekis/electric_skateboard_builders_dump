# Is this BMS diagram right?

### Replies: 12 Views: 2352

## \#1 Posted by: Smorto Posted at: 2017-04-28T22:45:03.655Z Reads: 207

```
Hi, simple question here, does this wiring diagram look right? I know next to nothing about BMS's so I need some input. I would like to bypass it and use it only for charging and I don't think my diagram bypasses so i would like some input on this as well. 

https://docs.google.com/drawings/d/1tXLadrh44pFh265D3_fWR32QnZEoWXcDMkGyta21g6Q/edit

Also would this charging port
http://www.ebay.com/itm/10pcs-DC-5-5-x-2-1mm-Power-Female-Jack-Adapter-Cable-Plug-Connector-for-CCTV-S2-/262887247109?hash=item3d354d0d05:g:glsAAOSw4A5YwP~H

And this charger 

http://www.ebay.com/itm/DC42V-2A-Adapter-Charger-Two-wheel-Self-Balanced-for-36V-Li-ion-Lithium-Battery-/302269834907?hash=item4660afa69b:g:kp0AAOSwWWxY-YWr

And this

http://www.ebay.com/itm/3dRCparts-JST-XH-10S-TO-2-5S-BALANCE-SERIES-SERIAL-ADAPTER-LIPO-CHARGE-CORD-/381951421626?hash=item58ee142cba:g:GDMAAOxyUrZS8bPv
 
All work together?
```

---
## \#2 Posted by: smurf Posted at: 2017-04-28T23:00:27.789Z Reads: 176

```
http://m.ebay.com/itm/Waterproof-3A-5-5-X-2-1mm-DC-Socket-plug-Power-Charger-Plug-Female-Panel-Mount-/231660804404
```

---
## \#3 Posted by: Smorto Posted at: 2017-04-28T23:13:32.192Z Reads: 170

```
Does that only support 3A charging? Also can you comment on the diagram? Thanks! :slight_smile:
```

---
## \#4 Posted by: smurf Posted at: 2017-04-29T00:34:10.522Z Reads: 165

```
http://www.elifebike.com/upfile/dtpic/2011/4Q/MW0Q.1NEXH/9KD0HW_4HQBF.jpg
```

---
## \#5 Posted by: Namasaki Posted at: 2017-04-29T00:56:44.552Z Reads: 158

```
[quote="Smorto, post:1, topic:21994"]
I don't think my diagram bypasses so i would like some input on this as well.
[/quote]


You are correct, this diagram doesn't bypass the bms for discharge
```

---
## \#6 Posted by: Smorto Posted at: 2017-04-29T01:09:24.508Z Reads: 153

```
I'm sorry but for whatever reason this diagram just goes straight over my head, also the BMS I am looking at doesn't have a C-.. that I know of 

http://www.batterysupports.com/36v-37v-42v-10s-30a-10x-36v-lithium-ion-lipolymer-battery-bms-p-265.html
```

---
## \#7 Posted by: Smorto Posted at: 2017-04-29T01:10:41.801Z Reads: 152

```
If I did it like this, do you think I would be fine with a 60a BMS? I am using an 8s 5000mah 20c LiPo battery setup with Ollin VESC, and @Jlabs 6354 190kv motor.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-29T01:24:34.826Z Reads: 148

```
I think you will be fine if you discharge through a 60a bms. If your running a single drive, you can set your vesc battery max at 60a and the bms and battery should  handle it no problem.
A 60a Battery Supports bms is rated for 60a continuous current.
And if you set your vesc battery max at 60a, you theoretically should only pull that much at full throttle.

And, discharging through the bms gets you all of the protective features the bms has to offer.

And since your bms does not have a dedicated charge connection for the negative charger wire, Use the P- connection for the negative charge wire

And in case you didn't know it, Battery Supports and Supower are the same.
<img src="/uploads/db1493/original/3X/f/c/fc206732fb42709953b58f492fd3dcd99fbe77ae.png" width="673" height="358">
```

---
## \#9 Posted by: Smorto Posted at: 2017-04-29T01:36:38.089Z Reads: 136

```
So my batt max is only set at 30A right now though I might want to increase that in the future, I would definitely be fine with a 60A BMS right? And would my diagram would for that 60A BMS?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-04-29T02:22:37.572Z Reads: 127

```
You should be able to increase your battery max to 60a no problem.
As far as your diagram, I can only assume that it is correct because displaying the xt90 connectors as you did, obscures the actual wiring path.
I would need to see your diagram without the connectors in order to say for certain that it is correct.
I need to see the wiring path, How you connect the wires is irrelevant.
Example:
Here is a version of your diagram wired to bypass the bms during discharge.
(I made this before I found out that you where using a bms that you could discharge through)

<img src="/uploads/db1493/original/3X/1/1/1178ddfba6f46276ce977b4faec74f9030986aac.png" width="690" height="250">
```

---
## \#11 Posted by: Smorto Posted at: 2017-04-29T02:38:34.920Z Reads: 121

```
Without the connectors 

https://docs.google.com/drawings/d/1QNTjsXTlInK7Asc_5bsF3VJ25lTbVYBYGbl3RTpI6aE/edit
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-29T03:24:16.130Z Reads: 113

```
Ok, looks good to me :+1:
```

---

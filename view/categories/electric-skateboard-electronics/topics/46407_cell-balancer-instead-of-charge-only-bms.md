# Cell Balancer instead of &ldquo;Charge only&rdquo; BMS

### Replies: 8 Views: 911

## \#1 Posted by: bevilacqua Posted at: 2018-02-14T18:33:02.609Z Reads: 119

```
Hi, I recently bought a 10s Li-Ion cell balancer on ebay.de. It looks like a Bestech model (link below) witch costs just 5 USD, but has to be bought in a group buy...

I have seen many mods with a "charge only" BMS. Mostly some cheap 15-30A BMS. 

Since the vesc has already a low voltage cutoff, what is the benefit of using a "real" BMS (Just for charging), which will take more precious space and will cost more?

The balancing current is not so high, but since it balances even without a plugged in charger, I dont think that it would be a problem. 

Does anyone have any experience with such a balace-board? 

It is really tiny (Euro for scale): 

![10s balancer|666x500](upload://jsTYtlwlo1qJwK3ZQohjR26Dvvk.jpg)



Ebay.de: 
https://www.ebay.de/itm/Balancer-fur-10S-36V-Li-ion-Akkupacks-Balance-Board-Lastmodul-4-2V-Zelle/323028686150?hash=item4b36029546:g:uRQAAOSwRTVaaZvn
Bestech:  
http://bestechpower.com/balanceboard/JH-D105B.html
```

---
## \#3 Posted by: ZackoryCramer Posted at: 2018-02-14T19:09:21.472Z Reads: 101

```
I am not sure about the positives but I heard somewhere that having a full discharge bms can apply current cutoff when breaking at near full capacity which could be dangerous when you are going downhill.
```

---
## \#4 Posted by: bevilacqua Posted at: 2018-02-14T19:17:03.709Z Reads: 97

```
The balancing current has nothing to to with the charge current, you effectively charge directly through the main positive and neg port. It just takes longer to balance
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2018-02-14T19:17:57.137Z Reads: 93

```
@JLabs  This balancer doesn't charge, it can **only** discharge. You plug this module into the balance connector of the 10S battery and it then starts to discharge a cell once it goes over some voltage level (4,2V +-25mV according to specs). 

Problems with this approach?
* Well the most obvious is that it can't stop the charger from charging. If you for example mismatch your battery pack and charger (11S charger, 10S pack) it will keep pumping juice into the battery and the module will start to balance, but will not be able to discharge the cells faster than the charger is charging, so it'll probably go nuclear at some point.
* Other one is that it can't protect single cells from being overcharged if the cells are for some reason unbalanced.
* Balance voltage is set, you can't change it.
* No indication when it's balancing, so you can't for example lower the charging current if you're using a lab power supply

Does the 10S module support <10S packs?

Otherwise if you know what you're doing, it's a simple module with a simple job that should work.

[quote="JLabs, post:2, topic:46407"]
charge current of 84mA which is 0.84A
[/quote]
84mA = 0.084A
```

---
## \#6 Posted by: bevilacqua Posted at: 2018-02-14T19:20:34.390Z Reads: 86

```
It is indeed very limited, but it does the basics, witch is balancing :) 
Im using it in a light portable build. My main board has a propper BMS
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2018-02-14T19:25:10.567Z Reads: 83

```
I'm very familiar how BMS' work quite intimately, in fact I'm designing one for the esk8 community at the moment
http://www.electric-skateboard.builders/t/poll-announcement-flexible-configuration-and-charging-bms/46117

It's gonna be quite a configurable module for 4S-12S battery packs with flexible charging options.
```

---
## \#8 Posted by: bevilacqua Posted at: 2018-02-14T19:27:57.567Z Reads: 77

```
I already have my eyes set on that thread ;) 

The voltage boost option is really interesting. I think that having the option to use your lower voltage laptop charger on your esk8 is very convenient.
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-02-14T19:31:28.228Z Reads: 76

```
Laptop chargers also usually have a pretty slim form factor so they won't take much space in a backpack for example. And it also supports the higher power bulk chargers. For example a 42V 2A charger for 10S packs that skips the boost converter and goes directly through a charging FET, so if for example the pack is unbalanced and one cell starts to creep too high, we can cut the current, balance the pack and start charging again.
```

---

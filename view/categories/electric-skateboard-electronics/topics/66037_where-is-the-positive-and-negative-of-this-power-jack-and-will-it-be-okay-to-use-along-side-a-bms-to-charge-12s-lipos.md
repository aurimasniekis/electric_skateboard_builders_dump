# Where is the Positive and Negative of this Power Jack? And will it be Okay to use Along side a BMS to charge 12s Lipos?

### Replies: 19 Views: 384

## \#1 Posted by: Toohat Posted at: 2018-08-25T15:48:59.025Z Reads: 71

```
this is the bms https://www.ebay.ca/itm/12S-15A-Balance-Protect-Circuit-PCM-BMS-for-43-2v-44-4v-Li-ion-Li-Po-Battery-873/323217175378?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649
This is the power jack https://www.amazon.ca/gp/product/B076P97Z2G/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1 ![IMG_0097|375x500](upload://b9efwuXZa6O5Sa4n4y7tw75NB5P.JPG)
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-08-25T16:12:21.572Z Reads: 58

```
Positive is usually the longer prong
```

---
## \#3 Posted by: Namasaki Posted at: 2018-08-25T16:59:01.376Z Reads: 53

```
You have to match it to your charger when you wire it.
```

---
## \#4 Posted by: Toohat Posted at: 2018-08-26T00:31:51.789Z Reads: 41

```
its rated at 30v and my lipos are 44.4v total is that okay? cuz i will only be using it for charging
```

---
## \#5 Posted by: Toohat Posted at: 2018-08-26T00:40:51.648Z Reads: 40

```
And I got this charger https://www.amazon.ca/gp/product/B0776TDRL8/ref=oh_aui_detailpage_o03_s01?ie=UTF8&psc=1

How does it work like is it going to charge at whatever the charger is giving to the bms?
```

---
## \#6 Posted by: Namasaki Posted at: 2018-08-26T03:14:17.427Z Reads: 37

```
[quote="Toohat, post:4, topic:66037, full:true"]
its rated at 30v and my lipos are 44.4v total is that okay? cuz i will only be using it for charging
[/quote]


It should be fine because you will be charging at relatively low current
```

---
## \#7 Posted by: Namasaki Posted at: 2018-08-26T03:15:35.743Z Reads: 38

```
[quote="Toohat, post:5, topic:66037"]
And I got this charger https://www.amazon.ca/gp/product/B0776TDRL8/ref=oh_aui_detailpage_o03_s01?ie=UTF8&amp;psc=1

How does it work like is it going to charge at whatever the charger is giving to the bms?
[/quote]


That charger is only 12v, it will not charge your battery.
You need a 12s charger 50.4v

44.4v is the nominal voltage for lithium ion and lithium poly 12s battery
50.4v is full charge voltage. 4.2v per cell
```

---
## \#8 Posted by: Toohat Posted at: 2018-08-26T03:18:49.259Z Reads: 34

```
now it makes sense, thanks
```

---
## \#9 Posted by: Namasaki Posted at: 2018-08-26T03:21:01.555Z Reads: 35

```
something like this
https://www.amazon.com/WAOUKS-Charger-Lithium-Auto-Stop-Aluminum/dp/B07G9VHY8N/ref=sr_1_6?ie=UTF8&qid=1535253587&sr=8-6&keywords=12s+lithium+charger
```

---
## \#10 Posted by: Namasaki Posted at: 2018-08-26T03:30:57.228Z Reads: 36

```
it is best to fully balance charge your Lipos before connecting them in series and to the bms if you have a hobby balance charger.
If your Lipos are not evenly charged before putting them together, the bms will struggle to balance them so that they can fully charge.
```

---
## \#11 Posted by: Toohat Posted at: 2018-08-26T03:31:20.689Z Reads: 31

```
will this one be okay?
https://www.ebay.com/itm/50-4V-2A-Power-Adapter-For-Self-Balanced-Vehicle12S-Li-ion-Battery-Charger-Plug/291922334252?hash=item43f7ed522c:g:ckUAAOSwEH9ZZ0u2
```

---
## \#12 Posted by: Toohat Posted at: 2018-08-26T03:33:15.559Z Reads: 31

```
I didnt know that, thanks a lot
```

---
## \#13 Posted by: Namasaki Posted at: 2018-08-26T03:33:35.603Z Reads: 32

```
It will work, it will just take twice as long to charge the pack and those type of chargers tend to get hot while charging because it has no cooling fan or adequate heat sink. Heat breaks down electronics so it will fail eventually.
```

---
## \#14 Posted by: Toohat Posted at: 2018-08-26T03:34:56.750Z Reads: 30

```
Okay I see, thanks again for your help, I truly appreciate it.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-08-26T03:38:25.629Z Reads: 31

```
I started out using Lipos and taking them out to charge them with my hobby charger. 
Then later I setup my Lipos with a bms for convenience but I found by experience that a good hobby charger balance charges Lipos better than the bms can.

I still have my hobby charger on hand in case I need it for maintenance.
It's a good idea to have one if your going to use Lipos.
```

---
## \#16 Posted by: Toohat Posted at: 2018-08-26T03:41:17.864Z Reads: 29

```
Yeah I got one but its just inconvenient, it takes way too long cuz im charging my lipos from the balance leads and there is two of them so after im done charging one i have to charge the other.
```

---
## \#17 Posted by: Namasaki Posted at: 2018-08-26T03:46:36.468Z Reads: 29

```
You have one, good. Once you balance your packs with it, the bms will be able to sustain the balance. It just can't do it if the packs get too far out of balance.

Another tip:
get some balance extensions to connect to your Lipos and wire to the bms so you don't have to remove the balance connector from the Lipo pack. This way it will be much easier to do maintenance on the packs if necessary or to replace them if necessary.
I set mine up that way and was really glad I did when one of my packs failed and had to be replaced.
```

---
## \#18 Posted by: Toohat Posted at: 2018-08-26T03:49:43.814Z Reads: 29

```
Sure I got those too, thanks boss.
```

---
## \#19 Posted by: Namasaki Posted at: 2018-08-26T03:50:44.243Z Reads: 29

```
Here is a link to my build thread in case you haven't seen it.
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---

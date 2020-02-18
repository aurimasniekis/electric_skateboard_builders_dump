# Would this bms work?

### Replies: 31 Views: 2054

## \#1 Posted by: Quinlanbrown Posted at: 2016-09-29T15:49:19.248Z Reads: 168

```
http://m.ebay.com/itm/221644780045?_mwBanner=1#rwid
Would this work, I'm running 4 zippys I'm sereas and keep killing batterys by havein one not balanced
```

---
## \#2 Posted by: 2-alex-2 Posted at: 2016-09-29T16:06:24.249Z Reads: 161

```
It's a little on the low side for 60a ideally 80a or the 100a version would be better. But what esc or vesc are you using and what charger are you using as if they are setup right then don't need a bms. I run 3x2s lipo in series with no bms. But my esc is sit-up to shut down if voltage drops to low and then I balance charge all the time.
```

---
## \#3 Posted by: thefer Posted at: 2016-09-29T16:06:30.042Z Reads: 150

```
Yeah supower makes decent ones. Mine is a lower voltage one.
```

---
## \#4 Posted by: chinzw Posted at: 2016-09-29T16:16:52.286Z Reads: 139

```
He won't be pulling 60A with 12S
```

---
## \#5 Posted by: Jinra Posted at: 2016-09-29T16:20:59.009Z Reads: 131

```
60A is more than enough. I barely ever pull more than 40A and I'm on 10s and live in San Francisco. Though if I recall correctly @quinlanbrown is a maniac and wants the torque of hercules himself, so maybe 60A isn't enough for his crazy motor.
```

---
## \#6 Posted by: Quinlanbrown Posted at: 2016-09-29T17:13:55.813Z Reads: 122

```
What kind of charger do I need for this, could you thro me a link
```

---
## \#7 Posted by: Jinra Posted at: 2016-09-29T17:17:04.075Z Reads: 116

```
Depends on the charge port you use on it. I use a 5.5x2.1mm dc connector

http://www.ebay.com/itm/Two-wheel-self-balanced-vehicle-12S-43-2V-44-4V-Li-ion-Battery-Charger-50-4V-2A-/222180188366?hash=item33baf8a0ce:g:Nm0AAOSweWVXf1pc

This one has a 5.5x2.5mm connector

http://www.ebay.com/itm/New-AC-100V-240V-TO-DC-50-4V-1-5A-63W-12-series-lithium-Battery-Charger-Adapter-/222242430492?hash=item33beae5e1c:g:29MAAOSwh-1W5qWo
```

---
## \#8 Posted by: michaeld33 Posted at: 2016-09-29T17:25:29.020Z Reads: 106

```
I thought the two wheeled segways were 10S? Idk maybe I'm wrong but mine has the same output as my 10s
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-29T17:27:33.772Z Reads: 104

```
Beats me ¯\\\_(ツ)_/¯, but as long as the output voltage is correct, it doesn't matter.
```

---
## \#10 Posted by: michaeld33 Posted at: 2016-09-29T17:29:12.045Z Reads: 103

```
Haha I guess so...
```

---
## \#11 Posted by: Quinlanbrown Posted at: 2016-09-29T17:32:35.644Z Reads: 100

```
[quote="Jinra, post:7, topic:10348"]
5.5x2.1mm dc connector
[/quote]

Thanks 
If I use a 12v connector for the charger and my board would it work
```

---
## \#12 Posted by: Jinra Posted at: 2016-09-29T17:35:14.972Z Reads: 93

```
What are the dimensions of the connector? 12v doesn't say much about it's physical properties.
```

---
## \#13 Posted by: Quinlanbrown Posted at: 2016-09-29T17:49:24.448Z Reads: 93

```
http://m.ebay.com/itm/5pair-12V-5-5x2-1mm-Male-Female-DC-Power-Socket-Jack-Connector-Cable-Plug-Wire-/272180991208?nav=SEARCH

With 

http://m.ebay.com/itm/10pcs-DC-Power-Supply-Jack-Socket-Female-Panel-Mount-Connector-5-5-x-2-1mm-EF-/401119290150?nav=SEARCH
```

---
## \#14 Posted by: Jinra Posted at: 2016-09-29T17:51:15.937Z Reads: 93

```
You don't need the male side since it comes with the charger, and you only need 1 DC port. This is the one I used.

http://www.ebay.com/itm/221909154788?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#15 Posted by: ABuildEnthusiast Posted at: 2017-07-19T01:00:23.761Z Reads: 58

```
 @Jinra I have two 6s LiPo's in series (12s). For a BMS set, Obviously charging charges but I never understood why I would discharge. Also, would all these work for my BMS setup and am I missing anything? Here are the links:
BMS: [http://www.ebay.com/itm/221644780045#rwid](http://www.ebay.com/itm/221644780045#rwid)
Charger: [http://www.ebay.com/itm/Two-wheel-self-balanced-vehicle-Battery-Charger-50-4V-2A-to-43-2V-Li-ion-Cell-US-/222430137024?hash=item33c9de8ac0:g:Nm0AAOSweWVXf1pc](http://www.ebay.com/itm/Two-wheel-self-balanced-vehicle-Battery-Charger-50-4V-2A-to-43-2V-Li-ion-Cell-US-/222430137024?hash=item33c9de8ac0:g:Nm0AAOSweWVXf1pc)
```

---
## \#16 Posted by: ABuildEnthusiast Posted at: 2017-07-19T01:01:47.092Z Reads: 57

```
@Jinra Also, an On Board Port: [http://www.ebay.com/itm/221909154788?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT](http://www.ebay.com/itm/221909154788?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
```

---
## \#17 Posted by: Jinra Posted at: 2017-07-19T01:09:28.097Z Reads: 56

```
yep looks good. The BMS is pretty worthless for over-discharge on your batteries though so make sure you set the setting appropriately on your ESC/VESC.
```

---
## \#18 Posted by: ABuildEnthusiast Posted at: 2017-07-19T15:46:06.106Z Reads: 52

```
@Jinra I have a VESC from Tourque Boards. What would I change on the setting If I hook up this BMS??
```

---
## \#19 Posted by: Jinra Posted at: 2017-07-19T15:51:32.818Z Reads: 52

```
Battery cutoff start/end probably 44 start and 42 end would be good.
```

---
## \#20 Posted by: ABuildEnthusiast Posted at: 2017-07-19T15:57:24.625Z Reads: 50

```
At 4.2 volts per cell right?
```

---
## \#21 Posted by: Jinra Posted at: 2017-07-19T15:58:26.058Z Reads: 47

```
No, cutoffs are when you want the board to start shutting down. 4.2 volt/cell is full charge. For lipos start at about 3.6-3.7/cell and end at 3.4/3.5
```

---
## \#22 Posted by: ABuildEnthusiast Posted at: 2017-07-19T16:02:20.110Z Reads: 46

```
Oh gotcha. Will this BMS setup i listed charge it to 4.2 v per cell?
```

---
## \#23 Posted by: Jinra Posted at: 2017-07-19T16:03:38.656Z Reads: 47

```
Yep, says right there in the description

> Balanced current: 60mA (VCELL = 4.20V when)
Balanced for: 4.20 ± 0.05 V
```

---
## \#24 Posted by: ABuildEnthusiast Posted at: 2017-07-19T16:07:27.979Z Reads: 44

```
Also, do you think 60 A will be enough? I have two 6s 5000 mah Lipo's in series (25c). And a VESC and 190kv motor. And Im about 105 Ib.
```

---
## \#25 Posted by: Jinra Posted at: 2017-07-19T16:08:30.787Z Reads: 44

```
Yea 60A is fine
```

---
## \#26 Posted by: ABuildEnthusiast Posted at: 2017-07-22T01:51:03.488Z Reads: 42

```
@Jinra  The steps it provides in the product description are confusing. Can you please explain what I have to do in order? Thanks so much for your help. Here is the BMS I purchased: [http://www.ebay.com/itm/221644780045#rwid](http://www.ebay.com/itm/221644780045#rwid)
```

---
## \#27 Posted by: Jinra Posted at: 2017-07-22T02:37:42.318Z Reads: 39

```
Check out the diagrams thread, there's a lot of pictures there that will describe it much better than words. Here are some general tips though.

* P- is discharge negative (also charge negative if C- doesn't exist on your bms)
* B- is battery negative
* C- is charging negative
```

---
## \#28 Posted by: Jammeslu Posted at: 2017-08-07T12:22:02.156Z Reads: 31

```
one end of the pin is longer than the other with is pos and which is neg
```

---
## \#29 Posted by: ABuildEnthusiast Posted at: 2017-08-21T12:02:47.558Z Reads: 29

```
 @Jinra  How would I connect the balance cables? Are there any 6s converters to a 12s (Y cable).
```

---
## \#30 Posted by: Jammeslu Posted at: 2017-08-21T14:19:35.103Z Reads: 24

```
no, you have to buy a 12s bms which supports 12s
```

---
## \#31 Posted by: ABuildEnthusiast Posted at: 2017-08-21T16:03:40.235Z Reads: 21

```
I have the 12s Bms, Im just wondering how I connect the balance cables to the bms.
```

---

# Help with li ion batteries

### Replies: 8 Views: 993

## \#1 Posted by: ninja Posted at: 2017-06-24T11:52:42.564Z Reads: 134

```
Hi! 

So I've read many posts about li ion batteries, but not sure that I understund all I need. I have 8s4p 25r battery pack with 60A batterysupports.com BMS, with 2A brick charger from ebay.

1) I have 3.0v cut off start and 2.9v end on the vesc settings, so how low should I drain my battery when driving? Last time I drain it to 3.15 per cell, it's still not cut off start- its o.k to ride till 3.0v or 3.15v? Or I should count voltage sag and never go lower than 3,2v for an example? Or it's not a problem drain till cut off starts kicks in?

2) I charged my battery till green light was on laptop style charger, but when I wanted to ride- my phone with Ackmaniac app showed me 4.26v per cell :scream: So it means that it's overcharged? It means that bms not doing his job like it should? Or it is o.k. those 0.06v extra? I know that in bms parameters say that it has over charge protection 4.2 +/- 0.05v, but does those 0.05v are harmful for cells? 
 So better would be monitor voltage while charging and never go above 4.2v? How can I monitor voltige while charging? Asking because long time ago when I was in rc boats we used nimh batteries, we checked V while charging with voltmeter and numbers was compleate different vhen checking V with no charger attached vs charging. If I remember full battery was 1,5v  when charger is attached and 1,35v should be consider full battery when no charger is attached. So I don't know how to say if li ion cells are full when checking voltage while charging. 

3) After ride should I put battery to charger or it can stay drained (3.0v for an example) for x days? Or 3.0v per cell is already to low to store batt. even 2 days?
For longer storage there is storage v, that is clear.
100% full can be stored few days, isn't it?
I can put my board on charger whatever I want, I mean, even after 15 min ride I can put it on the charger if I need, isn't it? Because there is no memory on li ion cells like it is on nimh


Maybe, stupid questions, but I just didn't find 100% answers on my questions yet. 

Thanx  for your time, guys! Have a great day!
```

---
## \#2 Posted by: rojitor Posted at: 2017-06-24T12:05:06.119Z Reads: 118

```
You are doing right but..... If you want your cells to last do not charge them above 4v and do not discharge below 3.3v 
Every now and then you must make a full charge and leave the charger on over night so the bms does its function.
To check the voltage use a voltmeter, multimeter...etc they might be not accurate but will give you a hint.
About the full charge it is ok to have them fully charged for a couple weeks but if you plan to store the skate for months leave them at 3.5-3.7v or they will pay for your mistake.
```

---
## \#3 Posted by: ninja Posted at: 2017-06-25T06:32:37.350Z Reads: 87

```
Thanx @rojitor for answer, but I want hear more people thoughts about subject like @wmj259, @whitepony, @chaka, @esk8, @sl33py     

1) So 3.3v should be set like 0% on app? 
2) Even when cells are overcharged straigh afer green light kicks in on the charger, sometimes I need to leave for night to bms do his job? Does BMS not supose to balance and not overcharge before green light shows on charger? 
3) For weeks I can store at any v, for longer there is storage v and full can also be stored for week or so with no problem, Am I right?
```

---
## \#4 Posted by: esk8 Posted at: 2017-06-25T10:36:20.559Z Reads: 74

```
I have build many batteries with LG, Sony Sanyo and Samsung.
And i have al Battery charged and discharged and measure the mAh whats going in
and whats going out, before i connected with the BMS and let it work about BMS.
So i have al time the full capacity when i discharge the battery to 3.0V 
When you want the full range, so it was ok when you make the Setup 
B-Start by 3.2 V and B-End by 3.0 V.
Then yo can al time decide your self, if you ride the battery so long thats came
the cut off ore no.
When the Vesc beginning regulated the Power down so you know that you was now
by 3.2V.
You can make the setting higher, but so you became not the full mAh.
I think when you can discharge the cells to 2,5 V so i think, thats you 
have no problem with the setting 3.2-3.0 V
I have storage one Board from me over one Year and last time i measuring 
the Volt, and the cels going down from 37V to 36,8 Volt.
And thats over one Year.
```

---
## \#5 Posted by: wafflejock Posted at: 2017-06-25T10:58:11.326Z Reads: 68

```
@ninja from what I've read and experienced most of what you said is true.  The balance chargers for LiPo batteries will only bring the voltage up to 4.2V, mine is current limited so it is currently set to pull 3.6A because the 5S battery is ~21V when full so 21V*3.6A ~= 60ish Watts  and my charger is rated for 80W (it gets hot and thermal shutdown if I increase the amperage even though my batteries can handle it fine).  The charger keeps the current consistent by adjusting the voltage being applied to the battery leads, so it slowly drags the battery voltage up from wherever it is to 4.2V, at a rate of 3.6A, so if the battery is at 3.3V it will use maybe 3.5V so it controls the flow by measuring and applying the correct voltage based on the momentary voltage of each cell as far as I can tell.  Regarding the overcharge, I believe for some Li-Ion cells they have higher or lower max voltages depending on the exact chemistry, that said I'm not sure how unsafe that small amount of overcharge is for the cells you have.  Regarding storage my charger has a storage option to discharge the cells to something like 3.7-3.8V which from what I understand is important for long term life of the batteries if you plan to shelf them for more than a few days.  Regarding cells discharging on the shelf in my experience and what I've heard from others this isn't really a problem the self draining is typically very slow, have seen some guys on youtube that have had cells on a shelf for literally years and very little effect on them really, it's really the charge cycles and heat that wears on them it seems.
```

---
## \#6 Posted by: ninja Posted at: 2017-06-26T10:23:15.950Z Reads: 49

```
O.k. all is clear about storage v, about draining to 3,0v, but I still don't understund my situation with BMS!!

So when I reconnect my charger when green light shows up, in app is showing that cells are bit overcharged- 4,26v per cell. It is o.k.? bad? Should I leave for longer on charger so that BMS do his job to bring cells down to 4.2v? So BMS ir balancing only after battery is full, sounds like nonsence? 

I have batterysupport.com 8s BMS. My cut off start is 3,0v and end is 2,9v.
```

---
## \#7 Posted by: wafflejock Posted at: 2017-06-26T16:31:09.639Z Reads: 42

```
Typically with my balance charger it brings the cells up in voltage together and if they vary too much from one cell to another it will pull some charge back out of the whole pack to slowly get everything balanced.  At the end of charging as it approaches 4.2V the amperage slowly gets trickled down and it spends the last 10-15 minutes just balancing those last couple of hundredths of a volt to get everything with +/- .01V.  If you are just using an app to get the voltage info I'd use a multimeter or voltmeter to double check it to make sure it's not just giving you the wrong value.
```

---
## \#8 Posted by: wmj259 Posted at: 2017-06-28T03:57:26.820Z Reads: 34

```
I am not quite familiar with li-ion batteries so I wouldn't be much help, as well as I don't use a BMS. Sorry.
```

---

# 6S LiFePo4 - BMS and Charger Advise

### Replies: 16 Views: 1433

## \#1 Posted by: ofekp Posted at: 2017-02-15T22:37:22.609Z Reads: 109

```
Hello everyone,

Did not find many who tried that so I thought I would ask here (tell me the truth but please go easy on me, it is my first build),
As the topic suggests I want to use a 6S LiFePo4 with a 190kv motor setup (is that too low of a voltage? Is that too low of a kv motor?) for my DIY board (which I laminated myself) and I want to have the ability to charge it using a **BMS**.

#BMS
I am trying to buy one on **Bestech Power** via e-mails but I am not sure this is how I should do it, their site offers no cart!
I was specifically looking at this item:
***Battery Protection Circuit Module (PCM) for 19.2V 6 cells in series LiFePO4 Battery Packs***
http://www.bestechpower.com/192v6spcmbmspcbforlifepo4batterypack/PCB-D092.html
By the way, **BatterySupports** do not even have any 6S LiFePo4 BMS :frowning: whaaaat?
I need to add, that I intend to use the BMS for charging only and bypass the BMS for the load.
I also understood that I need it to have balanced charging functionality.
Since I am not sure if 6S is enough, I have a spare 3S battery (LiFePo4 of course, so it will fit the others) that means I would need a 9S BMS if I do decide to go that way. I do not suppose there is a way to use 9S BMS as a 6S BMS right? 

#Charger
Also, I cannot find any **LiFePo4 6S charger** in any store that has international delivery.
Can anyone suggest anything please?
Is it important to have a specific LiFePo4 charger, or can I use, say, 6S LiPo charger instead? Its all about the voltage here right?
Same question here, for 9S I will need another charger right? Can't go with a 9S charger and use, say, a voltage divider, right?

Thank you all!
```

---
## \#2 Posted by: anorak234 Posted at: 2017-02-15T23:54:34.816Z Reads: 93

```
1) you want at least 24V to run your board - go with a 9s LiFePo or 6s Li-ion
2) Forget about the charger - use a BMS, but it is tough to find LiFePo BMS's
3) If you want a great battery from the start, get one from @barajabali. Yes, it costs more. Yes, it is worth it.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-02-16T00:10:37.026Z Reads: 88

```
You've sent an email to the sales dept at Bestech. Now in a couple days they will contact you to initiate your order.
They will email you a spec sheet for approval, then you accept the settings or request any changes. Some settings are adjustable at the factory. They will also send you  an invoice. You will send payment through Paypal.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-02-16T00:12:17.458Z Reads: 84

```
[quote="ofekp, post:1, topic:17763"]
I do not suppose there is a way to use 9S BMS as a 6S BMS right?
[/quote]


Correct, the bms has to match the cell count. or it will not work.
```

---
## \#6 Posted by: ofekp Posted at: 2017-02-16T10:38:31.563Z Reads: 74

```
They did reply! They seem professional from first look, and if I can pay with PayPal then that is great!
```

---
## \#7 Posted by: ofekp Posted at: 2017-02-16T10:41:56.756Z Reads: 71

```
If I will change the motor to 245KV instead of 190KV will I be able to use my 6S LiFePo4 battery?
I am in contact with Bestech Power who seem to have what I need 6S and 9S BMSes.

Since you said a 9S would be better for me, can anyone confirm that this will be OK as a charging BMS:
http://www.bestechpower.com/288v9spcmbmspcbforlifepo4batterypack/BMS-D239.html

I already have the batteries but I will consider @barajabali the next time I will need to buy batteries, thanks!
```

---
## \#8 Posted by: ofekp Posted at: 2017-02-16T10:43:11.069Z Reads: 70

```
Right... Thanks for the confirmation! I do not know why I did not post here before...
```

---
## \#9 Posted by: Namasaki Posted at: 2017-02-16T13:03:51.858Z Reads: 64

```
I would see if they have one with higher amp capability. 8a is very low. 
It would be much better to get one you can discharge through and have short protection along with over current and over discharge protection.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-02-16T13:09:40.699Z Reads: 58

```
I highly recommend this one for charge and discharge. It is the lifepo4 version of what I've been using and it has a built in E-switch 
This is the best possible option for you. 
80a continuous 240a peak discharge 20a charge.
http://www.bestechpower.com/288v9spcmbmspcbforlifepo4batterypack/PCB-D223V1.html
```

---
## \#11 Posted by: ofekp Posted at: 2017-02-16T15:43:00.525Z Reads: 54

```
This looks really good, how important it is to have the discharge go through the BMS, I see a lot of builders choosing to bypass the BMS on discharging
```

---
## \#12 Posted by: Namasaki Posted at: 2017-02-16T16:30:18.911Z Reads: 51

```
Charge only is compromise. 
Charge and discharge is no compromise 
Charge only is minimum protection 
Charge and discharge is much more protection 
Charge only is ok
Charge and discharge is best.
Plus,
If you get a charge only BMS, you will also need a HV E-switch that cost up to $60 + shipping 
The price of this BMS is $50 + shipping
```

---
## \#13 Posted by: Namasaki Posted at: 2017-02-16T17:19:35.796Z Reads: 52

```
My opinion is that you should never skimp on batteries, electronics or motors.
```

---
## \#14 Posted by: ofekp Posted at: 2017-02-20T10:00:22.911Z Reads: 49

```
OMG, they want me to buy two of them because "They are not made by SMT"...
Any ideas, what I can do to make them sell me just one piece?
Maybe other suggestions for something that is made by SMT? whatever that means...

Thanks!
```

---
## \#15 Posted by: Namasaki Posted at: 2017-02-20T13:25:06.150Z Reads: 47

```
SMT surface mount technology 
Every order at Bestech is a custom order because they give you options in the specifications  that are very important and no other BMS maker gives you that. So their min order is 2. So you buy 2 and save one for a backup or a future build or sell it on the forum.
Or you buy a battery supports with no options and then spend the additional $60 for an external 
e-switch that you will need since battery supports is a bare bones BMS.
```

---
## \#16 Posted by: ofekp Posted at: 2017-02-20T13:53:43.166Z Reads: 45

```
:slight_smile: Thank you man.

This is what I will buy, can you confirm that it is OK please?
http://bestechpower.com/192v6spcmbmspcbforlifepo4batterypack/BMS-D223V1.html
http://www.bestechpower.com/288v9spcmbmspcbforlifepo4batterypack/PCB-D223V1.html

They are both what you suggested, just that one is for 6S and one is for 9S, both are for LiFePo4

Thanks again!
```

---
## \#17 Posted by: Namasaki Posted at: 2017-02-20T15:19:49.997Z Reads: 44

```
Those are the ones. 
When they send you a spec sheet for approval, you need to request your custom settings. 
If you need help with that. I will help you later when I get home from work
```

---

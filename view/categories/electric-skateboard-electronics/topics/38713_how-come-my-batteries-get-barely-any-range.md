# How come my Batteries get barely any range?

### Replies: 17 Views: 817

## \#1 Posted by: mgertner Posted at: 2017-11-18T23:06:12.047Z Reads: 116

```
So i built a board a month or s ago and then i got some major upgrades (like a bms) and put them on last weekend. I realized i didn't have a charger with enough voltage to charge my batteries. So i bough this charger here off amazon:

https://www.amazon.com/LM-YN-Transformers-Interface-Communications/dp/B01LXBQVRY/ref=sr_1_1?ie=UTF8&qid=1511045977&sr=8-1&keywords=32+volt+power+supply

I chopped off the connector it came with and put an xt60 connector to the cord. My issue is that when i plug it in, it progressively charges slower, but when i go to ride it after my indicator says a decent percent (around 50%), i barely made it around my block which is about 0.4 miles (0.7 km) and then it just completely died. Maybe i wired the BMS incorrectly or i need a charger like this: 

https://www.amazon.com/33-6V-Smart-Battery-Charger-Li-ion/dp/B0759YN37J/ref=sr_1_1?s=electronics&ie=UTF8&qid=1511046286&sr=1-1&keywords=33.6+volt+charger

Let me know your thoughts as this would be greatly appreciated!
```

---
## \#2 Posted by: willpark16 Posted at: 2017-11-18T23:06:56.613Z Reads: 107

```
We don't even know what battery ur using
```

---
## \#3 Posted by: mgertner Posted at: 2017-11-18T23:08:01.292Z Reads: 104

```
2x Zippy flightmax 5000mah 4cell lipo in series
```

---
## \#4 Posted by: b264 Posted at: 2017-11-18T23:08:19.607Z Reads: 105

```
Tell us more about the battery.  What kind is it?  How many cells does it have?  Can you photograph it?
```

---
## \#5 Posted by: evoheyax Posted at: 2017-11-18T23:08:22.572Z Reads: 100

```
You need the second one...

You can't charge lithium batteries with a direct voltage like that, theres multiple phases to charging with lithium batteries.
```

---
## \#6 Posted by: mgertner Posted at: 2017-11-18T23:11:08.727Z Reads: 98

```
Ok. So i need a specific charger for lithium batteries?
```

---
## \#7 Posted by: evoheyax Posted at: 2017-11-18T23:11:09.778Z Reads: 96

```
**Li-ion battery charging**

Charging lithium ion batteries can be split into two main stages:

- Constant current charge:   In the first stage of charging a li-ion battery or cell, the charge current is controlled. Typically this will be between 0.5 and 1.0 C. (NB: for a 2 000 mAh battery the charge rate would be 2 000 mA for a charge rate of C). For consumer based LCO cells and batteries, a charge rate of a maximum of 0.8C is recommended.

During this stage the voltage across the lithium ion cell increases for the constant current charge. The charge time may be around an hour for this stage.

- Saturation charge:   After a time the voltage peaks at 4.2 Volts for an LCO cell. At this point the cell or battery must enter a second stage of charging known as the saturation charge. A constant voltage of 4.2 volts is maintained and the current will steadily fall. The end of the charge cycle is reached when the current falls to around 10% of the rated current. The charge time may be around two hours for this stage dependent upon the type of cell and the manufacturer, etc..

From http://www.radio-electronics.com/info/power-management/battery-technology/lithium-ion-battery-charging.php
```

---
## \#8 Posted by: evoheyax Posted at: 2017-11-18T23:11:39.747Z Reads: 89

```
Yes, the second one is just that.

What happened is you got to the end of the first stage, but never entered the second stage, because that charger can't do the second phase, only the first.
```

---
## \#9 Posted by: mgertner Posted at: 2017-11-18T23:13:33.332Z Reads: 83

```
Ok that link you sent made a lot of sense. So that charger will essentially l slowly increase from 29.6 volts to 33.6 volts?
```

---
## \#10 Posted by: evoheyax Posted at: 2017-11-18T23:14:20.806Z Reads: 83

```
yes. 10char
```

---
## \#11 Posted by: mgertner Posted at: 2017-11-18T23:15:15.375Z Reads: 78

```
Ok thank you so much.
```

---
## \#12 Posted by: mgertner Posted at: 2017-11-18T23:23:59.556Z Reads: 74

```
Wait, even if I have a BMS wired with the batteries?
```

---
## \#13 Posted by: evoheyax Posted at: 2017-11-19T00:07:37.127Z Reads: 64

```
Yes, get the right charger and if you havn't already messed up your battery, all will work fine.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-11-19T00:18:30.808Z Reads: 62

```
You can charge the batterys also with a normal power supply. As long as it doesn't exceed the voltage of 4.2 a cell it will be fine. The 2 phases happen automatically when the power supply doesn't exceed the voltage. So in the first phase it will be regulated by the current (voltage is lower than 4.2V a cell) and when it reached 4.2V a cell the current will decrease automatically because higher current can only be achieved with higher voltage.
Guess the issue with the power supply of mgertner is that when it can't achieve 32V it shuts down or something like that.
```

---
## \#15 Posted by: mgertner Posted at: 2017-11-19T00:46:51.590Z Reads: 54

```
So you’re saying that a 32 volt charger should work fine, but something with the charger itself is causing it to shutdown or something.
```

---
## \#16 Posted by: MysticalDork Posted at: 2017-11-19T00:49:58.454Z Reads: 46

```
No. Get a real charger. If you still have problems once you have a real charger, come back to us and we'll help you.
```

---
## \#17 Posted by: mgertner Posted at: 2017-11-19T00:51:23.929Z Reads: 42

```
Just ordered it.
```

---

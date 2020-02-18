# Battery charges to 42V when charger plugged in but 40.7V after plugged out

### Replies: 19 Views: 711

## \#1 Posted by: nikoli280 Posted at: 2018-04-15T10:19:55.476Z Reads: 120

```
Hi Everyone i have made a 10S pack with a BMS. I normally charge the battery with a 42V brick charger, but it charges to 42V and then when i unplug the charger the battery is around 40.7V i know that the battery voltage is increased when a 42V power source is in. But the charger turns off at 42V, So i can not get the pack up to 42V. Is this normal or can i fix it some how?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-04-15T10:28:06.012Z Reads: 120

```
I Would try just leaving it in for a while as the pack my be charging just very slowly. It does seem a little odd though. What charger are you using?
```

---
## \#3 Posted by: nikoli280 Posted at: 2018-04-15T10:31:12.972Z Reads: 121

```
There is no current running through the leads. I am using a standard 42V 3A brick charger from Aliexpress.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-04-15T10:34:52.462Z Reads: 118

```
It might just be that the charger has a cheap voltage sensor and cuts off too early. Do you have another battery to test on? Or another charger to test the battery with?
```

---
## \#5 Posted by: nikoli280 Posted at: 2018-04-15T10:37:33.625Z Reads: 117

```
I have just tried to charge the battery the rest way with a lab bench power supply, and that has no problems with charging it the last 1V. So it seems that the brick charger turns up the voltage of the battery pack when charging so it makes the bms turn of charging and then when unplugged the voltage drops.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-04-15T10:50:36.831Z Reads: 108

```
That is very weird. I would be careful using a lab power supply. Make sure it has cc/cv charging mode
```

---
## \#7 Posted by: nikoli280 Posted at: 2018-04-15T10:53:55.967Z Reads: 102

```
The lab bench has CC/CV what does that mean? I have left the lab bench on at 42V and the current draw has fallen from 4A to now 0.8A with 42V constant
```

---
## \#8 Posted by: pat.speed Posted at: 2018-04-15T10:57:19.575Z Reads: 96

```
Yep that’s what cc/cv does. It means constant current / constant voltage. Basically it it charges at s fixed rate until it hits the set voltage then holds that voltage and decreases current to a very low amount
```

---
## \#9 Posted by: nikoli280 Posted at: 2018-04-15T10:58:47.594Z Reads: 97

```
A okay that is maybe what my brick charger is missing. Since it has no problems with charging up to it hits 42V but when unplugged the battery still misses some voltage which is what the CV does take care of. Is there a way to moddifie or to fix
```

---
## \#10 Posted by: Tuomalar Posted at: 2018-04-15T11:10:35.146Z Reads: 83

```
Check your cell voltages. BMS might cut off charging if some cellgroup is above 4.2V
```

---
## \#11 Posted by: nikoli280 Posted at: 2018-04-15T11:11:15.114Z Reads: 81

```
The BMS is not the problem since i can charge the pack to 42V with my lab bench with CC/CV
```

---
## \#12 Posted by: pat.speed Posted at: 2018-04-15T11:16:13.361Z Reads: 77

```
Well I know that some chargers have a little knob inside them that adjusts the output voltage, you could always open it up and see.

On the bright side though at least you will get lots more charge cycles by only charging to 4.07v per cell
```

---
## \#13 Posted by: nikoli280 Posted at: 2018-04-15T11:22:23.632Z Reads: 72

```
That is true and i have a big battery so i can get 20-30 km on the charge i have now so its possible i just dont know if the pack is ballanced or it will first be that when charging the last current around 42V
```

---
## \#14 Posted by: pat.speed Posted at: 2018-04-15T11:25:01.388Z Reads: 71

```
Oh yes I forgot about that. The bms may not balance the cells properly if they don’t reach ~4.2v
```

---
## \#15 Posted by: nikoli280 Posted at: 2018-04-15T11:49:45.426Z Reads: 67

```
Hmm i dont see how i can fix this
```

---
## \#16 Posted by: Jebe Posted at: 2018-04-15T12:13:08.879Z Reads: 64

```
Sounds like a failed cell
Can you measure across each individual cell? Should be balanced.
What happens to the voltage if you put load on the battery?
```

---
## \#17 Posted by: nikoli280 Posted at: 2018-04-15T12:16:12.970Z Reads: 62

```
The pack can be charged to 42V without problems with my lab bench power supply with CC/CV but not with the brick so its not a bad cell, the constant V of the pack without charge is now 42V.

When i use the pack the voltage stays around the same with a very small decrease in high power usage
```

---
## \#18 Posted by: sayreul Posted at: 2018-05-04T12:35:21.141Z Reads: 45

```
hello 
same issue for me
i made a 10S3P with Nkon cells Sony VTC6 

I use a Aliexpress 42V 2A charger. the charger turn green when the battery is 40.7. 

I thought it was a BMS problem, I sent the battery to a guy who charged all cells and change the BMS. with his charger it was ok. 
he sent me back the battery and advise me to buy a new charger. I ordered another 42V 4A on AliExpress, 
this new charger also stop at 40.7 ... 

not lucky with charger or cells problems ?
```

---
## \#19 Posted by: sayreul Posted at: 2018-05-04T12:43:04.423Z Reads: 45

```
hello 
same issue for me
i made a 10S3P with Nkon cells Sony VTC6 

I use a Aliexpress 42V 2A charger. the charger turn green when the battery is 40.7. 

I thought it was a BMS problem, I sent the battery to a guy who charged all cells and change the BMS. with his charger it was ok. 
he sent me back the battery and advise me to buy a new charger. I ordered another 42V 4A on AliExpress, 
this new charger also stop at 40.7 ... 

not lucky with charger or cells problems ?
```

---

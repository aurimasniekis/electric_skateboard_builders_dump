# Charging 2 x 3s Batteries in series

### Replies: 13 Views: 1684

## \#1 Posted by: Sleepingalex24 Posted at: 2016-10-22T23:07:44.941Z Reads: 122

```
Hey everybody! I have already built my board and it works great but there are a few improvements I want to make. 1. I want a way to tell how much farther I can ride. 2. I want to be able to charge without taking everything out. I am planning on doing this by adding a voltmeter and also creating some charging ports. This is the layout I'm thinking about doing:<img src="/uploads/db1493/original/3X/1/8/182a893bb0a5d0ffbfe5773bc71ec128c48ada98.png" width="690" height="388">
I just wanted to know if all of this would work correctly. I'm not so sure about the XT60 charging port. Would I have to plug an XT60 key in there in order for the circuit to be close or would it work without one?
```

---
## \#2 Posted by: Aborn Posted at: 2016-10-22T23:12:32.891Z Reads: 117

```
This is not charging in series, if you plug this into a 6 cell balance charger you will be just fine

*i could be wrong*
```

---
## \#3 Posted by: Sleepingalex24 Posted at: 2016-10-22T23:16:11.980Z Reads: 113

```
Oh wouldn't I be charging 2 batteries in series as one though?
```

---
## \#4 Posted by: Aborn Posted at: 2016-10-22T23:19:11.619Z Reads: 107

```
No because your balance charging connector in this picture has 7 leads, 
1 negative lead and 6 positives, one for each cell. this way you can balance all 6 cells individually (with you i mean your charger)

connecting them in series would be using a 4 lead charge connector and connecting 2 cells to each lead, that would be a bad idea as the charger wouldnt be able to balance the cells probably.
```

---
## \#5 Posted by: Sleepingalex24 Posted at: 2016-10-22T23:21:27.738Z Reads: 101

```
Ok I see now. Alright thank you so much!
```

---
## \#6 Posted by: Aborn Posted at: 2016-10-22T23:22:28.008Z Reads: 94

```
*Wait for someone else to confirm this though*
```

---
## \#7 Posted by: benwong Posted at: 2016-10-23T07:34:02.758Z Reads: 84

```
i have a same questions also. 
i have 2 4S and 8S balance charger, i wan to charge in series. 
My two lipo had using series [XT60](http://www.hobbyking.com/hobbyking/store/__10264__XT60_Harness_for_2_Packs_in_Series_1pc_.html) to connect as 8S as my setup is 8S. 
Just wondering how to i modify the balance lead port. 
9lead or 5lead?
```

---
## \#8 Posted by: chinzw Posted at: 2016-10-23T08:06:30.659Z Reads: 82

```
The diagram above is correct for 6s charging of 2x3s batteries. What you are refering to would be parallel charging.
But be carefull, in that diagram the balance leads are inverted, the battery that has the negative lead going to the vesc should have the negative balance lead and the positive battery leading to the vesc should have the positive balance lead.

Once you have everything wired up, before connecting anything use a multimeter to test your balance lead. With the negative multimeter probe on the negative balance pin start moving the positive probe 1 pin at a time, you should get 4.2v, 8.4v, 12.6v, 16.8v, 21v, 25.2v on fully charger batteries.
```

---
## \#9 Posted by: AlenJk Posted at: 2016-11-16T08:23:08.963Z Reads: 59

```
This is a wrong way, Charging a [3s battery](http://www.genstattu.com/3s-11-1v-lipo-battery.html) need a 11.1v charger, but you have two 3s batteries in series, so you need a 6s balance charger to charge them.
```

---
## \#10 Posted by: tueboard Posted at: 2016-11-16T08:55:27.900Z Reads: 60

```
i can charge two 3s batteries in series at 2.0A with this:

turnigy charging harness 2 x 3s
http://www.ebay.es/itm/261417566979

turnigy accucell balance charger 80W
https://hobbyking.com/en_us/turnigy-accucel-6-80w-10a-balancer-charger-lihv-capable.html

power supply 12V-24V
https://www.amazon.es/gp/product/B015IVALEU
```

---
## \#12 Posted by: chinzw Posted at: 2016-11-16T16:20:09.948Z Reads: 54

```
Erm, not its no the wrong way. He never mentioned what type of charger he had, but almost all hobby chargers are 6s anyways.
```

---
## \#13 Posted by: danyCRO Posted at: 2019-05-06T19:33:00.388Z Reads: 14

```
[img]http://www.rcuniverse.com/forum/attachment.php?attachmentid=1312340&d=1375486401
[/img]
Hi. What is defference with diagram above and this diagram in balance cable? Is better cut of (+)red wire or (-) black wire?
```

---
## \#14 Posted by: danyCRO Posted at: 2019-05-12T11:15:38.221Z Reads: 10

```

Anybody here??
```

---

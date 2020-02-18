# Powering a BMS 6s

### Replies: 17 Views: 694

## \#1 Posted by: Armitage Posted at: 2018-04-08T08:27:52.647Z Reads: 52

```
Hello, so I am new to the bms territory. If I have a 6s BMS that is labeled as 25.2V, can I use it with a lower voltage power supply? For example, would a 24v power supply work?
```

---
## \#2 Posted by: e.board_solutions Posted at: 2018-04-08T08:47:58.347Z Reads: 50

```
yes, but you will not charge your batteries 100%
```

---
## \#3 Posted by: E1Allen Posted at: 2018-04-08T08:48:08.198Z Reads: 49

```
Up to 24v.  It wouldn't fully charge the batteries
```

---
## \#4 Posted by: e.board_solutions Posted at: 2018-04-08T08:49:02.566Z Reads: 49

```
And it needs to be a charger not a powersupply
```

---
## \#5 Posted by: pat.speed Posted at: 2018-04-08T08:58:37.661Z Reads: 41

```
It will not balance the cells if only charged to 24v as most bms modules balance the cells at around 4.19v
```

---
## \#6 Posted by: Armitage Posted at: 2018-04-08T09:03:24.526Z Reads: 38

```
Okay, but where can I get a cheap 25.2v charger for the bms?
```

---
## \#7 Posted by: pat.speed Posted at: 2018-04-08T09:04:52.256Z Reads: 36

```
eBay, Amazon, AliExpress and banggood I think have them
```

---
## \#8 Posted by: Zimbombe Posted at: 2018-04-08T09:06:06.543Z Reads: 36

```
https://www.banggood.com/25_2V-2A-Smart-Charger-For-21_6V-22_2V-25_2V-Li-ion-Li-Po-Lithium-Battery-US-Plug-p-1167937.html?rmmds=myorder&cur_warehouse=CN

not high quality but it does the job.
```

---
## \#9 Posted by: b264 Posted at: 2018-04-08T09:18:52.363Z Reads: 31

```
You can't use a power supply to charge lithium batteries.  It needs to be a lithium charger.  Lithium chargers run in constant current mode (with variable voltage) until target voltage is reached, then change to constant voltage (variable current)
```

---
## \#10 Posted by: Armitage Posted at: 2018-04-08T09:22:11.757Z Reads: 31

```
Thanks for that!
```

---
## \#11 Posted by: Zimbombe Posted at: 2018-04-08T09:36:55.260Z Reads: 29

```
If he has a 6s Li ion Pack with a BMS he can use the power supply i linked ?! the bms should step down the constant when the cells are nearly full. 

Pls tell me if i´m miss conceptioning something.
```

---
## \#12 Posted by: Acido Posted at: 2018-04-08T09:38:48.250Z Reads: 29

```
If it is a bestech bms it will balance when any of the end voltages has been hit on any cell
```

---
## \#13 Posted by: pat.speed Posted at: 2018-04-08T09:41:08.224Z Reads: 28

```
Yes but it won’t balance them properly because they will all be around 4v per cell which isn’t even close to 4.2v
```

---
## \#14 Posted by: Acido Posted at: 2018-04-08T09:42:19.633Z Reads: 28

```
Yes, anyways the problem is not the bms it is his power supply
```

---
## \#15 Posted by: pat.speed Posted at: 2018-04-08T09:43:50.476Z Reads: 28

```
Yep, totally agree with that. Unless you can lower the balance voltage to 4v it won’t work very well. He would also lose range because the pack won’t be getting its full capacity
```

---
## \#16 Posted by: b264 Posted at: 2018-04-08T09:45:31.028Z Reads: 29

```
[quote="Zimbombe, post:11, topic:51559, full:true"]
If he has a 6s Li ion Pack with a BMS he can use the power supply i linked ?! the bms should step down the constant when the cells are nearly full.

Pls tell me if i´m miss conceptioning something.
[/quote]

You did not link a power supply.  You linked a lithium charger.
```

---
## \#17 Posted by: Armitage Posted at: 2018-04-09T14:44:51.571Z Reads: 20

```
So  I just have to connect the power supply to the bms?

https://www.banggood.com/25_2V-2A-Smart-Charger-For-21_6V-22_2V-25_2V-Li-ion-Li-Po-Lithium-Battery-US-Plug-p-1167937.html?rmmds=myorder&cur_warehouse=CN
```

---

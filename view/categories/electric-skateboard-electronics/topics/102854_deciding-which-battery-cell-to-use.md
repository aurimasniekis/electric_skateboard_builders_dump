# Deciding which battery cell to use?

### Replies: 9 Views: 182

## \#1 Posted by: YoddlingTaco Posted at: 2019-10-12T12:52:24.106Z Reads: 58

```
Hello! I'm making my meepo mini 2 smaller by getting a smaller battery and different enclosure so that I dont get in trouble with the German polizei. Right now I have a 10s2p battery, I want to switch to a smaller 10s1p. I can either buy the meepo 10s1p with 25R cells, or a custom 10s1p with 30Q cells. Which battery cell is better? I have the meepo Hobbywing 12A ESC. Also, does a BMS help reduce voltage sag, or does it make no difference?
```

---
## \#2 Posted by: BillGordon Posted at: 2019-10-12T12:59:38.073Z Reads: 58

```
30Q definitely better. Sag comes comes from cells falling off during discharge, not the BMS.
```

---
## \#3 Posted by: Chaki Posted at: 2019-10-12T13:06:41.216Z Reads: 58

```
30Q is 3ah
40T is 4ah - a bit more $$

Both is a good choice.
```

---
## \#4 Posted by: Voxu Posted at: 2019-10-12T15:56:02.246Z Reads: 54

```
30Q>25R 100% for sure. Samsung 30q cell is all around the best cell to use. I would say there are 3 top cells people use. Samsung 30q most "balanced" cell in size, price, discharge, sag and capacity. Then there is a VTC6 for more power and Sanyo cells (like in Tesla cars) for range. 

BMS=Battery management system. It's purpose is to balance all the cells to the same voltage. You can also use BMS for discharge which adds over-current protection for example. It also adds size (discharge grows with size of the BMS) I personally run/will run... (long story) bypassed BMS which only balances my cells while charging but it doesn't discharge through it. That means that I can run as much current as I want with a bypassed BMS.
```

---
## \#5 Posted by: BillGordon Posted at: 2019-10-12T16:28:23.631Z Reads: 49

```
Nicely explained.
```

---
## \#6 Posted by: deucesdown Posted at: 2019-10-14T01:08:18.081Z Reads: 32

```
[quote="YoddlingTaco, post:1, topic:102854"]
Hobbywing 12A ESC.
[/quote]

Is that 12a per side or total? 1p packs of 25r or 30q can handle about 20a. If its 24a total you might consider a differert cell like vtc5a or 30t.
```

---
## \#7 Posted by: Anubis Posted at: 2019-10-14T11:44:13.587Z Reads: 24

```
12A motor amps though so you could run that on a 1A battery if you wanted, hell it wouldn't even get bottlenecked that hard. Obviously an extreme example but still, duty cycle.
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-10-14T12:32:52.626Z Reads: 22

```
Wait chinese ESCs dictate motor current? 

I was always under the impression that the value shown was batt max for one side :o
```

---
## \#9 Posted by: Anubis Posted at: 2019-10-14T12:39:41.880Z Reads: 20

```
They do have duty cycle I belive. I ran a 40A yingli with a 20A battery and experienced the same power when I switched over to a 50A battery (In the low range ofc, at times it was bottlenecked)
```

---

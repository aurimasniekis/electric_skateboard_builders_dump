# BMS Not Balancing Properly

### Replies: 3 Views: 748

## \#1 Posted by: NickTheDude Posted at: 2017-09-09T16:45:47.289Z Reads: 84

```
Hey guys, I've had a couple BMSs now and both seem to have the same problem. The cells only really get charged to around 4.16-4.18 and never actually get balanced. I've heard that most BMSs are set to start balancing after 4.2, and this might be why it's not working.

Does anyome else have this problem? Any ideas to fix it or do you know of any BMSs that balance correctly?
```

---
## \#2 Posted by: Silverline Posted at: 2017-09-09T18:45:25.845Z Reads: 74

```
I would look at your Charger. It's the Charger that decides when the voltage is high enough to stop charging. Lets say that you have a 10s charger, then it should charge to the voltage reach 42volt. But if the Charger is imprecise and stops at 41volt , that could course the problem.
```

---
## \#3 Posted by: Tomash Posted at: 2017-09-09T18:57:47.742Z Reads: 66

```
When i first charged my new LiPO 8S  battery. 
BMS was cutting down/switching off charger to early, the total battery charge was about 33,53V , and should be 33,6 V for 8S and i had for example:
1 cell charged to 4,23
2 cell to 4.20
rest of the cells from 4.19 to 4.16
( i checked them with multimeter)

I thought something was wrong with bms. But after about 2 or 3 charge/use cycles, voltages for each cell corrected, and i was able to fully charge my battery.

In my case, i think it was a problem with very unbalanced cells, with big voltage diffrences or maybe BMS had to "learn" the battery :slight_smile:.

In your case, it may also be the case. 
Try to charge and discharge the battery with your bms few times. And use compatible charger, with right voltage.

Best for you would be to check with mulitimeter each cell, and if it's possible, charger voltage - if it's correct, and what is the total battery voltage after charge.
For example, my 8S battery, after charge have 33,6 Volts. (8x 4,2 V) Each cell is full at 4,2 Volts.

Or maybe you are unlucky to have a bad cell in battery, or faulty bms, hope it's not that problem.

Some bms'es have blue led diods, that inform you if a cell is bad or bms is balancing.
On my bms, after i charge, those diods, are flashing blue.
But if BMS and battery are ok, after some time (it can be minutes or few hours), all led lights should stop flashing and go blank. (no light at all), and that mean everything is ok with battery and bms.
But not all BMS's have those diods.
```

---

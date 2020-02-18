# Can&rsquo;t get my head around BMS&rsquo;

### Replies: 9 Views: 221

## \#1 Posted by: Marsh369 Posted at: 2019-01-20T03:56:51.138Z Reads: 95

```
I have been looking into building my own board and have been doing a ton of research. I know most of what the parts I am going to need and just need to look I to some of the smaller parts. 
I just can't figure out what BMS I need to be using for my setup. The motor is going to be a Turnigy 6354 200 kV with max 55A. The VESC is 60A continuous and 150A instantaneous. I will hopefully be running 10s2p Sony VTC5's. 
So do I need a BMS that is the same as the continuous Amps of the pack, so 60A, or does it need to be higher? And does it have to be able to handle the charge Amps of the motor if using regenerative braking?
Any help will be greatly appreciated 😁.
```

---
## \#2 Posted by: M.Hboards Posted at: 2019-01-20T04:03:00.671Z Reads: 90

```
there are 2 two ways to wire your bms charge and discharge which you will need a more expensive bms for and charge only which almost any 10s bms will work for. use the search button you could fined most of the info you need there.
```

---
## \#3 Posted by: janpom Posted at: 2019-01-20T04:03:06.030Z Reads: 88

```
You only need to worry about the current rating if you are going to use the BMS for discharge protection. We often use BMS only for charging (bypassed). Then the current rating doesn't matter.
```

---
## \#4 Posted by: janpom Posted at: 2019-01-20T04:16:08.461Z Reads: 81

```
If I simplify, you can think about the BMS as a device with two switches. One switch cuts off charging, which typically happens when battery cells are full to prevent overcharging. We always use this. 

The second switch cuts off discharge. This can happen when too much current is drawn from the battery or when the the battery voltage gets too low (to prevent overdischarge). We sometimes use this and sometimes not.

The BMSes to be bypassed (charge only) are typically smaller and cheaper. You get undervoltage protection from a VESC, so you don't really need the BMS for that. Bypassed you're mainly loosing the overcurrent/short-circuit protection. On the other hand, you don't risk that the BMS cuts power supply because it thinks there's a problem when there's actually not (which can be dangerous in some situations).
```

---
## \#5 Posted by: Marsh369 Posted at: 2019-01-20T04:26:52.470Z Reads: 68

```
Right that makes sense, didn't think about bypassing the discharge. But do I still need to take regenerative braking into account?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-20T04:55:15.039Z Reads: 65

```
No.
Your bms is wired parallel to the load.
If you break your bms will not see any load.
You only need to worry about the current of your battery charger.
```

---
## \#7 Posted by: Marsh369 Posted at: 2019-01-20T05:23:41.913Z Reads: 59

```
Right ok, so if I get a BMS that has a 2A charge current and a 10s 2A charger I should be good. Given my capacity should take it just over 2 and a half hours to charge. 
Now if I plan to add more batteries in the future (say 10s4p) I can still use the same BMS but the charging time will double?
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-01-20T05:32:03.175Z Reads: 53

```
Yes, that's correct.
```

---
## \#9 Posted by: Marsh369 Posted at: 2019-01-20T23:49:08.789Z Reads: 28

```
Thanks guys, now I just need to get a couple more parts ordered and I can maybe start a build thread 😁
```

---

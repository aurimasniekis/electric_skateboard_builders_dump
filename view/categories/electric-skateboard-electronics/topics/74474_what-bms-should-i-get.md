# What BMS should I get?

### Replies: 7 Views: 203

## \#1 Posted by: Doodles Posted at: 2018-11-12T21:19:39.971Z Reads: 76

```
Hello. I am brand new to building and electric skateboard and I am trying to figure out what parts to get. I am interested in the Zippy Flightmax 4200mAh 3S1P 30C LiFeP04 Pack on Hobby King but I don’t know what BMS to get that goes with the battery’s. I will have two of these batteries. What charger and what BMS should I get? I am new so I am sorry if I am being dumb. Just tying to figure out what works well. Thank you!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-11-12T23:57:52.826Z Reads: 60

```
hi mate, firstly, you're not being dumb. you're just not making use of the thousands of threads that are available to you.
Do some reading
Secondly, running 4200mah at 6s will get you maybe 8km or so of range, which really isn't much. 
At 6s, there are alot of bms' available. It is up to you if you want to run charge AND discharge through the bms, or charge only. Charge only bms' are far smaller and cheaper, yet you have to be sure that all cells are fine after charging. (eg i run discharge through my 80a bms and was experiencing cut offs due to one cell being at 3.0v and all others at 3.8v). Running discharge just adds that little bit of protection. 
Bestech and Supower make a good bms.
```

---
## \#3 Posted by: Gustdd Posted at: 2018-11-13T00:17:56.636Z Reads: 53

```
Hi, I'm basically in the same situation as @Doodles. I'm thinking about building a 12s system, but I have some questions about the BMS. If I have a 12s 8AH 12C (peak 24C) battery I need a BMS with 200A discharge to get the maximum out of my batteries right? That would be something like 80€. Could I just charge my batteries with a iMAX (they are two separate 6s packs) which goes for 20€?
```

---
## \#4 Posted by: ShutterShock Posted at: 2018-11-13T00:52:06.655Z Reads: 38

```
I mean tbh unless you are a huge guy you probably don't need over 80A battery discharge.  I have a 60A discharge, 12S, dual motor and I barely reach 60 on max accelleration.

Motor amps and battery are very different
```

---
## \#5 Posted by: mynamesmatt Posted at: 2018-11-13T02:18:40.248Z Reads: 34

```
@Gustdd you won't need over 80a. anything between 60 and 80a will be just fine. or you can run charge only and then it doesn't matter
```

---
## \#6 Posted by: Gustdd Posted at: 2018-11-13T08:00:00.618Z Reads: 26

```
But why not? From my calculations battery max would be way higher than 80A. If the BMS is going to be the limiting factor I would rather go without.
```

---
## \#7 Posted by: mynamesmatt Posted at: 2018-11-14T03:08:50.918Z Reads: 18

```
if you're using vesc 4 or focbox you'll never really draw more than 40a from each esc. so whem in parallel it'll be 80a. you can cap this off in the vesc tool but you can still floor your motor Max (eg mine can go to 100a motor Max, but i run 40a batt max)
Your esc will limit the current throughput anyways so you only need what the esc can take
```

---

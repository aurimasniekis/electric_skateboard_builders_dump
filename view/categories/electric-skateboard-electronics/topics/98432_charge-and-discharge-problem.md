# Charge and discharge problem

### Replies: 10 Views: 154

## \#1 Posted by: Skatebro1 Posted at: 2019-07-14T10:00:23.876Z Reads: 53

```
Hey! I started making my first board in good faith, however now I am stuck. First I connected everything together (Batteries (Samsung 30q 3000mAh 3,6v 10s2p) , BMS(36v), vesc (8V- 60v), controller and motor) and it worked! Then I plugged the charger into the battery just to check that the charger worked. The light became red and then I unplugged it since it seemed to work. Later I resoldered some connections since I had too long wires.

My problem is that I don´t understand what possibly could be wrong. The first issue is that I can´t charge the battery. I think that could be because the BMS is only rated for 36V and it is blocking the 42V charger, but that does not explain why the VESC won´t turn on. Currently I have 25.7 V coming from the battery to the VESC. Could all my problems be related to the 36V BMS, and do you think that it will work with a 42V BMS?

![11|444x500](upload://mEpRFJ7UOb7h5gwLBcQFUaJHG06.png) 
![IMG_2753-kopi|375x500](upload://urKm2xUHb7Ggr1cEPCkvixOyYRE.jpeg)
```

---
## \#2 Posted by: L3chef Posted at: 2019-07-14T10:54:01.059Z Reads: 45

```
Link to the bms? You should re solder the wires again. That doesn't look safe with strings sticking out everywhere.
Also your jst connector from balance wire is lot plugged in all the way
```

---
## \#3 Posted by: Skatebro1 Posted at: 2019-07-14T12:08:14.303Z Reads: 43

```
This is the one I have currently:
https://www.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell/311862435323?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

This is the one I am thinking to buy:

https://www.ebay.com/itm/36V-37V-42V-10S-45A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System/322445471781?hash=item4b133f7025:g:tDYAAOSwkHFb85js

The jst connector is all the way in I think, just a poor quality BMS.
I will resolder my connections :+1:
```

---
## \#4 Posted by: L3chef Posted at: 2019-07-14T12:29:43.447Z Reads: 40

```
Are you sure you want to go with those cheap bms? Since you are using them both for charge / discharge.. This one I been using for 3 years without any issues. It's on the cheaper side aswell..
https://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/221769582503
```

---
## \#5 Posted by: Skatebro1 Posted at: 2019-07-14T12:42:37.574Z Reads: 39

```
I will try that :+1: thank you so much for your help.

But are you using a 42v charger on your pack?
```

---
## \#6 Posted by: L3chef Posted at: 2019-07-14T13:06:49.035Z Reads: 34

```
Np.
Yes 42v charger. You have 2p battery pack so try to find a charger between 1 and 2a
```

---
## \#7 Posted by: Skatebro1 Posted at: 2019-07-14T17:24:51.393Z Reads: 32

```
I already have a 2a charger :) thanks a lot
```

---
## \#8 Posted by: accrobrandon Posted at: 2019-07-15T12:40:59.796Z Reads: 19

```
Did/do u get a bms cutoff for full battery regen braking? I got this bms for a budget battery build I did... Only time ive ever had brakes cut out while using focbox.... After I bypassed the bms and wired it for charge only the issue went away... Just curious..never had issues with my bestech
```

---
## \#9 Posted by: L3chef Posted at: 2019-07-15T13:28:14.004Z Reads: 15

```
I never got a cutoff ever. But I don't charge my battery to 42v either..
```

---
## \#10 Posted by: ShutterShock Posted at: 2019-07-15T16:39:36.601Z Reads: 14

```
This BMS is made by SuPower (batterysupports.com) originally but they also are sold on ebay.  Very reliable, only company I trust with my batteries at the moment.
```

---

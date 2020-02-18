# CC-CV Charging question

### Replies: 6 Views: 1641

## \#1 Posted by: brabbit Posted at: 2016-06-26T23:34:59.736Z Reads: 135

```
I want to build a custom 10S5P battery pack for my build. I want to use the following parts:

**50 LG HG2 Cells**

**BMS:** 
http://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/221769582503?hash=item33a27f47a7:g:VV0AAOxywCJRa-m2

**AAANNNDDDD either one of these power supplies:**
http://www.ebay.com/itm/500W-48V-10A-220V-INPUT-Single-Output-Switching-power-supply-for-LED-Strip-light-/252414466576?hash=item3ac5131a10:g:UUAAAOSwjwlXBLtn
OR
http://www.ebay.com/itm/Lithium-Ion-Battery-Charger-Li-ion-LiPo-10S-42V-2A-for-36V-37V-Wall-Socket-AC-DC/321555510511?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D20131003132420%26meid%3D22f913f92fee4cd9bfc2bb73514e1a81%26pid%3D100005%26rk%3D2%26rkt%3D6%26sd%3D221769582503

I am trying to achieve **Constant Current Constant Voltage** charging to safely charge each cell to max capacity whilst charging the pack quickly as possible.

Is the BMS responsible for providing the trickle charge of 50-100mA to charge each cell to its full capacity once the cell voltage reaches 4.2V (i.e. by only drawing 50-100mA from the power supply) 
OR 
Should the power supply itself be responsible for the trickle current/Constant Voltage charging?


**BMS Specs say this:**
Technical Parameters:
Balanced current: 60mA (VCELL = 4.20V when)
Balanced for: 4.20 ± 0.05 V
```

---
## \#2 Posted by: lox897 Posted at: 2016-06-26T23:52:46.080Z Reads: 114

```
That top power supply outputs 48v. That is too much for 10S. @whitepony may be able to answer your other questions.
```

---
## \#3 Posted by: brabbit Posted at: 2016-06-26T23:53:41.026Z Reads: 114

```
Yep but it can adjusted within the voltage ranges of 41-56V it says on the spec sheet so I thought it would be ok.
```

---
## \#5 Posted by: whitepony Posted at: 2016-06-27T04:10:09.066Z Reads: 102

```
the power supply is doing the cc/cv switching, a bms just checks if each parallel pack is within 2.5-4.2V (or whatever the bms specs are). im charging since 1.5years with a "link 2" kind of charger, set to 41.4V cv saturation with 4A cc current!
```

---
## \#6 Posted by: brabbit Posted at: 2016-06-27T10:24:05.391Z Reads: 79

```
Ahhh right I see. So I should then go in for the 2A charger you think?
http://www.ebay.com/itm/Lithium-Ion-Battery-Charger-Li-ion-LiPo-10S-42V-2A-for-36V-37V-Wall-Socket-AC-DC/321555510511?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D20131003132420%26meid%3D22f913f92fee4cd9bfc2bb73514e1a81%26pid%3D100005%26rk%3D2%26rkt%3D6%26sd%3D221769582503
```

---
## \#7 Posted by: oyta Posted at: 2017-05-03T19:40:59.378Z Reads: 41

```
I am also building a battery pack 10s3p with HG2 batteries. What charger did you buy? And what BMS did you buy?
```

---

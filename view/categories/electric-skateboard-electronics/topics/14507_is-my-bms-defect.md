# Is my BMS defect?

### Replies: 8 Views: 1042

## \#1 Posted by: Fabian287 Posted at: 2016-12-11T15:21:21.238Z Reads: 111

```
Hello

today i build my secound e-skate board with bms (hcx-d345) and 10S3P li-ion the bms output was 36V so it sounds good but after i conected the vesc to it the voltage was 2,4V?(the vesc did not turn on)
I removed the Vesc and the voltage was again 36V :sweat:<img src="/uploads/db1493/original/3X/d/d/ddad5c5231728f0487491fa57dd012cc46638a78.jpg" width="666" height="499"><img src="/uploads/db1493/original/3X/f/2/f22d9b6998e73c3addac11479a5bd9ac4b78a62f.jpg" width="375" height="500">
sry for my english im german^^
```

---
## \#2 Posted by: Fabian287 Posted at: 2016-12-11T15:31:16.184Z Reads: 102

```
Now i soldered the vesc to my power bench and it worked but why drops the voltage to 2.4V?
```

---
## \#3 Posted by: Lukas Posted at: 2016-12-11T15:52:28.902Z Reads: 100

```
Be careful with these open solder joints, i don't know how your BMS performs, but you risk a short of your battery.

Second thing i noticed is that you don't have capacitors.
```

---
## \#4 Posted by: Fabian287 Posted at: 2016-12-11T18:09:28.297Z Reads: 84

```
the caps are coming but i dont think that they solve the prob
```

---
## \#5 Posted by: rpn314 Posted at: 2016-12-12T16:48:11.192Z Reads: 62

```
If anything (like the balance leads) isn't hooked up properly, it should cut off the output. Did you find a data sheet?
```

---
## \#6 Posted by: Fabian287 Posted at: 2016-12-12T17:23:25.686Z Reads: 56

```
yes
<img src="/uploads/db1493/original/3X/e/8/e8547025537a5c2d8e37024f797b576d23629105.jpg" width="375" height="500">
No, when i disconnect the vescs the voltage of the BMS is 36.11V but after i conect the vesc it drops to 2.4V
```

---
## \#7 Posted by: rpn314 Posted at: 2016-12-13T17:59:45.896Z Reads: 39

```
Hm...can you check the individual cell voltages? If the voltage drops as soon as any load is connected it kind of sounds like an unbalanced cell.
```

---
## \#8 Posted by: Fabian287 Posted at: 2016-12-18T20:09:46.976Z Reads: 33

```
no the cells are all 3.6 V with or without connected to the BMS
```

---

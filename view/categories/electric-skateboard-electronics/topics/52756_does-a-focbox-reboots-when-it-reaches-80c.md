# Does a Focbox reboots when it reaches 80C?

### Replies: 4 Views: 289

## \#1 Posted by: Eboosted Posted at: 2018-04-19T05:47:50.829Z Reads: 86

```
I has several reboots on my slave vesc today but only after pushing the board a lot, I might be getting a heatsink soon, almost 80C seems to be too much for the Focbox. 

![Screenshot_20180419-004625|690x335](upload://11LnewCM9wIFiapMzSJaWLO2ZTR.png)

After let it cool down a bit it was fine again.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-04-19T06:06:04.559Z Reads: 82

```
Yes it doesn't reboot but more like a cut off voltage it just will refuse to function, in bldc tool there is a mosfet start and end just like voltage cut off stock settings are "Mosfet start 80c" "mosfet end 100c"
Same thing with motor it's 80c and end 100c ( you can change them but do at own risk)
```

---
## \#3 Posted by: lrdesigns Posted at: 2018-04-19T07:21:52.057Z Reads: 74

```
It should not re-boot but it should make you go SLOW until the temp goes back down. Over 100c I think it cuts all power.
```

---
## \#4 Posted by: E1Allen Posted at: 2018-04-19T07:31:56.953Z Reads: 67

```
How many amps are you pulling to reach that continuous
```

---

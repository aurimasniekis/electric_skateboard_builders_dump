# Board Appears to be Over Charging with BesTech BMS

### Replies: 9 Views: 437

## \#1 Posted by: kuphjr Posted at: 2018-05-31T17:19:27.855Z Reads: 116

```
I recently installed a 15A D140 BMS on both my boards, but I just noticed that my charger seems to be overcharging my batteries by .1 to .2 volts when I look an my battery meter I have installed on my board.

I have heard that the charger is responsible for stopping charging as soon as the battery is at the correct voltage, so is this an issue with my charger?  It is just a cheap 2A charger I bought off eBay.

I have a 12s setup with 4x3s 8000mah Zippy Flightmax batteries.

Any tips would be great!
```

---
## \#2 Posted by: telnoi Posted at: 2018-05-31T18:22:57.372Z Reads: 103

```
Measure with a multimeter instead. Volt meters may not be that accurate.
```

---
## \#3 Posted by: kuphjr Posted at: 2018-05-31T18:31:12.417Z Reads: 102

```
I'll do that as soon as I get home. Thanks
```

---
## \#4 Posted by: kuphjr Posted at: 2018-05-31T18:47:21.021Z Reads: 89

```
@telnoi I just checked with a multimeter and It is reading 50.5 volts at the moment.  I plugged it back into the charger and the charger still has not turned itself off. I also measured the voltage on the charger and it is 50.7 volts.  How dangerous is this realistically?
```

---
## \#5 Posted by: kuphjr Posted at: 2018-06-01T16:48:00.639Z Reads: 71

```
Just as an update if anyone else ever has this issue, I read a little more about this and it turns out charging each cell less than .05v above 4.2 really isn’t that big a deal. It might slightly lower the life of the battery but not significantly enough to matter. Also BesTech D140 BMSs should protect the battery from overcharging more than .05 volts. In the future I think I’m going to buy a little bit better quality charger though.
```

---
## \#6 Posted by: Jebe Posted at: 2018-06-07T19:47:46.450Z Reads: 57

```
is this a lipo li ion or lifepo4 bms? different chemistry batteries run different voltages.
```

---
## \#7 Posted by: kuphjr Posted at: 2018-06-07T20:07:19.768Z Reads: 54

```
lipo
10chars
```

---
## \#8 Posted by: deucesdown Posted at: 2018-06-08T04:53:32.651Z Reads: 41

```
If you're lucky your charger may have a pot to adjust the termination voltage. It's usually right next to the output if present.
```

---
## \#9 Posted by: kuphjr Posted at: 2018-06-08T05:28:42.635Z Reads: 37

```
I got a new 6A charger anyway to charge more quickly.  That one should be higher quality and hopefully a more accurate voltage.
```

---

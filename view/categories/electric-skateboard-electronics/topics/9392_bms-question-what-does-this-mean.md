# Bms question: what does this mean?

### Replies: 9 Views: 1217

## \#1 Posted by: kyo Posted at: 2016-09-11T14:42:53.287Z Reads: 110

```
My battery pack is 10s5p. When i connected a bat indicator direct to the bat(before bms) it showed 64% like this
<img src="/uploads/db1493/original/3X/4/1/41c1d774f8e3d82d5a56061d12b20ddfe597ca08.jpeg" width="375" height="500">

But when the indicator connected after bms it showed 0% and no light
<img src="/uploads/db1493/original/3X/c/2/c2be3ba83827e7148cd84006a81d9691673e6ff0.jpg" width="375" height="500">

I used multimeter after the bms, it showed 36v 
I think the bms is cuuting off, its only 36v. Doesnt make sense.

One more weird thing, that i connect bat ( after bms) to vesc, the led on vesc flashing blue repeatedly. It is like there is no amp is coming out, and the computer could not detect a usb device when i i pluged it in. 

Then i switched to laptoplike charger, the veac connected to computer with no issue.

@longhairedboy @lowGuido @MasterCho @Jinra @Michaelinvegas
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-11T14:47:25.287Z Reads: 109

```
Is the meter negative going to P- or B- on the bms? You should be going to B-, assuming you have an eswitch on the bms. If you're running a power switch after the bms, you should have the meter after the switch or it'll always be on.

How are you wiring the meter?
```

---
## \#3 Posted by: kyo Posted at: 2016-09-11T14:58:34.114Z Reads: 106

```
@Jinra thanks for quick reply. In the case that it showed 64% , yes the meter connected to the b- of the bms. In the case it showed 0% it connected to p- 

One more weird thing, that i connect bat ( after bms) to vesc, the led on vesc flashing blue repeatedly. It is like there is no amp is coming out.

This is the bms i am using 
http://m.ebay.com/itm/221769582503?_mwBanner=1
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-11T15:03:33.369Z Reads: 88

```
Yea sounds like you don't have enough current going through. Did you wire battery negative to B- and VESC negative to P-? Battery positive doesn't go to BMS at all right?
```

---
## \#5 Posted by: kyo Posted at: 2016-09-11T15:15:52.492Z Reads: 85

```
Yes, i solder it right, negative bat to B- and negative power out to P- 

And the computer could not detect usb device when i i pluged it in.

Then i switched to laptoplike charger, the vesc connected to computer with no issue.
```

---
## \#6 Posted by: lowGuido Posted at: 2016-09-11T15:30:51.390Z Reads: 78

```
the BMS has probably cut out because of low voltage. charge your batteries and try again.

36/10= 3.6
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-09-11T16:23:00.706Z Reads: 72

```
It is looking like one of your cell pack is not correctly link to the BMS (on the JST connector), causing a shutdown over a Undervoltage error..
```

---
## \#8 Posted by: kyo Posted at: 2016-09-12T03:01:34.920Z Reads: 61

```
Thanks @lowGuido

@JohnnyMeduse thats a possibility. I will check that this weekend. Thanks
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-12T03:31:44.883Z Reads: 54

```
just fyi, low voltage cut off is 2.9v per cell, I'm guessing it may be an incorrect balance lead as well.
```

---

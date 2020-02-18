# Battery percentage indicator wiring

### Replies: 2 Views: 712

## \#1 Posted by: Koto Posted at: 2016-12-18T08:50:57.155Z Reads: 100

```
Hi,
I am about to start my first build but i am a little worried about my Battery indicator and its wiring. I am probably going to use this: http://www.ebay.com.au/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
I am a little uncertain how to wire it. http://www.electric-skateboard.builders/t/wiring-schematic/14290 my schematic.
I know i have to put it after the battery and befor the charge port so I can check my charge, but do i need a buck convertor or something so it doesnt blow the display (and other stuff)?
thanks,
Oscar
_xxXX KOTO XXxx_
```

---
## \#2 Posted by: lox897 Posted at: 2016-12-18T08:54:31.047Z Reads: 98

```
Put it between your anti-spark loop key switch and your vesc. That way it isn't constantly, only when the switch is connected. You will not need a buck converter since it accepts up to 48v.
```

---

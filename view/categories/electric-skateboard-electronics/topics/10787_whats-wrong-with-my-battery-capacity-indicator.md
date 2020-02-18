# What&rsquo;s wrong with my battery capacity indicator?

### Replies: 9 Views: 963

## \#1 Posted by: tueboard Posted at: 2016-10-07T21:08:37.421Z Reads: 124

```
hi,

i use this battery capacity indicator
http://www.ebay.es/itm/2016-Battery-Capacity-Tester-Indicator-for-12V-24v-36v-48v-CAR-Lead-acid-lithium-/172143986261?hash=item281494c655&_uhb=1

i've a 12s setup 44.44v (2 batteries 6s 8000mah 35c 22.22v each one), they are almost full 99%
battery 1 - 4.19, 4.20, 4.20, 4.19, 4.20, 4.19
battery 2 - 4.19, 4.19, 4.19, 4.20, 4.20, 4.20

i use this power switch
http://www.ebay.es/itm/221547512340?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

this is a picture of my build, i only want to show the capacity indicator when i turn on the switch
<img src="/uploads/db1493/original/3X/6/f/6ff1069c09bfa5cb6848211379d2dbc83e656be6.png" width="690" height="271">

but the battery capacity indicator only indicates 84%, why? any idea?

thank you
```

---
## \#2 Posted by: lox897 Posted at: 2016-10-07T21:10:08.136Z Reads: 110

```
It might be on the wrong mode. There is a button on the back. Hold this down as you power the board on and you should be able to change the mode.
```

---
## \#3 Posted by: Jinra Posted at: 2016-10-07T21:22:01.321Z Reads: 108

```
Also, your power switch might melt given it handles such low current.
```

---
## \#4 Posted by: rpn314 Posted at: 2016-10-07T21:22:14.984Z Reads: 108

```
Yeah, wiring looks great. Definitely some configuration issues
```

---
## \#5 Posted by: tueboard Posted at: 2016-10-07T21:52:31.729Z Reads: 96

```
thank you for all your responses! :)

@lox897 yesss!!! it works! when i turn on with the button indicator pressed i can choose an option from 0c to 15c, then to save the setting turn off and turn on again.
```

---
## \#6 Posted by: lox897 Posted at: 2016-10-07T22:33:52.323Z Reads: 84

```
Awesome. Set it according to what 12s is.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-07T22:55:38.596Z Reads: 82

```
Personally, I think it's better to monitor voltage. 
It doesn't seem like percentage meters are accurate enough.
Also, you need a high voltage anti spark switch. 
The switch you have won't hold up.
```

---
## \#8 Posted by: tueboard Posted at: 2016-10-07T22:59:13.017Z Reads: 80

```
Any recommendation of volt meter?
```

---
## \#9 Posted by: Namasaki Posted at: 2016-10-07T23:00:07.920Z Reads: 79

```
I think the meter you have can switch to volts.
```

---

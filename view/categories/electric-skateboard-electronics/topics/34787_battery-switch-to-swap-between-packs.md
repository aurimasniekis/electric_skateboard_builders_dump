# Battery switch to swap between packs

### Replies: 16 Views: 853

## \#1 Posted by: UltimaA380 Posted at: 2017-10-04T21:13:34.605Z Reads: 108

```
Im planning to make an 18650 pack, I also still have my old 6s (1 cell dead, so 5s) and was wondering how would I go about making a switch that switches between the packs? I dont want connectors I would just like to wire up a switch, thanks.
```

---
## \#2 Posted by: Jammeslu Posted at: 2017-10-04T21:20:59.181Z Reads: 106

```
I was thinking the same like when you trim an EPA and have a hidden gear thing and can max out when you need it.

Like s switch from 6s cruisng and switch to 10s to high speed
```

---
## \#3 Posted by: krloz Posted at: 2017-10-04T21:35:24.823Z Reads: 97

```
never tried but i bet the esc would reset if you swiched power.
```

---
## \#4 Posted by: UltimaA380 Posted at: 2017-10-04T21:50:36.336Z Reads: 88

```
I have no problem with that, just want more range
```

---
## \#5 Posted by: Okami Posted at: 2017-10-04T23:37:01.317Z Reads: 79

```
3 position switch. U would select positive wire. Ground would stay the same (would need 2 ground wires to esc)
```

---
## \#6 Posted by: UltimaA380 Posted at: 2017-10-04T23:50:03.071Z Reads: 75

```
I'm a little bit confused, mind getting a little bit more into detail?
```

---
## \#7 Posted by: UltimaA380 Posted at: 2017-10-04T23:51:10.077Z Reads: 71

```
Actually I think I understand, but wouldnt the current passing through destroy the switch?
```

---
## \#8 Posted by: krloz Posted at: 2017-10-05T08:46:03.960Z Reads: 69

```
Well yes if your switch is not properly rated for the voltage and amps. I guess spark may not be a problem as the esc caps would already be charged but I'm not sure about that
Some people have had success using relays. If not, maybe arv/boat/rtf battery bank switch (btw they are huge)
```

---
## \#9 Posted by: Okami Posted at: 2017-10-05T09:37:00.166Z Reads: 61

```
<img src="/uploads/db1493/original/3X/1/8/18ae7d6138719123fa8d0316629459e7ba830a0c.jpg" width="690" height="387">

There should be one more "input wire"

Switch is rated for about 20A at 125volts, i solder each wire to 2 terminals (6terminals total), so i would like to believe it is good up to 40A or so

Raw description

Esc receices 2 ground wires.and 1 positive wire. With switch u would select either pack to "activate", u would chain either lipo or 18650

---

Something like this:
https://m.ebay.com/itm/DPDT-Double-Pole-Double-Throw-6-PIN-on-off-on-20A-Rocker-Switch-/171489655398?_mwBanner=1

U can also get waterproof cover for it.
```

---
## \#10 Posted by: UltimaA380 Posted at: 2017-10-05T19:54:26.419Z Reads: 43

```
Awesome, would this work? http://www.ebay.com/itm/1-Pcs-Waterproof-16A-125V-10A-250V-ON-OFF-ON-6pin-Boat-Rocker-Momentary-Switch-/172863361695?hash=item283f75929f:g:In8AAOSwaIRZuL3e
```

---
## \#11 Posted by: Pedrodemio Posted at: 2017-10-05T21:12:20.567Z Reads: 36

```
Current rating doesn't change with voltage, so it still 20A
```

---
## \#12 Posted by: Okami Posted at: 2017-10-05T21:16:16.847Z Reads: 33

```
Yeh i saw it says up to 36v also 20A. For 220v it might suggest 15A
```

---
## \#13 Posted by: Okami Posted at: 2017-10-05T21:17:51.096Z Reads: 33

```
No, u need non-momentary. 

Momentary wont stay turned on and will return to off position
```

---
## \#14 Posted by: UltimaA380 Posted at: 2017-10-05T22:41:17.225Z Reads: 26

```
Oh crap I didn't see it saying momentary. But will this switch with its ratings work if it was non momentary?
```

---
## \#15 Posted by: UltimaA380 Posted at: 2017-10-05T22:42:47.410Z Reads: 26

```
http://www.ebay.com/itm/1pc-12V-12A-Car-Boat-ON-OFF-ON-SPST-6-Pin-Rocker-Toggle-Switch-Waterproof-/162495533062?hash=item25d57d1006:g:2GYAAOSw42JZBAt~&vxp=mtr ?
```

---
## \#16 Posted by: Okami Posted at: 2017-10-06T09:04:21.100Z Reads: 22

```
This looks better yes. Though i would suggest to go to local electronics parts shop and find one there,  otherwise u can order from china but it will take a while.

So yes, u need toggle switch. And u will need to cut out plastic part between the contacts if you want to solder the wire 2 terminals at once (do it with hot knife or soldering iron specially for cutting, for example)
```

---

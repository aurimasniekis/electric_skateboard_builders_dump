# Vesc and motor and the others

### Replies: 4 Views: 359

## \#1 Posted by: cypa9904 Posted at: 2017-06-09T18:00:54.265Z Reads: 61

```
Hi 
Do somebody knows if faradaymotion VESC may be used for electric mountainboard 2WD?
50A cont., 240Amax, 
Voltage: 8V – 60V (Safe for 3S to 12S LiPo).
http://shop.faradaymotion.com/shop/18-electronics/4-vesc-motor-controller/

motors: 2x Turnigy 149kv (70A) or 2x Turnigy 192kv (80A)
accu: 12s

*Has somebody a photo of this VESC? I'd like to know how it looks :D*

*To connect 2x vescs to 1 reciever, Futaba Y Servo Lead would be ok?*

*Do I need to buy something to programm it?* 

*Sorry for (maybe) stupid questions. I just wan't to be sure if I'd have everything that I need, because shipping costs are terrible and I don't want to buy some parts after I start building my e-mountainboard :)*

Thanks for replies :)
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-06-09T18:10:23.821Z Reads: 55

```
[quote="cypa9904, post:1, topic:24984"]
Do somebody knows if faradaymotion VESC may be used for electric mountainboard 2WD?
[/quote]

Yes

[quote="cypa9904, post:1, topic:24984"]
Has somebody a photo of this VESC? I'd like to know how it looks
[/quote]

https://www.google.com/search?q=vesc&source=lnms&tbm=isch&sa=X&ved=0ahUKEwje0pu-rbHUAhWJvbwKHRWHCfEQ_AUIDCgD&biw=1578&bih=881

[quote="cypa9904, post:1, topic:24984"]
To connect 2x vescs to 1 reciever, Futaba Y Servo Lead would be ok?
[/quote]

yup, this is how i'm connecting two vescs instead of the CAN bus.

[quote="cypa9904, post:1, topic:24984"]
Do I need to buy something to programm it?
[/quote]

http://vedder.se/2015/01/vesc-open-source-esc/ and a usb cable.
```

---
## \#3 Posted by: sl33py Posted at: 2017-06-09T19:10:01.609Z Reads: 36

```
I would stick to 10s if you want to use the 192kv motor - very close to a 60k ERPM limit which is known to fry the DRV chip on the VESC 4.xx.  

you can go 12s on the 149kv, or the 168kv as alternatives with room to avoid exceeding 60k ERPM.
```

---
## \#4 Posted by: cypa9904 Posted at: 2017-06-09T19:23:04.462Z Reads: 35

```
Okay, thanks :slight_smile:
```

---

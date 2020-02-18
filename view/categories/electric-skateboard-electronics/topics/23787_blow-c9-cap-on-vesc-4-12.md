# Blow C9 Cap on VESC 4.12

### Replies: 9 Views: 844

## \#1 Posted by: Eboosted Posted at: 2017-05-24T03:33:14.336Z Reads: 78

```
Hello guys, I disassembled my board today, cleaned the electronics, made motor detection and when I went to ride it one one motor spinned even though it worked perfect on the bench.

I disassemble everything back again and one VESC did not turn on.

<img src="/uploads/db1493/original/3X/f/5/f5c2ed03c7cf6d8d3abd8ac24025347385f6b8b2.png" width="375" height="500">
<img src="/uploads/db1493/original/3X/0/3/03b683efd2d1975e26f3eab3fae08d3435e874ca.png" width="690" height="388">

C9 seems to be fried.

On a brightside I had a new VESC here laying around and installed it on the board, everything went smoothly but when I did motor detection, I heard a click, VESC disconnected and the led is not turning on at all, damn!

Would it be possible that I'm getting a short on the motor?, the phase wires are perfectly isolated.

How can I know if the motor is not shorted?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-24T03:35:17.488Z Reads: 72

```
If you can spin your motor by hand with no heavy resistance, the phase wires shouldn't be shorting. I'd run it on the bench more, maybe grab the wheel to simulate some load.
```

---
## \#3 Posted by: Eboosted Posted at: 2017-05-24T03:44:06.802Z Reads: 67

```
As soon as I clicked on "detect" the brand new VESC blew! 

It didn't even tried to spin at all
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-24T03:46:02.167Z Reads: 64

```
Are you sure your not just having a bad nightmare right now. Try pinching yourself.
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-24T03:46:42.898Z Reads: 62

```
Sounds like a cursed motor. Did you find any resistance when spinning by hand?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-24T03:47:28.507Z Reads: 62

```
Sounds like a short inside the motor
open the motor and have a good look inside
```

---
## \#7 Posted by: Eboosted Posted at: 2017-05-24T04:01:14.736Z Reads: 61

```
Damn! I wish this is only a nightmare, pinching myself only left me a bruise. 

I'm able to freely spin the motors by hand, no resistance whatsoever, I even was able to update the VESC firmware and set the motor maximum values as always, but as soon as I pressed detect, a  clak sounded inside the VESC followed by a disconnection from BLDC tool and no led at all. 

What would be the best way to repair both VESCs, how do I know what are the specs of the C9 in order yo buy it locally?

There are no signs of blown C9 on the new VESC
```

---
## \#8 Posted by: Eboosted Posted at: 2017-05-24T05:03:20.750Z Reads: 59

```
According to the VESC 4.12 BOM, the C9 seems to be a 10uF 50v capacitor. 

Hope some electronic expert  could give me a hand here in order to confirm this? 

[img] http://i.imgur.com/DsnywYs.png[/img]
```

---
## \#9 Posted by: Sander Posted at: 2017-05-24T06:12:04.004Z Reads: 48

```
There should be a BOM list where all the parts are listed and the manufacture number for them too.
C9 =10uF 50V	
MOUSER	963-UMK316BBJ106ML-T	

https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC4.12_BOM.ods
```

---

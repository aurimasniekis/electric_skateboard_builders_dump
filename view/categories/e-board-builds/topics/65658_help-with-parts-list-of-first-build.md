# Help with parts list of first build

### Replies: 5 Views: 397

## \#1 Posted by: FakeIphone Posted at: 2018-08-22T00:52:33.384Z Reads: 78

```
Hi guys I would love to hear some advice on my first budget built 

**motor (already bought) - racerstar 6368 280kv** https://www.banggood.com/Racerstar-6368-BRD6368-280KV-6-12S-Brushless-Motor-For-Balancing-Scooter-p-1117657.html?utm_source=Youtube&utm_medium=cussku&utm_campaign=10638587_1117657&utm_content=1087&cur_warehouse=CN

**VSEC** - collections/electric-skateboard-parts/products/torque-esc-bldc-electronic-speed-controller

**remote** - collections/electric-skateboard-parts/products/torqueboards-2-4ghz-nano-remote-controller

**battery 4x 5s1p to make 10s2p** - https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-40c.html

**7" china trucks** - https://www.aliexpress.com/item/-/32838198601.html?spm=a2g0s.13010208.99999999.266.53e13c00aUOQMn

**motor mount, wheel pulley and motor pulley (i will drill 8mm to 10mm) it is kit 2-** https://www.aliexpress.com/item/83mm-90mm-97mm-Electrical-Skateboard-1800W-Motor-5M-Gear-270mm-Belts-Kit-And-Motor-Mount-Parts/32831988158.html?spm=a2g0s.13010208.99999999.273.53e13c00aUOQMn

**97mm wheels  (already bought) ** - https://www.aliexpress.com/item/Big-80mm-87mm-83mm-90mm-97mm-Longboard-wheel-SHR78A-Red-Color-PU-Wheels-High-Level-Soft/32829853751.html?spm=a2g0s.9042311.0.0.3f034c4dHXgk0t

Im trying to have it as low-cost as possible but i dont wanna kill myself with some shitty stuff. :slight_smile: Is 11mm belt enough ?  Thanks
```

---
## \#2 Posted by: yelnats8j Posted at: 2018-08-22T02:37:43.858Z Reads: 61

```
How will you be charging your board?

I would get different trucks.

[quote="FakeIphone, post:1, topic:65658"]
**7" china trucks** - [https://www.aliexpress.com/item/-/32838198601.html?spm=a2g0s.13010208.99999999.266.53e13c00aUOQMn ](https://www.aliexpress.com/item/-/32838198601.html?spm=a2g0s.13010208.99999999.266.53e13c00aUOQMn)
[/quote]
The Motor mount is reallt not good

[quote="FakeIphone, post:1, topic:65658"]
**motor mount, wheel pulley and motor pulley (i will drill 8mm to 10mm) it is kit 2-** https://www.aliexpress.com/item/83mm-90mm-97mm-Electrical-Skateboard-1800W-Motor-5M-Gear-270mm-Belts-Kit-And-Motor-Mount-Parts/32831988158.html?spm=a2g0s.13010208.99999999.273.53e13c00aUOQMn
[/quote]
```

---
## \#3 Posted by: Jacobee Posted at: 2018-08-22T04:04:08.981Z Reads: 50

```
With a 280 kv motor on a 10s battery you risk going over the erpm limit of the vesc. I guess you could limit the erpm but you won't have as much torque from that motor as a similar sized 190-200 kv motor and since your speed would be limited by your erpm wouldn't be going any faster with a 280 kv motor.
```

---
## \#4 Posted by: FakeIphone Posted at: 2018-08-22T10:10:50.078Z Reads: 38

```
Alrighty then, im switching to diy battery pack with 18650 and BMS i love that i would be able to charge that think with laptop charging brick, but im not sure what to do with motor, should i ditch him and buy new one with lower kv ? Are there any benefits from lower kv motor vs limiting erpm on this motor to 60k in vsec settings ? Thanks a lot for your patients with my guys. :)
```

---
## \#5 Posted by: rey8801 Posted at: 2018-08-22T10:14:26.861Z Reads: 39

```
if you limit the erpm in the vesc setting for a motor that has Kv close to the limit doesn't change that much, becuase anyway you are not going to reach that speed when loaded. On the other hand if you limit the erpm for a motor that is way above the limit, then you cut the power of the motor when it is more efficient. Usually we all try to stay within the Kv becsause you will have a good torque/speed balance. Read this topic to better understand https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
In your case 97mm wheels are already towards speed and less torque so better you go with a <200Kv motor. Moreover 10s2p battey in a bit underrated for a belt drive. I would choose something different.
```

---

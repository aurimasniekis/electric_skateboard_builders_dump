# HELP! Hobby King Build Single Motor

### Replies: 9 Views: 515

## \#1 Posted by: GameOver Posted at: 2018-06-16T23:49:41.955Z Reads: 126

```
Deck - [is something like this](http://www.whateverskateboards.com/cart/longboards/beebop_v2--329?ref=featuredlongboards)

Trucks - Caliber II 50

Motor - [Sk8 6374 190kv](https://hobbyking.com/en_us/turnigy-sk8-6374-192kv-sensored-brushless-motor-14p.html)

Speed Controller - [Sk8 ESC](https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html)

Mount - [Turnigy Skateboard Conversion Kit Mount](https://hobbyking.com/en_us/motor-mount-5.html)

Pulley - [Turnigy Skateboard Conversion Kit Pulley Set](https://hobbyking.com/en_us/gear-set-with-belt.html) 15/36T

Battery - [2 x 5s 5000 mah in Series](https://hobbyking.com/en_us/turnigy-battery-5000mah-5s-20c-lipo-pack-xt-90.html)

Wheels - 90mm ABEC Clones

Remote: [HK G2TB](https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html)

ESC Settings: Ackmaniac Firmware

FOC
Motor Max: 60A
Motor Min: -60A
Batt Max: 30A
Batt Min: -15A

Rider: 205lbs

It runs and it's ride-able. It feels though it doesn't have much power. Acceleration leaves you wanting for more. And it seems to have difficulty going up even the slightest incline. Is this normal for a single drive setup? The roads are wet though and the wheel might be slipping so I'm thinking this could be the case.

Just for comparison's sake, my first build is a DIY Ebay 90mm dual hub + ebay esc combo with LiPo batteries and I've had no problems with it on wet roads and going uphill. Although, yeah, it's dual motors. I was expecting though that a single 6374 belt drive would smoke the dual hub away.

Am I doing something wrong? Or is this normal for a single drive, wet road and rider weight?
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-16T23:59:25.752Z Reads: 111

```
you can increase batt max to about 60amp motor to 70amp. batt min also can be -20 
try that.
Since you are using hobbyking vesc I do not know the max amp draw for the set up, it is conservative suggestion.

And you are a heavy class rider. Dual would be more appropriate.

also try BLDC, instead. I think it has slightly have more kick. Also FOC heats up the vesc more so for single it is a bit risky.
```

---
## \#3 Posted by: GameOver Posted at: 2018-06-17T01:28:12.743Z Reads: 89

```
I will try BLDC and increase max amp. Hopefully it makes an improvement.
```

---
## \#4 Posted by: GameOver Posted at: 2018-06-17T02:05:15.088Z Reads: 80

```
Tried BLDC, during motor detection, magic smoke... is this dead?
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-06-17T02:13:59.744Z Reads: 80

```
how? what kind of motor detection you did to kill with smoke?... we have @JohnnyMeduse here, he can fix most of vesc. show him picture of drv and detection setting.
```

---
## \#6 Posted by: GameOver Posted at: 2018-06-17T02:20:01.625Z Reads: 75

```
![Magic%20Smoke|690x442](upload://4W6nTKhSt2FSyYLO4GIyyi4tEvS.PNG)

It said "Detection Failed". It made a sound then sparky sparky smoky smokey
```

---
## \#7 Posted by: onepunchboard Posted at: 2018-06-17T02:24:32.505Z Reads: 72

```
it is possible your motor have been shorted. in any case you should've use the detection wizard. please talk to johhny, if your vesc is burned in anyways. I'm sorry to hear this.
```

---
## \#8 Posted by: GameOver Posted at: 2018-06-17T02:32:05.850Z Reads: 72

```
Yeah I used the wizard. I was at that point oin the wizard when it happened. I think it is the chip that got burned. Blue and other light still blinking but no more red light.

It's not cost effective to send this for repair from where I am in the world... damn...
```

---
## \#9 Posted by: pat.speed Posted at: 2018-06-17T05:48:59.175Z Reads: 58

```
I’d say the motor shorted or phase leads did. Anyway I would ask HobbyKing about a refund, as they told me it has a 1 year warranty
```

---

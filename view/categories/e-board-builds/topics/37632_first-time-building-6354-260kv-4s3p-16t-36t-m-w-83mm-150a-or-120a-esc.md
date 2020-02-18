# First Time Building &#124; 6354-260Kv &#124; 4S3P &#124; 16T:36T (M:W) &#124; 83mm &#124; 150A or 120A ESC

### Replies: 9 Views: 926

## \#1 Posted by: jjalibwa Posted at: 2017-11-07T15:55:02.131Z Reads: 70

```
Hello everyone,

I am new to this website and I started building my board way before I was introduce to this site. Currently, my board is half way done., however, I don't mind switching parts if the change is justified. My goal was to make an e-board that could go around 15 mph max weighted with 5 miles of range minimum. This is my following setup.

Motor: [Turnigy Aerodrive SK3 - 6354-260KV Brushless Outrunner Motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html)

Batteries: 3 x [Multistar High Capacity 5200mAh 4S 10C Multi-Rotor Lipo Pack](https://hobbyking.com/en_us/multistar-high-capacity-4s-5200mah-multi-rotor-lipo-pack.html) ( They will be in parallel, giving a max continuous current output of 156A but that's probably less than that, plus 230W-h was the best I could do for my budget) 

ESC: I am considering the [HobbyKing® ™ X-Car Beast Series ESC 150A](https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html) or [HobbyKing® ™ X-Car Beast Series ESC 120A](https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html). I do plan on upgrading to a VESC when this setup works. 

Wheels: 83mm 78a wheel, nothing fancy.

Gears: HTD-5 12mm 16T:36T (MOTOR:WHEEL) I do wonder how tight the pulley should be. 

Motor mount: Some cheap Chiness thing off [ebay](https://www.ebay.com/itm/DIY-Electric-Skateboard-Kit-Parts-Pulleys-Belt-and-Motor-Mount-For-80MM-Wheels/253240269060?epid=897131934&hash=item3af64bd904:g:Z9QAAOSw8zdZ~DeP), holds up well so far.

TX/RX: [Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System](https://hobbyking.com/en_us/quanum-2-4ghz-3ch-pistol-grip-tx-rx-system.html)


What do you think? Will that setup work? Do you have ways you might want to improve it?
```

---
## \#2 Posted by: aponty Posted at: 2017-11-07T17:17:58.120Z Reads: 52

```
I think the standard is 6s or higher for voltage for a reason, anything lower than that is going to be pretty inefficient. Maybe get another battery and put two in series to make it 8s?
```

---
## \#3 Posted by: cwazy1 Posted at: 2017-11-07T17:32:58.731Z Reads: 43

```
1. minimum 6s for your battery if you want 15mph. 
2. just get a vesc to start with. I understand that you're "ok" with changing parts later, but honestly, why would you if you don't have to.
3. get a mini remote. same price, and smaller.
```

---
## \#4 Posted by: jjalibwa Posted at: 2017-11-07T17:46:39.699Z Reads: 36

```
what is a mini remote?
```

---
## \#5 Posted by: cwazy1 Posted at: 2017-11-07T17:49:22.565Z Reads: 33

```
https://psychotiller.com/product/24ghz-remote-controller
```

---
## \#6 Posted by: jjalibwa Posted at: 2017-11-07T18:03:23.805Z Reads: 32

```
What VESC would you recommend? 
So far I am upgrading to a 62 12Ah battery with XT90 connectors
```

---
## \#8 Posted by: Sk8Board Posted at: 2017-11-07T18:06:11.115Z Reads: 32

```
If you have  a 3d printer get the http://www.electric-skateboard.builders/t/gt2b-mad-munkey-v1-enclosure-now-ready-for-download/2814
 I agree with @aponty that you should get 1 more battery to make it 8s. I will give you a bit faster speed and you still have 10400mah which is plenty to get you 5 miles. You could go even farther with that
  

(Didn't want to reply to someone that's why I edited)
```

---
## \#9 Posted by: cwazy1 Posted at: 2017-11-07T18:21:22.164Z Reads: 29

```
I really don't recommend a beginner to build a gt2b mod controller. Just get a simple turn key remote and then down the line if OP has resources/time/the desire, then start getting better components. 

@jjalibwa If you want cheap and don't plan on running FOC, then go with any VESC 4.x  

collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller

If you want to run FOC or just have a more reliable VESC, get a FOCBOX.
```

---
## \#10 Posted by: aponty Posted at: 2017-11-07T19:41:43.451Z Reads: 26

```
Also there's this option if you're looking for a cheap decent ESC. You'd have to up it to 6s (these go 6/8/10s, you have to specify when you order), but they're decent quality (meepo and many other boards use them) and it comes with the remote. Plus it's cheap.

https://www.ebay.com/itm/single-motor-electric-longboard-skateboard-controller-ESC-Substitute/302516117782?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D49007%26meid%3D97d412ca89154f5ebc5cd0321aadd1ca%26pid%3D100011%26rk%3D2%26rkt%3D12%26sd%3D322451239466&_trksid=p2047675.c100011.m1850
```

---

# Cafesk8 &#124; Arbor Axis &#124; Caliber &#124; TB 6374 230KV &#124; DIYelectric single &#124; 12S &#124; TB 12S 120A ESC

### Replies: 16 Views: 1205

## \#1 Posted by: ch3m1st Posted at: 2016-11-11T02:26:15.693Z Reads: 172

```
This is my first build and it is a work in progress. Currently, I do not have it running due to some ESC - rx issues. 
The name is derived from my love for caffeinated beverages and profession. 
 <img src="/uploads/db1493/original/3X/d/7/d7431ec913418288c58750c4b4151ff4d961f184.jpg" width="281" height="500">

The programming card...
<img src="/uploads/db1493/original/3X/3/4/3493cfbf82619ed3d1ecc3744695cb29a7c1279c.jpg" width="375" height="500">
Motor, mount, and trucks
<img src="/uploads/db1493/original/3X/0/e/0e56df77941ce13ff9513a46631a5b698bbc982a.jpg" width="375" height="500">
Unfinished system
<img src="/uploads/db1493/original/3X/e/0/e0790b73c72b312bfb62ad52647762a0eb9efa67.jpg" width="666" height="500">
Battery box and ESC
<img src="/uploads/db1493/original/3X/a/d/ad060335a9e84a6b8276e5d244fd2e3063760818.jpg" width="375" height="500">
rx tx
<img src="/uploads/db1493/original/3X/0/7/072cd5861a292526fc73954dfcad2b24932bbcf0.jpg" width="690" height="388">

Parts List:
Single Bolt On Motor Mount w/ Drive Wheel Kit 
Caliber Trucks
Otang Kegel 80a 80m 56m contact
Reds Swiss Bearings
16T/36T 9mm Kegel Drive Wheel Kit
TB  Motor 6374 230KV 3200W 
TB 12S 120A Car ESC OPTO HV 
Arbor Axis 
Turnigy 3S 5Ah x 4 batteries
3D printed parts are designed by @FLATLINEcustoms designer of the Mad Munkey
TorqueBoards 2.4ghz Nano Remote Controller

**Any and all input is welcomed, I love learning and look forward to riding this beast!**
```

---
## \#2 Posted by: JLabs Posted at: 2016-11-11T02:32:38.984Z Reads: 146

```
Looks good, is the esc issue because you don't have a UBEC?
```

---
## \#3 Posted by: ch3m1st Posted at: 2016-11-11T02:35:26.082Z Reads: 144

```
That is what I am trying to figure out...I haven't had a lot of time to dig into the issue, yet. @FLATLINEcustoms had the same input. I'm not sure what I need with this ESC
```

---
## \#4 Posted by: NNGG Posted at: 2016-11-11T02:43:59.762Z Reads: 134

```
Did you program the ESC? Did you bind the controller? Does you receiver have 5v? does the receiver get input signals
```

---
## \#5 Posted by: ch3m1st Posted at: 2016-11-11T02:48:13.883Z Reads: 129

```
First I bound the tx and rx connected to the single lead from my esc. All was fine. 
Second, I tested the throttle control. It was wonky and the motor went to full power and wouldn't stop unless I held the throttle stick all the way down. I had to power the board off. 
Then, I unplugged the rx and plugged the programmer in and the screen booted up like the youtube tutorial. I proceeded to follow those directions from YT and after the first input, the screen went blank. 
Now, I have an ESC that will only output 0.5V to that accessory cable.

Did I blow something in the ESC?
```

---
## \#6 Posted by: Jinra Posted at: 2016-11-11T02:50:37.034Z Reads: 115

```
The full throttle issue was because you need to reset throttle neutral by rebinding the remote. You need to do this anytime you change the throttle trim. I'd recommend getting 12mm belts for a single drive or you may find yourself breaking belts quite often depending on your weight and riding environment.

Also going that fast on a single drive is a recipe for disaster unless you know how to stop.
```

---
## \#7 Posted by: ch3m1st Posted at: 2016-11-11T02:55:47.861Z Reads: 115

```
First off, thank you @JLabs @NNGG @Jinra for your hyper-fast responses! I truly appreciate all of your input! 

@jinra Dually noted, but now I can not get my rx to power on?! All this happened after the first binding event.  
You are definitely right. I am about 200lbs and will be riding around Georgia Tech, which is super hilly!   
Do you have any recommendations? on belts? New drive systems?

Oh, and I have been riding a Boosted Dual+ for a year now and have improved my braking skills. Mostly to avoid getting run over by the Tech Trollies!!!!
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-11T02:57:29.914Z Reads: 114

```
Luckily you'll just need to upgrade your wheel and motor pulley and get a wider 12+mm belt. Or if you're looking for a better (but pricier) upgrade, you can get a second motor and 9mm drive kit and run dual diagonal. All the torque you'll ever need!
```

---
## \#9 Posted by: JLabs Posted at: 2016-11-11T02:57:46.964Z Reads: 107

```
That esc requires a UBEC to step down the voltage for the receiver. Not sure how you got the programmer tonight up with no ubec
```

---
## \#10 Posted by: JLabs Posted at: 2016-11-11T03:00:40.366Z Reads: 106

```
I sell the same esc, and have the Ubec for sale if u need it. 
https://electric-skateboard.market/product/ubec-12s-120a-hv-opto/
```

---
## \#11 Posted by: ch3m1st Posted at: 2016-11-11T03:00:53.172Z Reads: 104

```
I'm not opposed to upgrades but really need to get this thing running, asap. I have extra belts, and I even have 12mm belts sitting here, do you have a wheel-pulley recommendation?
```

---
## \#12 Posted by: ch3m1st Posted at: 2016-11-11T03:01:24.619Z Reads: 102

```
Me neither! Powered by ignorance!
```

---
## \#13 Posted by: Jinra Posted at: 2016-11-11T03:03:20.156Z Reads: 100

```
I think DIYES has those options. I use his mount and motor pulley, but I use the 12mm Enertion drive wheel pulley myself. I don't 100% recommend it unless you're comfortable cutting off a bit of your trucks. Though I fully recommend it if you are!
```

---
## \#14 Posted by: ch3m1st Posted at: 2016-11-11T03:03:24.698Z Reads: 103

```
That's awesome @JLabs thank you for the rec I will check it out!
```

---
## \#15 Posted by: FLATLINEcustoms Posted at: 2016-11-11T13:13:45.142Z Reads: 79

```
@ch3m1st glad to see you finally got on here.
```

---
## \#16 Posted by: ch3m1st Posted at: 2016-11-11T14:05:14.416Z Reads: 77

```
@FLATLINEcustoms me too! I need so much help to finish this thing! Everyone is super helpful!
```

---

# PSA; ackmaniac Bluetooth compatibility with the pixel 2 xl is extremely spotty

### Replies: 12 Views: 324

## \#1 Posted by: osbor Posted at: 2018-08-05T23:05:28.215Z Reads: 83

```
It actually connected fine with my old pixel 2 xl, but that one got stolen and I had to replace it a few weeks ago.

With my new one, the app -REFUSES- to communicate with my board. It's seen in the list and tries to connect, but nothing happens and it eventually disconnects without any errors.

I'm using dual focboxes, as well as This particular adapter from bkb https://buildkitboards.com/collections/parts/products/vesc-bluetooth-adapter
Which uses the hm10 module
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-08-06T02:11:42.019Z Reads: 66

```
Maybe its just this particular Pixel? If it worked on the old one it might be the quality of assembly, ive heard a lot of mixed feelings about the build quality and craftsmanship of the new gen Google phones
```

---
## \#3 Posted by: mmaner Posted at: 2018-08-06T02:18:16.297Z Reads: 66

```
I've got a pixel and a pixel 2, both if my BKB BT modules connect to both phones with no issues. I think its likely your phone.
```

---
## \#4 Posted by: nlamel Posted at: 2018-08-06T04:54:31.594Z Reads: 53

```
Android 8.0 included some bluetooth security upgrades that broke compatibility with certain HM-05 and HM-10 modules that don't pass whatever security checks are in. It's likely your new phone had the newer version of Android and that's what's causing your issue. There's plenty of threads here about which modules from which suppliers don't have this security issue, and swapping your HM-10 will likely solve your issue.
```

---
## \#5 Posted by: Maxid Posted at: 2018-08-06T05:35:00.498Z Reads: 44

```
@moderators can you close this? Feels to me like @Ackmaniac's app is shamed for no reason. This is probably a clone module with wrong firmware.
```

---
## \#6 Posted by: osbor Posted at: 2018-08-06T05:57:02.071Z Reads: 42

```
Module from build kit boards, actually, he's a good guy.
```

---
## \#7 Posted by: Maxid Posted at: 2018-08-06T06:38:38.498Z Reads: 41

```
so? doesn't mean the module couldn't be a clone. The genuine ones are actually quite hard to source.
I don't blame him or you - just do the update procedure i posted in the app's thread. If the problem persists we can continue trying to find a solution.
```

---
## \#8 Posted by: Acido Posted at: 2018-08-06T06:57:14.802Z Reads: 39

```
Try turning on your location, it doesnt work without it for me, im running lineage os that is probably the closest rom to the stock google one
```

---
## \#9 Posted by: osbor Posted at: 2018-08-08T20:56:26.937Z Reads: 30

```
Here's a direct link to the update procedure, by the way
https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/694?u=osbor
```

---
## \#10 Posted by: osbor Posted at: 2018-08-14T05:19:37.513Z Reads: 23

```
Ugh, nevermind.
Flashed the new firmware, thought it worked. Put it on my board aaaaand...

Same behavior.
```

---
## \#11 Posted by: osbor Posted at: 2018-08-28T02:49:34.365Z Reads: 14

```
alright i'm kicking this back to being the app or android's fault
i've gone through three different HM10s which all behave exactly the same, constant connect and disconnect cycle every few seconds with no data transmitted

one from BKB: https://buildkitboards.com/collections/parts/products/vesc-bluetooth-adapter
which i actually flashed to the latest firmware using the instructions posted a few posts up, didn't work

one from amazon: https://www.amazon.com/gp/product/B0140R8DGQ/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1
didn't work

and finally one from Psychotiller: https://psychotiller.com/product/mccloeds-blue-tooth-modules
which i know for a fact is the real deal hm10

so what the heck is going on?
```

---
## \#12 Posted by: Klaerke91 Posted at: 2018-08-28T07:03:07.276Z Reads: 12

```
Your phone is broken as the app work for everybody else or you have some broken hm10 modules's or your VESC is broken.
```

---

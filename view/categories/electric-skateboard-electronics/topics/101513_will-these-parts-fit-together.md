# Will these parts fit together?

### Replies: 8 Views: 194

## \#1 Posted by: gamlek Posted at: 2019-09-08T16:43:40.946Z Reads: 77

```
hey i have bought 60 x samsung 30q cells and im going to make a 10s6p.


i would like to have a BesTech D140 Charge Only BMS but i dont really see a place to buy in EU. if you have a place to buy in eu please send link me.

And i would like to get a Dual FSESC4.20 100A. (https://flipsky.net/products/dual-fsesc4-12-100a) again if you know a place in EU :slight_smile:

this is probaly unnecessary information but my motors are c6374 170kv 2900W max.

So. will the vesc be ok for the batteries and will the bms also be ok with the batteries ? or do i need to change somthing ?
```

---
## \#3 Posted by: gamlek Posted at: 2019-09-08T17:10:44.940Z Reads: 67

```
hmmm. smart :smile: i will consider it. but do you have a suggestion on with 2 to get ?
```

---
## \#4 Posted by: Ben.Nexus Posted at: 2019-09-08T19:53:13.251Z Reads: 59

```
Well 2 focboxes, but they are collector's items by this point, super hard to find.
2 Trampa VESC6 but that might be overkill

Otherwise, I'd just stick with a dual one, they're at least quite good value. Remember to grab a bms with a switch on it, or a loop key. Don't get the flipsky antispark, from what i've seen its kind of garbage right now.
```

---
## \#5 Posted by: whaddys Posted at: 2019-09-09T04:26:45.240Z Reads: 42

```
Also you can run each ESC to its own receiver so if one ESC fails you don't have total cut-out and failure the other one is still up and going.  Pair one remote to 2 receivers - dual independent as @b264 calls it.  I discovered this and there's no going back
```

---
## \#7 Posted by: whaddys Posted at: 2019-09-09T04:29:08.308Z Reads: 38

```
I feel waaaay safer doing it especially after hearing about so many cut-outs.  Plus I push my ESCs pretty hard.
```

---
## \#8 Posted by: gamlek Posted at: 2019-09-09T10:06:19.534Z Reads: 28

```
I have looked around on some webshops and there is really not many "cheap" parts... by that i mean based in EU, because if i order stuff from outside eu, my wallet is gonna be empty for the next 3 months :blush:.

so i found [this](https://www.robotshop.com/eu/en/maytech-vesc-50a-brushless-speed-controller-eskateboard-robotics.html#description) its gonna be like  189 EUR for 2 of them. but idk if they are safe or good ? what is your opinion guys ? 

i really appreciate your guys help and opinions.

Edit: maybe [this](https://www.robotshop.com/eu/en/maytech-mini-wireless-remote-e-skateboard.html) controller ?
```

---
## \#9 Posted by: gamlek Posted at: 2019-09-10T08:45:12.763Z Reads: 17

```
what tool will i have to use with the 2 vesc ? just the normal vesc tool free https://vesc-project.com/vesc_tool ???
```

---
## \#10 Posted by: Tinp123 Posted at: 2019-09-10T09:12:31.408Z Reads: 17

```
if you want to stay on low budget, I would go with 2x flipsky 4.12 from ebay:

https://www.ebay.com/itm/HGLRC-Flipsky-V4-12-50A-SK8-PWM-Input-Speed-Controller-RC-ACC-For-E-Bike-M7X8/382813349195?hash=item592174254b:g:fWEAAOSwy2Ncd6iN

for remote, I would choose GT2B + some 3D printed mod. this is probably most reliable remote with really long battery life.

https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html

for on/off, go with simple xt90-s loop key - cheap and reliable solution. 

you can connect two vescs with split ppm - you will need only one receiver, but you will wire it to both vesc at the same time (only 5V wire connects to one vesc only). in this case, you setup every vesc as master with same exact settings. and yes, you can use normal vesc tool or you can use ackmaniac:

https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---

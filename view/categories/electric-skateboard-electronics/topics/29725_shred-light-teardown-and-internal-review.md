# Shred Light Teardown and Internal Review

### Replies: 6 Views: 1591

## \#1 Posted by: JdogAwesome Posted at: 2017-08-04T20:44:53.973Z Reads: 216

```
First off thank you @Chicagojoshua! he gave me a shred light to tear down and I thought I'd post a topic about doing so. Pretty much the shred light is based around the Cree XLamp XP-G3 which is actually a pretty nice LED. Its however very small and not very bright. The lumen output on max brightness was reading 300 Lux and on low brightness 120 lux (my method of testing at the end). On the main PCB of the entire thing was a couple small IC's. The main driver chip is a [CN5728](http://www.consonance-elec.com/pdf/datasheet/DSE-CN5728.pdf) "Multi-function High Brightness LED Driver IC" according to its datasheet. It features inbuilt High Brightness, Low Brightness and flashing Modes which works well for this small footprint and minimal part count. However it seems kinda sketchy as I could only find the IC for sale on [Alibaba](https://www.alibaba.com/product-detail/New-Original-IC-Electronic-component-CN5728_60426257355.html), nothing on Mouser or Digikey. Then a smaller IC Marked K168, though next to it on the PCB is marked [AP5054B](http://www.junyi-ic.com/upfiles/video/2012101218118.pdf) which is its actual part name. Its a Linear Li-Ion Battery charger for charging the tiny 230mAh battery(rated at 300mAh but actual capacity is 230). It again seems a little sketchy being that I can only find it on Alibaba, though it works. Next to it is a smaller SOT-23 chip that reads 1AMx and below that says 3904 which helped me find its part number, [MMBT3904](http://www.s-manuals.com/pdf/datasheet/m/m/mmbt3904_diodes_1.pdf). Its a NPN transistor, and the only IC I could actually find on [Mouser](http://www.mouser.com/ProductDetail/ON-Semiconductor-Fairchild/MMBT3904/?qs=sGAEpiMZZMvAvBNgSS9Lqpg%252bOuqhHUdo) lol. It seems to be there to just turn the red LED on when the device is charging, though I could be wrong. And yeah thats pretty much the entire very simple circuit. Now onto the battery, fist off the charging current is right around 230mA which means the battery charges in about an hour which is fine charging at 1C. However when I got ahold of it the battery was discharged down to 2.6V which is way to low! The battery does have a small BMS within the thin foil on the tip of it, you can see it in the pics below, though its clearly not doing its job of protecting the battery. Battery life is stated as being 2 hours at full brightness, though that would mean a draw of 110mA is needed at max. However 180ma is drawn at full brightness giving it a battery life of 1.2 hours, quite a bit lower than the 2 hour rating. However at  low brightness it only draws 66mA which would give you a battery life of 3.4 Hours almost 3x the high brightness battery life. Also before I end this off the lense cap they use for the XP-G3 LED looks very similar to these[ Carclo Lenses](http://www.ledsupply.com/cree-xpg2-led-optics) from LEDSupply.com. All in all the shred light is an ok product. Its got crap battery life, its not super bright and its way overpriced. Anyways below are the pics from the teardown, I hope this gives some insight into the internals of the Shred Lights. Also love how theres scotch tape on the top of it, not even sure what its there for its not holding anything together.

My Crude LED Testing Method: I've ordered parts to make an Integrating Lux Sphere for testing LED's, but ATM this is how I do it will update once lux sphere is finished. Pretty much I just have the LED and a lux meter app 6" above a white piece of printer paper and I take the reading like that, not ideal but it works. I also do it in a dark room.

<img src="/uploads/db1493/original/3X/f/d/fd545c7de1d32203b30cfd79bbbab46e4d65a1f8.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/3/a/3a8e1df9b5f65e7950fbc96c3e10c4637a8f7198.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/b/8/b88bdabd764208faeccb17ad0e481df34d568e43.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/1/e/1ef60ce2cff6f143d1eb0de14965dde12094600b.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/1/6/166726363846b490f45c768de9e5c69e820313c9.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/6/3/6360a07e73a22671caeaf769d227cdbaa8d39303.jpg" width="690" height="389">

Edit: The PCB seems to be coated in some sort of thin conformal coating which is a nice touch, though its only covered on this side, not on the led PCB or the backside. Pic below is the PCB under a black light. 
<img src="/uploads/db1493/original/3X/1/f/1f7a20c26375f9e80810adb591974b4d7b2ccf30.jpg" width="690" height="389">
```

---
## \#2 Posted by: saul Posted at: 2017-08-05T03:35:05.009Z Reads: 173

```
a good note is that the front and rear are the same. and its only the lens thats dyed red.

also I accidentally scraped off the "filter" on one of the leds so it looks blueish now. like an hid ;)
```

---
## \#3 Posted by: Lambjr088 Posted at: 2017-08-05T06:44:58.248Z Reads: 148

```
May be something way better can come put of this tear down with a better price lol
```

---
## \#4 Posted by: nmagz3 Posted at: 2017-08-07T19:08:08.951Z Reads: 115

```
Real thorough breakdown!  For me, understanding everything mentioned is a little above my paygrade.  However, as @Lambjr088 mentioned we can only hope for competitive products.  At the moment though, I really enjoy my ShredLights!
```

---
## \#5 Posted by: PJAM Posted at: 2019-09-18T17:31:32.109Z Reads: 36

```
Nice, thanks a lot for this post, gave a lot of useful info.
Got into reading it as I tried to tear down one of my own which started to defect. 
Got the weirdest symptoms: light stays on all the time and thus drains the battery. I did a quick test, plugged in and battery detached: Third push of the button does nothing apart from making it blink once.
Can't figure out what's wrong there. Best guess is that the main IC's f*cked up, but I understand that's rather unusual to have a component like this breaking all of a sudden.
Either I get a new IC and try to replace it, but I fear that's above my soldering skills. Or I could install a switch somewhere to bypass the defectuous turn-off function.
Any advises or ideas? Anyone else experiencing same issue?
```

---
## \#6 Posted by: murdomeek Posted at: 2019-09-19T22:38:57.905Z Reads: 24

```
just install a manual on/off switch
```

---

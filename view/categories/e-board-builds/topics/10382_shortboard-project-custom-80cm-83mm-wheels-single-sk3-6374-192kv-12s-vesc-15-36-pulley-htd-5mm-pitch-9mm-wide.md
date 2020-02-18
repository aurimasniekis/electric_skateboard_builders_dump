# Shortboard Project &#124; custom 80cm &#124; 83mm wheels &#124; single SK3 6374 192KV &#124; 12S (?) &#124; VESC &#124; 15/36 pulley &#124; HTD 5mm pitch, 9mm wide

### Replies: 9 Views: 1236

## \#1 Posted by: Artie Posted at: 2016-09-29T21:35:20.240Z Reads: 182

```
Hi everyone, new user here. Looking to build my first eSkate, been doing some reading online but as any newbie in the field I’ve still got plenty of doubts.

Before talking specs, some clarifications: I’m a tiny lass of 51kg (112lbs for you Americans out there), and will primarily be using my eSkate to cover medium-short distances on fairly flat ground. Roughly aiming at a theoretical max speed of 45km/h (28mph), which as we all know is going to be a tad less in reality.

Because I need my board to be as light as possible and easy to carry around, I’ve opted for a 80cm (31.5") deck. Still far from definitive, but I think I’ve got wheels and motor more or less figured out:

- 83mm wheels, either [Everland’s](https://www.amazon.com/gp/product/B00JFBTDDK/ref=ox_sc_act_title_1?ie=UTF8&psc=1&smid=A2DQMI7AS28KLN) or [Enertion’s](http://www.enertionboards.com/buy-build-your-own-electric-skateboard-parts/83mm-enertion-power-wheels/)

- [Turnigy SK3 6374 192KV](http://www.hobbyking.com/hobbyking/store/%5F%5F18129%5F%5FTurnigy%5FAerodrive%5FSK3%5F6374%5F192kv%5FBrushless%5FOutrunner%5FMotor.html) single motor 

Battery: the SK3 6374 192KV requires a voltage of 10-12S. Would a 10S (2x [Turnigy 5000mAh 5S 20C](http://www.hobbyking.com/hobbyking/store/__9174__Turnigy_5000mAh_5S_20C_Lipo_Pack.html)) suffice, or am I better looking at a 12S (2x [Turnigy 5000mAh 6S 20C](http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=9176), or maybe even 4x [Turnigy 5000mAh 3S 20C](http://www.hobbyking.com/hobbyking/store/__9184__Turnigy_5000mAh_3S_20C_Lipo_Pack.html))? I know there are already a bunch of threads on this, but most of them deal with longboards and/or heavier riders wanting to climb steep hills, which isn’t my case.

ESC vs. VESC: from what I’ve read the latter works swell with both 10 and 12S, so unless you lovely folks have a cheaper and more efficient alternative to suggest, I think I’ll get a VESC, either [Enertion's](http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/) or [DIY's](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/).

Wireless Remote Control: similar story as above, still undecided between [Enertion's](http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/) and [DIY's](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/). I've also read all sorts of praises for the GT2B, but...ah, it's just too big.

What else — pulleys and belts, I guess a 5mm HTD pitch with a 9mm wide belt, wheels are going to be 83mm so 15/36 teeth should work nicely, but by all means correct me if I'm wrong.

Done rambling for now, any advice is most welcome!
```

---
## \#2 Posted by: lox897 Posted at: 2016-09-29T21:52:47.104Z Reads: 169

```
Battery: You should be fine with 10S and 192kv, it will probably get you the speeds you want. If you really want to go higher voltage, it is an increased risk of breaking the VESC.
2x 5S would be ok for 10S but you wouldn't have as much ground clearance so if you are going 12S use 3x4s batteries.

ESC: Sounds good!

Transmitter: Enertion's hasn't been tested yet and DIY 2.4ghz mini remote works well. DO NOT GET THE NANO, THEY ARE NOT RELIABLE. diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/ this one is good

Belt and pulleys: Yep
```

---
## \#3 Posted by: daanstoorvogel Posted at: 2016-09-29T21:53:34.276Z Reads: 163

```
hi great that you are getting started . my question if you are only 50 kg and fairly flat ground you want light and convience so why not a carvon single ?  remote gt2b with a mod ?  battery lipo is probberbly fine but charging so many different ones can be a pain in the ass  so maybe lipo + BMS or just a 18650 pack + BMS
 eitherway good luck  dont short your lipo's i have learned from my mistakes
```

---
## \#4 Posted by: Artie Posted at: 2016-09-30T13:34:06.372Z Reads: 128

```
All right, 2x 5S then. Thanks for the advice on the transmitter, although why are you saying the nano isn't reliable?
```

---
## \#5 Posted by: Artie Posted at: 2016-09-30T13:55:19.851Z Reads: 122

```
I've considered hub motors myself, but they perform rather poorly compared to a good old geared system, plus they overheat easily.
```

---
## \#6 Posted by: SteveS Posted at: 2016-09-30T17:23:31.435Z Reads: 117

```
The configuration you've spec'd will give you a top speed of about 34mph at 12S. Given your speed objective, I'd suggest you get a 168kv or 149kv SK3, which will give you top speeds of 30 or 27mph, respectively, but better torque/acceleration. 

My first build was nearly the same as you propose and I switched from the 192kv to a 149kv motor and am much happier.
```

---
## \#7 Posted by: Spek Posted at: 2016-09-30T17:35:04.462Z Reads: 118

```
A gt2b enclosure mod was easy for me to do with 0 experience. Dremel and one quick solder to the battery were the hardest parts. I'm not sure what my modded enclosure is called but it's 3d printed and very nice and pocket sized. It's worked perfectly for me with no signal issues at all.

<img src="/uploads/db1493/original/3X/b/a/ba68e55c178fc753aeb6a6cc743ce407b1e4d31c.jpg" width="281" height="500">
```

---
## \#8 Posted by: lox897 Posted at: 2016-10-01T02:56:36.315Z Reads: 96

```
Lots of bad reviews
```

---
## \#9 Posted by: Namasaki Posted at: 2016-10-01T05:32:21.735Z Reads: 95

```
one option is 2s lipos in series with a bms. 
Plenty of power and low profile, only 1" thick 
I've been using these high output 2s/5000/60c lipos for a short time but they seem to deplete much slower than lower C rated packs and have very little voltage drop under load.
Also, I agree with Lox897, 10s is perfect with 190kv motors. 
<img src="/uploads/db1493/original/3X/0/9/0946e4b712a96f418f028b67367f857d2b903243.PNG" width="281" height="500">
<img src="/uploads/db1493/original/3X/7/e/7e1bb8dbc6a563eac07ff44f2e39578de922bdf4.JPG" width="666" height="500">
```

---

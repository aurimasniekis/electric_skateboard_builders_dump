# Proofcheck for my first build before I buy

### Replies: 20 Views: 1586

## \#1 Posted by: MicroRAsus Posted at: 2016-07-22T20:56:17.705Z Reads: 135

```
Hi electric skateboard builders,
        For the past few days I have been researching how DIY electric skateboard works, and I have few parts I found that I'm really interesting in. I have 1 years of experience on building RC quad-copter and fix-wing but have never touched cars or some thing that runs on ground, I also never skate before, so for my first build I want it to be easy to build and low chance of error. My ideal top speed is 30MPH ± 5MPH, I really don't want to go too fast because I never skate before and using this [calculator](http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html) I got Weighted Top Speed ~27MPH. so my concerns are if my parts gonna fit other parts and are there any better alternatives? your input would be much appreciated :)

Dual Motor Mechanical Kit  $325.00  from 
diy-electric-skateboard-kits-parts/torqueboards-dual-motor-mechanical-kit/
Motor Mount, Trucks, 16/36T Pulleys, 90mm wheel etc.  Kinda expansive but all I need for low chance of error and better looking.

YOCAHER PUNKED CREST ONYX LONGBOARD DECK     $45  from ebay
https://www.yocaher.com/product/punked-crest-onyx-drop-through-longboard-deck
The shape of this drop thru deck looks great. low flex.

Dual Motor Electric Skateboard Kit + VESC CanBus Connector $366.99  from 
diy-electric-skateboard-kits-parts/vesc-canbus-connector/
diy-electric-skateboard-kits-parts/dual-motor-electric-skateboard-kit/
2X opensource VESCs + 2x 6355 230kv motors + CanBus Connector for VESC slave mode
I really like VESC, they are open source and has many features like reverse direction when using nunchuk, I wonder if this feature will ever come to normal controllers. also headlight, I wonder how he did it, never found any tutorial on it.
motors seems ok to me, 55 motor looks like the only option for dual rear, I would go for 76 for diagonal but I heard the board would want to turn one way if brake hard. @onloop 

controller:
Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System      $22.39   from hobbyking
http://www.hobbyking.com/hobbyking/store/__51700__Quanum_2_4Ghz_3ch_Pistol_Grip_Tx_Rx_System_US_Warehouse_.html
This one looks small enough and cheap, I wanted to use nunchuk so I can do reverse direction and cruising control but I heard nunchuk drop out a lot and dangerous.

Batteries:
Turnigy 2200mAh 1S 40C Lipoly     x21            from hobbyking
https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=59008
I brought these batteries for my racing quadcopter, and I have 21 of them left, I'm thinking on DIY it into 9S2P, so I don't reach max RPM on VESC, at 9S2P I will have 37.8V 4400mAh full charged and capable of outputing 176 amps. I will build it as 6x3s batteries because my power lab 6 charger can only charge and balance up to 6s, so there will be a lot of connectors.. you guys have any better idea?

electronic enclosure:
Plano 3600 Waterproof Stowaway      from  walmart
http://www.walmart.com/ip/Plano-Guide-Series-3600-Waterproof-Stowaway/17126450
Cheap and easy, although it doesn't look good but I want to gain access to batteries because 6x3s is too much connectors and I need to take out to charge. I will use some Velcro on batteries and VESC inside so it won't fall off if lid pop open. the only concern is how I install this Plano box, do I just drill holes in the deck and Plano box then use bolts and nuts? what if these hole caused box to crack? any ideas?

LED:
9 Mode Multi Colour/Multi Function LED strip with Control Unit   from hobbyking
https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=65188
I will use a spare channel from receiver for this led control. does control of esk8 only take 1 channel?

miscellaneous:
XT90, XT60, 10AWG WIRE, loctite, velcro, epoxy and tools
is skate T tool necessary? I have bunch nut screwdrivers will they fit?

Thanks in advance, looking forward to your suggestions!
```

---
## \#2 Posted by: mason Posted at: 2016-07-22T21:13:47.836Z Reads: 106

```
looks good! you will need some [aluminum solder](https://www.amazon.com/Aluminum-Solder-Wire-062-Flux/dp/B00DC3102Y/ref=sr_1_5?ie=UTF8&qid=1469221987&sr=8-5&keywords=aluminum+solder) for the batteries because the usual stuff will not stick to the tabs.
```

---
## \#3 Posted by: MicroRAsus Posted at: 2016-07-22T21:15:00.728Z Reads: 101

```
Got these [aluminum solder flux](http://www.ebay.com/itm/like/272285066105?lpid=82&chn=ps&ul_noapp=true) ! It is pretty messy stuff, though. any idea on the enclosure? that is my biggest concern.
```

---
## \#4 Posted by: anorak234 Posted at: 2016-07-22T21:21:59.263Z Reads: 99

```
Looks good, but I've had mixed experiences with yocaher products. I'd say go for a different deck, or better yet just build your own.
```

---
## \#5 Posted by: lox897 Posted at: 2016-07-22T22:16:01.922Z Reads: 93

```
Don't get the quanum, it works for a bit and then after a while, it can't bind. Also, battery is shit. No one on this forum will recommend the quanum.
```

---
## \#6 Posted by: MicroRAsus Posted at: 2016-07-22T22:35:45.567Z Reads: 86

```
What about [GT2B](http://www.hobbyking.com/hobbyking/store/__31671__HobbyKing_174_8482_HK_GT2B_3CH_2_4GHz_Transmitter_and_Receiver_w_Rechargable_Li_ion_Battery.html)? It seems bulkier.
```

---
## \#7 Posted by: barajabali Posted at: 2016-07-22T22:53:43.145Z Reads: 81

```
I have a 12s lipo never used if you're interested
```

---
## \#8 Posted by: lox897 Posted at: 2016-07-22T22:55:36.446Z Reads: 80

```
There are a few good remote options:
GT2B with 3d printed casing mod
2.4ghz trigger remote aliexpress sold by diyelectricskateboard
2.4ghz thumb remote sold by @Kaly
```

---
## \#9 Posted by: sl33py Posted at: 2016-07-22T23:07:51.642Z Reads: 81

```
Also suggest the GT2b over the Quanum.  Quanum worked for me, but went through batteries pretty fast.  And worst of all - looks like a gun.  Not the best idea nowadays!

here's an old how-to for moving GT2b into smaller badwolf enclosure.  Relatively simple w/ some basic tools and solder skills.
http://www.electric-skateboard.builders/t/how-to-hack-build-compact-controller-using-gt-2b-badwolf-v2-enclosure/114

HTH - GL!
```

---
## \#10 Posted by: MicroRAsus Posted at: 2016-07-22T23:12:04.597Z Reads: 72

```
I can't use 12s because my motor is 230kv
```

---
## \#11 Posted by: sl33py Posted at: 2016-07-22T23:20:04.870Z Reads: 70

```
CORRECT ANSWER!

hehehe - it looks like you have done your reading and research at least!  

for wire i would suggest the wet noodle or superworm wire (on Amazon).  12g should be enough, but 10 will definitely work too.

Skate tool - YES!  everything right where you need it when you need it.  Go skate sometime with loose trucks and you'll wish you had it in your pocket/bag to tighten them up!  even an el-cheapo one of $5-6 is great to have.

Sometimes it will be easier to use your sockets like when assembling, but a skate tool is really handy for adjusting and small changes and maintenance.
```

---
## \#12 Posted by: barajabali Posted at: 2016-07-22T23:20:08.455Z Reads: 67

```
Sure you can i do.

I use dual 230kv on 12s. Gives me about 35 top speed with my weight. I weigh 210
```

---
## \#13 Posted by: MicroRAsus Posted at: 2016-07-22T23:20:23.322Z Reads: 66

```
great tutorial! I have access to most tool needed but 3d printer, I think I will do the modding when I'm back to university, thanks for the suggestion!
```

---
## \#14 Posted by: sl33py Posted at: 2016-07-22T23:21:42.703Z Reads: 64

```
not doubting, but i thought that wasn't possible.  Multiple folks have killed their VESC trying.

what hw version VESC and any mods to support >200kv on 12s?
```

---
## \#15 Posted by: MicroRAsus Posted at: 2016-07-22T23:22:06.795Z Reads: 63

```
are you using vedder esc?
```

---
## \#16 Posted by: sl33py Posted at: 2016-07-22T23:22:48.527Z Reads: 64

```
I didn't have a 3d printer either - got mine printed from 3dhubs and another online store.  worth the $ to make it so nice and small IMO.  If you have access to one at university - even better!
```

---
## \#17 Posted by: barajabali Posted at: 2016-07-22T23:24:26.525Z Reads: 66

```
I don't use the VESC. I use TB ESC's which I have for sale if you're interested.
```

---
## \#18 Posted by: barajabali Posted at: 2016-07-22T23:24:44.693Z Reads: 67

```
No I don't use the VESC I use TB
```

---
## \#19 Posted by: MicroRAsus Posted at: 2016-07-22T23:37:15.031Z Reads: 69

```
TB esc doesn't have RPM limit, that is why you can use 12s on it.
```

---
## \#20 Posted by: MicroRAsus Posted at: 2016-07-23T02:40:15.413Z Reads: 59

```
I found your reply on a old thread, using heat gun to DIY abs enclosure!? great inspiration. I think I will use my lamination iron to do that, 450 degc enough? will it stick to the base of my iron?
```

---

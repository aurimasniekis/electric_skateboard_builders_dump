# Can I use this BMS with these cells? / Equipment check

### Replies: 5 Views: 165

## \#1 Posted by: iMattcat Posted at: 2019-06-13T14:49:08.448Z Reads: 40

```
Hey guys, I'm new here so let me know if this is in the wrong place or something.

So I have decided that I need a new board; I had a Meepo Campus 2 for a year now and she's been fantastic, but I think it's time for an upgrade. So I decided I wanted a Meepo Mini 2 ER because it can go 20 miles (range) and 29 mph, and it's compact. But the thing is pretty expensive, so I did a bunch of research and decided to build my own. The Meepo ER battery is a 10s2p battery with Samsung 21700 40T cells and it has a 60A discharge current. (I'm not an expert on the numbers) Problem is, it's 300 bucks.

So I've decided to make my own. I've done my research and I know how to assemble the battery and everything. On Liion wholesale I've secured the cells for around 150 bucks, and the rest of the supplies I need to construct the battery pack on amazon. However I'm still a little iffy on the compatibility of the electronics. My greatest concern is that I have a sinking feeling that maybe this choice of BMS or ESC will limit the power that the battery can supply to my motor, decreasing speed, power, or worse: range.

Will this BMS allow the battery to operate to its full potential, will it limit the battery/performance, or will it not allow the board to function at all? 
Will the ESC or Motor choice limit the board's performance?
Do you guys see any red flags with my equipment? 
Do you have any warnings or advice?

My goal is to make a functional board that can go 20 miles or more. Speed isn't as important, but being able get to 29 like the Meepo Mini ER would be nice.

The Cells: 
https://liionwholesale.com/products/samsung-40t?variant=12252585885790

The BMS:
https://www.amazon.com/gp/product/B074WZL5NF/ref=ox_sc_act_image_2?smid=A2KRDQ1AI5Y5G6&amp;psc=1

The ESC:
http://www.diyeboard.com/v20-dual-hub-motors-sine-wave-foc-esc-speed-controller-p-674.html

The Hub Motors:
http://www.diyeboard.com/replaceable-pu-dual-hub-motor-9055mm-500w2-power-truck-kit-p-671.html


Thanks in advance! I really appreciate any feedback!
```

---
## \#2 Posted by: TheSebas Posted at: 2019-06-13T15:05:05.805Z Reads: 35

```
I'd stay away from that BMS, it's not rated for 40A. What you probably want to do is use your BMS for charging only, this means that your battery (depends on your ESC) can deliver it's full potential.
And diyeboard is a sketchy site, i wouldn't order from them.
```

---
## \#3 Posted by: iMattcat Posted at: 2019-06-13T16:15:52.375Z Reads: 31

```
Okay, how do you set up a BMS so that it only regulates the charging and not the battery's flow to the ESC? And if I do set it up that way, would I still be able to use this same BMS to charge the battery but not deliver from the battery to the ESC?

Also what Ampere rating (or just BMS in general) would you recommend?
```

---
## \#4 Posted by: TheSebas Posted at: 2019-06-13T16:34:12.091Z Reads: 28

```
Most BMS's have 3 ports, the CH-, P- and B-
The CH- goes to the negative side of your charging port, the P- is if you want to discharge with the BMS (So you won't be using that in your case)
And the B- takes care of the balancing of the cells.

Yes, you will be able to use the BMS for charging.

The ampere rating doesn't really matter for charge only, something like this: https://www.aliexpress.com/item/10S-16A-PCM-PCB-BMS-for-36V-lithium-battery-pack-for-electric-bicycle-and-scooter-and/32810007406.html will do.
If you want you can shoot me a PM :smiley:
```

---
## \#5 Posted by: iMattcat Posted at: 2019-06-13T20:10:07.643Z Reads: 14

```
I appreciate your advice more than you know! Thank you so much, I'll keep you updated
```

---

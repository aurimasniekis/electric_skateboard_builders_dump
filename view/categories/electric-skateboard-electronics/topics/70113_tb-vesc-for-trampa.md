# TB Vesc for trampa

### Replies: 16 Views: 238

## \#1 Posted by: JensSjogren Posted at: 2018-10-04T08:18:26.754Z Reads: 95

```
I'm just about to recieve my package from , it will contain the parts i need to electrify my trampa MTB. After reading alot of negative stuff about the Torqueboard Vesc (products/torque-esc-bldc-electronic-speed-controller) i'm starting to get worried if it will be able to handle my build. I will use a 12s5p li-ion battery and 2 149kv 3500 watt motors with a max amp of 80. 

According to the description of the TB vesc it should be able to handle 14s battery voltage and 50A continious current (240A peak). This should in theory be enough for my build but why does it seem like most people use this ESC for low powered builds? Would the Focbox be better/safer? 

Best regards//Jens
```

---
## \#2 Posted by: Lumaci Posted at: 2018-10-04T08:22:17.304Z Reads: 88

```
Yes a Focbox would be a lot safer, the quality of the parts used on this vesc is low and they cant handle much also in generel the vesc 4.xx layout isnt that good.

A focbox or one of the better vesc 4.12 with upgrades or one of the vesc 6s / clones would be better.
```

---
## \#3 Posted by: JensSjogren Posted at: 2018-10-04T08:42:27.965Z Reads: 79

```
Okay i see, would there be any harm in trying the TB vesc? If it gets fried do i risk harming my battery or motors?
```

---
## \#4 Posted by: Lumaci Posted at: 2018-10-04T08:43:42.873Z Reads: 71

```
You would most likely just fry the DRV really fast on it, i would just not use it and sell it here.

They are really aimed at budget boards using a single small motor at like 30 - 40A MAX for reliability.
```

---
## \#5 Posted by: JensSjogren Posted at: 2018-10-04T09:04:57.515Z Reads: 68

```
I see, but why would the TB vesc be specified to handle 12s and 50a continous if it doesnt? 

Even ther biggest diy kit has the same Vesc (collections/electric-skateboard-conversion-kit/products/pro3-electric-skateboard-conversion-kit). This kit has 12s battery and 2 3150 watt 80a motors. Feels a bit funny that they would sell this Vesc togheter with those components if its not rated for it
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-04T09:16:20.860Z Reads: 64

```
motor amps not battery amps.
and you know... marketing ;)
as far as I know all components on the vesc can handle 50a cont. 
but this was testet with a big heat sink on each fet.
on this vesc no heatsink at all so...
yes you can write 50a as it´s what the datasheet of the components say but that´s not real live values.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-04T09:26:36.416Z Reads: 62

```
no problem to use them as you anyhow bought them.
just limit your bat max to 35A per vesc maximum.
if you have an opportunity, try to add a heatsink and place them with a good airflow (heatsink should stay out of the enclosure or box).
If you fry something than it probably will first fry your drv.
which could cause a dangerous cut out though... depending on your riding skills and speed.

one thing to notice too. 
all the vesc based esc rated to 60V. which does not mean it´s safe to go on the limits. I think it´s a bit not so good to advertise that product for 14s, which will be with fully charged batteries already 58,8V.
Always expact voltage spikes (because of long battery wires etc.) this spikes can fry your esc too.
```

---
## \#8 Posted by: JensSjogren Posted at: 2018-10-04T10:44:48.472Z Reads: 58

```
Thanks for the input, i went ahead and ordered 2 focboxes since they are on sale for  120€ each anyways! :) ill just try to sell the vescs here when they arrive
```

---
## \#9 Posted by: JensSjogren Posted at: 2018-10-04T10:45:36.026Z Reads: 57

```
The focbox is rated for 50v max though, my battery will be 52v when fully charged, could this cause issues?
```

---
## \#10 Posted by: Lumaci Posted at: 2018-10-04T10:49:05.773Z Reads: 57

```
[quote="JensSjogren, post:8, topic:70113"]
120€
[/quote]

Where did you get them for that cheap? :O


Edit holy shit just got two on enertions website for 200 Euro in total.

They are dirt cheap atm.
```

---
## \#11 Posted by: JensSjogren Posted at: 2018-10-04T11:08:34.014Z Reads: 53

```
My was 240 in total, that seems a bit wierd 🤔 191 AUD on enertion website?
```

---
## \#12 Posted by: Andy87 Posted at: 2018-10-04T11:09:01.810Z Reads: 52

```
12s is 50,4V minus the sag you will have non the less and you goo with 50V :stuck_out_tongue_winking_eye:
i think it´s same with focbox, the volatge spikes shouldn´t exceed 60V.
50V is the recommendet max volage you should operate them.
There are guys here running focbox on 13s too. if good or not, it´s a other question
```

---
## \#13 Posted by: Lumaci Posted at: 2018-10-04T11:09:39.016Z Reads: 52

```
if you put them in your cart and close the website they email you a 11% code.

So each of mine were 103 euro in total incl tax so a total of 206.
```

---
## \#14 Posted by: JensSjogren Posted at: 2018-10-04T11:52:33.474Z Reads: 43

```
Awww damn, didnt know that trick 😅
```

---
## \#15 Posted by: JensSjogren Posted at: 2018-10-04T18:11:36.037Z Reads: 27

```
I see that focbox uses xt60 plugs, i can just cut those of and solder xt90 plugs instead right?
```

---
## \#16 Posted by: Pedrodemio Posted at: 2018-10-04T18:14:02.572Z Reads: 26

```
Test them before going forward, lot of work to mount everything to find they don’t even work, that was my experience with them

Hopefully they improved que QC since I bought
```

---

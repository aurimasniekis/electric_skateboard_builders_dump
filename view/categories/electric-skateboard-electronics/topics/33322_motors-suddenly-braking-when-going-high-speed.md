# Motors suddenly braking when going high speed

### Replies: 22 Views: 1218

## \#1 Posted by: Lulu Posted at: 2017-09-17T09:31:05.139Z Reads: 135

```
Was riding two days ago fairly fast and the motors just hit the brakes for a second and threw me off the board. lost a lot of skin and swollen n bruised knees
Anyone know why it did this? It did a similar thing while trying to get to the hospital but going low speed. every few minutes the brakes would go on then off.
Set up is 
10s4p Space cell
2x 4.12 VESCS
Carvon V3 motors
Winning Remote.
Photos of current settings<img src="/uploads/db1493/original/3X/e/1/e19f0fb2d67c2f5b330053c76307364ebcb38632.png" width="690" height="406"><img src="/uploads/db1493/original/3X/7/f/7fa112280a5a0c4e6386e67bed7c321e305b342f.png" width="690" height="406">
```

---
## \#2 Posted by: Silverline Posted at: 2017-09-17T09:35:10.400Z Reads: 123

```
Pretty sure it's your winning remote. Many people including me, have similar Problems with that Shitty remote. I now use Gt2b without any problems at All.
```

---
## \#3 Posted by: Lulu Posted at: 2017-09-17T11:35:20.322Z Reads: 118

```
damn, well that sucks. I bought it from enertion and this is what i got. 
So it seems to be the remote not having a connection and sending a 0 signal which is the same as full brake to my motors. which was a fun trip to the hospital
Any other smaller remotes around that are good, i think the gt2b is too bulky for my tiny hands.
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-17T11:43:09.016Z Reads: 113

```
You can 3d print an enclosure for the gt2b or buy a 3d printed one
```

---
## \#5 Posted by: pat.speed Posted at: 2017-09-17T11:45:56.973Z Reads: 114

```
You could buy a mini remote from @torqueboards, @JLabs or eBay for cheap
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-09-17T13:25:53.704Z Reads: 109

```
Just connect to bldc-tool and go to the ppm tab. Enable the "Display" Checkbox and switch on your remote. Then switch it off again. If the percntage that is displayed is far less than 50% then this is the reason for your braking behavior. 
So the failsafe needs to be adjusted so that when the the remote is off the signal should be at 50% percent.
Mostly you can do this by adding the bind plug and remove the bind plug while the remote is switched on an in idle.
By this the receiver knows where the idle position is.
Because when the Reciever looses the connection to the remote it still sends this failsafe signal to the VESC. And if this is set too low the VESC will brake. If it is set too high the VESC will accelerate.

Would be great if there is a possibility to let the VESC know that the PPM receiver lost connection to the PPM remote.
```

---
## \#7 Posted by: JLabs Posted at: 2017-09-17T13:41:32.942Z Reads: 104

```
Thanks for the shout @pat.speed! I can ship tomorrow if the order is placed today (and it’s 50% of the price compared to DIY)

https://buildkitboards.com/products/mini-remote
```

---
## \#8 Posted by: Lulu Posted at: 2017-09-17T14:16:32.741Z Reads: 99

```
Thanks, I've rebinded and set it to the 50% and when switched off it goes to 50%.
The remote still has the issue of losing connection and reconnecting about once a minute.

Just checked out your remote @JLabs and it costs more than the actual remote to ship to australia :< The feels.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-09-17T16:03:49.135Z Reads: 88

```
Check eBay for the mini remote. 
You might be able to get free shipping directly from the China supplier.
```

---
## \#10 Posted by: darkkevind Posted at: 2017-09-17T17:40:15.579Z Reads: 79

```
Just as another possible cause for this, althoug I'm pretty sure it's the Winning remote as it's crap...

I just had this kinda happen to me but it was basically because of the shitty cycle paths around my way... One of my phase wires' 4mm banana connector came loose (inside my enclosure) and as soon as it happened the motor behaved like it was braking! Then it would connect for a sec, (as I got slower - less bumpy), then I had power again, then as I got faster and more bumpy, it disconnected again!
I only found this out as I pulled over and took my enclosure off mid-ride.

Put it back together tightly, put the enclosure back on and it was fine again. So just check your phase wires are really tight and secure :thumbsup:
```

---
## \#11 Posted by: pat.speed Posted at: 2017-09-17T21:15:41.027Z Reads: 70

```
Ahhh yeah I live in Aus too and shipping is a real pain otherwise I would have gotten some wheels from JLabs. They sell the remotes on eBay for about $25 Aus
```

---
## \#12 Posted by: Surfer Posted at: 2017-09-17T21:57:38.916Z Reads: 66

```
I use benchwheel and is awesome, no one cut of in a year, battery last for a week or more, 2 speeds, a sound like a "piiit" when switch on or off, and nice form factor, 45 bucks in Alibaba. Now I think even cheaper, just check if the receiver is included!
```

---
## \#13 Posted by: Clonkex Posted at: 2017-09-17T23:33:13.065Z Reads: 57

```
I'm also in Aus. I'm going to be buying some wheels from @JLabs but the shipping means it'll take me a couple more weeks to save enough money. I feel your pain.
```

---
## \#14 Posted by: JLabs Posted at: 2017-09-17T23:35:35.349Z Reads: 58

```
Yeah I'm really sorry guys, I wish it was cheaper but shipping anything from the USA is not cheap, even domestically.
```

---
## \#15 Posted by: Clonkex Posted at: 2017-09-17T23:38:47.801Z Reads: 55

```
We know man, not trying to guilt you ;) Most stuff on eBay has free shipping or very low cost shipping so we get used to that and it's hard to accept when shipping costs nearly as much as (or more than!) the product itself :P
```

---
## \#16 Posted by: Ulfberht Posted at: 2017-09-18T00:08:19.750Z Reads: 51

```
Winning=Losing skin...
It's not the cheapest, but the @MasterCho  mod is awesome. http://www.ebay.com/itm/GT2B-Electric-Skateboard-Controller-Housing-Case-Enclosure-BLACK/252496558132?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2648
You have to get a GT2B, the most reliable known controller, and gut it. It's super easy. 
@Smorto put together a really great tutorial here: http://www.electric-skateboard.builders/t/gt2b-mastercho-chozen-mod-full-length-tutorial-how-to/16005
<img src="/uploads/db1493/original/3X/3/f/3f6d5787fb398edee98d298390021698a21e3552.jpg" width="500" height="400">
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-09-18T00:43:56.550Z Reads: 47

```
Just buy one here.

[Mini Remote from Aliexpress](https://www.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32573238408.html?spm=2114.search0104.3.1.A4d0gr&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10344_10342_10343_10340_10341_10193_10194_10304_5550020_10307_10137_10060_10302_10155_10154_10056_10055_10054_5470020_10059_100031_10099_5460020_10338_10339_10103_10102_440_10052_10053_10107_10050_10142_10051_10320_10321_10322_5380020_10326_10084_10083_10080_10082_10081_10177_10110_10111_10112_10113_10114_143_10180_10312_10313_10314_10184_10078_10319_10079_10073_10186,searchweb201603_19,ppcSwitch_5&btsid=afa74c38-95db-4f2f-a45b-dc7ea4fdfb4e&algo_expid=7171b750-714a-41d4-af90-b91a41f7be33-0&algo_pvid=7171b750-714a-41d4-af90-b91a41f7be33)
```

---
## \#18 Posted by: mmaner Posted at: 2017-09-18T00:47:25.432Z Reads: 48

```
The Nano-X and Benchwheel remotes are great, @psychotiller has the new version of the stressing remote and it's pretty awesome too. The mini remote that @torqueboards and @JLabs sell is a solid remote but I like a thumb trigger better.
```

---
## \#19 Posted by: caustin Posted at: 2017-09-18T02:09:05.627Z Reads: 46

```
Actually I would like to hear more about the new maytech remote @psychotiller and Carvon are selling. @mmaner how does it compare as a thumb trigger to nanox and benchwheel?  Am hearing pretty positive comments, have not tried one yet though, how is the connectivity?
```

---
## \#20 Posted by: psychotiller Posted at: 2017-09-18T02:33:38.826Z Reads: 40

```
Jerry just told me tonight (in vegas, near casinos) he had interferance. But I'm wondering if the casinos employ technology to hinder hustlers that may also mess with 2.4ghz?

This is the first negative I've heard on this remote. Love the actuation on this thumb controller. Best so far.
```

---
## \#21 Posted by: mmaner Posted at: 2017-09-18T02:35:38.585Z Reads: 38

```
I haven't actually used it a lot, about 6 rides for maybe 50 miles total.  That being said I never had a dropout, the throttle response is actually better (more even) than the benchwheel.  I'm not crazy about the form factor but it works great.
```

---
## \#22 Posted by: darkkevind Posted at: 2017-09-18T07:51:25.679Z Reads: 28

```
Me too. Once I got over the initial supply problems with mine, my benchwheel remote & receiver have been faultless!
```

---

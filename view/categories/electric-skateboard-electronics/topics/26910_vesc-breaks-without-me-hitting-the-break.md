# VESC breaks without me hitting the break

### Replies: 11 Views: 883

## \#1 Posted by: faaailix Posted at: 2017-07-06T13:24:25.108Z Reads: 98

```
Hi,
I'm having a serious problem with my VESC build and wonder if someone has made the same experiences/knows a solution to it:

I run a single mounted 270KV motor with an 8S LiPo (2x4S in series), and I use VESC in BLDC mode. I used the BLDC tool to set all up. I skated with it about a 100 km without any problems. However, from one moment to the other while cruising, the break kicked in and threw me off my board (no injuries) - very scary! I first though I unintentionally hit the break. However, after running smooth for some time after it happened again and I'm sure VESC is hitting the break without me actively breaking. Does anyone have made the same experiance? Is it possible that motor parameters change over time due to wearing and rerunning a detection can solve this? It's quite scary since there is no good testing methods that guarantees that the problem is resolved.
* Remote: http://alienpowersystem.com/shop/radio-transmitters/alien-power-system-2-4ghz-electric-skateboard-remote-control/
* VESC: version 4.12; firmware version 2.18
<img src="/uploads/db1493/original/3X/0/8/080b30d35f552a7b4eaedcefa962ce7611987602.png" width="690" height="388"><img src="/uploads/db1493/original/3X/5/6/5690b2784249f410d223545dcb67e1506f684be3.png" width="690" height="388"><img src="/uploads/db1493/original/3X/1/d/1d598e8cb927731360416ba87b9b911c39077bae.png" width="690" height="388"><img src="/uploads/db1493/original/3X/2/c/2cc2498e7b2604944c9931cf41e171271c833a55.png" width="690" height="388">
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-06T13:25:10.359Z Reads: 86

```
Post some screenshots. What remote are you using?
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-07-06T13:28:23.280Z Reads: 88

```
Sound like an erpm brake with that setting. Post your BLDC tool screenshots.
What gearing are you using?
```

---
## \#4 Posted by: faaailix Posted at: 2017-07-06T13:31:39.343Z Reads: 86

```
Thanks for your quick response. Have updated the original post (VESC hardwear version + remote control information). Posting screenshots of my BLDC setting in the evening.
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-07-06T13:53:17.963Z Reads: 87

```
probably just a PPM setting. Probably got your min and max set wrong.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-07-06T14:26:36.666Z Reads: 74

```
Agree with @longhairedboy check your PPM setting... here is a tutorial that may help you

 http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes-ppm/244
```

---
## \#7 Posted by: Silverline Posted at: 2017-07-06T14:41:15.845Z Reads: 72

```
270kv motor on 8s gives a lot og rpm's. Shouldn't the rpm's be lower on 8s ?
```

---
## \#8 Posted by: faaailix Posted at: 2017-07-06T17:48:59.965Z Reads: 58

```
I added the screenshots to the initial comment. Anything suspicious?
```

---
## \#9 Posted by: wafflejock Posted at: 2017-07-06T18:51:14.174Z Reads: 53

```
Check the display box on the ppm configuration page check pulling full throttle vs pushing full brake and let it sit idle, is it at 50% if not adjust the min/max ms value to match what you actually see it read out when you push to min and max.  If it drifts more than your deadband % away from center (if deadband is 15 +/-7.5% of 50) then it starts to go into motion.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-07-06T20:34:28.765Z Reads: 44

```
Just watch the ppm Display in tue BLDC Tool and shake and squeze your remote. I also had One where the potentiometer send crazy Signals when I squezed it in the potentiometer area.
I guess there is a better in english to describe that but hopefully you get my point.
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-06T20:58:18.971Z Reads: 36

```
Yeah this is definitely true if you squeeze the potentiometer itself you can change the surface contact and ultimate resistance between the parts in the potentiometer so if it's flexing around you might get weird values.  I also had a stereo system with a crappy potentiometer that had the same problem, replaced it with my own from a pile, problem solved :)
```

---

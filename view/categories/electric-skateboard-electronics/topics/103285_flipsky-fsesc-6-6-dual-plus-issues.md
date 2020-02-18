# Flipsky FSESC 6.6 Dual Plus issues

### Replies: 39 Views: 891

## \#1 Posted by: levan634 Posted at: 2019-10-25T14:48:46.285Z Reads: 176

```
Super new to DIY eskates and was looking to upgrade my cheap complete longboard I got from diyeboards. I figured I would try my luck with FSESC 6.6 dual plus.

After setting it up in VESC tool and tested it on the actual road, I ran into some cut out issues. On the Xmatic app on my phone, I tracked my ride and noted that I received two fault codes repeatedly. The two codes are FAULT_CODE_DRV & FAULT_CODE_UNDER_VOLTAGE (i have attached a screenshot below). The cut out happens when I am doing full-throttle on the remote (VX2) for about 5-8 secs straight. I hit about 25-30kph before the cut out. The vesc itself would actually power off. Below are my specs and settings:

Belt Driven Longboard

5055 x 2 motors 270KV (from diyeboards) - 80a max continuous
motor pulley - 13t, wheel pulley - 35t
Flipsky FSESC 6.6 dual Plus w/ Switch
10s5p 10ah battery -> 50a continuous current
UART VX2 Remote
NRF for bluetooth connectivity 

Motor Settings on VESC TOOL (FOC sensorless mode):

Motor Amps max: 60a

Motor Amps min: -40a

Battery amp max: 50a

Battery amp min: -20a

Max ERPM: 60000

![PNG|230x500](upload://gsRySMp3sRFmUU8123ccjhRLAEM.jpeg) ![PNG|230x500](upload://ArWnD5HEM3MTbC8G9aTAWmYaSUH.jpeg) 

I searched this forum for suggestions and tried to flash firmware again. Went through the same process and still had the cutout issues. Also read that, the DRV chips could be faulty. 

I contacted flipsky directly. After speaking to Xu at flipsky over email, she told me to reprogram and make sure to use default settings (100K ERPM). I used everything default, I did motor set up in FOC in VESC tool and did not change anything. The cutting out is still happening. This time the vesc tool defaulted to these settings after running detection in FOC mode:

Motor Amps max: 49.69a

Motor Amps min: -49.69a

Battery amp max: 130a

Battery amp min: -60a

Max ERPM: 100,000

Same exact problem. FYI, I also tried it in BLDC mode with now success. They are now just asking me to show a video of how I set it up. To me, that will get me nowhere, but I may just do that just to give them something. 

Any help would be greatly appreciated!

Here are the logs from the default vesc tool settings as mentioned above.
I’ve highlighted the rows where the cut outs happened. starting at 320t ish row then another around the 1100th row. You can see the motor current goes up to 70a.

Please visit google drive link here --> https://drive.google.com/open?id=1dKBvWBK3zJavOXHx3jUHM38AnxXv10Eq
```

---
## \#2 Posted by: trampa Posted at: 2019-10-25T18:47:55.702Z Reads: 149

```
Hi @levan634, sorry to hear about your issues. Please do not refer to the hardware a VESC 6.6. 
VESC is the original hardware. The FSESC is third party hardware. 

If you get these fault codes there is probably an issue with the hardware. These faults should not pop up if the ESC or electrical system is healthy.
```

---
## \#3 Posted by: levan634 Posted at: 2019-10-25T19:02:09.301Z Reads: 147

```
Noted and edited. My apologies!

Unrelated, but I have a trampa wand and BT module on the way from you guys. Can't wait. Might be picking up two VESC 6s from you as well due to this issue with my FSESC 6.6
```

---
## \#4 Posted by: BillGordon Posted at: 2019-10-26T00:50:22.503Z Reads: 139

```
PM sent your way.
```

---
## \#5 Posted by: mmaner Posted at: 2019-10-26T02:31:25.561Z Reads: 138

```
[quote="trampa, post:2, topic:103285"]
Please do not refer to the hardware a VESC 6.6. VESC is the original hardware. The FSESC is third party hardware.
[/quote]

He's an end user, not a manufacturer. He can call it what he wants. Ease up please.
```

---
## \#6 Posted by: trampa Posted at: 2019-10-26T08:02:06.392Z Reads: 134

```
No worries. The HW seams to be damaged, they should send you a replacement.
```

---
## \#7 Posted by: levan634 Posted at: 2019-10-26T18:27:50.598Z Reads: 122

```
thanks I have also posted in that forum.
```

---
## \#8 Posted by: BillGordon Posted at: 2019-10-26T18:35:38.844Z Reads: 120

```
Yup, I see you now. Talk to you there.
```

---
## \#9 Posted by: levan634 Posted at: 2019-10-26T19:14:38.130Z Reads: 115

```
I have uploaded my logs from the run. I’ve highlighted the rows where the cut outs happened. starting at 320t ish row then another around the 1100th row. You can see the motor current goes up to 70a.

Please visit google drive link here --> https://drive.google.com/open?id=1dKBvWBK3zJavOXHx3jUHM38AnxXv10Eq
```

---
## \#11 Posted by: Soflo Posted at: 2019-11-13T16:39:02.717Z Reads: 87

```
Flipsky are shit. Do a charge back and buy something else
```

---
## \#12 Posted by: levan634 Posted at: 2019-11-13T16:56:32.436Z Reads: 86

```
Thank you, Flipsky sent me a replacement non plus version. Waiting for it to arrive.
```

---
## \#13 Posted by: levan634 Posted at: 2019-11-13T16:58:54.789Z Reads: 87

```
Before I pass judgement on Flipsky as I whole, I will see how the replacement performs. I may have just gotten a bum unit. It happens. I am however, impressed with their response time and effort to remedy the issue.
```

---
## \#14 Posted by: Soflo Posted at: 2019-11-13T20:55:11.448Z Reads: 83

```
Im glad you are impressed.  I am not.  Let me know if you actually get the replacement.
```

---
## \#15 Posted by: flipskytech01 Posted at: 2019-11-14T08:17:32.196Z Reads: 82

```
@Soflo Please send the e-mail to our after sales service e-mail: flipsky-service@outlook.com if you have any question. It's appreicated you can send any video to be clearer. Thanks
```

---
## \#16 Posted by: levan634 Posted at: 2019-11-27T15:03:43.402Z Reads: 74

```
Forgot to post but I got a replacement two weeks ago. It only took a week and a half to receive the replacement. I have yet to test as there is 4 inches of snow outside.

![IMG_5755|375x500](upload://cfy629c5CmsooA1wwr9yyrrcTMW.jpeg)
```

---
## \#17 Posted by: Soflo Posted at: 2019-11-27T17:13:36.494Z Reads: 69

```
Waiting for mine to be shipped back after repair.  Beeb tying to get them to replace it with (2) singles. They want me to pay $150 more.  No thanks,  I'll put that money towards something reliable
```

---
## \#18 Posted by: flipskytech01 Posted at: 2019-12-03T07:56:18.312Z Reads: 64

```
We have contacted and sent over 20 e-mails to you for your aftersales service. As mentioned before, regarding the long logistics lead time for return from your place to our company, it's out of our control but your choice of the forwarder. We arranged the repairment since the same day afternoon. Also, we have told you, it's firmware blocked due to the new firmware upgrade without any issue of the hardware, reflash the firmware via ST-Link, then workable. While, you mentioned to change the new two single fsesc6.6 based on double 11 promotion prices after the repairment. I think this is really dufficult to accept for most of companies and not the rules of RMA return. Asking to replace another products after the repairment and on the basis of promotion price. Anyway, we have tried our best
```

---
## \#19 Posted by: Soflo Posted at: 2019-12-03T18:42:18.223Z Reads: 65

```
I don't trust your product! Your software is corrupt,  there's no reason your software should lock up a controller and need to be sent back to China to be unlocked.  This is unacceptable. why should I put my life on the line for your profit.  I an not a beta tester, but it seems like you think I am. I paid for a complete,  finished, working product. You did not supply that.  You supplied me with an unreliable piece of junk with corrupted software. You know you have a problem with your dual esc and won't admit it.  You are trying to push a faulty product on the consumer in the hopes that we will simply give up on the warranty process because you make it almost impossible.  I don't know what else to tell you,  your dual esc has bugs that need to be worked out,  not at my expense. For the money and time I have wasted on your failure of a product,  I could have bought a name brand VESC that is reliable. I am growing very tired of this back and forth with you concerning a known problem with your product. Im also not very happy that you require your customers to lie to China post about the value of your broken VESC.  Maybe I should bring this up to them?  im tied of being taken advantage of by your company.
```

---
## \#20 Posted by: levan634 Posted at: 2019-12-03T20:28:00.048Z Reads: 63

```
That is unfortunate that they are giving you the run-around. I def know how frustrating that can be. I do agree that having them send it back with low value so they don't take a hit with customs. A bit unethical in my opinion. 

I have yet to test the replacement I received from them as there is a foot of snow outside right now. I have a maker X dual I am running that I need to put through the paces too. As a back up plan, I am going to pick up the Torque Boards VESC 6 that they will soon have in production. As a last resort, I will pick up a Unity or actual Trampa vedder units.

Anyways, good luck with everything mate.
```

---
## \#21 Posted by: gee Posted at: 2019-12-03T21:51:59.156Z Reads: 61

```
You for sure burn the drv chip. I have the same problem. I wonder if they gonna send me another one. Use Xmatic too.
```

---
## \#22 Posted by: Soflo Posted at: 2019-12-04T01:20:32.891Z Reads: 62

```
@gee actually no my drv chip is fine.  The flipshit factory received my bad 6.6 mini and said it was a corrupted software problem.  They used an st link to reprogram it, said its working now.
```

---
## \#23 Posted by: AlanZhou Posted at: 2019-12-04T01:52:39.641Z Reads: 63

```
[quote="Soflo, post:19, topic:103285"]
Your software is corrupt, there’s no reason your software should lock up a controller and need to be sent back to China to be unlocked
[/quote]

did you update the firmware via the vesc tool then it got bricked?
```

---
## \#24 Posted by: Haze-Gray Posted at: 2019-12-05T13:39:59.961Z Reads: 56

```
saw the warning on this when flashing my 2nd vesc. been having odd issues with my 2nd dual 6.6 mini 1st was perfect but 2nd wont run wizards and keeps reporting firmware mismatch across the can bus but if you move usb cable and connect version shows to be identical. work around was to manually configure and it is working but clearly a glitch in there somewhere... Anyone got the skinny on this yet or is it still evolving?
```

---
## \#25 Posted by: Pantata Posted at: 2019-12-05T20:37:18.172Z Reads: 54

```
And you wonder why I and many others don't trust your products. Millions versions, all with problems. And then you mention BTW latest fw is not stable enough and might reverse at high speed... Jesus christ, I use it as a vehicle, ride among heavy traffic up to 65 km/h... lol... Thank God for Trampa.
```

---
## \#26 Posted by: flipskytech01 Posted at: 2019-12-06T06:00:59.193Z Reads: 52

```
not in high speed reverse due to the strengthen of braking. Normally no big influence
```

---
## \#27 Posted by: Pantata Posted at: 2019-12-06T09:03:46.104Z Reads: 49

```
YOu specifically say "fw might not be stable enough" How can you push a fw that is not stable enough? Do you understand what happens when a ESC cuts out, off or the system does anything else but what I want it to do? Most likely I will end flying head first and it's just a matter of luck whether it's the road I am landing or If I will hit a pole and smash my skull and die... Maybe think about that, this is not ice cream you are selling... You will cause deaths.. just sayin...
```

---
## \#28 Posted by: Haze-Gray Posted at: 2019-12-06T14:06:55.719Z Reads: 46

```
I am certainly not trying to defend or insult FLIPSKY. Like most i come here for knowledge and experience and so far they have certainly tried to help me so no complaints there. In all fairness, look at the early cars, COMPLETE DEATH TRAPS!!! took a long time for tech to catch up. take lights for instance, as a safety feature, should have been there all along especially brake lights. Unfortunately it has always been up to the consumer to verify manufacturer claims about products. look at all the defective airbags killing people in cars today... This is just 1 of the many reasons i am grateful for this site. so much knowledge available that manufacturers would kill or die for and us lowly end users can learn from each other. Much appreciated!
```

---
## \#29 Posted by: Pantata Posted at: 2019-12-06T18:44:19.452Z Reads: 47

```
If original VESC firmware developed by B. Vedder was used as it is on all regular VESC type ESC 
units, then there would not be any problems (presuming the hardware is quality and up to specs) Once you decide to go your own way you have to deal with the consequences. It took Vedder years of developing. Great example was Enertion and their buggy software. even after a year they didn't manage to fix many of the problems. At the beginning there were cut outs, I eneded up crashing because of that... It's money over safety and I don't take that. Not sure why no one is making quality vesc type ESCs. The only option nowadays is the original Trampa VESC and maybe unity with a questionmark as it is fully stable now, but Enertion seems to be in the ditch so who knows whether you even get a warranty. They don't answer to emails...  Similar story with motors. People would save so much money in the long run If they bought the expensive Trampa VESCs and motors. Not mentioning the safety aspect of having the best quality stuff.
```

---
## \#30 Posted by: Soflo Posted at: 2019-12-08T03:36:54.162Z Reads: 44

```
Hopefully the new neobox will solve this
```

---
## \#31 Posted by: Haze-Gray Posted at: 2019-12-09T14:56:21.570Z Reads: 39

```
6th ride on new board still working out the bugs. Relocated the radio to a plastic box and had no apparent interference issues. I did have a new issue, after about 10 minutes of riding, my speed would surge and pulse with throttle in same spot. No brakes applied but sudden burst of speed is scary!!! My top speed would fall off from 35 to 22 to 17 max until i stopped for a bit. i am pretty sure this is heat related as i was able to recreate issue by stopping and letting board cool the ride some more and about 10 minutes in it started again for at least 5 cycles. anyone run into this before? Still dont trust this VESC config...it lies about firmware version over the bus so no clue what that is about. My 1st 6.6 plus vesc had none of these issues so i am a bit baffled. flipsy 6374 190 kva motors  so should all work well together or so i thought LOL
```

---
## \#32 Posted by: Soflo Posted at: 2019-12-09T17:23:17.870Z Reads: 38

```
Sounds like thermal throttling.  Do you have a way to record your stats?  Metr? That will tell you if you have a motor that's getting warm or an esc. I had the same problem with 6374 sk3 190kv motors on the 6.6 dual mini.  I ended up switching to 6380s 170kv.
```

---
## \#33 Posted by: Haze-Gray Posted at: 2019-12-09T18:08:36.382Z Reads: 38

```
Thanks for the info! yes same vesc 6.6 plus recently bumped up from 100 amp to 120 amp in esc so hoping that is just too much? Also possible i over tightened a belt. Do you think that could be causing the heat issue as well? still a new board so got some bugs and i tend to mess with things too much causing other issues LOL but getting closer
```

---
## \#34 Posted by: Haze-Gray Posted at: 2019-12-09T18:33:57.461Z Reads: 38

```
forgot to add, did not see this issue on 1st few rides so probably something i changed...
```

---
## \#35 Posted by: Soflo Posted at: 2019-12-09T19:34:01.458Z Reads: 37

```
Overnighted belt will cause big issues. What battery are you running?  Also 120a Is waay too high for that motor.  It's only rated at 85a.
```

---
## \#36 Posted by: Haze-Gray Posted at: 2019-12-09T19:51:56.337Z Reads: 35

```
yeah, my bad braking was causing belts to slip so i think i got carried away... will fix tonight. batteries are huge 6s 28 amp hour 25 c X 2. so 12s 1 p. on dual vesc i think amps it total so only 60 amp max per side right? found new vesc tool out now so going to try wizard again.great advice, spot on dude i didnt have to call psycic hotline or anything LOL thanks much @Soflo ! I am an old electronics engineer but new to vesc so still learning...
```

---
## \#37 Posted by: Haze-Gray Posted at: 2019-12-09T21:08:47.579Z Reads: 35

```
this just in, NEW VESC TOOL 1.26 and new firmware is out. I downloaded and updated firmware on both sides of esc. I was even able to run the motor wizard. Power cycle board and everything appears right again. re-tensioning belts for evening test drive now but think i am good to go. fingers crossed! @flipskytech01 you might want to remember this as it appears to have resolved my mystery comm issue where the 2 sides of VESC report firmware mismatch even when identical.
```

---
## \#38 Posted by: levan634 Posted at: 2019-12-09T21:28:09.479Z Reads: 36

```
nice, looking forward to what your findings are.
```

---
## \#39 Posted by: Haze-Gray Posted at: 2019-12-09T23:17:15.873Z Reads: 35

```
test ride complete, all good now!!! Still have to do a longer distance check but short ride showed plenty of speed and power cruising at 25 mph hit full throttle makes the board leap smoothly forward as it should. Top speed is 35ish so yeah :slight_smile:  no more surging while cruising at speed so that part had to be heat related. Spot on there @Soflo, thanks again for all your help. Big rookie mistake was over tightening belts. Lesson learned...
```

---
## \#40 Posted by: Soflo Posted at: 2019-12-10T00:04:35.916Z Reads: 35

```
Glad it was an easy fix!!!
```

---

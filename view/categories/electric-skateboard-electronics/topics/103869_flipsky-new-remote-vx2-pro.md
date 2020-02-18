# Flipsky New Remote VX2 PRO

### Replies: 50 Views: 1184

## \#1 Posted by: sweet Posted at: 2019-11-14T02:08:03.426Z Reads: 226

```
Want to get a new remote recently. I heard flipsky VX2 PRO came out. Does anyone used it?How do you feel? What's the difference between VX2 and PRO?
```

---
## \#2 Posted by: flipskytech01 Posted at: 2019-11-14T08:27:43.573Z Reads: 216

```
Hello. The pro version is color screen display, MPH/KPH exchangable, vesc&Unity compatible. We do the pro version per customers needs and make some modifications for the UART signal communicate way to be compatible with the Unity.
The VX2 is the black&white screen. MPH or KPH setting and flashed before the shipment, not exchangable via the remote directly, suitable for vesc only.
Both VX2 and Pro version support UART mode only, not PPM, as it's screen and needs the UART mode to read the data via chip directly instead of the PPM via receiver first and the gain from the receiver.
```

---
## \#3 Posted by: Stan8 Posted at: 2019-11-14T11:35:55.051Z Reads: 209

```
Would there be a user upgradable firmware update? It would be nice if you guys would have software upgrades on the remote, like how Trampa does it with the wand, so you can add more features/fix bugs.
```

---
## \#4 Posted by: flipskytech01 Posted at: 2019-11-15T03:30:51.668Z Reads: 195

```
Sorry. The software is flashed in our factory before the shipment. Update by users is not available.
```

---
## \#5 Posted by: chopper698 Posted at: 2019-11-17T17:45:33.427Z Reads: 185

```
I have the VX2 and using it with the dual 6.6 as well as programming it through the vesc app through blue tooth. I cant get the mph, amp and board battery level to work. And the motors only run in high without any sort of transition when you rotate the wheel, takes right off. I tried putting it in uart but it keeps going back to ppm and uart. What am I doing wrong?
```

---
## \#6 Posted by: flipskytech01 Posted at: 2019-11-19T09:13:53.490Z Reads: 170

```
Hello. The screen remote VX2 supports UART mode only as it has to read data via the esc board directly. If choose PPM mode, then the screen useless. Regarding run in high, do you mean cannot exchange the speed between H, M, L or it runs at the same speed? Do you test in no load? If in no load, the speed keeps the same. As you know the vesc is current control, if no load, no friction etc., same current output, same speed. When doing parameters setup, please make sure all data correct, or the speed will be incorrect, especially the motor pole pairs q'ty. For example, pole pair 14, then 7 pairs; pole pair 20, 10 pairs.
```

---
## \#7 Posted by: moon Posted at: 2019-11-19T09:58:07.241Z Reads: 160

```
Oh Hello..
```

---
## \#8 Posted by: dareno Posted at: 2019-11-19T09:58:24.373Z Reads: 159

```
Hey sweet.   Its sweet that you are asking these sweet questions because sweet jesus we need some sweet answers.
```

---
## \#9 Posted by: Pura-Vida Posted at: 2019-11-19T10:38:18.597Z Reads: 154

```
WD40 is not for drinking nor cocktail :smile:
```

---
## \#10 Posted by: chopper698 Posted at: 2019-11-19T14:50:00.328Z Reads: 156

```
I have 14 for my motor poles what do you mean by 7?
```

---
## \#11 Posted by: Crashmaster Posted at: 2019-11-19T18:12:02.053Z Reads: 144

```
Mmmm. WD40. Tasty.![0411191232_Film1|666x500](upload://A2sEQY9sjt5d2uUONAw9HXDjrrx.jpeg)
```

---
## \#12 Posted by: Haze-Gray Posted at: 2019-11-19T19:11:07.837Z Reads: 140

```
just got my remote working. Anyone know how to tweek teh power band yet? i see l m and h but no apparent difference in speed...way too fast at 12s with 6374 twin 190 kv motors might have a gearing issue to overcome...
```

---
## \#13 Posted by: bigben Posted at: 2019-11-19T20:20:17.807Z Reads: 132

```
You should be able to alter the throttle curve in the nunchuck app on the tool and it will affect the curve on your vx2.
```

---
## \#15 Posted by: flipskytech01 Posted at: 2019-11-20T01:53:40.035Z Reads: 129

```
Yeah. 7 pairs please. If 14, the speed will be incorrect
```

---
## \#16 Posted by: chopper698 Posted at: 2019-11-20T02:12:26.457Z Reads: 124

```
So do I set the 7 on the remote because on the vesc app for pole settings there is no 7.
```

---
## \#17 Posted by: Haze-Gray Posted at: 2019-11-20T14:10:59.249Z Reads: 124

```
Thanks @bigben! much appreciated and will give that a try tonight. about 3 grand in parts on this build so test drive time is very exciting!

Hi @flipskytech01 nice to meet you and thanks for jumping in. was wondering the same thing vesc and remote says 14 poles and max sped was only 19 MPH at full rpm on 6374 190k flipsky motors and a 12s \28 AH battery pack, 66\14 gearing 200 mm tires so no way that could be right...  will pole change from 14 to 7 resolve speed on remote and should i change in vesc as well?
```

---
## \#18 Posted by: Haze-Gray Posted at: 2019-11-20T14:20:42.292Z Reads: 123

```
might have to start a separate thread but need new name for her, cant keep calling her board 4... Ideas?![board%204|419x354](upload://A6gBsBGQKuzFlsrrOTaEYR3cys.jpeg)
```

---
## \#19 Posted by: Haze-Gray Posted at: 2019-11-20T14:31:39.913Z Reads: 119

```
Thanks for the tip, appears to have resolved  remote speed.
```

---
## \#20 Posted by: flipskytech01 Posted at: 2019-11-21T02:53:16.617Z Reads: 113

```
Glad to hear this. Some customers meet with the same problem as you. smiley:
```

---
## \#21 Posted by: Haze-Gray Posted at: 2019-11-21T17:09:04.745Z Reads: 105

```
i was able to get things working but not exactly right. very odd ,vesc tool connected to #1 would often report #2 firmware as wrong version then fail to configure input device when wizard was run. It is not the wrong version, both sides firmware were successfully updated and do match so i believe there is a glitch somewhere as i ran into it several times in a row. Hopefully someone will make a configuring video ... near as i can tell mine is working just not able to adjust the throttle range as much as i would like. test drive this weekend so cant wait! Thanks again for your assistance, much appreciated.
```

---
## \#22 Posted by: flipskytech01 Posted at: 2019-11-22T05:40:55.550Z Reads: 100

```
Doing firmware upgrade successfully doesn't mean  success in vesc tool. Sometimes, it means finish. Need to check the bottom of vesc tool to see if both are the same. If not the same, it will have the problem as yours. If the same, have you inserted in any remote receiver or bluetooth module during the parameters setup process. They may have effect. It's appreciated if you can provide the video to be clearer
```

---
## \#23 Posted by: Haze-Gray Posted at: 2019-11-22T17:00:44.399Z Reads: 91

```
will see what i can do on a video and thanks again for ht help but 1st test ride Saturday so don't want to mess with anything just yet LOL I did connect to each vesc separately and verify it is reporting the same version which is why i mentioned it, odd problem like it cant read version correctly across can bus sometimes. if you are willing to help, i will see what i can do about getting you some real solid data so you can figure out what i am doing wrong :slight_smile: anything else you would like to see, let me know.Thanks again!
```

---
## \#24 Posted by: mattsdominion Posted at: 2019-11-23T16:57:21.900Z Reads: 86

```
Ordered a new vx2pro remote and received it yesterday.  It's definitely nicer in construction than the VX2 non pro.  There was no receiver in the box, though.  Does anyone know if it's possible to pair the old receiver to the new remote or vice versa?  I'd like to use it while Flipsky customer support rectifies this situation.
```

---
## \#25 Posted by: mattsdominion Posted at: 2019-11-23T18:04:20.688Z Reads: 89

```
pairing is brain dead simple.  It's done entirely from the remote accessory button.  im operational for the time being.  Just missing my 2nd receiver so swapping it between two boards for the time being until my 2nd one arrives.
```

---
## \#26 Posted by: bigben Posted at: 2019-11-23T19:31:47.107Z Reads: 86

```
You can use the old receivers.
```

---
## \#28 Posted by: Haze-Gray Posted at: 2019-11-24T17:45:06.090Z Reads: 81

```
was this teh post about having 6 remotes? If so, Thanks dude!!! spot on for my issue i have a work around massive curve for throttle and break 85 \ 75 % roughly... Much appreciated!
```

---
## \#29 Posted by: flipskytech01 Posted at: 2019-11-25T06:53:15.193Z Reads: 75

```
The non-pro version receiver cannot be used for the pro version for different software programmes. Can you please double check and show the photos? We inserted the receiver into the receiver box and haven't met with this problem before. Please provide the photos to our after sales service e-mail: flipsky-service@outlook.com. We will do support. Thanks.
```

---
## \#30 Posted by: flipskytech01 Posted at: 2019-11-25T06:56:05.446Z Reads: 72

```
Can I know your firmware version? Please do the parameters setup as this. https://youtu.be/SaLwRQ503jk
```

---
## \#31 Posted by: Haze-Gray Posted at: 2019-11-25T21:26:57.596Z Reads: 68

```
on call tech for work this week but will have some free time the end of this week to dig deeper. Much appreciated!
```

---
## \#32 Posted by: flipskytech01 Posted at: 2019-11-26T09:40:55.078Z Reads: 67

```
Yes. Please change to be 7, 14 poles means 7 pairs
```

---
## \#33 Posted by: Haze-Gray Posted at: 2019-11-26T13:07:02.236Z Reads: 70

```
Hello again. I already did that on the remote. That was the 1st thing you helped me and 1 other person fix so thank you for that.If i understand correctly, in the vesc it is 14 poles and in the remote it is 7 pairs. so believe mine is already correct, right?  Speed was wrong until that was fixed. Now speed on remote appears to work. Only issue i have now is the throttle response is only about have the travel of the throttle switch. Again, someone posted they had 6 of these remotes and that is normal. Not complaining if that is the case, it is working correctly as near as i can tell now just not as much travel for the throttle as the switch. When i tested the remote it gave a range of movement of roughly 99.9 forward and 79.9 back. This range was maxed out in both directions BEFORE the switch gets anywhere near end stop position. When i set up the throttle, it is the same. I know the power curve i have is a little too aggressive so will be adjusting over the 4 day weekend but that will not change the travel of the throttle switch right? I am an old RC guy and EE so i think i understand what is happening here just not sure there is a fix for that, may be nature of the design unless you tell me different?
```

---
## \#34 Posted by: flipskytech01 Posted at: 2019-11-27T08:38:50.581Z Reads: 64

```
Hello. Anything I can do for you? Thanks.
```

---
## \#35 Posted by: flipskytech01 Posted at: 2019-11-27T09:01:33.688Z Reads: 60

```
Can you show the video to be clearer? The remote throttle is controlled via hall sensor and two springs pull and push. During the production process, any little tolerance value will result in the two sides difference. It has no effect on speed and other data display. Setting this as an example, the less 79.9 one will be more sensitive when pulling.
```

---
## \#36 Posted by: Haze-Gray Posted at: 2019-11-27T13:11:50.123Z Reads: 55

```
Good Morning and thanks again for sticking with this. Vacation starts tonight so will get on those videos as promised. This sounds exactly right. Only question i have is where is that setting located? I hope this is not the throttle curve I have been playing with.  I can't wait to get the throttle dialed in, everything else appears to be going well with the new board so this is the last tech hurdle to make it a truly sweet ride. Too bad, Thanksgiving is not a holiday on your side of the world but I wish you a happy 1 none the less. :)
```

---
## \#37 Posted by: flipskytech01 Posted at: 2019-11-28T09:49:06.772Z Reads: 55

```
Hello. Happy Thanksgiving. Yeah. The data you mentioned is the hall sensor ADC sample data, display not in the middle for some mechanical structure tolerance value in physical production. It doesn't have the effect on speed, battery and other data display. The hall sensor is located in the case. The throttle control via the spring pull&push nearby.
```

---
## \#38 Posted by: Haze-Gray Posted at: 2019-11-30T02:41:04.579Z Reads: 53

```
SIDE NOTE... after a successful 15 mile road trip yesterday, decided to try to ride dirt trails along power lines today. Both board and remote fully charged. Was cruising at about 15 mph when suddenly the board starts acting odd then applies full brake while i still have throttle in same spot. Near as i can tell, i picked up some serious interference from the power lines. Anyone else experience this? Any work arounds? as you can see my receiver![esc%20mount|375x500](upload://dG4m5OArqJu6zuHw2XmoENDZEpa.jpeg)  is mounted inside an aluminum box so that can't help... Should i drill a few holes in the top maybe? I ride goofy with remote in left hand so never more then a few feet from esc at most.
```

---
## \#39 Posted by: Haze-Gray Posted at: 2019-11-30T02:50:29.360Z Reads: 55

```
unable to do video sorry @flipskytech01. Here are some pics showing esc firm ware version from both sides of esc and error i get before wizards bomb. not that it matters i suppose as i get it working but maybe not as designed.... LOL also had gear wrong on motor. was 13 not 14 tooth as configured. i correctd this and adjusted throttle curve. looking forward to ride tomorrow.
![motor%20firmware|480x360](upload://upnnaHoPR3VYbWXc4sbh0rdulBQ.jpeg) 
![motor2%20firmware|480x360](upload://xET0TjDEDQsMMyhkjbeNyVhU6rt.jpeg) 
![error|480x360](upload://dqvoGNE1twkoLFz3yd08k165t7L.jpeg) 
![throttle%20curve%20new|480x360](upload://2HQIElmP2gHiFTExhkRJ9pQt2dz.jpeg) 


let me know if this helps cover your question. sorry no way to do video.
```

---
## \#40 Posted by: Haze-Gray Posted at: 2019-11-30T02:53:34.555Z Reads: 49

```
forgot to add, error occurs when connected to primary esc side and asking to read other sides firmware version. works fine if i move usb cable.
```

---
## \#41 Posted by: bigben Posted at: 2019-11-30T08:47:02.910Z Reads: 51

```
When you shut that box up, your receiver would be pushed onto the main power lead and the motor phase wires? This is normally best avoided. Try to situate your receiver elsewhere.
```

---
## \#42 Posted by: Haze-Gray Posted at: 2019-11-30T19:50:39.415Z Reads: 50

```
the esc is mounted upside down in the top of the case and there is a good 1 inch gap between for the wires to lay down and not touch esc but yes more or less. It has a long enough leash so could move it anywhere in box but am wondering if drilling some holes wold be a good idea for reception. esc in middle and motors on both sides so where to put it? Wish it had a external \remote antenna or something...
```

---
## \#43 Posted by: bigben Posted at: 2019-11-30T19:59:42.809Z Reads: 47

```
It could be electrical interference even if it’s not touching.
```

---
## \#44 Posted by: flipskytech01 Posted at: 2019-12-03T07:28:26.630Z Reads: 41

```
It's better to use some plastic enclosure. The metal material will influence and has signal interference, which will be easy to cause the remote response delay for accelarating or braking. It's dangerous
```

---
## \#45 Posted by: flipskytech01 Posted at: 2019-12-03T07:32:05.063Z Reads: 38

```
The screenshot is not clear enough. Sorry. Also, not sure if your way of doing parameters setup is correct or not. Please from the "Welcome&Wizards", do the motor foc setup from this instead of motor settings directly. You can also review via our blogs.
```

---
## \#46 Posted by: Haze-Gray Posted at: 2019-12-04T15:57:53.942Z Reads: 37

```
as you may recall, planned receiver had a real antenna wire which was supposed to extend outside the box. not fond of pcb antennas for just that reason but no worries. I live in Florida. The dew on the grass is enough to soak my board on morning rides. Guess i will have to change enclosure out soon.
```

---
## \#47 Posted by: Haze-Gray Posted at: 2019-12-04T16:07:44.608Z Reads: 37

```
I believe i mentioned  i cannot run the wizards because of the error i get about the firmware mismatch witch is not right .vesc firmware for both is 3.62, HW:60 53 00 37 00 06 50 4B 4D 52 32 30 20. working on video solution stand by for that :slight_smile:
```

---
## \#48 Posted by: flipskytech01 Posted at: 2019-12-05T08:18:40.153Z Reads: 35

```
Have you tried via the bluetooth module? Can it be successful?
```

---
## \#49 Posted by: sweet Posted at: 2019-12-05T09:30:20.423Z Reads: 36

```
Yes,thank you. I was lucky enough to get one VX2 PRO during the black Friday flash sale at your store, and I am looking forward to receive it. Actually, I had one VX2 remote with black and white screen not long ago, but considering the new function, I decided to purchase a new one. Hoping it will bring better riding experience to me!
```

---
## \#50 Posted by: Haze-Gray Posted at: 2019-12-05T13:16:49.270Z Reads: 37

```
Bluetooth? i will have to look into that as i am not familiar. I also think i have a solution for antenna. since transceiver is on separate card, going to relocate it outside the metal box in a small plastic box on top. That should resolve interference issue. Thanks again for the help!  Still working on video maybe this weekend if i am lucky. Like i said, got it configured and even managed to adjust throttle and brake curves with the help here so this is more of a pest than a problem as the 1st vesc i configured never had a problem like this and the wizards worked great.
```

---
## \#51 Posted by: Haze-Gray Posted at: 2019-12-09T18:19:34.911Z Reads: 29

```
remote leash wtf moment...:):grinning: Was riding with my buddy and had remote leash Velcroed to my wrist guard so it cant fall off and hit the ground  if i let it go or so i thought. We stopped to take a break and i let the remote dangle from strap.Next thing i know the remote is in 2 pieces on the ground and the leash is still attached to me. Apparently the case just snaps together which is fine but terrible design on leash connector can cause case to pop open when hanging from strap. Low tech fix is rubber band on handle to keep it from spreading apart. Again remote was dangling from leash under own weight and just popped open then hit the ground. bummer that my new remote is getting scuffed up already and not even from a combat roll...ugh should have been a hook shaped connector and not just a tab to hold leash inside so pressure on leash cant pop open case...![radio|480x360](upload://A8Arz4u9PvNekBxOXzT3xqkyZn4.jpeg)
```

---
## \#52 Posted by: Haze-Gray Posted at: 2019-12-09T18:28:50.248Z Reads: 26

```
can i get some more details on the bluetooth option you mentioned? would like to look into it.
```

---

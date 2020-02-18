# My Board is just too fast, some vesc advice please

### Replies: 36 Views: 2576

## \#1 Posted by: overclocker_kris Posted at: 2016-12-03T17:58:07.384Z Reads: 299

```
Hi guys, i have just finished making two awesome boards, one for me and one for my girlfriend, my one is dual drive with two 6355 motors and dual vesc my girlfriends one is single motor single vesc. her board rides like a dream but mine is just hard work. it has to much power it wont maintain a constant speed it just keeps pulling and pulling. it also has a little stutter when starting from a standstill. 

i have messed with some setting to try and fix the stutter but nothing seems to work. i have the vesc set to master and slave as per information found on this forum does anyone have any other ideas of what could be causing the stuttering? Also does anyone know if there is a setting a can change to make the board more controllable at a constant speed instead of just pulling and pulling? both boards are useing the same controler so i cant see that that could be anything to do with it. my pulleys are 16t 36t on 80mm wheels so i dont think that is the problem. 

and advice would be great. im now to the vesc so im still figuring out the settings.
```

---
## \#2 Posted by: JuniorPotato93 Posted at: 2016-12-03T18:06:50.956Z Reads: 295

```
Post a picture of your settings and also whats your kv and system voltage?
```

---
## \#3 Posted by: overclocker_kris Posted at: 2016-12-03T18:08:36.481Z Reads: 292

```
i will plug it in a take some pictures of the setting in a second. the kv is 190 and im running an 8s battery
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-12-03T18:10:31.186Z Reads: 288

```
Have a look at my modded firmware. I am pretty sure this will solve the problem
```

---
## \#5 Posted by: overclocker_kris Posted at: 2016-12-03T18:24:31.692Z Reads: 278

```
<img src="/uploads/db1493/original/3X/e/5/e5154283f09f08092fd8e0b3f483de0fca2b3a48.png" width="690" height="431"><img src="/uploads/db1493/original/3X/6/1/6187e443dcca452919b26e607fdc9b33d4ce6365.png" width="690" height="431"><img src="/uploads/db1493/original/3X/2/9/293b24e8ba0819602078ca7e5b4f4de71668463d.png" width="690" height="431"><img src="/uploads/db1493/original/3X/7/a/7ac232c2b4c43d8e81100a11fef20137471ba6d5.png" width="690" height="431"><img src="/uploads/db1493/original/3X/7/1/710a7b16a6d7c6ae82cbc996907076b9a9b32b5c.png" width="690" height="431"><img src="/uploads/db1493/original/3X/3/6/36cfb5eba3c1dd0139a17eb259d272130f9ec9ac.png" width="690" height="431"><img src="/uploads/db1493/original/3X/a/9/a977f108520cd0e03fdb663a5193d3c48899c8a5.png" width="690" height="431"><img src="/uploads/db1493/original/3X/e/6/e6becd1e700373314d6edf1f27396a7c1cf1bc1e.png" width="690" height="431">

the top 4 images are slave the bottom four are master
```

---
## \#6 Posted by: overclocker_kris Posted at: 2016-12-03T18:31:24.800Z Reads: 240

```
i just looked at it, it looks great but on only have a mac laptop and i think it is for windows right?
```

---
## \#7 Posted by: rpn314 Posted at: 2016-12-03T18:33:41.210Z Reads: 247

```
It is currently windows and Linux, but he's working on a mac version.

As for your settings, when the Mac one comes out I would definitely go for that, but in the mean time you could turn down your erpm limit and your battery current. And on an unrelated note, I would also set your low battery cuttoff higher than 8v.
```

---
## \#8 Posted by: overclocker_kris Posted at: 2016-12-03T18:35:47.692Z Reads: 247

```
i will have to keep a look out for that then. that looks really interesting, thanks for the info
```

---
## \#9 Posted by: overclocker_kris Posted at: 2016-12-03T18:37:28.184Z Reads: 246

```
<img src="/uploads/db1493/original/3X/5/f/5f5e323518efe544e23d7c9dba6acb93a1cff4c5.jpg" width="375" height="500">

just incase anyone wants a picture
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-12-03T19:16:48.066Z Reads: 233

```
So 2 things. First of all you should do a motor detection. Because you didn't do that for both motors. Second you should adjust the battery cutoffs. And third of all your board must drive like a monster.
Set the battery max to 30 on each VESC and try that first. If that is not enough then you can go higher. But 70 each is crazy. If you have a li-ion battery you might even damage it.,

Your master VESC should not send the status over can in the aplication general tab.
```

---
## \#11 Posted by: overclocker_kris Posted at: 2016-12-03T19:19:24.262Z Reads: 227

```
Ok great i will change those now, it has a 17ah battery so there are 6 18650 in parallel 8 series so it is just a monster, hopefully changing those setting will calm it down a bit.  i will change them now and let you know how it goes
```

---
## \#12 Posted by: NickTheDude Posted at: 2016-12-03T19:36:05.046Z Reads: 221

```
Yeah you should definitely set your voltage cutoffs. Cutoff start is the point that your VESC will go into safe mode, and cutoff end is when it will stop altogether. Cellphones and stuff usually cutoff at like 3.0V but my cutoff starts at 3.4V and ends at 3.2V.

Since you have a 8S pack yours should be around 3.4 * 8 = **27.2** and 3.2 * 8 = **25.6**

Also, If you're sensorless and are having trouble launching, you could try turning up the startup boost. It's under Motor Configuration > Advanced. I think mine is set to 0.40.
```

---
## \#13 Posted by: overclocker_kris Posted at: 2016-12-03T20:10:01.761Z Reads: 211

```
i made all of those changes and it is a completely differant board still mountains of power but it is controllable nd easy to keep a steady speed. i even set the cruise control and it just sat at a perfect speed. it would have never done that before. it just kept no going. Thanks so much for the help. 

i have made a complete build video series that i will upload over christmas. i made the battery, motor mounts, enclosure all myself so it might be of some interest. i will also do a build post for people that dont want to watch videos. 

thanks again for the help.
```

---
## \#14 Posted by: NickTheDude Posted at: 2016-12-03T20:12:15.994Z Reads: 206

```
No problem. I'll look forward to those videos, your boards look sweet!
```

---
## \#15 Posted by: Dedbny Posted at: 2016-12-03T20:32:25.207Z Reads: 199

```
Definitely post it up soon.  Alot of ppl are finalizing their builds over the break,  so could be helpful for others.
```

---
## \#16 Posted by: overclocker_kris Posted at: 2016-12-03T20:34:08.924Z Reads: 199

```
i will do my best, do you think people would like links to a youtube playlist of the build? i have got quite a bit of editing to do but i will get them up asap and do a full build post as well.
```

---
## \#17 Posted by: Dedbny Posted at: 2016-12-03T20:40:06.650Z Reads: 195

```
If youve got the time. Ive seen alot of vids.  They go from actual truck motor build then all of a sudden they are riding.  Be good if there was a more detailed one on vesc set up. Motor detection. How you just resolved ths issue you had.
```

---
## \#18 Posted by: SirDiff Posted at: 2016-12-04T00:07:35.890Z Reads: 177

```
This is the expression of "vesc power"
```

---
## \#19 Posted by: Eboosted Posted at: 2016-12-04T03:24:29.942Z Reads: 163

```
I can't wait to have my parts here and start fidling with the VESCs settings until I get to the point you are right now! 

Congratulations!
```

---
## \#20 Posted by: Namasaki Posted at: 2016-12-04T03:39:37.997Z Reads: 158

```
-20 for Batt Regen is probably too high. Unless I am mistaken, This means that you are recharging your batteries with 20a of current while braking.
```

---
## \#21 Posted by: NickTheDude Posted at: 2016-12-04T04:05:30.273Z Reads: 148

```
Yeah, I've heard that a safe regen is 1C of your pack. So if you had a 7500mAh pack than it'd be -7.5A
```

---
## \#22 Posted by: Eboosted Posted at: 2016-12-04T04:23:52.029Z Reads: 145

```
Where do you guys get this information from?
```

---
## \#23 Posted by: Jinra Posted at: 2016-12-04T04:45:30.700Z Reads: 146

```
cell datasheets. I use -16A for my 4P Samsung 25R pack since their max rated charge is 4A per cell.
```

---
## \#24 Posted by: overclocker_kris Posted at: 2016-12-04T09:09:55.911Z Reads: 138

```
the pack is 17.5 ah so it isnt to far off i dont think?
```

---
## \#25 Posted by: overclocker_kris Posted at: 2016-12-04T09:11:55.944Z Reads: 139

```
the board took me about two months of saving and collecting parts and many hours to make. i got on it any it was almost unusable. but now it is just awsome. the sun is out today so im going to go out on it. it is just so much fun.
```

---
## \#26 Posted by: saul Posted at: 2016-12-04T15:34:05.532Z Reads: 125

```
wow i'm surprised your vescs survived with 70A motor/batt!
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-12-04T16:02:24.848Z Reads: 128

```
Thats  because the shortly boosted him to max speed and then they don't need much amps anymore. Most people think at max speed you use max amps. 
For example with a street setup you need around 1000 watts power to do 50 km/h. That is around 28 amps in total for a 10S battery. So only 14 amps on each VESC. If max speed is only 40 then you need only 650 watts which is around 18 amps in total and 9 amps on each VESC. 
Uphill is another story and the acceleration to that speed as well. But once you reached that speed you don't need that much power anymore.
```

---
## \#28 Posted by: Eboosted Posted at: 2016-12-04T16:55:53.534Z Reads: 122

```
What formula do you use to calculate the amount of watts needed for a given speed and acceleration?
```

---
## \#29 Posted by: Ackmaniac Posted at: 2016-12-04T16:59:18.168Z Reads: 122

```
Just by testing 250 watts is good for around 25 km/h,
If you wnat to know the watts for the speed of 40 km/h you have to calculate
40/25 = 1,6
1,6 * 1,6 = 2,56   (<-exponetial because for double the speed you have 4 times the wind and rolling resistance)
250 watts * 2,56 = 640 watts
```

---
## \#30 Posted by: skiboyscuba Posted at: 2016-12-04T18:16:31.366Z Reads: 118

```
[quote="overclocker_kris, post:13, topic:14126, full:true"]
i made all of those changes and it is a completely differant board still mountains of power but it is controllable nd easy to keep a steady speed. i even set the cruise control and it just sat at a perfect speed. it would have never done that before. it just kept no going. Thanks so much for the help. 

i have made a complete build video series that i will upload over christmas. i made the battery, motor mounts, enclosure all myself so it might be of some interest. i will also do a build post for people that dont want to watch videos. 

thanks again for the help.
[/quote]
I would love to see the video. Let me know when you post.
```

---
## \#31 Posted by: overclocker_kris Posted at: 2016-12-04T19:48:19.006Z Reads: 112

```
thanks for the info but i believe, wind resistance is squared. so if you double your speed the wind resistance goes up by 4x but the amount of power required goes up by 8x, because the are covering twice the distance.
```

---
## \#32 Posted by: overclocker_kris Posted at: 2016-12-04T20:10:23.212Z Reads: 107

```
i will do, i have 8 videos in total i am working on, a complete build process in 6 parts, a shorter version more for inspiration  and test riding. i will post them up when they are done.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2016-12-04T20:12:34.682Z Reads: 110

```
I embarrassed myself again. You are right. i have to do some testruns again to figure out how many watts are needed. 250 watts is also good for nearly 30 km/h. 
So it would be 
50/30 = 1,6666666
1,6666 ³ = 4,629
4,629 * 250 = 1157 watts

Need to make some videos again to get the right values from life recordings before i throw out more stupid stuff. And maybe the VESC's current readings are not very reliable when it comes to max power output.
```

---
## \#34 Posted by: overclocker_kris Posted at: 2016-12-04T20:18:38.942Z Reads: 103

```
haha, nah its an easy mistake to make. 250w sounds about right to me but i do love seeing the number so id be interested in seeing your tests.
```

---
## \#35 Posted by: yaca Posted at: 2016-12-04T20:21:35.646Z Reads: 109

```
On your screenshots it looks like you didn't set your min and max pulsewith!?
```

---
## \#36 Posted by: overclocker_kris Posted at: 2016-12-24T12:01:43.284Z Reads: 88

```
http://www.electric-skateboard.builders/t/dual-motor-loaded-cantellated-tesseract-build-album-with-descriptions-plus-build-video-playlist-and-test-ride/15148

my build post is up and running as promised.
```

---

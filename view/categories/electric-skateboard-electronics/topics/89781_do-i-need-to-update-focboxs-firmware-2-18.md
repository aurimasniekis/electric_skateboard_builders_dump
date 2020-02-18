# Do I need to update FOCBOXs firmware 2.18?

### Replies: 30 Views: 337

## \#1 Posted by: vortek Posted at: 2019-04-08T09:19:22.293Z Reads: 110

```
Hi guys!!
I have everything connected to test. Did the first setup of my dual focboxes using BLDC tool and set them to FOC.

![IMG_3810|666x500](upload://3jN5wCk0qyZ6StYFiGBLY3oGHIh.jpeg) 

I Bought them 6 months ago so the firmware they have is 2.18. Should I update the firmware to be able to use VESC tool? I have seen so many versions I really don't know where to start... 

Thanks
```

---
## \#2 Posted by: High-roller Posted at: 2019-04-08T10:24:30.776Z Reads: 105

```
The short answer is you probably don't need to, but it wouldn't hurt. I recommend you use the vesc tool exclusively now, it has an update wizard to help you get the right firmware version. There's a few YouTube tutorials around on how to do this as well.
```

---
## \#3 Posted by: StefanMe Posted at: 2019-04-08T11:29:03.877Z Reads: 96

```
U ll lost your warenty if u upgrade. Ask @EnertionSupport .
```

---
## \#4 Posted by: pjotr47 Posted at: 2019-04-08T11:40:44.267Z Reads: 95

```
Haha lol... it is Enertion. Most off the time all those focbox’s don’t have any warranty. 

I also think it is punishable in Europe for not giving a warranty on a product after a software update
```

---
## \#5 Posted by: taz Posted at: 2019-04-08T12:02:59.268Z Reads: 82

```
I think they have bypassed all the European warranty laws by simply not selling in Europe.
If you buy from a retailer in EU then it is the retailer's responsibility to honor the warranty.
```

---
## \#6 Posted by: barajabali Posted at: 2019-04-08T12:46:28.208Z Reads: 76

```
You’re wrong. 

[quote="pjotr47, post:4, topic:89781"]
Most off the time all those focbox’s don’t have any warranty.
[/quote]


So wrong.

Anyhow, 2.18 is the latest focbox firmware
```

---
## \#7 Posted by: briman05 Posted at: 2019-04-08T12:50:18.392Z Reads: 74

```
If you are running Acks esc tool then you will have to update.  I actually like that better it was a lot easier to set up as there is a wizard for the setup.  For the bldc tool on enertions website I think it can only run on 2.18 as the most current firmware.
```

---
## \#8 Posted by: taz Posted at: 2019-04-08T12:54:54.176Z Reads: 72

```
Is there a reason for that?
I truly believe that the  “temperature acceleration decrease” feature implemented in later vesc fw revisions is an important safety feature.

I was left without brakes after a steep hill one too many times to not upgrade the fw.
```

---
## \#9 Posted by: pjotr47 Posted at: 2019-04-08T12:58:24.146Z Reads: 71

```
@taz I know. That is the easiest solution for them. 

 
@barajabali I know: Enertion give “ * 60 Days for self-installed applications” warranty. But most off the high quality motor have 5.5mm bullets. So you must use a adapter or change the vesc bullets and lose warranty. 

But I was more talking about the focbox’s what are sold here on the forum. I formulated it incorrectly
```

---
## \#10 Posted by: barajabali Posted at: 2019-04-08T14:09:11.560Z Reads: 63

```
Im not sure... Likely some open source litigation or something..
```

---
## \#11 Posted by: CarlCollins Posted at: 2019-04-08T14:17:31.162Z Reads: 61

```
Looks like there are many wrong perspectives about FOCBOX (Original) In terms of warranty on the forum.
FOCBOX (by default) comes with 60 days warranty covering only manufacturing defects.
But If you purchased it with a platinum warranty then there will be 1-year support for it.

@pjotr47 That's true it's punishable in EU but only if there is a software update. FOCBOX's default firmware is 2.18 and also it's the latest one.
Please don't confuse Unity with FOCBOX :wink: because Unity has software updates. 
@taz the temperature thing is implemented well in Unity (not in default FOCBOX).

@vortek
So, here is the answer to your question
If you have the warranty still available on your FOCBOXes then I recommend you to stick with 2.18 but if you don't have any warranty on it then go for the latest firmware available on the forum.
```

---
## \#12 Posted by: briman05 Posted at: 2019-04-08T14:25:44.786Z Reads: 61

```
He stated that he bought it 6 months ago, I'm guessing the black friday specials.  This unit would no longer have a warranty correct?
```

---
## \#13 Posted by: MrDGOrman Posted at: 2019-04-08T14:55:26.240Z Reads: 58

```
Yes because as @CarlCollins said the FOCBOX comes with a 60 day warranty as standard. After that point, do what you like with it. If you purchased the year long warranty then don't play with it. Set it up, use it, done.

That's what I see from it anyways!
```

---
## \#14 Posted by: CarlCollins Posted at: 2019-04-08T15:12:01.168Z Reads: 55

```
@briman05
As @MrDGOrman explained, I am indicating same thing
```

---
## \#15 Posted by: vortek Posted at: 2019-04-10T20:30:10.374Z Reads: 39

```
Hi there,

So this is what happens when I connect to the vesc tool:
![Screeshot%202019-04-10|690x397](upload://64I8rjEgci6gDM6CsMrwsoQR6p3.png)
```

---
## \#16 Posted by: briman05 Posted at: 2019-04-10T20:39:25.535Z Reads: 39

```
for the vesc tool it is tool old of firmware and you would have to update it as for the bldc tool it is the most current.  The bldc tool is outdated compared to the vesc tool or acks esc tool
```

---
## \#17 Posted by: vortek Posted at: 2019-04-10T20:39:43.963Z Reads: 37

```
I don't have warranty anymore.
Which firmware do you advise? I have the MetrPro bluetooth module so was hoping to use the Metr App.![IMG_5CBA45EE924F-1|230x500](upload://bAPflsKaEhnnIdS3RwdUiGP9NUp.jpeg)
```

---
## \#18 Posted by: trampa Posted at: 2019-04-10T20:42:58.535Z Reads: 35

```
Bldc tool should not be used any longer, due to safety issues and no support. If you are concerned about warranty, remember that you can drop on FW 2.18 at any time you like. No one can see that you used later FW versions before. The FW tab in VESC-Tool allows to upload any FW you like.
```

---
## \#19 Posted by: Bjork3n Posted at: 2019-04-10T20:44:00.551Z Reads: 35

```
I use ackmaniac fw 3.102. Works perfectly with metr pro 👍
```

---
## \#20 Posted by: briman05 Posted at: 2019-04-10T20:45:45.410Z Reads: 35

```
You would want the firmware that is for hw_410, hw_411 and hw_412
```

---
## \#21 Posted by: vortek Posted at: 2019-04-10T20:49:23.333Z Reads: 33

```
Thanks going to try it now. And where do I download it?

![52|690x394](upload://gCdqqmCxrmc6SFyh6N2z3VXDxCv.png)
```

---
## \#22 Posted by: briman05 Posted at: 2019-04-10T20:52:37.019Z Reads: 32

```
do the default.bin
```

---
## \#23 Posted by: mmaner Posted at: 2019-04-10T20:53:44.900Z Reads: 35

```
[quote="trampa, post:18, topic:89781"]
No one can see that you used later FW versions before.
[/quote]

That's a bit dishonest?
```

---
## \#24 Posted by: vortek Posted at: 2019-04-10T21:02:43.796Z Reads: 35

```
Done. Disconnected both focboxes, updated 1, update 2 and now both are connected via canbus. The remote (nano-x) does not respond now. Could you point me to a "new configuration for rookies" please? :) 

![15|690x420](upload://8YFpaaHjSDBUusF5zPEPij6cEn.jpeg)
```

---
## \#25 Posted by: SeanHacker Posted at: 2019-04-10T21:04:35.662Z Reads: 33

```
Just go through the "Welcome & Wizards" tab of the tool. It will walk you through everything.
```

---
## \#26 Posted by: High-roller Posted at: 2019-04-10T21:33:04.681Z Reads: 27

```
If you're unsure, this tutorial should explain everything. 
https://youtu.be/v1glLDO-EjA
```

---
## \#27 Posted by: vortek Posted at: 2019-04-10T21:34:05.881Z Reads: 27

```
Great just did it!
Now I am having trouble with the values to configure the Enertion Nano-X. Where do I get the numbers?
```

---
## \#28 Posted by: SeanHacker Posted at: 2019-04-10T21:38:14.241Z Reads: 26

```
Did you use the wizard to setup the input (remote) yet? You will need to make sure to turn on RT App in order to see the mapping. Then continue with the remote setup. 

![Screenshot%20from%202019-04-10%2014-36-13|46x465](upload://t6NL8KsaLg51HLzsaJUOapzfs7V.png)
```

---
## \#29 Posted by: vortek Posted at: 2019-04-10T21:50:07.827Z Reads: 25

```
Great everything working :slight_smile:
Thanks very much.

Now, is there a way to define a curve for acceleration and break? For faster acceleration and smooth breaking for instance...
```

---
## \#30 Posted by: SeanHacker Posted at: 2019-04-10T23:10:51.820Z Reads: 24

```
Yep.

![Screenshot%20from%202019-04-10%2016-09-52|690x449](upload://isbybtqYPykpbF7YLj07HS6MIlH.png)
```

---

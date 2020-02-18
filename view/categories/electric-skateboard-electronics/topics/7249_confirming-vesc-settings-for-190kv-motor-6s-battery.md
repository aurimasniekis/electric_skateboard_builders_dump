# Confirming VESC Settings for 190kv Motor/6S Battery

### Replies: 14 Views: 5882

## \#1 Posted by: paul775 Posted at: 2016-08-07T04:23:26.612Z Reads: 473

```
Just received my VESC 4.12!

<img src="/uploads/db1493/original/2X/4/4c9dd50352cbf60cabbef6d427576b0d93c2ea5e.png" width="180" height="300">

Before I run the program, I would like confirm that my configuration is correct. Please confirm these settings so I can stay away from fried DRV chips and shorts.

From YouTube videos, I picked these **Current Limits**. I believe these can be tweaked since I have seen different numbers with everyone’s setup. If someone can point me out a thread that I can follow to calculate the Current Limits that would be cool!

For the **Voltage Limits**, I believe they are correct by following the Voltage Cells chart using my 6S setup.

<img src="/uploads/db1493/original/2X/7/7ce141821391f0a8609018188a64b105f817de68.png" width="690" height="341">

<img src="/uploads/db1493/original/2X/9/9bed76d81f6dbdd45061db3c7c98fe82dbdecd26.png" width="586" height="196">
```

---
## \#2 Posted by: Namasaki Posted at: 2016-08-07T04:36:13.764Z Reads: 447

```
What is the safe charge rate of your battery.
You need to set the Batt min (regen) accordingly
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-07T04:38:40.798Z Reads: 465

```
Don't set your voltage max to 25.2. You'll probably trigger an overvolt error when braking at near max battery. Also you may want to set your cutoff start a little lower due to voltage sag. I set mine at 3.3v per cell and end at 3.2v per cell.

Your motor current parameters are a bit low, but I'm sure you'll realize this when riding and adjust accordingly.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-08-07T04:42:01.183Z Reads: 458

```
There was reported a glitch in the latest bldc tool that can fry the drv chip.
http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
http://www.electric-skateboard.builders/t/faulty-v2-17-2-18-bldc-tool-win-osx/4213
http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
http://www.electric-skateboard.builders/t/vesc-faq-easy-vesc-configuration-in-windows-mac-for-noob/2963
```

---
## \#5 Posted by: paul775 Posted at: 2016-08-07T22:31:48.018Z Reads: 368

```
**Voltage Limits**

[quote="Jinra, post:3, topic:7249"]
Don't set your voltage max to 25.2.
[/quote]

Okay I read this thread: 
[VESC FAQ | Limit output voltage](http://www.electric-skateboard.builders/t/vesc-faq-limit-output-voltage-according-to-motor-maximum-specs/683/10) and adjusted my Voltage Limits from that.

Min: 8V
**Max: 50V**
Battery Cutoff Start: 21V (I can go less but I want to be safe for now)
Battery Cutoff End: 19.8V 

Still wondering about the Maximum Input Voltage. That user said to leave it at 50V but that would be at 10S right? For 6S I should leave it around 32V I believe?

---
**Current Limits:** 

[quote="Namasaki, post:4, topic:7249"]
There was reported a glitch
[/quote]

Thanks I fixed that. It is at 0.04 now.

Still confused on the Current Limits. Here is the battery specs, 2 of them in series.
Is my Safe Charge Rate the same as my Max Charge Rate, which is 2C?

<img src="/uploads/db1493/original/2X/2/286f46783f510a9ed209799a0134ecaf37232c2b.PNG" width="259" height="346">
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-07T22:35:37.629Z Reads: 311

```
There's not much need to change it. I leave mine at the default 57v. You're running 6s so you shouldn't overvolt, and leaving it higher will give you wiggle room for regen braking voltage spikes. 

Just be aware that if you start getting sluggish response/speed it may be because your battery cut off is too high. You may have capacity left, but voltage sag will cause your cut off to start.

2C (10 amps) for battery regen would be fine
```

---
## \#7 Posted by: makevoid Posted at: 2016-08-08T05:50:18.665Z Reads: 289

```
30 A as motor max seems a bit too low... Which motor do you have? I would set it to 40 and maybe go up a bit? But if are light and/or you feel you got enough acceleration/speed then 30 would work too... Otherwise increase it, I guess most people have it around 60? Also I guess the amp values are proportional to the voltage so a 30A motor max on 12S should be a 60A at 6S am I right?
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-08T05:52:40.171Z Reads: 279

```
I wouldn't say it works out exactly like that. You can set it to 40-60 for most applications and the VESC will only draw the current it needs anyway.
```

---
## \#9 Posted by: paul775 Posted at: 2016-08-08T06:07:08.762Z Reads: 273

```
[quote="makevoid, post:7, topic:7249"]
30 A as motor max seems a bit too low
[/quote]


Yes I had updated it to 60A. Below are my current settings.

---

The Motor Min Regen at -30A felt a bit hard for me so I set it to -40A and feels a bit better. 

Also it seems like I have to repeat that 0.004>0.04 glitch every time I update the motor settings.

I have ordered 1 more 3S battery since I had the space and did not want to worry about the heat that 6S produces versus 9S. Plus the speed! haha

<img src="/uploads/db1493/original/2X/c/c6aa63501b59c3fe5391e648d7e226038082c909.png" width="484" height="190">
```

---
## \#10 Posted by: makevoid Posted at: 2016-08-08T07:35:08.423Z Reads: 262

```
The motor min at -40A should make your board break more than at -30A as it's a negative value so the lower you set it, the more braking force you will get. Also a good practice is to try not to set batt min and motor min regen too far apart from each other, so I guess that -30A was better for your vesc rather than -40 as there's the possibility of current building up on the vesc because of braking too hard/long and not being able to put that current back into the battery, if I'm not mistaken...
```

---
## \#11 Posted by: paul775 Posted at: 2016-08-08T07:47:31.724Z Reads: 256

```
When I had it at -30A it felt like my brakes were about to break. Now (maybe cause I tightened the belt a bit more now) I go to a stop much nicer. But that may be cause I fixed the belt and loctited the mount.
```

---
## \#12 Posted by: makevoid Posted at: 2016-08-08T07:56:02.481Z Reads: 254

```
Y then set motor min back to -30A or even a little bit lower if you want your vesc to not get overheated from braking and if you still feel enough braking force. If you want to have more breaks you should upgrade your battery and get another two packs in parallel so you can put your batt-min (regen) to -20A so it will be inline on its nominal charge value. Also you could try to put -15A on that value now because it should be able to handle a bit more than it's nominal charging capacity for a short charge but you have to check if the battery doesn't become warm/hot after a long/frequent braking session.
```

---
## \#13 Posted by: DivenParker Posted at: 2016-10-26T02:11:36.517Z Reads: 213

```
I think you should set your [6s battery](http://www.genstattu.com/6s-22-2-v-lipo-battery.html) about at 22.2V . 1S= 3.7V.
```

---
## \#14 Posted by: nick191 Posted at: 2017-02-16T06:24:59.493Z Reads: 163

```
Can you please put up he setting you are now using I'm not to sure and would like to know as I am using the same setup as you?
```

---

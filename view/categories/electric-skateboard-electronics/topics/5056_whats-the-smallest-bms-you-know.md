# Whats the smallest BMS you know?

### Replies: 21 Views: 2208

## \#1 Posted by: Nordle Posted at: 2016-06-23T18:26:19.580Z Reads: 200

```
Hey folks,
I'm looking for a new 10S BMS, would like to know if someone knows a model thats smaller than [this one (53x63 mm)](http://de.aliexpress.com/item/New-Battery-Protection-BMS-PCB-Board-For-10-Packs-36V-Li-ion-Cell-Max-40A-W/32607634513.html?spm=2114.13010208.99999999.261.wI0Zcr) ? Should have balance function don't care about discharge.
```

---
## \#2 Posted by: longhairedboy Posted at: 2016-06-23T18:56:51.883Z Reads: 189

```
That's pretty damned small compared to what I've been using. Do they have a 60 amp version that size? I'm looking for something way smaller than what i currently use, and this looks a lot like the ones i've seen in posts on Instagram that i was never able to hunt down.
```

---
## \#3 Posted by: Nordle Posted at: 2016-06-23T19:13:48.907Z Reads: 184

```
Don't think so. But anyways I want to bypass discharge, just switch a p-fet off the discharge line who then switches my anti spark (vedder/fechter design) wich is actually another n-fet off. If any cell drops below 2.5V or whatever the BMS is rated for. Max amp draw should be handled from VESC.
```

---
## \#4 Posted by: lowGuido Posted at: 2016-06-23T19:17:25.589Z Reads: 179

```
just be careful with that. 
if you are hill climbing or accelerating with full forward lean when you switch your FET you can SYF!
```

---
## \#5 Posted by: Nordle Posted at: 2016-06-23T19:37:09.018Z Reads: 167

```
Without power should freewheel, don't stop? Same effect as I would leave the trigger?
```

---
## \#6 Posted by: treenutter Posted at: 2016-06-24T00:05:52.909Z Reads: 151

```
 [quote="lowGuido, post:4, topic:5056"]
if you are hill climbing or accelerating with full forward lean when you switch your FET you can SYF
[/quote]

@lowGuido I've been thinking about this as I am [building a new battery pack.](http://www.electric-skateboard.builders/t/18650-10s3p-battery-for-the-village-build/2087) Wouldn't it actually be better to have VESC handle max amp draw, when compared to the BMS? The BMS will cut power immediately to protect itself. This leads to a total SYF situation.

But VESC has cuttoff settings that will throttle down if amp draw gets too high, right?

So wouldn't it be safer to slow down gradually as you approach the threshold vs the BMS completely cutting off? I must be missing something here...
```

---
## \#7 Posted by: treenutter Posted at: 2016-06-24T00:07:24.225Z Reads: 139

```
@longhairedboy not to mention that these are $10, compared to our group buy that's a sweet price!
```

---
## \#8 Posted by: lox897 Posted at: 2016-06-24T00:30:22.921Z Reads: 136

```
Be careful will the small ones. I saw on YouTube the other day, a guy builds battery packs and he has like 4 of those small ones failed on him.
```

---
## \#9 Posted by: lowGuido Posted at: 2016-06-24T02:22:33.822Z Reads: 132

```
The difference is that when you release the trigger you are expecting it! If you are full lean up a hill and it cuts when you are **not** expecting thats a full load of street. In your face.
```

---
## \#10 Posted by: Nordle Posted at: 2016-06-24T05:08:37.837Z Reads: 122

```
Thats rigth, I'll use VESC LVC too, that should cut off before the BMS does. The above described method only should cut power if any single cell grp fails.

@lox897 can you link that video, does this guy discharge trough BMS? or fail while charging? I saw some guys on ES using this, didn't read about any problems.
```

---
## \#11 Posted by: lox897 Posted at: 2016-06-24T05:09:38.402Z Reads: 122

```
I'll have a look for it now.

EDIT: here it is: https://youtu.be/Tg8L6vKX0ho skip to 3:00
```

---
## \#12 Posted by: longhairedboy Posted at: 2016-06-24T16:14:43.050Z Reads: 108

```
which makes me immediately question the quality, of course, but i'm still very curious. 

Also, while max amp draw should be handled in VESC, it should probably also be handled in the BMS at a higher threshold than what the vesc cuts off at in my experience, and the BMS should probably be set to cut off just above its continuous rating. 

for example i use an 80amp continuous BMS on a pack rated for 80amps continuous but i've got my max current set at 60amps with 30 amps per motor in the VESC. If there is a serious problem and the VESC fails in some horrible way the BMS can still protect the pack. So even during hill climbing you barely get warm in the pack and probably won't ever reach those thresholds.
```

---
## \#13 Posted by: Nordle Posted at: 2016-06-24T16:39:59.280Z Reads: 104

```
Makes also sense, but my fuse already cares about that if VESC should ever fail. I just want the BMS for charging balance function mainly.

Your video doesn't say anything specific about the linked BMS, he says the small ones fail for him in higher voltage applications;) And I'm pretty sure they do while discharging.
```

---
## \#14 Posted by: akira Posted at: 2016-06-24T17:38:10.924Z Reads: 102

```
I wonder why there are not more people doing like OKP and using the BMS only for charging.
The 18650 are very stable and the drift in one discharge is very small. 
If you bypass the BMS for discharge and only balance/charge through the BMS, you can use a much smaller one.
The charge BMS can be chosen to handle the charging current which is only a fraction of the max discharge.

What is the disadvantage of this solution ?
Are there good reason to avoid it ?
OK the BMS in discharge adds another protection of the VESC but apart from that ??
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-06-24T18:27:00.989Z Reads: 94

```
i just requested a sample of these from BestTech.

http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCB-D345.html

<img src="/uploads/db1493/original/2X/2/2e31b239d4ba757f2ce290225a524e4bc489e4d9.png" width="450" height="338"> 

I'm going to drop to 60 amps from 80 because i think 80 is a little too much overkill and these have a better layout in my opinion. Although i wish i could find some with the balance ports, p- and b- terminals all on the same damned side. But i guess that's asking too much.
```

---
## \#16 Posted by: Nordle Posted at: 2016-06-24T22:26:14.644Z Reads: 82

```
Okp is using this ''small white'' BMS to from what I saw him posting on ES. And he's bypassing discharge from what I remember. You know maybe if it worked out for him?
```

---
## \#17 Posted by: akira Posted at: 2016-06-24T22:40:21.158Z Reads: 82

```
It works very well from what I know.
He already built several baord with this system.
```

---
## \#18 Posted by: Nordle Posted at: 2016-06-24T22:46:44.967Z Reads: 86

```
Thank you.
I read also from [Nobuo (on ES)](https://endless-sphere.com/forums/viewtopic.php?f=14&t=71410&hilit=bms+bypass&start=25), that he's using this one without problems. And I think he knows what he says:D

So back to topic:
You know any smaller?
```

---
## \#19 Posted by: Nordle Posted at: 2016-06-27T19:13:27.367Z Reads: 73

```
Rather than turn my board off, it should trigger a warning light or buzzer. Would be like an RC voltage buzzer. And somehow i like riding with these buzzers... _when you go up a steep hill and your tiny lipo begins to cry._
```

---
## \#20 Posted by: longhairedboy Posted at: 2016-06-27T19:14:24.565Z Reads: 73

```
Ride the flames, my freind.
```

---
## \#21 Posted by: Nordle Posted at: 2016-06-27T19:33:08.148Z Reads: 69

```
What can i put between my board and my old lipo pack?
:smiling_imp:Tell me and i leave the buzzer at home!
```

---

# Got my VESC! But is there a problem?

### Replies: 24 Views: 2346

## \#1 Posted by: wiehan Posted at: 2016-07-11T15:03:39.685Z Reads: 183

```
After ordering my VESC on the 15th of February, I finally received it today! Nobody can say I'm not patient.

This is my first VESC and only my seconds eboard build, so I have a few (noob) concerns.

Uploaded you will find a pic highlighting one area of concern. It looks like the ground wire's solder spills over onto (what to me looks like a) MOSFET, the same thing occurs on the other side. Is this normal? Would this not cause a short circuit somehow?

Second total noob question: The thermal plastic covering the VESC, does that generally stay on, or do some people take it off in their builds? 

Thanks.

<img src="/uploads/db1493/original/2X/b/b778e57e07da7b2a5eaf45b7295b8d478f014762.jpg" width="375" height="500">
```

---
## \#2 Posted by: Blasto Posted at: 2016-07-11T15:52:18.596Z Reads: 175

```
yes that is perfectly normal, if you notice on all the other mosfets, the same pins are "shorted" together
```

---
## \#3 Posted by: treenutter Posted at: 2016-07-11T16:00:48.044Z Reads: 174

```
@weihan I think it's fine and won't affect performance, although I agree that the soldering job isn't very precise.
```

---
## \#4 Posted by: Jack Posted at: 2016-07-11T16:11:26.504Z Reads: 173

```
Leave the plastic heat shrink on, it protects against shorts and has a little bit of moisture protection :slight_smile:
```

---
## \#5 Posted by: Pablo_702 Posted at: 2016-07-11T21:00:17.962Z Reads: 136

```
Is this vesc from enertion?
```

---
## \#6 Posted by: Jinra Posted at: 2016-07-11T21:09:06.530Z Reads: 132

```
I got my Enertion VESC today and it has a single big cap, so I don't think so.
```

---
## \#7 Posted by: Nordle Posted at: 2016-07-11T21:14:43.916Z Reads: 131

```
[quote="Jinra, post:6, topic:5911, full:true"]
I got my Enertion VESC today and it has a single big cap, so I don't think so.
[/quote]

that is very sad
```

---
## \#8 Posted by: Jinra Posted at: 2016-07-11T21:15:41.013Z Reads: 128

```
Why is that sad?
```

---
## \#9 Posted by: Nordle Posted at: 2016-07-11T21:27:17.122Z Reads: 126

```
Cause it's shown with 3 caps + pcb on enertion's store. And multiple small caps > one biggie.
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-11T21:28:30.896Z Reads: 125

```
Number of caps doesn't really matter, as long as there's enough capacitance and voltage that the VESC needs. But I agree, a bit misleading on the website.
```

---
## \#11 Posted by: Nordle Posted at: 2016-07-11T21:30:12.453Z Reads: 122

```
ESR is everything that matters and esr is much lower with multiple caps
```

---
## \#12 Posted by: Ulfberht Posted at: 2016-07-11T21:35:29.991Z Reads: 119

```
@wiehan You may want to take a sharp blade and trim out a patch right above your mosfets for cooling. It allows more airflow to let those mosfets "breathe", but I wouldn't take it all off. It's a pretty durable material that will protect your VESC. You are going to have to cut it to get to your JST connectors anyway. :wink:
Here's an example from http://www.ollinboardcompany.com/product/vedder-s-speed-controller
<img src="/uploads/db1493/original/2X/d/d5607aa29d32e1026b2fe06f5711f83b2e5dcee3.png" width="659" height="500">
```

---
## \#13 Posted by: Nordle Posted at: 2016-07-11T21:42:13.102Z Reads: 115

```
Is this from enertion too?
```

---
## \#14 Posted by: Ulfberht Posted at: 2016-07-11T21:51:20.723Z Reads: 117

```
To address your solder concerns....Here's a couple of quick pics.
<img src="/uploads/db1493/original/2X/7/7ca828f8880f9a3498c78d927002b96426f08f1a.png" width="375" height="500">
<img src="/uploads/db1493/original/2X/9/9bf213864af65a3ccb9bd97d7b4cba3f262ee9fd.png" width="690" height="331">
If you comare the two pics, you can clearly see the pad in the highlighted area and how it connects to the traces on the PCB.
Looks clean, dude! Not the slickest solder job, but should be fine!
```

---
## \#15 Posted by: Sboard342 Posted at: 2016-07-11T22:03:11.563Z Reads: 115

```
I received my enertion VESC today, and it has 2 capacitors vs 3 like the Ollin board VESCs I have.
```

---
## \#16 Posted by: Nordle Posted at: 2016-07-11T22:09:01.110Z Reads: 114

```
@onloop
is it at least possible after 3 months of delay that i get my vesc's with 3 caps like they are on the pic's from ur page?
```

---
## \#17 Posted by: Jinra Posted at: 2016-07-11T22:09:10.901Z Reads: 114

```
I guess it depends where you get it shipped from. My Enertion VESC came from a Texas mfg and it only had 1 cap.
```

---
## \#18 Posted by: Lizardking0069 Posted at: 2016-07-11T22:10:12.426Z Reads: 113

```
That doesnt look right
```

---
## \#19 Posted by: Sboard342 Posted at: 2016-07-11T22:10:39.482Z Reads: 114

```
Mine came from texas as well, "MacroFab, inc."   I am fine with two, as long as when I order the second one it matches this one.

<img src="/uploads/db1493/original/2X/4/4e76f358c99c03a5a15fedca6f4381172722f9d5.JPG" width="375" height="500">
```

---
## \#20 Posted by: Jinra Posted at: 2016-07-11T22:11:14.500Z Reads: 114

```
Hm yea same factory. I wonder why mine came with one.
```

---
## \#21 Posted by: Nordle Posted at: 2016-07-11T22:30:25.701Z Reads: 107

```
cause it's less expensive... poor..
```

---
## \#22 Posted by: wiehan Posted at: 2016-07-12T05:17:57.941Z Reads: 82

```
Yes, Enertion VESC
```

---
## \#24 Posted by: flatsp0t Posted at: 2016-07-12T09:46:27.416Z Reads: 72

```
Oh, somebody is a little bit Salty.
```

---
## \#25 Posted by: wiehan Posted at: 2016-07-12T13:16:14.844Z Reads: 64

```
I know this is slightly off topic. But I also ordered the SPACE cell battery from enertion and ended up getting refunded as due to shipping legislation (and I presume due to stupid chinese hoverboards catching fire) it could not be shipped to South Africa. Has anyone else managed to get the SPACE cell shipped "overseas"?
```

---

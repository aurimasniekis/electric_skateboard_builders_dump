# Any issues with Unity and sudden slow downs

### Replies: 24 Views: 431

## \#1 Posted by: RafaelinMissouri Posted at: 2019-05-16T03:42:30.513Z Reads: 184

```
so 12.5 miles into my ride I'm going up a hill not super fast and the board did this sudden slow down.  Does the Unity freak out sometimes?  It was not just loosing throttle. It was kind of breaking and made me jump off my board.
I looked at the battery % right away on the app thinking it might be critical. But was at 40%
I think it did that before on a slightly different set up and the battery was lower.


![Screenshot_20190515-215141|243x500](upload://u148AvXiew574YMXWpFfCjad2xU.jpeg) ![20190514_202559|690x388](upload://tIPyXOMdZA0YOzm5BZqt9xAuu1v.jpeg) 
The new new. Little rocket.  Ralleycat board. 12S3P discharge only Bms. Unity. TB 6355s. Caliber II. Dickytho mounts. 14/30t 83mm
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-05-16T04:03:40.302Z Reads: 171

```
Check the support thread.

Other users have had similar reports. This is not a common incident and only seems to be occurring with a small number of Unities in each batch.
```

---
## \#4 Posted by: sk8l8r Posted at: 2019-05-16T08:55:24.959Z Reads: 143

```
[quote="RafaelinMissouri, post:1, topic:93994"]
Ralleycat board
[/quote]

Really like that deck!!
```

---
## \#5 Posted by: sayekim Posted at: 2019-05-16T13:44:25.022Z Reads: 121

```
I think you might be hitting your soft cut off value. 

40% on a 3p is not a lot under load. 

Some logging app would instantly show this.
```

---
## \#6 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:03:06.005Z Reads: 115

```
Well, I was wondering if if has to do with hitting the soft cut of value on the battery.  And if that is the case it should just coast, not kind of break.
I dont see that I can adjust those values on the App. I wonder if the Computer version allows for a change.
```

---
## \#7 Posted by: venom121212 Posted at: 2019-05-16T14:04:58.536Z Reads: 111

```
Going from acceleration to not very much feels like a brake... especially going uphill
```

---
## \#8 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:10:08.442Z Reads: 109

```
It really feels like more than just going into coasting. I was not going very fast and it threw me off my board.  If this is normal behavior I'm going to be super sketched out riding.
```

---
## \#9 Posted by: venom121212 Posted at: 2019-05-16T14:11:00.240Z Reads: 105

```
It has never happened with a well charged battery though?
```

---
## \#10 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:19:07.631Z Reads: 102

```
Correct.  Has happened twice wiht this Unity.  1st time I was a 10S5P and it was really low.
Last night was the 12S3P and I had already gone 12 miles.  I don't have a battery meter on this set up and was using the Focbox app to see batery percentage.  I was surprised to see it was still 52% at 9.5 miles. and when the cutout happened I checked it and it was 48%.  do you know if you can change the cut out values?
```

---
## \#11 Posted by: venom121212 Posted at: 2019-05-16T14:21:41.549Z Reads: 99

```
That would be dependent on your BMS discharge setup. You can change cutoff values using the windows tool for sure.. not sure if you can in the mobile app.
```

---
## \#12 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:23:02.905Z Reads: 100

```
It is a Psychotiller Pack.  Charge only BMS.
I will hook the Unity up to the computer tonight.
Appreciate your comments.
```

---
## \#13 Posted by: venom121212 Posted at: 2019-05-16T14:26:29.708Z Reads: 97

```
No problem! Do you have thermal throttling enabled on your unity? I could be overheating while going uphill.
```

---
## \#14 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:29:33.034Z Reads: 100

```
Are you calling me fat? (well, you would be right, 215lbs) 
 I did not change that setting.
so looks like it is on.  But  right after it happened it said the motors were at 46 and 47.  not sure how fast they spike.

![Screenshot_20190516-062206|243x500](upload://793dALfkO6lV3dqchckOhzlbmFr.jpeg)
```

---
## \#15 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:30:15.929Z Reads: 90

```
wrong screen shot![Screenshot_20190516-062225|243x500](upload://AojB7zZJLDcWYJpuQ5isTpALVn1.jpeg)
```

---
## \#16 Posted by: venom121212 Posted at: 2019-05-16T14:30:58.432Z Reads: 87

```
Unfortunately, testing failures is never fun. 

But it is another option to try haha
```

---
## \#17 Posted by: sayekim Posted at: 2019-05-16T14:35:34.668Z Reads: 88

```
Yeah hitting a cut off going up a hill will definitely not feel soft under load. 
I’d say try that same hill on a full battery and a 40% battery again. Mystery solved if it doesn’t happen on a full charge then.
```

---
## \#18 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:44:38.100Z Reads: 85

```
I will take yours and venoms word for it.
It freaked me out and seems really abnormal to me.
the first time if happened several weeks back I totally ate it and went down hard. 
that battery was really low.
I have ridden so many other boards and never had it be such a sudden hit.
Metroboard micro Slim,
Evolve Bamboom GT.
Wowgo 2S.
Diy 10S5P with dual Maytech Vescs.
Diy 10S5p with Dual Focboxes.
Diyeboard 10S5P kit  with their ultra crappy ESC.
```

---
## \#19 Posted by: Blasto Posted at: 2019-05-16T14:52:23.491Z Reads: 82

```
If you switch from a 10s to a 12s battery, you do need to change your battery parameters (battery limits tab)
```

---
## \#20 Posted by: Jinra Posted at: 2019-05-16T14:54:30.045Z Reads: 82

```
Though the cutoffs would be lower.
```

---
## \#21 Posted by: RafaelinMissouri Posted at: 2019-05-16T14:55:51.541Z Reads: 79

```
Thanks,  this was a whole new build. So I had started from scratch on the set up.  Also was new firmware.  it was set to 12S
```

---
## \#22 Posted by: RafaelinMissouri Posted at: 2019-05-16T17:24:32.870Z Reads: 66

```
Looks like you can change it on the app.  first drop down go all the way down to custom, then jumps over to cutoffs.  I am not at home now to actually try...
```

---
## \#23 Posted by: RafaelinMissouri Posted at: 2019-05-19T18:15:03.623Z Reads: 45

```
Updated app settings. Cut off at 37 and 35. Turned off motor temp.

I also changed my the wheel gear from 30 to 34 t.  Motor is 14 t on 83mm wheels.

I did a ride similar to the one the other day with the issue.  No problems today.
I am riding very concervatively in general.  

https://www.relive.cc/view/rt10005279086
```

---
## \#24 Posted by: venom121212 Posted at: 2019-05-19T18:17:28.156Z Reads: 46

```
That's a pretty neat app. Never heard of it before, thanks!
```

---
## \#25 Posted by: RafaelinMissouri Posted at: 2019-05-19T18:19:33.234Z Reads: 47

```
Relive is really cool. Totally free. What I use any way. You can put up to 10 fotos on the story and it places them where you took them. So that was a cool reference of where the battery was at
```

---

# Ready to go 12s, please check my battery diagram

### Replies: 56 Views: 942

## \#1 Posted by: rey8801 Posted at: 2018-09-26T10:03:31.465Z Reads: 175

```
Hi guys I have already posted this question but inside another thread and so the discussion didn't answer to my questions. If someone wants to contributes please feel free...

"
I am going to make a 12s3p. I made this diagram.
![BatteryDiagram12s3p|690x341](upload://dp3ZOC76aeeE6JLX3cPrU2MDjFR.jpeg) 
I have to follow this distribution because I do not have a lot of space. basically the last two P groups are on a second layer. I would have few questions:
I will use 10x0.15mm nickel strip, planning to use 2 nickel strips for P group
1- For series connections do you think 12awg or 2 16awg is enough or better on 12 paired with one 16awg. Online I found 12awg rated for 41A, while 16awg for 21A. My battery would be max 60A.
As isolation I will use Isolation rings on the positive side and fish paper under the balance leads. Between parallel group I will use fish paper and also on top to separate it from the second layer. P groups glued together. Kapton tape on both of the sides of each 6 parallel groups and foam in the middle to keep the two cell lines isolated.Then I will heat shrink the two layers separately and place the bms externally.
The enclosure is covered by foam internally to protect the battery, which is secured to the desk using Velcro.
What do you think about the diagram and the plan? Thanks a lot to everyone that wants to contribute.
I uploaded here the pptx in case someone want to correct it or use it for is purpose :grin:
https://mega.nz/#!ztknFCga!turUECUE_nF5vsvOhscW7wPgSiK21h_MCj-ENsBgXFw"

Thank you!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-26T11:39:13.313Z Reads: 133

```
maybe it helps to tag some battery builder
@b264 @Eboosted @Acido @chaka @Namasaki
```

---
## \#3 Posted by: rey8801 Posted at: 2018-09-26T11:41:05.416Z Reads: 130

```
True, thanks.
```

---
## \#4 Posted by: b264 Posted at: 2018-09-26T11:41:23.153Z Reads: 129

```
This would be much safer if the P groups across from one another connected together like at the B11 & B5 connections ... except on the whole battery.  It's SO MUCH safer.
```

---
## \#5 Posted by: rey8801 Posted at: 2018-09-26T11:46:28.623Z Reads: 127

```
Thanks for the input. What do you mean except for the whole battery? You mean the genral negative and positive. To do what you say I should use cell level fusing distribution, having the nickel strips parallel to the cells. right?
```

---
## \#6 Posted by: b264 Posted at: 2018-09-26T11:51:29.098Z Reads: 127

```
No

The series connections should go across to the P-group that's right there.  So under extreme vibration if the insulation between the P groups is breached, they are already connected together, preventing one kind of failure mode.

![connections|305x230](upload://abaq8WOXm5Cc1sQiBRd5nC6sJoz.png)
```

---
## \#7 Posted by: rey8801 Posted at: 2018-09-26T11:53:43.124Z Reads: 118

```
I see thanks!
Do you think 12awg is enough or better 12awg and 16awg paired for series connections?
```

---
## \#8 Posted by: b264 Posted at: 2018-09-26T11:58:45.657Z Reads: 119

```
I would not use 12S nor would I use 12AWG.  10AWG is better which is rated for 57A continuous and also 10S is much better on your ESC components
```

---
## \#9 Posted by: rey8801 Posted at: 2018-09-26T12:01:33.618Z Reads: 121

```
Is gonna be tricky to solder it in between...I can not make it too wide otherwise won't fit in the enclosure. I guess cell fusing level is the way then. If I do little loops with 10awg is gonna be too thick to be folded.
```

---
## \#10 Posted by: b264 Posted at: 2018-09-26T12:02:40.158Z Reads: 119

```
use 2 layers of the 0.25" tinned copper braid which is good for 40A per
```

---
## \#11 Posted by: b264 Posted at: 2018-09-26T12:03:28.632Z Reads: 116

```
![20180924_001917_HDR|690x345](upload://llAAbGcprXCEwPwOFfcRNQoR3EU.jpeg)
```

---
## \#12 Posted by: rey8801 Posted at: 2018-09-26T12:03:40.418Z Reads: 114

```
40A each or total?
```

---
## \#13 Posted by: b264 Posted at: 2018-09-26T12:04:00.801Z Reads: 118

```
per
(each)
```

---
## \#14 Posted by: rey8801 Posted at: 2018-09-26T12:04:29.593Z Reads: 115

```
Cool. Do you then fold it and place it in between cells? I mean with the front one
```

---
## \#15 Posted by: b264 Posted at: 2018-09-26T12:05:39.712Z Reads: 114

```
I think it's much safer when those cells butting up against each other are electrically connected already

Imagine the battery in a paint shaker for 24 hours and holes being rubbed in insulation

I'd much rather two things touch that are already connected together ;-)

also, use fish paper
```

---
## \#16 Posted by: rey8801 Posted at: 2018-09-26T12:07:20.480Z Reads: 113

```
Sure that's clear I was asking about the final disposition
Do you have a picture? I would like to see if the copper braid is in between or it makes a loop on top of the battery.
```

---
## \#17 Posted by: rey8801 Posted at: 2018-09-26T12:07:45.161Z Reads: 114

```
Find the fish paper is the problem in EU!
I ordered from Ali but will take a while
```

---
## \#18 Posted by: rey8801 Posted at: 2018-09-26T12:11:03.616Z Reads: 114

```
![BatteryDiagram12s3p_2|690x341](upload://twDT1Gas9gZuJhMlfQc7rIVngVj.jpeg) 
Better now?
```

---
## \#19 Posted by: b264 Posted at: 2018-09-26T12:13:13.306Z Reads: 118

```
Yes, that's exactly what I meant :smiley:
```

---
## \#20 Posted by: rey8801 Posted at: 2018-09-26T12:13:58.923Z Reads: 114

```
I am listening :grin:
```

---
## \#21 Posted by: Acido Posted at: 2018-09-26T12:18:15.830Z Reads: 112

```
theres some on nkon
```

---
## \#22 Posted by: Andy87 Posted at: 2018-09-26T12:18:27.641Z Reads: 106

```
is there an advantage of tinned copper instead of only copper braid?
```

---
## \#23 Posted by: b264 Posted at: 2018-09-26T12:18:58.456Z Reads: 106

```
Easier to solder which means less chance of cells getting more hot
```

---
## \#24 Posted by: rey8801 Posted at: 2018-09-26T12:19:01.289Z Reads: 99

```
Fish paper is over. Already asked. I buy the cells from there. :weary:
```

---
## \#25 Posted by: sk8l8r Posted at: 2018-09-26T12:31:23.124Z Reads: 90

```
[quote="rey8801, post:9, topic:69248"]
10awg
[/quote]

I regretted using 10 awg on my battery I wish I'd used 2x 14 awg instead - 10 is really stiff and I suck at soldering it!
```

---
## \#26 Posted by: rey8801 Posted at: 2018-09-26T12:32:29.625Z Reads: 85

```
Well I have access to a really big soldering iron. For industrial application. Basicay in less than 2 sec you can solder 12 awg at the first contact. I guess 10 awg would be feasible too. It is like 360watt.
```

---
## \#27 Posted by: rey8801 Posted at: 2018-09-26T12:37:04.884Z Reads: 85

```
I was wondering do you use any foam in between the cells in series. I know they are connected but maybe to preserve the nickel strips. if yes how do you place it? Since the copper braid is in the way.
```

---
## \#28 Posted by: b264 Posted at: 2018-09-26T12:48:31.385Z Reads: 92

```
I set the iron at 850 degrees F (454 C) and it works fine.  I use 700 F (371 C) for regular stuff.

I do put fishpaper there but not foam -- but I'm not a battery building expert though, try @Eboosted  @Acido  @chaka @Namasaki
```

---
## \#29 Posted by: Acido Posted at: 2018-09-26T12:49:36.326Z Reads: 93

```
i never really considered braided wire, i just ordered 2 meters to test how it will work
```

---
## \#30 Posted by: rey8801 Posted at: 2018-09-26T12:55:18.691Z Reads: 96

```
Where did you find them? :grin:
I actually used a braided wire for my first battery but I made it by braiding 4 copper wire together. Never again :laughing:
```

---
## \#31 Posted by: Acido Posted at: 2018-09-26T13:30:49.113Z Reads: 91

```
China

I could only find 300m spools here in croatia and super thick ones for grounding houses idk what like 5cm wide and 5mm thick
```

---
## \#32 Posted by: rey8801 Posted at: 2018-09-26T13:54:16.755Z Reads: 92

```
https://www.ebay.de/itm/Flat-Tinned-Copper-Braid-30-Amp-4mm-x-0-8mm-Various-Lengths-www-alcoltd-com/122628649748?hash=item1c8d3cb314:m:mESHZXIU5DZXuKpNYdhsDSg I found this one. A bit expensive but EU.
```

---
## \#33 Posted by: Acido Posted at: 2018-09-26T14:00:18.981Z Reads: 87

```
Yea, but you wont need much of it anyways
```

---
## \#34 Posted by: rey8801 Posted at: 2018-09-26T14:01:42.145Z Reads: 86

```
Well I guess 2 meter would be enough. Still 20GBP
```

---
## \#35 Posted by: Acido Posted at: 2018-09-26T14:03:12.242Z Reads: 88

```
You should be able to find it locally in the uk for sure i order all the weird stuff i need from UK
```

---
## \#36 Posted by: rey8801 Posted at: 2018-09-26T14:03:48.949Z Reads: 88

```
I am in Belgium. Here I only find water locally :laughing:
```

---
## \#37 Posted by: Acido Posted at: 2018-09-26T14:05:49.946Z Reads: 92

```
I guess we are in the same situation then, but we are selling our waters to foreigners because of shitty government :D
```

---
## \#38 Posted by: rey8801 Posted at: 2018-09-26T14:23:29.039Z Reads: 99

```
This one has better price and more choice https://www.aircraftspruce.eu/tinned-copper-braid-1-4-.htm
and http://www.techflex.nl/index.php?main_page=advanced_search_result&search_in_description=1&keyword=tinned+copper&x=0&y=0
```

---
## \#39 Posted by: Acido Posted at: 2018-09-26T14:47:47.874Z Reads: 96

```
this is probably way higher in quality
```

---
## \#40 Posted by: rey8801 Posted at: 2018-09-26T14:48:40.330Z Reads: 99

```
I bought it from the first one. 14 euro 3 meters not bad compare to the other prices.
```

---
## \#41 Posted by: rey8801 Posted at: 2018-09-28T06:10:33.050Z Reads: 86

```
Last question  how do you then place the two parallel cell groups? In eon front the other but do you use something in between, like foam pad? Because since there is the copper braid in between I do not see how to place the foam. The only solution I can immagine is that the copper braid makes a loop above the battery. Do you perhaps have a picture of that type of groups connected and with the damping material? Thx a lot!
```

---
## \#42 Posted by: b264 Posted at: 2018-09-28T07:34:25.378Z Reads: 89

```
[quote="rey8801, post:41, topic:69248"]
something in between, like foam pad?
[/quote]

Never foam

I mean, do use foam for the top and bottom after the battery is made for shock absorption

Don't ever use foam for electrical insulation, it will wear out under vibration and short out.  Use fish paper or plastic

Also see how I soldered the positive ones first?  That's no accident.  Make sure no solder goes under that nickel strip on the positive side
```

---
## \#43 Posted by: rey8801 Posted at: 2018-09-28T07:38:45.537Z Reads: 82

```
Yes noticed the positive first. So actually the two group are phically in contact between them? I know they are electrically connected but I thought metal on metal under vibrarion will affect the nickel strips welds.
```

---
## \#44 Posted by: b264 Posted at: 2018-09-28T08:05:48.249Z Reads: 81

```
I insulate them anyway, even though they're connected electrically
```

---
## \#45 Posted by: rey8801 Posted at: 2018-09-28T08:10:46.161Z Reads: 74

```
With fish paper?
```

---
## \#46 Posted by: b264 Posted at: 2018-09-28T08:42:40.035Z Reads: 76

```
&nbsp;yes&nbsp;
```

---
## \#47 Posted by: rey8801 Posted at: 2018-09-28T08:52:34.987Z Reads: 82

```
Last question so the copper braid is parallel to the nickel strip and you make cut in the fish paper to allow the copper braid to go through or the braid is perpendicolar to the nickel strips and you folded later on when you wrap it with heat shrink?
```

---
## \#48 Posted by: b264 Posted at: 2018-09-28T08:57:51.701Z Reads: 81

```
That's just what I do, I would trust more the battery professionals like @Eboosted and @darkkevind 

I do know the photo of EBoosted's battery below is one of the best-looking I've seen

[![KmCwUPY|281x500](upload://c9IXwL56splTsiD54Zi22W4Ky0m.jpeg)](https://www.electric-skateboard.builders/t/looking-for-feedback-on-the-battery-i-built/69287/23?u=b264)
```

---
## \#49 Posted by: rey8801 Posted at: 2018-09-28T09:02:11.600Z Reads: 76

```
I agree that that battery looks sick! I really appreciate your advice. Now I need to wait for the fish paper. Thank a lot
```

---
## \#50 Posted by: sk8l8r Posted at: 2018-09-28T10:24:26.568Z Reads: 69

```
[quote="b264, post:42, topic:69248"]
Don’t ever use foam for electrical insulation, it will wear out under vibration and short out. Use fish paper or plastic
[/quote]

I combine foam and fish paper (stick the paper to each side of the foam) for combined isolation/insulation of p-groups - foam on its own  would get destroyed in a couple of rides
```

---
## \#51 Posted by: janpirate Posted at: 2018-10-07T09:34:33.643Z Reads: 63

```
wow thanks! nice diagram. this help me a lot to build 12S4P.
those charger already bypass the BMS correct?
```

---
## \#52 Posted by: rey8801 Posted at: 2018-10-07T10:13:17.386Z Reads: 63

```
Yep is the 12s BMS from Bestech D140. Do you see that you can dowload the pptx file so yuu can modify the diagram fro your personal use.
```

---
## \#53 Posted by: janpirate Posted at: 2018-10-08T13:39:09.641Z Reads: 58

```

the diagram edited from yours ;)  however i need to confirm about the loop key. is it correct?

![diagram|690x412](upload://h8xTAES2ddVHLJKbk8OlaxRweT0.jpeg)
```

---
## \#54 Posted by: Andy87 Posted at: 2018-10-08T14:06:20.822Z Reads: 56

```
Loop key looks good 👍
```

---
## \#55 Posted by: janpirate Posted at: 2018-10-08T14:16:24.295Z Reads: 54

```
thanks ;)  now waiting for my batteries
```

---
## \#56 Posted by: rey8801 Posted at: 2018-10-08T14:28:01.145Z Reads: 54

```
As @Andy87 siad, loops key is fine. You already have the antisparks BTW.
```

---

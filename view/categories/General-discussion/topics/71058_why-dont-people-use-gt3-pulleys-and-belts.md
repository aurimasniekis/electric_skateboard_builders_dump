# Why don&rsquo;t people use GT3 pulleys and belts?

### Replies: 86 Views: 7211

## \#1 Posted by: TowerCrisis Posted at: 2018-10-13T06:50:56.329Z Reads: 427

```

[details="Original post here"]
I've been doing some calcs. A 28T to 60T GT3 3mm pitch belt is mechanically capable of giving 46.5 lbs of forward thrust using a 90mm wheel. And that's while staying in spec.

the 28T HTD pulley can handle 7.0 inlbs of torque. The GT3 pulley can handle 17.9 inlbs. These are all ballpark numbers but it's a general trend, over twice the load capacity...

So that brings up my question. As the DIY community has so many people pushing the boundaries of what is possible and putting our components past their limits, why does nobody use GT3 belts?

That 46.5 lbs of thrust is the max while in spec.. We obviously are exceeding the load capacity of our belts hence why people tend to shred them so often or have issues with skipping. So if we push GT3 to the limit we could surely get much better force out of it.

This may not apply to acceleration since we are usually motor limited, but i think it's important for braking. If you can't push your brakes to the max without skipping belt then you're not at peak performance.

And in addition to better wear resistance and load rating, they also cite quieter operation.
[/details]


**EDIT:** After further research, I have come to these conclusions.

**HTD VS GT2**

Here are some direct comparisons followed by interpretations of the data.

**General Lifetime:**

![Durability|690x322](upload://vmeDmCXk5UdpbR9TDgjcjuzyN9G.png) 
This is the general lifetime testing of the different belts. Each test was conducted with the same pitch, pulley sizes, speeds, and torque. It concluded upon belt replacement was necessary, or until enough data was collected (no need to go further, in the case of GT). The baseline for these tests was the HTD performance, set at 100%. These tests were conducted at speeds and pulley sizes that result in accelerated belt wear, which will be explained further down this post. **GT 5M has nearly 190% the lifespan of HTD 5M.**

**Tooth Jump:**

![Tooth%20Jump|690x430](upload://42YuYD2Yv9YS2ftFRV0oJ6eAYHJ.png) 
These results are not particularly favorable for GT 5mm pitch, at least upon first glance. HTD and GT seem to be very similar in the 5mm pitch, however it is important to see that this **test was only tested up to 2300 RPM, while we typically run our motors around 6000 rpm**. This results in much worse tooth skip, as it is far beyond the specifications of the tooth profiles. This higher rpm with higher torques is where GT shines greatest, and as you can see GT and HTD profiles begin to diverge as installation tension decreases. We run our tension somewhere in the 2-3 lb range. Some with idlers as low as 0 or 1 lb of tension.

**Operating Belt Tension:**

![Belt%20Tension|690x432](upload://ox5wgUr0UhRd7JBzrCSEXwReWGT.png) 
Here is the exact maximum belt specification for the tension on the taut side. For explanation's sake, I'm going to divide numbers by 2, so the belt width is equal to 12.7mm, which is close to our use case. **HTD 5M is rated at 51 lbs of tension. GT is is rated at 80 lbs.** Please note that this is independant of ratcheting or pulley size, this is only the maximum allowable tension on the belt.

**Minimum Pulley Size Per RPM Unit:**
![Pulley%20Size|349x500](upload://9v7Hy8wuQdsLLPtnBPpFxC7GHZi.png) 

This is fairly straightforward. A 22 tooth HTD 5M pulley is rated to operate at 1160 RPM. **This is over 5 times less than the 6000 rpm we operate at.** A 22 tooth GT 5M pulley is rated to operate at 2000 RPM. Again, we are far out of spec, but by much less. **This is 3 times less than the 6000 rpm we operate at.** Unfortunately, **both will experience accelerated wear, but HTD will suffer much worse**.

**Exact RPM And Torque Ratings:**

![HTD%20torque|457x500](upload://al5e5s8J82oxbHrNzPdQWvIkFXI.png)
![GT%20torque|446x500](upload://xQJ4ZwLPpqXldzLSo0qniXtcY1B.png) 

These graphs show the operating RPM and torque ratings. **HTD 5M is rated to 75 in lbs of torque at 6000 RPM. GT 5M is rated to 250 in lbs of torque.** This means that GT 5M can run at **3 times the torque** of HTD 5M. While we are not typically exceeding these, it still means that GT will suffer much less wear over time. Please note that this data is unrelated to pulley size, that data will come next and will show further disparity between HTD and GT.

**Exact Torque Ratings Per Pulley Tooth Count:**

![HTD%20exact%20torque%20and%20lifetime|690x413](upload://ygHvQm97uafduIdtbhiyt3qZcQ8.png)
![GT%20exact%20torque%20and%20lifetime|678x500](upload://fbRtJWSvGaifurH8tVLaWgJP7aQ.png) 

I'm going to use the math for 5000 RPM, as it is the closest common value to 6000 rpm between the two graphs. **HTD 5M is rated to 11.6 in lbs of torque with an 18T pulley. GT 5M is rated to 25.2 in lbs of torque with the same rpm and pulley.**

What is more interesting is the low RPM values. **At 100 rpm, HTD is rated to 25.7 in lbs of torqe, while GT is acceptable up to 58.5 in lbs** with an 18T pulley. Our intense startup torques far exceed HTD specifications.

However, HTD is already in the "accelerated wear" category all the way up to 28T pulleys at 5000 rpm. HTD suffers from excessive wear from an 18T pulley at any rpm of 1160 and up. GT is acceptable wear at 5000 rpm at any pulley size 18T and up. GT is functional from 200 rpm to 14000 rpm with an 18T pulley. It only suffers from excessive wear from 100 rpm and lower, which we are rarely in when riding. For a visualization, this is when the motor makes a full turn every .6 seconds, which is a very slow creep for us.

We will be exceeding the torque ratings of these, so GT will also suffer accelerated wear, but not nearly to the extent of HTD since it is already going to wear excessively at any torque.

**Other Details, Unrelated to Performance:**

**Ignore this if all you care about is raw performance, only the above information will be relevant to you.**

![Sound|690x461](upload://cBBQjS7dKpfShHPlKgLUxnvlYFC.png) 
The sound levels are not easily interpreted from this. Decibels are determined on a logarithmic scale, not linear. So 100 dBA is much more than 2x louder than 50 dBA. GT is significantly quieter than HTD.

![Idler%20Size|690x230](upload://bb2cQLZPjjtidkLTb00JHXWOZZ8.png) 
We use backside idlers. GT and HTD perform the same here, but the data shows that we are seriously exceeding the spec here lol. Reversed bend radius very negatively affects belt life (given that all other wear factors are already in spec. We use idlers so other factors like belt slippage don't occur, which is objectively a greater concern for wear).

**Totally random thing I found about belt movement that I thought was kinda neat:**
![Interesting%20detail|690x365](upload://mZunUhHb9B2r4OejzGlAuMMIsbn.png) 

I found this very interesting. In a tuned pulley setup where they are in line and not twisted of offset at all, the belt will always ride to one side. If you have a precision CNC'd motor mount setup that ensures your pulleys are properly lined up, then you will still suffer from belts moving sideways. It is dependant on the direction the fibers internal to the belt are twisted. S twist is the opposite of Z twist. So if you're using two of the same belts, they will both move in the same direction, ie: one will move away from your truck and the other towards it. Just thought this was interesting to read about.

**TLDR:**
All Gt profiles are far superior to HTD, particularly in lifespan, torque ratings, and rpm. If you want a quick interpretation of the data, here is a comparison of many profiles:
![In%20Conclusion|690x305](upload://fKrxnBIrEEFn6spBHNLKpjl6nZj.png)
```

---
## \#2 Posted by: Maxid Posted at: 2018-10-13T07:03:54.031Z Reads: 371

```
What are the numbers for HTD5? If anything you should compare HTD5 vs GT3.
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-10-13T07:17:49.156Z Reads: 368

```
GT3 is the tooth profile, the 3 isn't the pitch. GT3 comes in 5m as well.

Also, my mistake on the calcs. Those were all for 6mm wide belt, so doubling the numbers for 12mm wide would be accurate.

For 18T pulleys with 15mm wide belt, HTD is rated to 27.7 inlbs of torque at 1600 rpm, while a GT3 belt would be capable of 49.1 in lbs at the same RPM. These are pretty significant numbers... All for 15mm wide belt 5m pitch.
```

---
## \#4 Posted by: Boardnamics Posted at: 2018-10-13T07:17:53.249Z Reads: 359

```
I have had this same question for a while
```

---
## \#5 Posted by: TowerCrisis Posted at: 2018-10-13T07:22:21.057Z Reads: 348

```
GT3 belts seem to be 50% more expensive but that's pretty insignificant considering it's still less than 20 bucks and you crazies are strapping over 1K in electronics and hardware onto a board :rofl:
```

---
## \#6 Posted by: Maxid Posted at: 2018-10-13T07:30:37.727Z Reads: 337

```
In your first sentence you said 3mm - so everything that comes after I read as HTD3. That's why I said the numbers should be for 5mm as that's what we use.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-10-13T07:34:30.234Z Reads: 320

```
Either way, the numbers are pretty similar, but ofc there are variations along the rating curves.
```

---
## \#8 Posted by: Maxid Posted at: 2018-10-13T07:40:50.480Z Reads: 318

```
What is that supposed to mean? If you cite numbers they need to be for the proper belt pitch and as basically everyone is using 5m pitch you should cite the 5m numbers.

Also the cost difference is not solely the belt but you need different pulleys as well. I am not aware of any seller that has either motor or wheel pulleys with GT3 tooth profile.
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-10-13T07:47:43.999Z Reads: 318

```
The exact numbers don't matter, it's the ratio that's important.

GT3 in all pitch lengths generally has 2x the load rating for the RPM's we use.

And yes, that's the whole point of my question. Why aren't these being made? They're objectively better.
```

---
## \#10 Posted by: Maxid Posted at: 2018-10-13T07:52:17.516Z Reads: 303

```
You have to imagine a noob reading your numbers and using them from now on when he talks about what his belt can deliver. If I had not said that those numbers are only for 3mm pitch he would be using wrong numbers.
Also the numbers do matter: if a HTD belt is good enough there is no reason to go for a GT3 even if it's twice as good.

And nobody is using them because as you said yourself: they are more expensive when you have to find the right pulleys as well. Also no idea about trademarks and patents and whatnot. Are sellers even allowed to make GT3 Profile pulleys themselves?
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-10-13T07:55:13.394Z Reads: 278

```
You're allowed to sell products that include the GT3 profile, but I'm not sure about selling individual pulleys.

Many companies sell pulleys that they say are "GT3 compatible" and name them something else, they just have slight variations but still maintain compatibility. The name is allowed to be used in marketing, aka you can market a product as GT3 compatible.
```

---
## \#12 Posted by: Maxid Posted at: 2018-10-13T07:57:00.669Z Reads: 264

```
I imagine as soon as you have slight variations in your profile your numbers are all over the place and nobody can tell you if there would indeed be even a difference to HTD.
Also I expect tooling for a square tooth profile like GT3 to be much more more expensive than the round HTD. So pulleys will be more expensive as well. It all adds up and since the HTD belts have shown to work well enough nobody bothers using GT3. With 3D printed pulleys this might not make a difference so go ahead and test them side by side for science.
```

---
## \#13 Posted by: Tamatoa Posted at: 2018-10-13T08:19:25.991Z Reads: 246

```
@TowerCrisis
Do you have a link where we could find GT3 pulleys with 5 mm pitch?
I looked on aliexpress but was not able to find any, I am just curious to see the cost. If I did not already have so many HTD pulleys and belts I would probably be tempted to try.
```

---
## \#14 Posted by: TowerCrisis Posted at: 2018-10-13T08:24:52.514Z Reads: 242

```
IDK where you read that but GT3 is not a square profile. They are round toothed, deep groove belts made by Gates to be the successor to GT2, which was the successor to HTD.
```

---
## \#15 Posted by: TowerCrisis Posted at: 2018-10-13T08:39:27.640Z Reads: 245

```
I can't manage to find any, but it's quite possible to 3d print them.

GT2 and GT3 are both backwards compatible with HTD pulleys. So using an HTD wheel pulleys would be fine. It's the motor pulley that you would really want to match to get peak performance.

Gates says that 5M GT2/3 is not recommended for HTD, citing that htd pulleys may not be rated for the additional loads of a GT2/3 belt. But for our use this really doesn't matter, the wheel pulleys isn't the bottleneck in this situation. So long as you use a GT2 pulley then you'll get the benefits.

Also, an important distinction to make: GT2 is the same profile as GT3, the only difference being in the tensile strength of the belts. You won't find any results for GT3 pulleys as there are none, they're all named GT2 pulleys and are inclusive of GT3.

GT2 pulleys can be bought from B&B manufacturing, or sdp-si.
```

---
## \#16 Posted by: Maxid Posted at: 2018-10-13T08:39:54.765Z Reads: 229

```
![Screenshot_20181013-103901_Dropbox|243x500](upload://nH5EEbVbags8N5jzhELWf8nlhOd.jpeg) 
That's why - HTD is much rounder (the 20mm at the bottom is HTD and is basically circular) while GT3 are "squarish"

I am also wondering if all your calculations are based on Gates marketing material. They will obviously say that their own brand is better than HTD and the information should be taken with a grain of salt. Are there independent comparisons out there?
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-10-13T08:54:30.804Z Reads: 221

```
[quote="Maxid, post:16, topic:71058"]
They will obviously say that their own brand is better than HTD
[/quote]

HTD and GT2 are both made by Gates. They don't have marketing material, they have test results giving specific load ratings for these profiles that's meant for people designing industrial machines.

And also gt2 not being perfectly round does not affect cost at all. Both HTD and GT2 pulley stock are hobbed using specialty cutters designed specifically for one profile. The difference in curvature is just a matter of having a slightly different grind on the cutting edge.
```

---
## \#18 Posted by: Okami Posted at: 2018-10-13T09:14:05.781Z Reads: 214

```
https://www.ebay.com/itm/2GT-Aluminium-Alloy-Timing-Belt-Pulley-Teeth-Width-10mm-Bore-5mm-8mm-40-Teeth/172009756616?hash=item280c9497c8:g:BVsAAOSwIFtaJ4jcL

https://www.ebay.com/itm/Pack-of-5pcs-Aluminium-Timing-Belt-Pulley-16-Teeth-2GT-Bore-5mm-Teeth-Width-10mm/172126124457?hash=item28138439a9:g:FSUAAOSwyYFaJ5un

Though wheel pulleys would be a lot harder to make / get (right form) unless 3d printed. I guess
```

---
## \#19 Posted by: Jmding Posted at: 2018-10-13T15:21:28.135Z Reads: 195

```
Only 2 valid reasons to use htd instead that I know of: idler make gt3 somewhat less important, and availability is annoying

Let's the community forward! If someone does a build with gt3, 3mm pitch and idlers to achieve aggressive gearing (4:1 or something) and vesc 6, then they'd be able to use higher Kv motors which are more powerful, and build a dual 5060 setup with as much power and torque as a dual 6374 setup.
```

---
## \#20 Posted by: Blitz Posted at: 2018-10-13T15:36:50.478Z Reads: 187

```
I would love to see GT3's hit the market,

If they could handle loads of torque then we would all be less interested in gear drives.
```

---
## \#21 Posted by: Brdchris Posted at: 2018-10-14T08:16:54.675Z Reads: 164

```
I use a gt3 belt on my normal htd pulleys. I was unable to get 12mm wide htd belts to work going up hills so i switched to 15mm gt3 and now I can run them loose with no tensioner pulleys. I’m 200lbs and can go up steep hills at full throttle.
```

---
## \#22 Posted by: Maxid Posted at: 2018-10-14T08:18:16.960Z Reads: 162

```
So a 15mm HTD belt would have worked just as well? How is that an argument for GT3?
```

---
## \#23 Posted by: Brdchris Posted at: 2018-10-14T08:21:34.873Z Reads: 160

```
wow pissy much? Just sharing my experience. I didn’t feel the need to waste money on a 15mm htd belt when I knew something better was on the market. But feel free to continue using something “just good enough” and not trying to improve the quality of your ride. The rest of us will continue to innovate and you can just copy us later.
```

---
## \#24 Posted by: Okami Posted at: 2018-10-14T08:32:32.143Z Reads: 155

```
@Brdchris Thanks for info. Might consider such option in future also, if u say it works even better and stock htd pulleys can be used.
```

---
## \#25 Posted by: Maxid Posted at: 2018-10-14T08:34:01.574Z Reads: 154

```
Its about the scientific method - all these posts are meaningless if there is no proper test. Your experience would have been valuable but only if your went from a HTD12mm to a HTD15mm.
So go get a HTD 15mm belt do the tests and tell us how it went - then we finally know.

Edit: oh and yes I am salty because this whole discussion is not how something like this should be done. We need real life test results and proper comparisons. And if we find out GT3 is twice as good as HTD I'd be happy to use GT3.
```

---
## \#26 Posted by: Maxid Posted at: 2018-10-14T08:35:19.565Z Reads: 144

```
But right now he didnt. He just said that a 15mm wide belt is better than a 12mm one.
```

---
## \#27 Posted by: GreasyGearsWRX Posted at: 2018-10-14T08:38:30.648Z Reads: 141

```
Where certain members of this thread have said that the current belt standards are acceptable I would beg to differ. Those building single drive rigs or those wanting to try to fit dual configurations with narrower belts on smaller hangers like 9” calibers could find these more effective belt options extremely beneficial to their applications! I’m very interested to see where this topic goes!
```

---
## \#28 Posted by: Maxid Posted at: 2018-10-14T08:39:50.944Z Reads: 141

```
I am riding a single 15mm wide HTD belt on a 15 to 42 gearing and have no belt skipping even downhill. Just for reference.
All I want is the proper numbers and proper tests - that's all.
```

---
## \#29 Posted by: GreasyGearsWRX Posted at: 2018-10-14T08:42:26.103Z Reads: 138

```
Well, just for reference I’ve been running 16 36 on 83’s with 15mm belts for almost a year and it’s complete trash. Even with tensioners it’s not a perfect science.

There’s criticism and then there is constructive criticism. Rather than complain that they aren’t presenting the information the way you like or testing the ways you see fit, offer to them how you would like this to be carried out.. ya know rather than shitting on it :)

So on that note! Do some testing on this and if it’s promising I may give it a try!
```

---
## \#30 Posted by: TowerCrisis Posted at: 2018-10-14T08:44:25.119Z Reads: 139

```
I agree that his experience is anecdotal, but...

[quote="Maxid, post:25, topic:71058"]
We need real life test results and proper comparisons. And if we find out GT3 is twice as good as HTD I’d be happy to use GT3.
[/quote]

It is. Gates has done the testing. They define the numbers. Believe it or not, many members of this forum are willing to trust the test results of a 5.4 billion dollar corporation whose two biggest product markets are belt power transmission and hoses. It's in their best interest to give valid numbers, they wouldn't be worth what they're worth if they couldn't properly advise businesses that use their products.
```

---
## \#31 Posted by: Maxid Posted at: 2018-10-14T08:44:50.867Z Reads: 128

```
[quote="GreasyGearsWRX, post:29, topic:71058, full:true"]
There’s criticism and then there is constructive criticism. Rather than complain that they aren’t presenting the information the way you like or testing the ways you see fit, offer to them how you would like this to be carried at.. ya know rather than shitting on it :)
[/quote]
Which is why I said that he should get a HTD 15mm belt and compare.
```

---
## \#32 Posted by: GreasyGearsWRX Posted at: 2018-10-14T08:48:29.528Z Reads: 126

```
That is fair. I agree testing is important. As per your request above.. What are proper numbers and proper tests in your opinion? So that we can accommodate your needs?
```

---
## \#33 Posted by: Maxid Posted at: 2018-10-14T08:48:54.803Z Reads: 128

```
I don't agree with that. They try to make as much money as possible and find ways to keep doing that. This whole belt science looks totally weird to me as finding relevant information on the internet seems super hard. For example I was not able to find any info on the evolution from HTD to GT3 and the iso standard that is referenced when it comes to the design costs like 200€ to download.

If we want GT3 to become our new standard because it is objectively better then we need to do the tests ourselves and confirm whatever Gates told us. At least that's how I see it.
```

---
## \#34 Posted by: Maxid Posted at: 2018-10-14T08:50:12.108Z Reads: 127

```
I was talking about how this thread started where  HTD3 was compared to GT3. That's obviously invalid as we use HTD5. Proper numbers are thus: you keep everything the same (belt length tooth count etc.) And only switch from HTD to GT3 profile.
```

---
## \#35 Posted by: TowerCrisis Posted at: 2018-10-14T08:54:09.668Z Reads: 124

```
It was a comparison of HTD 3M and GT3 3M. GT3, again, is the name equivalent to the name HTD.

And comparisons of different types of belt at the same pitch size is valid. It's a comparison between tooth profile, pitch does not matter as it does not affect one tooth profile more than the other.
```

---
## \#36 Posted by: Maxid Posted at: 2018-10-14T08:58:46.535Z Reads: 126

```
But if HTD5m would have a torque rating of 1000000Nm and GT3 of 1000001 then this discussion would not be necessary. I have no idea if the ratio between HTD and GT3 will stay constant between pitch sizes - only that it is much better between HTD3 and 3mmGT3.

I probably could do the math myself but I am lazy and I kind of feel that the one who claims GT3 is better is supposed to deliver the correct arguments. 

To emphasize: I am fundamentally not against a switch to GT3 - but it needs to be done right.

Edit: I kind of feel like the next @b264 who usually pushes for this type of thing.
```

---
## \#37 Posted by: TowerCrisis Posted at: 2018-10-14T09:02:19.860Z Reads: 120

```
[quote="Maxid, post:36, topic:71058"]
I have no idea if the ratio between HTD and GT3 will stay constant between pitch sizes
[/quote]

It's nearly a direct ratio. I hope you know this is a total "on the spot fallacy". But lucky for you I know a thing or two about belts. I'll be back with exact numbers.
```

---
## \#38 Posted by: Maxid Posted at: 2018-10-14T09:06:07.061Z Reads: 123

```
Isn't OTS about being required to cite information immediately when asked? I am not asking you to tell me the numbers right now. 
Also thanks for looking them up I am looking forward to it.

Edit: I also wanted to say that this is the internet and I have no idea about your experience with belts. So please  don't take my criticism personally.
```

---
## \#39 Posted by: TowerCrisis Posted at: 2018-10-14T09:06:56.977Z Reads: 116

```
In the mean time, feel free to read up on the differences between tooth profiles. This document was created by SDP-SI, a company unaffiliated with Gates. http://www.sdp-si.com/d265/pdf/d265t003.pdf
```

---
## \#40 Posted by: rojitor Posted at: 2018-10-14T10:02:08.935Z Reads: 117

```
Where did you buy them?
```

---
## \#41 Posted by: Maxid Posted at: 2018-10-14T10:21:29.516Z Reads: 115

```
In Germany I found them here:
https://www.zahnriemen24.de/zahnriemen/gates-powergrip-gt3/3m-gt3/?gclid=CjwKCAjw0oveBRAmEiwAzf6_rK6AWjdl3PKwONk-W3lWRF77OIHB2WeQVfHSLdwCZcAYxziH8rbZNBoCgXMQAvD_BwE#/gates-powergrip®-gt3-267-3mgt-15/
Seems like they have quite a wide length selection
```

---
## \#42 Posted by: rojitor Posted at: 2018-10-14T11:25:50.196Z Reads: 109

```
That link has 3 pitch. They have 5 pitch too.
https://www.zahnriemen24.de/zahnriemen/gates-powergrip-gt3/5m-gt3/#/gates-powergrip%C2%AE-gt3-400-5mgt-15/
I Will consider testing those. They are NOT cheap
```

---
## \#43 Posted by: Maxid Posted at: 2018-10-14T12:58:04.841Z Reads: 112

```
Oh yeah damn it my bad. Thanks for posting the correct one.
```

---
## \#44 Posted by: Benjamin899 Posted at: 2018-10-14T13:23:13.355Z Reads: 109

```
too me the GT3 and HTD profile look the same, both are round. So whats the big fuss about them? Or better put, why can the GT3 carry more torque
```

---
## \#45 Posted by: Pedrodemio Posted at: 2018-10-14T13:32:51.247Z Reads: 109

```
I tried to use HTD3 on my first build

The main problem has nothing to do with torque transfer, but with alignment. Since the tooth is smaller, you have less margin to to get thing out of roundness or your belt will skip

For this same reason you can’t run them loose like HTD5, Boosted use them, never held one in my hand, but from vídeos the belt tension they use is way higher than I am able to use on my HTD5 setup

In resume, everything have to be perfect in your drive train for them to work, your pulleys as perfect centered as possible, your motor mount to have as little flex as possible, and ideally have a bearing inside the wheel pulley to help with that

A positive point is that they have less loses since the rubber is thinner and takes less energy to flex and because of that the board “CAN” free roll better. I highlighted the can since that only happens if your construction is solid, if it’s not, you have to run the belt tension really high to avoid teeth skipping and the lower rolling resistance will not happen 

I’m my opinion is not worth, specially from those who are starting that generally use cheaper components since it will be a pain to get it working ok when your pulley may not be perfect and your motor mount flexing under load like a lot of the cheaper one that are sold

HTD5 can tolerate all that much better
```

---
## \#46 Posted by: Maxid Posted at: 2018-10-14T13:43:22.286Z Reads: 105

```
Did you mix up HTD3 and GT3?
```

---
## \#47 Posted by: Maxid Posted at: 2018-10-14T13:44:06.616Z Reads: 102

```
They are not - look at my image above. The HTD at the bottom is completely round while the GT3 has a different shape.
```

---
## \#48 Posted by: Pedrodemio Posted at: 2018-10-14T13:45:21.738Z Reads: 104

```
I only used HTD3, Which is almost the same as GT3, the latter has a more oval shaped tooth profile that according to gates improves the torque transfer capacity a little bit, but the problems with alignment will be the same for both
```

---
## \#49 Posted by: Maxid Posted at: 2018-10-14T13:46:34.131Z Reads: 107

```
As previously discussed in this topic we are talking about 5mm pitch but the tooth shapes HTD vs GT3. GT3 does not mean 3mm pitch (so has nothing to do with HTD3) but is simply the name of the tooth shape.
```

---
## \#50 Posted by: Pedrodemio Posted at: 2018-10-14T13:47:39.910Z Reads: 107

```
Oh sorry for that, completely my mistake

Is the GT2 that is equivalent to HTD3 right?
```

---
## \#51 Posted by: Maxid Posted at: 2018-10-14T13:48:30.151Z Reads: 107

```
According to @TowerCrisis the evolution was: HTD then GT2 as an improvement and then the current GT3 shape. All of these come in various pitch sizes.
```

---
## \#52 Posted by: PXSS Posted at: 2018-10-14T20:59:51.536Z Reads: 96

```
For what it's worth I've been using GT3 since my first build and all is good...
```

---
## \#53 Posted by: Blitz Posted at: 2018-10-14T21:03:25.567Z Reads: 98

```
Man tells us how you made it fit your wheels etc.
```

---
## \#54 Posted by: TowerCrisis Posted at: 2018-10-14T21:24:17.186Z Reads: 103

```
Alright, I'm going to include an extensive write-up here and put it in an edit in the original post for any newcomers.

**HTD VS GT2**

Here are some direct comparisons followed by interpretations of the data.

**General Lifetime:**

![Durability|690x322](upload://vmeDmCXk5UdpbR9TDgjcjuzyN9G.png) 
This is the general lifetime testing of the different belts. Each test was conducted with the same pitch, pulley sizes, speeds, and torque. It concluded upon belt replacement was necessary, or until enough data was collected (no need to go further, in the case of GT). The baseline for these tests was the HTD performance, set at 100%. These tests were conducted at speeds and pulley sizes that result in accelerated belt wear, which will be explained further down this post. **GT 5M has nearly 190% the lifespan of HTD 5M.**

**Tooth Jump:**

![Tooth%20Jump|690x430](upload://42YuYD2Yv9YS2ftFRV0oJ6eAYHJ.png) 
These results are not particularly favorable for GT 5mm pitch, at least upon first glance. HTD and GT seem to be very similar in the 5mm pitch, however it is important to see that this **test was only tested up to 2300 RPM, while we typically run our motors around 6000 rpm**. This results in much worse tooth skip, as it is far beyond the specifications of the tooth profiles. This higher rpm with higher torques is where GT shines greatest, and as you can see GT and HTD profiles begin to diverge as installation tension decreases. We run our tension somewhere in the 2-3 lb range. Some with idlers as low as 0 or 1 lb of tension.

**Operating Belt Tension:**

![Belt%20Tension|690x432](upload://ox5wgUr0UhRd7JBzrCSEXwReWGT.png) 
Here is the exact maximum belt specification for the tension on the taut side. For explanation's sake, I'm going to divide numbers by 2, so the belt width is equal to 12.7mm, which is close to our use case. **HTD 5M is rated at 51 lbs of tension. GT is is rated at 80 lbs.** Please note that this is independant of ratcheting or pulley size, this is only the maximum allowable tension on the belt.

**Minimum Pulley Size Per RPM Unit:**
![Pulley%20Size|349x500](upload://9v7Hy8wuQdsLLPtnBPpFxC7GHZi.png) 

This is fairly straightforward. A 22 tooth HTD 5M pulley is rated to operate at 1160 RPM. **This is over 5 times less than the 6000 rpm we operate at.** A 22 tooth GT 5M pulley is rated to operate at 2000 RPM. Again, we are far out of spec, but by much less. **This is 3 times less than the 6000 rpm we operate at.** Unfortunately, **both will experience accelerated wear, but HTD will suffer much worse**.

**Exact RPM And Torque Ratings:**

![HTD%20torque|457x500](upload://al5e5s8J82oxbHrNzPdQWvIkFXI.png)
![GT%20torque|446x500](upload://xQJ4ZwLPpqXldzLSo0qniXtcY1B.png) 

These graphs show the operating RPM and torque ratings. **HTD 5M is rated to 75 in lbs of torque at 6000 RPM. GT 5M is rated to 250 in lbs of torque.** This means that GT 5M can run at **3 times the torque** of HTD 5M. While we are not typically exceeding these, it still means that GT will suffer much less wear over time. Please note that this data is unrelated to pulley size, that data will come next and will show further disparity between HTD and GT.

**Exact Torque Ratings Per Pulley Tooth Count:**

![HTD%20exact%20torque%20and%20lifetime|690x413](upload://ygHvQm97uafduIdtbhiyt3qZcQ8.png)
![GT%20exact%20torque%20and%20lifetime|678x500](upload://fbRtJWSvGaifurH8tVLaWgJP7aQ.png) 

I'm going to use the math for 5000 RPM, as it is the closest common value to 6000 rpm between the two graphs. **HTD 5M is rated to 11.6 in lbs of torque with an 18T pulley. GT 5M is rated to 25.2 in lbs of torque with the same rpm and pulley.**

What is more interesting is the low RPM values. **At 100 rpm, HTD is rated to 25.7 in lbs of torqe, while GT is acceptable up to 58.5 in lbs** with an 18T pulley. Our intense startup torques far exceed HTD specifications.

However, HTD is already in the "accelerated wear" category all the way up to 28T pulleys at 5000 rpm. HTD suffers from excessive wear from an 18T pulley at any rpm of 1160 and up. GT is acceptable wear at 5000 rpm at any pulley size 18T and up. GT is functional from 200 rpm to 14000 rpm with an 18T pulley. It only suffers from excessive wear from 100 rpm and lower, which we are rarely in when riding. For a visualization, this is when the motor makes a full turn every .6 seconds, which is a very slow creep for us.

We will be exceeding the torque ratings of these, so GT will also suffer accelerated wear, but not nearly to the extent of HTD since it is already going to wear excessively at any torque.

**Other Details, Unrelated to Performance:**

**Ignore this if all you care about is raw performance, only the above information will be relevant to you.**

![Sound|690x461](upload://cBBQjS7dKpfShHPlKgLUxnvlYFC.png) 
The sound levels are not easily interpreted from this. Decibels are determined on a logarithmic scale, not linear. So 100 dBA is much more than 2x louder than 50 dBA. GT is significantly quieter than HTD.

![Idler%20Size|690x230](upload://bb2cQLZPjjtidkLTb00JHXWOZZ8.png) 
We use backside idlers. GT and HTD perform the same here, but the data shows that we are seriously exceeding the spec here lol. Reversed bend radius very negatively affects belt life (given that all other wear factors are already in spec. We use idlers so other factors like belt slippage don't occur, which is objectively a greater concern for wear).

**Totally random thing I found about belt movement that I thought was kinda neat:**
![Interesting%20detail|690x365](upload://mZunUhHb9B2r4OejzGlAuMMIsbn.png) 

I found this very interesting. In a tuned pulley setup where they are in line and not twisted of offset at all, the belt will always ride to one side. If you have a precision CNC'd motor mount setup that ensures your pulleys are properly lined up, then you will still suffer from belts moving sideways. It is dependant on the direction the fibers internal to the belt are twisted. S twist is the opposite of Z twist. So if you're using two of the same belts, they will both move in the same direction, ie: one will move away from your truck and the other towards it. Just thought this was interesting to read about.

**TLDR:**
All Gt profiles are far superior to HTD, particularly in lifespan, torque ratings, and rpm. If you want a quick interpretation of the data, here is a comparison of many profiles:
![In%20Conclusion|690x305](upload://fKrxnBIrEEFn6spBHNLKpjl6nZj.png)
```

---
## \#55 Posted by: Benjamin899 Posted at: 2018-10-14T22:39:36.451Z Reads: 92

```
![aDVMj3nN_700wa_0|261x200](upload://j48LBv5P7yUFBhR8t6YKMTTtr2o.gif)
```

---
## \#56 Posted by: rojitor Posted at: 2018-10-14T22:40:10.380Z Reads: 93

```
Neat and thorough
```

---
## \#57 Posted by: Benjamin899 Posted at: 2018-10-14T22:46:34.817Z Reads: 92

```
well if i build a board with belt again i guess it is time to switch. but first i will build a direct drive.
```

---
## \#58 Posted by: jmasta Posted at: 2018-10-15T02:16:40.599Z Reads: 94

```
I've been using 5mm GT2 for 2 years now
```

---
## \#59 Posted by: lrdesigns Posted at: 2018-10-15T02:34:12.156Z Reads: 97

```
[quote="jmasta, post:58, topic:71058, full:true"]
I’ve been using 5mm GT2 for 2 years now
[/quote]

Where do you get them from?

Edit. My usual source has a GT variant of the HTD I normally get. See comparison below. Im no expert on how to read the specs but is this better? Breaking strength is similar but working tension is much higher, what does it mean? I need an engineer. :man_teacher:

[HTD](https://www.aliexpress.com/item/5pcs-lot-5M-synchronous-belt-265-5M-15-teeth-53-Rubber-width-15mm-length-265mm-HTD265/32257812576.html?spm=a2g0s.9042311.0.0.637b4c4deW2OIa)
[GT](https://www.aliexpress.com/store/product/High-Torque-GT2-Timing-belt-Pitch-2mm-0-079-Neoprenen-with-fiberglass-Customizing-all-kinds-of/702327_32245725336.html?spm=2114.12010612.8148356.10.28b859003FvOsX)

![image|690x434](upload://n1msD8kwlMLX0fm8kdtmx1JflwI.jpeg) 
![image|690x480](upload://uAgAbyrfIGaAwdbp5GTYVPtVT0V.jpeg)
![image|690x325](upload://kQg5U9ufb80M5iV6RINRpuIkJw7.jpeg)
```

---
## \#60 Posted by: TowerCrisis Posted at: 2018-10-15T06:16:19.978Z Reads: 96

```
Breaking strength doesn't really matter for our case. The breaking strength of 12mm belt is nearly 850 lbs! We will never reach that kind of tension, you will lose traction before that happens. Notice that the rating is followed by "not representative of the load-carrying capacity" ie: the belt will not operate properly at this tension.

What is a concern though is the working tension. This is how much tension the belt can have in one direction and still mesh properly with a pulley at speed. That specification isn't complete, the working tension should be affected by many other factors such as belt surface speed, fastest pulley RPM, and pulley size.

A specification of 712N or 454N is meaningless without the corresponding RPM and pulley size.

If you're having issues with excessively fast belt wear or belt slippage on HTD, a GT belt could solve your problem.

I would recommend buying belts from SDP-SI.com They have many sizes and types of belt, all manufactured by Gates themselves.
```

---
## \#61 Posted by: Okami Posted at: 2018-10-15T06:26:39.820Z Reads: 95

```
One thing I saw a while ago was that htd5 indeed doesnt match our rpm needs and power ratio intended.. 


I think it was somewhat around 2kw and 5000rpm (in chart seller provided) after that it goes out of its recommended use range.

@Duffman also used different belts/pulleys, if i remember correctly
```

---
## \#62 Posted by: Eretron Posted at: 2018-10-15T06:40:36.953Z Reads: 94

```
Evolve boards are using GT3 pulleys and belts originally, but I've used HTD5 belts without even knowing that there is a difference. 🤦‍♂️

Now I am a bit concerned regarding rpm on those belts.
```

---
## \#63 Posted by: TowerCrisis Posted at: 2018-10-15T06:41:39.103Z Reads: 91

```
If the belt's aren't skipping, the biggest risk you're running is dramatically reduced belt life. But that's about it.
```

---
## \#64 Posted by: Maxid Posted at: 2018-10-15T07:05:27.991Z Reads: 94

```
I assume those numbers are only when using the corresponding pulleys. Do you know the effect of using a GT3 belt with HTD pulleys? Will there be an improvement in terms of less belt skipping etc. as well or is the belt/pulley combination the most important part?

Edit: according to this http://www.pfeiferindustries.com/documents/Timing%20Belt%20Tooth%20Profile%20and%20Pitch%20(Interchangeability).pdf
a so called RPP (Reinforced Parabolic Profile) belt is also compatible with HTD pulleys. Is an RPP better than GT3?

Edit2: Well looks like using a GT2 belt on a HTD pulley is actually not a good idea (at least at 5M pitch)
https://www.klee.dk/wp-content/uploads/2014/12/Hvilke-remme-passer-til-hvilke-skiver.pdf
I am not sure who to trust though as this document even says an RPP is not recommended to be used with HTD pulleys while the other link shows the RPP to be a drop-in replacement for HTD belts.
```

---
## \#65 Posted by: TowerCrisis Posted at: 2018-10-15T07:28:48.590Z Reads: 94

```
Gates has cited:

• Reduced performance
• The sprocket/bushing capacity may be
too low for new designs

Which equates to reduced belt life (I'm speculating not nearly as bad as HTD currently lasts, since we're overloading HTD so much).

And that pulley systems currently designed for HTD belts may not be strong enough for the load capacity of GT2 belts. This essentially confirms that using a GT3 belt will increase available torque.

Typically in a drive system the belt is the weakest link, so in the case of failure or lockup of some sort many designs will rely on that belt breaking. If the belt doesn't break, it could supply excessive torque and damage other systems. This is not true in our case as we aren't shearing pulleys off of wheels or motors.


[details="This hidden statement was incorrect, my bad."]
I'd also like to point out that the document you linked says nothing about GT2 belts on HTD 5M pulleys, it only says not to use GT2 8M and GT2 14M on equally pitched HTD pulleys.
[/details]
```

---
## \#66 Posted by: Maxid Posted at: 2018-10-15T07:32:57.971Z Reads: 93

```
[quote="TowerCrisis, post:65, topic:71058, full:true"]
I'd also like to point out that the document you linked says nothing about GT2 belts on HTD 5M pulleys, it only says not to use GT2 8M and GT2 14M on equally pitched HTD pulleys.
[/quote]
It says not to use a 5M GT2 belt on a HTD5 pulley - or am I reading this wrong? :thinking: 
![image|399x500](upload://wSNzpROsQK5LQDjRGXOkShEBkrE.jpeg)

Edit: checked again and it is actually the other way around int he document. HTD5 should NOT be replaced with 5MGT2 while 8M and 14M apparently can be replaced.
```

---
## \#67 Posted by: TowerCrisis Posted at: 2018-10-15T07:41:57.230Z Reads: 91

```
My bad! I must've missed that page, my apologies. 

Anyways, yes it is "not recommended" however it is not "not compatible"

What's important to distinguish is that "not recommended" is defined as having potentially reduced service life, or if a different product line is more suitable. I'd say it's fair to conclude that it isn't too bad (I've personally used GT2 belts on HTD pulleys many times before, not on a skateboard though) and that it's mostly designated as not recommended because HTD is more suitable for HTD pulleys. 5M HTD differs from 5M GT2 more than the other pitches of GT2 and HTD, so it makes sense that they wouldn't recommend it.
```

---
## \#68 Posted by: Maxid Posted at: 2018-10-15T07:47:16.006Z Reads: 94

```
I just find all this information very confusing.
One document shows the belt to be perfectly fine to use while the next does not recommend exchanging them. Then we have the situation where we are actually exceeding the HTD specifications which in turn however could mean that a previously not recommended belt is in fact the better option. Also what happens then if we only rarely exceed the HTD specifications (during acceleration etc.) and most of time stay in spec when cruising. It's just so much to consider...
:exploding_head: 

Do you know of any science papers on this that might shine some light? I can somehow only find very little documentation online.

Edit: I checked out a German [book on belts by Raimund Perneder](https://books.google.de/books?id=e2U0lMIy1D0C&pg=PA20&lpg=PA20&dq=zahnriemen+profile+gt3+htd&source=bl&ots=pH96AJPhm7&sig=puJy9oZCJgTCR8_4d0iF-swfrp8&hl=de&sa=X&ved=2ahUKEwjuw7DR_IfeAhWGxIsKHUBvDic4HhDoATAAegQIChAB#v=onepage&q=zahnriemen%20profile%20gt3%20htd&f=false) that also says:
GT3 belts with 2, 3 and 5M pitch are only compatible with GT3 pulleys. Only pitch 8 and 14 are usable with HTD pulleys.
```

---
## \#69 Posted by: TowerCrisis Posted at: 2018-10-15T08:11:40.446Z Reads: 92

```
[quote="Maxid, post:68, topic:71058"]
we have the situation where we are actually exceeding the HTD specifications which in turn however could mean that a previously not recommended belt is in fact the better option. Also what happens then if we only rarely exceed the HTD specifications (during acceleration etc.) and most of time stay in spec when cruising. It’s just so much to consider…
[/quote]
basically... yeah. There are some boards that will always exceed the HTD spec when going at higher speeds, and there are some that won't. But I can guarantee you that nearly all exceed spec on high acceleration.

@Brdchris and  @PXSS wanna share some more details of your builds? What kinda ratios, motors, etc are you using? PXSS are your GT3 belts on HTD pulleys or did you manage to find GT2 pulleys? If they're on HTD, how would you describe the tooth mesh?
```

---
## \#70 Posted by: Okami Posted at: 2018-10-15T17:39:17.333Z Reads: 92

```
I found in duffmans thread he used AT5/T5 belts:

[quote="Duffman, post:15, topic:17143"]
initially used HTD5m belts in 15mm width could not hold up against the motors and got ripped every 10 km. Therefore I tried T5 and AT5 belts, which have 2x / 3x the tensile strenght of HTD. Even more important is that they don’t fail instantly like HTD, but get louder and louder, loose teeth or get spliced and remain still rideable for tens of km.

[![|340x191](//www.electric-skateboard.builders/uploads/db1493/optimized/3X/9/b/9bffa33c6ea2bda2f23bf0f51988cae1dc97cdf8_1_345x194.jpg)](//www.electric-skateboard.builders/uploads/db1493/original/3X/9/b/9bffa33c6ea2bda2f23bf0f51988cae1dc97cdf8.jpg)
[/quote]
```

---
## \#71 Posted by: Boardnamics Posted at: 2018-10-15T19:31:43.810Z Reads: 94

```
HTD belts cannot be used on gt2 pulleys and vise versa. You CAN do it, definitely. I have tried. But the performance and service life will suffer. The ideal solution is gt pulleys with gt3 belt. Gt2 and Gt3 have the same profile, the only difference being Gt3 belts (from Gates) are made with improved materials.

The only way esk8 could benefit from this is if our pulleys were made with the gt profile, otherwise forget it.

Oh and: 
The performance and reliability of your belt has much to do with how you're using it as much as what belt system it is. HTD with excellent for many people and doesn't work at all for others. Alignment, running conditions, pulley runout and material, all play a role here. The answer is not as clear cut as a graph from SDP-SI wants it to be
```

---
## \#72 Posted by: PatRocks Posted at: 2018-10-15T23:46:00.721Z Reads: 88

```
@TowerCrisis bravo on your contribution above, easily the most interesting read I've had in weeks. Thank you
```

---
## \#73 Posted by: PatRocks Posted at: 2018-10-17T17:41:47.456Z Reads: 91

```
Anyone able to find a source for these types of pulleys? Just searched for 30min and no luck 😡🤬

Edit: for motor pulleys
```

---
## \#74 Posted by: Benjamin899 Posted at: 2018-10-17T17:46:44.931Z Reads: 92

```
rly? 5 sec search on ebay
https://www.ebay.de/sch/i.html?_from=R40&_trksid=p2380057.m570.l1313.TR12.TRC2.A0.H0.Xgt3+8mm+pulley.TRS0&_nkw=gt3+8mm+pulley&_sacat=0
edit: nvm they are the wrong ones mostly.
```

---
## \#75 Posted by: rojitor Posted at: 2018-10-19T14:45:24.518Z Reads: 80

```
![IMG_20181019_163047|375x500](upload://mVxKOQoQ2pBeS8wuxxahfwlw0Hx.jpeg) 
I got my GT3 belts today. I am no expert at this but i have a couple eyes in my face....
They look 100% compatible with htd to me.
I am busy today but i will test them on my trampa, let's see the difference.
```

---
## \#76 Posted by: rojitor Posted at: 2018-10-19T19:50:08.322Z Reads: 78

```
I just went to the park on my trampa for a test ride. I was really unlucky tho. The cops were bored to tears and decided to tag me(it's illegal here) so i had to escape from them, ride slowly and try not no draw attention. Even like that i managed to climb a steep hill, sprint a lane and test brakes.
I didn't notice a better torque but the brakes somehow work better.
Please don't take my opinion as a reference because i just had a lousy ride with the cops on my butt. Right now i think it's totally worth It if you have no belts, the upgrade is not worth It if you have small pockets. That's just my first impression, i could find cheaper belts and change my mind so again, don't mind my opinion.
```

---
## \#77 Posted by: trancejunkiexxl Posted at: 2018-10-19T21:43:32.314Z Reads: 77

```
when in doubt just dip out!! :stuck_out_tongue_winking_eye:
```

---
## \#78 Posted by: PatRocks Posted at: 2018-10-19T21:58:41.259Z Reads: 81

```
Glad you evaded the cops!! Based on the above information, I would think that the motor pulleys in the gt2/3 profile will have the most significant impact on performance, no? I've only seen teeth skip on the motor side...
```

---
## \#79 Posted by: rojitor Posted at: 2018-10-19T22:03:33.558Z Reads: 82

```
I also wonder how the performance would change using GT3 motor pulleys
```

---
## \#80 Posted by: biggdaddyhawk Posted at: 2018-10-19T22:49:01.838Z Reads: 84

```
Interesting topic... the science seems convincing. Has anyone ever bought the upgraded htd5 Kevlar belts.They were more money than the regular ones so I didn't try them.
```

---
## \#81 Posted by: Boardnamics Posted at: 2018-10-21T07:16:51.079Z Reads: 81

```
The gt3 belts do not fit perfectly on htd. It could be because your pulley is 3d printed so the profile isn't perfect, but I have matched them up and there is a difference. There is more clearance between the bottom of the tooth and the belt tooth itself, so the stress isn't carried as good.

You should test it though
```

---
## \#83 Posted by: epster Posted at: 2019-09-30T12:48:25.905Z Reads: 34

```
Year later and still no one used HTD belts sad thing to see.
```

---
## \#84 Posted by: TowerCrisis Posted at: 2019-10-22T06:10:16.965Z Reads: 27

```
Not sure what you mean by that, almost everyone uses HTD.

Just a quick update for everyone: I'm using GT3 3M, 15mm wide belts on a 60:28 reduction with idler. Have never skipped a tooth and the belts still look brand new after 100+ miles.
```

---
## \#85 Posted by: TheSebas Posted at: 2019-10-22T07:48:13.387Z Reads: 29

```
Where did you get a gt3 profile pulley?
```

---
## \#86 Posted by: TowerCrisis Posted at: 2019-10-22T08:06:35.186Z Reads: 29

```
I ordered the motor pulleys custom from B&B manufacturing. They custom hobbed them (not a stocked size, 28T), put a 3mm keyway, and two setscrew holes. Fully steel. Same silver colored with a rust protective coating and oil.

Their pricing when I ordered was:

$59 unit price for 4

$38 unit price for 8

$7.75 unit price for 1000

Quite cheap if you're buying in bulk. My guess is price wouldn't go above $10 for 200 of them.


The motor pulley was 3d printed on a SLS machine. I grabbed the initial tooth profile from SDP-SI.com . They have free cad if you sign up. Be weary of their HTD profiles though, some of them seem wonky with inconsistencies. GT3 and GT2 are both good though.
```

---
## \#87 Posted by: epster Posted at: 2019-10-23T08:03:37.564Z Reads: 24

```
Sorry meant gt3 haha my bad
```

---

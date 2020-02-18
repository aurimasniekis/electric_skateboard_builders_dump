# 12S vs 10S for new builders

### Replies: 43 Views: 1865

## \#1 Posted by: Brendan Posted at: 2018-11-24T03:48:12.646Z Reads: 414

```
Hi, I ordered my stuff for my first build today, but the last remaining variable for me is the battery. I'm not sure if I want to go with a 10s5p or a 12s4p. It's going to be attached to dual 6374s from bkb and two focboxes. I'm leaning towards the 10s5p just because I'm afraid of frying the focboxes. I may be misunderstanding something but it seems that running a 12s4p battery on focboxes in foc is flirting with the limits of the capabilities of the ESC. I'd love to have something capable of that extra speed though. Am I analyzing this situation right?
```

---
## \#2 Posted by: accrobrandon Posted at: 2018-11-24T03:58:19.426Z Reads: 412

```
12s is fine... this was my dilemma earlier in the year on my first build... i went 10s and it was great.. then when I slapped in a 12s theres no way Im going back to 10 unless space is an issue or some other factor.... the extra voltage  is nice and as many have said, but doesn't make sense till you have ridden both, 12s has less noticeable sag...

the bottom of a 12s charge rides like a 10s at 80% IMO
```

---
## \#3 Posted by: ksfacinelli Posted at: 2018-11-24T04:03:31.075Z Reads: 405

```
I would go 12s4p have both and from my opinion the 12s has a bit more kick and run dual Foxboxs and have not had any issues.... you should check out @psychotiller for your battery uses 30Q and I have two and no issues.. solid and when I compared pricing a very good deal.
```

---
## \#4 Posted by: Brendan Posted at: 2018-11-24T04:07:15.206Z Reads: 391

```
Thanks for the input man!
Any particular guides you used to make sure you didn't fry the focbox? I've watched a few guides but nothin specifically for a 12s on a focbox. I've never programmed an ESC so its a bit freaky playing with that kinda fire your first time
```

---
## \#5 Posted by: Brendan Posted at: 2018-11-24T04:08:57.479Z Reads: 371

```
Thanks man! Do you happen to know a guide or setting list to avoid frying the DRV?
```

---
## \#6 Posted by: accrobrandon Posted at: 2018-11-24T04:12:59.879Z Reads: 364

```
i mean everyone is gonna have their fav settings... vesc tool is pretty easy to use and does all the work for you so i recommend it... off the top of my head on a 4p 30q i think i run

60, -60 on motors and
30, -10 on the battery

i have dual 6355 at 15/36 on 107 and its has great pull and speed... i had 18/36 and still great torque and top end was supposedly mid 40s mph but i dont have riding gear to test the limits but i do frequently ride in the 30+ range comfortably for sure
```

---
## \#7 Posted by: ksfacinelli Posted at: 2018-11-24T04:13:34.651Z Reads: 348

```
I think the DVR issue is when you go over 6000rpm...The settings I have used depend on the build however in general don't go 60A battery and depending on motor 60A to 80A...
```

---
## \#8 Posted by: Brendan Posted at: 2018-11-24T04:24:06.701Z Reads: 334

```
Alright so now I am leaning towards 12S, I'm gonna keep researching this DVR issue thing and hopefully I can find a guide on what the safe parameters to enter in the VESC program will be for my set up.
```

---
## \#9 Posted by: ksfacinelli Posted at: 2018-11-24T05:03:07.685Z Reads: 325

```
Make sure you know you are getting a quality battery with good cells and reputable BMS it is your power plant....and a quality product will perform well for a long time,,,,one that is less quality you roll the dice, not to mention you could experience a fire department call not to scare you but in this case you really get what you pay for...the Enertion Focbox product is solid and used by thousands of riders..If you have time I would wait for the Unity controller as Jeff @Deodand is an amazing engineer and do a little research and I think you will agree.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-11-24T07:13:35.752Z Reads: 295

```
The problem is not the erpm.
Focbox can handle save 100000.
The problem is that voltage spikes can occur which could exceed 60V more easy with 50,4v instead of 42v.
This voltage spikes will fry you esc sooner or later.
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-11-24T07:15:18.862Z Reads: 284

```
10S if u want to be safe. 

12S if u wanna push it and go faster.
```

---
## \#12 Posted by: Psmrman90 Posted at: 2018-11-24T07:15:23.427Z Reads: 280

```
Not to throw a wrench in your progress deciding, but BKB has an 11s too. Middle ground of 12s and 10s, goldilox zone if you want it.
```

---
## \#13 Posted by: Brendan Posted at: 2018-11-24T07:19:19.600Z Reads: 276

```
Fair enough, but I have full gear and a smooth, straight path to unleash this thing on. I just want to know if there's a way I can do 12s and 6374 motors without risking the destruction of my focbox, and if so what those settings are
```

---
## \#14 Posted by: taz Posted at: 2018-11-24T07:37:02.426Z Reads: 272

```
Many people (myself included) run 12S on Focboxes with no problems.
Some have even run 13S with no problems.
IMO keep the motor amps to 60A, maybe lower depending on your motors and the temperatures they are reaching, braking amps the same (I use -40A since I prefer it). 
Battery amps depend on your battery (and BMS if you discharge through it). I use 40A per esc.
Battery regen -10A but you can go a lot higher since it will probably never happen and if it does it will be for such a short period of time and will not harm your battery.
That said I can understand the point of view of people that believe that a bigger safety factor should be employed and that 12S is close to the 60V max of the Focbox. However empirical evidence says you are more likely to destroy your Focbox through some sort of user error than 12S.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-11-24T07:38:14.092Z Reads: 254

```
What he ☝️ said 😅
A lot of people run 12s on focboxes.
Just be sure there is a risk that you fry them sooner or later.
The settings not causing the voltage spikes.
Long and too slim cables more a reason for it.
```

---
## \#16 Posted by: Bjork3n Posted at: 2018-11-24T08:08:28.356Z Reads: 252

```
I was also under the impression that 12s is risky. My last build was 10s had no issues for over 1000km but friend's using 12s had some minor issues.
12s and Foc seems to be what is causing issues for most. 12s and Bldc seems safer from what I understand. 
I don't want any problems so i went with 10s again since it worked great last time 👍
```

---
## \#17 Posted by: Schulerbible Posted at: 2018-11-24T08:31:33.465Z Reads: 253

```
People have utilized the power of 12S on the old Vescs, just saying.
```

---
## \#18 Posted by: pat.speed Posted at: 2018-11-24T11:41:29.326Z Reads: 241

```
Yeah I run 12s on Torqueboards vescs and it runs fine, no issues. I do have an extended capacitor bank of something like 13000uf, which helps reduce voltage spikes. I also run 58k erpm limit and only 45, -45 motor amps and 30, -5 battery amps. I am a light rider and have a high gear ratio so I get good torque even with low settings
```

---
## \#19 Posted by: AndresIGC Posted at: 2018-11-24T13:52:37.689Z Reads: 227

```
Planning a very similar build, how many kv are your motors?
```

---
## \#21 Posted by: Brendan Posted at: 2018-11-24T19:41:38.212Z Reads: 218

```
190 kv. Here are my motors in case you’re looking for some. Seems like a great deal. https://buildkitboards.com/collections/black-friday/products/6374-190kv-motor
```

---
## \#22 Posted by: Brendan Posted at: 2018-11-24T19:43:22.786Z Reads: 213

```
I was hoping to use FOC, I could be wrong but I read somewhere that I cant set an ERPM limit. Could be that I have to compromise, either FOC or 12S but not both.
```

---
## \#23 Posted by: Michael319 Posted at: 2018-11-24T19:46:09.223Z Reads: 215

```
If your build is set up correctly then you don't need an ERPM limit. I run 12s 6374 149kv I think and I don't need an ERPM limit on foc
```

---
## \#24 Posted by: Brendan Posted at: 2018-11-24T21:03:28.980Z Reads: 209

```
Well I plan on having pretty short cables and just connecting everything together on the back end of a long single enclosure that I'm buying from psychotiller, and I'm gonna use the BKB antispark switch. Any tips on pitfalls to avoid to make sure this is set up correctly?

I'm thinking I'll go with: 

Motor Max 80A
Motor Min -65A
Battery Max 40A
Battery Min -20A
```

---
## \#25 Posted by: Eboosted Posted at: 2018-11-24T22:42:42.881Z Reads: 201

```
Focboxes do not fry at 12s, the 12s fear is part of the past, only Chinese ESCs are prone to fail on 12s
```

---
## \#26 Posted by: murdomeek Posted at: 2018-11-24T23:34:13.211Z Reads: 195

```
whats the difference between 12s
and 10s with faster pulley gearing?

is 12s just higher speed?
```

---
## \#27 Posted by: torqueboards Posted at: 2018-11-24T23:36:10.875Z Reads: 192

```
12S is best! :stuck_out_tongue_closed_eyes:
```

---
## \#28 Posted by: pat.speed Posted at: 2018-11-24T23:38:46.860Z Reads: 193

```
12s will be faster and have more torque
```

---
## \#29 Posted by: accrobrandon Posted at: 2018-11-25T00:00:07.228Z Reads: 193

```
its the extra voltage... its like a small turbo vs 10s =)
```

---
## \#30 Posted by: murdomeek Posted at: 2018-11-25T06:41:28.905Z Reads: 188

```
is running 12s at 80% top speed (or whatever it is to make it equivalent top speed of 10s), more, less, equal efficiency than running 10s?

Will the battery life last longer or shorter or negligible? (assuming all else equal. 12s4p vs 10s5p)


I always thought 10s5p would get more range, but if i never max out the throttle, might as well go 12s for the rare times I need it?
```

---
## \#31 Posted by: y.k Posted at: 2018-11-25T07:19:47.131Z Reads: 177

```
i have a 8s2p 2600ma 5C li ion battery pack.i want to configure my vesk.
 what i fill in the Max amper blanket?
```

---
## \#32 Posted by: Vanarian Posted at: 2018-11-25T09:31:16.405Z Reads: 176

```
Wh is Wh so as long as your setup keeps similar efficiency, your range will be the same.

But at 12S you might draw more power easily if you use the same VESC settings (batt max motor max etc)
```

---
## \#33 Posted by: Bjork3n Posted at: 2018-11-25T12:29:38.034Z Reads: 170

```
I also must say that 10S is more than enough for a first build. 
The performance you can get from 10s is not bad, sure 12s may be better but honestly when can you use that power to its full potential?
On my previous build i used a 10s4p and had it setup to draw 60A motormax and 30A batterymax and the performance on 90mm wheels with 16/36 gearing was great...topspeed was 46km/h
When i tried 80/40 on the settings it was crazy fast.

The majority of my friends had issues with 12s sure it may be user error and such but we use almost the exact same settings and i had no problems on 10s and they had a fair bit.

This is a acceleration test from 2km/h to 46km/h on my previous build with dual 6355 just to give you an idea of the performance. (settings on the focboxes 60/30A)
https://www.youtube.com/watch?v=90DWXmj55_g
```

---
## \#34 Posted by: MannyM0E Posted at: 2018-11-25T17:17:38.647Z Reads: 163

```
I’m also curious about 12s. On my first build I went 9s Lipo then eventually went with 30q 10s4p. I like it, rode a friends kaly board that’s 12s and OMG I feel in love. Just finished a 12s6p, almost done with a emtb project just waiting on enclosure to finish. Looking forward to 12s 😊
```

---
## \#35 Posted by: Eboosted Posted at: 2018-11-25T23:34:30.298Z Reads: 158

```
[quote="murdomeek, post:26, topic:75798, full:true"]
whats the difference between 12s
and 10s with faster pulley gearing?

is 12s just higher speed?
[/quote]

If you keep the same amount or parallel cells, the only difference would be more capacity in Whr on the 12s
```

---
## \#36 Posted by: MrGSR Posted at: 2018-11-26T12:14:39.150Z Reads: 150

```
Our best comparison is Watt hours.
10s5p= 36V, 15000mAh, 540Wh nominal
12s4p= 43.2V, 12000mAh, 518Wh nominal
 Assuming 30q batts. 
           Formula is (mAh)×(V)÷1000=(Wh)
My opinion, 12s is more  FUN.
```

---
## \#37 Posted by: linsus Posted at: 2018-11-26T15:51:53.900Z Reads: 145

```
12S Will give you greater benefit on bigger wheels such a pneus. You'll need every bit of extra power you can get. For a normal streetbuild with smaller wheels 10s is enough. 12S with dual 6374 on 80mm wheels is scary if u ask me...Rides well on my trampa with pneus however.

For a given setup, 12S will generally generate less heat(losses) than a 10S setup. It's not alot, but its there. A factor most dont think about.
```

---
## \#38 Posted by: ThermalChild Posted at: 2018-11-26T16:07:49.245Z Reads: 143

```
I'm running dual 200KV 6374's 10s4p with 16/38 on boa's with pretty high settings and it'll put you on your ass if your not careful. The same with my 16/62 on trampa 6.5's. Never tried my caguamas though.
```

---
## \#39 Posted by: Bjork3n Posted at: 2018-11-26T16:35:54.462Z Reads: 141

```
Less heat with 12s is not my experience, I read it on here all the time but my friends running 12s has substantially higher heat than me running 10s on same settings. 
I'm confused 😩
```

---
## \#40 Posted by: UKRider Posted at: 2018-11-26T19:20:41.473Z Reads: 127

```
Interesting, conversation. 

I'm upgrading from LIPOs to Li-Ion, I'm thinking going **10S4P**.  I have dual 6354 190KV, 15 teeth motor pulley and 36 teeth in wheels. 90mm wheels and weigh about 90KG. Street riding with some hills but nothing extreme.  How many miles can I expect in range??

Maybe I will go 12S4P or even 10S5P. But if I can get 15 miles in 10S4P I'm happy.
```

---
## \#41 Posted by: linsus Posted at: 2018-11-26T20:33:18.742Z Reads: 121

```
It depends on more than 12S, gearing ratio and kv on motor plays a big part as well. They prob have less ratio and/or higher kv then
```

---
## \#42 Posted by: linsus Posted at: 2018-11-26T20:34:02.273Z Reads: 122

```
Google esk8 calculator
```

---
## \#43 Posted by: Bjork3n Posted at: 2018-11-26T20:49:50.703Z Reads: 120

```
Nope they have the same gearing and kv. They do however use 97mm and I use 90mm. 
They are up at 70-80c quite often and I never reachd higher than 68c
```

---
## \#44 Posted by: linsus Posted at: 2018-11-26T20:53:58.855Z Reads: 118

```
That would be it then, 97xpi vs. 90xpi. Thats the difference on one spin. Belt tension, motor size and cabling length play a role as well
```

---

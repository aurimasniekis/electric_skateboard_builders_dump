# 10s6p vs 12s5p can&rsquo;t decide

### Replies: 78 Views: 1223

## \#1 Posted by: SynteX Posted at: 2019-01-13T22:33:27.831Z Reads: 290

```
Hey Guys,

I've got a trauma over here with 4x3s 8000mah lipos.
It is time for a battery upgrade to Samsung 30q since I don't trust lipos that much.

I can't choose between a 10s6p pack or a 12s5p pack.

I am running a dual motor set-up with 2 149kv sk3 motors. With E-toxx system(direct drive?)

Use 2 focboxes.

Also any safety tips configuring the focboxes? With this kind of pack? Or isn't it anything special?

![20181216_100230|375x500](upload://traoN7SH4TEUM7jAJyuMb8rqv9D.jpeg)
```

---
## \#2 Posted by: Alex753 Posted at: 2019-01-13T22:36:30.196Z Reads: 273

```
Hello ! 

You need to choose between speed or range, 10S6P should give you more range but a lower max speed than a 12S5P.

Generally the type of Esc is a good help because some of them may not handle 12S for a long time use but I think that focboxes can manage it.
```

---
## \#3 Posted by: pat.speed Posted at: 2019-01-13T22:37:15.286Z Reads: 274

```
12s5p is the choice for you, same if not better range, faster top speed, more efficient, less amps required, running closer to motor efficiency range of 8k rpm and more punchy torque.

However 10s is more reliable
```

---
## \#4 Posted by: pat.speed Posted at: 2019-01-13T22:38:33.443Z Reads: 267

```
Wrong! they have the same amount of cells in the packs therefore the same Watt hours, therefore the same range. However 12s will use less amps due to higher voltage meaning more range.
```

---
## \#5 Posted by: Alex753 Posted at: 2019-01-13T22:40:10.768Z Reads: 260

```
Well I didn’t know that, really interesting thank you !
It’ll help me to choose my battery update too !
```

---
## \#6 Posted by: pat.speed Posted at: 2019-01-13T22:40:57.185Z Reads: 258

```
Whenever comparing batteries with different voltages Ah is irrelevant. It’s always about Wh
```

---
## \#7 Posted by: SynteX Posted at: 2019-01-13T22:45:23.098Z Reads: 251

```
Thanks. But i have to make sure focbox can handle this.
```

---
## \#8 Posted by: dareno Posted at: 2019-01-13T22:52:29.012Z Reads: 249

```
[quote="pat.speed, post:3, topic:80810"]
However 10s is more reliable
[/quote]

I'd question that statement.  So long as you use the correct vesc then there is nothing wrong with 12s reliability.  See me being me would run a 10s 4p pack at max amps and then ride it like I stole it.  With the 12s 4p to get the same punch the current can be lower and therefore less stressful on the set up.  Also I tend to not flat stick 12s everywhere because that way lies madness.  Had more vesc fails on 10s set ups than 12 so far.  Remains to be seen whether this will play out in the long term as this 12s is only a few months old.  It definitely doesn't run the motors as hot though compared to the same parallel 10s.  Just saying so far so good.  

I've just put the kiss of death on my 12s set up now though with that statement.  :grimacing:
```

---
## \#9 Posted by: Gamer43 Posted at: 2019-01-13T22:58:46.077Z Reads: 235

```
12s will run a higher risk blowing up the FOCBoxes (but that chance is still pretty small) in exchange for a higher max speed. To reduce this risk, I'd recommend undercharging the pack by one or two volts to 48-49V.

More cells in parallel means higher battery current settings (depending on how you ride, this may not make much of a difference). 

[quote="dareno, post:8, topic:80810"]
I’d question that statement. So long as you use the correct vesc then there is nothing wrong with 12s reliability. See me being me would run a 10s 4p pack at max amps and then ride it like I stole it. With the 12s 4p to get the same punch the current can be lower and therefore less stressful on the set up. Also I tend to not flat stick 12s everywhere because that way lies madness. Had more vesc fails on 10s set ups than 12 so far. Remains to be seen whether this will play out in the long term as this 12s is only a few months old. It definitely doesn’t run the motors as hot though compared to the same parallel 10s. Just saying so far so good.

I’ve just put the kiss of death on my 12s set up now though with that statement. :grimacing:
[/quote]

What hardware version and current settings are the VESCs running, also what was the failure mode and use rate between 10s and 12s? When my friend switched to FOC on a 12s4p setup, one of his VESCs immediately died. 
MOSFETs are only rated for 60V, meaning transients will trigger avalanche breakdown (the IR fets, despite their poor electrical characteristics, actually have really rugged avalanche characteristics) and the DRV830x is only rated for 65V on VIN and phase nodes.
12s fully charged barely passes the 20% headroom rule. This is why DRV failures are not uncommon at 12s.
```

---
## \#10 Posted by: dareno Posted at: 2019-01-13T23:11:24.780Z Reads: 203

```
Not game to run 12s foc even on focboxes.  Too many horror stories.  I like reliable and don't need the bells and whistles that come with foc.  I build very simple set ups for this reason.   **K**eep it **S**imple **S**tupid **S**afe.  Works for me.  
The 12s is running the latest version of the foc boxes but I did have a drv fail when I ran some HK 4.12 for a while. I was at the testing stage so was pushing the current settings too hard.  Hard braking etc for science.  Focboxes are imo the most reliable 4.12 vesc derivative and its just my opinion based on experience before the inevitable flurry of replies.  Once something works for me I stick with it because if its not broke don't fix it.
```

---
## \#11 Posted by: PatRocks Posted at: 2019-01-13T23:18:26.496Z Reads: 199

```
Ummm... I've been running 12 foc for a year and a half. Focboxes are running smooth as tits. So much so that I haven't even bothered to swap them out with my dual Escapes lol.
```

---
## \#12 Posted by: Skunk Posted at: 2019-01-13T23:19:37.720Z Reads: 200

```
12s is officially safe. Let's talk 13s lol
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-01-13T23:20:52.868Z Reads: 201

```
Can't wait until I can build by 12s5p :drooling_face:
```

---
## \#14 Posted by: yelnats8j Posted at: 2019-01-13T23:22:43.131Z Reads: 194

```
Same everything is here except the spot welder.
```

---
## \#15 Posted by: Sn4pz Posted at: 2019-01-13T23:23:48.397Z Reads: 193

```
I've got no materials yet 😂 

I'm hoping the Samsung 30ts are going to drop in price so I can build a fatty pack with them
```

---
## \#16 Posted by: Skunk Posted at: 2019-01-13T23:26:30.943Z Reads: 193

```
[quote="Sn4pz, post:15, topic:80810"]
Samsung 30ts
[/quote]

How big of a gain are they over 30q batterys?
```

---
## \#17 Posted by: dareno Posted at: 2019-01-13T23:31:05.348Z Reads: 183

```
Another 15amps discharge  apparently.
```

---
## \#18 Posted by: Surfer Posted at: 2019-01-13T23:31:31.343Z Reads: 185

```
6p probably will have more torque at low speeds, cuz less voltage saaag.
I went from 10s4p to 12s4p medium and high speed increased. Low speed torque decreased even with better cells, I'm still tweaking it
```

---
## \#19 Posted by: Skunk Posted at: 2019-01-13T23:31:48.080Z Reads: 182

```
[quote="dareno, post:17, topic:80810, full:true"]
Another 15amps discharge apparently.
[/quote]

Similar life span?
```

---
## \#20 Posted by: Sn4pz Posted at: 2019-01-13T23:33:25.347Z Reads: 182

```
Yep, ive been looking at mooch graphs and all sorts of other graphs

I dont want to push huge amps anyways, I just like the safety overhead as well as the Voltage sag prevention
```

---
## \#21 Posted by: dareno Posted at: 2019-01-13T23:34:09.488Z Reads: 175

```
According to all the tests and Alan eboosted they are the tits.  Been scouring the vapers for info and they can safely discharge up to 40amps.  Thats crazy.  They state 35a but as the 30q states 15a and we all run them safely at 20a  Bigger size 21700 but when you factor in less P it makes sense.  More dollars though
```

---
## \#22 Posted by: Skunk Posted at: 2019-01-13T23:34:22.106Z Reads: 169

```
13s5p 30t :smiling_imp: yaaas
```

---
## \#23 Posted by: Sn4pz Posted at: 2019-01-13T23:35:13.599Z Reads: 176

```
Damnit youll probably build it before I get mine :anguished:

either way all that range and all the potential power :drooling_face:
```

---
## \#24 Posted by: dareno Posted at: 2019-01-13T23:35:32.933Z Reads: 173

```
That will tear the thane off the cores.  Have to be careful to stay under the limits of the motor controllers with that pack.
```

---
## \#25 Posted by: venom121212 Posted at: 2019-01-13T23:35:46.535Z Reads: 173

```
Psh samsung just unveiled a new EV 2170 battery. This pack below charges in 20 minutes and goes 370 miles supposedly ![samsung_sdi_battery_cell-e1483989875932|690x342](upload://6jtvTYEWl6yO3nznGzKMkfgSZNl.jpeg)
```

---
## \#26 Posted by: dareno Posted at: 2019-01-13T23:37:17.075Z Reads: 174

```
Is that that solid core lithium cell?  Been rumours of a completely safe solid pack that outperforms anything by a country mile
```

---
## \#27 Posted by: venom121212 Posted at: 2019-01-13T23:39:39.101Z Reads: 172

```
I can't tell, they're keeping tight lipped but it's supposed to be a direct competition to teslas new cells. Slated to hit mass market 2021 😢
```

---
## \#28 Posted by: dareno Posted at: 2019-01-13T23:44:13.293Z Reads: 171

```
Not the same things then because these ones are due to drop soon apparently.  Nice to have some more choices coming through though.  Definitely not the time to sink dollars into a new 30q pack.
```

---
## \#29 Posted by: pixelsilva Posted at: 2019-01-13T23:50:08.444Z Reads: 171

```
2021 is too far away for me. Anybody knows whats the largest 30Q cell battery type I can fit inside a @psychotiller Evo enclosure with two VESCs and BMS? 

![IMG_20190113_154845|690x388](upload://4SBKl3zTu6rYmfBjMm4uJWR7p8W.jpeg) 

![IMG_20190113_154804|690x388](upload://qZuUQzfuA0xnfmlXzeqq43maPfz.jpeg)

Edit: first warning up there :point_up_2: with @dareno's neg. 30Q advice. :roll_eyes:
```

---
## \#30 Posted by: dareno Posted at: 2019-01-13T23:59:29.956Z Reads: 163

```
Don't take anything I say seriously dude lol   Still the best bang for your buck out there right now.  I just won't be spending on a new pack just yet.
1.  because I've got nothing for it to go in
2. because I've got nothing for it to go in
```

---
## \#31 Posted by: b264 Posted at: 2019-01-14T00:00:44.866Z Reads: 167

```
[quote="pat.speed, post:4, topic:80810"]
Wrong! they have the same amount of cells in the packs therefore the same Watt hours, therefore the same range
[/quote]

That's not entirely true.  If the 12S can offer more acceleration then in theory you could use the same amount but in reality, you will use more which means less range.
```

---
## \#32 Posted by: psychotiller Posted at: 2019-01-14T00:04:13.253Z Reads: 165

```
12s5p. Tight fit. laid out like this pack on the bottom of the pic.
https://www.instagram.com/p/BgJiA2eDA0N/
```

---
## \#33 Posted by: pixelsilva Posted at: 2019-01-14T00:14:57.913Z Reads: 161

```
Wow!! Nice @psychotiller!! Now the sweet news... how much foh da brick ?

( 12s5p or 10s6p )
```

---
## \#34 Posted by: psychotiller Posted at: 2019-01-14T00:59:06.221Z Reads: 160

```
$515 either way. However. I've found an issue with our 12 bms's looking for a new supplier/model.

I have alot of 10s bms's that are sweet.
```

---
## \#35 Posted by: Skunk Posted at: 2019-01-14T01:01:44.312Z Reads: 162

```
[quote="psychotiller, post:34, topic:80810"]
e found an issue with our 12 bms’s
[/quote]

Should i be worried or thinking about replacing mine?
```

---
## \#36 Posted by: psychotiller Posted at: 2019-01-14T01:12:37.778Z Reads: 163

```
No. what it is, is that some of the bms's they sent me like to stay at nominal voltage. So, if you charge your board to 4.2v per cell and ride it works perfectly. If you charge to full voltage and let your board sit for a month it will take your cells back down to 3.6v per cell. Not necessarily a bad thing, but it means your bms always feels warm until it gets back to nominal. just annoying really, because it's not what I friggen ordered!!

The way to check is fully charge your pack. check the voltage to confirm it's 100%. Then wait 10 or 15 minutes. Feel the bms. If it's cool to the touch you're good! If not we can switch it out if you want. (when I get new Beemusses)
```

---
## \#37 Posted by: deucesdown Posted at: 2019-01-14T04:19:56.691Z Reads: 146

```
@psychotiller what say you, 10s6p or 12s5p?
```

---
## \#38 Posted by: Skunk Posted at: 2019-01-14T04:23:33.469Z Reads: 147

```
Lol i know the answer.  I didn't listen
```

---
## \#39 Posted by: psychotiller Posted at: 2019-01-14T04:27:06.782Z Reads: 148

```
Well, personally my bros and me like 10s. No issues with power anywhere. No issues with switches. No issues with foc on any speed controller. No issues with bms's. 
The new 6 type vescs, focboxes, and unities are great with 12s anyway.

I'd say go 10s. 60 cells is 60 cells.
```

---
## \#40 Posted by: SynteX Posted at: 2019-01-14T06:20:52.863Z Reads: 140

```
Unless somebody wants to trade their unity against 2 focboxes I better stick with 10s6p for safety reasons.?
```

---
## \#41 Posted by: dareno Posted at: 2019-01-14T06:24:48.956Z Reads: 140

```
[quote="psychotiller, post:39, topic:80810"]
The new 6 type vescs, **focboxes,** and unities are great with 12s anyway.
[/quote]

<abdcjdbhb>
```

---
## \#42 Posted by: Allofyoush Posted at: 2019-01-14T06:32:46.902Z Reads: 136

```
*EDIT* Not worth your time

I have an honest question. Do you guys think the electric skateboard industry will gear more towards more and more distance? Once you hit 35mph on a board, very few people are willing to go over that. But it seems like we're limited by the amperage of ESCs as far as I can tell. How can we break through to 13s or 14s, etc? Real commuter vehicles.
```

---
## \#43 Posted by: Bjork3n Posted at: 2019-01-14T07:04:20.217Z Reads: 136

```
There are far more failures that I know of using 12s compared to 10s. 
Don't know why but it seems like a hit or miss. 
Been using 10s for over 1000km with zero problems. 
I would go 10s if you are on a budget and want reliability, 12s if you like power and can comprise on reliability. This is my opinion and experience. 
Will probably be bashed now after this post...
```

---
## \#44 Posted by: Andy87 Posted at: 2019-01-14T07:11:47.136Z Reads: 136

```
[quote="Allofyoush, post:42, topic:80810"]
we’re limited by the amperage of ESCs as far as I can tell
[/quote]

No we aren´t

[quote="Allofyoush, post:42, topic:80810"]
How can we break through to 13s or 14s
[/quote]

We already have this.

[quote="Allofyoush, post:42, topic:80810"]
Real commuter vehicles.
[/quote]

what you speak about?

did you ever ride an esk8?
```

---
## \#45 Posted by: Andy87 Posted at: 2019-01-14T07:13:54.332Z Reads: 127

```
driving your electronic close to your rated limit is sure not the best way.
I´m fan of 12s but totally nothing bad with 10s. 
especially if you need your board to drive to work etc.
you want something you can trust that will work.
```

---
## \#46 Posted by: dareno Posted at: 2019-01-14T07:13:56.307Z Reads: 130

```
[quote="Bjork3n, post:43, topic:80810"]
This is my opinion and experience.
[/quote]

These 2 terms are not mutually exclusive in my opinion.  I run 10s and 12s and both seem to be the same reliability wise.  Used 10s for longer though so had more failures but thats time related.  Actually had more failures running 8s back in the day but that was due to ignorance.  So many factors at play its a really a moot point.    
Do you run 12s?
```

---
## \#47 Posted by: Allofyoush Posted at: 2019-01-14T07:24:13.110Z Reads: 128

```
This is a thread about whether or not 12s is reliable. I don't think 13s or 14s would be more reliable than that

I don't know of ESCs that can withstand over 200A, but they probably exist
```

---
## \#48 Posted by: Andy87 Posted at: 2019-01-14T07:28:01.030Z Reads: 127

```
You started to speak about 13-14s.
Get the right vesc and you can run even 16s if you think you can control it.
https://vesc-project.com/node/339

Without any disrespect, but why you think we on the limit and why you didn’t answer my full reply?
```

---
## \#49 Posted by: Allofyoush Posted at: 2019-01-14T07:30:39.212Z Reads: 120

```
*EDIT* Not worth your time

I've only seen what people have been talking about on here. I haven't seen anything above 12s, so I was wondering why it wasn't more popular. Especially with the DIY community. For me, a commuter vehicle can go all the way across the city and back. 20, maybe 30 miles per charge. I may be wrong about what the limits are, I just haven't seen anything above 12s yet. And I haven't been here that wrong either, which was why I asked in the first place. I'd be interested in the boards you're talking about
```

---
## \#50 Posted by: dareno Posted at: 2019-01-14T07:33:31.197Z Reads: 126

```
[quote="Allofyoush, post:42, topic:80810"]
How can we break through to 13s or 14s,
[/quote]

[quote="Allofyoush, post:47, topic:80810"]
This is a thread about whether or not 12s is reliable.
[/quote]

You are entering into the realms of ridicule here dude.   Its pretty obvious you need to read and not comment when you start contradicting yourself.  You bring up 13s or 14s when nobody else had and then point out that the thread is about 10 or 12s  For your own good and for the sake of the mods keep quiet and learn.
```

---
## \#51 Posted by: Andy87 Posted at: 2019-01-14T07:34:24.482Z Reads: 130

```
I know you not long in here.
maybe sometimes it would be good to use the search function.
it´s in the right upper corner.

https://www.electric-skateboard.builders/t/clone-evo-landyachtz-evo-falcon-abec-107mm-13s5p-top-mount-focbox-sk3-6374-metr-pro/57765?u=andy87
https://www.electric-skateboard.builders/t/13s-evo-from-hell/41468?u=andy87
https://www.electric-skateboard.builders/t/room-for-40-cells-10s4p-or-13s3p/74766?u=andy87
https://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411?u=andy87

I stop here... there way much more of them.
```

---
## \#52 Posted by: Allofyoush Posted at: 2019-01-14T07:39:16.531Z Reads: 112

```
Ok thank you
```

---
## \#53 Posted by: SynteX Posted at: 2019-01-14T08:32:30.727Z Reads: 113

```
Just a question like I said i’m running 4 lipo’s with 3s of 8000mah
Someone said this is comparable with 12s1p?
Since the lipo’s are all connected in serie?

Aren’t I sure then that i can safely run 12s5p since this board is working for over a year?
```

---
## \#54 Posted by: Andy87 Posted at: 2019-01-14T08:42:10.473Z Reads: 118

```
if you run 4 lipos with 3s in 12s config than you connected them in series not parallel.

[quote="SynteX, post:53, topic:80810"]
Someone said this is comparable with 12s3p?
[/quote]
this all depents on which 12s3p liion pack and which 12s1p lipo pack you want to compair.

[quote="SynteX, post:53, topic:80810"]
Aren’t I sure then that i can safely run 12s5p
[/quote]
? don´t get what you want to ask. more more 3p, 5p, 20p doesn´t have an influence on the vesc. just with 3p your constant current you can run through your vesc is smaller than with 5p or 10p of the same cells.
```

---
## \#55 Posted by: SynteX Posted at: 2019-01-14T08:48:06.526Z Reads: 111

```
Thanks Andy,

Already changed my message haha.
So I'm comparing it to a 30q pack.

So If i safely run 12s1p in lipo's
I wouldn't have any issue changing it with a 12s5p 30q pack?
```

---
## \#56 Posted by: Andy87 Posted at: 2019-01-14T08:56:18.773Z Reads: 107

```
for sure not.
with your 12s5p you would have 100a constant discharge from the pack.
so max battery max setting at 50a per vesc (depending on your vesc, some should set only to 35a)
```

---
## \#57 Posted by: SynteX Posted at: 2019-01-14T08:57:19.630Z Reads: 106

```
[quote="Andy87, post:56, topic:80810"]
depending on your vesc, some should set only to 35a
[/quote]

Focboxes with 4.x software
They used to have old oftware but already updated them.
```

---
## \#58 Posted by: Andy87 Posted at: 2019-01-14T08:58:08.957Z Reads: 104

```
focboxes are fine with 50a bat max settings.
```

---
## \#59 Posted by: SynteX Posted at: 2019-01-14T09:01:10.204Z Reads: 108

```
Thanks Andy Just to make sure!

12s5p -> Will have no problems seeing my current set-up
Both focboxes should be set to -> 50a bat max Which also means i put 50A in motor max?

It still doesn't matter if I run in FOC nor BLDCS?
Don't even know anymore what my current settings are.

But following this will have no issues at all?
```

---
## \#60 Posted by: Andy87 Posted at: 2019-01-14T09:08:01.715Z Reads: 111

```
if you set up your focboxes right, there shouldn´t be a higher setting at the moment with the old lipo.
you set the bat max value always (maximum) to the constant current rating of your battery /2 (if you run dual). if your your max output ability of your pack exceed the vesc rating  (for example a 10p pack) than you set it for sure on the max constant current your vesc can handle (or lower).

your motor max you can set to the max rating of your motors.
idk which motors you use and for which current they rated.

you can run focbox in FOC and 12s.
```

---
## \#61 Posted by: SynteX Posted at: 2019-01-14T09:09:09.670Z Reads: 110

```
![8e2f3d09-c2ba-4a2b-891c-4ef911c29884|236x500](upload://A0YTIQ4G3AVv9xpubOlPOcCOtnl.jpeg)
```

---
## \#62 Posted by: SynteX Posted at: 2019-01-14T09:10:15.056Z Reads: 105

```
So battery max = 50A
Motor max = 70A

And that will be Okay
```

---
## \#63 Posted by: Andy87 Posted at: 2019-01-14T09:13:11.266Z Reads: 105

```
should work!
just have a look that your bat min value is not over the top.
i would start with -10A per focbox
```

---
## \#64 Posted by: SynteX Posted at: 2019-01-14T09:14:00.859Z Reads: 106

```
Thanks for the help Andy!

Now I know what to do! Appreciate it.
```

---
## \#65 Posted by: SynteX Posted at: 2019-01-14T09:39:35.350Z Reads: 106

```
Okay just had a small talk.

I heard that -4A per p is the max so for safety reasons i use -3A per p
Mening a battery min of -15A

I have to focboxes so that means -15/2 = -7.5A per focbox?

And you told me to set the battery max on 50A
Does that also mean in the focbox settings i do
75/2 = 37.5A per focbox or 75A per focbox since a 12s would have 75A discharche
```

---
## \#66 Posted by: Andy87 Posted at: 2019-01-14T09:52:31.823Z Reads: 108

```
[quote="SynteX, post:65, topic:80810"]
-4A per p is the max
[/quote]
yes but this value is for a full charge cycle 2.5V-4.2V.
you think you can break that long? I guess you need a very very long hill for this.
10A is a good value (that´s my opinion) probably you will anyhow never reach that value....

[quote="SynteX, post:65, topic:80810"]
75/2 = 37.5A per focbox or 75A per focbox since a 12s would have 75A discharche
[/quote]
how you come to it?
i guess i know from where.
idk who you was talking with but this person told you that the 30q rated to 15a.
so 5+15a is 75a.
but the 30q are 20a cells, not 15a cells.
nothing bad with 37.5A, always better less than too much, but you can set the values to 50A (again my opinion).
If you not sure, read a bit in here, use the search function and than set it to what ever you think is right.

one more thing, with a 10s4p 30q you would have your 75A too same with 8s4p or even with 1s4p.
if somebody told you the discharge capabilty depents on the S count than you better doing your own research.
```

---
## \#67 Posted by: SynteX Posted at: 2019-01-14T09:55:58.270Z Reads: 108

```
Thanks Andy I got this from him:

![image|281x499](upload://zw11pq4QdxdsbVWI4ZF4i3YHL3l.jpeg)
```

---
## \#68 Posted by: Andy87 Posted at: 2019-01-14T10:02:44.463Z Reads: 105

```
i´m not fan of posting facebook links... but i couldn´t find the website and i don´t want to search any longer.
here is a real life test with the 30q,
https://www.facebook.com/batterymooch/posts/samsung-30q-3000mah-18650a-great-15a20-batterybottom-line-this-is-a-retest-of-th/2018668968422679/

so in fact you can use them as 20a cell.
read a bit here about cells and there rating and you will understand why i chose the values i chose.
```

---
## \#69 Posted by: Sebike Posted at: 2019-01-14T10:11:15.013Z Reads: 103

```
... And you will find that 15A rating in nearly every store that sells these cells, because that's the OFFICIAL amp rating that Samsung has decided to put on the specs sheet for this cell. Real life testing sais what Andy has said already, ie that these cells can safely deliver up to 20A as long as temp is kept at normal levels.
```

---
## \#70 Posted by: Schulerbible Posted at: 2019-01-14T10:49:59.843Z Reads: 103

```
12s3p or better 4p with graphene lipos :ok_hand:
```

---
## \#71 Posted by: Andy87 Posted at: 2019-01-14T11:00:30.489Z Reads: 101

```
Aren’t you the one who like to post his 500a battery? 😅😜🤔
```

---
## \#72 Posted by: Schulerbible Posted at: 2019-01-14T11:16:23.148Z Reads: 101

```
Must be a different person :sweat_smile:
```

---
## \#73 Posted by: Andy87 Posted at: 2019-01-14T11:20:06.890Z Reads: 100

```
No seriously I thought you have a big lipo battery pack.Something like 4p graphens.
No?
```

---
## \#74 Posted by: Schulerbible Posted at: 2019-01-14T11:23:44.321Z Reads: 100

```
Not yet, I will have a 12s3p pack and for long distance rides an external pack for charging while riding.
```

---
## \#75 Posted by: b264 Posted at: 2019-01-14T17:16:26.712Z Reads: 90

```
@Allofyoush we could have this same discussion about using 12S or 14S on [VESC 7](https://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26293.html) but this is about 10S or 12S on VESC 4-6 and clones
```

---
## \#76 Posted by: Allofyoush Posted at: 2019-01-14T17:29:17.278Z Reads: 87

```
@b264 Holy shit! I've never seen this before. Thanks man
```

---
## \#77 Posted by: SynteX Posted at: 2019-01-22T08:04:55.673Z Reads: 73

```
I'm going for a 12s6p :smiley:
```

---
## \#78 Posted by: dareno Posted at: 2019-01-22T09:12:36.664Z Reads: 72

```
Boom!!  Do not mess about there my man!!  Just don't push the battery amp settings with this set up or whatever 4.12 vesc variant will not like it.  Focboxes will handle it on paper but I personally try to keep everything under by at least 10.  Wiggle room.
```

---

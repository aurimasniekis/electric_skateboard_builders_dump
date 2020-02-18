# First build &#124; 6&rdquo; pneumatic &#124; RKP 273 &#124; dual SK3 6364 245kv &#124; homemade mounts &#124; 12s &#124; dual VESC

### Replies: 28 Views: 2381

## \#1 Posted by: eaglo Posted at: 2017-02-15T23:28:05.261Z Reads: 235

```
Hi guys,

This is my first build/post. A few months ago I saw a picture of an evolve all terrain board and fell in love with the idea of it. I come from the FPV multirotor world (seems like there's a lot in common), so after talking with some friends who'd dabbled, I thought I'd try building an eboard myself and seeing if I could save some money. I truly appreciate the learning experience, but if I could go back in time I'd probably just work one overtime shift and buy the evolve board for the sake of spending a little more time with my family lol. This community is awesome, and I am grateful to everyone who has shared their knowledge and experiences. Thanks to Dexter at DIYelectricskateboard and @psychotiller for their help and information. Also thanks @treenutter for helping troubleshoot my speed/torque problem.

My goal was to build something that could ride over well kept grass, so that I could ride my board around at the park and retrieve my FPV drone after I crash it. Riding on the street would be a bonus. I wanted to come in under $1000 (google doc of [spending](https://docs.google.com/spreadsheets/d/1218oE-bFaQYgCTBBQcoRZPYRkBIgxHJ1M1xCGyvtRFs/edit?usp=sharing) fortunately I had many tools and material already at my disposal which kept some costs down). I came in around $850 and so far I've done a few test runs that were REALLY fun. I kind of just mocked everything up for the test run (no thread lock or anything) cause I was so excited to try it out. Turns out a motor pulley came loose and while the board road amazing on the street it didn't go very far at all on the grass. I'm hoping that has to do with either the loose motor pulley or the VESC settings. 

You can refer to the spending link above if you want to see more specifics about the parts I used, but I basically tried to cut costs on the deck, wheels, bearings, battery, mounts, and diy enclosure.

some notes about my parts choices:
-I went 12s cause I wanted POWAH!!!!
-deciding which trucks to use was very difficult for me. I wanted them as narrow as possible without having wheel bite and while still allowing for dual rear mounted motors. I ended up having to offset the mounts in order to fit both motors, otherwise they would have touched. The nuts also aren't on all the way so I'm gonna hunt for some low profile nuts.
-the cheap 6" pneumatic wheels seem ok for now with the home made gears, but I wouldn't be surprised if the hubs broke. not sure what route I'll go if that happens. maybe save up for psychotillers awesome aluminum ones.
-I had no idea how the deck would turn out for the generic cheap thing that it is, but it seems great so far. Just had to sand a bit off to avoid wheel bite.
-home making the battery enclosure was fun. I ended up attaching it to the deck and using a heat gun to slowly go around the perimeter and get the flange to contour more closely to the deck's curves. 

 <img src="/uploads/db1493/original/3X/b/7/b70aab107707a84e5ff8d43524109a6195799e5d.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/e/7ea578a56b9abd26b3ff67900bde8ac2f8cffab5.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/c/b/cb3c76f4831ec388d3ecd252cad861a193719a23.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/e/3/e3e8ee124851999b5a093cc04227865c3b50dbb0.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/9/0/900975ab1d42e10bd7146ae3e6700d91d83045b9.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/5/8532285a5c32d9be33714fbb5d4f93fc08ee07ee.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/e/deaa38c3f866262ac4774719d93629da53140533.jpg" width="374" height="500">

VESC settings are the same for master and slave except for the controller IDs. Here are some pics in case anyone is willing to make some recommendations for what I should change. I'm not sure exactly what min and max limits to set with the RPM and amps given the 12s, dual 245kv situation. I'm also trying to figure out how to keep braking power but loose the regeneration part since I don't want to shorten battery life with lots of short recharges...
<img src="/uploads/db1493/original/3X/2/9/29daf0911e06f23679b5edfa5f7f8a7a060cf604.png" width="690" height="406"><img src="/uploads/db1493/original/3X/6/c/6cac2a529235fc24db1141bd1c102039e2eeffc4.png" width="690" height="406"><img src="/uploads/db1493/original/3X/b/9/b98d386e0843706196f28c072f5fc94ba580631c.png" width="690" height="406"><img src="/uploads/db1493/original/3X/e/1/e1848c09c3956c9c970f233c1ee4da1c3873040c.png" width="690" height="406"><img src="/uploads/db1493/original/3X/7/8/78f43f35e580df205c3fa649c4f6fd9a23bd0248.png" width="690" height="406">

Thanks for reading!  :]
Nick
```

---
## \#2 Posted by: Martinsp Posted at: 2017-02-15T23:31:26.992Z Reads: 174

```
hello nick, your board looks really cool! :3 

I just wanted to tell you (joke dont take it seriously) that my OCD just cant handle your motors not being in line with each other! :D :D 

Ride safe! cheers from Slovakia.
```

---
## \#3 Posted by: eaglo Posted at: 2017-02-15T23:34:06.852Z Reads: 174

```
Thanks! Oh I hear you, my OCD almost gave me a heart attack when I realized I'd have to do it like I did haha. It just doesn't look right :/ But every time I overcome those OCD thoughts I'm so proud of myself!
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-15T23:37:46.592Z Reads: 166

```
[quote="eaglo, post:1, topic:17766"]
I'm also trying to figure out how to keep braking power but loose the regeneration part since I don't want to shorten battery life with lots of short recharges...
[/quote]

It's not possible. Just don't worry about it.
```

---
## \#5 Posted by: eaglo Posted at: 2017-02-15T23:39:19.673Z Reads: 150

```
perfect response! thank you for saving me the worry :)
```

---
## \#6 Posted by: psychotiller Posted at: 2017-02-16T00:03:14.601Z Reads: 150

```
Hey man! I love the Props!

Also, nice job on your first build. I had bad luck with those wheels. Blew out the outside bead and the tire fell off. Too much air pressure will crack that plastic. I weigh 210lbs though and was riding up the walls at the Santa Ana Riverbed. 

I really like what you did with the pulley and the retainer. I'm guessing the way you did it may even balance the wheel against the weight of the valve stem?

Nice deck choice too.

You'll eventually find that those batteries are sag monsters! When that happens have a li-ion pack made or make one. You'll never look back.
```

---
## \#7 Posted by: Martinsp Posted at: 2017-02-16T00:08:54.692Z Reads: 134

```
You should also keep an eye on those motor cables. They dont look like silicone insulated high strand count. If they are than you are ok but if not they might break if they bend a lot while turning.
```

---
## \#8 Posted by: eaglo Posted at: 2017-02-16T00:11:16.903Z Reads: 140

```
Thanks man! I'm 200 lbs myself, so perhaps its only a matter of time til the tires go. I imagine riding on the grass will take quite a toll too...

I never thought about balancing the wheels...I could probably figure it out, but the way it is, it might be overcompensating for the weight of the stem valve. I just wanted to make use of all the available hub holes for strength (I printed with ABS), but you bring up a very interesting point... 

sad news about the batteries, but for just over $100 I guess I figured it'd be a decent starter setup. I'll definitely look to li-ion for the next time around.
```

---
## \#9 Posted by: eaglo Posted at: 2017-02-16T00:13:16.601Z Reads: 129

```
ooohhh, gosh I never thought about that. Do you think that cutting them short and soldering them into high strand wire would be the best way to mitigate the issue?
```

---
## \#10 Posted by: psychotiller Posted at: 2017-02-16T00:14:02.752Z Reads: 126

```
Hope not to bring you down! What you put together is really nice. Have fun.
```

---
## \#11 Posted by: eaglo Posted at: 2017-02-16T00:15:06.286Z Reads: 124

```
its all good, I appreciate the insight. I'll enjoy it til it breaks or dies and I'll go from there :)
```

---
## \#12 Posted by: Okami Posted at: 2017-02-16T12:59:37.986Z Reads: 118

```
@eaglo do you mind, if ''we'' ask where did you get your nice 6'' wheels?

Also - are they 1 - 1/4 in thich?

--

I think there could be a demand for such wheels if someone came up with a source where to get them easly and cheaply.. :slight_smile:
```

---
## \#13 Posted by: riva_00 Posted at: 2017-02-16T13:47:13.417Z Reads: 113

```
@eaglo Hows the deck, does it have a lot of flex? And is the concave steep/sharp?
I currently have a landyachtz 35" with a full drop, and I want to try a longer board with just a micro-drop for more ground clearance and more room underneath.
```

---
## \#14 Posted by: Martinsp Posted at: 2017-02-16T14:05:24.928Z Reads: 119

```
I have done that, cut the wires short and solder silicone ones on. It is easier said then done though 😀 Definitely doable but you will have to get rid of the enamel on the wires with either a hot solderimg Iron or carefully with a lighter. It is better to do it now because they might break so close to the stator that you wont be able to solder them.
```

---
## \#15 Posted by: ninja Posted at: 2017-02-16T18:10:36.697Z Reads: 116

```
12S on 245 kv motors, isn't it too much for VESC? :astonished:
```

---
## \#16 Posted by: eaglo Posted at: 2017-02-18T09:59:55.104Z Reads: 104

```
Yes I believe that is the size. I found them on accesscasters.com for $18 each I think before shipping. When I go back to look I can only find them attached to caster hardware and significantly more expensive. I have a feeling they'll break cause psychotiller and a few others have had that experience, but I figured I'd give them a go for the price.
```

---
## \#17 Posted by: eaglo Posted at: 2017-02-18T10:00:53.133Z Reads: 101

```
Per @treenutters recommendation I set the erpm max to 60k and so fast haven't had any issues
```

---
## \#18 Posted by: eaglo Posted at: 2017-02-18T10:04:36.533Z Reads: 104

```
I don't have another board to compare it to bit I'm 200lbs, and it flexes a very appropriate seeming amount. Medium stiff flex maybe? It was a generic blank deck that showed up a lot online through various wholesale websites when I searched for a micro drop deck. It barely has a drop at all if any but I think it looks good. The concave is pretty sharp Id say, but again I don't have any other skateboards.
```

---
## \#19 Posted by: eaglo Posted at: 2017-02-18T10:13:23.660Z Reads: 105

```
I was gonna ask, do you have a preferred/trusted reference for li-ion building? And perhaps a preferred brand of 18650? That will be my second upgrade. My first is gonna be some better wheels...
```

---
## \#20 Posted by: psychotiller Posted at: 2017-02-18T13:10:57.846Z Reads: 108

```
Pretty much Samsung 25r 18650 cells. @barajabali is the place to go for custom packs.  Read up though, theres plenty of information on the forum about building your own packs. 

As for wheels I know a guy 😁
```

---
## \#21 Posted by: Okami Posted at: 2017-02-18T13:13:05.154Z Reads: 115

```
I think it has turned up that Samsung 30Q are actually a bit better (less sag and all) but you should ask this sort of stuff from @PXSS .. Otherwise yeah, @barajabali can step in and recommend what cells for what setup to best get

Though the 30Q ones are a bit pricier.. but also offer about 400-500mah more (depending on discharge)

---

Chart: 25R vs 30Q:
http://budgetlightforum.com/node/42075

--
30Q vs Sanyo GA
https://endless-sphere.com/forums/viewtopic.php?p=1150344#p1150344
---


https://www.dropbox.com/s/nle8ol3eq8s5tp9/Samsung%20INR18650-30Q%2015A%203000mAh%20Constant-Current%20Tests.bmp?dl=0
https://www.e-cigarette-forum.com/forum/threads/samsung-inr18650-30q-15a-3000mah-bench-test-results.681259/

<img src="/uploads/db1493/original/3X/7/c/7ca191576bc88694134f95b24d5736900065a930.png" width="563" height="84">

--

25R seems to come at arond 2.2-2.3Ah when discharged at 5A or so.. In comparison, 30Q seems to give off about 2,7-2.8Ah, so yeah ~0.4-0.5 ah more per cell. 

Also, for eboards the cells probably wont be discharged till 2.5v.. so a somewhat good cut-off at load might be at 2.8-3.0v probably.
```

---
## \#22 Posted by: PXSS Posted at: 2017-02-18T13:35:44.230Z Reads: 92

```
The reason I suggest not to use samsung 25Rs is because they really are no better than Sanyo GA cells, which have 3500mah capacity, power wise even though they are rated twice as high. The best power cell avail is VTC6, samsung 30Q is similar but cheaper.
```

---
## \#23 Posted by: psychotiller Posted at: 2017-02-18T14:34:40.069Z Reads: 90

```
Good info. My packs from @barajabali have been great and are performing very well.
several 8s and 10s packs.
```

---
## \#24 Posted by: eaglo Posted at: 2017-02-18T17:51:04.645Z Reads: 82

```
Thanks! I will start my li-ion research soon...

I love the idea of getting some of your wheels, trust me. Those things are works of art. Unfortunately I've welded my motor mounts in place, so I don't know if they would fit on the trucks and still have room in between the motor mount for the pulleys (I'm using your awesome trucks of course). I checked out your website last night and it looked like you have newer wheels designed too, but I couldnt see a picture (might have just been because I was on my phone). If your wheels work with my existing hodge podge of a mechanical setup I'll definitely buy some. Otherwise I may see how expensive it is to make some metal ones of my own that are just replicas of the plastic hubs I'm using. I have a little bit of 3d designing experience, asks might be able to pull it off. And if that doesn't work I'll just buy your wheels and all new everything!! Bwahahaha
```

---
## \#25 Posted by: eaglo Posted at: 2017-02-18T17:52:20.728Z Reads: 78

```
Wow, great info I really appreciate it!
```

---
## \#26 Posted by: eaglo Posted at: 2017-02-18T17:54:35.883Z Reads: 82

```
So good to have someone just hand me this information...much gratitude :grin:
```

---
## \#27 Posted by: psychotiller Posted at: 2017-02-18T22:49:36.548Z Reads: 84

```
My wheels are designed for use with versapulleys. They are adjustable width wise. Also my V1 wheels are centerset. V2's are offset by about a 1/2 inch. This allows more room for 15mm pulleys. I think you'd be able to use them with your set up.

Thanks!
```

---
## \#28 Posted by: eaglo Posted at: 2017-02-18T23:10:45.351Z Reads: 84

```
Ok, I definitely gotta check numbers out and stuff cause if your v2 wheels will work I want in!
```

---

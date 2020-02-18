# Long Range/Budget Build &#124; DIY 18650 Battery &#124; VESC &#124; 280kv &#124; Wood Deck

### Replies: 93 Views: 13759

## \#1 Posted by: seanpain4 Posted at: 2016-05-05T12:29:47.561Z Reads: 822

```
So, i have decided after watching many videos and reading many posts i am going to build my own Electric Longboard. 

I don't have a lot of money to spare, so my budget is fairly limited at around $500 (excludes chargers and misc wires, connectors,etc as i have all of that), but i think i can make it work. My goal is to get the longest range for the cheapest price. 

For the battery i will be going the DIY route and will be making a 6S13P 18650 Battery. The battery itself will weigh around 3.5kg and will be soldered together and wrapped by myself. I will post progress pictures throughout this thread as i get to those stages. 

I have ordered all of my parts, and i am only waiting on the motor, belt, controller, some more 10AWG wire and a VESC. (I ordered a cheap HobbyKing ESC as a temporary solution due to the VESC delay.)

This is just a small intro into my build thread. I will keep it updated with pictures and progress posts. 

Thanks :slight_smile:

EDIT:
I am using recycled laptop batteries for my source of 18650's. They will go through thorough testing and i will be using any cells from 2000-2400mAh. I get quite a few that are 2400mAh+ but i am using them for a different project of mine.
```

---
## \#2 Posted by: Krudte Posted at: 2016-05-05T13:44:55.519Z Reads: 744

```
13p?!?!  That's a lot of potential range......
```

---
## \#3 Posted by: Karmannghiagirl Posted at: 2016-05-05T13:49:59.261Z Reads: 755

```
[quote="seanpain4, post:1, topic:2919"]
budget is fairly limited at around $500
[/quote]

[quote="seanpain4, post:1, topic:2919"]
making a 6S13P 18650 Battery
[/quote]


lol wut? where did you buy those cells at that you were able to fit them into a $500 budget?
```

---
## \#4 Posted by: seanpain4 Posted at: 2016-05-05T13:51:43.552Z Reads: 723

```
Shit, i forgot to mention i am using recycled laptop batteries. 

They will go through testing and i will be using any cells from 2000-2200mAh.
```

---
## \#5 Posted by: laurnts Posted at: 2016-05-05T14:00:41.740Z Reads: 706

```
I am afraid laptop batteries wont work that well because they have very low discharge rating. Although you have 13p each batteries needd to he able to do continuos discharge about 10a to be stable. Not quiet sure if laptop battery spec able to do that.
```

---
## \#6 Posted by: treenutter Posted at: 2016-05-05T14:01:53.493Z Reads: 678

```
@seanpain4 that's the biggest 18650 DIY esk8 battery I've heard of! 32,500mAh! I'm looking forward to seeing it. 

What is the intended use of a pack like that? Some quick calculations, using average settings, tells me that is about 6.5 hours of ride time, which would easily get you 70 miles or so! How will you use it?
```

---
## \#7 Posted by: seanpain4 Posted at: 2016-05-05T14:07:16.024Z Reads: 653

```
@laurnts The max current draw from this motor will be about 60A. Divide that by 13 and it is only around 4.5, at peak.

Like i stated these batteries will be tested very thoroughly to ensure they can handle the work load.
```

---
## \#8 Posted by: seanpain4 Posted at: 2016-05-05T14:09:53.653Z Reads: 643

```
@treenutter I tend to walk/longboard around my town quite a bit. I often spend the day out and then i might spend the night at a friends place then ride my board to school, then that night i will go home. I intend to be able to go a couple of days without the need to charge the board or carry extra batteries or my charger with me. 

I also had access to lots of laptop batteries, so why not utilize that?

Plus, it seemed ridiculous so i thought it would be fun.
```

---
## \#9 Posted by: chaka Posted at: 2016-05-05T14:10:29.190Z Reads: 651

```
You will have a lot of fun with this build. Once you find out the capacity of each cell you will want to distribute them equally into each paralleled pack. Each pack should add up to same capacity if you distribute them accurately.

Get used cells rather than recycled if you can. You will get a lot of bad cells in "recycled" packs. 

A great way to discharge cells in mass is by making a balance harness with rare earth magnets soldered to the ends of the wires.  This way you can discharge many cells at once by connecting them in series with the magnetic balance wires.. Each time the discharge cycle completes pull the lowest cell and replace with a charged cell taking note of how many mAh have discharged. Next time the cycle completes you add the previous mAh measurement to get the total mAh of the remaining cells. There are a few more details to the process but it becomes clear once you begin implementing the technique.
```

---
## \#10 Posted by: seanpain4 Posted at: 2016-05-05T14:13:21.402Z Reads: 641

```
@chaka Majority of the packs are just used, not sourced from recycling facilities. 

I already have a very similar setup to what you are suggesting for the discharging of the cells. I discharge a large amount with an iMax B6 then i have a couple of 4 slot independent chargers that will charge them back up and tll me their capacity. So far i have processed around 50 cells and found about 44 usable cells.
```

---
## \#11 Posted by: Karmannghiagirl Posted at: 2016-05-05T14:17:36.232Z Reads: 627

```
I have seen them used for electric bikes. So i would assume they would be just fine.

https://www.youtube.com/watch?v=DJaToOJcZ_o
```

---
## \#12 Posted by: chaka Posted at: 2016-05-05T14:22:51.453Z Reads: 611

```
Sounds like you have done your research! @laurnts he  will be able to output close to 1500 watts continuous with bursts well over 2000 watts in a 6s13p configuration.  Most riders never use this much power.
```

---
## \#13 Posted by: treenutter Posted at: 2016-05-05T14:29:38.604Z Reads: 602

```
@seanpain4 Ridiculous is always fun! I love the idea of using upcylcled laptop batteries, I've seen folks do it for their bike packs and think that's it's both cost efficient and a nice way to use stuff that would otherwise be junk! It would be a  great contribution to the forum here if you documented how the build goes, what you have to do, etc.
```

---
## \#14 Posted by: seanpain4 Posted at: 2016-05-05T21:54:31.067Z Reads: 593

```
The main item i am waiting for is my Hot Glue Gun. Once i have that i can begin assembling my batteries.

By the time i get the batteries done, the other components that i am waiting for will arrive, these are, Motor, ESC, Controller/receiver, Pulley belt, 10AWG wire, along with some bullet connectors for the Motor to ESC. These are all due to arrive in the next week, maybe two weeks.
```

---
## \#15 Posted by: seanpain4 Posted at: 2016-05-06T08:26:40.154Z Reads: 609

```
UPDATE: I Started Re-Wrapping the tested cells that i am going to be using. 

I think i will be able to start making the batteries tonight or tomorrow.

Before, During and Afters:

<img src="/uploads/db1493/original/2X/3/3a6f70b23a4dcab224174586d488722c0fb540c2.jpg" width="333" height="250">

<img src="/uploads/db1493/original/2X/a/a4717c0c7322e0a79067fb8016b40b75b898f89a.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/f/fc4765721b3695e61d786a2a1360694c5d090cae.jpg" width="375" height="500">
```

---
## \#16 Posted by: seanpain4 Posted at: 2016-05-08T08:21:45.288Z Reads: 584

```
This is the board I'm going to use, bought it online from Awol Sports. It was pretty cheap and well made. I don't particularly like the branding on the grip tape or under the deck so i am planning on repainting it and putting new grip on. 

<img src="/uploads/db1493/original/2X/e/eff4f01637f8aca3b1a04d5b33226c311aebf7c8.jpg" width="285" height="350">

The trucks were originally mounted in a drop through style, but i will need to mount them under the deck as shown in the image. But as a result it leaves that hole there in the deck which i don't really like. So, as per @treenutter suggestion, i am going to fill the hole with some form of epoxy or resin. Then i can repaint the deck with my own design and then put some new grip on. You can see a close up below.

<img src="/uploads/db1493/original/2X/4/4135ec2e7db40c8ce88d43237b8c11edffa306da.jpg" width="285" height="375">
```

---
## \#17 Posted by: seanpain4 Posted at: 2016-05-10T12:43:34.517Z Reads: 572

```
Change of plan again. Instead of filling the hole with an epoxy or resin, i am going to get a cap 3D printed with the assistance of @Danpooed. I decided to go this route as i will be able to convert the board back if i ever decide to get a different deck. I will also be able to mount my XT90-s key loop on there as well so i dont have to plug it in underneath. 

I measured up the holes and came up with a 3D model using 123D. @Danpooed also assisted a little bit with this as well. 

Topside:
<img src="/uploads/db1493/original/2X/0/072fe7f98a9e7643530ceb96c8e238139cf1d685.png" width="345" height="236"> 

Underside: 
<img src="/uploads/db1493/original/2X/d/de6ccd21568c2210a8de4690039af01623b84146.png" width="345" height="151">
```

---
## \#18 Posted by: HTownBomber Posted at: 2016-05-10T12:59:07.934Z Reads: 552

```
Good idea. If you're running wires to the caps, you might as well integrate a USB port or LEDs in there for night riding. Hell, you could squeeze a voltmeter into the cap to better monitor your range while riding.
```

---
## \#19 Posted by: seanpain4 Posted at: 2016-05-10T13:01:04.934Z Reads: 558

```
Good ideas! 

I'm planning on adding some LED's underneath and maybe a couple facing forward to light up the path.
```

---
## \#20 Posted by: covert Posted at: 2016-05-12T07:36:32.326Z Reads: 550

```
I've seen this deck online. What are your thoughts on the flex and the feel under your feet ? It's the grip tape good ? I think the shape might be goof for the oversize wheels we tend to use on our E-Boards.
```

---
## \#22 Posted by: seanpain4 Posted at: 2016-05-12T08:00:10.339Z Reads: 523

```
For me the flex is good. I wanted it fairly stiff as i will have batteries running most of the wheel base, but also to have some flex for comfort. I am only light though (61kg).

Grip tape is pretty good. But i will most likely replace it as i don't like the logo on it.
```

---
## \#21 Posted by: lox897 Posted at: 2016-05-12T11:36:51.785Z Reads: 477

```
2 posts were split to a new topic: [Where can I find the best motor parts?](/t/where-can-i-find-the-best-motor-parts/3166)
```

---
## \#23 Posted by: seanpain4 Posted at: 2016-05-13T12:46:26.814Z Reads: 549

```
Electronics Update!

All of my electronic components have arrived and i have been soldering on the XT60 and bullet connectors. 

<img src="/uploads/db1493/original/2X/5/5e6e941b6be31ab8fadf6863a5b64f7df05a0cef.jpg" width="188" height="250">

<img src="/uploads/db1493/original/2X/4/4dad86a41a954ac35359c2b24c0c889452d04e82.jpg" width="333" height="250">

Tightly packed enclosure. I will be getting a custom enclosure 3D printed. 
<img src="/uploads/db1493/original/2X/b/bf5a72d23757325d4a43d4309ad0b7d35169577d.jpg" width="333" height="250">

Had to modify the 3 pin connector as it sat up too high and wouldn't allow the lid to close. 
<img src="/uploads/db1493/original/2X/d/d8c80fd60cbf66cda4b2844dc2171f23e06d2e2c.jpg" width="188" height="250">
```

---
## \#24 Posted by: seanpain4 Posted at: 2016-05-13T12:56:53.595Z Reads: 542

```
Still processing batteries. I have been able to speed up my process to about 8 a day. and about 70% are usable cells.

<img src="/uploads/db1493/original/2X/2/2ecf239a9416b29f7b56f6b52efa3db8110b07a3.jpg" width="333" height="250">

<img src="/uploads/db1493/original/2X/2/253c0d884d43c30c79c81cfbbec81c12827ded0f.jpg" width="333" height="250">
```

---
## \#25 Posted by: seanpain4 Posted at: 2016-05-16T14:14:28.014Z Reads: 544

```
**Update!** 

@Chris_KP I did the wire mod to my SK3. I used about 8cm lengths of black 10AWG Silicon wire. 

I think it turned out pretty good. Only issue i had was scraping of the enamel coating on the wire so i could solder to it correctly. Other than that, no issues. 

<img src="/uploads/db1493/original/2X/e/e6d7a1dc09b17e25d4866a73608cb379accfd682.jpg" width="333" height="250">

<img src="/uploads/db1493/original/2X/5/5c272004527491208e57b36f6dc7084c38f98d0e.jpg" width="333" height="250">

<img src="/uploads/db1493/original/2X/6/645216598a41e9a47933988d117e8f6c56cc339b.jpg" width="333" height="250">
```

---
## \#26 Posted by: seanpain4 Posted at: 2016-05-16T14:23:02.038Z Reads: 536

```
**Another Update!**

I am still sorting and testing cells. I am going to start building my packs when i have all 78 of them so that i can distribute the cells evenly, to result in even capacity packs. 

This pack that i build was just made out of lower capacity cells and is a 6S2P pack. I needed some power source to power up all my electronics to make sure everything was working correctly, and i wasn't going to use those cells for anything else.


This is basically what my 6 proper 1S13P packs will look like, just with one extra cell in it. 

<img src="/uploads/db1493/original/2X/1/1d96e6be543f9b9261a4d3a447509ce0aedf0fa6.jpg" width="333" height="250">

<img src="/uploads/db1493/original/2X/9/9de915f8c229e0b0f27e767c782cb06275817d23.jpg" width="333" height="250">
```

---
## \#27 Posted by: Chris_KP Posted at: 2016-05-17T00:05:55.027Z Reads: 514

```
Nice work! I forgot to mention that about the enamel coating. 
Those battery's are looking great Im saving up laptop 18650s as we speak!
```

---
## \#30 Posted by: OskarCastrone Posted at: 2016-05-17T19:10:17.045Z Reads: 505

```
Will you be selling these? 
I would love to buy some pre-assembled packs from you! You seem like you know your shit :D
```

---
## \#31 Posted by: seanpain4 Posted at: 2016-05-17T21:26:11.474Z Reads: 502

```
Probably not, I just don't have the time to make any more than I need
```

---
## \#32 Posted by: OskarCastrone Posted at: 2016-05-17T22:31:29.334Z Reads: 491

```
Well, that's a shame! :)
```

---
## \#33 Posted by: DeathCookies Posted at: 2016-05-18T07:45:40.350Z Reads: 491

```
[quote="seanpain4, post:23, topic:2919"]
All of my electronic components have arrived
[/quote]

I just noticed that you have a quanum transmitter. Well i had this one too and it is very bad...honestly it is crap. You should better buy a GT2E or GT2B (older version) because it is much better.

With the quanum transmitter the binding is hard. It takes just soooo long. Sometimes i need to rebind it to get it working...Since i used my GT2E i will never change my transmitter. Maybe i use sometimes a nunchuck or steez but i dont use this transmitter voluntary.

But this is just my opinion.
```

---
## \#34 Posted by: seanpain4 Posted at: 2016-05-18T07:49:10.013Z Reads: 461

```
[quote="DeathCookies, post:33, topic:2919"]
With the quanum transmitter the binding is hard.
[/quote]

It is almost instantaneous, one of the easiest remotes i have every had to bind. 

I haven't had any issues with binding on my remote as of yet. I have tested the range and its awesome.

May have just been yours. 

Also, IMO the GT2E looks like shit and is too bulky. the Quanum is a lot more slimline and compact.
```

---
## \#35 Posted by: DeathCookies Posted at: 2016-05-18T07:53:44.558Z Reads: 471

```
[quote="seanpain4, post:34, topic:2919"]
It is almost instantaneous, one of the easiest remotes i have every had to bind. 

I haven't had any issues with binding on my remote as of yet. I have tested the range and its awesome.

May have just been yours.
[/quote]

Well... maybe? I dont know but i did read some people hating this transmitter as well... But if you are happy with it stick with it ;)


[quote="seanpain4, post:34, topic:2919"]
Also, IMO the GT2E looks like shit and is too bulky. the Quanum is a lot more slimline and compact.
[/quote]

That was the reason why i bought the same transmitter. But the GT2E feels like it has wider pulsewidth and is much more accurate (for me). But i am going to print the GT2E custom enclosure and then it will be the perfect transmitter ?! :D
```

---
## \#36 Posted by: mcfly777 Posted at: 2016-05-18T17:27:00.998Z Reads: 459

```
Hi Sean
Really like how you're putting together the battery packs. I also have access to used laptop batteries, and am considering doing something similar to what you're doing. A few questions
- what is your workflow for each cell? discharge, charge to full and log the mAh ?
- how do you know when a cell is bad?
- how are you grouping the cells in each pack?
- will you use a BMS for all this? if so, which one?

Sorry these are many questions but I want to make sure I get it right. I'm probably going to build something smaller, perhaps 8s4p. I'm thinking of 3d printing the cell spacers so I can just line them up first, then solder, then wrap. 

thanks
```

---
## \#37 Posted by: monkey32 Posted at: 2016-05-19T08:52:37.432Z Reads: 430

```
endless sphere > Batteries and battery tech may be useful
```

---
## \#38 Posted by: seanpain4 Posted at: 2016-05-19T10:54:43.995Z Reads: 470

```
[quote="mcfly777, post:36, topic:2919"]
- what is your workflow for each cell? discharge, charge to full and log the mAh ?
- how do you know when a cell is bad?
[/quote]

I charge every single cell to max. Through the charging process if the cell gets hot or even too warm then i will take it out and put it in the dud pile. Or if the cell won't charge i will also put it in the dud pile. Once i have enough cells charged up, i connect about 8 in parallel and then discharge them to about 3.3v. I then put them in a charger that charges each cell individually and gives you the capacity of each cell. I write the capacity on the cell and put it in my tested pile. 

[quote="mcfly777, post:36, topic:2919"]
- how are you grouping the cells in each pack?
[/quote]

Once i get all 78 cells i will order them from smallest to the largest that i am using. I am using the 2400mAh+ cells for a different project so for this i am using 2000mAh - 2400mAh cells. Once in order from smallest to largest i will grab equal quantities from each end to make a pack. Each pack is 13P.

[quote="mcfly777, post:36, topic:2919"]
- will you use a BMS for all this? if so, which one?
[/quote]

Currently i will just have some small JST connectors coming out of each parallel pack and then i will make a harness that i can hook up when i want to charge up the battery. I will be using my iMax B6 to charge my packs. In the future i will probably change the configuration of the cells to probably 10S. When i do that i will buy a BMS.
```

---
## \#39 Posted by: seanpain4 Posted at: 2016-05-19T10:56:38.929Z Reads: 450

```
@monkey32 Thanks, but i don't need any assistance in making the packs :) I have been making them for a while.
```

---
## \#40 Posted by: seanpain4 Posted at: 2016-05-19T11:06:09.719Z Reads: 473

```
**Very Small Update!** 

Currently waiting on a  couple tools so that i can drill out my mount and get the truck hole to the right diameter to be welded to the truck. 

Also made my anti-spark loop with an XT-90S. I also found out that 18650 PVC wrap is the perfect size for wrapping an XT-90S, which is pretty cool.


<img src="/uploads/db1493/original/2X/7/7ab3ad1407da8782d496bcc72025ede18965a2a0.jpg" width="188" height="250">   <img src="/uploads/db1493/original/2X/9/9f52036a430d92c57b62d6f017d590f436210ac6.jpg" width="188" height="250">
```

---
## \#41 Posted by: monkey32 Posted at: 2016-05-19T13:42:30.957Z Reads: 461

```
 appologize for not being clearer. that was a comment @macfly777
```

---
## \#42 Posted by: mcfly777 Posted at: 2016-05-19T15:15:50.839Z Reads: 455

```
Thanks Sean for the detailed response. I have 2 LiPo packs right now that I'll use as a 6s system, but I'm already looking at upgrading it, mostly for greater range.
```

---
## \#43 Posted by: chaka Posted at: 2016-05-19T15:32:12.843Z Reads: 425

```
Nice work! Looks clean, you are going to be really happy with this pack when you are done. However that Quanum is going to leave you stranded 20 mile out if you don't heed our warnings. 

I think the problem is the trim pots, they seem to fail by not allowing the throttle to reach 50% in order to bind. First you will notice that you need to adjust the throttle pot constantly followed by difficult binding and eventual total failure to bind.

The battery life is another terrible aspect of this remote. Even when switched off it continues to drain the cells.
```

---
## \#44 Posted by: seanpain4 Posted at: 2016-05-19T22:15:55.790Z Reads: 429

```
[quote="monkey32, post:41, topic:2919, full:true"]
appologize for not being clearer. that was a comment @macfly777
[/quote]

Oh, sorry about that

[quote="chaka, post:43, topic:2919"]
However that Quanum is going to leave you stranded 20 mile out if you don't heed our warnings.
[/quote]

Now that I have seen that 3D printed casing for the GT2E, I think i might get one. But I will see how this goes first
```

---
## \#45 Posted by: Chris_KP Posted at: 2016-05-21T23:15:05.925Z Reads: 397

```
Where did you get the XT-90s in aus?
```

---
## \#46 Posted by: seanpain4 Posted at: 2016-05-21T23:59:11.311Z Reads: 388

```
I bought it on eBay from China :slight_smile:
```

---
## \#47 Posted by: seanpain4 Posted at: 2016-06-08T08:59:49.530Z Reads: 383

```
**Small update!**

I am about to start making my battery packs. Although i have decided to go with 11P instead of 13P. This will probably reduce the size of the battery by about 100Wh. But it will cut down on about half a kilo of weight. And save me some time.

More updates to come soon!
```

---
## \#48 Posted by: lox897 Posted at: 2016-06-08T09:00:37.017Z Reads: 370

```
What are your total wh now?
```

---
## \#49 Posted by: seanpain4 Posted at: 2016-06-08T09:01:55.031Z Reads: 358

```
It will be approximately 540Wh
```

---
## \#50 Posted by: lox897 Posted at: 2016-06-08T09:02:41.966Z Reads: 362

```
Nice. Are you going to have a trailer to carry that monster? :joy:
```

---
## \#51 Posted by: seanpain4 Posted at: 2016-06-08T09:08:16.688Z Reads: 369

```
Haha, may as well. 

I am having 6 separate packs that will be held on by heavy duty velcro and eventually a custom cover.
```

---
## \#52 Posted by: zk8_builder Posted at: 2016-06-08T09:25:14.854Z Reads: 359

```
If you don't mind me asking a few question:
1. What was your succes rate for finding cells with your desired mah
2. Aprox how long did it take to test the mah of a cell
3. How many volts are you looking at per cell
```

---
## \#53 Posted by: seanpain4 Posted at: 2016-06-08T09:35:45.440Z Reads: 374

```
1. Probably around 70% are greater than 2Ah, which is the minimum capacity i am using. 
2. I charge every cell up to about 4.2v then discharge 8 on my imax b6 then charge 4 at a time on a charger that charges them individually and gives me their capacity.
3. Not entirely sure what you mean.
```

---
## \#54 Posted by: zk8_builder Posted at: 2016-06-08T09:58:34.445Z Reads: 375

```
What my third question is saying is that each cell (so for you 11 batteries in series) has to equal the same voltage
```

---
## \#55 Posted by: seanpain4 Posted at: 2016-06-08T10:03:06.921Z Reads: 392

```
11 cells in parallel? At the end of the testing they will be at around 4.15v and i will leave them at that until i connect them all together.
```

---
## \#56 Posted by: zk8_builder Posted at: 2016-06-08T10:19:21.083Z Reads: 406

```
Still not sure we are on the same
Page I will do a diagram <img src="/uploads/db1493/original/2X/2/26c65d643013a60a7c46f68bbadb070a84f81330.jpg" width="375" height="500">
```

---
## \#57 Posted by: Maxid Posted at: 2016-06-08T10:24:43.756Z Reads: 378

```
No they don't. In series it does not matter as voltages just add up.
In parallel they need to be the same. So in your case the 2 batteries in each pack need to be identical.
```

---
## \#58 Posted by: zk8_builder Posted at: 2016-06-08T10:29:25.916Z Reads: 368

```
so if my first set of cells that are in parallel add up to a average voltage of 4v and my second set of cells that are in series add up to 4.2v this is okay even though one set will have more than the other
```

---
## \#59 Posted by: zk8_builder Posted at: 2016-06-08T10:34:10.350Z Reads: 364

```
so as long as in the first set there is 2 4v it is fine and in the second 2 4.2v?
```

---
## \#60 Posted by: Maxid Posted at: 2016-06-08T10:37:17.944Z Reads: 379

```
[quote="zk8_builder, post:58, topic:2919, full:true"]
so if my first set of cells that are in parallel add up to a average voltage of 4v 
[/quote]
they don't add up in a parallel set - that is why they need to be the same.
[quote="zk8_builder, post:58, topic:2919, full:true"]
and my second set of cells that are in series add up to 4.2v this is okay even though one set will have more than the other
[/quote]
in series it does not matter if there are differences
```

---
## \#61 Posted by: zk8_builder Posted at: 2016-06-08T10:38:27.399Z Reads: 352

```
what needs to be the same? sorry really confused thanks for all your help
```

---
## \#62 Posted by: Maxid Posted at: 2016-06-08T10:58:47.789Z Reads: 359

```
Again:
Voltages in parallel group -> need to be the same.
Voltages in series -> can be different.

In your example it twas 6S2P so:
the six packs can be different from each other - the voltage will be added
the two batteries in a pack need to have identical voltages
```

---
## \#63 Posted by: zk8_builder Posted at: 2016-06-08T10:59:41.344Z Reads: 329

```
so if i was making a 1s 2p pack both of the cells would have to be identical in voltage but not in parralel
```

---
## \#64 Posted by: zk8_builder Posted at: 2016-06-08T11:00:00.162Z Reads: 324

```
it meant to be but not in mah
```

---
## \#65 Posted by: seanpain4 Posted at: 2016-06-08T11:10:06.503Z Reads: 332

```
Okay, jsut toclear things up. 

If two cells are placed into parallel and are a different voltage they will eventually even out to the same voltage. 

When two cells are placed in series that are a different voltage then they will stay like that and not balance. This is bad because one will end up getting over discharged and one will get over charged. 

It is just best to have all cells at the same voltage.
```

---
## \#66 Posted by: Maxid Posted at: 2016-06-08T11:31:33.227Z Reads: 345

```
[quote="seanpain4, post:65, topic:2919, full:true"]
If two cells are placed into parallel and are a different voltage they will eventually even out to the same voltage. 
[/quote]

Sure - but that makes it sound like as if it is not a problem and you could easily do that everytime.
With slight voltage differences this might not be a problem but could be really dangerous at higher differences when a large current will be supplied by the battery with higher voltage.

A quote from endless-sphere user dogman dan:
> In paralell connections, different chemistry OK, different ah size OK but best if not hugely different. Different voltage, Not OK. Voltage can be a little off, like the difference between 24v sla and 24v lifepo4.

> Series connections, Idealy eveything the same except for voltage. Some have gotten away with different chemistries but whether it works or not depends on how similar the internal resistance of each one is. Different voltages are ok, like a 24v with a 36 v.
```

---
## \#67 Posted by: seanpain4 Posted at: 2016-06-08T11:36:33.407Z Reads: 317

```
The current flowing from a cell at 4.2v to a cell at 3.5v is fairly negligible compared to how much current will be getting pulled from the motor. It is usually only around 1.4A and drops a fair bit within 1 minute.

 There isn't a huge rush of current flowing between them, unless you are using a few fully charged cells and one discharged cell.
```

---
## \#68 Posted by: zk8_builder Posted at: 2016-06-08T11:47:00.806Z Reads: 310

```
All I'm hearing is that it is better to have every cell at the same voltage
```

---
## \#69 Posted by: seanpain4 Posted at: 2016-06-08T11:47:45.996Z Reads: 316

```
That is the general rule to go by.
```

---
## \#70 Posted by: zk8_builder Posted at: 2016-06-08T11:50:43.493Z Reads: 313

```
Surely that means you were not getting 70% of your batteries to have the same voltage
```

---
## \#71 Posted by: seanpain4 Posted at: 2016-06-08T11:56:18.447Z Reads: 313

```
No, when they come out of the laptop batteries they are at different voltages. 

70% of the cells i get have a capacity of 2,000mAh or above. They are the ones i use
```

---
## \#72 Posted by: zk8_builder Posted at: 2016-06-08T11:57:06.648Z Reads: 305

```
I am also taking out of laptop batteries how can i solve the voltage problem now
```

---
## \#73 Posted by: Maxid Posted at: 2016-06-08T11:57:10.794Z Reads: 308

```
you do realize that you can charge batteries to be at the same voltage? He was talking about the capacity - 70% of the batteries can still hold a charge and have between 2000-2400mAh
Edit: too late
Edit2: I get the feeling that you should not be doing this type of work.
```

---
## \#74 Posted by: zk8_builder Posted at: 2016-06-08T12:03:26.942Z Reads: 311

```
I do get that but you guys seem to be contradicting each other that is what is confusing me. So I would like you to forget what has been discussed now come in open minded and tell me how I can get each battery to have the same voltage
```

---
## \#75 Posted by: seanpain4 Posted at: 2016-06-08T12:03:47.762Z Reads: 306

```
What is the voltage problem? You take them out and charge them to the same voltage?

Are you sure you are able to do this? It can be quite dangerous if you don't know what you are doing.
```

---
## \#76 Posted by: zk8_builder Posted at: 2016-06-08T12:05:16.599Z Reads: 311

```
Firstly I am capable and I will have assistance from professionals
```

---
## \#77 Posted by: zk8_builder Posted at: 2016-06-08T12:10:44.869Z Reads: 321

```
The problem is that you first tell me that I should have all my cells at the same voltage then you says they can all be diffrent
```

---
## \#78 Posted by: seanpain4 Posted at: 2016-06-08T12:15:39.371Z Reads: 324

```
You are misunderstanding, each laptop battery will be at a different voltage to the next. Once you pull the cells out, you put them into a charger and charge all of them up to 4.2v so they are all the same.
```

---
## \#79 Posted by: zk8_builder Posted at: 2016-06-08T12:20:21.956Z Reads: 320

```
So weather I buy a battery I will always be able to put it up to 4.2v
```

---
## \#80 Posted by: zk8_builder Posted at: 2016-06-08T12:20:47.363Z Reads: 324

```
I think with both just landed on the same page
```

---
## \#81 Posted by: seanpain4 Posted at: 2016-06-08T12:21:10.351Z Reads: 324

```
as long as it is Li-Ion cells that are in the laptop battery
```

---
## \#82 Posted by: zk8_builder Posted at: 2016-06-08T12:25:06.393Z Reads: 335

```
Ok thanks
So when assembling a pack you would have every cell charged at 4.2v and then now to parallel does each set of cells in parallel have to have the same voltage
```

---
## \#83 Posted by: seanpain4 Posted at: 2016-06-08T12:26:48.884Z Reads: 298

```
Just have every parallel pack at the same voltage with the same voltage cells.
```

---
## \#84 Posted by: zk8_builder Posted at: 2016-06-08T12:28:01.370Z Reads: 310

```
Yes but say I have 6 sets of 3cells in parallel do all 6 sets need to have the same ah
```

---
## \#85 Posted by: seanpain4 Posted at: 2016-06-08T12:40:02.231Z Reads: 334

```
Get the 6 sets to have the closest Ah possible. My 6 packs deviate by about 1% so they are really close to each other.
```

---
## \#86 Posted by: zk8_builder Posted at: 2016-06-08T21:20:53.313Z Reads: 343

```
Ok that's what I thought
```

---
## \#87 Posted by: seanpain4 Posted at: 2016-06-10T02:38:34.551Z Reads: 370

```
**Update!**

I have separated all of my cells into their 6 individual packs. After about half an hour i have got their capacities within 60mAh of each other which is a tiny difference compared to each one being about 29,000mAh.

I have also PVC wrapped, pre tinned and hot glued two packs of the 6. Next up is to solder the two packs and add some wires then do the final PVC wrap! And of course, do it for the other 4 packs. 

<img src="/uploads/db1493/original/2X/3/3d7f7f8bd3a4d75dfa4d575f9e170d1203fb0eb7.jpg" width="188" height="250">

<img src="/uploads/db1493/original/2X/0/0082ebf21328a8d18e66274a2d7f1f5b7274aa5e.jpg" width="333" height="250">

<img src="/uploads/db1493/original/2X/e/e7462a61bc5537afe7e56b5d5959b0990b7d09b4.jpg" width="188" height="250">
```

---
## \#88 Posted by: paoloalb Posted at: 2016-07-01T14:43:01.578Z Reads: 335

```
Nice! I found just now this thread and it is very useful for me cause I'm planning on using laptop batteries too. You talked about using a BMS for 10s batteries, so I assume I should buy one cause I want to make a 12s pack. Do you have something to suggest me about what BMS to buy? Also is it possible to run a powerful motor using 18650 cells arranged in a 12s 2p configuration, or should I use more parallel cells? I was thinking about the sk3 149 kv ( it's about 2700 W at maximum load)
```

---
## \#89 Posted by: Pantologist Posted at: 2016-07-01T14:52:52.822Z Reads: 339

```
The max current draw I've seen from laptop battery cells is around 5-10A. A 2P pack will not be enough. You'll probably have to do like a 4p pack to safely run a motor, but even then, the cells might not be able to handle max current ratings being already used. 

I suggest getting some new cells. A 12s2p Samsung 25R pack would be a far better idea.

Check out bestechpower for some BMS boards.
```

---
## \#90 Posted by: psychotiller Posted at: 2016-07-01T15:00:46.177Z Reads: 335

```
Nope! I had 3. That remote has major issues. Once the binding issue starts with them they are useless.
```

---
## \#91 Posted by: OskarCastrone Posted at: 2016-07-02T14:01:16.942Z Reads: 327

```
I have had the same experience as Psychotiller... That remote is crab!
```

---
## \#92 Posted by: Weberp7593 Posted at: 2016-08-28T20:12:31.346Z Reads: 299

```
http://mo-bo.de/product_info.php?info=p755_mo-bo---ersatz-akku---lithium-36v-48ah---block---panasonic-cells.html :slight_smile:
```

---
## \#93 Posted by: Okami Posted at: 2017-01-15T02:52:41.483Z Reads: 208

```
Do you have any more pics to share?

It looks like your diy laptop battery pack build caught a lot of attention.. 

:slight_smile:
Would be interested in the final parameters of the pack you made.. if you sticked to 11p, that would mean over 20ah probably :)
```

---
## \#94 Posted by: thepali94 Posted at: 2017-09-19T08:55:31.891Z Reads: 115

```
Hi,

Where/How do you get all those laptop batteries? And are those all 18650?
```

---
## \#95 Posted by: Tijmen Posted at: 2018-01-22T20:47:29.397Z Reads: 74

```
Update to this build? :D I'm intrigued!
```

---

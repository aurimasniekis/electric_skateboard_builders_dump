# New user looking for battery? Read this - COMPLETE WALKTHROUGH OF BATTERIES

### Replies: 89 Views: 18095

## \#1 Posted by: evoheyax Posted at: 2017-06-23T19:12:21.904Z Reads: 1728

```
So I was recently asked for a good link to a break down about batteries. Unfortunately, I didn't have a good link to point him to, so I wrote my own. I decided to share it and build on top of it for the community. I will try to remove my opinions as much as possible, so sorry if I seem biased at times.

**A FOR WARNING:** Take all manufacturer ratings with a grain of salt. A guy on reddit named mooch315 has tested a lot of cells of all different formats, but especially 18650s, and you can find those test results [here](https://www.e-cigarette-forum.com/forum/blog-entry/list-of-battery-tests.7436/). His tests show some cells rated to 15a are actually higher discharge cells then some that are rated to 30a. Manufacturers do their own testing, so mooch315's goal is to give the world an objective rating and view of the cells he tests.


----------

**Formulas you need to know:**


----------

    mAh = 1000*Ah
    Wh = Ah * max voltage
    W = Amps now * voltage now



----------
**Lipo vs Li-ion**

----------

Li-ion is great for:

- Flat ground riding
- Riding slowly
- Light riders

Unless you do a really large pack (6p or higher at 10s or 12s). They sag, which means the voltage drops quickly for a short period of time under heavy discharge, to go back up to slightly less than where is was before the heavy discharge after the heavy discharge is over. If your using current control (as most are with the VESC), this means you lose power (since you have less watts, reference formula #3 above). They are incredibly safe. The tests they do which are listed in the spec sheet are incredibly abusive, yet none caused a fire or explosion. Likely most of those same tests on a lipo would cause a fire or explosion. Larger packs (10s7p or 12s6p or larger) can overcome the sagging issue, as does setting your amp limits lower. Most cells say you can discharge up to 20 amps continuous. However, you will lose quite a bit of range at that number, and you want to aim for more like 10 amps continuous per cell in parallel.

Lipos give better performance if using a smaller pack, but they can't take abuse well (discharging too low or over charging too high), and can become volatile. The discharge curve is different. Li-ion drop off a lot at the beginning, and then discharge at a steady decline. Lipos drop off a lot at the beginning, and then slowly decrease in voltage, and around 3/4ths of the way through the discharge, they drop off a cliff. The result is lipos give a better performance in current control mode than li-ion batteries of the same size (i.e voltage and Ah).

There is a newer firmware mod which was created by @Ackmaniac that allows for watt control mode, which should get ride of this problem. But that's another whole discussion in it's own.

Here's the is discharge curves of an average lipo and li-ion cell. Look at how quickly the line going from right to left goes down.

NOTE: Not all lipos or li-ion cells discharge exactly like this. This is a generality.

**Lipo Discharge Curve:**
http://rightbattery.com/wp-content/uploads/2013/10/2s-life-700-mah-zippy-5c-battery-capacity.jpg

**Li-ion Discharge Curve**
https://is.alicdn.com/img/pb/962/532/197/1197532962_998.jpg


Li-ion cells come in a few varieties. The most common is the 18650. The 18 refers to the diameter of the cell in mm, and the 65 refers to the length of the cell in mm. There's also the 26650. The most common 26650 cell is the A123 cell.

Lipo cells come in all manners of shapes an sizes, expect cylindrical cells (funny enough). They can be very flat, or very thick, in any of the x, y or z directions. Instead of a storing energy in this cylindrical shell, they energy in a pouch. This pouch is easy to puncture, unlike the li-ion cylindrical shell, which is one of their weaknesses. I don't think I need to tell you want happens when you puncture a lipo battery.

http://www.sharegif.com/wp-content/uploads/2013/10/08/explosion-gif-81.gif

Another thing. Lipos are rated to around 1/3rd of the life cycle of li-ion packs. So while lipos look cheaper up front, li-ion can be cheaper in the long run if you take good care of the cells. Obviously, the higher rate of discharge per cell in li-ion packs, the less life they will have. This is not a linear thing, so a 12s3p will not have half of the life cycle of a 12s6p. At 20a con, the cell only gets 400 full cycles. at 10a max, you get 1200 full cycles. so the 12s6p should in theory, if they are both ran at the same max amps, get 3 times the life, not double the life, of the 12s3p.

So to sum it up, heres the cost/benefit analysis.

**Li-ion Pros**

- Safer (by a lot)
- Longer life cycle

**Lipo Pros**

- Sags less (thus when you draw high amps in current control mode, which most use with the VESC, you don't lose power (and in this case, power refers to speed and/or acceleration))
- Cheaper
- Can be put into shapes not possible with a li-ion cell (great for boards that need to be thinner than 18mm)

I should mention now, that there is another technology called LiFePO4 or Lithium Iron. These give you the same shape as a lipo, same high discharge rates of a lipo, but are safer and have a longer life cycle than lipos. Seems like a win-win, but they are very expensive compared to both li-ion and lipo, and theres not a lot of sources out there for Lithium Iron batteries, so they are not very commonly used.

----------

**Parallel vs Series**

----------

Theres 2 configurations of cells. Parallel and series.

http://www.12voltbattery.info/images/content/batteryWireDiagram.jpg

Parallel means negative to negative and positive to positive. The result is two cells become essentially one. They will automatically balance each other out to the same voltage. Parallel config doubles the Ah, meaning you'll get more range.

Series means the voltage is doubled and the Ah stays the same. To do this config, hook one positive to one negative, and use the open positive on the one cell and open negative on the other cell to discharge.

Higher voltage means more power and less amps need to be drawn.
Higher Ah means longer range.

However, Wh or Watt Hours is the best measurement of the size of a battery.

Stay you have 12 li-ion cells. The typical li-ion cell is 2500 mAh in size, and is a 1s (since it's 1 cell at a 3.7 nominal voltage).

You could do a a 12s1p (12 cells in series, 1 cell in parallel) or 1s12p (1 cell in series, 12 cells in parallel) or, since nobody would typically do either of those con figs (unless using the A123 cells, which are the cells boosted uses, in a 12s1p), a 6s2p would be usable, but still weak. The point though, is going between series and parallel, they all have the same Wh, since we have the same amount of electricity being stored in all of those configs.

Most people aim for a 10s or 12s, because you can get a lot of power and draw less amps. The more amps you draw from your battery, the hotter your battery and esc will get.

Many still use a 8s or 6s battery, but it's more of a budget board thing. Boards at those voltages are weak when compared to the same board at 10s or 12s.

To get more range though, since you can't really go higher than 12s (very few esc's can handle higher than 12s), you put more cells in parallel to get more range.

Back to our example, a typical li-ion battery in:

    12s1p will have 2.5 Ah total at 50.4 volts. 2.5 x 50.4 = 126 Wh
    6s2p will have 5 Ah total at 25.2 volts. 5 x 25.2 = 126 Wh
    1s12p will have 30 Ah total at 4.2 volts. 30 x 4.2 = 126 Wh

No matter the config, all of these batteries will have around the same range, since you have the same amount of cells (thus same amount of electricity) in all of these configs.

This is why when comparing peoples batteries sizes and ranges on here, we usually reference the Wh of our packs, not just the S and P of the pack.

IMPORTANT NOTE: The legal limit to fly on an airplane in the US with a battery is 99 Wh, so if that's important to you, keep this in mind. Europe has similar rules also.


----------

**Sag**


----------

Sag is directly correlated between max amps you will draw to max amps you can draw. if you plan to draw no more than 60 amps, and have 240 amps, your result is little sag. If both of those numbers are 60, expect a large amount of sag, which means decreased performance and less range.

Sag is completely normal, in both lipo and li-ion cells. They will both sag, but to different degrees.

----------

**Charging Batteries**


----------

Li-ion cells are pretty easy to charge. You can use a standard "laptop" style charger at the max voltage of your battery pack (for example, a 12s battery needs a 50.4v charger, since 4.2 (max voltage per cell)  x 12 (number of cells in series) = 50.4). Most Li-ion packs use a BMS or Battery Management System.

Lipo batteries however are usually charged using a balance charger. These chargers accomplish the same goal of balancing the cells during charging as the BMS, but without the need for a BMS. The downside is you need to plug balance cables into the balance charger, so charging now means more cables to deal with.

Both li-ion and lipos can be charged through balance chargers or laptop style chargers (with or without a BMS). You would not use a BMS and balance charger together however.

Most use balance chargers with lipos because a balance charger is cheaper and easier to use than a BMS, and lipos, according to manufacturer data, last about 1/3 of the life cycle of li-ions. Li-ion batteries are more expensive and last 3x times longer (again, theoretically), so a bit extra for the convince of the BMS makes sense. However, a BMS for a lipo is not a bad idea if you plan on replacing your lipos with the same lipos when they die, as you can use the BMS with the new battery pack, since it's the same battery.

----------

**Battery Management Systems**


----------
Most li-ion batteries use BMS's, but most lipo packs do not. The reason being lipos are usually charged using a balance charger, while li-ion's use a "laptop" style charger. The "laptop" style charger simple provides a voltage at a constant amperage. The battery charger does exactly that too, but when a cell reaches 4.2 volts, it will start discharging is at the same rate through that cells balance lead, thus leaving that cell at 4.2 while the rest of them catch up. The BMS does exactly the same thing.

The goal of the BMS is simple: make sure the cells are all very close to the same voltage after a full charge, prevent cells from discharging too low, and prevent cells from being charged too high. Since the VESC can prevent cells from discharging too low, most just use the balancing and preventing cells from charging too high features of the BMS.

Again, as stated above, both a BMS and Balance charger accomplish the same goal with respect to charging. The BMS is more convenient though, as you need 1 cable instead of multiple to charge.

**My opinion about flying with batteries**


----------
If you want hot swappable batteries that are under 99 Wh, Lipos are a better option IMO because 99 wh 18650 li-ion batteries will not output very many amps. This will result is horrible sagging and a bad experience (to me at least, cause I like a lot of power).

The Lipos I recommend are the Zippy Flight Max 8000 mAh series, either 2s, 3s or 6s linked in series. The 30c version at 12s and 8 Ah is capable of 240 amps continuous. The li-ion version of that would be basically a 12s3p, which is capable of 60 amps continuous. Remember, always take advertised numbers with a grain of salt also. Most of us will want 60 amps at least continuous. Though that 12s3p li-ion can do 60 amps continuous, it will sag very badly.




----------
**My Recomendations**


----------
If you do use lipos, get a good balance charger (not a knock off imax, cause those things are dangerous) and set it up so you can charge them quickly (if doing 4x3s, wire it so you can disconnect and charge them as 2x 6s's, since most lipo chargers are limited to 6s, and they'll charge faster this way). If you take care of them, lipos are safe. I've used over well over $1000 worth of lipos (which is quite a few battery packs) without any incidents, even when I have abused them. All lipo fires (besides when theres a known problem with a cell) start during charging or discharging, and almost always, it's during charging. That's why a good balance charger is important. They will almost certainly not explode if they are not charging or discharging, unless you puncture a cell or physically abuse the cell.

If you use li-ion, try to keep it to 10a max per cell in Parallel. This will reduce sag, increase battery life, and increase range. This can be tricky, which is why I recommend a 12s6p (the same pack that @chaka also recommends to eliminate sag) or higher in size. Smaller packs will work, but they will negatively impact performance.



----------
**Sourcing**
----------
The biggest problem for batteries is finding where to buy them.

Lipos are easy, I'd recommend [HobbyKing](https://hobbyking.com/en_us/lipo.html) first and foremost. They have a great battery finder that helps you find a battery that will fit to your specs.

Li-ion however, is hard. There are so many knockoffs out that that even telling the difference between a real and fake cell is almost impossible without testing the cells first for performance. I know some have recommended [Battery Bro](https://batterybro.com/) before. If others have some recommendations, please post below and I will update this. Amazon is hit or miss, and banggood from what I've seen is mostly miss.

For BMS's, [Best Tech Power](http://www.bestechpower.com/pcmbmspcbforli-ionli-polymerbatterypacks/) and [Su Power Battery](http://www.batterysupports.com/battery-pcbnbsp-bmsnbsp-pcm-c-32.html) are both commonly used sources.

----------
**Final Thoughts**



----------

I hope the world of batteries is a bit clearer to you now. Everything in this guide is what I have learned through first hand experience of building and testing electric skateboards for the past 2 years. If anything seems mis-leading or incorrect, as always, please let me know. My aim is to be as factual as possible, while giving new users a good insight into batteries.
```

---
## \#2 Posted by: Hummie Posted at: 2017-06-23T19:40:22.781Z Reads: 1224

```
another option lifepo4 or li-IRON which have about 4 times the cycle life of li-ion and you can literally cut a charged cell in half with a saw (done on endless-sphere), and it rebounds from over- charging or over discharging really well.  They run at a slightly lower voltage and they aren't quiet as energy dense so bigger and heavier and more expensive but looking at the cycle life it ends up being cheaper long run and piece of mind knowing no matter how stupid you act you can't blow up your house

http://www.batteryspace.com/LiFePO4/LiFeMnPO4-Batteries.aspx
```

---
## \#3 Posted by: evoheyax Posted at: 2017-06-23T19:46:33.375Z Reads: 1112

```
If you look carefully, I mentioned lifepo4 batteries. I just don't seem them as practical for a new user, given the voltage differences, they are more difficult to source, and harder to find information about. This is for new users :P
```

---
## \#4 Posted by: Hummie Posted at: 2017-06-23T20:29:55.962Z Reads: 1071

```
Iron you can get in all types of shapes and have roughly 4x the cycle life of li-ion and are much safer and really not hard to find.  I just convinced a new-to-this friend to get them as Iron being so safe they seem better suited for new people.  They also sometimes have cool screw connectors such as headways cells where you don't need to solder. 
I should probably have gotten long ago and saved myself a bunch in ruined lipos.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-06-23T20:45:40.209Z Reads: 1000

```
As far as I've seen, almost every lifepo4  on the market is sold from sketchy looking websites as off brand cells. Samsung, Panasonic, and LG are not making them. They are not a staple in the RC community either, so very select name brand RC companies are using them.

Once you get people using a different voltage system (not 2.8-4.2). I can see a lot of confusion. Getting help will be more difficult, and finding info will be more difficult.

These 2 reasons alone are enough for me to not encourage new users to use lifepo4.

Not to mention different BMS's, chargers, ect. The general rule of thumb when your teaching someone is you use tried and tested materials and techniques. Since not a lot of people are using them at this point, I wouldn't call them tried and tested, and the voltage difference adds another layer of complexity to it. Understanding the 2.8-4.2 voltage system along with this new voltage system, on top of everything else they need to learn, seems like a burden, that's more likely to lead to problems than success.
```

---
## \#6 Posted by: oldguy Posted at: 2017-06-23T20:54:06.199Z Reads: 901

```
As somebody totally new to Lipos I have a few very simple questions that may be useful to other beginners if you decide to incorporate them into your guide (which is really well written and informative by the way, thanks)  - What is best practice for brand-new, right out of the box lipo batteries? I thought I had read there is a typical "storage" capacity (3.7v???) so should you charge them first thing? I was planning on hooking up just 1 of my new 3s lipos immediately after my build just to test (like, does the motor move at all? Yes? Does it roll with me standing on it? Yes? - OK, I'll plug them in and go for first ride after they charge...)
 What are the nominal voltages? ie. a typical lipo can carry a max charge of x.x per cell, and should not be discharged lower than x.x per cell. 
  is it better/worse/no diff to balance charge 2x3s together or individually? Does it actually take twice as long to charge 2 3s batts one at a time as opposed to together?

Those are mostly the things I don't know and was going to ask over the weekend (the last of my parts just arrived, it is first-build weekend for me!)

Thanks again!
```

---
## \#7 Posted by: evoheyax Posted at: 2017-06-23T21:11:20.775Z Reads: 864

```
[quote="oldguy, post:6, topic:26010"]
What is best practice for brand-new, right out of the box lipo batteries?
[/quote]

Lipos storage voltage is 3.7 volts. The best practice is leave them their untl your boards ready. Then to charge them when your ready to 4.2 volts, and discharge them all together as one pack most of the way down. This primes the cells in a sense.

Then either charge them to 2.7 again, or back up to 4.2 if you want to ride.

Do not every discharge the cells without the other ones. As cells deteriorate, they their capacity goes down. You want all cells to be at the same voltage during the entire discharge. Using one pack more than the rest will result in the cells that have been discharged more being in a different place during discharge in the future. This will lead to cells coming unbalanced more, and possibly, killing a pack all together because you'll pull it too low while the other packs stay at a same voltage. Remember, the VESC can only save a battery a whole from going too low, not individual cells or packs. I've have wasted hundreds of dollars on cells by doing this multiple times before.

[quote="oldguy, post:6, topic:26010"]
What are the nominal voltages?
[/quote]

3.0 to 4.2, 3.7 is known as the nominal or storage voltage of a lipo. Remember than li-ions are different. li-ions range from 2.5 (I do 2.8 to leave some buffer room) to 4.2. (I know your dealing with lipos, but just a note for future users :P).

I would do 3.2 - 4.2 per cell cause lower than 3 and you shouldn't bother trying to charge it anymore for safety reasons (resistance goes up, which while charging, causes pressure to build up inside the cells, they puff, and eventually, explode. If you want to know how big of explosion, you'd be surprised. Just youtube "zippy explosion" and you'll see, lol).

If you really want them to last, do 3.2 - 4. Doing so means you cut off the top and bottom 15%, which should in theory, almost double the life of your battery pack. Theres also very little usable power in the top or bottom 15%, so your losing a few blocks of riding for a typical 8 Ah pack.

[quote="oldguy, post:6, topic:26010"]
is it better/worse/no diff to balance charge 2x3s together or individually?
[/quote]

No difference in terms of the cells health or life cycle. If you have a 6s charger for example, but charge them as 3s's, then your going to have to wait for one to charge, then charge the other. It's quicker to charge them together at a higher amp rating. But if you charge a 2x 3s at say 2 amps, one after the other, or a 6s at 2 amps, you'll wait the same amount of time. Amps are basically the unit that we use to describe power going in and out of the battery. Unless you charge the 6s at a higher amp rating, do them by them selfs will be no quicker.

What will speed things up though, is using a higher charging rate (Be careful not to set it too high. They say 2a or less is the best for the cells life cycle, even if it's rated way higher) or if you have a charger that can charge four batteries at once, charge them all separately at 2a each and it'll take have the time (since again, you've effectively double the rate on amps going into the battery).
```

---
## \#8 Posted by: Hummie Posted at: 2017-06-23T21:14:26.710Z Reads: 714

```
lifepo4 cell are far from new and untested.  They are sold by many vendors more reliable than hobbyking.

  you can easily adjust almost every charger's voltage.   Even li-ion and lipos have different voltage ranges and it's not that complicated.  

 I recommended them to beginners so they wouldn't need the complications of a bms as they're surely safe enough to monitor on your own.   I think that's a huge simplification.   

the only downsides are they're more expensive and less energy per cycle but as far as simplicity, reliability, and safety, which are key ingredients for beginners, I recommend them first.
```

---
## \#9 Posted by: Hummie Posted at: 2017-06-23T21:19:38.830Z Reads: 706

```
3.5 lowest discharge and up to 3.15 for lipo is the more common range for preserving the cell. there's almost nothing beyond 3.5.
discharging past 80% can result in extreme differences in voltage of different cells and that's where unbalanced cells really show up and cut off the bms or plummet into death
```

---
## \#10 Posted by: Minim Posted at: 2017-06-23T22:02:28.438Z Reads: 700

```
Does anyone have a data logged amp curve on a high voltage setup? I'm curious on how much amp is needed for the various tasks so I know how much amp i need to build the battery for. And how much can the vesc 4.12 or 6 handle of this amp. I see you Are takling about lipo with 200 amps plus but then I read about burning vescs above 50amp so where is the sweet spot? 

My goal is a dual 6374 setup for hill climb and cruise. 90kg rider (95ish all up).
```

---
## \#11 Posted by: evoheyax Posted at: 2017-06-23T22:20:05.564Z Reads: 694

```
Think of it like amps are the force that make you move. What will make you pull more amps?

- Weight
- Hills
- High speed (wind resistance is a quadratic formula)
- Punching the throttle
- Motor Efficiency

I think your question is the most basic question that everyone wants to know when they first start. The problem, theres no one size fits all answer, because our setups (board, environment, us as people) are all different.

I for example weight ~200 lb. I will pull 80 continuous at times on certain hills, peaks over 100 amps.

Most of the time, I pull more like 50 amps continuous. Bear in mind, the motors I'm using likely could improve in efficiency, I'm a bigger guy, and I live In hilly San Francisco. So my environment is extreme to say the least.

Remember, that a VESC 4.12 can do 50 amp max, 27 amp continuous. I think for 95% of riders, a dual VESC 4.12 is enough. Between the 2 VESCs, 100 amps max and 54 amps continuous. However, theres no one size fits all here, so it's something everyone will have to experiment with. In this tough environment, a dual VESC only let me down with the carvon v2's, because the KV is really high. It's great for high speeds, but terrible for low speeds. At low speeds, the dual hub motors would make the VESCs over heat after a little over 2 miles of tough, aggressive riding through the hills.

If your doing a belt drive, which is seems you are, then I think a dual VESC 4.12 will be enough for you. If you have over heating issues, you can change the gearing around to solve that pretty easily. Might mean you don't get the top speed you want, but if you o the math before hand and pick your motors kv right, you can have both top speed, torque, and fun without any issues.
```

---
## \#12 Posted by: Minim Posted at: 2017-06-23T22:32:13.974Z Reads: 628

```
Thanks. This new info kinda tells me that my planned 12S4P LG HG2 is going to lack amps since i will be at the very limit all the time. Need 5-6 and above like in OP :) 

It would still be nice to see a amp curve if anyone got it with some info on setup/rider as to what I can expect. 

It might be a language thing (English is not my first language) but 50A continuous/average at 12S sounds like an extreme. That's 2.5kW ish and I think I read somewhere that in Tour de France (bicycle) the top riders where putting out like 4-500W while climbing as at a very peak like 1500W. Is these really that inefficient?
```

---
## \#13 Posted by: Hummie Posted at: 2017-06-23T22:35:50.597Z Reads: 603

```
I eat tour riders or any spandex wearing cyclist like snacks
```

---
## \#14 Posted by: evoheyax Posted at: 2017-06-23T22:59:11.204Z Reads: 612

```
Yea, same here. Hummie and I ride very similarly. For some reason, most of the I ride with him, he rides kinda slow for me. But I'm always pushing full throttle when I can when I'm by my self.

My board with hummies motors run 4wd @ 1000 watts each, so 4000 watts max. I fly by spandex cyclists like they are standing still, lol.
```

---
## \#15 Posted by: Ackmaniac Posted at: 2017-06-23T23:07:19.111Z Reads: 618

```
A 10S4P or 12S4P will have more than enough power for 95% of the riders here.

When you have a 4P pack with 20A cells then you can use the 80A (4x20A) that this pack is capable of without any issues. You won't harm the batteries because the only moments you are able to draw that much power won't take longer than 5 seconds (mostly not even 2 seconds). And all the life time ratings are tests which were done under absolute worst conditions at 20 amps a cell continuously (limit of the cell). And even then the battery's would have been good for 10000km.
When we ride we use on average less than **10 amps** on the entire pack. That is **2.5A** a cell for a 4P, not **20A** a cell.

**So what is the noticeable difference between Li-Po and Li-Ion?**
Only at high speeds there will be a difference in the power output. This is because the Li-Po cells will have a higher voltage under load. And also when they are drained till a certain percentage. But the difference is only like 15%. That means that you will have more power close to max speed. 
So if your board can do 50 km/h (limited by the kv of your motor) you will only feel a difference of the power output above 42,5 km/h. And you might reach a 2 or 3 km/h higher speed. And that is also only noticeable when you go full throttle.
And your settings of the VESC needs to be high. Otherwise the settings would limit the power anyway. So if you have a dual drive, 10S4P and don't use more than 30A battery max on each VESC then you won't really feel a difference
And don't forget that Li-Po batterys are 50% heavier than Li-Ion when they have the same Wh capacity. 

**When does Li-Po make sense.**
When you are on a low budget.
When you want a really light board and don't need range. For example for race mountainbaord that only needs to run 5km in a race. Li-Pos are heavier but the pack can be sized smaller.

PS: My watt control isn't meant to reduce any effects of voltage sag.
```

---
## \#16 Posted by: oldguy Posted at: 2017-06-23T23:19:36.152Z Reads: 555

```
Thanks so much for a clear and thorough response!
```

---
## \#17 Posted by: evoheyax Posted at: 2017-06-23T23:21:22.470Z Reads: 572

```
[quote="Ackmaniac, post:15, topic:26010"]
PS: My watt control isn't meant to reduce any effects of voltage sag.
[/quote]

Well it makes sense that it would though. In current control mode, voltages drops on the battery and thus, watts drop, thus it feels sluggish. With lipos, it doesn't drop the same and thus, voltage stays higher, watts stay up and every things good.
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-06-23T23:28:55.899Z Reads: 594

```
Current control regulates the current at the motor side, not at the battery side.
As long as the duty cycle isn't too high (more than 80%) the battery is capable to deliver enough amps so that the VESC can transform it to the wanted motor amps. Only above 80% duty cycle the Li-Po cells perform a bit (20%) better and provide a little bit (2 or 3 km/h) higher top speed. But if you plan to get a 10S Li-Po Battery and don't go with Li-Ion because of the little performance difference then you should simply upgrade it to a 12S Li-Ion Battery. 
This will outperform any comparable 10S Li-Po battery. (I am talking about 4P packs because this is the most used size and provides enough power)
And the upgrade from 10S to 12S is only a increase of 20% more weight. The 10S Li-Po weights 50% more than a 10S Li-Ion Battery when they have the same range.

And don't forget that Li-Po battery's are dangerous if you don't know how to handle them. That is actually the reason i write this, because most of new users don't know shit about battery's. (This thread is for those people)

P.S. @evoheyax the graphs in your first thread are very irritating. Because you show the graph of a 2S Li-Po compared to a 1S Li-Ion. Actually you show graphs of a LiFe and LiFePo, so i don't really know what these are good for.
```

---
## \#19 Posted by: evoheyax Posted at: 2017-06-23T23:48:49.728Z Reads: 577

```
I included that gif above with your view of lipos in mind :stuck_out_tongue:

If you can find a more accurate graph of a lipo discharge, than please post it and I'll gladly update it. I don't mean to be miss leading, which is why I'm trying to have a constructive conversation.
```

---
## \#20 Posted by: Hummie Posted at: 2017-06-24T02:52:20.294Z Reads: 577

```
@Ackmaniac when u say 80% of duty cycle why that number..just because the lack of duty cycle's ability to make useful current and going direct from battery current which occurs at the higher duty/speed requires more from the cell?  At high speed there's a greater draw on the battery w a given wattage output?  Seems so
But w 4p ur good w Li-ion and good cells I believe nut it's just a question oh longevity from beginner perspective. Nicest maybe Li-iron at maybe 14p with it's great flat discharge curve.  As well as so mush more.  I'm obviously trying to push Li-iron.
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2017-06-24T07:17:07.635Z Reads: 519

```
@evoheyax thanks for the write up .... yet again
```

---
## \#22 Posted by: Okami Posted at: 2017-07-17T12:47:26.002Z Reads: 496

```
Good thread, kudos to @evoheyax and @Ackmaniac too bad stuff like this sometimes get lost :) (found it only recently, by a link in another thread ;) )
```

---
## \#23 Posted by: tung Posted at: 2017-12-04T22:27:01.928Z Reads: 457

```
my etwow scooter manufacturer said the battery is "33v, 6.5 ah, generates up to 500 watts."

my battery is dead now after 320 miles of riding. instead of paying the asking price of $280 for a replacement, i like to buy my own battery packs from HobbyKing.  what do i need? 
from basic math you showed above, i know to get 33v, i would need 8s.   and to get 6.5ah, i would need 3p.
but 4.2 x 8 x 3 x 2.5  = 252 W,  nowhere near the 500 watt that etwow quoted.

what bat packs and configuration should i use to power up my scooter once more? 
pls advise. thanks!
```

---
## \#24 Posted by: evoheyax Posted at: 2017-12-04T22:52:36.570Z Reads: 457

```
Seems like your confusing watts and watt hours.

Watts are a a way of measuring how much power there is going through a given system at a given time. It changes depending on the load, what part of acceleration/deceleration/coasting you are in, and many other factors.

Watt hours tells you more or less about range (instead of power output).

4.2 x 8 = 33.6 max voltage.

Since your doing 3 x 2.5 ah batteries, you have 7.5 ah total. 33.6 v x 7.5 ah (amp hours, not amps) means you have 252 Wh. The original battery had 33.6 v x 6.5 ah = 218.4 Wh.

Now, the C rating tells you about max power output. Not sure what battery your planning on using in specific, but say it's a 20c battery, then you can do 20 c x 7.5 ah = 150 amps max. Now, you want that number into watts, right? So do 33.6 v x 150 amps = 5040 watts max.

20c is pretty normal, 10c is also pretty common. Even at 5c, you will have 1260 W max.

You really don't need to worry about it. Aim for a 10c or higher to really make sure (they usually exaggerate their ratings), but your not limited with lipos. 18650's on the other hand though...
```

---
## \#25 Posted by: tung Posted at: 2017-12-05T14:02:58.995Z Reads: 431

```
ok. i think i got it now.
suppose i get two of this 6s1p 40C battery. https://hobbyking.com/en_us/zippy-flightmax-2650mah-6s1p-40c.html
i put them in series, so i will have a 12s1p configuration. capacity will then be 12 x 4.2 x 2.5 = 126 Wh,  about 1/2 of the 218.4 Wh of the original battery. therefore my travel range will then be half, correct?

as for watt, i will have 40c x 2.5 ah x 50.4 v = 5040 Watt.

should i worry about frying the ESC because the original battery is 33v, while my 12s1p will have 50.4v?
maybe i should use 10s1p battery pack?

thanks a lot,  this is very enlightening!
```

---
## \#26 Posted by: OleksiiF Posted at: 2017-12-24T18:38:22.543Z Reads: 416

```
i am using 12s1p lipo battery for 1.5 year at this point
and im pretty afraid of them (used lipos - fire, you know...)

and i am planning to change it to li-ion 12s2p, but i didnt knew anything about sag...
now its clear for me that 12s2p is not enough since i like to push it hard. what should i do? go with 12s3p? will this be enough? i mean compared to 12s1p lipo.
```

---
## \#27 Posted by: ZackoryCramer Posted at: 2018-01-31T20:47:20.970Z Reads: 393

```
Hey I have a question. Shouldn’t the way to calculate wh be ah times the average voltage of the pack while discharging? Why do some people use nominal voltage and you use max voltage? .5 volts is a lot of difference. Thanks 🙏
```

---
## \#28 Posted by: FredrikHems Posted at: 2018-01-31T21:37:57.538Z Reads: 389

```
You should use nominal, so 3.6 for Li-ion, and 3.7 for LiPos
```

---
## \#29 Posted by: PXSS Posted at: 2018-01-31T23:46:26.214Z Reads: 412

```
[quote="ZackoryCramer, post:27, topic:26010"]
Shouldn’t the way to calculate wh be ah times the average voltage of the pack while discharging?
[/quote]
This is correct. 

[quote="ZackoryCramer, post:27, topic:26010"]
Why do some people use nominal voltage
[/quote]

Your nominal voltage is the average voltage at a current rate specified by the manufacturer, usually 0.5C (the current it takes to discharge a battery in 2 hours) sometimes even lower, it's always specified on the datasheets. 

It is ok to use this value when the battery isn't run way higher than the nominal discharge rate. Once you start discharging at 5A+ per cell continuous, you should really take into account the extra voltage sag at 50% discharge but very few people do. 

[quote="ZackoryCramer, post:27, topic:26010"]
you use max voltage?
[/quote]
Dead wrong and usually done by people with little understanding on how batteries work.
```

---
## \#30 Posted by: ZackoryCramer Posted at: 2018-01-31T23:55:56.484Z Reads: 381

```
Thanks. The voltage sag explained it to me.
But @evoheyax confused me

[quote="evoheyax, post:1, topic:26010"]
Formulas you need to know:

mAh = 1000*Ah
Wh = Ah * max voltage
W = Amps now * voltage now
[/quote]

and

[quote="evoheyax, post:1, topic:26010"]
Back to our example, a typical li-ion battery in:

12s1p will have 2.5 Ah total at 50.4 volts. 2.5 x 50.4 = 126 Wh
[/quote]

Made me rethink my calculations for a second :rofl:
```

---
## \#31 Posted by: evoheyax Posted at: 2018-02-01T00:16:13.963Z Reads: 353

```
[quote="PXSS, post:29, topic:26010"]
Dead wrong and usually done by people with little understanding on how batteries work.
[/quote]

Back to trollin, eh?!?! You know that just because your an unhappy and miserable person, that you don't have to share that with the world, right?

First off, this is literally how 90% of people in the community calculate it, including board manufacturers.

Everything is really an estimate also. The Wh I have on my ride today will be different then tomorrow, based on my riding style and terrain (and for boards ridden by multiple riders, rider weight). This is because higher amp draw results in lower capacity (just look at an 18650 graph). So none of this is really very scientific.

I have actually found that measuring my amp draw per motor and adding it up that based on a max voltage Wh calculation, I get in the real world within 5% of that... It's close enough...
```

---
## \#32 Posted by: ZackoryCramer Posted at: 2018-02-01T00:45:38.045Z Reads: 338

```
I don't know how to exactly calculate wh, but by charging my lipos with a power supply, I got a wh count similar that of calculated using 3.9v
```

---
## \#33 Posted by: PXSS Posted at: 2018-02-01T00:45:59.895Z Reads: 364

```
Again, this would be wrong. Not having much understanding is the culprit. 

Lets take a look at some examples from actual test data. 

NCR18650GA datasheet:
Rated capacity: 3300 mAh
Nominal Voltage: 3.6V

Third party test data (not my own):
![image|690x195](upload://pvTD3zdAJGQprA94U6Mc2qaLkqV.jpeg)

Energy based on Nominal Voltage and Rated Capacity: 11.88Wh

Energy based on Maximum Voltage and Rated Capacity: 13.86Wh

Looking at the test data you can see that the measured output energy is almost matched with the energy calculated at nominal voltage between the 0.5A and 1A test condition. This is because Panasonic rates their GA cell at 0.67A. 

Datasheet:
![image|690x146](upload://qred5USjBgLa4OpWmFoLlTBl2tY.jpeg)

I can do this for every single cell you specify. Again, the test data isn't mine. There is no way for me to have manipulated these numbers. This is simple math. These cells are rated to 11.88Wh as the test data above confirms and not 13.86Wh as @evoheyax claims.
```

---
## \#34 Posted by: PXSS Posted at: 2018-02-01T00:46:50.416Z Reads: 329

```
I dont need petty insults to prove you wrong. Just look at the data.
```

---
## \#35 Posted by: ZackoryCramer Posted at: 2018-02-01T00:56:15.698Z Reads: 341

```
I have to agree with @PXSS for this argument. Maybe you're right, but from all the sources I've read, wh is calculated with nominal voltage 3.6. And a battery barely stays above 4v for 20% of its capacity, how can you use 4.2v to calculate energy?

[quote="evoheyax, post:31, topic:26010"]
Back to trollin, eh?!?!
[/quote]

:eyes: who's talking
```

---
## \#36 Posted by: PXSS Posted at: 2018-02-01T00:56:44.774Z Reads: 353

```
Lets look at Samsung 30Q datasheet:
https://eu.nkon.nl/sk/k/30q.pdf

This one is even easier, they give us rated capacity and energy on a single table!

![image|690x353](upload://cTeZuzDLtZmEZhyZaNauIj1RKOg.jpeg)

Nominal voltage: 3.6
Rated capacity: 3.0Ah
Energy calculated based on nominal voltage and capacity: 10.88Wh
Energy calculated based on max voltage: 12.6W
Energy calculated based on average voltage and capacity discharged @ 0.2C: 10.97Wh

@evoheyax, I'm happy to teach you how to google spec sheets any day.
```

---
## \#37 Posted by: evoheyax Posted at: 2018-02-01T01:18:04.963Z Reads: 328

```
[quote="ZackoryCramer, post:35, topic:26010"]
who’s talking
[/quote]

So I'm trolling now? PXSS literally comes into every thread and tries to start fights. He literally does this day in and day out. If a bully throws a punch at me, I'm not going to stand there and smile.

@PXSS Your assuming we pull the same amps at all times while we ride. Both you and I know that's not correct. Wh ratings are estimates, unless it's at a particular amp draw. Maybe my method is a bit higher than reality, and your method is likely to give a better numbers. But it still is not scientifically accurate. If you just ride and watch your phone with an app, you'll see how your amps bounce around. So it's impossible to give an accurate Wh rating for a particular battery.
```

---
## \#38 Posted by: ZackoryCramer Posted at: 2018-02-01T01:24:39.025Z Reads: 312

```
I had an app that tracked the amps and amp-hours count. Obviously, the current fluctuates, but the watt-hour has to converge to a value which is the average watt-hour in the pack. If you can agree that my way is better then so what if they aren't scientifically accurate or what's so important about the scientific way that people still calculate it even if it's wrong? Sorry if you feel insulted, I didn't mean to start a quarrel.
```

---
## \#39 Posted by: evoheyax Posted at: 2018-02-01T01:29:31.062Z Reads: 312

```
The problem is when someone comes in and says people with no understanding of how batteries work calculate it this way. That is insulting to say the least...

I agree that this is a better way. The reason I put the max voltage was because this was how companies like enertion and boosted and evolve calculate it... I guess they all have little understanding of how batteries work...
```

---
## \#40 Posted by: PXSS Posted at: 2018-02-01T01:53:40.070Z Reads: 336

```
[quote="evoheyax, post:37, topic:26010"]
Your assuming we pull the same amps at all times while we ride.
[/quote]
No I'm not. The examples above were constant current so that is what I used. 

[quote="evoheyax, post:37, topic:26010"]
Both you and I know that’s not correct.
[/quote]
Correct

[quote="evoheyax, post:37, topic:26010"]
Wh ratings are estimates,
[/quote]
The rating is a guaranteed amount of energy that you will get at an average current. 

[quote="evoheyax, post:37, topic:26010"]
But it still is not scientifically accurate
[/quote]
It is. Energy is a measurement and ***can be measured***.
You can measure voltage while you ride, correct?
You can measure current while you ride, correct?
So at any point in time you can calculate power, correct?
Energy is measured by integrating power over time. If you have instantaneous power being transmitted at 5hz then you can calculate the energy used every 0.2 seconds, integrate that over time and you can calculate the energy used throughout your ride very accurately. This is the method used in industry. It is only dependent on the accuracy of your voltage reading, current reading and the rate at which you sample. 

If you average your current draw and voltage through that same ride and multiply them together then you get your average power draw throughout the ride, if you multiply this by the duration of your ride then you will have the exact same energy measured as before. The only extra source of error would be any rounding error you introduce when you average your values. 

[quote="evoheyax, post:31, topic:26010"]
I have actually found that measuring my amp draw per motor and adding it up that based on a max voltage Wh calculation, I get in the real world within 5% of that… It’s close enough…
[/quote]
If you calculate your energy based on the average current and maximum voltage, you will have an answer that's at best 16% higher than actual, at worse, 30+% higher. 

[quote="evoheyax, post:37, topic:26010"]
So it’s impossible to give an accurate Wh rating for a particular battery.
[/quote]
My job requies me to write models that predict how much energy a particular battery uses during different missions for UAVs. Trust me, it is very much possible to give an accurate energy measurement and even predict it before your ride.
```

---
## \#41 Posted by: PXSS Posted at: 2018-02-01T01:55:54.486Z Reads: 296

```
[quote="evoheyax, post:39, topic:26010"]
how companies like enertion and boosted and evolve calculate it… I guess they all have little understanding of how batteries work…
[/quote]
They are selling you a product and will do practically anything (including lying) to convince you that they have the best and most innovative shit on the market. 

I'm not here to sell you anything. I'm just here to give you cold facts and truth based on physics and math as I've said plenty of times
```

---
## \#42 Posted by: Sampreston Posted at: 2018-04-03T01:41:50.345Z Reads: 271

```
Woah! Thanks for all the details mate! I appreciate you.
```

---
## \#43 Posted by: kocoz Posted at: 2018-06-04T14:57:14.960Z Reads: 254

```
Hey, thx so much for your topic. 
What are the difference between 8s li-po and 10s li-ion in performance? Is it critical for single motor build?
```

---
## \#44 Posted by: evoheyax Posted at: 2018-06-04T18:31:48.080Z Reads: 265

```
It all depends on the gearing. A good rule of thumb is to make sure your top speed is reasonable and not something too crazy.

for the same gearing, an 8s will feel weaker, because you simply have less watts going into the motors. Since watts = amps * voltage, increase either of these guys and you will feel more power. Set your amp limit higher (assuming your esc and motor can do the higher amps safely) or increase voltage and you'll feel the difference. I would say expect up to 20% less performance if you gear it the same. But you can get torque for 8s still. I personally like 12s, and might experiment with a higher voltage at some point.
```

---
## \#45 Posted by: Hummie Posted at: 2018-06-04T18:40:56.282Z Reads: 267

```
watts is amps x voltage but is the motor getting that voltage of the 12s when it's not up to a higher speed?
 I think the 12s would have the potential for greater power at full speed but at lower speeds the motor will only see the voltage supplied from the esc which at lower speeds just determines the current going to the motor.   ive never tried a lower voltage to see though
```

---
## \#46 Posted by: evoheyax Posted at: 2018-06-04T18:42:31.080Z Reads: 261

```
I've ridden 8s boards before that did better than 12s boards, lol. If your talking direct drive or hub motor, then yes, lower voltage will give lower performance if you don't change the motor kv.
```

---
## \#47 Posted by: Hummie Posted at: 2018-06-04T18:50:07.792Z Reads: 265

```
what is performance?  torque or speed or even efficiency it could be. 

  torque is decided by the amp settings of the esc, the kv and any gearing.  speed will be reduced with lower voltage, but at the same time you can run a low voltage and a high kv and get to the same speed and also the same torque if the esc amp setting are able to be increased.

you could run at a very low voltage and have a very high kv motor and run an esc that can do many more amps and get the same performance (torque, speed, efficiency) I believe
but @kocoz s question of lipo vs ion...you COULD get the same performance maybe on watt control or something but lipo will hold at a higher voltage for longer before dropping while ion has a more continuously dropping voltage and ends lower.

but at the same time when my battery is dropping I do notice less torque which goes against what I just wrote
```

---
## \#48 Posted by: kocoz Posted at: 2018-06-05T05:44:48.839Z Reads: 234

```
@Hummie @evoheyax thx for your answers. I also would like to find out about amount of C in li-po s - I think it does not matter if it would be 15c or 40c for our builds, am I right?
```

---
## \#49 Posted by: Hummie Posted at: 2018-06-05T05:52:03.800Z Reads: 255

```
it does a lot.   and  they exaggerate with lipo.  id do at least 30c if youre doing a 12s pack.  they pretty much double the stated discharge rate compared to what it really should be doing as seen in the eyes of people who test lipo.   Lipo are rarely tested to see how they do at their supposed discharge ability while ion are tested pretty thoroughly 
so if you had a 12s pack and it was 20c and 5ah that would be 100 amps continuously that the battery would be able to supposedly do and if you did over that it would be sagging and heating up.    If youre doing more voltage such as 12...vs doing maybe 8 lets say...then the battery will be able to use less amps OUT OF THE BATTERY for the same wattage so you can get away with having a lower c rate.   I wouldn't even mess with a 20c 5ah 12s battery and do 30c with 5ah.   if you go up to 10ah pack then you would have 200amps supposedly that the pack could put out continuously without it decreasing the cycle life much and then I think youd be good with just 20c
```

---
## \#50 Posted by: kocoz Posted at: 2018-06-05T06:22:22.223Z Reads: 265

```
Oh, I understood. As for me, I am thinking about all other components, and depend on how much money I am going to spend, I am choosing between li-po 2x4s 5ah (that way I need 30c+?) and 10s3p 25r. The difference is about 120$
```

---
## \#51 Posted by: AreaKruzer Posted at: 2018-06-06T04:23:49.993Z Reads: 281

```
I am looking to make my own 10s4p packs using the 18650 30Q with the U-solder tags ( some people call it C-solder tags)
![](https://www.nkon.nl/sk/k/old/18650-u-tags.jpg)

Is it ok for me to solder the tags onto the 18650 PCB that martinSP sells?
http://electricskateboard.repair/img/p/1/0/9/109-large_default.jpg
```

---
## \#52 Posted by: willpark16 Posted at: 2018-06-06T14:35:35.437Z Reads: 266

```
How long doesn’t nkon.eu take to arrive In Southern California
```

---
## \#53 Posted by: dougpage Posted at: 2018-09-24T15:36:38.910Z Reads: 235

```
Hi, Im doing a vanguard build and Im new to the diy scene and I need a 12s 18650 battery that will fit in the eboosted 12s vanguard enclosure. I would like a 12s3p battery and a good bms that does not limit the performance. Any suggestions? Thanks for reading.
```

---
## \#54 Posted by: Femo89 Posted at: 2018-10-12T09:10:56.014Z Reads: 233

```
Any of you guys has had experience with these batteries? http://www.diyeboard.com/10s3p-18650-lithium-battery-pack-10s-36v-6ah-with-charger-p-631.html
```

---
## \#55 Posted by: Wisp Posted at: 2018-12-12T16:02:21.149Z Reads: 216

```
Is there someone that has experience with the Sanyo UR18650NSX? Couldn’t find anything on this forum.

I got the following setup: single drive 6374, 10S3P

I was set to use the Samsung 30Q but I see that I can save quite some money by using the Sanyo’s.

The small loss in range is unimportant to me but I see that they perform better at 20A (and slightly less good at lower A)
```

---
## \#56 Posted by: thisguyhere Posted at: 2018-12-12T16:09:03.271Z Reads: 208

```
just use the 30q, they're pretty much proven at this point

http://esk8life.com/samsung-30q-18650-cell
```

---
## \#57 Posted by: maccmen Posted at: 2018-12-12T17:59:53.884Z Reads: 210

```
What about making a 10s4p with 12000mah instead of 3000mah, both 3.7v for a battery replaceement for a bamboo gtx?
```

---
## \#58 Posted by: stijn_da_sheep Posted at: 2018-12-25T23:00:30.244Z Reads: 201

```
Hi man, have you finished your build? Would love to hear how it turned out, I'm currently also doing a Vanguard build and still dont know where i should get my li-ion battery pack. 12s3p seems like enough, what kind of range and speeds are you getting?
```

---
## \#59 Posted by: Andreu Posted at: 2018-12-26T18:06:01.171Z Reads: 201

```
 I would like to build my first DIY electric mountain board.

I have the board and I have read hundreds of post to select the best and cheapest dyi.

I think i am going to a single motor, buy a 12s2p lipo batterie 8000mah (€ 100) one  SK3 - 6374-192KV (€ 85) and vesc from enertion (€ 90)

I want to know the best way to charge batteries, i am planning to buy 4x 6S4000mah and do 12s with 8000mah
Would you recommend me to charger for that batteries and how can i charge?
I think the best option is to balance the charger for 6s and disconnect the batteries in series and let the parallel so I can charge two and two.
 Is that safe for the batteries or is better charge one by one.
Thank you I have already learned alot of your post.
```

---
## \#60 Posted by: dougpage Posted at: 2018-12-26T21:23:16.262Z Reads: 197

```
Hey, no I haven't, Im on vacation with my family. When I get back on the 30th it will be the first thing I do. I will update my build page when I do tests and post pics throughout the process. Thanks for your interest!
```

---
## \#61 Posted by: Superflim Posted at: 2018-12-26T23:39:21.884Z Reads: 192

```
Get a bms!!
Saves so much hassle
```

---
## \#62 Posted by: stijn_da_sheep Posted at: 2018-12-27T17:52:49.870Z Reads: 190

```
good luck man! would love to see a parts list of your build! I've just ordered the first parts of my build :grinning:
```

---
## \#63 Posted by: dougpage Posted at: 2018-12-28T00:33:35.305Z Reads: 201

```
https://www.electric-skateboard.builders/t/the-non-boosted-stealth-board-first-build-hummie-hubs-and-deck-focbox-unity-12s3p-psyco-enclosure-nano-x/77959

I have the parts list here.
```

---
## \#64 Posted by: hyperIon1 Posted at: 2018-12-28T00:40:51.929Z Reads: 208

```
We are currently planning a battery build using the Samsung 50E 21700 cells. 
This is the price difference and cell difference calculations we came up with and it’s pretty significant. 
Note: prices are for cells only
![image|383x500](upload://4HJX5lZOsVMpF6EGQfuoxPgMrv6.jpeg) ![image|388x499](upload://zQ2f6dnUSg3OQ2LgaoD9YBXmE0q.jpeg)
```

---
## \#65 Posted by: Skunk Posted at: 2018-12-28T00:43:06.852Z Reads: 194

```
Oh what.  Dude... 2019 is gonna be rad.
```

---
## \#66 Posted by: Phillisuper Posted at: 2019-01-04T16:39:29.311Z Reads: 191

```
So just to make sure I have my understanding right, a 12S4P has four times the capacity and 12 times the power? Thus if I wanted to build a board with twice said range I would build a battery that was 12S8P? Also (this is off topic somewhat) If I wanted to get the most power possible, could I double the voltage of the battery and use 2 VESCs (ie if I wanted to build a AWD board but wanted each wheel to have as much power as if I'd built it as a 2WD board).  In that Scenario could I build a 24S8P, giving me twice the range and power output of the normal 12S4P and simply splitting the power between 2 VESCs? (sorry for the long question, I'm very new and want to learn all I can)
```

---
## \#67 Posted by: csjazzman Posted at: 2019-03-07T07:38:49.263Z Reads: 167

```
Hey would love some help. I purchased this battery (see link below) and charger with the hope of using it in my own home build only to realise that the charger is only compatible with the balance scooter board the battery is made for. Any advice on how I could incorporate the charger into the home build? I have the resources to solder ect but just don't know what I'm missing. 

https://www.ebay.com.au/itm/183103470870
```

---
## \#68 Posted by: rs1990 Posted at: 2019-03-14T03:15:59.089Z Reads: 155

```
Hey I was just wondering If anybody would know what I should do, I want to have a 10s lipo perferably two 5s in series I but i just don't know what batteries to use and if i should get a high discharge rate, Thanks
```

---
## \#69 Posted by: Travo Posted at: 2019-04-05T01:33:49.541Z Reads: 142

```
Question, I had my cells welded together.  When the company I got to do it welded them they did not put any rings around the top of the cells so the nickel is touching the plastic wrapping.  Will this be a problem in the future or can I just leave it and not have to get them welded again?
```

---
## \#70 Posted by: Kal-El_basically Posted at: 2019-04-09T10:10:44.110Z Reads: 131

```
I was wondering. I have a very small penny board setup and cant afford to incorporate a Li-ion pack because it takes up too much space. I am currently using 2 Turnigy 5000mah 20C 3s lipos in series and I've already accidentally puffed up 2 of them from excessive discharging. I'm only upset because I get like one ride out of them before they're "discharged beyond return". Would upgrading my setup to 4 batteries, 2 series configurations in parallel (2s2p), give me additional Ah that would extend my ride time but provide me with the same voltage and current to have an enjoyable ride?
```

---
## \#71 Posted by: Andy87 Posted at: 2019-04-09T10:17:34.244Z Reads: 129

```
don´t mix old and new lipos.
```

---
## \#72 Posted by: Kal-El_basically Posted at: 2019-04-10T20:33:02.359Z Reads: 121

```
If I have 4 new lipos is this possible.
```

---
## \#73 Posted by: Andy87 Posted at: 2019-04-11T03:29:40.165Z Reads: 120

```
Yes that would work
```

---
## \#74 Posted by: Kal-El_basically Posted at: 2019-04-11T03:51:08.674Z Reads: 123

```
So I just bought a lipo that is not enlarged at all. I took it on one ride and the other old one puffed up but this one is fine. Do I really need to buy another 4 lipos or will 3 and this one work?
```

---
## \#75 Posted by: Andy87 Posted at: 2019-04-11T03:58:58.212Z Reads: 124

```
Depends. Is it the same brand of lipo you buy? The thing is, that if you wire up lipos in parallel there internal resistance should be similar. If one is older that might be different from the new ones. As lipos way more sensible to overcharge and over discharge i just wouldn’t take that risk and get 4 new ones from the same brand with same capacity
```

---
## \#76 Posted by: Kal-El_basically Posted at: 2019-04-11T20:23:25.973Z Reads: 120

```
Damn, ok I understand. Thank you so much, just this little bit of insight is more than I had before.
```

---
## \#78 Posted by: LukeCool Posted at: 2019-06-13T09:45:19.539Z Reads: 83

```
 More info on LiPo's, "What the numbers mean".
file:///D:/RC%20stuff/RC%20Powers%20threads/LiPo%20INFO/What%20the%20numbers%20mean%20with%20regards%20to%20LiPo%20cells.pdf
```

---
## \#79 Posted by: korijn Posted at: 2019-07-27T10:25:09.582Z Reads: 73

```
@evoheyax If you use dual motors do you need twice the amp en thus twice as large of a battery?
```

---
## \#80 Posted by: evoheyax Posted at: 2019-08-07T00:38:12.719Z Reads: 73

```
That's too simplistic of a way of looking at it. You motor can handle a certain amount of heat. If you've ever cooked, you know a pot doesn't lose all of it heat the second you take it off the stove. Metal retains heat, including the stator (made of steel), the motor parts and the copper winding.


The by product of more amps is more heat. So by adding a second motor, your doubling the amount of space that can hold this heat. Thus you can adjust the settings to double the amps and you should expect the motors won't run hotter than they did before pulling double the amps.

An example:

*setup 1:*
- motor 1 with max 40a limit
- battery with 80a limit

output of setup 1:
- 40a amps will go to motor 1
- battery will output 40a
- You will likely move but you will be pushing the single motor very hard, resulting in a lot more heat.

setup 2:
- motor 1 with max 40a limit
- motor 2 with max 40a limit
- battery with 80a limit

output of setup 2:
- 40 amps will go to motor 1
- 40 amps will go to motor 2
- battery will output 80a and split it between the motors
- Motors will run at max power output

setup 3:
- motor 1 with max 40a limit
- motor 2 with max 40a limit
- battery with 60a limit

output of setup 3:
- 30 amps will go to motor 1
- 30 amps will go to motor 2
- battery will output 60a and split it between the motors
- Motors will run at medium power output, staying a bit cooler, but running at a higher power output than 1 motor

setup 4:
- motor 1 with max 20a limit
- motor 2 with max 20a limit
- battery with 80a limit

output of setup 4:
- 20 amps will go to motor 1
- 20 amps will go to motor 2
- battery will output 40a and split it between the motors
- Motors will run at max power output

There's many ways to configure it.

In terms of draw. Everything comes down to our evil friend called resistance. And if we brushed up on our physics, we can recall that Amps = Voltage / Resistance. Amps create heat through resistance. The way a battery can have a higher amp rating, without changing the voltage or size of battery, is by lowering the internal resistance of the battery. Which is what higher c rated batteries are doing.

It's always wise to spend extra on batteries with far higher ratings than you need. Voltage sag with a vesc in current control mode (i.e. controlling the flow of amps), which is the traditional way of running a vesc, doesn't care about your voltage dropping. Since watts (watts = amps*voltage) describe your overall power, you'll feel power dropping out from under you on hard accelerations since your voltage will drop. For this reason, bigger batteries are always advised as well.
```

---
## \#81 Posted by: FireSerpent Posted at: 2019-08-15T03:29:03.784Z Reads: 66

```
Has anyone ever purchased cells from cheap-batteries.com?

Their price for the Samsung 30Qs seem too good to be true. Do you think they are legitimate cells? If so, it would be a good vendor option in the US. 

https://www.cheap-batteries.com/mm5/merchant.mvc?Session_ID=9185b74c3e7e85ba82feeb931b8bfcee&Screen=PROD&Product_Code=INR18650&Category_Code=18650
```

---
## \#82 Posted by: evoheyax Posted at: 2019-08-15T15:04:04.075Z Reads: 64

```
Just buy these: https://www.imrbatteries.com/samsung-30q-18650-3000mah-15a-battery/

At least you know they are legit. So what if you have to pay $1 more per cell. It's not worth the risk to save $50 bucks or less when you might end up burning your house down or in the best bad case, wasting your money.
```

---
## \#83 Posted by: FriedTM Posted at: 2019-09-18T17:38:11.038Z Reads: 56

```
Hello I am a new user so I am sorry if this is not the right place. I have a meepo v3 and I am looking to build a 10s3p battery with the Samsung 40T
https://www.imrbatteries.com/samsung-40t-21700-4000mah-35a-battery/
I am looking for a BMS and as I am pretty knew to this I want to make sure it will work with the existing ESC. I can figure the pin outs but I would like to keep the features the board already has. I have some experience with soldering batteries from rc helicopters but I feel out of my depth here. I am excited to learn but I need some help.
```

---
## \#84 Posted by: Regulator Posted at: 2019-10-16T19:41:25.558Z Reads: 43

```
This is.. EXACTLY the explanation I have been searching months for. Thank you dedicating your time to putting this together!
```

---
## \#85 Posted by: dildoritos Posted at: 2019-12-04T00:45:20.556Z Reads: 33

```
first off, thank you guys for being so comprehensive here.

I'm wanting to switch from lipo to lion for my next build but I've never used lion cells before..

Can I get someone's opinion on this?
https://www.ebay.com/itm/36V-14Ah-Lithium-li-ion-Battery-Pack-500W-ebike-Bicycle-E-Bike-Electric-charger/293213343242

its for a mountain board with two 6374's and a unity supposedly delivering 75a to each under peak acceleration but the ebay listing says its peak discharge is a worrying 30 amps. I'm ready to buy two of these for 10s10p which should be more than plenty right? 

p.s. I read this thread 100% so anything mentioned about sag is clear to me but feel free to elaborate, I also know is hella china brand but if there are major concerns lmk please
```

---
## \#86 Posted by: Okami Posted at: 2019-12-11T17:28:00.888Z Reads: 31

```
@dildoritos 500W X 2 is no good. U want at least 60-80Amps for mountainboard, if not all 100+ to really feel power, in my opinion.

Aim for 2+ KW power.
For li-ion thats a lot of cells in parallel.
```

---
## \#87 Posted by: Okami Posted at: 2019-12-11T17:29:07.101Z Reads: 32

```
60Amp pack at 30A sags a lot, so best to use 1/5th or 1/4th of max amps or so

5p for 14ah would give 2.8ah, i think 10A at best for such cell, so in theory best would be to use only 2A x 5 = 10A

360W x 2 isnt much, would say at least 4 such packs would be ok for power hungry board

Otherwise u get cruiser which carries u around with 800W of sustained power but is capped to do more.

Personal opinion from running 3 setups so i might not be best source but ask around
```

---
## \#88 Posted by: hans_maier Posted at: 2019-12-14T15:20:01.533Z Reads: 26

```
Thank you very much for the explanations. Seems like I got the wrong battery ...

Do I have to specify the "Max Current" [Battery Current Max] for the 12S2P Samsung 30Q battery as 15A in the VESC tool/app (https://vesc-project.com/node/938) if it is connected to 2 VESCs (see picture below)?

What should I input as "Min Current" [Battery Current Regen]?

Thanks a lot!

![IMG_7677|371x500](upload://3UkOUVjir00rdpQrkXI01iqikJ1.jpeg)
```

---
## \#89 Posted by: dildoritos Posted at: 2019-12-18T00:08:12.328Z Reads: 21

```
could you post a link for a li-ion battery with enough juice that wont break the bank?

my fallback plan is a couple of these which I know will work but range won't be all I desire

https://www.ebay.com/itm/HRB-12S-5000mAh-Lipo-Battery-50C-EC5-for-Drone-RC-Helicopter-Airplane-Car-Truck/153440557614?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D1%26asc%3D20131003132420%26meid%3D8704d7352f894046aa55fc4c77bd76aa%26pid%3D100005%26rk%3D2%26rkt%3D12%26mehot%3Dpf%26sd%3D264498276367%26itm%3D153440557614%26pmt%3D1%26noa%3D0%26pg%3D2047675&_trksid=p2047675.c100005.m1851
```

---
## \#90 Posted by: Okami Posted at: 2019-12-29T12:25:11.815Z Reads: 15

```
Well im in search for such ready made battery as well. Chinese seem to offer up to 2kw of power for higher end ebike builds but havent really tested these.

AERDU 36V 10S4P 12.8Ah For LGEBMH11865 13ah 12ah with 25A BMS 42V lithium battery pack ebike electric car bicycle motor scooter
 https://s.click.aliexpress.com/e/UBRyg06FD
2x of these would give low end - medium performance.

But range would be more

So it depends are u after range or power more
Also if u are for it in long run, might as well order custom made one.

Though these chinese made packs could be a gamble, wires are rather thin on these and wouldnt compare to lipo pack

--
48V 20AH Battery 36V Ebike Battery 1500W electric bike battery 52V battery for Bike 30AH 25A 35A 45A BMS APP Powerful Customized
 https://s.click.aliexpress.com/e/tQf2sBimX

If they could do 44V and higher discharge might be good, but yeh if u got money might as well find someone in usa.

44V because ebike run 48v but that is too high for vesc in most cases, though some do 13s but on street boards i think
```

---

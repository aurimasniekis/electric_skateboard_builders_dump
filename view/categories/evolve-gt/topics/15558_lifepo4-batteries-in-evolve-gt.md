# LiFePO4 Batteries in Evolve GT?

### Replies: 136 Views: 13051

## \#1 Posted by: VikasG Posted at: 2017-01-02T23:22:49.380Z Reads: 479

```
Like the title says. Is it possible to install LiFePO4 batteries in the Evolve GT? As much as I love this board, the voltage sag is ridiculous and the only board I know that uses LiFePO4 is the Boosted Board. How would this affect range/performance? Would the board even work or would the BMS fail to work?
```

---
## \#2 Posted by: Pantologist Posted at: 2017-01-03T01:17:05.906Z Reads: 453

```
The BMS wouldn't work and it wouldn't be safe to even use it since it would be charging at a higher voltage compared to LiFePO4 cells. 

You'll be getting less range for sure in the same space. 

I am pretty sure my Boosted Board doesn't say that much and my DIY board with the same battery as my Boosted didnt sag much either.
```

---
## \#3 Posted by: VikasG Posted at: 2017-01-03T01:38:18.967Z Reads: 426

```
Shoot. I wonder how much it would cost to change the battery and have a new BMS+ESC. I really like the integrated deck concept of the GT - haven't seen anyone else do it. Carbon fiber is a pretty awesome material.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-01-03T01:50:27.819Z Reads: 405

```
I would be interested in what you experience and feel when the voltage sag is present. And do you also have that issue with the street setup? It also would be interesting which kind of cells they use.
```

---
## \#5 Posted by: VikasG Posted at: 2017-01-03T02:46:28.282Z Reads: 393

```
**Board I Use:** Evolve Carbon GT

**Battery They Use:** 360Wh(36v10ah) 10s4p Li-ion 

**My Experience:** 
*Part 1 - 100% Charge:*
When you're charged up to 100%, the voltage sag makes no difference in the performance of the board. The only reason I could tell the battery was sagging was because the percentage on the remote dips heavily. However, after reaching max speed or cruising speed, the battery percentage goes back to normal. Until you fall below 50% (12ish miles) you can floor the board and ride it as hard as you want with no issues. This is all in GT mode by the way.
*Part 2 - 50% Charge:*
However when you fall below 50% its a completely different story. The board will be fine, but you won't be able to use GT or FAST mode for very long as the battery sags below 20% and switches to ECO mode. This is a safety feature as Evolve doesn't want the board turning off on you sending your face into the pavement. If you stay in ECO mode for the rest of the ride, you'll be fine. That really is the only issue caused by the voltage sag. Oh, and the fact that the battery percentage indicator is pretty much useless.

In short: I still love the board.
```

---
## \#6 Posted by: Pantologist Posted at: 2017-01-03T02:55:10.678Z Reads: 357

```
A lot. Basically a whole new build except for the motors and deck. 

A new intelligent BMS is going to be like $100 like Raphael Chang's BMS. 

A new set of ESCs will be around $200-$400.
```

---
## \#7 Posted by: Pantologist Posted at: 2017-01-03T02:57:23.567Z Reads: 337

```
I can't believe Evolve is using a simple voltmeter for remaining battery capacity... it is a $1500+ board lol. 

So basically you can only have fun until the battery gets to 50%? Then you can't even climb a hill?
```

---
## \#8 Posted by: VikasG Posted at: 2017-01-03T03:10:14.506Z Reads: 331

```
Pretty much. You'll be able to climb a hill, but fairly slowly and maybe about 20% grade at most at a snail's pace. Honestly a board that costs $2K should've been better designed. The real appeal for me was the integrated enclosure - that was pretty much 100% my selling point. But I can say for now, that if you want a prebuilt board from an established company, Evolve is the best.
```

---
## \#9 Posted by: baxter Posted at: 2017-01-03T03:11:18.401Z Reads: 325

```
I think the more relevant questions are firstly; what are the dimensions of the CGT battery compartment, and secondly - what are the alternatives for configuring LiFeP04 cells and a BMS within that enclosure to give you less voltage sag with equivalent (or better) performance?  :slight_smile:
```

---
## \#10 Posted by: VikasG Posted at: 2017-01-03T03:31:29.247Z Reads: 316

```
I just unscrewed the board to measure it out and here are the rough measurements for the compartment:

**Length:** 59cm (23.2 in.)
**Width:** 13.5cm (5.3 in.)
**Height:** 2cm (0.78 in.)

59x13.5x2 cm

23.2x5.3x0.78 in.
```

---
## \#11 Posted by: Pantologist Posted at: 2017-01-03T03:33:56.095Z Reads: 293

```
So just based on height, A123 26mm cells won't be a possibility(Boosted cells). I guess you could go LiPos?
```

---
## \#12 Posted by: caustin Posted at: 2017-01-03T03:38:36.472Z Reads: 288

```
Have you ever tried another evolve CF GT to compare battery sag experience?  Or another evolve battery in your deck, if you have any local esk8 to test with.
```

---
## \#13 Posted by: VikasG Posted at: 2017-01-03T03:48:10.225Z Reads: 285

```
I don't know anyone else with an electric skateboard - much less an Evolve board :frowning:. But based on what I read online, the voltage sag is a common issue - in fact its common among all boards that use Li-ion cells but you can really tell on Evolve because of the powerful motors combined with the battery meter on the remote.
```

---
## \#14 Posted by: VikasG Posted at: 2017-01-03T03:52:30.546Z Reads: 281

```
Aren't LiPos unsafe? I also feel like charging them would be more complicated and annoying. 

How about these?

http://www.batteryspace.com/A123-System-Nanophosphate-LiFePO4-18650-Rechargeable-Cell-3.2V-1100mAh.aspx

I know they are 18650, but would the fact that they are LiFePO4 make a difference?
```

---
## \#15 Posted by: evoheyax Posted at: 2017-01-03T04:05:29.582Z Reads: 271

```
[quote="VikasG, post:3, topic:15558"]
integrated deck concept of the GT - haven't seen anyone else do it.
[/quote]

You should check out my latest 4wd build. I use wood, which is more flexible (not a lot of flex, but enough to absorb some road vibrations) and more durable than carbon fiber. Chaka's free ride deck uses the same idea (I got some of my ideas from his deck). I should have hollow core decks ready for sale in the near future for sale. And I'm working on a complete also.

[quote="VikasG, post:8, topic:15558"]
You'll be able to climb a hill, but fairly slowly and maybe about 20% grade at most at a snail's pace
[/quote]

With my 4wd hub motor board, I can climb 20% grade hills at speeds above 20 mph... This is the kind of power my completes will have. Everything on the market right now is a toy. But 2017 is going to be a big year, power we've never seen before will become available to the public.
```

---
## \#16 Posted by: baxter Posted at: 2017-01-03T04:09:43.099Z Reads: 257

```
In terms of making an equivalent battery with that type of cell, the A123 cells you have noted are lower capacity cells (1100 mAH as opposed to 2500mAH), and they are lower voltage (3.2 as opposed to 3.6v), so a rough calculation should indicate that If you made a battery of the same dimensions as your existing CGT battery, it would be at a lower voltage and smaller capacity (in watt hours).
```

---
## \#17 Posted by: VikasG Posted at: 2017-01-03T05:27:30.025Z Reads: 249

```
Wow, that's not even half the capacity. Do you think it would be worth the trade off for the increased output?
```

---
## \#18 Posted by: VikasG Posted at: 2017-01-03T05:40:04.032Z Reads: 253

```
I would assume carbon fiber is a lot more durable than wood? I mean wood may feel more solid but from what I know, carbon fiber is used in high end cars for a reason.

Your board sounds really cool and read your post on the importance of redundancy. I'd love to see pictures of it! Maybe when I get more money I'll buy your decks as I am still a high school student working part time. The Evolve Carbon GT was a really big expense (almost all my money in fact) and I'm very low right now. As for hill climbing - I live in Ohio so I don't have to worry about large hills as many are 10-15% at most and the GT accelerates up those hills up to 22mph without breaking a sweat.
```

---
## \#19 Posted by: baxter Posted at: 2017-01-03T05:44:29.748Z Reads: 241

```
To get the best bang for your buck at higher discharge rates, I would go for pairs of 5S Lipos and wire them in series and then parallel. 

Maybe wire in a 10S BMS for simplified charging (evolve charger compatible?)  It really comes down to $.
```

---
## \#20 Posted by: VikasG Posted at: 2017-01-03T07:08:31.010Z Reads: 229

```
I'm just scared of the potential hazards that come with having LiPos. Just for the sake of having the option - if cost wasn't an issue, what would you recommend? 26650 A123 LiFePO4 cells are ruled out because of their width being more than 0.7in.
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-01-03T09:41:55.653Z Reads: 212

```
And how far can you go after the board switched to eco mode. And are you riding all terrain or street wheels?
Too me it sounds like a software issue and not a voltage sag issue. The battery would do fine but they restrict the performance by the software.
```

---
## \#22 Posted by: jga Posted at: 2017-01-03T11:27:30.236Z Reads: 204

```
How can you do series then parallel?
```

---
## \#23 Posted by: baxter Posted at: 2017-01-03T14:01:49.775Z Reads: 202

```
By connecting two packs in series you increase the voltage, but keep the same mAh rating, so two 5s in series would be 10s. 

Connecting another pair of 5s batteries in parallel, might be done to  increase the total mAh of the pack, keeping the voltage the same.
```

---
## \#24 Posted by: Pantologist Posted at: 2017-01-03T14:13:59.220Z Reads: 201

```
All we have to do is reprogram the board to not be retarded. I wonder what would happen if you used a regular remote. Where exactly is the"Switch to Eco mode" command. The remote, ESC or BMS?
```

---
## \#25 Posted by: PXSS Posted at: 2017-01-03T15:23:09.434Z Reads: 197

```
Not a software issue imo. Would you rather sag until the esc cuts off? Would you rather it sag under 2.5V/cell and damage the cells permanently? Cause that's what happens when you run them under 2.5V/cell.
I've ran a pack down to 2V/cell and it now holds roughly 80% capacity after a FOUR cycles.
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-01-03T15:36:39.538Z Reads: 207

```
Just a little explenation.
The evolves battery % value shows the battery capacity for a no load situation. So i guess when it shows 0% then the battery should bet at roughly 3.5V a cell with no load. If you would add load in this Siutaion it would drop to 2.5V.
Now as VigasG mentioned the board is at 50% in a no load situation. Now you add load and the % value drops below 20%. I bet money that we are not even below 3.0V under load in this situation. When you do this a bit too long the board switches automatically to ECO mode. And i would say they do this too early. 

**But why would they do this?** 
**first guess:** Their motor controller is not really smart and the ECO mode switch is controlled by the remote. And if the software is bad the remote would not even know that the board is at a load situation with voltage sag and thinks the battery is that low in a no load situation. 
**second guess:** Could be that they want to be on the very safe side with their batterys and try to avoid service calls because of broken batterys. On a street setup you won't stress the batterys too much but on the All Terrain setup they can get warm.
**third guess:** They tell that the board can do a lot of miles. And by reducing the power you can achieve a much better range. Otherwise the costumers would complain very soon that the board has a bad range.
```

---
## \#27 Posted by: E-Boarding Posted at: 2017-01-03T16:21:06.018Z Reads: 195

```
Can you tell what brand and model of Li-ion is build in there?
Maybe they can be replaced with some major-brand higher-quality li-ion cells that sag much less?
```

---
## \#28 Posted by: PXSS Posted at: 2017-01-03T17:00:08.338Z Reads: 193

```
Batteries get damaged when under 2.5V, regardless of the load... you can be running 25A through them or no load through them, if they go beneath 2.5V at ANY point, they get damaged. 

I ran batteries under load to 2.0V, they sprung back to 2.8V at no load. They were still permanently damaged even though they were barely cycled. I would love to post the graphs but it is work related and I cannot do so.

You could test it yourself with a single cell and a programmable load. Try running your cells down several cycles and just watch the capacity go to crap.  

The 3.0V sag limit might be conservative, but it's a safety feature to keep your batteries from dying 6 months from now and claiming warranty or something because the battery is bad. You can say it's too early, but it really isn't if you want your batteries to last 100s of cycles. 

So yes, guesses 2 and 3 are probably right.
```

---
## \#29 Posted by: VikasG Posted at: 2017-01-03T17:02:22.741Z Reads: 177

```
I'm riding on the street wheels. I haven't really done an all-out range test. But based on how the board reacts and the battery percentage, I could easily get 22+ miles. If I was light and didn't go up hills I could probably get fairly close to the 31 miles they advertise (28 I'm guessing). I've seen some people (not Evolve) get almost 37 miles on ECO so I'm not all that worried about range.
```

---
## \#30 Posted by: VikasG Posted at: 2017-01-03T17:05:38.146Z Reads: 178

```
No one quite knows what exact brand they are using but I can confirm they aren't a brand name - which is awful considering this board is $2000+. They haven't had any issues with quality but the voltage sag could be because they cheaped out on the cells. I'm 100% sure the batteries aren't manufactured by Samsung, LG or Panasonic.
```

---
## \#31 Posted by: Ackmaniac Posted at: 2017-01-03T17:06:55.591Z Reads: 174

```
@PXSS i think you got me wrong. Just to make it clear, what do you think at which load the cell is when the remote shows 50% without load.
```

---
## \#32 Posted by: VikasG Posted at: 2017-01-03T17:09:19.761Z Reads: 175

```
I don't know if I'm getting your question. But if you are asking whether the 50% reading is accurate - I'm assuming it is, since riding on ECO mode limits motor power and the sag is down 2% while accelerating and goes back up to 50%/ non-load percentage while cruising.
```

---
## \#33 Posted by: VikasG Posted at: 2017-01-03T17:12:44.823Z Reads: 175

```
I'm pretty sure 2 is correct. The cells aren't of the highest quality so restricting them from sagging too much would stop them from dying. 3 might not be so accurate as they pretty clearly state everywhere that ECO mode will give you the most range and that the 31 mile estimate came from ECO mode etc. etc.
```

---
## \#34 Posted by: Ackmaniac Posted at: 2017-01-03T17:14:09.110Z Reads: 171

```
No the sentence was for PXSS. Because he thinks that i meant to put load on a cell which is already down to 2.5V even without load. But all of this doesn't matter because we can't change it anyway. Only if you would use VESCs you could control it. But you don't have access to the evolve software.
```

---
## \#35 Posted by: E-Boarding Posted at: 2017-01-03T17:22:46.298Z Reads: 173

```
[quote="VikasG, post:30, topic:15558"]
confirm they aren't a brand name
[/quote]

How do you know, you can't b 100% sure.

You want to fix the voltage sag, but you've to find out the exact battery specs first to see what causes the sag.
Or you can replace random parts of the board and in the end nothing helps because the whole drive-drain is bad enginerred.
```

---
## \#36 Posted by: Pantologist Posted at: 2017-01-03T17:43:49.751Z Reads: 165

```
What's wrong with the drive train? 

Is there anything good about this board lol?
```

---
## \#37 Posted by: PXSS Posted at: 2017-01-03T17:58:29.513Z Reads: 162

```
@Ackmaniac, no I got what you meant. When it is at 50%, no load voltage is ~3.6V. What I meant is if he puils enough current to sag them down to 2.5V, the battery gets damaged regardless of the no load voltage.  

@VikasG. My recommendation is go to a LiPo setup. You can still add a BMS to LiPos. They're no different than Li-ions in that regard. 
Pros: little/no sag, more power, cheap. 
Cons: lower energy density, needs a new bms and esc.
```

---
## \#38 Posted by: VikasG Posted at: 2017-01-03T18:33:22.710Z Reads: 162

```
I've done some research and kinda confirmed with Evolve that the batteries aren't from any major brand. The only real specs I can give are that the the batteries are 10s4p 360Wh at 36V/10a.
```

---
## \#39 Posted by: VikasG Posted at: 2017-01-03T18:34:53.880Z Reads: 160

```
Nothing is wrong with the drive train. He was just saying that hypothetically - as in if I spent all my money replacing parts but in the end the whole drive train was the issue, it would've been pointless.
```

---
## \#40 Posted by: VikasG Posted at: 2017-01-03T18:36:50.958Z Reads: 161

```
Honestly, thanks for the recommendation. But my only real concern with LiPos are the extensive care you have to take of them to prevent fire-hazards etc. I doubt the Carbon GT has a fire retardant casing like the Boosted Board since the entire casing is underneath your feet.
```

---
## \#41 Posted by: E-Boarding Posted at: 2017-01-03T18:46:22.252Z Reads: 146

```
The Evolve Gen2 used LiPos with same enclosure but I think it's a step backwarts.
Take a look at the market, 90% of all major brand with powerful boards use Li-ions and they sag less (mostly with major brand cells)

I don't know what is wrong with board, I guess the motors draw more power than the battery can handle, so replace the motor or the battery or the BMS, who knows...
As we don't know what the battery can handle it is hard to guess what would make the drive-drain better.

Good luck :)
```

---
## \#42 Posted by: VikasG Posted at: 2017-01-03T18:49:06.991Z Reads: 142

```
It could be the motors. They really are incredibly powerful - probably too much for their own good. I've seen them get the Carbon up to 70km/h on those motors. Crazy
```

---
## \#43 Posted by: PXSS Posted at: 2017-01-03T18:53:20.799Z Reads: 148

```
What extensive care??? You have to take the exact same precautions with Li-ions...

Make a pack out of VTC6s or Samsung 30Qs if you want cheaper. Evolve BMS might still work with either of those. 
It'll be a 432Wh pack if you go with VTC6s. They are about $7/cell though. 30Qs are cheaper and almost the same Wh
```

---
## \#44 Posted by: VikasG Posted at: 2017-01-03T19:07:08.732Z Reads: 149

```
With that knowledge, I'm much more inclined to do with LiPos. Do you think the Evolve BMS/ESC combo will get fried if I make the LiPos 12s? If I do make it 12s what would my Wh rating be/what range would I get? Thank you so much for the help!
```

---
## \#45 Posted by: Pantologist Posted at: 2017-01-03T19:19:50.972Z Reads: 148

```
10S BMS isn't going to work with a12S battery. Wouldn't have enough balance connectors.
```

---
## \#46 Posted by: oripaamoni Posted at: 2017-01-03T19:20:50.835Z Reads: 152

```
i think the issue you will run into with lipos is the lower energy density, Not sure there is enough space and cell that will fill the space adequetly
```

---
## \#47 Posted by: Pantologist Posted at: 2017-01-03T19:34:51.852Z Reads: 149

```
Lipos don't waste as much space since they are pouches instead of cylindrical cells but lithium ions are usually of higher density.
```

---
## \#48 Posted by: VikasG Posted at: 2017-01-03T19:41:38.645Z Reads: 148

```
I think the biggest issue will be the height of the enclosure. Its only 0.78" thick. Most LiPos I've seen are boxes and seem too thick.
```

---
## \#49 Posted by: evoheyax Posted at: 2017-01-03T19:42:14.302Z Reads: 157

```
[quote="E-Boarding, post:41, topic:15558"]
Take a look at the market, 90% of all major brand with powerful boards use Li-ions and they sag less
[/quote]

Lets take a step back and look at why cells sag. A cell has a certain amount of resistance (which determines what the highest safe rate of discharging is). The higher the resistance, the more the sag. If a put cells in parallel, you get less sag, because you lower the resistance across more cells. The C rating in lipos gives an idea of resistance, as the higher the C rating, the lower the internal resistance (li-ion manufacturers usually give you an internal resistance number, while lipo manufacturers usually just give a C rating). The C rating of lipos are usually much higher than li-ion. Since they have a lower resistance, they tend to sag less. Evolve exacerbated it's sagging it had with the GT (which I believe uses lipos) when it switched to li-ion in the CGT.

If sagging is an issue, look at motor efficiency (which I would imagine they engineered to be pretty good) and mostly, the battery. Lipos were designed mostly for RC hobbyists. You don't see a lot of RC guys using li-ion, becuase the lipos perform way better. We require drastically more power from our boards than in the standard RC world (there's always some out liars), so why would we go to li-ion? There's some safety benefits for sure, but li-ion batteries in a 10s4p config will never supply enough amps without drastically sagging on say 15% grade hills, which I'm surrounded by. It may work great if you live in a flat environment, but I need double that to reduce sag.
```

---
## \#50 Posted by: evoheyax Posted at: 2017-01-03T19:56:11.013Z Reads: 155

```
Zippy makes some of the best lipos. I would recommend this:

https://hobbyking.com/en_us/zippy-flightmax-8000mah-2s1p-30c.html

You can probably use the same bms if you use 5 of these in series to make a 10s 8000 mAh zippy lipo pack. I can guarantee that you'll get less sag, as at 30 c and 8 Ah, that's 240 max continuous amps, which is probably way higher than what they are using now. Not a cheap upgrade, but will likely solve your issues. If the bms doesn't work, you might need to replace the bms also. If I were you, I'd replace the bms with any 10s bms, upgrade the esc to the VESC in FOC (maybe direct fet vesc from chaka or a vesc-x or even the VESC 6 when it comes out, and replace the battery with the zippy cells I posted above. Regular VESC is not good enough for a mono drive with hills).
```

---
## \#52 Posted by: VikasG Posted at: 2017-01-03T21:28:06.444Z Reads: 146

```
Thanks! I'll look into it
```

---
## \#53 Posted by: evoheyax Posted at: 2017-01-03T21:31:18.193Z Reads: 146

```
I have used many of these cells with great results in high amp situations btw. If they get below 2.8, don't try to charge them. Otherwise, as long as you don't cut the pouch open, your batteries won'tt blow up.
```

---
## \#54 Posted by: VikasG Posted at: 2017-01-03T22:18:38.655Z Reads: 139

```
How can I see voltage. The remote shows voltage for the GT but in case I switch out the BMS+ESC, how am i supposed to keep track? Sorry, as you can see I'm a complete noob at this stuff
```

---
## \#55 Posted by: evoheyax Posted at: 2017-01-03T22:20:47.468Z Reads: 141

```
You can use a small volt meter. They cost around $7 each on amazon. You can also use a smart phone app. I make one, and there's a few others.
```

---
## \#56 Posted by: Ackmaniac Posted at: 2017-01-03T22:48:18.973Z Reads: 139

```
Can you see the voltage on the Carbon remote or only the percentage?
```

---
## \#57 Posted by: VikasG Posted at: 2017-01-03T23:03:07.953Z Reads: 138

```
If you double tap the button on the left and go to more info it will show you voltage. I'm confused though. I just checked and it says it has 41.7v when the battery is 36v/10a. Maybe I'm stupid.
```

---
## \#58 Posted by: Ackmaniac Posted at: 2017-01-03T23:08:28.510Z Reads: 140

```
That is awesome. Now please tell us what the voltage is when the battery shows for example 50% without load and what is the voltage when it sags below 20% under load, so that it switches automatically to ECO mode? That would be very very interesting.
```

---
## \#59 Posted by: VikasG Posted at: 2017-01-03T23:13:55.979Z Reads: 138

```
I would love to but I'm in Ohio and its the middle of winter. Surprisingly there's no snow but its raining pretty heavily. It's going to be a while before I can do more testing.
```

---
## \#60 Posted by: Pantologist Posted at: 2017-01-03T23:30:16.619Z Reads: 143

```
[quote="VikasG, post:57, topic:15558"]
just checked and it says it has 41.7v when the battery is 36v/10a. Maybe I'm stupid.
[/quote]

Nominal voltage per cell is 3.6v

10 in series is 3.6v x 10 = 36v. Batteries are listed at their nominal voltages.

Charging voltage per cell is 4.2v. Multiplied by 10, is 42v. So everything is good with the battery.
```

---
## \#61 Posted by: Ackmaniac Posted at: 2017-01-03T23:36:26.193Z Reads: 140

```
Maybe somebody else with a evolve GT can test and share the values with us. I really would be interested at which voltage under load the board switches automatically to ECO mode.
```

---
## \#62 Posted by: Pantologist Posted at: 2017-01-04T00:15:00.030Z Reads: 135

```
Honestly, this whole endeavor isn't really worth it. The deck isn't exactly flawless either. There have been multiple cases of random cracks in the carbon fiber. 

The value on these things are quite high still. You could try selling it and going DIY to get exactly what you want. Modifying your expensive board with a bunch of issues will probably end in a money pit.
```

---
## \#63 Posted by: VikasG Posted at: 2017-01-04T00:28:45.302Z Reads: 138

```
You're probably right, but I will have to point out that they did a quick revision of the board after the first batch. The cracking is said to have been fixed. Maybe its the sentimental value since its my "real" first E-Board or that I spent so much time working for it, but I really love the board. I find it has plenty of power, the remote is awesome, and even for going distances, the board is fine until it reaches 50%. 12 miles is plenty. Granted, I don't plan on doing any major modifications except making a 26T gear until maybe its truly necessary.
```

---
## \#64 Posted by: PXSS Posted at: 2017-01-04T01:24:28.969Z Reads: 149

```
LiPos vs LiIons

If you go with LiPos,
Pros
You will have no power issues at all, the discharge curve for LiPos is very flat (4.15V at 95% and 3.5V at 15%) so your performance throughout most of your ride will not vary until your batteries are about 15% when the voltage drops extremely fast 3.5V to 3.0V empty). Since their internal resistance is low you also do not get a lot of voltage sag. 
Cons
You have to get a new VESC and BMS. The BMS on the CGT is meant for Li-ions and if it's really just a voltmeter measuring capacity, it will tell you you have 20% left when your LiPos are completely dead. You also have to make sure that whatever setup you get fits within the CGT compartments. Lastly, you won't have as much endurance, a 10S 8Ah battery like @evoheyax suggested only has  288Wh. 

If you go with LiIons, 
Pros
You can keep your current BMS and VESC. The cells are very likely to be the same size as whatever is in the compartment already so no need to worry about a 10S4P pack fitting in. If you get a VTC6 pack like I suggested earlier, you will get more endurance as the pack has a total of 432Wh. 
Cons
You will still have some power issues, not nearly as bad as you do now but basically the discharge curve for LiIons decreases linearly from about 4V to 3.2V from 95%-20% at which point the voltage drops fast (3.2V to 2.5V empty). The VTC6s are known not to sag much but they will still sag more than a LiPo.

Both options would be pretty expensive, ~$350-450
```

---
## \#65 Posted by: VikasG Posted at: 2017-01-04T03:34:17.820Z Reads: 140

```
Thanks for the comparison. I'm trying to keep my BMS+VESC because of its compatibility with the remote. The VTC6 seem to also be rated at 10a - wouldn't that mean they would have the same issues?
```

---
## \#66 Posted by: PXSS Posted at: 2017-01-04T04:16:27.180Z Reads: 145

```
VTC6 are rated up to 30A/cell as long as you keep them under 80C.

Here's a graph of the voltage sag so you have an idea. The cells in the CGT are probably knock offs of the samsung 25R that a lot of people around here use. 

In this graph, red is 25R and blue is VTC6. 
Top curve is 0.2A which is close enough to no load. The next one down is 1A, then 5A, then 10A and finally 20A continuous. 

<img src="/uploads/db1493/original/3X/7/3/736b4f980b7f142a4a56d4c52100a390040c1f37.PNG" width="690" height="387">

As you can see, VTC6 sag a little less when at 20A than the 25R at 10A, yours being knock offs are probably slightly worse.

You can also see that at 50% capacity (1.25Ah) 25R are at 3.7V pulling 0.2A and they sag down to 3.1V pulling 20A, which is probably what you're seeing. 
VTC6 at 1.25Ah go from 3.8V pulling 0.2A to 3.4V pulling 20A.

In reality, motors are a power load and not a current load so the sag at equivalent power levels is slightly lower for the VTC6. 

What you see is worst case scenario
```

---
## \#67 Posted by: Rob.Endless Posted at: 2017-01-04T04:30:11.644Z Reads: 135

```
When did you get your CGT? I guess I am just lucky, living only a few hours from Evolve US, I was one of the first non beta testers with a CGT and I haven't had any issues (minus the motor pulleys eventually wearing out). 1500 plus miles later and everything works flawlessly (I do live in a flat area tho).

I have never noticed the board going into eco mode on it's own. Maybe it's for newer batches of CGTs. On a few occasions, I rode the board till it was pretty much dead lol and I was in GT mode the whole time. Also, it didn't just instantly go from 26mph to zero mph when it died. (Side note, I even use bigger motor pulleys so I go faster than 26mph and I still feel really safe at lower battery percentage)

Edit: off topic, but let me add, after riding my Trampa build from Bara, I feel way safer on the CGT lol. The Trampa build is not only powerful but riding on ESCs compared to a commercial board is a night and day difference . ESC acceleration and braking is scary.
```

---
## \#68 Posted by: VikasG Posted at: 2017-01-04T04:54:48.604Z Reads: 133

```
Don't get me wrong. I love my CGT - not even remotely regretting purchasing it. From what I know, the voltage sag issue is widely accepted as being in all GT boards but it really only caused issues once the batteries drained to 50%. 

When the first batch of GTs came out, there were two main issues everyone was talking about. Engaging reverse being too easy while riding and voltage sag to the point where the board shut off. The first issue was fixed by sending out remotes with new firmware (you can get yours updated if you send yours back as well) that required multiple clicks to switch to reverse - thus eliminating the problem. 

Voltage sag has always been talked about as the battery percentage going down during hard acceleration confirmed this. The first batch had the board shut off when in GT mode and accelerating since the battery couldn't handle it - I imagine this would just make the board coast to a stop but its still an issue. This was resolved in the same firmware update mentioned above by making the board switch to ECO mode when the battery sags below 20% to avoid shutting off or damage to the cells. This may also help with range when the battery genuinely falls below 20%. 

I've never heard of a case like yours where everything is flawless. I'd love to find out what changed if yours is perfect. Also, about the motor pulleys, I'd like to increase the speed as well - could you help me out and tell me what you did and what kind of speeds you're reaching? I wanted mine to hit 30mph, so I planned on making 26T gears for the wheels but I'd love to hear what you did.
```

---
## \#69 Posted by: Rob.Endless Posted at: 2017-01-04T05:08:05.773Z Reads: 125

```
Oh I love my CGT as well. I also love my Trampa build, it is a beast in every aspect. However, for daily use, I use the CGT for a few simple reasons, size and weight and I also don't want to wear out my Trampa tires lol. Urethane wheels just seem to last forever.

Crap, forgot to add that the only other issue I had was a BMS issue only after a few days of owning my CGT, I sent it back and it has been working flawlessly since then. I would be pretty damn pissed if my board just shuts off from hard acceleration. I would think I would have experienced this by now as I ride my CGT very aggressively.

I haven't had any issues with accidentally pressing buttons lol. I even wear gloves at times.

My main interest at this topic is the board switching to eco mode. I would totally hate this. Mine stays on GT mode even say at 20% battery life. I should take a video but I am too lazy on video editing and uploading lol.
```

---
## \#70 Posted by: VikasG Posted at: 2017-01-04T05:27:11.575Z Reads: 122

```
You can probably find out more about the reasoning behind the update by talking to Evolve AU as they are the ones that issued it.

Could you tell me more about your gearing setup? I'd love to hear more about it as I really want to be able to go a bit faster on my board.
```

---
## \#71 Posted by: VikasG Posted at: 2017-01-04T05:28:12.822Z Reads: 119

```
Its ridiculous how in-depth you guys go just to help a random dude on the internet like me. Seriously, thank you so much.
```

---
## \#72 Posted by: jga Posted at: 2017-01-04T18:36:37.446Z Reads: 127

```
Yes I know how it works, but from you post I thought you were connecting the same pair of batteries in parallel and in series. Now I understand there's actually two pairs! :wink:
```

---
## \#73 Posted by: E-Boarding Posted at: 2017-01-04T19:10:59.156Z Reads: 131

```
[quote="PXSS, post:66, topic:15558"]
As you can see, VTC6 sag a little less when at 20A than the 25R at 10A, yours being knock offs are probably slightly worse.
[/quote]

The Bamboo Enclosure fits 40cells, so assuming the Bamboo GT is 10S4P with 6,5Ah that would mean 1625mAh per cell but 25R is 2500mAh...
If it's a 10S3P, you could go up to 10S4P to decrease the sag.

Same with the Carbon GT, could be 10S5P or 10S6P.

http://i.imgur.com/d3AR7fV.jpg
looks like 5P...
```

---
## \#74 Posted by: Ackmaniac Posted at: 2017-01-04T20:07:44.211Z Reads: 127

```
What are the dimensions of the battery?
```

---
## \#75 Posted by: PXSS Posted at: 2017-01-04T20:28:16.122Z Reads: 128

```
@VikasG had stated it's a 10S4P 360Wh pack.
Each cell is 18.3mm diameter and 65.1mm long. Measure the pack  and you can figure out how many cells are in there...

@E-Boarding 
Plus your numbers are not making any sense. 
25R is 2500mAh not 2500Ah and I have no clue where you're getting the 16250Ah number from
```

---
## \#76 Posted by: IDVert3X Posted at: 2017-01-04T20:32:47.843Z Reads: 127

```
About the LiPo vs Li-ion topic, I created an informative thread about it already: 
http://www.electric-skateboard.builders/t/lets-talk-about-lipos-and-li-ions/12554

There was no interest in it tho...
```

---
## \#77 Posted by: VikasG Posted at: 2017-01-04T22:37:29.387Z Reads: 124

```
I'm reading that there are 40 cells so it would be 366mm/36.6cm long for just the cells and no wires. Since 20*18.3 = 366.
```

---
## \#78 Posted by: VikasG Posted at: 2017-01-04T23:10:39.621Z Reads: 125

```
Weird, I feel like that would one of the most debated topics. Maybe another thread regarding the same topic was created before?
```

---
## \#79 Posted by: Ackmaniac Posted at: 2017-01-04T23:27:11.899Z Reads: 124

```
To measure the physical size would be helpful.
```

---
## \#80 Posted by: Fiori Posted at: 2017-01-05T03:13:45.541Z Reads: 129

```
That's my photo from my tear down. This issue has literally been beat to death.... I really feel like people don't understand...... I read your original post. Honestly, if you are smashing around full throttle on GT mode and you've already traveled 12 miles(like you said in your original post)  you have to understand that your battery really isn't at 50 "percent" charge. 

I feel like that situations have less to do with Voltage sag, and more to due with people not understanding that you've probably depleted 80 percent of your battery capacity by that time. I can drain my battery on my CGT in 8 miles if i wanted to, or i can make it last 25 miles and take it easy. I can do the same thing in my car with gas.... I could make this same argument with the gas gauge in a car. The same car can get 5 MPG, or 25 MPG, just depends how you drive. 

Evolve is probably the only company that uses a battery percentage display(since they are the only company with an LCD remote out currently) and I feel like if other companies offered this, you'd see this complaint far more often with other brands and manufactures as well. Feeling like it really bit them in the butt, because some people just don't understand how it works and calculates that percentage,  I personally love the percentage display, and after having the board for less than a month i can actually use it to get a pretty good gauge of how much distance I have left.

The only real feasible thing you could do is research the HIGHEST QUALITY, HIGHEST CAPACITY, HIGHEST DISCHARGE RATING 18650 cells you can find and builds a custom pack to those dimensions. I believe you'd be surprised though..even if you did that you'd spend way more money than you're expecting just to get a lackluster result that is MAYBE a little bit better. Just my two cents...
```

---
## \#81 Posted by: baxter Posted at: 2017-01-05T03:34:28.237Z Reads: 130

```
I would have expected that by now there would be more complete board vendors offering packs of 26650 cells in their enclosures, given the performance figures they advertise.  But I suppose that would give you a reason to keep upgrading to their latest and greatest products (or go DIY!).

@VikasG, If it doesn't turn out to be a BMS/ESC issue, here's another idea to address voltage sag: 

You could build another CGT enclosure lid that increased the enclosure height about 7mm more than stock (using the existing bolt holes). With this you might be able to fit a low sag 26650 LiFePO4 pack in. You could make it out of fibreglass, aluminium, lexan (see through!) or whatever you like to build with, as long as it doesn't compromise the structural integrity of the deck and block the remote control signal (not carbon fibre :sob:).  

The higher enclosure lid height might compromise the drop-down style of the deck, but I am sure some of the more aesthetically minded members of the forum (like @MasterCho, or @whitepony to name just a couple) would be able to assist you in designing an awesome stealthy raised enclosure lid to fit flush on your CGT deck. :sunglasses:

Plus, you could always return it to its stock battery configuration later!  

I think this could be a popular mod for the Carbon GT for the DIY Community when the evolve factory warranties expire; or, I could just be talking out of my arse.
```

---
## \#82 Posted by: VikasG Posted at: 2017-01-05T03:39:41.796Z Reads: 127

```
I was actually considering what you said when I realized there was a volt meter on the remote. After you said it, It pretty much confirms my thought so I think putting the voltage underneath the percentage might be very helpful. <img src="/uploads/db1493/original/3X/1/4/146ba9aacd760bef8f175ecd6a159a3ca3505c2c.jpg" width="690" height="395">
The picture above comes from the early GT teaser and I drew an arrow to point out the fact that it shows voltage beneath the percentage. I wonder why this didn't make it to the final version as it probably would've helped people a lot more than the battery percentage and significantly reduce the amount of complaints.
```

---
## \#83 Posted by: Fiori Posted at: 2017-01-05T03:44:05.505Z Reads: 122

```
I agree I would love to have that view on my remote. Iv'e been meaning to monitor it when the battery gets low(yaknow, for science :p) but just have never really had much of a reason to do so.
```

---
## \#84 Posted by: VikasG Posted at: 2017-01-05T03:45:10.226Z Reads: 119

```
You are definitely on to something. If the aforementioned @MasterCho or @whitepony can design a nice looking lid, I'm pretty sure a LOT of Evolve owners would be glad to buy or modify their decks to fit those batteries. There's something wrong with me since I'm obsessed with having everything look perfect - I take 20 minutes or more after every.single.ride (yes, every)  just to inspect and clean the board with a cloth and make sure everything looks great. I'm like a 65% Form and 35% Function kinda guy - but I also have expect things to work perfectly when I'm dropping 2 grand on them.
```

---
## \#85 Posted by: VikasG Posted at: 2017-01-05T03:47:23.280Z Reads: 119

```
I also wish you could program the controller since I want to setup a 26T gear for higher top speed and reduction in low end torque. So I'd love to have a setting for 97mm 26T so we can have perfect readings no matter what.
```

---
## \#86 Posted by: VikasG Posted at: 2017-01-15T02:09:03.777Z Reads: 107

```
The size of the battery (if you still care) is:

40.6x12.7 cm

16x5 in.
```

---
## \#87 Posted by: Ackmaniac Posted at: 2017-01-15T02:15:40.867Z Reads: 104

```
Thanks for the measuring. The dimensions would fit a 10S4P battery.
```

---
## \#88 Posted by: VikasG Posted at: 2017-01-15T02:27:39.891Z Reads: 106

```
Yep. So overall, I'm assuming getting higher quality Samsung or Sony cells would effectively eliminate voltage sag? I'd have to ask someone to build me a pack with Sony VCT6 or Samsung 25R.
```

---
## \#89 Posted by: Ackmaniac Posted at: 2017-01-15T02:30:46.509Z Reads: 103

```
No, seems that your remote is switching to ECO mode too early which is regulated by the remotes software. If i was you i would ask Evolve if your behavior is normal or if they have already a software update for the remote. With another battery the automatic switch to ECO mode would only happen a bit later.
```

---
## \#90 Posted by: VikasG Posted at: 2017-01-15T02:45:32.162Z Reads: 104

```
I've confirmed with Evolve that its completely normal. Its caused by voltage sag since the motors are pulling too much power from the board at once
```

---
## \#91 Posted by: Ackmaniac Posted at: 2017-01-15T02:47:01.799Z Reads: 102

```
Then we need to know at which voltage (not percent) the battery when it switches automatically to ECO mode under load.
```

---
## \#92 Posted by: VikasG Posted at: 2017-01-15T03:14:26.019Z Reads: 99

```
I don't know if I'll be able to test that. I won't be able to see the percentage or mode while looking at voltage so in case the percentage gets too low the board might shut off (maybe it won't but I can't take the chance). Sorry
```

---
## \#93 Posted by: PXSS Posted at: 2017-01-15T04:25:16.135Z Reads: 101

```
It can be fixed by a VTC6 pack. A 25R pack wont be enough.
```

---
## \#94 Posted by: Ackmaniac Posted at: 2017-01-15T12:45:21.396Z Reads: 101

```
Then wait until it switched the first time to ECO mode. Then switch back to GT mode and have a look at the voltage when you do a hard acceleration where it would switch normally to ECO mode.
```

---
## \#95 Posted by: VikasG Posted at: 2017-01-16T03:09:16.990Z Reads: 98

```
Would you happen to know what 0% charge on the board would translate to in volts? If 42v is max, then what is empty?
```

---
## \#96 Posted by: Pantologist Posted at: 2017-01-16T03:20:52.455Z Reads: 97

```
It should be 3v per cell. 30v. That is a recommended safe cutoff but who knows with Evolve.
```

---
## \#97 Posted by: VikasG Posted at: 2017-01-16T03:33:28.679Z Reads: 102

```
Thanks. So assuming Evolve follows, to answer @Ackmaniac's question, 32.4v should be when the board switches to ECO mode. 

But oddly enough, even though it switches to ECO mode and the remote shows it, you don't feel the effect until you let go of the accelerator and try to accelerate again. 
Scenario that happened: I'm in GT accelerating up a hill, but the percentage drops below 20% (hits 9% during acceleration) - which switched it to ECO but the board still had the same relentless acceleration until I stopped accelerating and started again, at which point it accelerated like ECO mode.
```

---
## \#98 Posted by: Fiori Posted at: 2017-01-16T04:18:54.750Z Reads: 101

```
I tested today. The board drops into eco at 34.0V. I tested it multiple times.
```

---
## \#99 Posted by: VikasG Posted at: 2017-01-16T04:39:22.928Z Reads: 99

```
Thanks for testing it out! Huge help! There you have your answer @Ackmaniac!
```

---
## \#100 Posted by: PXSS Posted at: 2017-01-16T05:19:50.469Z Reads: 100

```
Yikes! That is way early. Still got plenty to go at that point imo
```

---
## \#101 Posted by: VikasG Posted at: 2017-01-16T06:07:01.863Z Reads: 101

```
If you read my previous statement about how the board behaves when it sags and switches to ECO, maybe that explains it. Usually when it sags below 20%, it sags almost down to 9%. So, maybe its to prevent the board from shutting down and making you lose balance as it goes from its max acceleration to coasting - which is quite jarring. Remember that the board doesn't give up its torque ever, it is ridiculous.
```

---
## \#102 Posted by: Ackmaniac Posted at: 2017-01-16T07:15:03.435Z Reads: 101

```
But as I said two weeks ago. They switch into ECO far too early and it is a software issue and not a hardware issue. I think because they try to reduce service claims or want to extend the range by that so that they come closer to the range they advertise. 
And they don't have the VESCs feature to reduce the power only when necessary by voltage cutoff start and end.
```

---
## \#103 Posted by: PXSS Posted at: 2017-01-16T12:37:48.606Z Reads: 101

```
What I meant is 3.4V is not 20% left if you discharge to 2.8V. You can sag from 4.1V down to 3.4 V if you go up to 20A/cell. Or from 3.8V if you do 10A/cell. What is the empty voltage?? I think they are leaving too much energy on the table but that still doesn't mean is not a battery issue. 

@Ackmaniac, whether they relax the limits or not. Voltage drop is instantaneous and that can only be fixed by a better cell. Look at the curves... its all right there.
```

---
## \#104 Posted by: Ackmaniac Posted at: 2017-01-16T13:35:29.671Z Reads: 101

```
What I mean is when they switch to eco when the cell is below 3.4V under load then they do it too early. 
When the cell is at 3.4V without load then I guess they show already 0%.
```

---
## \#105 Posted by: VikasG Posted at: 2017-01-16T16:36:45.759Z Reads: 109

```
Huge thanks to **jpark13b** from the Evolve forums because he made a graph showing how the curve works for the Evolve board. This should help us a lot:
<img src="/uploads/db1493/original/3X/f/4/f44d7a0d151ab48636d69678c8d30d66babbb8c8.JPG" width="690" height="372">
```

---
## \#106 Posted by: PXSS Posted at: 2017-01-16T17:08:51.890Z Reads: 102

```
3.4V no load would show the SAME percentage as 3.4V under load. They're going by the voltage. They dont care whether its under load or not. That is why voltage sag is an issue
```

---
## \#107 Posted by: Ackmaniac Posted at: 2017-01-16T17:21:19.134Z Reads: 109

```
What I mean is that when they reach 3.4V under a lets say 15A a cell load then the remote thinks that it is at below 20% without load because it's not smart enough. 
So in a load moment they detect that the voltage is low and think they have no load. So they switch the mode.
```

---
## \#108 Posted by: PXSS Posted at: 2017-01-16T17:37:52.565Z Reads: 111

```
No. When they are at 3.4V their controller simply thinks it's at 3.4V, it does not care about no load voltage and neither should you. 

Unless you know discharge curves for every load condition, you cannot make a controller that is "smart enough". You cannot say ignore the voltage while we're drawing XX amps because that is literally how you would damage them. 

Their curve could be pulled lower by about .2V/cell but that would still not fix the problem just delay it slightly further.
```

---
## \#109 Posted by: PXSS Posted at: 2017-01-16T17:45:49.147Z Reads: 109

```
This is literally part of my job description. To come up with battery discharge models that are accurate whether you draw no load or 20A/cell so that we can have an accurate battery indicator during all flight conditions for military UAVs

Trust me, it is not a trivial task.
```

---
## \#110 Posted by: VikasG Posted at: 2017-01-16T17:50:19.568Z Reads: 109

```
Then would someone know how much it would cost to build a pack out of VTC6 cells that effectively eliminate voltage sag and have the necessary connectors to connect with the existing BMS+ESC combo?
```

---
## \#111 Posted by: PXSS Posted at: 2017-01-16T17:54:55.819Z Reads: 110

```
$400 if you DIY. Someone else will probably charge up to $600 based on the markups on 25Rs. 
$300 for the cells alone at Liionwholesale + 100ish bucks in wiring and stuff.
```

---
## \#112 Posted by: VikasG Posted at: 2017-01-16T18:03:36.983Z Reads: 113

```
I don't have the materials nor experience to work with batteries so someone else would have to do it. Would that be $600 to make a battery that's plug and play? I'd like it to be as easy as following this video:
https://www.youtube.com/watch?v=pkJfhjVHpyA
```

---
## \#113 Posted by: Ackmaniac Posted at: 2017-01-16T18:04:39.613Z Reads: 117

```
It is possible because the vesc is doing that. When you adjust the cutoff start to 3.0V and the cutoff end to 2.8V then it starts to reduce the power output when it reaches 3.0V and doesn't go below 2.8V.

So if the Battery can output 3.0V at 15A and we only draw 15A then there is no reduction. When we try to draw 20A then the we would go below 3.0V so it starts to reduce the power so that we end up somewhere between 3.0V and 2.8V which would result in something between 15A and 20A. It doesn't switch the mode. It only takes care that you stay in that range.
```

---
## \#114 Posted by: E-Boarding Posted at: 2017-01-16T19:13:23.427Z Reads: 122

```
[quote="PXSS, post:108, topic:15558"]
you cannot make a controller that is "smart enough"
[/quote]

Mellow is doing that with their BMS:
"It’s not all about protecting and preserving: bad battery management 
impacts fun riding as well. Two huge issues affect almost every e-skate 
on the market today, even the pricier models:  “false low capacity 
shutdown” after hill climbing due to voltage sag and “brake shutdown” 
due to inability to use regen brakes on a full battery.Mellow is 
unique in having eliminated both. The BMS uses triple fuel gauge 
measurements (voltage, Coulomb counting, Impedance TrackTM) to 
accurately read battery level and eliminate false readings."
```

---
## \#115 Posted by: VikasG Posted at: 2017-01-16T19:30:13.519Z Reads: 122

```
Mellow is actually really interesting. They seem to have the best tech out of any eSk8 available right now. Something that interested me about their system was the "Endless Ride: Acceleration 10% (pushing with cruise control)". I wonder if this means whatever speed you kick the board to, the board will keep its speed, or if the board has a max speed you kick up to.
```

---
## \#116 Posted by: VikasG Posted at: 2017-01-21T02:20:14.379Z Reads: 123

```
Guys I just made a thread. I feel like you guys would know best as a lot of you seem to be extremely knowledgeable in the topic. I'd love your opinions, thanks!

http://www.electric-skateboard.builders/t/what-would-happen-if-i-changed-the-motors-ultimate-evolve-gt/16415
```

---
## \#117 Posted by: okp Posted at: 2017-04-15T12:48:58.330Z Reads: 108

```
hey ! I was about to put replace the battery with 18650 to double the range in AT of my friends GT Bamboo. any recommendations? Are these BMS with switch / UART plug available somewhere ? I could still try to keep the BMS and just plug into a big 18650 pack.
```

---
## \#118 Posted by: VikasG Posted at: 2017-04-16T17:41:25.865Z Reads: 106

```
You have to take the BMS from the original battery and use that. Otherwise it won't work. Evolve also doesn't sell the BMS separately. But after you take the BMS, you can just make a normal 10s pack and it should work fine.
```

---
## \#119 Posted by: Nerdclot Posted at: 2017-06-20T09:53:02.445Z Reads: 91

```
board has bad range... I have one and it gets me 20miles tops in fast and eco the rest of the remaining 3-5
```

---
## \#120 Posted by: Nath Posted at: 2017-07-24T16:26:15.963Z Reads: 83

```
gts are lipo pouch cells not 18650s. i dont think you have opened your board at all have you mate? they are 10 x 10Ah batterys in series.
```

---
## \#122 Posted by: Jinra Posted at: 2017-07-25T04:58:12.511Z Reads: 83

```
LiPo pouches are the same tech as li-ion. People just use li-ion to describe cylinder cell batteries, so saying they're pouches but are li-ion, while technically correct, is not common nomenclature
```

---
## \#123 Posted by: BigBoyToys Posted at: 2017-07-25T04:59:43.700Z Reads: 83

```
Im confused, so are u saying they are lipos? Do we even know if they are using a polymer or liquid electrode in them?
```

---
## \#124 Posted by: Jinra Posted at: 2017-07-25T05:02:16.183Z Reads: 82

```
I'm actually not sure what the GT battery is anymore.. I thought they were cylinder cell li-ions, but I've never actuallly seen anyone take off the blue shrink wrap to see what's underneath. I'm basically saying lipos are still lithium ion (li-ion) technically, but we just use the term lipo to describe li-ion packs that are housed in polymer pouches, thus the term "li-po"
```

---
## \#125 Posted by: BigBoyToys Posted at: 2017-07-25T05:11:40.800Z Reads: 82

```
Well here's a pic of the pack.
<img src="/uploads/db1493/original/3X/7/d/7d6e5fbfb134c3e35de80c7ec7d34c2fa74443e2.jpg" width="600" height="315">
```

---
## \#126 Posted by: Jinra Posted at: 2017-07-25T05:14:36.382Z Reads: 82

```
Ah they do look like pouches, have you tried prying into it further? Perhaps it's a housing containing cylinder cells.
```

---
## \#127 Posted by: Nath Posted at: 2017-07-25T06:12:54.581Z Reads: 78

```
lithium ion batterys are a polymer based adhesive stuck to the anode and the cathode. that is why they are called lipo or li ion. the name does not refer to the external construction of the cell it refers to the cells chemistry. so lipo batterys are li ion batterys. they both use lithium ions to effect the storage and release of electrons from the polymer based medium.
```

---
## \#128 Posted by: Nath Posted at: 2017-07-25T06:19:44.480Z Reads: 78

```
and yes i have taken mine apart and yes they are 10 x 10Ah 3.7v li ion/polymer cells in series. i have built many thing with them over the years and have professional qualifcations in the area. lithium ion is a broad term. it can mean many different types of cell chemistry. it means it uses lithium ion exchange as the means of releasing stored energy. so to be clear they are not 18650s they are pouches. it is quiet obvious they are not cylinders they are flat .
```

---
## \#129 Posted by: Jinra Posted at: 2017-07-25T07:02:13.275Z Reads: 83

```
Lithium polymer has a dual meaning. The term commonly used in hobbyist equipment is for lithium packs in a polymer casing (pouch cells). The other meaning for lithium polymer batteries are batteries using a solid polymer electrolyte, which is not common place in the hobby world.

I also wouldn't say it's "obvious" it's lipo given that it can easily just be a housing for the cells.

From Battery University
> With gelled electrolyte added, what is the difference between a normal Li ion and Li ion polymer? As far as the user is concerned, lithium polymer is essentially the same as lithium-ion. Both systems use identical cathode and anode material and contain a similar amount of electrolyte.

> Li-polymer is unique in that a micro porous electrolyte replaces the traditional porous separator. Li-polymer offers slightly higher specific energy and can be made thinner than conventional Li-ion, but the manufacturing cost is said to be higher than cylindrical design. For the purpose of discussion, pouch cells are often identified as being Li-polymer.
```

---
## \#130 Posted by: Nath Posted at: 2017-07-25T08:03:57.919Z Reads: 84

```
without going into detail how every lithium ion cell works (which you could learn if you did a little research and would answer all your questions) all li ion cells have a lithium metal that is coated in a polymer based coating. then have a polymer either a polymer gel or polymer sheet sperating the anode and cathode. so. all li ions are lithium and polymer construction. there seems to be alot of confusion is this community because people are just repeating what they have heard. these forums are set up to spread knowledge. if people just keep repeating them selves and give there opinons as fact then you get confusion. if you want to help spread knowledge then please be clear if you are speculating or you know some thing to be true and be honest about how you got that knowledge. references ecetera

no lithium polymer are not pouch cells. lithium polymer batterys can be in metal cans. look at tesla batterys, look at power walls, look at every device that has a lipo battery in it. they can be pouch or can. if you want to be in a community that spreads knowledge accurate language is the first step to understanding. this is why every industry and science has a set language were words mean specific things. there is no double meaning for technical language. double meaning is a word for the arts. not science.
```

---
## \#131 Posted by: Nath Posted at: 2017-07-25T08:13:49.011Z Reads: 85

```
the reason i say it is obvious is because the battery dimensions and specs. if you do some math you can instantly know it is not cans. secondly if you have ever seen a battery comprised of pouches or cans before then it is obvious. thirdly i have the exact battery you are speaking of and i have told you its construction. hopefully this information helps you
```

---
## \#132 Posted by: OlivierDud Posted at: 2017-09-10T10:32:37.512Z Reads: 83

```
Hey guys! I’ve seen people making or buying better battery packs for their bamboo gt. Are you guys aware of anyone selling or that could make a custom pack for my carbon GT? 

Cheers.
```

---
## \#133 Posted by: BigBoyToys Posted at: 2017-09-12T07:52:13.319Z Reads: 77

```
@longhairedboy has made a few I believe.
```

---
## \#134 Posted by: longhairedboy Posted at: 2017-09-13T18:21:00.698Z Reads: 73

```
Evolve runs a BMS set up for 10S li-ion, not lifepo4. But if you can get a close enough voltage by stacking 40 or less 18650 cells in there, go for it. I wouldn't bother trying.
```

---
## \#135 Posted by: caustin Posted at: 2017-09-13T18:54:51.123Z Reads: 70

```
People do it with LG HG2 cells working OK
```

---
## \#136 Posted by: longhairedboy Posted at: 2017-09-13T19:57:27.846Z Reads: 73

```
LG HG2s, yes. I've done that. 

I've used 25Rs, 30Qs, VCT5s, HG2s, some bizarre clone of the HE2 that i've never seen before, and genuine HE2s. 

All of those were li-ion. LiFePo works on a different nominal voltage IIRC, but if you find 40 18650 cells that run at 3.6 volts you're golden.
```

---
## \#137 Posted by: Jps224psu Posted at: 2018-06-27T02:21:23.075Z Reads: 47

```
@longhairedboy hooked me up w evolve Carbon GT battery mod. Saw some people wondering about performance on this board i can tell you the stock battery blows so bad that you might as well toss it as soon as you get the board.   The samsung 30q 18650’s totally stop the sag until battery % is around 5%. Evolve software still kills it around 34v regardless. 

Lhb carbon Gt mod
100-42v
82%-37.4v (% around 65 under load rested to 82)
60%-36.4 (% around 44 under load)
28%-34.2 (% read 4 rested to 28) first switch to eco.

 9.4 miles 50/50 mix on\off rd all terrain tires...hard carving on road
```

---
## \#138 Posted by: longhairedboy Posted at: 2018-06-28T04:58:51.431Z Reads: 41

```
I keep telling people they build a solid platform then pour a shitty pack into it. It makes no sense. I really like the evolves once the battery is fixed. They're fun as hell. Fucking torquey ass racer stars on their own specially designed ESC/BMS combo, its insane. MAd respect for everything EXCEPT THOSE LOSER ASS PRISMATICS. fucking lamo pack. 

These boards are like the esk8 equivalent of the Civic CRX or the fucking Ford Fiesta. Total tuner platforms. Not bad stock, but you can easily tweak them for the better.
```

---

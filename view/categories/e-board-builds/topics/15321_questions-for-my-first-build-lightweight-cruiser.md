# Questions for my first build- Lightweight Cruiser

### Replies: 72 Views: 4093

## \#1 Posted by: dominic Posted at: 2016-12-29T04:48:41.858Z Reads: 308

```
Hi, My name is Dominic and I have been reading in this forum for awhile. I am 16 and I am in a FRC robotics team. Also working a project car (MGA 1600). But all of that is irrelevant. 

I have some questions for my first build. I am trying to make a lightweight cruiser that I can quickly take me a mile or two here and there when I miss the bus. I weigh less than 115 pounds so weight isn't an issue. I also want to have a mixture of speed and torque, which is why I chose to run the motor at 8s instead of the usual 6s (I can gear down). I used Solidworks to CAD a motor mount. I know there are a lot out here I just like the pride of designing it yourself.

Parts of my build (some stuff I have already):
-custom 29in cruiser that I made + hardware (have already)
-Caliber Trucks 50 degree baseplate + riser pads (have already)
-Abec 11 76mm flywheels + bearings (have already)
-36T HTD 5mm pulley + pulley itself (have already)
-SK3 280KV (have already)
- RC 2.4 GHZ controller (like gt2b but from a Tacon RC car)
-Custom mount that I designed: (plan to mill)  https://grabcad.com/library/dominic-s-electric-skateboard-caliber-motor-mount-1
-HTD 5mm 16T (plan to buy)
-vesc (plan to buy)
-26650 8s1p battery (plan to make)

I have some questions:
1. Does my mount look good? I wanted everything to use locknuts cause why have it adjustable when you have to Loctite it?
2. Does 36:16 sound good? I have some moderate hills that I need to climb but I am not looking to use this as my entire commute, maybe a last mile kind of tool.
3. I want to use the vesc but I am scared that I am going to break it. I have some experience with electronics but after reading about the vesc on these forums I am worried I will waste my money by destroying it.
4. How will the 8s1p battery work? I want to get maybe 4-5 miles of ride distance but not too worried about that, wanna have it be really light. I also want to use sleds for this so I can change out the batteries if they are not working so well. What battery is best? Sleds? https://www.fasttech.com/products/3023/10018241/3827705 Also, what kind of wire to wire it up? Best BMS? 
5. Suggestions for enclosures? I might be able to 3d print a single piece cause my battery is really small, idk.

I appreciate all the help. I will be posting updates and further questions in this post so I wont be obnoxious by making new forums for the same topic.
```

---
## \#2 Posted by: JLabs Posted at: 2016-12-29T05:05:40.535Z Reads: 283

```
16 to 36 gear ratio will suit you just fine. From what I know 26 650 cells have a lower nominal voltage, so an 8s battery will be more like 7s or 6s (correct me if I'm wrong). batterysupports.com is the best place to get a BMS in the states, but I think they're having some pain issues at the moment. You can either spot while the pack with pure nickel strip or solder it with pure copper wire, but do not use sell holders because the tabs cannot handle the amount of current going through them. They are also not secure for the bumps when riding. A 3D printed enclosure is very possible  if your battery is small. I find mine works great because I customize everything on it. I would not be afraid to use the VESC. You can just post all of your specs before you ride and have an expert check it on here.
```

---
## \#3 Posted by: saul Posted at: 2016-12-29T05:20:00.942Z Reads: 276

```
[quote="JLabs, post:2, topic:15321"]
26 650 cells have a lower nominal voltage
[/quote]

This is based on cell chemistry not the size. 
a123 cells use LiFe are 3.3 nom 3.6V full
li ion/lipo use LiMn (i think) 3.7 nom 4.2 full.

if they are liion like basen 26650 the motor might be a bit high kv. but since you are light, its not problem just limit max erpm on the vesc. 

Also those battery holder **can not handle the current**, especially in a 1p pack. You need to spot weld, or solder.

I just did a post about range, with a simple calculator to estimate based on battery.
[Esk8 Range Calculator](http://esk8.today/2016/12/28/how-far-can-i-ride/#rc)
```

---
## \#4 Posted by: dominic Posted at: 2017-01-01T23:26:07.688Z Reads: 237

```
Ok, getting basen 26650 for 8s1p with a 60amp bms. Also getting switch from diyelectricskateboards.com. Problem is that i need something that can supply 32 volts to the bms so I can charge. All options that I found were super expensive for so little amps, and it would take 1/3 or the day to charge. Anyone know places to get cheap power supplys for 8s1p 26650 basen batteries? 

Also, will 10 awg wire be sufficient for soldering the batteries together?
```

---
## \#5 Posted by: IDVert3X Posted at: 2017-01-02T09:43:47.772Z Reads: 210

```
Basen 26650 are overrated. They are 20~25A continuous.
Better go with A123 cells.
```

---
## \#6 Posted by: dominic Posted at: 2017-01-02T17:16:56.455Z Reads: 206

```
Oh, shoot. Already bought the basens. I could just limit the amps with the vesc for protection, right?
```

---
## \#7 Posted by: IDVert3X Posted at: 2017-01-02T17:39:21.779Z Reads: 196

```
Yes, you can set 20A battery limit, but the voltage will still sag a lot in a 1P pack.
Basen cells are good if used 3 in parallel or more.
Only A123 cells or LiPos can do 1P.
```

---
## \#8 Posted by: SirDiff Posted at: 2017-01-02T18:08:49.660Z Reads: 185

```
What about limiting the damage done buying 8 more cells and making 8s2p? 40A should be enough, space cell is rated for that. It will weigh a bit more but should still be acceptable
```

---
## \#9 Posted by: dominic Posted at: 2017-01-02T20:49:30.737Z Reads: 184

```
Can i return the basen batteries from liionwholesale.com. I dont think they shipped yet. They  advertised that the battery could do 30 amps continuous? Why do i need to limit them to 20 amps if they can supposedly do 30 amps? Im still kind of confused on what voltage sag is. I am assuming its like our robot when too many motors run at once, it makes everything slightly slower?
```

---
## \#10 Posted by: IDVert3X Posted at: 2017-01-02T21:10:05.191Z Reads: 181

```
They can do 25A continueous from the tests.
But if you draw 25A, voltage will drop.
Ideally, you want to draw < 10A from the cell.
That's why guys there make 4P packs of 20A cells and use 40A fuses / BMS instead of 80.
Even this sometimes is still not enough.

Back to the voltage drop ( sag ).
Less voltage = less POWEERRRRRRRRR.
Now, seriously, in the end, you may end up not beign able to climb a steep hill and so on.
Also, the battery will wear quickly and get quite hot.

Why hot?
Because V ( drop ) = I * Ri
Every single cell has it's internal resistance.
Imagine it as a resistor connected in series with the cell.
Higher current = higher voltage drop. Energy won't disappear. It transfers into heat.
```

---
## \#11 Posted by: dominic Posted at: 2017-01-02T21:19:50.394Z Reads: 162

```
Option 1: I limit the amps from the battery to 25, i get less heat but more voltage sag. 
Option 2: I limit the amps from the battery to 30, i get more heat and less voltage sag.

Am i doing this right?
v=ir
and the resistance is constant so the voltage is proportional to the amps?

Thanks for clarifying for me, I really appreciate it cause I just started physics his semester. Im taking  AP physics 1&2, and we haven't got to the 2 (electricity and magnetism) stuff yet.
```

---
## \#12 Posted by: IDVert3X Posted at: 2017-01-02T21:45:21.687Z Reads: 162

```
Heat is directly proportional to the voltage drop.
Voltage drop = heat.
More current => higher voltage drop => more heat.
Internal resistance is constant.

And yes, V = I*R.
In this case, we are calculating the voltage drop itself.
R = const, higher I = higher V ( voltagr drop ) = more heat.

With 1P pack, you ideally want to set your current limit to 15A.
```

---
## \#13 Posted by: PXSS Posted at: 2017-01-02T22:16:52.182Z Reads: 151

```
More current/cell equals:
-More voltage sag (bad)
-More heat (bad)
-Less range (bad)
-Lower life cycles (bad)
-Lower max power (bad)

I cant actually find any discharge curves for these cells so I can't tell you how much is too much. 

@IDVert3X, can you post some please if you know where to find them.

Either way, I recommend you either get a different cell or double your cell count.
```

---
## \#14 Posted by: PXSS Posted at: 2017-01-02T22:19:14.140Z Reads: 145

```
[quote="IDVert3X, post:12, topic:15321, full:true"]
Heat is directly proportional to the voltage drop.
Voltage drop = heat.
[/quote]

Wrong.
P = V^2/R. 
Or
P= I^2*R
P = Heat in watts

V=I*R in purely electrical systems. Batteries are not electrical systems. They are electrochemical systems, way more complex. Their internal resistance varies with temperature, state of charge, state of health, current draw, etc. This is why you want to rely on discharge curves and not V=IR
```

---
## \#15 Posted by: IDVert3X Posted at: 2017-01-02T22:22:29.584Z Reads: 150

```
Correct. Both are correct.
You just written the complete formula.
From my formula, you get the voltage drop.
And it is directly proportional to heat as higher drop = more heat.
If you want the amount of heat in watts, you have to multiply it by current.
And yes, that's when I^2*Ri comes in place.
Or step by step:

V(drop) = I * Ri [ Volts ]
U = V(drop) * I [ Watts ]
Which is equal to I * Ri * I which is equal to I^2*Ri.

This is all I have for the Basen discharge curves.
https://www.e-cigarette-forum.com/forum/attachments/image-jpg.523780/

Drops are ridiculous.
```

---
## \#16 Posted by: PXSS Posted at: 2017-01-02T22:29:56.298Z Reads: 142

```
That is not what directly proportional means... 
Directly proportional would be
P= c*V(drop)
Where c is some constant...
Heat increases with voltage drop squared.

E: Read my edit above for the V=IR part of your comment...

Those curves are useless. They are with respect to time and not capacity, plus they are also resting the cell between draws. Very different from our application.

E2: You don't learn this stuff in physics. You have to get to the Electrical engineering/ Chemical engineering courses to fully understand it
```

---
## \#17 Posted by: IDVert3X Posted at: 2017-01-02T22:46:18.681Z Reads: 151

```
Well, I was taugh that directly proportional means when something increases by certain amount, something else increases too.

In my language, its called "priama úmera" which google translated as directly proportional.

And if voltage drop increases, watts increases too.
Basically P=V(drop)*I and if drop is not directly proportional with heat ( watts ), how do you call it in english?
```

---
## \#19 Posted by: PXSS Posted at: 2017-01-02T23:22:41.364Z Reads: 149

```
Directly proportional is this equation by definition.
I'm pretty sure that's a math thing not a language thing, but I dont know. 
X=cY where c is a constant.
This is wrong because
P=IV and I is NOT a constant. 

This is the correct way to say it power is directly proportional to voltage squared.
P = (1/R) * V^2 where 1/R is a constant
```

---
## \#20 Posted by: dominic Posted at: 2017-01-02T23:23:24.780Z Reads: 146

```
My whole topic deleted? Or someones comment? I kinda need this so i dont mess up anything.
```

---
## \#21 Posted by: PXSS Posted at: 2017-01-02T23:23:51.886Z Reads: 143

```
He deleted his comment. Not thread.
```

---
## \#22 Posted by: dominic Posted at: 2017-01-02T23:25:44.853Z Reads: 122

```
ok, thanks. What kind of heat would I expect with vesc limiting amps to 25 from battery that is 8s1p with basen cells. Would a battery heatsink solve any issues? Does vesc heat up from limiting amps? Dont wanna destroy it.
```

---
## \#23 Posted by: PXSS Posted at: 2017-01-02T23:32:53.395Z Reads: 129

```
Dont know. But the heat isn't your main problem. 
I do not think your board will have enough power to climb any hills without your esc hitting the low voltage limit. 
If you draw too much power you can sag your cells to 20V and your esc would shut power down, depending on the discharge curve, this could happen at 50% capacity like it happens to one of the other guys here or worse.
```

---
## \#24 Posted by: dominic Posted at: 2017-01-02T23:40:59.681Z Reads: 132

```
@scrant made a 10s1p build that seems to be working great for him. Its the same cells and i dont think he gets any voltage sag. Does the 8s vs 10s make a big difference with 2 extra cells... its the same parallel, 4500mah, 30 amps.
```

---
## \#25 Posted by: Ackmaniac Posted at: 2017-01-02T23:45:30.642Z Reads: 141

```
I deleted my comment because I thought we are in a different thread and talk about a 10S4P pack. With a 1P li-ion pack you push the limits I guess. But for a cruiser it should be doable. But more cells would be better. If you want to go for 26650 cells then I can recommend some cells which are realy cheap and perform great.

In the endless sphere forum they are very surprised how good the cells are. For example they ae rated at 5000 mah but by tests they mostly reach 5400 mah. And the discharge curves are normal. If you would have them in a 10S2P then it should be fine for any cruising.
http://www.gearbest.com/batteries/pp_360842.html
```

---
## \#26 Posted by: PXSS Posted at: 2017-01-03T00:10:06.116Z Reads: 131

```
2 extra cells in this case is 20% more power so maybe?
```

---
## \#27 Posted by: willpark16 Posted at: 2017-01-03T06:50:37.541Z Reads: 137

```
He most likely does sag but doesn't care/doesn't notice, Sag is something that develops over time ur pack will be ok for a week maybe more but after a while it will fail on you and ur cells will be all over the place, I get what a 16 year old mind like ur own understands and basically it's like this the more cells you have, the more current( which is the power for ur board)the more heat you have, you want less current distributed amongst ur cells during load, so get more cells with lower internal resistance id highly recommend a 10s 3p he4 pack because resistance wise he4 are better than 25r
```

---
## \#28 Posted by: dominic Posted at: 2017-01-03T06:56:17.048Z Reads: 140

```
Ok, i am ordering some more cells to make a 2p pack. Hopefully it solves the issues ,and according to a calculator I can get about 15 miles of range that I probably wont need!!!! In a more serious note i need a charger for my 8s 60 amp bms. I need 32 volts i think, and i prefer 2-4 amps to charge quickly. I cant find any that are reasonably priced, if you guys know where to get a cheap good one let me know. Links pls!!!
```

---
## \#29 Posted by: willpark16 Posted at: 2017-01-03T07:22:16.280Z Reads: 132

```
2p is still voltage sag
```

---
## \#30 Posted by: PXSS Posted at: 2017-01-03T15:14:47.753Z Reads: 135

```
2P is fine for a cruiser.
```

---
## \#31 Posted by: okp Posted at: 2017-01-03T15:34:44.689Z Reads: 135

```
great build; I'm also looking to build a cruiser; will go with 12S2P / 190kv / 15/32T / Bustin Bonsai deck (29')
```

---
## \#32 Posted by: dominic Posted at: 2017-01-14T16:36:16.580Z Reads: 137

```
So all the supplies for the batteries came in. 8s2p basen 26650. Any tips for soldering? I plan on tinning both the battery and the wire and then melting the two together also going to use flux. I got a 60 amp bms from battery supports i think, but i still need the charger. Will this charger work for my battery configuration? 
http://www.ebay.com/itm/8S-28-8V-29-6V-Li-ion-Li-Po-Battery-Intelligent-Smart-33-6V-2A-Charger-for-US/221896637604?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D40757%26meid%3Dba2db937eae549b69b7158b94148bf58%26pid%3D100005%26rk%3D2%26rkt%3D6%26sd%3D321471399664
```

---
## \#33 Posted by: Lucas123 Posted at: 2017-01-14T17:02:58.874Z Reads: 130

```
hi I've recently received the parts for my first build to realize that my space cell pro 3 had an xt60 connector and I was wondering which one is better, xt90 or xt60?
```

---
## \#34 Posted by: saul Posted at: 2017-01-15T00:21:31.034Z Reads: 129

```
xt60 is fine for space cell because the low amps..

xt90 can do more continous current but they are a pain to disconnect and take up more space...
```

---
## \#35 Posted by: dominic Posted at: 2017-01-23T00:33:00.070Z Reads: 126

```
Ok, before i purchase the charger from my last reply, I have a few questions. The basen batteries have a nominal voltage of 3.7. Does that mean stop charging at 3.7? The charger I am planning to get charges to 33.6 (for 8s2p) which equates to fully charged at 4.2 volts per cell. Is this ok for my cells? I want to purchase tonight or asap. Im really excited to start making my battery! @saul could you answer this question for me? You seem the most experienced person that has responded to me so far regarding my batteries.

Edit: Did some digging and I am positive i can charge each cell to 4.2 volts which is why the charger voltage was higher than nominal. I went and bought the charger...
```

---
## \#36 Posted by: saul Posted at: 2017-01-28T03:09:20.897Z Reads: 118

```
looks like you found your answer already, but yea nominal in this case means average V. li-ion range from about 3V empty to 4.2 full. 3.7V about where the battery stays for most of the discharge cycle so its used for most calculations like pack capacity.

let me know how that charger works, my 8s 10ah lipo pack needs a faster charger! :thinking:
```

---
## \#37 Posted by: Okami Posted at: 2017-01-28T08:08:41.978Z Reads: 119

```
You can charge to 4.2v.. though, if you are interested in longer cycle life.. it is said that it is best to charge till 4.1v.. or maybe even 4.05.. middle ground is 4.15v.. 

My balance charger charges li-ions to 4.1v as default.. I think it is also related with that, there is a bit tighter tolerance for li-ions and their max charge..

Though, if you are after 200-400mah extra for each cell (dont know your case).. then charging till 4.2v is totally fine :) Happy e-riding once you get everything set up
```

---
## \#38 Posted by: will_manners Posted at: 2017-01-28T10:07:29.160Z Reads: 121

```
I'd forget about trying to "prolong" the life of your Li-ions by setting a lower charging cutoff voltage.

Li-ions will degrade over time quicker than they will degrade due to charging to their specified voltage. Even in a worst case scenario a cell specified with 500 cycles equates to around 5000km of riding (that's only at 10km per cycle). Most riders won't get anywhere near that mileage and thus the battery degrades over time quicker than the user over cycles the cell. 

Setting a lower charge voltage is like filling your tank up only half full in order to get better mileage due to the decrease in weight. You may theoretically get better fuel efficiency, but the decrease in range is hardly worth it.

The only scenario where it might be a good idea is if you know that your charger over charges the cells above 4.2v. But even in that case you may as well throw out the charger and buy one that is more accurate with its cutoff voltage.
```

---
## \#39 Posted by: Okami Posted at: 2017-01-28T12:49:05.439Z Reads: 111

```
That is a somewhat good point! I have not got till 2-3yrs of age for my battery so cannot tell anything from personal experience yet.. 

So I would agree - if  board / battery is used only occassionaly, then go after higher capacity.. 

On the other hand it looks like ppl who have better weather and uses their batteries a lot can wear down (at least lipos) a lot faster. Depends on applicationi think
```

---
## \#40 Posted by: dominic Posted at: 2017-01-29T06:22:55.715Z Reads: 110

```
Thanks for all the responces! I was practicing my soldering on some dead double A's the other day in preparation for soldering my basens. So far i have found that scuffing up the surface and a tiny bit of flux has been working well for me. I prep the batteries with the scuff and flux and then put a glob of solder on my iron and lower it onto the battery and spread it out quickly. Then i let the battery cool off a little and then remelt the solder and attach the solid gauge wire. Just have been practicing with 22 guage and AA batteries, wondering if this technique will work with basens and copper welding rod? Heard some people say that rod is easier to solder. How long should the molten solder / iron be in contact with the battery, i got my technique down to 2 seconds...
```

---
## \#41 Posted by: willpark16 Posted at: 2017-01-29T08:51:39.651Z Reads: 108

```
Not my experience with copper rod it requires lots more heat than wire in my opinion
```

---
## \#42 Posted by: dominic Posted at: 2017-01-29T21:22:54.240Z Reads: 97

```
What kind of wire do you use? I tried 10 gauge but it was too big / bulky to solder... When i finally got a decent joint i could easily pull it off...
```

---
## \#43 Posted by: willpark16 Posted at: 2017-01-29T21:36:11.390Z Reads: 98

```
12awg high strand
```

---
## \#44 Posted by: dominic Posted at: 2017-03-15T20:28:46.114Z Reads: 93

```
Still deciding between soldering vs DIY spot welder. I learned how they work in AP physics and I am not scared of using them because i know how they work. (we completely destroyed a soda can in class). I have a spare microwave i can rip the transformer out of. Do i need to have an arduino time each weld, or can i just hold it down for a fraction of a second? Also what is the best nickel strip to use. And should I get / 3D print cell holders or will hot glue work fine (im scared of it melting) or another type of glue (heat resistant)?
```

---
## \#45 Posted by: willpark16 Posted at: 2017-03-16T00:46:54.172Z Reads: 90

```
I wouldn't recommend this without a bit more research also soldering can be just as easy took me 30 mins-1hr for a 10s3p
```

---
## \#46 Posted by: PXSS Posted at: 2017-03-17T13:12:40.982Z Reads: 101

```
I had forgotten about this thread until it popped back up on my feed today.

If you do not intend on using a full charge in a single ride or in a day then I suggest you do not charge your battery to 4.2V.
@will_manners is wrong, Li-ions can last almost twice as many cycles if you don't charge them to 4.2V or discharge down to 2.5V. It's how the chemistry works. The analogy is also wrong, it's nothing like filling your tank half way in order to get better efficiency... how is 3lbs of less gas going to matter in your 4000lbs car for a regular sedan?

Charging your cells to 4.1V and not fully discharging your cells can easily increase your life cycle from 250-300 cycles to over 500 cycles. Cell don't degrade over time just because if you keep your cells at the proper voltage which is the whole point of not fully charging and discharging.

If you dont see yourself using more than 80% of the full capacity a day, I recommend charging to 4.1V and setting your low cutoff voltages to 3.0V for start and 2.8V for end.

---

About the soldering on cells,
get yourself some 12ga flat copper braid. If you're in the US, you can source it through mcmaster.
I personally spot weld my batteries but I also have all the equipment to do so already. If you can afford the equipment and are going to make more than a single pack then by all means, get a spot welder.
If not, keep practicing your soldering on AA with copper flat braid and post some pictures, we can tell you if your soldering is good or bad, and how to improve it.

You're headed in the right path!
```

---
## \#47 Posted by: Maxid Posted at: 2017-03-17T13:44:04.500Z Reads: 88

```
Saw @will_manners' post also just now - that analogy is so off...
Charging to 4.1V is nothing like filling your tank only half way. 
You "lose" maybe ~3% capacity - not half of it.
```

---
## \#48 Posted by: will_manners Posted at: 2017-03-18T03:46:34.266Z Reads: 82

```
@Maxid @PXSS 

The analogy was not meant to represent a real situation in quantitative terms...

Obviously charging to 4.1v won't decrease capacity by 50%, but it will reduce capacity by a tangible amount. Where are you getting the information from that not charging to their full capacity doubles their life-cycle? That sounds utterly absurd. True you may only lose 5% of capacity by not charging to 4.2V, but in a 10S4P configuration that extra 5% equates to an additional 20W/hr, which is potentially an extra 2km that you could travel. The chemistry is designed to be charged to 4.2V.

If you can prove to me that only charging to 4.1V **doubles** a cells life cycle (which is what you are suggesting) then I will agree that is a worthwhile compromise. As an example don't you think that smartphone manufacturers would be taking advantage of this "huge" life cycle boost by setting parameters that prevents them being fully charged? But they don't obviously, because the increase in capacity provides a real world benefit which is far outweighed by the possible increase in cell lifespan.
```

---
## \#49 Posted by: Maxid Posted at: 2017-03-18T05:03:20.521Z Reads: 82

```
"Table 4: Discharge cycles and capacity as a function of charge voltage limit. Every 0.10V drop below 4.20V/cell doubles the cycle but holds less capacity. "
http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries

Just one of many google hits.

The information with 3% capacity comes from looking at this
http://lygte-info.dk/review/batteries2012/Samsung%20INR18650-30Q%203000mAh%20%28Pink%29%20UK.html at the lowest discharge rate.
```

---
## \#50 Posted by: PXSS Posted at: 2017-03-18T14:27:33.053Z Reads: 86

```
@will_manners 
Look up spec sheets for batteries. Also that link from battery university that @Maxid posted, it has hours and hours of research and citations you can read. They just combine it and put it nicely in tables for you.

And smartphone manufacturers don't care about longevity. If you have to replace your battery in two years, so what? Guess who's getting to do the service on your phone and making a profit??? Besides, no smartphone is meant to last more than 2 years. Oh and how many times do you actually let your phone die before charging it? Do you always let it go down to zero and then charge all the way to 100?

Electric car manufacturers on the other, do care about the longevity as they lose consumers if the $15k battery has to be replaced every few years. 
Here's an excerpt from the article linked below. 

---

http://blog.evandmore.com/lets-talk-about-the-panasonic-ncr18650b/

"_Now let’s look at the cycling chart. (Cycle Life characteristics)_

_To estimate the number of cycles that the cell can undergo in its lifetime, we charge it at a maximal current of 0,5C and discharge at a current of 1C at 25 degrees Celsius and then we count the number of charge/discharge cycles until the cell degrades down to 70% of its initial capacity (2250mAh). In the case of these cells, the number is about 500 cycles._
_500 cycles? But that’s (relatively) low! Yes. But what is not shown on the spec sheet is that when you partially charge and discharge, degradation of the battery capacity is reduced. Thus, you can do over 40 000 charge/discharge cycles when going from 30% to 70% only. Or over 35 000 charge/discharge cycles from 20% to 80%; 28 000 cycles from 10% to 90%; 15 000 cycles from 8% to 92%, 7500 cylces from 6% to 94%, and the capacity reduction goes faster and faster, finally reaching 500 cycles when recharging from 0% to 100%._

_This explains the partial cycling strategies implemented by car manufacturers: GM limits the cycle from 17% to 80% of energy storage levels for the Volt. Nissan limits maximum charge level of the LEAF to 90% (4,15V). Tesla invites owners to limit the maximum load to 90%, and recommends avoiding deep depletion of the battery pack. All these strategies work well and significantly increase the number of battery cycles. When I manage the power levels of my own Tesla, I try to keep my maximum load below 90% and avoid depleting below 20%. Following this practice since the purchase of my Tesla, I have seen no capacity degradation. My wife’s 2012 Volt shows no degradation either. In fact, no Volt has yet shown degradation below 70% of the initial capacity which would have resulted in a warranty claim. In conclusion, we can trust the reliability of our Lithium batteries!"_

---

This is my daytime job. Trust me. I'm right.
It wasn't the fact that your analogy was meant to represent it in quantitative terms, it's the fact that your analogy didn't make sense.  Filling your tank to 50% in order to save 3lbs on a car that weighs 4000lbs to get better fuel efficiency is so wrong I don't even know how you came up with the idea... lol
It's something I can see one of my exes doing though
```

---
## \#51 Posted by: dominic Posted at: 2017-03-27T15:52:08.744Z Reads: 81

```
Probably going to solder cause I dont have plans for using a transformer to make a spot welder. If i have 2 columns of 26650 cells with the long ends touching, what kind of heat shrink do i need to connect the columns together, and then the entire thing together. 

Also bought 3 vescs from @chaka. (for me and 2 friends) Hopefully they come in soon, but im not sure when?

My main mount plate is water jetted (put it in the same order as robotics team parts). But i still need to mill the clamp for the truck. 

How would I know when to stop charging? Should I buy a voltage meter thing to wire in series where my vesc is (after the on/ off switch)? I dont trust those % meter ones, I'd rather have the raw values. 

Hopefully I finish in the next few days! I want to bring it to a robotics competition in silicon valley so i can ride around during my free time and get food!

Links for Heatshrink tubing for my specific pack size?
Links for simple voltmeter?
```

---
## \#52 Posted by: trampalovesshekels Posted at: 2017-03-29T22:08:57.113Z Reads: 73

```
go for 18650's, if you stack them diagonally you can fit a  4p pack for example it will be better(instead of 2p 26650), if you want to go exotic battery this is not it.

I have tesla cells from a p90d I sell 4, I am on the other side of sf
```

---
## \#53 Posted by: dominic Posted at: 2017-04-05T06:47:58.160Z Reads: 66

```
i already bought the batteries awhile ago, I was planning on making an 8s1p but soon figured that wouldn't be enough. So i bought 8 more cells to make 8s2p.
```

---
## \#54 Posted by: willpark16 Posted at: 2017-04-05T06:50:58.686Z Reads: 66

```
That's gonna be heavy voltage sag after a bit
```

---
## \#55 Posted by: dominic Posted at: 2017-04-05T06:53:46.875Z Reads: 66

```
we already had this conversation above but i weigh only 115 pounds. Board should be able to handle it?
```

---
## \#56 Posted by: trampalovesshekels Posted at: 2017-04-05T06:54:40.033Z Reads: 66

```
mashallah, you should start going to to mosque and pray almighty allah for the voltage sag my frien
```

---
## \#57 Posted by: willpark16 Posted at: 2017-04-05T06:55:22.778Z Reads: 68

```
Not really will still have sag it's mainly because of the cell itself not being meant for esk8, it won't mean u can't ride but it will deplete cell life from overextending cell capabilities or when u wanna go up a hill
```

---
## \#58 Posted by: dominic Posted at: 2017-04-05T07:00:52.154Z Reads: 67

```
Math? How many amps will i be pulling up hill or while accelerating? I see some people on this forum who use reused batteries or even a 2p pack with 18650. And that works fine for them? Boosted uses 12s1p 26650 A123 cells which works fine for them?
```

---
## \#59 Posted by: willpark16 Posted at: 2017-04-05T07:01:42.770Z Reads: 65

```
As in estimated? If ur riding flats the setup is fine, it's a first build so stick to what u uave
```

---
## \#60 Posted by: willpark16 Posted at: 2017-04-05T07:02:56.546Z Reads: 65

```
A123 have 70a cont discharge also It will work but over time you and all thiseb10s2p users will feel the effects of voltage sag
```

---
## \#61 Posted by: dominic Posted at: 2017-04-05T07:04:43.965Z Reads: 64

```
sure, estimations work. Max continuous discharge of basen 26650 is "40amps" but someone said that was fake. A123 26650 max continuous discharge is "50 amps." (also probably fake) If boosted can do a 12s1p with a123 cells, why wont 8s2p work with basen cells?
```

---
## \#62 Posted by: willpark16 Posted at: 2017-04-05T07:06:00.045Z Reads: 61

```
Different chemistry and a123 actually really  do discharge 70a if say you can pull about 20a up a 15-20% incline maybe more
TBH the effects for some are minimal but a bms or voltage alarm is definitely necessary with these
```

---
## \#63 Posted by: dominic Posted at: 2017-04-05T07:09:40.577Z Reads: 66

```
i bought an 8s 60 amp bms from battery supports. i plan on charging and discharging from it. Unless someone recommends otherwise.
```

---
## \#64 Posted by: willpark16 Posted at: 2017-04-05T07:10:05.386Z Reads: 65

```
Great Ull be fine then
```

---
## \#65 Posted by: dominic Posted at: 2017-04-05T07:10:32.371Z Reads: 67

```
awesome, thanks for the help
```

---
## \#66 Posted by: willpark16 Posted at: 2017-04-05T07:10:57.438Z Reads: 68

```
Yep no problem keep posting updates
```

---
## \#67 Posted by: PXSS Posted at: 2017-04-07T11:47:43.918Z Reads: 60

```
@willpark16 and @trampalovesshekels
Its a cruiser board not a speed or torque demon. 
He'll be more than fine with the 8S2P as long as he rides easy and isn't bombing uphill.
```

---
## \#68 Posted by: jmasta Posted at: 2017-04-07T15:18:55.949Z Reads: 57

```
Didn't read through your thread, but I took a look at your motor mount in the first post 

If you can, I'd recommend doing away with the rotating slots on the motor plate to the clamp. I did the same thing with my design, and nothing I do can seem to stop it from slowly rotating back toward the ground.  Red loctite + specialized washers is still not good enough 

You could likely achieve a similar adjustability with a hole pattern instead of the slots. I wish I had 3D-printed my design first to figure out the desired angle... and then milled the plate without the circular slots

PS.  If you stick with the slots, make sure you design it so that even if the rotating mount fails, your motor can't hit the ground. Less adjustability is better here
```

---
## \#69 Posted by: dominic Posted at: 2017-04-07T17:09:44.044Z Reads: 56

```
I redesigned my mount but i still have yet to upload it to grabcad. The one on grabcad right now is bad, has wrong measurements. It was a semi quick fix in solidworks. I just waterjetted the mount and polished it! Circle clamp thing still needs to be milled, when i get the chance... so far, it looks good! I love the feeling of knowing you made and designed something yourself!
```

---
## \#70 Posted by: will_manners Posted at: 2017-04-26T05:59:44.388Z Reads: 52

```
Honestly I'd long forgotten about this thread but here we are again. Thank you for the links @Maxid and @PXSS. I have of course already come across battery university many times but have only just seen that specific article a few days ago. I am surprised about the results so I'll admit I did not know that setting a lower cut-off voltage would make such a difference to life-cycles. 

The interesting thing to note is that the tests are prefaced by the fact that the data tables do not address "ultra-fast charging and high load discharges", the latter of which is certainly relevant to our applications. Nor does it address the fact that there are different chemistry's which aren't included in the tests (the Samsung 25R being NCA). I would be curious to know how both those two factors affect the data regarding life-cycles and by how much.

@dominic Any updates? :) Did you still end up going with 8S2P with the Basen cells?
```

---
## \#71 Posted by: Okami Posted at: 2017-04-26T10:40:37.571Z Reads: 55

```
@will_manners so do you discharge your batteries at its maximum rating all the time?

I think then your ''battery design'' is a bit off, since people strictly stick to 30% use of max battery discharge here, I think :D

Batteries start to degrade with high temperatures.. and I believe only with proper methods of measuring the internal temp someone can adress this issue - whenever at his discharge levels batteries get hotter than they should be..

--

For example, Im not sure how many people here constantly draw 50-60A out of their battery packs when going on flat and using a longboard.. for me, that amount of constant power is a bit ridiculous but I can justify it, if they travel at 50-60kph of speed all the time.. then it might be somewhat close to this amount, if not even more..

What im trying to tell here is this - most of us (at least many) are a bit sissy about batteries :D but maybe it is good we are that way and that we dont abuse them hardly, otherwise they would start to fail pre-maturely (abusing in a way - like discharging below the limit a couple of dozen times)...

 So, back to original topic - at 1C-2C discharge the batteries should be fine, with chemisty 18650 cells use. I believe NMC chemistry might ''act'' a bit different, since its higher output ratings.. but that is a bit different story and I just want to point out that not all of use push up hard up hills all the time to see maximum demand.. or use chinese underspeced boards with only 1 cell group in Paralell.. (1P systems)

So back to the topic, at 10s (36v) and let''s say 3P pack of 2.5ah cells, it should be safe to discharge 7.5 - 15A out of the pack probably (1-2c). That is without stepping into 3C zone.

So, for 10s system, these 7.5 - 15A would ''yield'' about: 270 - 540W. 
For lower ''pressure'' on the cells, a 4P probably might be recommended if someone wants to regularly take 1000w out of the batteries.

--
Some temp data about HG (20A) cell:

<img src="/uploads/db1493/original/3X/4/e/4e3720cfaea2e8d1a6da877763388fbf11286591.png" width="690" height="214">

Source: https://www.e-cigarette-forum.com/forum/threads/vrk-20a-3000mah-18650-bench-test-results-accurately-rated-looks-like-hg2.758835/

So I might actually say that it is possible to ''push'' till about 4C without problems, but as always, the less load, less stress/heat probably.

--
20A discharge for high power cells and their temps:

https://www.e-cigarette-forum.com/forum/attachments/image-jpeg.584749/

--

From the same source @PXSS gave info from:

<img src="/uploads/db1493/original/3X/b/f/bfa1eb8e7b59ae1adb8637c3bc54950bfedd84bd.png" width="690" height="121">

@will_manners for specific effect on temperature / heat impact on battery cycle life you probably gonna need a different source.. but for now, I think, all you need to know is that in order to increase the life of batteries, just design a battery which you wont use at maximum.. basically doing a 2P system for 10S is probably just fine in most cases.. opposed to chinese practice of 1P packs and ''super range'' of 3-4km or something.
```

---
## \#72 Posted by: will_manners Posted at: 2017-04-27T03:53:07.094Z Reads: 52

```
Some good points Austris. Internal temperature sensors on the battery pack would indeed be quite beneficial, although many have said that those kind of safety measures are overkill. A few problems I can see with this is the temperature sensor may only be located at one point on the battery pack. Meaning it only has one point of reference to measure temperature, more often than not a battery pack may fail because of one bad cell, as opposed to the entire battery pack progressively overheating due to stress. The problem therein lies that the temp sensor only covers a very small area and not each individual cell (perhaps there are methods to get around that).

In terms of the temperature data you linked for the HG2, that particular cell has been shown to rise in temperature by a greater degree compared to similarly spec'ed cells under the same load. HJK noted the same thing with temperatures rising above 90 degrees C. The graphs show that the HG2 reaches 81°C at 20A and the 30Q reaches 75°C at 20A. 

<img src="/uploads/db1493/original/3X/2/2/228059784cfd049c80b3f47991706e0e7ac4cc71.PNG" width="690" height="392">

<img src="/uploads/db1493/original/3X/b/a/ba81545410b765c8a3ea3192191eab60b35b8832.PNG" width="690" height="378">

I guess the take away from this as you've mentioned is that these cells will get hot under high loads, so we should design our battery systems and drive-trains around maximising efficiency and minimising high amp draw.
```

---
## \#73 Posted by: dominic Posted at: 2018-07-31T21:28:22.335Z Reads: 21

```
Hello all. I finally finished my board. I think the gearing was geared too high so it takes a few good pushes to get up to speed. Also it can not climb any sort of hills, literally none. Recently, my board started spazzing out, as the motor can not handle any sort of load. Even when I try to do a motor detection the motor sort of wobbles back and forth. Attached are the vesc settings, let me know how I can get more power out of my setup. Much Appreciated, Dominic.![38177097_1886836994956958_2995275965636018176_n|498x280](upload://306y22kJ0EebnT5br2mwQDWnENN.png)![38018077_1886837528290238_2303481120798277632_n|498x280](upload://cMYbLgwMH63XALOavp8De1oRRgm.png)![38197364_1886836371623687_6100535821700431872_n|474x280](upload://9WrWzw8oCGIMIlibQasIMJeRWch.png)![38151532_1886838721623452_5578528511611633664_n|498x280](upload://qW4xu2Ps8EWdpOf4IvyPWZh9Uag.png)![IMG_1666|375x500](upload://32psqk8WcceqKtuP2coVXv397zz.jpg)![IMG_1667|666x500](upload://8pz8yE78U7hKVyFX3rbs6zYzUK2.jpg)![IMG_1668|666x500](upload://kD1sULG2ZeBzYCpQj6ctrvoDiDL.jpg)![IMG_1670|666x500](upload://46LXyDFCV84VzJjXHfwgJo1dLSN.jpg)![IMG_1669|666x500](upload://oNfmEf6RwgsMH1cuJeGeBsnklhd.jpg)
```

---

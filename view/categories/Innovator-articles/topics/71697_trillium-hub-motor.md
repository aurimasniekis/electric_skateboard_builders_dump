# Trillium Hub Motor

### Replies: 85 Views: 2294

## \#1 Posted by: Trillium Posted at: 2018-10-19T08:00:31.223Z Reads: 464

```
https://www.youtube.com/watch?v=Vhs697f6K7o

Not my original intended way of revealing this motor to this forum, but hey, development sucks sometimes and I couldn't wait any longer. I had hoped to have them in boxes by now but life got in the way. This project has a lot of other goals and is taking quite longer than I'd like. I was hoping to get some discussion going here so that I could answer some questions but also get feedback so I can eliminate some of the features I was going to implement. 

1)Full 2WD integration onto Ronin trucks (no shafts to worry about) Option of 4WD for you insane folk. Full Integration basically means you can't remove the motors from the trucks and the phase wires would be hidden inside
 2)10mm thick 130Wh batteries (sold separately with own extrusion) with custom 1S 250A controllers
3) 10-12S version that works on any truck (within reason). This was actually the original intent, but 1S requires full integration due to the amount of copper I have to run out of the motor. 10-12S wouldn't be as efficient but might not really matter based on the stuff I see you guys run, you likely wouldn't even care
4) Non-split wheel (if new version runs cool)

I'm more curious what your reactions are before I spill many beans. The split wheel I have mixed feelings about. Seems to ride decently but my only prototype I sent off to another country for wind tunnel testing and I haven't gotten it back yet to be able to do a direct comparison to some other motors.
```

---
## \#2 Posted by: nuttyjeff Posted at: 2018-10-19T08:15:25.895Z Reads: 428

```
At $500 per pair.. i'm out.
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-10-19T08:20:35.945Z Reads: 425

```
I'm kind of confused, what exactly is this? By 1S do you mean running only on 3.7V nominal? Is the battery pack  30Ah? That seems like a really bad idea, even with a 250A esc. There's a reason we use higher voltage batteries.
```

---
## \#4 Posted by: Maxid Posted at: 2018-10-19T08:28:21.289Z Reads: 418

```
Me too - is this a standard Hub motor? What does 1S mean? At 500$ - what's the USP?
```

---
## \#5 Posted by: linsus Posted at: 2018-10-19T08:32:02.065Z Reads: 419

```
Lets try keep generic definitions out of model names xD
```

---
## \#6 Posted by: Trillium Posted at: 2018-10-19T08:33:06.695Z Reads: 416

```
Define "standard"

1S means you could run a single thin pouch cell with each motor pair. It also simplifies the wiring and eliminates need for bms and complicated charging.

$500/pair - You get a good form factor, lightweight, and high performance for the size. Can also run multiple colors of urethane per wheel to make more customization.
```

---
## \#7 Posted by: pixelsilva Posted at: 2018-10-19T08:35:17.337Z Reads: 401

```
How about the thane thickness? Sick of all hub motors with thin sleeves. Now that you will enjoy some form of cooling with that air flow over the motor why not installing thick PU ?
```

---
## \#8 Posted by: Maxid Posted at: 2018-10-19T08:35:37.744Z Reads: 394

```
You actually want to run this at 3.7V? Can't imagine this being a good idea but for science I'd say try it.
Also you'd still need wiring as a single cell probably won't cut it and you'd need several put in parallel.
I also doubt that a Hub motor is a good idea in the current market with a clear trend towards direct drive motors that can use standard wheels with lots of urethane or even AT wheels.
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-10-19T08:38:15.050Z Reads: 392

```
Nah, a single cell can be more than enough, that's the benefit of prismatic lithium cells. You can make them have as much capacity and current draw capability as you want.

However, running at such high current and low voltage is going to make that each heat up like there's no tomorrow.
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-10-19T08:39:49.964Z Reads: 390

```
What kv are those motors 800? :D

![image|632x500](upload://dz2WRJLYig4q5fsmUiFRcPI42Uq.png)
```

---
## \#11 Posted by: Maxid Posted at: 2018-10-19T08:41:28.110Z Reads: 387

```
Do you have a link for such a cell? I'd like to check them out. The largest sensible Lipo pouch I found was [10000mAh with a 5C discharge rating](https://shop.lipopower.de/10000-mAh-37V-Einzelzelle-5C) (which was stated to be only valid for less than 30s).
```

---
## \#12 Posted by: linsus Posted at: 2018-10-19T08:42:57.620Z Reads: 379

```
[quote="Trillium, post:6, topic:71697"]
1S means you could run a single thin pouch cell with each motor pair. It also simplifies the wiring and eliminates need for bms and complicated charging.
[/quote]

I've seen a Phd project running 15kW motor on 8V and around 2kA. It was highly experimental and meant for big ass motors that could dissipate the heat properly.. The phase leads were beyond fat however, There are no practical application here on the esk8 scene more then for sience I'm afraid. I'd try aim for 10S and improvise a good kv ratio from that.
```

---
## \#13 Posted by: Trillium Posted at: 2018-10-19T08:44:45.539Z Reads: 367

```
14.1mm thane thickness
```

---
## \#14 Posted by: Trillium Posted at: 2018-10-19T08:46:35.768Z Reads: 366

```
Right around 700kv I've simmed. I haven't actually built the 1S motor yet.
```

---
## \#15 Posted by: Trillium Posted at: 2018-10-19T08:49:23.078Z Reads: 371

```
It's a cell that actually isn't on the market yet. It's not readily available on gray market. There are a lots of good substitutes though. This is an example of prismatic.. I can't find the one I like at the moment. I never reallly was attracted to prismatics. I'm more interested in single pouch that is very thin.

https://www.electriccarpartscompany.com/72Ah-CALB-UL-Certified-Batteries
```

---
## \#16 Posted by: Trillium Posted at: 2018-10-19T08:50:04.454Z Reads: 367

```
1S is tricky to do on a skateboard but I think it can be packaged nicely and the weight can be kept down.
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-10-19T08:50:16.488Z Reads: 366

```
A123 makes cells like that.http://www.a123systems.com/automotive/products/cells/

  There's probably a few niche websites you could buy large NMC cells like this, maybe even a reseller for the 26Ah A123 cell.
```

---
## \#18 Posted by: pixelsilva Posted at: 2018-10-19T08:50:49.202Z Reads: 363

```
At least double that...triple if you could. ALL hubs in the Universe lack that... thick PU :roll_eyes:
```

---
## \#19 Posted by: linsus Posted at: 2018-10-19T08:51:51.816Z Reads: 362

```
Dont see how the weight is affected other then a smaller BMS and maybe less wires. The energy density doesn't change cause its lower voltage.
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-10-19T08:54:57.051Z Reads: 356

```
Energy density most certainly changes. A smaller surface area of cells decreases volume and weight, relative to the overall volume of functional anodes and cathodes internally.

Weight could be negligable, but size actually changes. Prismatic cells have crimped edges that are usually 3-4mm ish thick. The more cells butted next to each other the more space is wasted.
```

---
## \#21 Posted by: Trillium Posted at: 2018-10-19T08:54:57.322Z Reads: 341

```
That's correct. The overall weight should be about the same as what you guys are used to. Weight doesn't seem that important to you guys anyways. I see these monster builds. BMS becomes just a temperature sensor that most controllers can handle by themselves. The motors themselves are more power dense than what I've seen.. but we're talking grams, not lbs off the wheels.

Would I best be putting my time into a 8" OD hub motor that would work well on scooter as well?
```

---
## \#22 Posted by: Trillium Posted at: 2018-10-19T08:57:24.120Z Reads: 338

```
The energy density can actually improve because there is less interconnections and smaller enclosure necessary for a single pouch... but that's really talking grams, and not the selling point. Selling point is mainly simplicity and no bms. But I think for the size, the motor should be able to pull full torque to 20mph which is uncommon for motors this small.

Sounds like so far people really want big ass motors, not boosted-esque, sleek, "at home" to the longboard scene type motors.
```

---
## \#23 Posted by: sk8l8r Posted at: 2018-10-19T09:09:30.763Z Reads: 331

```
agreed... sounded cool until the 

same old thin thane :(
```

---
## \#24 Posted by: linsus Posted at: 2018-10-19T09:11:23.366Z Reads: 316

```
Meant the energy density of the battery obviously. Not the airgaps in the enclosure. I see your point tho.
```

---
## \#25 Posted by: pixelsilva Posted at: 2018-10-19T09:18:25.779Z Reads: 306

```
Yeah, why?  ...well I know why. Is all heat exchange. Motor temperature rises, but if is covered by thick Uro layer, heat will not disipate properly. Thats why Sleeves are so thin. But is time for a changes. We want hub motors covered by thick PU.
```

---
## \#26 Posted by: Grozniy Posted at: 2018-10-19T09:24:19.382Z Reads: 299

```
We also want 12mm axle, quality bearings, quality glued magnets, thick hanger to dissipate the heat, thick urethane
```

---
## \#27 Posted by: dareno Posted at: 2018-10-19T09:29:05.470Z Reads: 309

```
Whats the benefit here?  If you don't mind me asking?  I mean boosted territory?  If you want to market hub motors to the diy community then it better be a bit better than that regardless of the science involved.
It could be the smartest idea anyones ever had but if it performs like a cheap chinese hub motor then really whats the point?  I don't get it sorry.
```

---
## \#28 Posted by: dareno Posted at: 2018-10-19T09:38:16.487Z Reads: 313

```
[quote="Trillium, post:22, topic:71697"]
not boosted-esque, sleek, “at home” to the longboard scene type motors.
[/quote]

Thats because we already have that in chinese abundance.  Think you might be in the wrong place.
```

---
## \#29 Posted by: Sn4pz Posted at: 2018-10-19T12:51:54.040Z Reads: 316

```
![image|220x220](upload://5kAsL2SLuvcFXixWPXurWMcyc2R.jpeg) 

you right tho :man_shrugging:
```

---
## \#30 Posted by: Jmding Posted at: 2018-10-19T14:43:12.198Z Reads: 300

```
Ah! This is your 1s idea. Interesting. A lot of challenges ahead, but exciting nonetheless!
```

---
## \#31 Posted by: Trillium Posted at: 2018-10-20T02:24:13.183Z Reads: 285

```
Whoever would like to send me motors to dyno, I'll get more benchmarks on the power you are actually putting to the ground with your setups. Just because you're running 2000W limits doesn't mean you're getting it to the ground.

If you guys want, I will design a motor exactly to your preference, but I can't guaranntee it will cost less than $500 per pair.
```

---
## \#32 Posted by: Trillium Posted at: 2018-10-20T02:28:39.679Z Reads: 278

```
How about 107mm? I could do that. That's a wheel size that would match well to abec11s.

How many people would put down $2k for a 4WD setup these days? What is the going rate?

What is it about the thick thane that you want? Better ride quality? Do you want large diameter or thick thane? What is too wide of a wheel in your opinion?
```

---
## \#33 Posted by: professor_shartsis Posted at: 2018-10-20T03:18:35.536Z Reads: 292

```
[quote="Trillium, post:16, topic:71697, full:true"]
1S is tricky to do on a skateboard but I think it can be packaged nicely and the weight can be kept down.
[/quote]

it so happens i simulated a one cell hub motor with the same performance characteristics as a pair of @hummie 73kv hubs w/100a motor current limit the other day...

what ESC do you plan to use that allows 1250a motor current?

what connectors and wire gauge will you use when pulling 1400a from your 3.7v battery?

[quote="professor_shartsis, post:46, topic:70807"]
one cell dual hub motor:

one cell 4v battery, dual 900kv hubs w/ 0.0005ohm &amp; 84mm tires, 1250a motor current limit, 690a battery current limit per motor (1380a battery combined):
[/quote]
https://image.ibb.co/m4OvKU/1cell.jpg

https://www.batteryspace.com/productimages/lifepo/5907.jpg

https://www.batteryspace.com/lifepo4-prismatic-module-3-2v-100ah-10c-rate-320wh-un38-3-passed-dgr.aspx?gclid=eaiaiqobchmiuvo_ood_3qivgksnch3yfay-eakyasabegklfvd_bwe
```

---
## \#34 Posted by: Trillium Posted at: 2018-10-20T04:02:58.200Z Reads: 275

```
I don't know where you get your numbers for your model. Maybe I could have a closer look at your stuff.

it'll be a 200-300A motor current limit, with a custom controller my buddy and I are working on.

@Hummie can I dyno a pair of your hubs? Need to borrow VESCs and battery to do it.
```

---
## \#35 Posted by: Hummie Posted at: 2018-10-20T04:12:12.557Z Reads: 267

```
yes please do.  Give me a week to finish things n then
```

---
## \#36 Posted by: professor_shartsis Posted at: 2018-10-20T04:55:59.325Z Reads: 272

```
[quote="Trillium, post:34, topic:71697"]
I don’t know where you get your numbers for your model. Maybe I could have a closer look at your stuff.

it’ll be a 200-300A motor current limit, with a custom controller my buddy and I are working on.
[/quote]

sure, let's suppose we use 1250a motor current limit with a 900kv motor....

60 / (2 * pi * 900 kv) = **0.01061 newton meter per motor amp** = KT
0.01061 nm/a * 1250a = **13.26 nm torque**
(13.26 nm torque * 1000mm) ÷ ((1 / 2)× 84 mm tire diameter) = **315.71 newtons thrust per motor**
315.71 newtons * 0.2248 lbs force per newton = **70.97lbs thrust per motor at 1250a motor current**

^70.97lbs thrust per motor requires 1250a motor current

now let's compare to 73kv @hummie hub w/ 100a motor current...

60 / (2 * pi * 73 kv) = **0.13081 newton meter per motor amp** = KT
0.13081 nm/a * 100a = **13.081 nm torque**
(13.081 nm torque * 1000mm) ÷ ((1 / 2)× 84 mm tire diameter) = **311.45 newtons thrust per motor**
311.45 newtons * 0.2248 lbs force per newton = **70.01lbs thrust per motor at 100a motor current**

^70.01lbs thrust per motor requires 100a motor current

conclusion... same thrust as 73kv 100a motor current @hummie hub w/ 900kv hub requires 1250a motor current
```

---
## \#37 Posted by: Jmding Posted at: 2018-10-20T06:45:12.068Z Reads: 249

```
Or quick and dirty, 1/12th the voltage needs 12x the current to yield equal power. People here like to run dual 60a motors, so that puts you at 1440A approximate target current.
```

---
## \#38 Posted by: pat.speed Posted at: 2018-10-20T07:14:06.137Z Reads: 243

```
Just a question that’s got nothing to do with this particular topic, but does stator size affect torque in any way? Apart from staying cooler at higher amps
```

---
## \#39 Posted by: Jmding Posted at: 2018-10-20T07:22:29.963Z Reads: 253

```
There's no "apart from" staying cooler at higher amps. It's ALL ABOUT staying cooler at higher amps. Staying cool means more current. More current means more electrical power. More electrical power means more mechanical power (i.e. torque and speed).

Torque = current / Kv, so cooler motors = more current = more torque
```

---
## \#40 Posted by: Trillium Posted at: 2018-10-20T07:29:00.265Z Reads: 252

```
Current isn't what you're after.. amp-turns is what you're after. Current by itself is not really worth comparing things by. 1000A through 1 turn is the same as 100A through 10 turns.

cooler motors = more copper volume. More torque is the result of making use of your amp-turns effectively and having a balance of high amp turns and high steel content

Keeping your motor operating at a low current with more copper is how you keep a motor cool.
```

---
## \#41 Posted by: pat.speed Posted at: 2018-10-20T07:30:04.678Z Reads: 232

```
Well there is, and I realise bigger motors handle more current that’s why I said “apart from”. I was asking if larger sized motors create more torque, which would make sense and is what is generally found
```

---
## \#42 Posted by: Andy87 Posted at: 2018-10-20T07:33:50.401Z Reads: 227

```
My kind of thoughts are, bigger stator bigger magnets, bigger magnetic forces results in more torque.
```

---
## \#43 Posted by: Trillium Posted at: 2018-10-20T08:49:22.423Z Reads: 243

```
I looked at the numbers again. I was mixing things up. I simulated 4.45Nm/230A = 0.01935 Nm/A

493kv or so, but let me re-sim things.

Thrust should be 4.45Nm / 0.042m = 106N per motor, which is plenty.

This is only 21A/mm^2 current density. It can be increased to about 45A/mm^2 so I expect 660A will work just fine at approx. 12.77Nm. I don't have any plans to pursue a 660A motor controller, as its another $40 of controller to make.

The thing is, that's an insane amount of thrust for a skateboard. You have to be strapped in. This is why we need to dyno test Hummie's motors, because I suspect they are saturating well before your 13Nm number or you guys are just insane. :smiling_imp:

If he is truly at 13Nm, that's great. I think you're better off though with 4WD and more urethane with that kind of power level.

I might take it up to the 300A level and lengthen a little bit, but I need to model up the ronin trucks first and see what looks good.
```

---
## \#44 Posted by: Grozniy Posted at: 2018-10-20T08:51:28.816Z Reads: 224

```
And more resistance :thinking:
```

---
## \#45 Posted by: Jmding Posted at: 2018-10-20T08:53:20.075Z Reads: 236

```
[quote="Trillium, post:40, topic:71697"]
Current isn’t what you’re after… amp-turns is what you’re after. Current by itself is not really worth comparing things by. 1000A through 1 turn is the same as 100A through 10 turns.
[/quote]

Yes actually you are right. Turns is correlated with Kt, and torque = kt * current. In most of our builds where our motors basically cannot be over-volted and where gearing is a thing, current is basically the only way that motor selection can affect output power. Voltage is already limited by our ESCs, so the only thing we can play with is finding ways to increase motor current.
```

---
## \#46 Posted by: Jmding Posted at: 2018-10-20T09:04:14.184Z Reads: 223

```
There are so many challenges for this build! Even just wires and connectors desoldering themselves! But it sounds like you know your physics, and I imagine you might have had a few sleepless nights thinking through the engineering. Keep us posted!
```

---
## \#47 Posted by: Andy87 Posted at: 2018-10-20T09:19:04.049Z Reads: 223

```
Maybe the reason why @Kug3lis 80xx motors become more hot than his 60xx ones 🤔
```

---
## \#48 Posted by: professor_shartsis Posted at: 2018-10-20T13:59:05.000Z Reads: 226

```
[quote="Trillium, post:43, topic:71697"]
493kv or so, but let me re-sim things.
[/quote]

17mph top speed?
```

---
## \#49 Posted by: Trillium Posted at: 2018-10-20T17:12:05.359Z Reads: 215

```
field weakening will get it up to 23-25
```

---
## \#50 Posted by: Battosaii Posted at: 2018-10-20T17:51:19.425Z Reads: 218

```
That's pretty slow IMO and with "boosted" level torque it's gonna be super weak. Imo a meepo will perform about the same but you get a whole board for the same price.
```

---
## \#51 Posted by: Trillium Posted at: 2018-10-20T18:47:46.482Z Reads: 215

```
So what is the acceptable conversion between $ and thrust per wheel?

@hummie is doing what $425 for a set of trucks with two hubs? 311N per $212.50 (one motor/one truck). $0.68/N. So my hubs with two trucks need to cost $72 each, or double that if I pull off a 660A controller. That might be workable. 

What would you guys say is the max you'd pay for a premium dual motor + two premium downhill racing trucks + dual controller combo + 90mm wheels? Everything but battery and charger basically.

Separately, what would you pay for the same setup but 4 hub motors instead of 2?
```

---
## \#52 Posted by: professor_shartsis Posted at: 2018-10-20T19:03:25.311Z Reads: 206

```
if you’re going the route of a custom ESC, why not build one that can handle 75v-100v and a motor which is around 73kv? then you can get the better performance than presently available (same torque but higher top speed)?
```

---
## \#53 Posted by: Trillium Posted at: 2018-10-20T19:06:15.377Z Reads: 207

```
We will make a version of the ESC that will do higher voltage, but to increase the urethane it helps to get the motor diameter down, which is what I've done with this 1S motor geometry. However, if I did higher voltage I would need to go to a larger diameter motor because there isn't enough space to fit the copper in smaller diameter multi-turn motors. The OD is only about 52mm. so a 90mm wheel would give 19mm of urethane, which is better than average right?
```

---
## \#54 Posted by: Battosaii Posted at: 2018-10-20T19:06:38.431Z Reads: 210

```
FYI most of the DIY community thinks Boosted is very very very slow, I don't hate on it it's a decent board but it shouldn't be the one your comparing your self to, not here cause it's not impressive.
```

---
## \#55 Posted by: Trillium Posted at: 2018-10-20T19:07:24.293Z Reads: 205

```
I'll from now on just compare to hummies.
```

---
## \#56 Posted by: professor_shartsis Posted at: 2018-10-20T19:12:26.220Z Reads: 219

```
[quote="Trillium, post:53, topic:71697"]
to increase the urethane it helps to get the motor diameter down
[/quote]

i believe many folks also want efficiency which is generally achieved by making the motors and copper mass larger...

[quote="pat.speed, post:38, topic:71697, full:true"]
Just a question that’s got nothing to do with this particular topic, but does stator size affect torque in any way? Apart from staying cooler at higher amps
[/quote]

@pat.speed if the KV is the same then different size stators will produce the same torque for the same quantity of motor current, but the larger stator can handle more current before it becomes magnetically saturated -- a state which means the torque no longer increases with a linear relationship to motor current.

[quote="Trillium, post:55, topic:71697, full:true"]
I’ll from now on just compare to hummies.
[/quote]

https://image.ibb.co/jHuqmL/IMG-6658.jpg
```

---
## \#57 Posted by: Trillium Posted at: 2018-10-20T19:13:13.572Z Reads: 211

```
What does the split wheel do for you guys cosmetically?
```

---
## \#58 Posted by: Sn4pz Posted at: 2018-10-20T19:19:47.060Z Reads: 210

```
to be honest i would feel safer on a completely unified contact point/pitch

but i could definitely be proven wrong x)

it does look sick though, very future....y
```

---
## \#59 Posted by: Trillium Posted at: 2018-10-20T19:32:00.416Z Reads: 213

```
This is 90mm OD x 65mm wide
https://uc346518667fe9825f6052a830b6.previews.dropboxusercontent.com/p/thumb/AAPe2IQvcRcUpJfPUo4TVOfklggqS7CoY3oij6b0bnUvjIy4p3lRNED3Pq8zUhgU56m_viupJFkMcbBsF7w8FQ8ICchyy0VKryKw1iy1UieV39AthAJQ4x-7AuUpVI_ziKJNSqn1ShmIpnPzg5IQcMeRGyGEGEYNoihaiKKmGpcl5Qn0vp2dM2VrYcApfGCFBd9V73QkR6OTsBwEKg6FMIZ1NvahTe35Ep5EFOrmNbDmIw/p.jpeg?size=1024x768&size_mode=3
```

---
## \#60 Posted by: trancejunkiexxl Posted at: 2018-10-20T20:59:05.093Z Reads: 209

```
whatever happens i just hope there is an option for pneumatic wheels. the roads near me are just awful :tired_face:
```

---
## \#61 Posted by: Battosaii Posted at: 2018-10-20T21:18:25.773Z Reads: 206

```
Hmm wouldn't road grime just gunk up in that slit till it's filled completely like how mud fills tire treads. This would require frequent cleaning to keep the cooling aspect effective.
```

---
## \#62 Posted by: Trillium Posted at: 2018-10-20T21:24:35.319Z Reads: 204

```
I'm not sure. I think you'd have to be pretty careless to get it dirty enough to matter... Idk. A toothbrush and some alcohol would solve that problem. You probably wouldn't even need to take the urethane off or maybe just the outside most urethane
```

---
## \#63 Posted by: Trillium Posted at: 2018-10-20T23:33:45.351Z Reads: 207

```
@professor_shartsis I'm getting 7.7Nm at 500A with my original small stator, not even saturating the motor hardly.... 171N in 90mm wheel. That comes out to a price of around $120 per motor + truck to be competitive, or $500 for a complete truck  + 4 motor set which would outperform dual hummie motors and have more urethane and likely look better. I don't think that price will leave enough room to grow the business though.
```

---
## \#64 Posted by: skatardude10 Posted at: 2018-10-21T00:04:52.533Z Reads: 202

```
What wire guage are you going to be using? Everything I'm reading says that for lengths on a skateboard you are going to need at least 4awg or thicker to carry >2-300 amps
```

---
## \#65 Posted by: Trillium Posted at: 2018-10-21T00:10:02.583Z Reads: 205

```
About 7AWG equivalent. I want to integrate the controllers beneath the truck base as a sort of riser, all heatsinked to the truck base. So the phase lead runs are a lot shorter this way, so the wires don't have to be quite as thick as 4AWG.
```

---
## \#66 Posted by: professor_shartsis Posted at: 2018-10-21T00:41:07.465Z Reads: 213

```
[quote="Trillium, post:63, topic:71697, full:true"]
@professor_shartsis I’m getting 7.7Nm at 500A with my original small stator, not even saturating the motor hardly… 171N in 90mm wheel. That comes out to a price of around $120 per motor + truck to be competitive, or $500 for a complete truck + 4 motor set which would outperform dual hummie motors and have more urethane and likely look better. I don’t think that price will leave enough room to grow the business though.
[/quote]

if you're getting 7.7Nm @ 500a, that comes out to about 620kv.... 4 motors gives about 153lbs thrust with 500a motor current limit... close to 1800a battery current full throttle accelerating through 20mph... this is assuming 500a motor & battery current limits per motor (3.7v 1 cell battery pack) and resistance of 0.001ohm @ 620kv... both top speed and thrust per motor appear to be lower than the 73kv @hummie -- 20-25mph & about 38lbs per motor.

https://image.ibb.co/cm0mBL/620kv.jpg
```

---
## \#67 Posted by: Trillium Posted at: 2018-10-21T00:58:00.569Z Reads: 201

```
We're on the same page I think. Dual hummies is about 140lbf I thought. 4WD Trillium would be slightly more thrust than dual hummies.

The idea would be to somehow magically offer 4WD around the same price  but higher quality components. Maybe can justify another $500 if including 4 controllers +
```

---
## \#68 Posted by: professor_shartsis Posted at: 2018-10-21T01:01:39.465Z Reads: 204

```
i think folks will be very interested in a controller that can do such high current limits, especially if it can also do  higher voltage limits than about ~60v as well, and especially if there are no erpm limits. this would enable a performance or efficiency boost even with off-the-shelf existing drivetrains by enabling the use of higher pack voltages, higher kv motors w/ higher motor current limits & higher gear ratios.
```

---
## \#69 Posted by: Trillium Posted at: 2018-10-27T19:23:03.606Z Reads: 195

```
What do you guys really want and need.. those are the two questions.
```

---
## \#70 Posted by: trancejunkiexxl Posted at: 2018-10-27T20:00:23.057Z Reads: 197

```
Speed and lots of it
```

---
## \#71 Posted by: professor_shartsis Posted at: 2018-10-28T09:46:46.340Z Reads: 196

```
high thrust (low kv, high motor current), high speed (high voltage), high efficiency (low electrical resistance), low cost, availability, wheels don’t fall off the board (12mm+ axles) & won’t burst into flames (LiFeSO4?), low controller heating (controller with high current/voltage ability, low resistance & heatsinks)
```

---
## \#72 Posted by: deucesdown Posted at: 2018-10-28T14:59:21.471Z Reads: 195

```
Durable, good brakes, decent torque and top speed, ride quality. In that order I think. Price is not as important, as shown by carvon and enertion?
```

---
## \#73 Posted by: linsus Posted at: 2018-10-29T08:50:36.579Z Reads: 191

```
Good, Fast and Cheap. Choose two.

![](https://media.giphy.com/media/DWt9KVC5GIVqM/giphy.gif)
```

---
## \#74 Posted by: Jacobee Posted at: 2019-01-09T02:45:24.125Z Reads: 166

```
Sorry to revive an old thread but did this ever go anywhere? This looks like an interesting idea. @Trillium
```

---
## \#75 Posted by: Benjamin899 Posted at: 2019-01-09T02:48:35.351Z Reads: 168

```
Same. Still on my watchlist. Even though i think it is misplaced brainpower.
```

---
## \#76 Posted by: Trillium Posted at: 2019-01-09T04:01:46.107Z Reads: 168

```
It's a slow, expensive process.
```

---
## \#77 Posted by: Trillium Posted at: 2019-01-21T00:44:20.831Z Reads: 140

```
How much thane do you guys really want? and what's the widest wheel you'd want. Preferably would be nice to get like a dozen or so responses. maybe I should make a new thread.
```

---
## \#78 Posted by: brenternet Posted at: 2019-01-21T00:49:57.623Z Reads: 143

```
Honestly, I know you're probably sick of hearing it but Hummie has nailed it. Centrax width with high quality thane at a decent thickness.
```

---
## \#79 Posted by: mmaner Posted at: 2019-01-21T01:31:58.628Z Reads: 138

```
At least 30mm and 77mm wide.
```

---
## \#80 Posted by: Trillium Posted at: 2019-01-21T01:48:20.141Z Reads: 136

```
I'm hearing all sorts of opinions. good. 30mm diametric? so 15mm thick?
```

---
## \#81 Posted by: mmaner Posted at: 2019-01-21T02:31:01.036Z Reads: 130

```
No, 30 from the can out, diameter.
```

---
## \#82 Posted by: skatardude10 Posted at: 2019-01-21T04:02:39.367Z Reads: 124

```
I did my best with my finger. ![Screenshot_20190120-210151_Keep%20Notes|561x500](upload://u5vZwe2mWiCLyxH7ECCvuEdyvpl.jpeg) 

And I agree. Thicker is better.
```

---
## \#83 Posted by: Trillium Posted at: 2019-01-21T05:04:54.565Z Reads: 123

```
I see. So what width is considered too wide?
```

---
## \#84 Posted by: Trillium Posted at: 2019-01-21T06:10:50.228Z Reads: 118

```
30mm thane cross section... This would be 115mm OD x 78mm wide.... with 32mm offset from standard 180mm truck. 273mm outer to outer. What wheelbase would sort of be middle ground for wheels this size?

I think this would be too wobbly. I don't see this working well.

![image|658x329](upload://plmYtIzOOrWw0hQrf2FiTEkeU89.jpeg)
```

---
## \#85 Posted by: TowerCrisis Posted at: 2019-01-21T11:09:59.097Z Reads: 100

```
Well, most people aren't using 180mm trucks nowadays. Most have moved onto 195mm or 215 or caliber-e which have an effectively longer length..

I'd personally say you don't need the full 30mm, if it means you can cut down on that size. Like 25mm would probably cut it. 115mm is getting on the larger size but I'm not one to speak on that. I'm perfectly satisfied with my 85mm cagumas lol
```

---

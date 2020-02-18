# You really don&rsquo;t NEED a BMS with cheap lipos

### Replies: 63 Views: 6036

## \#1 Posted by: RogerD Posted at: 2017-02-15T23:16:09.719Z Reads: 580

```
I keep seeing people getting confused with BMS setups. Building a new board and trying to understand why they need a BMS, which BMS?, will it be for charging and discharge?, or just charging? How do they wire it? etc etc.

You really don't need one in most cases.

My board charges directly from a £14 lipo charging brick from ebay (2 packs of 6s 15000mah each). You can get them for 8s, 10s, 12s...  I use this http://www.ebay.co.uk/itm/21-6V-22-2V-2A-DC-25-2V-Three-stages-Lithium-Battery-Charger-14500-14650-18650-/182209541446?hash=item2a6c88f546:g:0XQAAOSwNKRXjIVP

It means I can install a 3.5mm power jack on my board and simply plug in the charger and walk away. When it's charged the LED on the charger will go from red to green.

I've been using lipos for years and years, well before eelctric skateboards. Unless you have a bad pack, or you regularly run your packs below 3.2 volts per cell they will stay mostly in balance. By mostly, I mean close enough it makes zero difference. If you have a bad pack then no amount of BMS balancing will make it good. If a pack has a lazy cell i.e. all at 4.2v and one at 3.95v , it will never really recover.

Set your ESC to cut off before your batteries get to 3.2v (at rest) and you can't flatten your lipos. On most ESCS choose the middle to cautious cut off setting. If your pack doesn't seem to run for long before cut off, measure the voltage at rest, and if it's ok, reduce the cut off voltage, then retry. This is the key. Over discharging packs kills them. You don't need a BMS to stop this happening, you need to use the correct low voltage cut off on your ESC.

When you charge packs, they equalise automatically. Once near full they'll all end up at 4.2v per cell. If you have a duff cell then you can of course run into trouble as it lags way behind, but I've not had this happen on probably 40 packs I currenty have in use (heli's quads, cars, esk8).

With some packs (heli/quad) I "treat" them to a balance charge once or twice a year, but no more. It takes ages, and makes near to no difference. They only real benefit is it will show if you have a duff cell.

For the low cost of lipos it's really not worth obsessing about balancing.

Sure, if you have spent a lot if time and money  making a 18650 slim pack, I'd probably install a BMS too - to protect your investment, and you are using MUCH lower Mah cells than big lipo packs, so you run a higher risk of knackering them all if one starts going down as it will go from full to empty much quicker. Plus it can be a fun project. But I'm seeing lots of people building boards with cheap lipos being told they need a BMS. You just don't.

As a case in point , I've just metered my two 6S Turnigy Multistar (cheap) 15000mah packs (normally connected in parallel but unplugged for measuring voltage). Used all last year, never balanced, always charged as above.

Pack 1: 
4.01
4.02
4.00
4.02
3.99
4.01
Pack 2:
3.95
3.95
3.98
4.05
4.04
4.05

Pack 1 is near perfect, Pack 2 is fine, not quite the quality of pack 1 but easily good enough - a max of 0.1v cell difference. Those packs have been sitting unused in my garage since last summer. All the cells will equalise under charge. And because I don't run my packs under 20% of their capacity, it doesn't matter that I've got a 0.1v cell difference.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-15T23:32:02.415Z Reads: 508

```
If you want to go this way, fine. But you really shouldn't be giving this kind of advice especially since there are people on this forum who are just starting out and have little or no experience with Lipo cells.
You say its ok to charge without balancing. But what if you have a couple bad cells. So your no balance charger keeps charging until it overcharges and ruins the cells that where good. Or even worse causes a fire.
True, you don't have to use a bms. Using a bms is about extra protection and convenience.
However if your not going to use a bms, then you should use a hobby charger and balance your Lipos every charge for maximum safety and performance.
```

---
## \#3 Posted by: RogerD Posted at: 2017-02-15T23:43:26.210Z Reads: 494

```
You've ignored what I've said. It isn't bad advice.  It's not "going this way". It's why I posted this thread. There is a lot of unnecessary fear over charging.

You can "what if" all day but the reality is that uneven cells balance themselves pretty well . If they are massively out you'll know when you receive them and test them, from new.
```

---
## \#4 Posted by: emepror Posted at: 2017-02-15T23:53:19.204Z Reads: 464

```
You've been using Lipo cells for years, but have you put hundreds of hours on said lipo packs? Sure to start they will be "perfect" but they will all have varying internal resistances etc. They will charge and discharge differently every so slightly eventually potentially killing cells. There's a reason hoverboards are banned, which is an extreme example with poor quality cells but its what would happen in the worst case scenario. Discharging AND overcharging is what can damage cells as well as heat. The biggest problem with not using a BMS when charging is that while the charger may see 42V that doesn't mean each cell is at 4.2V some could be 4.3V which will continuously degrade the cells until issues occur. And they dont automatically equalize when you charge them..... 

In the end its 40 bucks for a decent BMS, its worth the expense, especially considering it will extend the life of the battery.

Finally I'd more likely not put a BMS on quality 18650's than lipo packs as a personal note.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-02-16T00:05:12.682Z Reads: 411

```
[quote="RogerD, post:3, topic:17765"]
You've ignored what I've said. It isn't bad advice.
[/quote]


I didn't ignore what you said.
But I feel strongly enough about this subject that I had to disagree with you.
Safety needs to be a priority. That means using quality Lipos and balancing them regularly.
```

---
## \#6 Posted by: PXSS Posted at: 2017-02-16T00:21:39.273Z Reads: 399

```
It is dangerous to say you do not need a BMS. Have you seen a LiPo fire? I've seen tens, most of them under controlled experiments but some accidental fires at RC airfields. It's one thing for it to happen on an RC airplane that you fly in a controlled environment, it's a completely different thing if it happens on a skateboard under your feet in a populated street or as someone in this forum already experienced in their apartment. 

Most are likely a cause of stupid mistakes by people. You cannot possibly believe that everyone will do things properly when setting up their skateboards for the first time specially if they have no experience with electronics or rc toys.

A VESC with bad settings could easily be the cause of a LiPo fire. A BMS does not have any settigs to mess up and will save a battery when the VESC would be the cause of a failure. 

A wall charger like yours does not balance cells and cells do not balance automatically when charging, that is completely false. If cells are in parallel, they will balance each other, if cells are in series they will not. That is the issue, if you have a bad cell and your wall wart charges to 25.2V for a 6S, then the bad cell will be overcharged while the others stay below 4.2V. As you keep cycling the cell, the problem will get worse and worse, at the low end the bad cell will be over discharged and at the high end the bad cell will overcharged. This unbalance will eventually drag the other cells out of balance and from there it's only a matter of time before they blow.

A BMS prevents this by balancing your bad cell every time you charge and prevents it from quickly deteriorating. Now, a real BMS monitors cell voltages individually and cuts off the pack when any one cell reaches the low voltage cutoff. I do not think the BMS most people here use (the one from batterysupports) does this. It only monitors pack low voltage so in this case your cell will still deteriorate but much slower than if it wasn't being protected at the high end. 

Balance charging literally takes an extra 15minutes on a good charger with fast balance settings. 

I agree that a BMS is not required if you use quality packs (which if you buy the cheapest from hobbyking you are not), set up your vesc properly and nothing goes wrong. 

Do you know how FETs usually fail? (FETs are the switches on your VESC) They usually fail closed which means a direct external short to your batteries. A BMS could save your battery in this case. 

And it's not only about defective electronics. What happens when you hit a curb wrong or a rock or go through a puddle and your wires or ESC or anything down the line of your battery shorts? A BMS could prevent a fire. 

There are plenty more reasons to use a BMS if you do not have a balance charger or monitor your cells. 
Do you need one? No.
Will you regret not having one when your VESC shits on you or when you get a defective pack or when you get a charger that tends to overcharge your pack constantly? Absolutely. 

So yeah, everyone here should advice others to get a BMS. Your post is like saying you dont really need a helmet to ride, all you need to do is not fall on your head ever.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-02-16T00:23:14.853Z Reads: 335

```
I have never used a BMS.
just careful battery voltage monitoring. you don't need one.

however, if you are not an experienced lipo user a BMS is a bit of "idiot proofing" so to speak. 


TLDR: BMS not needed but recommended.
```

---
## \#8 Posted by: lowGuido Posted at: 2017-02-16T00:28:45.624Z Reads: 333

```
oh, and one more thing. a lot of people around here seem to thing that a BMS is full of magical unicorns that will save their battery from everything. its not.
BMS can and do fail.

 [quote="PXSS, post:6, topic:17765"]
Do you know how FETs usually fail? (FETs are the switches on your VESC) They usually fail closed which means a direct external short to your batteries. A BMS could save your battery in this case. 

And it's not only about defective electronics. What happens when you hit a curb wrong or a rock or go through a puddle and your wires or ESC or anything down the line of your battery shorts? A BMS could prevent a fire.
[/quote]
everything you have said here can just as easily kill your BMS. they are still made of FETs and resistors after all...

the bottom line here is that lipos need to be looked after.. BMS or not.
```

---
## \#9 Posted by: PXSS Posted at: 2017-02-16T00:35:59.452Z Reads: 319

```
Yes, BMSs can also fail, but what are the odds of your VESC failing and your BMS failing?

As one user here experienced, he burned his VESC and his vedder switch saved him. Then for some unknown reason he decided to turn the board back on and his switch failed which led to a battery fire. A BMS, even a cheap one would add an extra layer of protection. 

Properly designed BMSs do not suffer these issues as they are set to cut off current well below their rated capacity. I've tested this many times at work :slight_smile: (My job is fun)
```

---
## \#10 Posted by: benwong Posted at: 2017-02-16T00:43:44.837Z Reads: 307

```
I wish to have simple and easier way to charge my lipo, if without using BMS, can it be using laptop style charger charge directly to Lipo? 

I am BMS is for charging purpose. Make it more convinient and simple.  
I have less knowledge or experiance about lipo or li ion battery, and there is tons of thread in here talk about BMS. so i just follow the commend way of here. 

Beside using BMS, any other way ?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-02-16T00:58:40.421Z Reads: 303

```
[quote="benwong, post:10, topic:17765"]
Beside using BMS, any other way ?
[/quote]


Besides a bms, a good hobby balance charger is actually better for charging than a bms.
As mentioned already the short protection that a bms has is a huge plus. I had a short once at the charge port on my board while the bms was on and it instantly shut the circuit down so nothing was damaged and the batteries didn't even get warm or loose any noticeable voltage.
```

---
## \#12 Posted by: benwong Posted at: 2017-02-16T01:02:57.814Z Reads: 286

```
I have a cheap balance charger using when i haven install BMS. It take sometime to charge the battery and feel abit troublesome to charge. Last two day i just installl my BMS. Everything find.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-02-16T01:41:05.582Z Reads: 281

```
[quote="PXSS, post:9, topic:17765"]
he decided to turn the board back on and his switch failed which led to a battery fire.
[/quote]


I've had 2 external E-switches fail on me both times it was stuck in on position. The first one failed due to heat.
the 2nd failed in the first 5 min of operation. The built in E-switch on my Bestech BMS is still working perfectly after months of use.
Funny part is the E-switches cost almost as much as the BMS!
```

---
## \#14 Posted by: Namasaki Posted at: 2017-02-16T01:45:25.813Z Reads: 269

```
[quote="lowGuido, post:7, topic:17765"]
I have never used a BMS.just careful battery voltage monitoring. you don't need one.
[/quote]

I totally agree with you on the voltage monitoring. I have my voltage meter showing through the top of my deck and keep a close eye on pack voltage even with a BMS.
```

---
## \#15 Posted by: PXSS Posted at: 2017-02-16T01:53:58.916Z Reads: 262

```
I mean, you guys would chew up anyone who showed up here and posted a thread about "You really don't NEED a helmet with a cheap longboard"
We have a sticky thread about it. 

In that same manner, you would get chewed up at an rc airfield if you showed up with a laptop charger and no charging protection to charge Lipos, you most likely would get kicked out! I don't know why you guys insist in risking yourselves and others like that. If you want to do it, fine. You have been warned but don't tell other people to make unsafe decisions based on you not having accidents. 

You dont need a seatbelt or airbags to drive your car, you dont need a helmet or a bms or a fuse to ride an electric skateboard/bike, you dont need a fire extinguisher in your home. You don't need a pilot since we have autopilots that can take off, fly and land automatically. You dont need a reserve parachute to skydive. I can think of sooo many things that are similarly important, lives are at stake. Take your chances with your own, not someone elses.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-02-16T03:25:49.310Z Reads: 252

```
Amen to that!
```

---
## \#17 Posted by: emepror Posted at: 2017-02-16T03:33:47.762Z Reads: 255

```
A hobby balance charger is nothing more than an external BMS,  it's almost the exact same circuit as the BMS's that people put on their boards.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-02-16T04:49:46.164Z Reads: 256

```
A BMS can't balance cells that are drastically out of balance.
That's why cells need to be equally charged before they are connected to a BMS. 
This is usually not an issue if using new cells or new Lipo packs because they come pre balanced within 1 tenth of a volt. 
But if your building a pack of used or mixed cells, or replacing cells or a pack on a used build then you will need a hobby charger to balance them prior to assembly.
Maybe they both balance the same, I can't say for sure but with a hobby charger you can isolate cells or packs for individual balancing during maintenance. 
So really, it's good to have a hobby charger on hand even if you use a BMS.
```

---
## \#19 Posted by: PXSS Posted at: 2017-02-16T08:56:48.688Z Reads: 250

```
Ish. Hobby balance chargers usually have the ability to discharge up to 1A on balance leads. The way they balance in principle is the same, all cells get charged but power is dissipated through a resistor on the cells that are fully charged. A BMS usually doesn't have this kind of current capacity (its more like in the order of tens of milliamps) in their balance circuit and that is why they recommend pre-balancing when you assemble a new pack. Otherwise, you would take an absurd amount of time balancing. 

Now, real good and expensive BMS have gates on each balance connection and can charge/discharge through them. Making them a lot faster and efficient since now you only charge the cells that need charging instead of the whole pack.
```

---
## \#20 Posted by: PXSS Posted at: 2017-02-16T09:04:09.324Z Reads: 238

```
@RogerD please explain to me how uneven cells "auto" balance with your brick laptop charger.
```

---
## \#21 Posted by: RogerD Posted at: 2017-02-16T09:06:17.771Z Reads: 233

```
You know none of us were balance charging when Lipos were first in use right? The vast majority of our helis didn't go down in flames (and when you do get a burning pack it's under load when over discharged a lot of the time -- think "hover boards")

I have put 100's of charges and hours through many many packs. I've been flying helis since I was 32 (16 years ago) Prob 14 years with lipos. I'm still using some of the same lipos for lesser duties, like powering FPV ground stations.

I have only ever had one pack swell in a big way (didn't cause a fire) - and it was due to me trying to...... add balance leads to a non balance leaded pack and messing up the soldering with a simple mistake. This was when balance chargers came to the market and everyone made out it was a must have feature. So I added balance leads to my older packs.

I'm willing to bet that more people here have damaged lipo packs by cutting the balance leads and adding BMS boards (when they are not experienced with working with high voltage and soldering) that just natural charging damage from inbalance.

I understand that lipos can cause a fire if overcharged. I understand that balanced cells are healthy. I don't argue that.

However, charging with a power brick is low current (circa 2 Amps). In the high capacity packs we are using - one of my parallel setups is circa 24000 Mah - you are pretty much trickle charging the pack. It will equalise during this charge. It would take days for a duff pack to swell. You'd notice your charger had not completed before that.

I also fast charge at max amps (16amps on my RC charger) when I'm in a hurry - I do this in my garage. The risk is extremely minimal.

Saying that advising no balance charging is akin to advising not to wear a helmet is not really a fair comparison. Not wearing a helmet on a board going over 15 + mph is a known, high risk. You are inches from the ground and a crash will likely result in an uncontrollable fall (head impact to ground). But then many of us don't wear a helmet cycling (and won't unless forced) - this is NOT a high risk, it is a calculated risk. Most of survived our childhood without a helmet. Studies show you are statistically more likely to be hit by motorists when wearing a cycle helment as motorists see you as "safer" and give you less room. But still, people call you an idiot for not wearing a cycle helmet. You calculate the risk and take what you deem is acceptable. You shouldn't base this decision on what others "insist" is true, or, try and 100% mitigate all risk.

If you rummage through your gadgets and take them apart, you will find that a LOT of them have multi cell lipos and do NOT have balancing circuitry in them. They "dumb" charge them to 4.2v/8.4v/12.6v but you still use them.....
```

---
## \#22 Posted by: RogerD Posted at: 2017-02-16T09:15:32.426Z Reads: 211

```
PXSS - the moment you plug in the charger all the cell voltages start climbing. The lower cells lag behind but catch up as they charge. At the top of the charge, as the cells approach 4.2v each, the total pack voltage approaches (for 3s in this example) 12.6 volts. Lets say one cell is a little behind. You have 4.2, 4.2 and 4.0v. That's 12.4, so the charger slowly trickles in power until it sees 12.6v. This will either happen as the cells go 4.3,4.3,4.1, for example, = 12.7 volts. The charger stops. The pack settles back to 4.2, 4.2, 4.1. This equals 12.5v so the charger puts a little more in. It keeps doing this until the pack settles at 12.6 v at rest. This will happen when all the cells settle at 4.2 volts, or you end up with something like 4.3, 4.3, 4.0. (this pack, I would bin)

It's fine for a pack to be a little over 4.2v per cell. When you use a hobby balance charger with high current, it will take the cells way over 4.2 briefly, and wait for them to settle back to 4.2, and then deem the pack charged. It has to go over 4.2 to get the charge in (you need higher voltage to charge).

Even with a perfect balance charge, with the above example, I guarantee the pack would balance charge, and then settle back to 4.2, 4.2, 4.0 after 20 minutes of rest. 

With "brick" charging you are effectively trickle charging. Your pack will hit max voltage, and the charger will back off, and only resume when it drops below full charge. If you have a dead cell, then yes, it will overcharge the remaining cells, but really, how often does this happen?

Incidentally, I'm talking about cells in series, any cells you have in parallel balance themselves though natural physics. That's been discussed to death and proven on many RC forums.
```

---
## \#23 Posted by: TarzanHBK Posted at: 2017-02-16T09:40:09.314Z Reads: 207

```
I see your point if you have long time experience with these kind of things and know how your batteries behave.
BUT: There are a lot of people here who never had any contact with batteries before and ask questions like "help! why is my pack at 23V, it´s a 6s 22,2V?". So i wouldn´t tell someone like that, that it´s ok to throw a brick on their battery and charge without anything else!
An other point: You mentioned a 16000mah and a 24000mah pack, so lot´s of juice!
People build beginner boards with 6s 5000mah and 20c batteries. With a big pack like yours you´re not stressing your pack and the single cells won´t really discharge differently and unbalance. With that small poor 6s 5ah, a fat ass at above 90kg (like mine) and the first hill you encounter, you throw a massive unbalance in that pack! Then people go home soon after the ESC cuts out here, scream at the battery manufacturer what a sht they build and charge their pack again. No time to let the battery rest a bit and you have huge unbalances! 
If you just use a brick in that case, you´re likely damage them!

So just be safe and only do experienced stuff if you now your parts and how they behave :slight_smile:
```

---
## \#24 Posted by: PXSS Posted at: 2017-02-16T12:59:01.994Z Reads: 203

```
[quote="RogerD, post:22, topic:17765"]
At the top of the charge, as the cells approach 4.2v each, the total pack voltage approaches (for 3s in this example) 12.6 volts. Lets say one cell is a little behind. You have 4.2, 4.2 and 4.0v. That's 12.4, so the charger slowly trickles in power until it sees 12.6v. This will either happen as the cells go 4.3,4.3,4.1, for example, = 12.7 volts. The charger stops. The pack settles back to 4.2, 4.2, 4.1. This equals 12.5v so the charger puts a little more in. It keeps doing this until the pack settles at 12.6 v at rest. This will happen when all the cells settle at 4.2 volts, or you end up with something like 4.3, 4.3, 4.0. (this pack, I would bin)
[/quote]
What you are describing would never happen. I'm going to break it down a lot here so bare with me. 

Same 3S scenario with your brick on what actually happens. 

Your brick charger does not charge to 4.2v per cell to be exact they usually have a tolerance of 0.05V per cell and most of these usually overcharge. 
So lets assume your brick actually charges to 12.7V. Your charger is also not capable of charging extremely small currents. Most bricks shut off at 5-10% of the current rating. This is because if you didn't have a shut off, your cell would be on charge for an infinite amount of time and they would blow. 
So another assumption is that your laptop charger shuts off at 0.1A if its a really good one.
So your charger will over charge to 12.7V at 0.1A. At no load this could absolutely mean exactly 12.6v for the pack but you already overcharged them for however many hoirs they were at 12.7. 

You have a cell that is 0.2v behind all others while charging. This suggests that it's internal resistance is lower than the others. If you have a decent hobby charger, it actually tells you the internal resistance of each cell in a pack. This is important because internal resistance is really the measurement of health. The lower, the better and no two cells will ever have the same. If you buy from a good lipo brand (Thunderpower) you can call them and ask them to send you cells that are closely matched. You have no control over this if you buy from hobbyking. 

So lower internal resistance is good, high is bad. This is because when you apply a current through the batteries, your voltage sag or rise (discharge and charge respectively) is equal to current x internal resistance. The heat generated is current ^2 x internal resistance. So for a higher internal resistance, you get more voltage sag and more heat. 

Back to your example, the cell that is 0.2V lower while charging is actually in better health than the other two and not the other way around. So you stick them in the charger and lets say it stops at 12.7 and your cells settle at 4.0, 4.2, 4.2 after a while. 
IF (thats a big if) this total voltage of 12.4V is under the charge trigger, then the brick will start charging again, otherwise it will leave them there. So they start charging again, now only at 0.1A, the cell with lower ir will increase voltage slower than the other two because of v=i*r. So your battery reaches 12.7 and the current dips below 0.1A so your charger stops. 
Your battery now settles at 12.6, your cell voltages will NEVER (physically impossible) be better than 4.133 4.266 and 4.266 (This would be the scenario where your cells have perfectly matched internal resistance but one was simply at a different point in the charge cycle which is unrealistic). 

Now if you have quality cells and they have a .01V spread more than likely they also have a good spread of internal resistance values and they will not go out of balance over night. This happens over tens of cycles and if you like me have lots of batteries, you really don't cycle them all that much. The only cells I've cycled more than a hundred times are cells that are a few years old and belong to specific aircraft. 
The problem arises when you don't have quality cells and your voltage spread is larger as these could have large varying internal resistances which would go out of whack in a matter of a few cycles. 

But even then, if you have good cells and you never check them. They will go out of balance and your board is now a serious hazard under your feet. 

As far as balance chargers charging above 4.2V. You're wrong. A good balance charger will charge to whatever voltage you tell it to and the batteries should settle at a voltage lower than this. If you are doing it another way then you're doing it wrong. I don't have any more time to explain but hopefully later today I can explain this to you

I hope you find this informative.
```

---
## \#25 Posted by: RogerD Posted at: 2017-02-16T13:47:38.082Z Reads: 161

```
I have an Astro 109 charger from back in the days, which I still use. It's not a balance charger- they didnt exist then. It "pulses" in charge towards the end, pushing the cells way over 4.2, then waits a second or so for them to settle/rest, checks the voltage, and then repeats, until the cells stay at 4.2 for at least "x" seconds (around 10 I believe). I use thsi charger as my skateboard "fast charger". Whereas my modern balance charger (which I use indoors) reduces the current as the cells approach full.

I'm currently charging my board with the "brick". I'll post what the cells do as the charge progresses today.
```

---
## \#26 Posted by: RogerD Posted at: 2017-02-16T14:02:07.155Z Reads: 166

```
Checked it.

Pack 1:
4.18
4.18
4.18
4.17
4.18
4.19
Pack 2:
4.12
4.11
4.21
4.21
4.21
4.22

Both packs are 25.08 each in total (charged in parallel), So that's obviously the limitation of my brick charger. (i.e. a 1.2volt deffieciency)

Pack two has two cells that are 0.08 and 0.09 volts out (from 4.2v) and the other cells have been overcharged by 0.01v.

I can live with that, and that's the point. I've used the packs loads. lots of 15 mile runs last year, never balance charged. Simply plugged into the brick charger.

As a final test, I'll now balance charge them and see how they fair, particularly pack 2. Though as I say, I'm happy to live with 0.09v difference on a couple cells.

p.s. PSXX I did indeed find your post informative.
```

---
## \#27 Posted by: RogerD Posted at: 2017-02-17T13:54:25.252Z Reads: 158

```
Ok, balance charged both packs (although this thread wasn't really meant to be about balance charging, more about BMSs).

I left the packs overnight to settle back to rest.

Pack 1:  (pretty much the same, just dropped 0.01 here and there at rest

Brick charger  --      Balance charged

4.18         --           4.17
4.18         --           4.18
4.18         --           4.17
4.18         --           4.18
4.17         --           4.16
4.18         --           4.16
4.19         --           4.17

Pack 2:  (again, pretty much the same, dropped 0.01 here and there, and first two lower cells have gained 0.02v each)

Brick Charger   --   Balance Charger

4.12         --          4.14
4.11         --          4.13
4.21         --          4.17
4.21         --          4.20
4.21         --          4.19
4.22         --          4.20 

So all in all, the balance charging made sod all difference......
```

---
## \#28 Posted by: PXSS Posted at: 2017-02-17T14:46:10.559Z Reads: 154

```
I haven't heard of that charger, but I've also only been seriously involved in RC for about 4-5 years.
I have 4 iCharger 308 Duos, 1 iCharger 4010 Duo, A hobbyking Reaktor and some SkyRC B6s. 

All of my iChargers will charge batteries within 5-6mV of each other when balancing. The reaktor has a 10mV ish range while the B6 has a 20mV range. I suspect your balance charger isn't that great. 

I've charged 8S batteries that are way out of balance and brought them back within 5mV
```

---
## \#29 Posted by: Hummie Posted at: 2017-02-17T17:22:59.887Z Reads: 156

```
I can't find what about lithium cells makes them not capable of trickle charging at the end of a charge...if it sits on a 4.2 for more than hours. I read about how ideally there's four charging stages starting w a trickle, and then cc, then cv, and then it shuts off. Is it due to using a switching charger or truly the chemistry and if the chemistry why?  I think it's the chemistry as I've seen linear power supplies that use a timed cut off when at full charge
Edit
Seems "floating" lithium isn't a problem and it's just the high voltage the cell is at from this article
http://www.electronicsweekly.com/market-sectors/power/float-charging-lithium-ion-cells-2006-02/
```

---
## \#30 Posted by: PXSS Posted at: 2017-02-18T00:18:57.929Z Reads: 152

```
I can lead you to the proper articles as of why. Not right now though as it's date night. If I dont post by the AM, remind me. 

@Hummie 
I have a few minutes so I'll try to explain it really quick. It has to do with the chemical reaction. Charging the battery is an exothermic reaction so this means that heat is released during charging, not only that but you also have electrical heating effects on the battery, that is the heating due to I^2*R.
The chemical reaction on lithium batteries is also not 100% reversible which is why you lose capacity over time. The non reversible part of the reaction creates some kind of oxide within the cell, (I don't remember exactly what it is but it is not usable) this oxide causes the internal resistance of the cell to increase which increases heat generated, the reaction produces more oxides at voltage states and high temperatures. More oxides -> more heat -> more oxides. This is what battery engineers call thermal runaway. The more time your batteries spend at 4.2V, the more oxides you generate, that is why a lot of RC guys only charge their batteries before they fly and dont leave them stored at full charge. 

So you have the whole thermal runaway issue. Above that, the oxides occupy more space within the cell than the electrolyte. LiPo pouches have a constant volume. PV = nRT. That means that if temperature rises within a cell, you have to increase the volume or pressure. You have a shrinking volume since the oxides occupy space and your temperature is rising. The only other variable is pressure (n is the number of molecules and R is a specific constant). So LiPos puff and eventually blow up. I'm not sure which of the chemicals ignites with oxygen but yeah. LiPo fire yayyy. 

Li-Ions have the vents to release gases and delay the explosion but eventually they also catch fire. 

I think batteryuniversity.com has some of this info but most of it is explained in scholar articles.
```

---
## \#31 Posted by: Hummie Posted at: 2017-02-18T02:15:19.450Z Reads: 138

```
some articles tell that its a sure fire if you were to trickle charge lithium.   All regulated chargers will shut off, but some after even an hour or two.  If the only reason that floating the cells on a charge of 4.2 is bad is the oxides or plating or whatever is happening at that high voltage then it wouldn't be fire worthy no?  I charge to 4.2 and leave my cells around and while they may sink to 4.15 or something quickly, even if I charged them to sit at 4.2 it's not asking for a fire.  Isn't there some other reason articles scream fire if you try to float lithium?  They dont even state that it's a high voltage.  I'd be happy to float at 4.1.
```

---
## \#32 Posted by: benwong Posted at: 2017-02-18T06:01:07.591Z Reads: 127

```
is the title means i can use laptop style charge to charge my lipo direct without BMS? 
i have charge spec 33.6v 3A.
```

---
## \#33 Posted by: RogerD Posted at: 2017-02-18T11:29:06.164Z Reads: 134

```
Benwong, that's exactly what I am saying, and it's exactly what I do with 4 boards in total.

Your numbers suggest 8s lipo pack. 2 to 3 amps is common for brick chargers.

All you have to do is just keep an eye on your packs once in a while.

With balance charging (or a BMS board), you are going to find out of a cell has dropped significantly when you do the charge, because the charger will come up with an error, or take forever.
Without balance charging you won't get the warning. It's not a common problem, but it can happen.

For me, I would know if I has a cell problem because the boards performance and range would drop significantly.

I "brick" charge mine most of the time, and once in a while I balance charger them as a kind of "service". To keep an eye on them.

If you dont have a balance charger to check them once in a while then a simple lipo checker/alarm like this: http://www.ebay.co.uk/itm/RC-Lipo-Battery-Low-Voltage-Tester-1S-8S-Buzzer-Alarm-Checker-Test-LED-Indicator-/252401918078?var=&hash=item3ac453a07e:m:md6n6fjcqhfTOJGZxs7q_gA       is a great idea - then you can keep an eye on things, when the board is in use, and when it is charging. It just plugs into your battery balance plug.
```

---
## \#34 Posted by: benwong Posted at: 2017-02-18T11:34:58.646Z Reads: 130

```
thank for your advise~~ 
finally i understand the "brick" that you all mention~~ :joy::joy:
<img src="/uploads/db1493/original/3X/e/1/e1e81da6cf61edf2a723fa0f3f3c7846db1e8cb0.png" width="398" height="400">
here is the "brick", actually not that big and heavy~~ haha. 

i am using this for changing.. withBMS. 

:blush::blush:
```

---
## \#35 Posted by: RogerD Posted at: 2017-02-18T12:56:13.530Z Reads: 126

```
Indeed :-)
```

---
## \#36 Posted by: PXSS Posted at: 2017-02-18T13:41:02.277Z Reads: 129

```
http://batteryuniversity.com/learn/article/charging_lithium_ion_batteries
```

---
## \#37 Posted by: PXSS Posted at: 2017-02-18T13:48:03.459Z Reads: 125

```
"Li-ion cannot absorb overcharge. When fully charged, the charge current must be cut off. A continuous trickle charge would cause plating of metallic lithium and compromise safety. To minimize stress, keep the lithium-ion battery at the peak cut-off as short as possible."
```

---
## \#38 Posted by: RogerD Posted at: 2017-02-18T15:19:24.731Z Reads: 127

```
No one is suggesting a trickle charge PXSS. I said it is "like trickle charging" in as much as it is low current.

The brick chargers won't trickle charge. They charge to 4.2v per cell then stop, only resuming if there is a significant drop.
```

---
## \#39 Posted by: Hummie Posted at: 2017-02-18T16:24:39.663Z Reads: 120

```
I think he's responding to my questions about the safety of "float" charging (having the cell constantly exposed to a certain voltage).  

 you can "float" charge to 4 volts with lithium and be fine.  It's just the danger of going over 4.2 thats the danger.
```

---
## \#40 Posted by: PXSS Posted at: 2017-02-18T16:35:51.324Z Reads: 115

```
The plating is dangerous @hummie. It increases the pressure inside the cell and the internal resistance goes up. At a certain point, your cells go into thermal runaway and there isnt a way to know when this will happen without closely monitoring temps and internal resistance
```

---
## \#41 Posted by: Hummie Posted at: 2017-02-18T16:35:57.833Z Reads: 113

```
a "brick" charger, as you're calling it, is still a regulated power supply and will cut off the cell at 4.2 even though the cell has been exposed to a higher voltage to increase current.  If it didn't have this cc feature it would take a long time to charge

yes.  pxss.  but plating won't happen if it's not getting to the high voltage and it can sit on that.  float
```

---
## \#42 Posted by: PXSS Posted at: 2017-02-18T16:42:37.312Z Reads: 119

```
@RogerD 
By now I think I've explained enough to show you why it's dangerous to use a brick charger without BMS. 
It is reckless and unsafe to give advice to people without any knowledge on the subject to use this method as they will most likely not monitor their voltages and wont know how to recognize if they have a bad cell.
We as a community are responsible for each other's safety as our whole community will suffer if someone dies and legislation makes what we do illegal
```

---
## \#43 Posted by: Hummie Posted at: 2017-02-18T16:45:20.670Z Reads: 121

```
 it's not that complicated to bulk charge using a brick or even an unregulated supply (more dangerous) but as long as whoever does it is aware that they are charging multiple individual cells that shouldn't go above...maybe 4.3 on the charger, and dont go below 3 volts in use, then that's all there is to it.

(and when using unregulated making sure the current isn't too high on initial charging)

@benwong  get a battery medic like device for balancing and get a multimeter.  cheap stuff and necessary if you're going to go that route without a bms or a balance charger
```

---
## \#44 Posted by: PXSS Posted at: 2017-02-18T16:50:37.184Z Reads: 122

```
I just feel strongly against giving strangers unsafe advice. You're putting someone else at risk. I dont really care if you understand the risks and decide to ignore them. Its just morally wrong in my opinion to put someone else at risk. This is the same issue I had with Devin's advice if you remember @hummie
```

---
## \#45 Posted by: Hummie Posted at: 2017-02-18T16:59:20.268Z Reads: 127

```
but is bulk charging inherently less safe if you're monitoring the charge and balance?  In my mind, when charging, I'm more safe as I'm aware of what's going on as apposed to relying on something else that could break.   And that's why I brought up the temp sensor: I think with it watching if anything were to get hot while riding I'd be safe during discharge too...safe enough in that if anything were to be way out of balance it will get hot when discharging and I could be aware that way before runaway.

the big benefit to not relying on the bms I think would be awareness and I think the large majority of people with a bms dont know the health of individual cells and could be riding at a much reduced output due to a single cell holding them back as that cell shuts down the discharge.  

devin felt he was improving safety actually and felt the acceleration curve needed to be consistent and smooth for that to happen.  fair enough.   a danger to the vesc... I haven't heard of enough people running at 200 motor amps to know.  Maybe with the 6 people will be emboldened and we'll find an answer to how it does.  the 6, being more robust, ..I think most people will end up at 200 motor amps for the increased performance
```

---
## \#46 Posted by: benwong Posted at: 2017-02-19T04:06:46.877Z Reads: 121

```
hey guy, 
any idea how to solve lipo unbalanced cell? 
i try to discharge and charge, result still the same. cause by overdischarge. 
1. 3.80
2. 4.20
3. 4.20
4. 4.20

before this issue, i ride as normal. last night riding half way 80% battery suddenly drop till 20%, then no more power, back home and check, first cell left 1.8v. is my lipo dead?
```

---
## \#47 Posted by: Hummie Posted at: 2017-02-19T04:15:00.922Z Reads: 115

```
snip it off and solder on another of the same if you have it.
```

---
## \#48 Posted by: benwong Posted at: 2017-02-19T04:16:15.103Z Reads: 116

```
too bad i don have~~ :disappointed_relieved:
```

---
## \#49 Posted by: Hummie Posted at: 2017-02-19T04:16:46.963Z Reads: 118

```
get a vesc and set the low voltage limit
```

---
## \#50 Posted by: RogerD Posted at: 2017-02-19T10:46:24.628Z Reads: 115

```
PSXX,  No, you have not "explained" that not using a bms is dangerous. You have " given your opinion".

In my opinion,  you are wrong. My opinion is that having a BMS is useful, and helpful, but it is not "needed" Hence this thread has "NEED" in capitals.
```

---
## \#51 Posted by: RogerD Posted at: 2017-02-19T10:47:46.219Z Reads: 114

```
O'r any esc for that matter. Set the low voltage limit and don't ignore it ( restarting esc to get extra mile out of it). 

Your pack with 3.8 and 4.2 v cells is for the bin I'm afraid :-(
```

---
## \#52 Posted by: Hummie Posted at: 2017-02-19T15:33:53.542Z Reads: 111

```
snip it off and run a cell lower and adjust the low voltage cut off.
```

---
## \#53 Posted by: Pedrodemio Posted at: 2017-02-20T01:51:06.265Z Reads: 115

```
I'm with @PXSS on this one

As you say, it's needed for a board to function? no, if you know what you are doing and know how things work

The problem is as this site and the numbers of  people with interest in eboards grow, the interest shifts from enthusiasts to a lot of people that have no idea whats they are doing

Is totally possible that someone has no idea that you have to monitor the cells voltage or has no idea that they have to be close to each other. If you spread the knowledge that the BMS is a must, people who have no idea what the are doing has a higher change to put one on their board and that can save some damage or worse.

For me if in a thousand eboarders, one has a  big fire on explosion or a room full of smoke that didn't happen thanks to the BMS, then all the discussion and insisting to use one was worth

The truth is, you can't use a board without a BMS, the options is you buy a electronic board that we call a BMS, or you go deeper and become the BMS by always measuring cells voltages and other safety precautions
```

---
## \#54 Posted by: Hummie Posted at: 2017-02-20T05:41:06.503Z Reads: 119

```
as you say at the end either buy a bms or become one.  
  I treat anyone who's making a board as an adult and tell them info as such.   State the danger,  simplify the knowledge, and trust that people will make the right choice.  no point communicating on here if the info is dumbed down for supposed nubies.
```

---
## \#55 Posted by: PXSS Posted at: 2017-02-22T02:25:20.974Z Reads: 115

```
Not an opinion. Fact. Your charger is more dangerous. 

You are mistaken in thinking you know more than I do about LiPos and Liions.  My company owns thousands of LiPos. Most in good health. Some not so much. I am required to know everything there is to know about batteries and I spend hours upon hours a day doing research and learning. 

These are all bad. There's about 12 more ammo cans full in the back. 

<img src="/uploads/db1493/original/3X/3/6/36885013684dbbb9fb17fedf8de6889cecb117bc.jpg" width="375" height="500">
```

---
## \#56 Posted by: RogerD Posted at: 2017-02-22T21:56:09.696Z Reads: 117

```
OK , I give in, like I said, it's advice, and you dont' have to take it.

Having dozens of cases of bad cells in ammo cases, through your line of work, is not exactly an accurate reflection of the average person's exposure to battery accidents, is it now? Really dude. Perspective.

How many people here, for example, can tell me they have had a laptop battery fire?

I'm still willing to bet more people on here have killed/puffed batteries cutting and soldering BMS wires than people have naturally had a lipo disaster.

For the last time, what I have posted is you don't NEED a BMS. OK? It's nice to have , sure, but you don't NEED one. I have never used one, and I'm still here. As have many, many people. I am the balanced opinion on the other side of the overly protective/safety side of the argument.
```

---
## \#57 Posted by: RogerD Posted at: 2017-02-22T21:57:03.079Z Reads: 117

```
[quote="Pedrodemio, post:53, topic:17765"]
If you spread the knowledge that the BMS is a must
[/quote]


But it's NOT a must, so you are spreading misinfomation. No matter how well you mean.
```

---
## \#58 Posted by: Hummie Posted at: 2017-02-22T22:06:40.409Z Reads: 114

```
the new lithium chainsaw from harbor freight is torn down by "less than zero" professor at MIT and it doesnt have a bms!  and no way to balance!  you can read the teardown when less than zero's page starts working again.  not lipos but lithium ion 18650 but still...no bms and no way to balance..now that's dangerous
```

---
## \#59 Posted by: Alanhunt123 Posted at: 2017-03-01T14:48:14.033Z Reads: 116

```
I agree that a BMS isn't necessary, BUT anyone who doesn't use one has to accept the responsibility of checking up on their cells periodically or balance charging. If you aren't balancing, it's a good idea to at least check the individual cell voltages before and after charging.

I just built a nice 10s4p pack that I charge to 4.1  for longevity purposes. I'm not using a BMS because I know how to take care of my cells. I'll balance charge maybe once out of every five charges and it should be fine, since I'm not charging to 4.2.

However, I feel like @RogerD should have been more explicit in his original post that in order to do what he is doing, you need to do your homework and be knowledgeable about lipos before using his technique. And unfortunately, the trend on this forum is beginners tend to use the cheapest lipos they can find on hobbyking, which simply do not stand up to many unbalanced charges without the cells going too much out of whack. Been there and done that with Multistar batteries.
```

---
## \#60 Posted by: guyguy Posted at: 2017-03-01T18:29:44.153Z Reads: 111

```
risk = probability * amount of harm

I think most of your argument centers around how low of a probability unbalanced lipos are but you're overlooking potential harm as a component of risk. From a risk perspective, comparing laptop batteries / RC batteries to the most of the batteries on this forum isn't equivalent. 

If a small battery on a laptop blows the harm is relatively small  and I think we can assume the cells becoming unbalanced is of low probability. 

With e-boarding you have much larger packs which makes the potential harm go way up. Even if the probability of cells becoming unbalanced stays the same as it is in a laptop the risk actually increases because the potential harm has increased due to the battery size. 

That's why a truck tanker carrying hazardous material is treated very differently than a truck carrying water. The probability of each truck getting in an accident is about the same but the potential fallout is very different so many more precautions are taken when transporting hazardous materials.
```

---
## \#61 Posted by: Jammeslu Posted at: 2017-03-06T14:48:45.647Z Reads: 110

```
hi, just wondering, Im going to buy a bms that supports a maximum of 60A, bet lets say if you buy a esc you buy higher ampridge than what you really need so do you do the same with bms, and if bms limits the current flow to the bms would that lower the performance that i will get in speed if it limits my current flow, I'm using 6s 5000mah, 120 esc, sk3 245 or 190kv motor
```

---
## \#62 Posted by: Hummie Posted at: 2017-03-06T20:58:02.906Z Reads: 108

```
wont limit the speed really just torque.  you'd want a bms that can do above what you plan to draw from the battery as you say, if you're incorporating it while discharging
```

---
## \#63 Posted by: Ackmaniac Posted at: 2017-03-06T23:28:54.719Z Reads: 110

```
Just for clarification about laptop battery packs. The all have a BMS. Mostly directly included in the battery pack.
```

---

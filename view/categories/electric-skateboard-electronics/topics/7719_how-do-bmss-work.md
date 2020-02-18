# How do bms&rsquo;s work?

### Replies: 72 Views: 5399

## \#1 Posted by: evoheyax Posted at: 2016-08-16T01:31:30.367Z Reads: 466

```
I think this is a good topic for the community to understand better. Having just built my first pack with a bms, there's somethings which are unclear to me, and I'm sure there's other people who feel the same way.

What I do know:
- The **B**attery **M**anagement **S**ystem's job is to balance cells while charging and prevent any parallel groups of cells from being over discharged.
- This balancing is done through a balancing cable, which is connected to the negative end terminal of the battery, then every positive in the battery, including the positive end terminal.
- You can discharge around the bms while still charging through the bms by splitting the battery negative input (usually marked B- on the bms) before the bms, essentially putting the bms and esc's in parallel. This allows you to draw more amps while discharging than the bms supports. Since lower amp bms's are smaller and cheaper, you can save money and space doing this, but risk over discharging a group of cells in parallel.

How does the bms balance? My understanding is that as the cells are charged, when a cell is fully charged, through the balance cable, the bms discharges the cell. The cell is essentially being charged and discharged at the same time, in equal proportion to keep it at 4.2v, while the rest of the cells not at 4.2 are charged.
Is this view correct?

The other part I'm confused about is there's only negative terminals on the bms (besides the balance port). The negative of the charging port (input), the negative of the battery (input) and the negative discharging (output). It's not like a power switch where it runs both negatives and positives through the pcb before it is outputed. 
Why is this so? How does this work?

Anybody with knowledge wish to shed some light on bms's.

Any other questions? Let put together all the info we have on bms's so that we can turn this topic into a topic full of all the info anyone would need to know about bms's.
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-16T01:42:49.658Z Reads: 423

```
AFAIK BMS charges cells to a set voltage (about 4.15v depending on bms) then continues charging with a smaller balance current until it reaches 4.2v. it doesn't actually start balancing until it hits that ceiling.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-08-16T03:13:35.914Z Reads: 398

```
So if a cell becomes largely unbalanced, it won't be able to fix it? I just tried to balance charge what used to be a space cell before I tore it apart and soldered it up in the shape I needed and added another p. The problem is, they didn't balance. My problem could be that some of the cells I used were at 3.6, others at 4.1. Since I didn't have a way of charging the new cells, I figured it would balance out when I charged them, but they didn't.
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-16T03:42:28.912Z Reads: 381

```
Are the series cells not balancing or the parallel? Once you hook up batteries in parallel they'll passively balance out and conform to a voltage.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-16T03:56:32.673Z Reads: 359

```
The series cells are not balancing. I checked my balance plug that goes into the bms, all the voltages are in the correct order. If I go cell by cell, I get 4.1, 4.1, 4.1, 4.2, 4.2, 4.2, 4.2, 3.6, 3.6, 3.6. Not even the 4.1's balanced. I looked up dozens of diagrams, and confirmed I hooked them up correctly. Does it matter if they are hooked up to vescs or not? Cause right now, they aren't hooked to anything other than the bms and charging port.
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-16T03:58:50.095Z Reads: 343

```
So they're all hooked up to to a 10s BMS right? If so, plug in the charger and leave it charging there. Don't unplug to check until the charging light goes green which indicates a full balanced charge. Right now your pack is at 39.9v. It'll continue to balance until your pack is at 42v, it just might take a bit of time since the balance current is lower than the normal charge current.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-08-16T03:59:43.707Z Reads: 325

```
The thing is, it went green... Does it still balance once it goes green?
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-16T04:03:05.098Z Reads: 320

```
hm are you using a 42v charger? Chargers are pretty simple and if it's a 42v charger it should only go green when it hits 42v. I'd get a multimeter to read the voltage of the charger when it's plugged in.
```

---
## \#9 Posted by: evoheyax Posted at: 2016-08-16T04:04:02.801Z Reads: 317

```
Let me read it, but yes, its 42 volt charger. Came with my space cell.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-08-16T04:04:55.502Z Reads: 312

```
42.10 volts coming from the charger. Should I just leave it plugged in? I'm afraid on over charging some cells if it's not working right for some reason.
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-16T04:06:39.187Z Reads: 304

```
It should only green once your pack has balanced out to 42v as well, which means something is broken or not reading correctly. Since it only turns green at 42v this means green = balanced. Your current series voltage is 39.9.
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-16T04:07:14.182Z Reads: 288

```
You won't overcharge the cells unless you weren't on a BMS. each balance lead is set to 4.2v so no current will flow to cells that have balanced out to 4.2v
```

---
## \#13 Posted by: evoheyax Posted at: 2016-08-16T04:08:24.187Z Reads: 272

```
my multi meter says 40.1 volts (I left off some decimals)
```

---
## \#14 Posted by: Pantologist Posted at: 2016-08-16T04:11:56.974Z Reads: 264

```
Just leave it charging. The whole point of the BMS is so you can do that. 

Come back after around 10 minutes and test the cells to see if they balanced way up to 4.2v or not. Balance charging takes awhile.
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-16T04:14:05.188Z Reads: 261

```
Right, try leaving it plugged in for an hour or so and check voltages again.
```

---
## \#16 Posted by: evoheyax Posted at: 2016-08-16T04:26:25.925Z Reads: 258

```
So i just checked again. all cells increased. 4.216 now is my max cell, up from 4.205
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-16T04:28:29.683Z Reads: 260

```
Cool, low cells too? If everything's hooked up right, just keep it on the charger until all cells balance
```

---
## \#18 Posted by: evoheyax Posted at: 2016-08-16T04:29:32.478Z Reads: 257

```
yes, low cells also went up. I want those 4.2 guys to stop charging though...
```

---
## \#19 Posted by: Jinra Posted at: 2016-08-16T04:29:53.567Z Reads: 254

```
they will, the BMS protects them from overcharging.
```

---
## \#20 Posted by: evoheyax Posted at: 2016-08-16T04:31:07.835Z Reads: 254

```
I know it should, but I'm worried there might be something wrong with the bms. It was a working bms and pack when I ripped it apart.
```

---
## \#21 Posted by: Jinra Posted at: 2016-08-16T04:31:58.904Z Reads: 243

```
It's dependent on BMS, but take a look at the spec sheet [here](http://www.batterysupports.com/36v-37v-42v-10s-100a-10x-36v-lithium-ion-lipolymer-battery-bms-p-390.html)

You'll see that it has an over-charge protection which is accurate to +/- .05v. Some BMS's might have a wider tolerance.

You can check the balance lead directly to see how much voltage it's giving off. It will never up the voltage on your cell higher than that.
```

---
## \#22 Posted by: kyo Posted at: 2016-08-16T05:27:42.628Z Reads: 242

```
This video has a good explanation of how bms work.

https://youtu.be/MZyY1dpka7c
```

---
## \#23 Posted by: evoheyax Posted at: 2016-08-16T16:00:38.182Z Reads: 225

```
So I left it charging for an hour. It didn't charge anything anymore. So the cells are still unbalanced. According to that video (what I've read before), the bms sheds the voltage of the 4.2 cells so that they lose while the gain, neutralizing each other. But where does that discharge current go?
```

---
## \#24 Posted by: Jinra Posted at: 2016-08-16T16:02:06.569Z Reads: 212

```
Have you checked all the balance leads to make sure they're giving off 4.2v?
```

---
## \#25 Posted by: evoheyax Posted at: 2016-08-16T16:03:28.334Z Reads: 216

```
While it's charging? I've checked them all one by one while not charging and the voltages I saw are what I posted last night.
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-16T16:04:55.023Z Reads: 206

```
I mean not for the cells, but from the BMS itself. Unplug the balance JST and probe each balance lead port to see check the voltage
```

---
## \#27 Posted by: evoheyax Posted at: 2016-08-16T16:06:22.932Z Reads: 199

```
yes, that's what I have always done. That's how I came up with the voltage of each cell.
```

---
## \#28 Posted by: Jinra Posted at: 2016-08-16T16:07:28.393Z Reads: 204

```
Again I don't mean checking the voltage of the cell, but the voltage on the BMS. If you're saying your getting 3.9 on some of the BMS balance leads then it sounds like the BMS is malfunctioning.
```

---
## \#29 Posted by: evoheyax Posted at: 2016-08-16T16:11:03.927Z Reads: 201

```
I get nothing. It doesn't show any voltage between pins of the balance port without being plugged in. And I don't see why it would, there's no positive connecting the battery to the bms. The balance leads are that positive. So why would I get any voltage like this?
```

---
## \#30 Posted by: Jinra Posted at: 2016-08-16T16:24:00.504Z Reads: 196

```
unplug the JST and measure from the balance port
```

---
## \#31 Posted by: evoheyax Posted at: 2016-08-16T16:43:02.863Z Reads: 189

```
I get nothing...
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-16T16:44:25.525Z Reads: 186

```
is it plugged in?
```

---
## \#33 Posted by: evoheyax Posted at: 2016-08-16T16:47:44.179Z Reads: 184

```
With the JST unplugged, and the negative from thebattery plugged in, I get nothing, because the circut is incomplete. Theres no positive going into the bms. The only positive meant to go into this bms is balance wires. Which is why I'm confused as to how I would get any voltages without the balance plug plugged in.
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-16T16:53:34.873Z Reads: 181

```
you can measure it with a multimeter, probe the positive to balance lead and negative to B- on the BMS.
```

---
## \#35 Posted by: evoheyax Posted at: 2016-08-16T17:00:30.547Z Reads: 184

```
I did that, but I'm getting nothing.
```

---
## \#36 Posted by: Jinra Posted at: 2016-08-16T17:10:45.588Z Reads: 180

```
Darn, thought that would work. Have you tried with your battery turned on? but balance leads not plugged in?
```

---
## \#37 Posted by: Nordle Posted at: 2016-08-16T17:17:35.800Z Reads: 187

```
[quote="Jinra, post:4, topic:7719"]
Are the series cells not balancing or the parallel?
[/quote]

How can parallel cells not be balanced?
:anger_right::skull_crossbones:
```

---
## \#38 Posted by: Jinra Posted at: 2016-08-16T17:17:54.939Z Reads: 189

```
bad cell

10 chars
```

---
## \#39 Posted by: evoheyax Posted at: 2016-08-16T18:36:27.814Z Reads: 187

```
The battery is not plugged into anything, including a switch. Was using dyi's switch, but it was broken. So right now, it's not hooked up to anything. It's essentially always on. Does it matter if I removed the switch on the bms? could hat affect anything? cause I never had to turn it on to charge. But could having remove it caused this?
```

---
## \#40 Posted by: Nordle Posted at: 2016-08-16T19:22:01.403Z Reads: 183

```
i still don't understand how parallel cells can not be balanced, even if they are bad
```

---
## \#41 Posted by: lowGuido Posted at: 2016-08-17T01:46:23.218Z Reads: 171

```
Because they cant be isolated from the cells they are in parallel with. 
A bad cell in parallel with a good cell will drag the good cell down to its level.
```

---
## \#42 Posted by: Nordle Posted at: 2016-08-17T07:13:52.197Z Reads: 174

```
parallel = balanced :punch:
```

---
## \#43 Posted by: lowGuido Posted at: 2016-08-17T10:40:09.497Z Reads: 169

```
not with the cell in series with them though.
```

---
## \#45 Posted by: bartroosen12 Posted at: 2017-07-23T13:28:56.483Z Reads: 138

```
Hi everyone, I really hope someone can help me with my easy question because I'm getting very confused.

I have a 6S2P Lipo pack connected to a bms, everything worked great but recently I the cells were dicharged to much so 2 cells in parallel broke so I replaced them today.

The other cells are fully charged 4,2V but the 2 other cells are 3,7V. If I charge them with my normal 25,2V charger all the other cells charged until 4,25V so I tought damn they will be overcharged so I stopped charging while the ''replaced'' 2 cells are 3,9V.

So now I'm charging them seperate but my question is does a bms always balance the cells?
Also when the charger isn't plugged in?
I thought a bms also balances the pack when no charger is connected but after 10h without the charger the batteries were still the same 4,25V and 3,9V.
```

---
## \#46 Posted by: TowerCrisis Posted at: 2017-08-07T02:45:32.092Z Reads: 134

```
Just stumbled on this thread, hope this information's still useful.

A BMS has a very limited ability to balance cells. In the specs, it will give a rated "balance current". This is the current it can use to charge or discharge individual cells when charging or in use. It's usually around 500mA. To charge a 10000mah cell at this current, it would take 20 hours. 

That's why BMS's should be installed with equalized cells, they can only account for very little variation in battery voltage. The 500mA is barely anything in comparison to the 2 or 3 amps we output from the chargers.
The charge current just affects the overall current on an individual cells level. So when charging a pack from a 2A charger, the cells will charge at 2A if they are in sync with the other cells, 1.5A if they are near full, and 2.5A when undercharged. When discharging the same effect is achieved to keep cells in sync. The small amount of current variation is why a bms could possibly overcharge a cell if it started with too high a voltage.

Sorry if this is a rant, formatting is hard on mobile :P
```

---
## \#47 Posted by: bartroosen12 Posted at: 2017-08-07T11:30:55.873Z Reads: 120

```
Ooh thanks man! Very useful for me :)
I was just a bit concerned that I broke my bms due the undervoltage of a few cells.
```

---
## \#48 Posted by: evoheyax Posted at: 2017-08-07T15:51:50.611Z Reads: 119

```
Thank you for this, very useful information that I had yet to find. I tried multiple bms's with no luck. But I was trying to balance a pack of cells that where 3.8 and 4 volts. Must have just been too much.

My only concern is do you know why it would keep charging a cell past 4.2 volts? My issue with the bms's I tried was it took that 3.8 cell to 4.2 and that 4 to a 4.4, ecensially, I saw no difference.

Every one keeps using (including enertion now) the bms in parallel with the bms, but so far, it seems like it just bypasses the bms and doesn't actually go through it.
```

---
## \#49 Posted by: Jinra Posted at: 2017-08-07T15:56:12.753Z Reads: 112

```
Only reason I can see is that your BMS isn't hooked up correctly or is flat out defective. FYI 3.8 and 4v isn't too much. I've had cells with a .2-.3 voltage differential and it was able to balance all cells to 4.22v just fine.

Your BMS should have a voltage cutoff celing where, once it triggers, charging for that cell will be disconnected until it discharges to the rated voltage release. Pick up one of the small bestech BMS's I have. I can assist in making sure it's hooked up correctly.
```

---
## \#50 Posted by: evoheyax Posted at: 2017-08-07T16:01:34.729Z Reads: 115

```
Could you link me to the one your using?
```

---
## \#51 Posted by: Jinra Posted at: 2017-08-07T16:03:45.029Z Reads: 121

```
The two I haven't aren't available in 12s, but just take a look here and find one that fits your size requirements.

http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/
```

---
## \#52 Posted by: evoheyax Posted at: 2017-08-07T16:42:12.202Z Reads: 120

```
I have 2 of these: http://www.batterysupports.com/36v-30a-12s-12x-32v-lifepo4-battery-bms-lfp-pcm-smt-pcb-system-p-249.html

How should I modify this so it's in parallel?

http://i1098.photobucket.com/albums/g378/lilianleung/12Slogo.jpg
```

---
## \#53 Posted by: Jinra Posted at: 2017-08-07T16:46:14.440Z Reads: 115

```
You plan to use LIFEPO cells? If so, not sure what you mean.
```

---
## \#54 Posted by: evoheyax Posted at: 2017-08-07T16:58:29.224Z Reads: 108

```
No, wrong one, they all look alike, cause they take 1 picture and use it for all, haha.

http://www.batterysupports.com/44v-48v-504v-12s-30a-12x-36v-lithium-ion-lipolymer-battery-bms-p-268.html
```

---
## \#55 Posted by: Jinra Posted at: 2017-08-07T17:03:42.539Z Reads: 108

```
I think there are parallel adapters for the balance connectors. Otherwise you can combine then yourself by soldering it together.
```

---
## \#56 Posted by: TowerCrisis Posted at: 2017-08-07T17:29:34.643Z Reads: 106

```
Honestly with my latest build, I just took the L and got a high amp rated bms. Being able to charge and discharge through the bms will make it balance cells faster, as opposed to only balancing cells when charging.
```

---
## \#57 Posted by: Jinra Posted at: 2017-08-07T17:31:11.766Z Reads: 108

```
From my experience cells don't drift at all during discharge, so I doubt it'll make much difference, for me anyway.
```

---
## \#58 Posted by: chinzw Posted at: 2017-09-01T18:50:57.589Z Reads: 103

```
Most BMS will balance cells all the time, not only when charging, even if its wired to bypass the bms for discharge. Most cheapo bms (bestech, supower) will overcharge the batteries and balance drain, so balancing only happens when cells are 4.2v or higher.
```

---
## \#59 Posted by: Jinra Posted at: 2017-09-01T18:53:11.783Z Reads: 103

```
No, most BMS's balance at the balance voltage which is near 4.2v. There is no passive balancing besides with individual parallel groups, only when charging.
```

---
## \#60 Posted by: chinzw Posted at: 2017-09-01T18:59:52.437Z Reads: 105

```
@Jinra i've measured it, numerous times. I have a supower, still balancing when the charger is not connected. And the only way to balance to 4.2 is to overcharge and drain with these types of bms.
```

---
## \#61 Posted by: Jinra Posted at: 2017-09-01T19:03:03.055Z Reads: 111

```
How have you tested that it's balancing when charger is not connected? You'd have to drain/charge one parallel group more than others and connect the bms and let it sit there. Supower states on their spec page that balance voltage is 4.2v because this is pretty much how all BMS's work.

<img src="/uploads/db1493/original/3X/4/e/4ed1c210ba0541ea72e0519deefeb8b82b7da272.png" width="690" height="277">
```

---
## \#62 Posted by: chinzw Posted at: 2017-09-01T19:06:02.428Z Reads: 106

```
@Jinra see where it says balance for 4.2+- 0.05v, that's the headroom to drain. The end balance voltage should be 4.2v, that doesn't mean that the voltage doesn't go over that to be able to balance.
```

---
## \#63 Posted by: Jinra Posted at: 2017-09-01T19:08:54.256Z Reads: 112

```
I never disputed that.. I'm saying there is no passive balancing on most BMS. They rely on hitting balance voltage in order to balance charge. Once voltage hits balance voltage it applies balance current (typically small) in order to let other cell groups catch up. However if the balancing cell group hits over-charge protection voltage before they other groups can catch up, it'll cut charging entirely potentially still leaving the pack unbalanced.
```

---
## \#64 Posted by: chinzw Posted at: 2017-09-01T20:50:50.103Z Reads: 111

```
@Jinra yeah, i guess we're saying the same thing in different ways.
```

---
## \#65 Posted by: e.board_solutions Posted at: 2018-02-02T11:21:35.184Z Reads: 97

```
What is the difference between:

over-charged protection: 4.2 +-0.05 V
over-charged release: 4.05+-0.05 V

What is release voltage? :open_mouth:
```

---
## \#66 Posted by: SilentException Posted at: 2018-02-02T11:36:24.874Z Reads: 92

```
Once the BMS goes into overcharge protection mode (cell over 4.2), it will stop the charging process and not charge again until the cell voltage gets less than release voltage.
```

---
## \#67 Posted by: e.board_solutions Posted at: 2018-02-02T11:44:57.672Z Reads: 91

```
And with discharge protection?

If a cel goes below 2.5V(detection voltage) the BMS will cut current until it's higher than 2.9V (release voltage), is that right?

![image|690x72](upload://shWEZr6QZpL6h7usJW16Zt8QFpT.png)
```

---
## \#68 Posted by: egzplicit Posted at: 2018-02-02T11:53:21.571Z Reads: 88

```
Yes 10 char
```

---
## \#69 Posted by: ZackoryCramer Posted at: 2018-02-04T09:12:27.368Z Reads: 79

```
Let me see if I understood this topic. The bms does two things. 
First, discharge cells that have voltage higher than the minimum given this minimum cell’s voltage is lower than the minimum rating, until all balanced.  
Second, discharge any cells with voltage exceeds 4.2(or similar). 

So the bms is as if it doesn’t exist when all the cells are below max rating and above min rating? Are there two minimum v ratings, one for minimum balance trigger voltage an one for minimum discharge voltage? Surly the bms would know when to stop discharging. Will bms get less practical the more cells in parallel u have because it takes much longer to balance them? I am still learning how to properly use a bms. 

Thanks for any comments and response.(no buttboard jokes plz😷😃)
```

---
## \#70 Posted by: krloz Posted at: 2018-02-04T11:08:52.548Z Reads: 80

```
Bms don't discharge when battery is at minimum. That would drain the battery and be dangerous.  When a battery reaches it set minimum the bms cuts power do your esc doesn't drain more.
It does balance when a cell exceeds its maximum. Additionally cutting charge power input also.

Edit. I think I understood you wrong. 
Anyway Very little bms  will active balance cells to keep then the same level when between max and min. Most will just drain power from a cell when going above 4.2
```

---
## \#71 Posted by: tex Posted at: 2019-01-15T21:38:29.231Z Reads: 44

```
what does it mean : Supports Max. Continuing Discharge Current: 30A

http://www.batterysupports.com/44v-48v-504v-12s-30a-12x-36v-lithium-ion-lipolymer-battery-bms-p-268.html

Because i saw many similar BMS, but with different A value, how can i know how many A i need?
```

---
## \#72 Posted by: evoheyax Posted at: 2019-01-15T21:49:12.660Z Reads: 38

```
It's tricky to know exactly how many amps you need because these depend on the motor and configuration of the battery. First you need to figure out how many watts your system will pull. Watts = Amps * Voltage. Totally depends on what kind of power you want.

Many today are putting bms's in parallel with the battery, which yields the balancing affect, but since the current to power the esc's is not going through the bms but around it, you can use low amp bms's and still pull higher amps. On 10s setups, 30a is good for some people. Others run 80a, some run much higher. I run a higher voltage 12s and 200a, but I'm an extreme case. It's hard to say what you will need, since factors like skateboarding riding experience, weight, riding style, and hills all play major roles in your system and what you will need. Even minor hills will draw 4 times as much power as flat ground to maintain your velocity.

Just keep reading about what builds others are doing and things will come together for you.
```

---
## \#73 Posted by: tex Posted at: 2019-01-15T22:38:19.429Z Reads: 27

```
Thanks now it's more clear for me.

i'm planning a new eskate, i think 6S 4P i'm interested in range, and ride on flat street
```

---

# Is this BMS legit?

### Replies: 48 Views: 3805

## \#1 Posted by: michaeld33 Posted at: 2016-07-01T18:06:56.641Z Reads: 301

```
I am wondering if this bms will actually work for a 10S4P battery pack. Seems a little cheap considering other BMS boards for a 10S setup can be up to $50. http://www.aliexpress.com/store/product/New-Battery-Protection-BMS-PCB-Board-for-10-Packs-10s-36V-Li-ion-Cell-max-30A/939205_32574042165.html
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-01T18:11:34.177Z Reads: 300

```
Output current is a bit low, might not work well when current demands are high.
```

---
## \#3 Posted by: lowGuido Posted at: 2016-07-01T18:43:55.112Z Reads: 295

```
I don't see any reason why you couldn't charge with a cheap low current BMS and discharge straight off the batteries using the VESC for low voltage protection.
all these people paying big bux for high current BMS, I don't think its even necessary.
```

---
## \#4 Posted by: jakobnator Posted at: 2016-07-01T18:48:18.474Z Reads: 287

```
I would guess it's just for another layer of protection to the batteries for better peace of mind, but I agree.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-07-01T18:50:55.599Z Reads: 262

```
I don't even like the BMS low voltage cut off.. it cuts so hard you SYF.
I don't even use BMS at all.
```

---
## \#6 Posted by: treenutter Posted at: 2016-07-01T19:14:09.031Z Reads: 239

```
@lowGuido I bought my BMS before fully understanding how LVCO works with BMS. Fearing a SYF scenario, I bought a 80a continuous discharge BMS (I think it's 240a burst) and now I'm thinking that it's overkill (and it's huge) and heavy! 

Does using the BMS for discharge help to assure consistent battery drain across the groups? Will the BMS detect the voltage of any of the cell groups and keep the voltages in spec across the pack? If not, I agree that bypassing BMS for discharge would be better, and it let's you buy a cheaper BMS that only comes into play when charging.
```

---
## \#7 Posted by: lowGuido Posted at: 2016-07-01T19:18:47.951Z Reads: 225

```
using the BMS for discharge generally just switches off a FET when the voltage sags to a particular level to stop you for accidentally over discharging.
the actual balancing of the cells is continuous so long as the BMS is connected. so even if you are not discharging through the BMS its still balancing them.
```

---
## \#8 Posted by: treenutter Posted at: 2016-07-01T19:29:07.408Z Reads: 215

```
Thanks @lowGuido 

[quote="lowGuido, post:7, topic:5429"]
so even if you are not discharging through the BMS its still balancing them.
[/quote]

My understanding was that balancing only occurs during charging, but you're saying that balancing happens during discharge as well, even if the BMS is bypassed during discharge. Have I got that right?
```

---
## \#9 Posted by: lowGuido Posted at: 2016-07-01T19:34:59.977Z Reads: 204

```
the BMS is essentialy a series of bleed resistors connected to each cell via a bunch of transistors. when one cell is higher than the rest its transistor is turned on and the excess V's bled out until it matches the rest. the charging and discharging circuits are then very basic hi and lo voltage cutoffs.
I mean you only have to look at the BMS board to see there's nothing too smart on it.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-07-01T19:36:50.909Z Reads: 202

```
If you're running an inline fuse it should be fine, yeah. If the VESC fails for some reason and shit starts shorting like what happened on one of the raptors i have in my garage at the moment, the pack could over discharge and set your toes on fire if you don't at least have a fuse to kill the power in lieu of the BMS. 

I've never seen a VESC short out the way these two did. It was so bad it blew the fuse in front of the space cell and took out the receiver and the other VESC with it just prior. Just a whole pile of dead shit in that board. Mind blown. but the space cell was fine because of the fuse. 

I'm thinking about doing this though, just using a small BMS to charge and directly discharging from the pack and then using a 60Amp automotive fuse to protect the pack which is rated at 80 continuous.
```

---
## \#11 Posted by: lowGuido Posted at: 2016-07-01T19:39:57.777Z Reads: 195

```
if this thing happened without a fuse the BMS would still feed it whatever its max current was until shit burns. so fuse is always a good idea.
```

---
## \#12 Posted by: treenutter Posted at: 2016-07-01T19:52:58.363Z Reads: 189

```
Awesome @longhairedboy and @lowGuido bIg thanks!

Summary: It's better to use VESC's LVCO, an inline fuse to between the battery and VESC, and a smaller, lower-cost BMS that is bypassed during discharge. So my next BMS will be a smaller 60A that supports 10A. 

@longhairedboy do you think the built-in power switches on the Bestech BMSs will still work if we bypass the BMS for discharge? I'd think not, since the cells would be wired right to the VESC with nothing in between.
```

---
## \#13 Posted by: lowGuido Posted at: 2016-07-01T19:54:25.412Z Reads: 181

```
no they wont work. the rely on the output FET's to switch on and off.

thats one downside I guess... although I have never been a fan of soft FET switching...
```

---
## \#14 Posted by: michaeld33 Posted at: 2016-07-01T20:09:22.915Z Reads: 180

```
I have never used a BMS before, and I am just getting ready to build my own 18650 battery, should I be using one, what's the difference in charging for BMS vs no BMS? You still need to balance charge it right?
```

---
## \#15 Posted by: lowGuido Posted at: 2016-07-01T20:13:51.297Z Reads: 176

```
you should definitely use a BMS, don't think that I'm spreading some anti BMS propaganda or something. 
if you are uncertain about anything at all then use the BMS exactly as directed.

but, if you are 100% certain you know exactly what you are doing and are super careful you can get away without one.
```

---
## \#16 Posted by: michaeld33 Posted at: 2016-07-01T20:16:38.814Z Reads: 170

```
-- So a bms is basically just a way of balancing the cells without using a balance charger? What do you use to charge your batteries then? Laptop power supply?
```

---
## \#17 Posted by: lowGuido Posted at: 2016-07-01T20:18:07.137Z Reads: 171

```
I use a balance charger.
if you have a BMS then you can use a laptop style charger
```

---
## \#18 Posted by: michaeld33 Posted at: 2016-07-01T20:23:45.320Z Reads: 179

```
Ok, I get it, although I could do it without one, being able to use a simpler charger is the deal breaker for me... I'm gonna pick up this bms: http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

And a laptop power supply. If I want to use a laptop power supply and I have a 10S4P battery, do I need a 36v 10A power supply? Or could I use something higher than 10A or higher/lower than 36v?
```

---
## \#19 Posted by: lowGuido Posted at: 2016-07-01T20:24:58.736Z Reads: 175

```
yeah I think the main reason people use a BMS is for the simple 1 plug charger and power switch.
which are great features.
```

---
## \#20 Posted by: michaeld33 Posted at: 2016-07-01T20:48:55.457Z Reads: 175

```
So what do you think, this bms: http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

with this charger: http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html

The only thing that bothers me about the charger is that it's MASSIVE! Feel like I am almost better off using a balance charger.
```

---
## \#21 Posted by: lowGuido Posted at: 2016-07-01T20:50:31.854Z Reads: 163

```
looks good.
massive charger.. who cares.. not like you have to ride with it on your board.
```

---
## \#22 Posted by: michaeld33 Posted at: 2016-07-01T20:51:51.962Z Reads: 163

```
Yep, only thing was if I wanted to carry the charger with me... But I guess I could always bring an extra battery...
```

---
## \#23 Posted by: lowGuido Posted at: 2016-07-01T20:52:37.869Z Reads: 164

```
or buy a second smaller charger to keep at work ...
```

---
## \#24 Posted by: michaeld33 Posted at: 2016-07-01T20:53:29.888Z Reads: 166

```
Oh nice, yeah a 2A charger so it can charge during the day (@ 2A, should take ~4hrs to charge to full) and then the big charger at home.
Good idea.
```

---
## \#25 Posted by: lowGuido Posted at: 2016-07-01T20:54:07.231Z Reads: 167

```
yep. Im full of them :stuck_out_tongue:

..or full of something..
```

---
## \#26 Posted by: michaeld33 Posted at: 2016-07-01T20:54:40.547Z Reads: 167

```
haha! alright, thanks!
```

---
## \#27 Posted by: devinalex64 Posted at: 2016-07-09T00:12:15.364Z Reads: 153

```
Hey why don't you try to put a boost converter into the space where you are trying to house the battery with a buck boost converter? if you carry around a laptop+laptop charger combo in a bag/backpack then chances are that you'll have a 19ish volt power supply in that laptop charger. Since you need 42 volts to charge the battery, you can get a boost converter  lie this one http://www.prodctodc.com/120w-dcdc-1032v-to-3560v-boost-converter-laptop-notebook-car-power-supply-p-58.html#.V4A3xbgrKhc and tune it to work with the specific voltage that your laptop charger is rated for. most all adjustable boost converters have little potentiometers that adjust the voltage output. that way you can have it inside the bord and have it charge at 42 volts whiles not having to worry about carrying around a secondary charger rated for 48 volts. just a thought!
```

---
## \#28 Posted by: Nordle Posted at: 2016-07-09T00:17:31.141Z Reads: 144

```
i use this one and bypass discharge, works fine
_~e~use fuse_
```

---
## \#29 Posted by: lowGuido Posted at: 2016-07-09T00:44:02.567Z Reads: 144

```
its 6 of one half a dozen of the other mate.
```

---
## \#30 Posted by: devinalex64 Posted at: 2016-07-09T01:57:49.799Z Reads: 141

```
im sorry im a little confused on what you mean.
```

---
## \#31 Posted by: lowGuido Posted at: 2016-07-09T02:51:41.486Z Reads: 143

```
you cant get something for nothing. ever. its a law of physics.
so if you are using an inverter to up the voltage, it's at a cost.

say you have a 24V 5A charger and you use an inverter to step up the voltage to 48V you will make your charger roughly 48V ~2.5A. the wattage of the charger can't change.

so if you wanted to charge at 48V 5A you would need a 24V charger that can do roughly 10A.

so the size and cost of a 24V 10A charger is probably going to be more or less equivalent to a 48V 5A charger..

24V * 10A = 240W
48V * 5A = 240W 

so if you have a 200W supply its only ever going to be a 200W supply regardless of how many Volts it outputs.

soo TLDR: 
having a small 48V 2.5A charger (stepped up) is the same as having a 24V 5A charger.
```

---
## \#32 Posted by: lowGuido Posted at: 2016-07-09T03:37:43.861Z Reads: 142

```
also, that inverter sports some hefty heatsinks on it.. which tells me it gets hot. so that heat energy has got to also come from somewhere (your charger) and I didn't even bother to factor that into my equation. so if you lose say 5 Watts in heat then your 200W supply is lowered to a 195W supply which means you will get even less Amps out ..
therefore making the larger voltage supply more efficient anyway.
```

---
## \#33 Posted by: tibal32 Posted at: 2016-08-10T04:28:30.291Z Reads: 129

```
hello guys, i'm new to this but i'm trying to make a dummy battery to test a few things out and i wanted to know what BMS would you recommend for a Li-ion 6S4P 22V 11mAh battery? im going to salvage a few 18650 batteries to create a testing battery before going all out building an esk8... would really apreciate suggestions.
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-10T04:31:42.254Z Reads: 123

```
http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html

or 

http://www.bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#35 Posted by: michaeld33 Posted at: 2016-08-10T04:32:09.796Z Reads: 122

```
Alright, sorry to correct but I believe you mean 11Ah battery, also a 6s battery seems a little small... Are you sure you want to build your own if you can just buy a pre made 6s battery? Battery supports has a good list of BMS systems. The capacity of the battery doesn't really matter, just the voltage and such.
```

---
## \#36 Posted by: Jinra Posted at: 2016-08-10T04:40:11.292Z Reads: 120

```
The number of cells in parallel (capacity) can be pretty important, but they should be fine on 4p.
```

---
## \#37 Posted by: tibal32 Posted at: 2016-08-10T05:03:24.670Z Reads: 122

```
thanks @Jinra!!! @michaeld33 i know is a small battery but its just for testing, after i test it ill go for a bigger one!!
```

---
## \#38 Posted by: michaeld33 Posted at: 2016-08-10T05:16:00.838Z Reads: 119

```
Yes, you are correct, but for this circumstance he should be fine with most 6s bms's
Thanks for correcting me!
```

---
## \#39 Posted by: kyo Posted at: 2016-08-10T05:25:01.846Z Reads: 128

```
[quote="lowGuido, post:3, topic:5429, full:true"]
I don't see any reason why you couldn't charge with a cheap low current BMS and discharge straight off the batteries using the VESC for low voltage protection.all these people paying big bux for high current BMS, I don't think its even necessary.
[/quote]


Can you explain further? without BMS, do you need extra care for the battery packs ?

Edit: @lowGuido nvm, I read the whole topic. :smile:
```

---
## \#40 Posted by: gattowx Posted at: 2016-09-29T22:53:26.695Z Reads: 103

```
Hi
anyone know where I can learn to build BMS?
```

---
## \#42 Posted by: Hillso Posted at: 2016-09-29T23:17:11.139Z Reads: 100

```
you mean connect the BMS to the battery?
what BMS do you plan to use?
```

---
## \#43 Posted by: VladPomogaev Posted at: 2016-09-30T03:39:41.923Z Reads: 96

```
Yes. You can bypass the current limit and use the BMS simply to balance the cells. You'll need a 10S constant current/constant voltage PSU. I made a video using a similar one here: https://www.youtube.com/watch?v=jxHQjlHv1y4
```

---
## \#44 Posted by: gattowx Posted at: 2016-09-30T12:01:48.654Z Reads: 95

```
I need to learn to make cards protection for lithium cells
```

---
## \#45 Posted by: michaeld33 Posted at: 2016-09-30T13:06:14.399Z Reads: 92

```
Are you using it for an esk8? Why do you need to build one vs buy one?
```

---
## \#46 Posted by: gattowx Posted at: 2016-10-03T21:15:52.187Z Reads: 88

```
I need to learn because I have special projects and need a BMS at hand, in my country are not achieved easily, must be imported, generating a delay in the applications
```

---
## \#47 Posted by: michaeld33 Posted at: 2016-10-04T13:29:05.821Z Reads: 87

```
I don't think it will be much easier making one yourself, you will need custom made PCBs and such. This may help you tho.

http://raphaelchang.com/projects/bms/
```

---
## \#48 Posted by: gattowx Posted at: 2016-10-07T11:26:46.232Z Reads: 81

```
thanks michaeld33

if anyone knows where I can learn to make a BMS would help me a lot.
```

---
## \#49 Posted by: michaeld33 Posted at: 2016-10-14T13:12:35.819Z Reads: 73

```
Look at the link above, that has helpful info for building a BMS
```

---

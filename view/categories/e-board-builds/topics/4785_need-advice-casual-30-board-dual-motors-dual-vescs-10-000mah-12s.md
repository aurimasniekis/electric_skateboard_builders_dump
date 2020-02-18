# NEED ADVICE Casual 30&rdquo; board/ Dual motors / Dual VESCs / 10 000mAh 12s

### Replies: 10 Views: 1276

## \#1 Posted by: nastyscaper Posted at: 2016-06-16T21:07:36.584Z Reads: 198

```
Hello guys :) This is gonna be my first build and i'm kind of on a budget but know how to fiddle with stuff so I can't buy a brand new already made eskate. Been reading alot and learning about it all and here is what i came up with

**This is gonna be my first e-board to ever build and need some advice, here are my expectations of the board:**
1. it will go at LEAST 15km(9miles) in range (Would like 20km [12miles])
2. it will go at LEAST 30km/h (18Mph) (Woule like to go 40km/h [24mph])
3. it will be reliable and won't be useless in about a year. I will probably ride aprox 200km on it per year and will take extremely care of it, wash the bearings and change the belts when needed etc.
4. It will be able to climb hill easily and not overheat because of the dual motors.


----------

**Now here is my buy list:**
1. This mechanical kit: product/torqueboards-dual-motor-mechanical-kit/
2. These motors (2x) : product/electric-skateboard-motor-6355-230kv-2650w/ OR http://www.enertionboards.com/electric-skateboard-parts/190kv-electric-skateboard-motor/ not quite sure yet, probably will stick with DIY's motors cause i'm on a budget.
3. These VESCs (2x): product/vesc-the-best-electric-skateboard-esc/
4. These batteries (2x) plugged in series: http://www.hobbyking.com/hobbyking/store/__9176__Turnigy_5000mAh_6S_20C_Lipo_Pack.html
5. This board for 0 flex and alot of space to work onto the back: https://www.muirskate.com/longboard/decks/71230/koastal-stringer-longboard-skateboard-deck-w-grip
6. This controller : product/torqueboards-2-4ghz-mini-remote-controller/ (OR Enertion's controller, not sure yet either on that)
7. This charger: https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=36905
8. This power supply: https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=36904

**Total cost: 961.32+shipping and blah blah = 1000$**


----------

I **THINK** I have EVERYTHING i need to build the board. I have a soldering tool to solder stuff i need and i will build my own encassing for parts that need protection.


----------


Now here comes questions:
1. Do i have EVERYTHING I need to build it? Even stuff that people normaly take for granted, tell me if i'm missing anything and you notice it
2. how do you even plug in two VESCs to a motor? I've been reading a bit and from all the info I gathered online this is what I got: http://i.imgur.com/xCkOgnc.png everything will look a bit like this?
3. Think it will meet my expectation? I weigh 140 pounds :slight_smile: 


----------

**Thanks! You guys taught me _so much_ on electric skateboard ! :smiley:**
```

---
## \#2 Posted by: Kaly Posted at: 2016-06-16T21:52:08.235Z Reads: 167

```
You are just missing an enclosure, can get one ready made or DIY one with ABS. 

Since you are on a budget and weight 140 pounds will be more better to get the 12S hub motor he is offering.
```

---
## \#3 Posted by: nastyscaper Posted at: 2016-06-16T22:00:14.878Z Reads: 163

```
Idk. If i get a hub motor i need to change alot of the setup. I also cant fix anything inside a hub motor
And hub motor = less torque abd there is this big hill i need to climb to get to the city hense why i really want a dual motor setup
```

---
## \#4 Posted by: sl33py Posted at: 2016-06-16T22:08:12.456Z Reads: 155

```
Looks like a solid build.  I would suggest for your weight a single setup if on a budget - even a pretty big hill on 10/12s i bet you'll do fine.

That said - 2 is definitely better than 1.  

My suggested edits - controller - go w/ the GT2b instead w/ mad monkey or badwolf enclosure.  It's about 1/2 the price, smaller - but you'll need to get a printed enclosure and take a bit of time to swap internals.  Not that hard, but not plug and play either.

Batteries - i'd get 4x slimmer batteries vs 2 big ones like that.  better ground clearance and possibly lighter (depending on battery).  I sort them by the "c" axis measurement on HK which is thickness usually.  

battery charger - i'd get the B6 AC v2 if you can swing it.  All-in-one is nice.  Or go fully to one that does 20+ Amps and runs off a 12v 350+ watt power supply.  (check out server supplies on ebay - cheap and super powerful).  I have a pair of 750w dell PSU in series for 24v - iCharger likes higher voltage!

HTH - GL!
```

---
## \#5 Posted by: Kaly Posted at: 2016-06-16T22:08:40.376Z Reads: 136

```
well the hill changes everything the hub motors are not good for hills
so better continue with your plan
```

---
## \#6 Posted by: sl33py Posted at: 2016-06-16T22:09:20.340Z Reads: 131

```
I think for 140lbs a hub motor would work great, but like you i prefer the ability to repair/fix/modify a modular setup with belts (and re-gear).

Looks like you've done your homework.  You are pretty much there - GL!
```

---
## \#7 Posted by: nastyscaper Posted at: 2016-06-16T22:25:34.070Z Reads: 120

```
Ay thanks mate!
I might get 4x batteries. Valid point, they're slimmer and i have alot of board surface!
```

---
## \#8 Posted by: nastyscaper Posted at: 2016-06-16T22:31:41.878Z Reads: 111

```
For the record though, the little diagram i made on paint is correct, right? 
Batteries in series to in parralel into the VESCs. one VESC is connected to the receiver. Both VESCs are connected with the CAN-BUS with the two middle connectors. Each VESC is connected to a motor and each motor to a belt to a wheel.
...right?
(mostly uncertain about the VESC part tbh, things i read online aren't so clear to me, i'm mostly a visual guy and english isn't my mother tongue :slight_smile:)
```

---
## \#9 Posted by: Kaly Posted at: 2016-06-16T23:30:14.572Z Reads: 105

```
the diagram is correct, you have do your homework really good
i like when people hit the ground running :thumbsup:
```

---
## \#10 Posted by: sl33py Posted at: 2016-06-16T23:30:29.347Z Reads: 111

```
I think your English is mo betta than mine... ;)  And i don't have any excuses about 2/3/4th languages...

I missed your drawing.  Took a look at it and it looks correct to me.  You'll obviously need to modify the wiring if you go to 4x batteries vs 2x, but looks good.  using a same 5000mAh packs - You will be in series throughout though.  No parallel, or you'd have 6s2p instead of 12s1p (3s + 3s + 3s + 3s = **12s 5000mAh**)  If you do 3s+3s and then in parallel you'd have 6s2p **10000mAh** 

A note on charging - make sure to disconnect everything to pull batteries to charge.  I also recommend a parallel charging board to simplify charging 4 batteries at the same time.  (this is when your 50W / 5A max on your charger might be painful)  A higher Amp charger will let you charge quickly (so you can go ride after work or on short notice) instead of trickle charging and riding the next day.  Realizing that charging at a low C value (.5 C is my preferred) does improve the life/length of your batteries - BUT sometimes you want to ride NOW!!  (long day at work, limited time before sunset, or spur of the moment ride)

A small battery voltage alarm is good to have so you don't over-draw and damage your batteries.  I like a conservative cutoff around 3.6v per cell.  Some do 3.4 and lower, but with less expensive batteries - there's a chance to damage a cell and ruin the pack (or you can take apart and replace the bad cell individually - PITA and i don't do this).

GL!

Edit - paraboard info:
http://www.buddyrc.com/power-system/paraboard-parallel-charge-board.html
[img]http://www.buddyrc.com/media/catalog/product/cache/1/image/700x/9df78eab33525d08d6e5fb8d27136e95/p/a/paraboard_v2_xh_xt60.jpg[/img]
You can get similar on ebay or Hobbyking for a lot less.  These are some of the best though - so a good investment if you can swing the $.  They have different connector versions and a bare wire option to use your own connectors.
```

---

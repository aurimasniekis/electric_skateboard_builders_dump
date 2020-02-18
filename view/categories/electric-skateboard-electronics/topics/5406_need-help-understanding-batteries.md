# Need help understanding batteries

### Replies: 8 Views: 2492

## \#1 Posted by: ouch_fiyah Posted at: 2016-07-01T03:33:22.814Z Reads: 235

```
Greetings everyone,

I'm in the process of learning what I can about building my first electric board, and pretty much have my parts list together.  At the moment, I'm having trouble with what battery setup to use. 

I'm planning on using: 
VESC
DIY's 230kv motor
16/36t pulleys
83mm wheels

Using toddy616's calc, I want to use either a 8s or 7s battery (I suppose 6s would be fine as well). I was looking at 18650 batteries and highly debated using them, but they are just out of my price range. So i'm gonna go with lipo's. I just have a few questions if anyone can please answer/explain.

1) How do you choose battery specs? is it based off the motor?
2) If it's not based off the motor, what would be good battery specs then? 
3) Why do the same batteries sometimes have different capacities?
4) So for an 8s battery, I would need 2x 4s4p batteries right? 
5) What battery brand would you guys recommend? 
     a) What battery brand would you recommend if I plan on disassembling to make a more low profile battery? I saw a post about multistar(?) batteries, but also heard they weren't that great. 


I'm sure you'll have more questions down the line, but thanks a lot for taking time to read this!
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-07-01T04:10:48.436Z Reads: 227

```
1. Battery Specs are slightly complicated, so I'll walk you through it.
---C rating is the discharge, for your sake, just get the lowest C rating you can (no lower then 10C) C basically means the amount of power that the motor can put out at one time. Electric skateboards don't need more than a few C, so it's not really a big deal with lipos- however, with 18650 batteries you need to get the ones that have a higher discharge rate since some are as low as 2C, I recommend the INR18650-25R.
---S is (as it seems you know) the number of cells the battery has, this determines the voltage, which can also determine the speed of the board, but make sure your ESC can handle the number of cells your board has.
---mAh (milliamp hours) is the capacity of your battery, 5000mAh is the same thing as 5Ah, milliamps is just a smaller unit (like millimeters and centimeters.) It depends on your setup, but 5000mAh should get you a few miles, good for short/mid distance trips < 5 miles

1.  I reccomend a 6S 5000mah 25C battery for beginners, should be about $50, but go with what ever you want. You can also do 2x 3S 3000mah 25C batteries connected in series, but then it will only have a capacity of 3000mah.

1. I'm not sure what you are trying to say...

1.  the XsYp naming convention is used for 18650 batteries, not so much lipos -- you would probably end up using 2x 4s lipos in series, if you use a 4000mah 4s lipo, then you will end up with a 4000mah 8s lipo, if you need more capacity you have to get 2 more 4s 4000mah lipos-- turn that into another 8s 4000mah lipo, and wire them in parallel to get an 8s 8000mah battery. (if this is confusing feel free to say so, I'll clear it up)

1. Doesn't REALLY matter, but go with a more credible brand-- turnigy, multistar, zippy compact, etc.

1. (5a) @barajabali had some luck with the multistar batteries because they were not glued together, which made getting them apart easier. In the long run it doesn't really matter because all batteries are basically the same thing, a bunch of lipo single cell batteries stuck together. You have to be really careful though when disassembling batteries. I recommend you check out @barajabali's tutorial (if you haven't already) http://www.electric-skateboard.builders/t/how-i-made-my-lipo-packs-slimmer/1415
```

---
## \#3 Posted by: ouch_fiyah Posted at: 2016-07-01T05:06:04.181Z Reads: 204

```
thanks a lot for the explanation @michaeld33! it really has helped me alot (and hopefully for anyone else who doesn't know)

1) So ~25c would be sufficient for (any/most) eboards? However, I'm just curious on what the difference/effect is between a 25c vs (say) a 65c battery.  

3) I saw some 4s lipos which looked the same but had different capacities:
Example: [1000mah](http://www.hobbyking.com/hobbyking/store/__91173__Turnigy_Graphene_1000mAh_4S_65C_Lipo_Pack_w_XT60.html) vs [3000mah](http://www.hobbyking.com/hobbyking/store/__91189__Turnigy_Graphene_3000mAh_4S_65C_Lipo_Pack_w_XT90.html)
Obiviously one cost more, but other than that, I could just choose whichever capacity I wanted right? Since all the other specs look identical.

4) Ah I see, the naming convention did mess me up since I was studying/debating about 18650's. So for 8s, 2 x 4s lipos (and another 2x4s in parallel if i want more capacity), got it, thanks!


----------

(Haven't bought a VESC yet) but provided the VESC has the same adapter as my batteries, would it be plug and play? Would I need a BMS (or equivalent or would VESC take care of that)

What would be the terminology for a cable that connects batteries in series? What about batteries in parallel? (So I can research/purchase them later)

And lastly, what would be the best way to charge a 2x4s or 4x4s (2 sets in parallel) setup? If you (or anyone) could offer me a suggestion on a charger or charger setup that would be great.
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-07-01T05:36:24.291Z Reads: 180

```
No problem!

1. 25C should work perfectly fine for 99.9% of Eboards unless you are adding big brushless motors on the side, with propellers, and planning on making it fly. Then your gonna need a larger discharge capacity such as 65C. The C rating is related to internal resistance, which basically prevents a battery from outputting too much power at once. In an ideal world, there would be no ISR (internal series resistance) and a battery could output as much current as it needed to at once, but the internal resistance can prevent that.  (Don't quote me on that one though.) *A 65C battery basically can deliver more current when its needed than a 25C battery.*

1. First, before I get to that.. HOLY S***, you are going for graphene batteries?? If you are going to spend that much, you should just get a 18650 battery pack made. You can get a 4S 3000mah battery for alot less then that, you don't need the C rating that the graphene batteries output to get a nice ride. The graphene batteries are made almost exclusively for high powered planes and multirotors which pull a lot of power, I mean this is a 4S 5000mah battery for almost half the price: http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=9179

1. Ok onto your question, if you are going to wire them in series you have to use the same capacity. This is very important. The same thing is true for parallel. What happens (when wired in parallel) is when the the battery with a smaller capacity gets fully drained, the other batteries try to refill it... and boom.
Basically, yeah, you are all good with either of those batteries, just use the same exact ones when connecting them together.

1. Yep naming convention is weird, it looks like you get it now though...

I believe that you can connect it directly to the VESC because it's a lipo, a BMS is for 18650 batteries and similar li-ion cells.

Terminology? Well most people diy it by soldering them directly together or something. Hobbyking does sell a series wiring thing though, so all you do is plug your batteries into it and then there is a connector which is the output, it does the wiring for you and you can also unplug it and use/charge the batteries individually. They also have one for parallel.

Series: http://www.hobbyking.com/hobbyking/store/__10264__XT60_Harness_for_2_Packs_in_Series_1pc_.html

Parallel: 
http://www.hobbyking.com/hobbyking/store/__64402__XT60_Harness_for_2_Packs_in_Parallel_1pc_AR_Warehouse_.html?strSearch=parallel
http://www.hobbyking.com/hobbyking/store/__10265__XT60_Harness_for_2_Packs_in_Parallel_1pc_.html
(two options for parallel, one is smaller format)

The best way to charge it? Well you could charge them all individually, or you could wire them together if you feel confident...
This link may be helpful, http://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734/6
Along with this hobbyking part: http://www.hobbyking.com/hobbyking/store/__27078__JST_XH_Parallel_Balance_Lead_4S_250mm_2xJST_XH_.html

Hobbyking only sells the balance leads for packs in parallel, not in series.

Honestly I would personally either charge them individually or just get one massive 8S lipo, because I don't want to mess around with the balance port.

Charger for 2-6S batteries: http://www.hobbyking.com/hobbyking/store/__5548__IMAX_B6_50W_5A_Charger_Discharger_1_6_Cells_GENUINE_.html

Charger for 1-8S batteries: http://www.hobbyking.com/hobbyking/store/__7523__Turnigy_Accucel_8_150W_7A_Balancer_Charger.html

Keep in mind that working with lipo batteries is dangerous and you have to be careful!
```

---
## \#5 Posted by: ouch_fiyah Posted at: 2016-07-02T01:41:58.167Z Reads: 124

```
Thanks again @michaeld33. I feel a lot more confident looking for batteries now. 

Time to order parts, then learn about vesc! But I'll cross that bridge when I get there haha
```

---
## \#6 Posted by: Namasaki Posted at: 2016-07-02T03:22:32.304Z Reads: 122

```
One word of caution. Don't even unpack the Vesc until you have read all of the setup info and downloaded the programing software. Then follow the setup criteria very carefully.
```

---
## \#7 Posted by: charliek Posted at: 2016-12-15T05:31:29.570Z Reads: 76

```
Hello I also have some questions here 
Would connecting 2 x 3s 5000mah battery in series  be same with connecting 2 x 6s 2500mah battery in parallel?  Both should be equivalent to 1 x 6s 5000mah battery right? Would discharge rate double if the batteries are connected in parallel (since connecting batteries in parallel doubles the current)
```

---
## \#8 Posted by: saul Posted at: 2016-12-15T05:49:01.401Z Reads: 74

```
[quote="charliek, post:7, topic:5406"]
2 x 3s 5000mah battery in series  be same with connecting 2 x 6s 2500mah battery in parallel?  Both should be equivalent to 1 x 6s 5000mah battery right?
[/quote]

Yes. they are equal.[quote="charliek, post:7, topic:5406"]
Would discharge rate double if the batteries are connected in parallel (since connecting batteries in parallel doubles the current)
[/quote]

Technically yes, but not in this example.
C rating is depended on the battery capacity.
so 20C for a 5000mah = 20 * 5 = 100Amps
for 20C for 2500mah = 20 * 2.5 = 50A.

then connecting 2 in parraelel you get 2 * 2500mah = 5000mah * 20 = 100A.
```

---

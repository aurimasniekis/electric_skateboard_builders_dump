# Metamorph &#124; Haya (2nd Rnd) &#124; TB218 &#124; Dual 6374 &#124; 10S5P &#124; Focbox

### Replies: 21 Views: 1048

## \#1 Posted by: skatardude10 Posted at: 2019-03-06T05:58:19.902Z Reads: 275

```
Well, i've committed to hopping on the Haya train with the second round coming at some point. 

The intent behind this build is to transplant my [current build](https://www.electric-skateboard.builders/t/the-demonseed-tb-218-tb-6374s-190kv-tb-mounts-chibattery-10s4p-dual-focboxes-superflys/50610) over to the Haya.

Originally I just wanted to start off by building a 12S8P battery, but the stress of adding up parts to make it totaling over $800 *literally* gave me shingles- had to take medicine. I still want to upgrade my board this year, hopefully without breaking the bank *too much*.

So, i've taken the plunge on some battery building supplies. I've purchased the MinispotA spot welder with lipo/charger, 10 additional 25R cells, battery shrink wrap, kapton tape, nickel strip, extra silicone wire I don't have on hand, cell terminal protectors... etc. The plan is to disassemble my current Chibattery 10S4P 25R, re-make it (keeping the spot welds on the original 4P groups) adding an additional cell per P group for 10S5P, re-wiring the BMS... making it my own, built for the Haya.

![unnamed|690x388](upload://b6l8De0SEms5a6lTlLdQmFgbMUR.jpeg) 

I haven't seen anyone paint their Haya yet, and I really like the look of the Exway X1's finish... some sort of Line-X type material. I'll be going for the same sort of finish with some truck bed liner spray, and possibly the Haya logo in a few primary colors (think Google colors :-) ) masked off from the truck-bed finish of the rest of the board

Plan is, with dyed black Nylon, TPU, conformal coating if needed, some good thin rubber sealing material, to make this thing as water tight as possible. On a similar note, all of my builds and projects are always looking janky. My goal with this is to make it look as clean as possible, and put time into cable management, routing, etc, with 3d printed cable routing, ESC and BMS holders, etc. I see a lot of freshly soldered bullets in my future.

I'm considering some way to be able to quick connect an entire boost converter module, similar to the one on my build now, but at the same time I don't want it to detract from the simplicity the Haya is able to provide. So, this might come at a (much) later date.

Here's some mockups I did real quick to make sure everything would fit. This is the mockup i'll be using to design the rest of the components (loop key, charge port) that will hopefully be cleanly nestled inside some risers that will eventually be printed.

![haya_original_2019-Mar-06_02-47-08AM-000_CustomizedView16632382385_png|690x388](upload://zAecXQaNRnjdw8Z7m8VDDBSyric.jpeg) ![haya_original_2019-Mar-06_02-47-16AM-000_CustomizedView26061410219_png|690x388](upload://d1dUuFmdGgN6yM9HlExGEf7aLNi.jpeg) ![haya_original_2019-Mar-06_02-47-33AM-000_CustomizedView12790452438_png|690x388](upload://4z2IIgvqm5bvVqvPEGR9fXROcpf.jpeg) ![haya_original_2019-Mar-06_02-48-01AM-000_CustomizedView8545100488_png|690x388](upload://adFvCr11NVDtYVBhraDEPuBLUzZ.jpeg) ![haya_original_2019-Mar-06_02-48-24AM-000_CustomizedView4066370811_png|690x388](upload://8XyndE7SHVHJ37Jj8A81iYc05kQ.jpeg) ![haya_original_2019-Mar-06_02-48-35AM-000_CustomizedView250251255_png|690x388](upload://azRHPwJpcD4knpAkOlgASthTedJ.jpeg)
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-03-06T07:35:04.056Z Reads: 235

```
isn't it kinda bad to add to the p-packs?  the one new cell on each will carry a disproportionate load since it will have lower internal resistance
```

---
## \#3 Posted by: rojitor Posted at: 2019-03-06T11:08:03.525Z Reads: 227

```
Depends on the age of the pack
```

---
## \#4 Posted by: skatardude10 Posted at: 2019-03-06T13:36:06.220Z Reads: 212

```
The pack is about a year old come end of April, it's had maybe 100 cycles and I'm considering running each P group through some testing to check IR and each groups total capacity to determine their health before adding the additional cells. Maybe I won't push the amps any higher than I do now, just hope for a bit better range and a bit less sag.
```

---
## \#5 Posted by: skatardude10 Posted at: 2019-03-16T06:37:07.329Z Reads: 198

```
Been working on the paint design mockup and riser pads 
* 7 degree dewedged rear 
* 5 degree wedged front 
* Charge port behind the front truck
* Loop key rear of rear truck (not fully modeled yet)
* Motor Phases vertical out of the front of the rear riser

Still need to model the cable routing, routing for inside of the board, etc... lots of work ahead. 

I'm considering giving the push to start switch a try for simplicity and getting rid of the anti-spark switch out of the back. If all you can (barely) see is the phase wires and plugged charge port, that would be fantastic.

![haya_original_2019-Mar-16_05-54-32AM-000_CustomizedView10974315262_png|690x388](upload://a9dDAsC6unqJj4pmTiFYJDI0uw5.jpeg) 
![haya_original_2019-Mar-16_05-36-18AM-000_CustomizedView9033142751_png|690x388](upload://8K7BxHXL4hBFS5TIXvlycR8NPJw.jpeg) 
![haya_original_2019-Mar-16_05-38-04AM-000_CustomizedView16630858776_png|690x388](upload://xqdEdFuXmCGAA6uknexKV2Hgz06.jpeg) 
![haya_original_2019-Mar-16_05-55-31AM-000_CustomizedView30979697419_png|690x388](upload://amOprR8myLPFnlqCjRkuKKxc5sW.jpeg) 
![haya_original_2019-Mar-16_06-19-33AM-000_CustomizedView19162275502_png|690x388](upload://fk9PFjSUv2WufbLAfnObVeewIbU.jpeg) 
![haya_original_2019-Mar-16_05-37-17AM-000_CustomizedView47283246819_png|690x388](upload://5WfFelyKQ4jRiiyn3jLrnUxJeiN.jpeg) 

From here I am planning on drawing up some nylon sleds to hold all but the battery in place, with TPU shrouds (and cutouts for airflow on the focbox heatsinks) for vibration dampening that will bolt into the nylon sleds. Also, i'm considering printing slim but 100% infill TPU shock pads to go under the risers. Obviously some TPU plugs for the holes for water resistance, and a single layer of TPU might serve well between the deck and metal top for vibrations and water-sealing- we will see... might just use some ultra-thin neoprene foam for that.

So far, all I need to complete this is the Haya, paint, extra Nylon filament, some black TPU filament, push to start switch and maybe a couple more bullet connectors if I can't find the one's i'm missing floating around in my esk8 parts drawers.
```

---
## \#6 Posted by: Linny Posted at: 2019-03-16T06:50:09.350Z Reads: 173

```
This looks waaaaaaay cool!
```

---
## \#7 Posted by: skatardude10 Posted at: 2019-03-19T22:01:49.490Z Reads: 170

```
Spot Welder arrived today!! 

I feel like a kid in a toy store with the best toys in the cart- the minispotA. Can I ask, do these look like good welds to you guys? Imo they seem great, but I'm new to spot welding.

https://youtu.be/ey_zZe65Wxk

Also, I took the plunge on all new cells, VTC5A from nkon, for the same 10S5P configuration. At 35A, I can't imagine pushing 175A total. I'm going to have to layer up the nickel on this battery, and maybe double up on the 10AWG silicone wires for the discharge leads and bridges between P groups... we will see. If anything I'll use more materials, but a goal with this will be to reduce as much voltage sag caused by resistance as possible. Also, I'll probably only run 60A battery max per vesc at the most.

I'm really liking these 30A discharge curves compared to the 25r cells I have now. 

![20190319_155117|690x396](upload://uz0ZL9lfWhTygjJgGHW7c78yhlH.jpeg) 

I'll use the Supower 10S 60A BMS in charge only configuration from my old Chibattery pack from Bara. 

I'll probably end up recycling the 25r cells into a range extending pack in 6S8P, or combine the 25r cells with a bunch of healthy Samsung 30p cells for an even more massive 6S14P range extending charge box.
```

---
## \#8 Posted by: skatardude10 Posted at: 2019-03-26T00:22:02.864Z Reads: 151

```
Would a capacitor bank hooked up via XT60/12AWG silicone wire to the XT90 splitter be effective, or do I need to use thicker wires and/or just even closer to or shorten the ESC power leads?
```

---
## \#9 Posted by: skatardude10 Posted at: 2019-03-26T05:30:14.999Z Reads: 148

```
![20190325_232439|690x335](upload://aSOXVQYoUxBtWyDs62LWabLyWlz.jpeg) ![20190325_232521|690x335](upload://8lParhgV67U8aTY6Ox78XSQFyHV.jpeg) ![20190325_232502|690x335](upload://uRrvFZ9cmzbqFPAdGJ9XEOl2hMu.jpeg) ![20190325_232717|690x335](upload://uhMADCyTEcWvAINdwy0C96XfjGm.jpeg) ![20190325_232708|690x335](upload://lyWUlzCKE0i39K7k0DMo6x7tGxk.jpeg) ![20190325_232817|690x335](upload://yvHcNYxXQ6v6NTo7M7b9KsmhcZo.jpeg) 

Getting late, solder and liquid electrical tape/e6000 tomorrow.
```

---
## \#10 Posted by: skatardude10 Posted at: 2019-03-27T05:01:15.014Z Reads: 141

```
Woh. photo heavy warning

Way less clean than I intended. Anyways... I don't even know if the barley paper, kapton tape, etc are all really necessary but i'd rather be safe than sorry. About half way I futzed up big time, but patched it up as best I could.

kapton
![20190326_202726|690x335](upload://jS4vdgWi2Trx4zgmjUqo6ktCgU4.jpeg) 

e6000 for vibrations and seat the caps
![20190326_203623|690x335](upload://n9vImQhLBlKJQhzTNJhyJeT8VIn.jpeg) 

clipping leads

![20190326_204225|243x500](upload://ybxYcbwOFPKvGhnGmW7lqLmKTxS.jpeg) 

cutting into wires
![20190326_205131|690x335](upload://iGMV0z4HO0RJ1cjctQtfItnlGNV.jpeg) 

soldered wires

![20190326_210920|243x500](upload://wx4Xc6SLBRSNFa5mTOk5cNmrNnM.jpeg) 

GAH Big fuck up. This whole time i'd been diligent about watching out for polarity. Patched it up with red and black heat shrink to make sure I don't forget when it's all done and sealed up.
![20190326_211537|690x335](upload://bV6WTlfuIUZRh7Y7LlsZ9Cd1HPh.jpeg) 

Liquid electrical tape
![20190326_212230|690x335](upload://xPhEuLL6jKIH6OcmgyI6Q2JmiTk.jpeg) 

smush and slather. Is this a bad idea? the caps seem pretty hardy, but I don't know.
![20190326_213037|690x335](upload://j66yRR6Pi39f6Qny4I5gKhWRfVJ.jpeg) 

After some curing time, I decided on adding barley paper and extra heat shrink. I don't want to look at that mess.
![20190326_223258|690x335](upload://6ScZuF81KOo0sgCDnRrPdrw2JVG.jpeg) 

more kapton
![20190326_223638|690x335](upload://aAddCR7x97z7wSpb50r6zicScay.jpeg) 

All kapton. At least it's somewhat consistent with orange color now.
![20190326_224944|690x335](upload://laBufcyW5XuLA4GBJ1wbYsTU9RW.jpeg) 
![20190326_225005|690x335](upload://xPIYII6OH4k6nMd71l6RXCEkNIA.jpeg) ![20190326_225040|690x335](upload://881ZTSpp9kTNyPbbj5hOY8TuWGG.jpeg) 

That's all for now.
```

---
## \#11 Posted by: skatardude10 Posted at: 2019-03-27T06:26:35.747Z Reads: 124

```
I tested it with by charging it up to 3V and 9V, and discharging to a DC buzzer, and it seems to work. The small buzzers buzz VEEERRYY quiet for a long time, and the large buzzer just lets out one ZOOP real quick and the voltage returns to 0 +/- 0.01v on my multimeter. 

For someone that knows this stuff, maybe @b264, when I hook up positive to positive and negative to negative on my multimeter to the capacitor bank, with the meter set to read ohms at 20k range, the reading slowly rises. Opposite to that, hooking up positive to negative and negative to positive, the reading drops, a bit quicker than when it rises. 

To me this sounds good, and I am 90% sure I got the polarity correct from my limited knowledge... It'd be nice to know for sure before hooking it up to a 42V pack down the line.
```

---
## \#12 Posted by: b264 Posted at: 2019-03-27T06:48:33.755Z Reads: 117

```
That's the correct behaviour.  I hope you're using a loopkey and not an antispark switch.
```

---
## \#13 Posted by: skatardude10 Posted at: 2019-03-27T07:02:56.196Z Reads: 118

```
Loop key for sure. AS150 x2 pairs and 8AWG just came in today. AS150 pair for battery connection and one of the other pairs connectors for the loop plug.
```

---
## \#14 Posted by: b264 Posted at: 2019-03-27T07:04:03.015Z Reads: 117

```
You might play with reducing the switching frequency on the VESC and see how that works, since you have enough capacitance to do so ;-)
```

---
## \#15 Posted by: skatardude10 Posted at: 2019-03-27T07:05:24.820Z Reads: 117

```
Ah I'll give that a try, thanks for the tip 🙂 

What benefit does that provide exactly? Stronger as opposed to smoother/quieter power delivery in FOC? Or, is it that efficiency is reduced with lower switching frequency *because* of the lack of capacitance...
```

---
## \#16 Posted by: b264 Posted at: 2019-03-27T07:10:35.463Z Reads: 118

```
Not sure, but I'd like to know ;-)

Is it noisier?  Is it quieter?  Does it feel different?
```

---
## \#17 Posted by: skatardude10 Posted at: 2019-04-13T00:14:21.692Z Reads: 108

```
Well I'm going with TB DDs, 90kV for this build now.

To make this board airline safe, I am considering making all series connections with 2X 10AWG with 5.5mm bullet connectors between series packs and individually wrapping each parallel group in its own barley paper and shrink wrap. Each pack would be 46.8 watt hours, and there doesn't seem to be a carry on limit for packs under 101 watt hours. I need to find some small connectors that I can use to disconnect and reconnect the balance leads for traveling.
```

---
## \#18 Posted by: RedBaron Posted at: 2019-05-03T04:53:39.036Z Reads: 90

```
Any progress?
```

---
## \#19 Posted by: neiru37 Posted at: 2019-05-03T05:51:56.617Z Reads: 94

```
[quote="skatardude10, post:17, topic:86280"]
I need to find some small connectors that I can use to disconnect and reconnect the balance leads for traveling.
[/quote]

I tried doing something similar for my build:

 [quote="neiru37, post:1, topic:82733"]
 To make it modular, I soldered some XT30 connectors to the ends of each module.

![20181130_144042.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/9/e/9ec1d8e846b450aefe9b8ace172dc390fdc0e362.jpeg)

I chose this connector because it’s small enough that it doesn’t eat up that much space and each pin supports 30 amps, for a total of 60.

 ![20181130_144203.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/a/3ad52a35602c83a90d7065a83eba7ae1bce410f5.jpeg)

 To make balance leads modular, I soldered some 2 pin jst plugs to the braid, one in the middle and one on the positive end.

![20181130_162636.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/9/c9441b9be8029195b9537dbb0e96b0902148ee2a.jpeg)

 ![20181130_170431.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/4/d488965ccdb8be3f887b8a8769f7da837cf65b3b.jpeg)
 [/quote]
```

---
## \#20 Posted by: skatardude10 Posted at: 2019-05-03T07:13:57.527Z Reads: 90

```
Not yet, waiting on board, drives, and a new spot welder.
```

---
## \#21 Posted by: Lobbie Posted at: 2019-06-04T13:29:18.951Z Reads: 54

```
Anything New!!
```

---

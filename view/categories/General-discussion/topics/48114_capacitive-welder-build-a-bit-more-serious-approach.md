# Capacitive welder build - A bit more serious approach

### Replies: 24 Views: 3764

## \#1 Posted by: SimosMCmuffin Posted at: 2018-03-04T12:04:43.004Z Reads: 264

```
So while I'm waiting for the PCBs for the http://www.electric-skateboard.builders/t/flexibms-first-prototype-kicad-project-files-released-flexible-configuration-and-charging-bms/46117/1 to get fabricated and shipped. 
I'm designing another tool that I need to upgrade in my arsenal, which is my battery tab welder.

If you're wondering about my gripes and gubles with my old welder, refer to my 50 cell pack build over here: http://www.electric-skateboard.builders/t/10s5p-battery-pack-build-log-50-pieces-of-samsung-35e-cells/23547

Overall, the welder is a sub-performing mess, due to the heavy batteries and mess of wires and I'm not happy with it's performance. So what do? Well first let's look at what the professionals use in a more industrial settings.
Video starts at the battery welder part.
https://youtu.be/oNfTEHBz_bg?t=1m2s


----

So usually there are one of two types of welder power sources used. 
They either use a capacitor bank that they charge up to a certain voltage and then discharge it with a precision pulse or double pulse, which' pulse lengths are configurable. Or they use a welding transformer to step-down wall AC voltage to lower a voltage, but higher current one.

In the video due to the manufacturer and model info being hidden by the tape on the welding machine, I can't confirm the power type for that particular one.

Practical examples of both:
Capacitive, front control knobs allow you to set the capacitor bank voltage, which is indicated as the stored energy in Ws (Watt-seconds) and two knobs to configure the lengths of the two pulses:
https://sunstonewelders.com/product/cd1000dp/


Welding transformer. Now, if you happen to check out the ebay link, you'll find that this particular machine runs in the 3000+ dollar range + same goes for the capacitive ones and I'm not willing to put in something like that.
https://www.ebay.co.uk/itm/Pneumatic-Pulse-Battery-Spot-Welder-Welding-Machine-18-Kva-3500-A-Ps300-B-/112415963445?hash=item1a2c837935

---
So DIY route to glory then? Ok, I'm familiar with capacitors and I can see many upsides if the welder is done right with them. I'm taking some concepts and ideas from this particular build http://www.zeva.com.au/Projects/SpotWelderV2/ ,but I'm looking in to make it a bit more refined, but still as simple and easy to assemble as possible (No soldering of any thick wires). And allow it's integration into a CNC setup like in the video.

I'm going to build the welder out of 3 main blocks. Capacitor bank, electronic switch and microcontroller board. This way I can make it more modular and not having to risk total redesign of something didn't work in single integrated package.

I currently have the capacitor bank and electronics switch boards modeled up with pictures below.

Capacitor bank board with integrated TVS diodes to protect from inductive voltage spikes, which can be a real issue with high currents and parasitic inductance in the cabling. Current capacitor choice https://www.digikey.fi/products/en?keywords=25USC47000MEFCSN35X50
![image|630x500](upload://d1ADQ9F0xkgsdUQElvxeQFc1dzX.jpg)

Electronic switch board. Uses https://www.fairchildsemi.com/datasheets/FD/FDBL86561_F085.pdf beefy mosfets, with added TVS diode to protect from inductive voltage spikes.
![image|690x486](upload://jlTx8gCHjLSGHotafgQNw1dl4Kg.jpg)
![image|690x486](upload://p0k60v3tDS0Lz0yqe11d19YGOqh.jpg)

And here's a quick and dirty blender render of the setup bolted together, without the microcontroller board.
![image|690x214](upload://5Cr8FVKDy9HkfME6m6Y2OeCuNQF.png)
![image|556x500](upload://lhVj2FJykPfIp5pGrbPaV0r1aIJ.png)

With 20 Caps of the before-mentioned model, it would have the theoretical energy of ~290 Ws, which is pretty beefy amount of energy and adding more capacitor boards is quite easy with just longer busbars and double side mounted boards, which are just bolted to the busbar.

All-in-all I want to build this welder to get away from the chemical power sources, AKA batteries. I see them problematic with repeatability and performance over time degrading due to the chemical breakdown happening inside them.

**Thoughts and discussion on this?**
```

---
## \#2 Posted by: Acido Posted at: 2018-03-04T12:19:26.191Z Reads: 213

```
I guess you would attach cables to these busbars?
How much would this cost, if it can weld ,2 mm it would be great...
Also small shorts don't degrade batteries, especially big car ones, even if they do its unnoticeable since they can discharge a shit ton of amps more than needed
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2018-03-04T12:33:26.734Z Reads: 222

```
[quote="Acido, post:2, topic:48114"]
I guess you would attach cables to these busbars?
[/quote]
Yes, I will most probably make a case for the welder so that the end of the busbars come out the front a bit, so I can attach with nuts and bolts more flexible cables  with the electrodes at the end.

[quote="Acido, post:2, topic:48114"]
How much would this cost, if it can weld ,2 mm it would be great…
[/quote]
I'm going to make at least one prototype with 20 caps, which are the bulk of the cost @ 95€ for 20 pcs and if it shows promise, then double that up to 40 caps. Quite frankly, I have no clear idea, how it will perform, but that's why I'm doing it in such clear separate blocks so I can change/upgrade individual blocks if necessary according to my testing.

[quote="Acido, post:2, topic:48114"]
Also small shorts don’t degrade batteries, especially big car ones, even if they do its unnoticeable since they can discharge a shit ton of amps more than needed
[/quote]
True, but still I think it's good way to go forward by looking at what is being used in industrial use cases, at least approach wise. 

Let's look at this way, I'm willing to test this and do R&D on my own cost, because I can see this working better then what people are using right now. At least we will get definitive answers through this.

EDIT: I believe the capacitor bank will be able to produce a higher current than a battery and therefore allow to use shorter welding pulse, resulting in a cleaner welds.
```

---
## \#4 Posted by: Acido Posted at: 2018-03-04T12:41:04.015Z Reads: 170

```
Im, not an electrician but im pretty sure you will need some kind of a controller to control the times
Because the more the caps the longer the discharge time, if you add 50 it will have the time 50 times longer than 1 cap... This is my logical approach of an electrical  Homo neanderthalensis
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2018-03-04T13:20:04.075Z Reads: 178

```
Not shown in the renders in the original post is the microcontroller board, that would allow you to set to which voltage to charge the capacitors to and what lengths the double pulses would be.

The point is not to completely discharge the capacitor's but just pulse them enough to make the weld. As shown in the picture below what the capacitor voltage looks like with the double pulses. They don't discharge completely. The higher voltage we charge them, the higher the initial current will be at the beginning of the pulse.
![image|365x290](upload://crk6wJrj0rdwKUxNOpl3ZfRYFFy.jpg)

The principle behind using capacitors as the power bank is explained in one the sunstone CD welder's user manual.
https://www.powerstream.com/ss/PSSunstoneDPWelderIP.pdf
```

---
## \#6 Posted by: banjaxxed Posted at: 2018-03-04T14:01:32.087Z Reads: 171

```
My LiFePo4 12v shorai does 270cca, 1kg, small, no real capacity really but 3 or 4 in series would be fun..,sorry wrong thread really![IMG_8605|666x500](upload://gEJXUVx413Tvd6UHZhwpc6VUm5B.JPG)
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2018-03-04T14:14:21.196Z Reads: 166

```
Would be fun to put in a board or use in a welder?

[quote="banjaxxed, post:6, topic:48114"]
no real capacity
[/quote]
18 Ah, that's pretty decent capacity.
```

---
## \#8 Posted by: banjaxxed Posted at: 2018-03-04T14:32:05.754Z Reads: 162

```
I have an @aulakiria welder/soldering iron but I appreciate what you are doing here & the thought patterns behind it, so interested onlooker :slight_smile:

It's primary duty is too run a starter motor which needs to move 2 x 500cc jugs in a vee config from a cold start. Those cca are needed but forget about it when it's cold outside like now, so it is living indoors untill weather improves.

I bought mine on sale for $200, they are $170 now. Which led me down a rabbit hole on primatic cells and price, there are options there now, camping/propecting power supplys, 4 of them fit neatly between a trampas bindings and do not exceed the height of the strap = 4kg nd easility weatherproofed/wired.
![IMG_8607|375x500](upload://8ZkZ0Ix8dHuXSDgeUSyEYyFpHyo.JPG)

Sorry I will stop polluting your capacitive DIY welder thread!
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-03-14T18:00:43.125Z Reads: 131

```
I received some cylindrical bois.
![IMAG0874|690x389](upload://i0puDYWIIyGEG71glh8n9A3j11j.jpg)

Will have to see how long before the PCBs arrive and wonder when the MOSFETs I was intending in using is back in stock.
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2018-03-16T19:55:32.119Z Reads: 130

```
Boards arrived today and proceeded to solder on the caps. I need to get the copper busbar drilled (shitty metalworking tools at home) and then it's more time wise dependent on when the MOSFETs will be back in stock anywhere, before this project continues, but when it does, I'll update you guys.
![IMAG0882|690x389](upload://nTSDdsC5ylJ9qtaZzOcoudEnOUq.jpg)
![IMAG0883|690x389](upload://tzWoGokfIlgKWPWk68XYkqllWgZ.jpg)
![IMAG0884|690x389](upload://lDaJVdUnMNu2iVyinDgT8080csc.jpg)
```

---
## \#11 Posted by: moon Posted at: 2018-04-10T13:17:25.837Z Reads: 120

```
Nice idea

Have you seen what @whitepony did. He used a 2f supercap, but I don't think it has pulse feature.
```

---
## \#12 Posted by: whitepony Posted at: 2018-04-10T20:37:40.285Z Reads: 117

```
its still up and running, just plain shorting that 2f cap, welds really perfect tbh :slight_smile:

![image|666x500](upload://pK46CWwYNAMGQG3wXOFH2swETCN.jpeg)![image|666x500](upload://iYRHTpNvrOe1IuPbY4oGOhn9A0P.jpeg)![image|375x500](upload://2tX0aTHhvWXH2WjmasaxWnfZKBh.jpeg)
```

---
## \#13 Posted by: moon Posted at: 2018-04-10T20:50:41.168Z Reads: 110

```
It looks great. How often do you need to charge it?

I saw a Youtube video earlier of someone using supercap - a really simple setup. But I don't know the best way to charge it so it doesnt go over the rated voltage

https://www.youtube.com/watch?v=RwTVxZgIoAM
```

---
## \#14 Posted by: whitepony Posted at: 2018-04-10T20:52:36.123Z Reads: 109

```
its constantly hooked up to a battery charger, basically im shorting it too for a splitsecond!
```

---
## \#15 Posted by: moon Posted at: 2018-04-10T21:06:29.454Z Reads: 115

```
And your charger is 12v?

It makes sense now, the video above is using a 2.7v cap. So I need a power source that is regulated at 2.7v or lower?

> Charging capacitors isn't very complicated. The capacitors will charge up to, and hold at, the voltage of your source. Really no need to turn off the source once the capacitors are fully charged. Once the capacitors match the voltage of the source, no more current will flow and the system will be stable*.
```

---
## \#16 Posted by: whitepony Posted at: 2018-04-11T05:27:38.767Z Reads: 113

```
your cap needs tohold the right energy to weld, which, if you dont work with pulse lengths, is just the energy stored in the cap, ie 0.5CU^2, so its easy to tune the energy with the charge voltage!

for me, C is 2F and U is about 17V
```

---
## \#17 Posted by: deucesdown Posted at: 2018-04-11T05:58:09.282Z Reads: 113

```
Didn't read the thread yet but the kweld guy has been worrying away at using super caps for welding. I think he's almost ready to sell a product.

The intent is to use mains power instead of lipo for his welder. He's balance charging the caps? ... Guy knows his stuff, at least on the electronics side.

https://endless-sphere.com/forums/viewtopic.php?f=14&t=89039&sid=4ceb6836b1ca19ff31886adac389809d&start=300#p1370058

He has a similar thread on eevblog.
```

---
## \#19 Posted by: SimosMCmuffin Posted at: 2018-04-28T10:48:07.617Z Reads: 100

```
Finally an actual update on the project!

Got the bus bars finally machined at a local shop and got the necessary bolts, washers and nuts from the hardware store and assembled the cap and switch boards with the bus bars, as shown below.


![IMAG0980|690x389](upload://fs7AscD6NB67zoG0Q7PRWGG7JNq.jpg)
![IMAG0978|690x362](upload://ybJieYPz1lxP4xH8o98cWn5NvGz.jpg)
![IMAG0981|690x389](upload://qUK6EyRuJui57H1H8Gv1IOJhbQy.jpg)
![IMAG0979|690x249](upload://tKehDRtzRXWGO0Wj0MrXLTUfaq2.jpg)

I did a capacitance test using a RC time constant measurement which gave a result of ~0.92 Farads, with the nominal value based of the caps ratings 20 x 0.047 F = 0.94 F is really close. Also accidentally blew a resistor leg, which accidentally shorted the Anode and Cathode bus bars :blush: 

I'm gonna start doing some tests on it's performance this weekend and I'm going to use an arduino as a temporary controller for the welder.
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2018-04-29T11:31:23.908Z Reads: 88

```
![IMAG0982|690x389](upload://g1JdNG0GPHCFHzNv5Si6rpslCLD.jpg)

Driving some serious, high currents here!

https://giant.gfycat.com/WarpedMeekIrrawaddydolphin.webm
```

---
## \#21 Posted by: SimosMCmuffin Posted at: 2018-04-30T14:48:31.294Z Reads: 82

```
It welds!

I have done some calculations on the welding current based on the discharge curve of the capacitor bank during a pulse. Pictured below is a 5 ms pulse with the bank starting at 22.5 V.
![IMAG0985|690x389](upload://uIJDyLfF2dxr5sjLAajemedRg5h.jpg)

By knowing the capacitance of the bank we can with two data points from the curve calculate the current flowing through the electrodes.

Bank capacitance: ~0.93F
1st point: 20.4V
2nd point: 18.2V
time difference: 800µs

Current: (0.93F * 2.2V) / (800µs) = ~2550 A

No problem getting double and triple stacks of nickel strip to weld. Pictured below are the second and third stacks of strip pulled off. Good clean weld points down to the next layer.
![IMAG0986|662x493](upload://7Pa869LlRjWclrA3IirfTjTsvnO.jpg)

At this point I'm more interested in better electrodes.

Would you @whitepony have any tips on the electrodes? I have some of these skinnier electrodes, but I haven't come up with a nice way to attach them to the cables.

![IMAG0987|673x500](upload://flvMl1141FaerXPNLykZ2QOPOAI.jpg)
```

---
## \#22 Posted by: moon Posted at: 2018-10-07T20:41:32.745Z Reads: 63

```
Hi, I know im a couple months late to the question and you probably have an answer but to mount the electrodes I use 

https://www.ebay.co.uk/itm/60A-Electrical-Terminal-Connector-Block-choc-bloc-cable-join-joiner-screw-/272579800717

![image|375x500](upload://sm47l3M45B8Nc3KN55RBlIgpExu.jpeg)
```

---
## \#23 Posted by: DougM Posted at: 2019-01-15T01:54:07.259Z Reads: 49

```
How is this project coming?  Did we decide that the easiest way to implement this was with a 2F supercap and simply load it up to the voltage that gives you the weld profile you want?  I'm not having much luck with my Sunkko 788, it seems to poop out after about the 4th weld, and I'm loathe to invest in a 709 as they are getting bad reviews.

Have we coalesced on this as the best method?

and if I'm reading [this](https://smile.amazon.com/MCIGICM-Capacitor-capacitance-tachograph-Electromechanical/dp/B07BLQGRQY/ref=sr_1_4?ie=UTF8&qid=1547517268&sr=8-4&keywords=supercapacitors) right, I can get 10 3.3F 2.7V supercaps for $10?

The only thing I can think is maybe the leads aren't big enough, but from the picture they look pretty beefy.  

Or am I missing something?
```

---
## \#24 Posted by: SimosMCmuffin Posted at: 2019-01-18T06:50:14.156Z Reads: 35

```
10 of those caps could store enough energy for even heavy welds, but I suspect you're going to be **HEAVILY** limited in your performance by the internal ESR of those caps. The can is **very small** at 8mm dia x 20 mm length so I looked for an equivalent sized and rated superCap at Digi-Key and found the following brand name capacitor

https://www.digikey.fi/product-detail/en/eaton-electronics-division/HV0820-2R7305-R/283-4197-ND/3878077

It's pretty much the same size at 8mm dia x 21 mm length and rated for 3F @ 2,7 Volts. So essentially this is direct apples to apples comparison.

The datasheet shows the ESR to be 80mOhm with the rated pulse current of **only** _3,3 Amps_. **THIS IS A TERRIBLE CHOICE FOR YOUR APPLICATION**. You're not going to get enough current from these to make any sort of welds. In capacitive welding, your capacitors are **everything**, if you can't put in the front cost of buying enough big caps, your welder is going to underperform.

I'd recommend you go for the Li-Po welder solution if you're tight on money. It'll perform better for lower price even if it might not be as long lived as a much bigger, heavier and costlier proper capacitive welder.
```

---
## \#25 Posted by: DougM Posted at: 2019-01-19T02:01:50.593Z Reads: 21

```
Thanks [SimosMCmuffin](https://www.electric-skateboard.builders/u/SimosMCmuffin)!  This is exactly the feedback I was looking for.  I don't mind spending the money on good caps - I just want the thing to work.

If you were going to choose a set of perfect supercaps for the job what would they be?

Is rated pulse current the most important thing?  For instance, [this](https://www.digikey.com/products/en?keywords=HV1860-2R7107-R) one's rated pulse current is 61A, but since there will be 10 of them in series I guess that's my max for the pack.

Should I be looking for more than that?  and should I be looking for an ESR above a certain number?  The above is 0.012 ohms.
```

---

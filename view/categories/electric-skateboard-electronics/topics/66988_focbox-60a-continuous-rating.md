# \[Focbox\] 60A Continuous rating

### Replies: 48 Views: 1017

## \#1 Posted by: somaht21 Posted at: 2018-09-04T07:11:07.037Z Reads: 299

```
I All !

I'm using a focbox with a 4kW motors and  a 12S Lipo Battery.
Everything works fine but the Focbox mosfets gets hot really fast: from 48°C to 76°C in less than 90secondes, pulling maximum 60Amps motor and average 40°C.


You can see the datas here:
https://metr.at/r/ifhNx

The Focbox was inside a box so no cooling but even though, I didn't expect it to get so warm so quickly.

What I don't understand is that the  Focbox is rated for 60Amps continuous. 
Is it only under perfect conditions with a really big fan blowing directly on the fets ? Or maybe is it because my focbox has an issue somehow ?

Any advice/ opinion is welcome here :slight_smile:
```

---
## \#2 Posted by: Acido Posted at: 2018-09-04T07:15:50.008Z Reads: 282

```
If it doesnt limit its amps till it cools down your good
```

---
## \#3 Posted by: Spatt Posted at: 2018-09-04T07:27:54.886Z Reads: 280

```
But you are not pulling all the 60 amps per focbox, maybe you should just put a new silicon pad for cooling. Where are you skating? How many degrees of temperature outside in you country
My conf is dual focbox 12s4p 30q bms 60 amps amps batt 60 no external cooling [https://metr.at/r/XlbKl](https://metr.at/r/XlbKl)
```

---
## \#4 Posted by: somaht21 Posted at: 2018-09-04T07:39:02.263Z Reads: 274

```
It does limit the amp after reaching 80°C which is the cutoff start limit I set up.

The focbox is not used inside a eskate but inside a Epaddle board, so on the water. The motor makes a propeller spin.

Spatt, from your data, I see that the temperature of your focbox doesn't rise as quickly as mine.
```

---
## \#5 Posted by: Acido Posted at: 2018-09-04T07:45:55.036Z Reads: 262

```
I guess thats the reason why, maybe you should have gone with a higher voltage and a diffrent esc
```

---
## \#6 Posted by: somaht21 Posted at: 2018-09-04T07:54:03.978Z Reads: 247

```
You don't really want to go higher than 50V when dealing with water, but indeed, maybe a different ESC would be better. But the Vesc architecture is so good, it's hard to change to something way more restrictive
```

---
## \#7 Posted by: Spatt Posted at: 2018-09-04T07:56:05.551Z Reads: 237

```
I read that water is more stressful for escs than ground. Btw focbox is rated for 60 amps for sure with a different cooling system, more efficient, and you are pulling more amps constantly than me...
```

---
## \#8 Posted by: Spatt Posted at: 2018-09-04T07:57:29.582Z Reads: 234

```
You can choose for a different cooling system using water for example... you should study something like that.
```

---
## \#9 Posted by: Acido Posted at: 2018-09-04T08:19:11.748Z Reads: 221

```
Yea that makes sense lol
```

---
## \#10 Posted by: somaht21 Posted at: 2018-09-04T08:29:29.473Z Reads: 220

```
Yes, I'm planning on mounting the Focbox to an aluminium plate on direct contact with the water. However, I'm wondering if there is not something wrong with the mosfet of temp sensor that would cause this lightning increase of temp.
```

---
## \#11 Posted by: Spatt Posted at: 2018-09-04T09:05:41.118Z Reads: 211

```
You can wait for someone more expert in focbox than me, but if you see carefully your log when the temperature raise it doesn’t drop quickly as mine so it seems like your stock cooling plate is not working at all! I would check first silicon pads, 
make also a photo of how and where you put your focbox, if you put it over the lipo pack for example, something that doesn’t let the focbox cool down.because after the 30 amps drowned it’s 0 amps so the cooling is really too slow
```

---
## \#12 Posted by: somaht21 Posted at: 2018-09-04T09:34:31.698Z Reads: 192

```
The focbox Alu plate is in contact with a big aluminium plate (A4 size) that is in direct contact with sea water, so this big Alu plate is always at 20°C.
I have bought new silicon pads with 8W/mk thermal conductivity and will try it as soon as I receive it.
Also, I will now use this Silicon pad between the Focbox and the big Alu plate that touches the water.
If this doesn't work out, the Focbox is probably the problem..
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-09-04T10:39:51.090Z Reads: 179

```
No you are right original focbox cooling is like a joke... that's why we have made heatsink cases/plates and etc stuff. I am running on 90A batt amps had never seen more than 50ºC on mosfets
```

---
## \#14 Posted by: Blitz Posted at: 2018-09-04T10:57:18.690Z Reads: 176

```
Did you make any modifications to the focbox besides the added cooling?
```

---
## \#15 Posted by: Kug3lis Posted at: 2018-09-04T11:03:15.243Z Reads: 175

```
Not much, I have added some solder on some places as it was bit lacking
```

---
## \#16 Posted by: Spatt Posted at: 2018-09-04T11:42:33.093Z Reads: 166

```
with the silicon between focbox and the aluminum plate in contact with water I think it will be for sure better.
```

---
## \#17 Posted by: somaht21 Posted at: 2018-09-04T13:04:39.692Z Reads: 160

```
Do you have a picture of your setup ? I'm really interested in knowing how to increase significantly the continuous limit current.
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-09-04T13:09:23.845Z Reads: 157

```
Basically this stuff:

https://shop.3dservisas.eu/collections/FocBox
```

---
## \#19 Posted by: somaht21 Posted at: 2018-09-04T13:28:37.191Z Reads: 151

```
Interesting, but it really looks like the one already integradted to the focbox
```

---
## \#20 Posted by: longhairedboy Posted at: 2018-09-04T13:33:19.761Z Reads: 152

```
definitely a lot more resistance with a prop in water than thane on a street. FocBox was designed for esk8, but i think if you can somehow add better cooling you'd be fine. 

Is there any possibility of mounting a sealed aluminum heatskink waterside so that the heat can sink faster? You're in the water, you should take advantage of it.
```

---
## \#21 Posted by: Kug3lis Posted at: 2018-09-04T13:34:31.573Z Reads: 145

```
I think the heatsink plate with proper gasket would work amazing in water... so much surface
```

---
## \#22 Posted by: kuphjr Posted at: 2018-09-04T13:45:40.421Z Reads: 149

```
This should have been the first comment and the thread could have been closed.
```

---
## \#23 Posted by: somaht21 Posted at: 2018-09-04T13:54:42.668Z Reads: 144

```
Yes, way more resistance, but not considering what's connected to the Focbox, if it states 60A continuous it should handle 60A continuous and not going nuclear after only 40A for 30 seconds IMO ?

I first mounted the Focbox to a big 2mm aluminium plate on the bottom of the board, in direct contact with water. This plate is 300x200m so it should dissipate a lot of heat.
The alu plate of the Vesc was mounted to this big plate via thermal grease (Artic MX2 5W/mK) but it didn't stop the mosfet from hitting 80°C super quickly.
```

---
## \#24 Posted by: mars Posted at: 2018-09-04T13:57:06.970Z Reads: 140

```
[quote="somaht21, post:12, topic:66988"]
I have bought new silicon pads with 8W/mk thermal conductivity and will try it as soon as I receive it.
Also, I will now use this Silicon pad between the Focbox and the big Alu plate that touches the water.
If this doesn’t work out, the Focbox is probably the problem…
[/quote]

Hi @somaht21 just a thought for when your designing your solution.

The thermal conductivity of a high-grade thermal paste is 8.5 W/mK, or Thermal pads some 14W/mK . 
The heat conductivity of copper is 385 W/mK, or for aluminum 205 W/mK.  
So the thermal compound is actually a poor heat conductor when compared to the aluminum itself.

In  computers the role of the thermal compound is to fill the tiny gaps between the cooler and the IHS (Integrated Heat Spreader)  promoting thermal conductivity (or just to make some additional heat conductivity possible if the two surfaces are convex or concave). In theory maybe the same holds true for your application solution? 

Some enthusiasts use lapping between CPU and IHS a process in which two surfaces are rubbed together with an abrasive between them thus smoothing the surfaces giving better contact or heat transference. 


Good luck with your solution.
```

---
## \#25 Posted by: Kug3lis Posted at: 2018-09-04T13:58:56.719Z Reads: 123

```
Welcome to esk8 continues power ratings :D Try flipsky 4.20 with 100A or v6.6 with 200A continues ratings :laughing:
```

---
## \#26 Posted by: Pedrodemio Posted at: 2018-09-04T13:59:54.161Z Reads: 126

```
Some FOCBOX had a plastic between the thermal pad and the mosfet’s that should have been removed at the factory

Make sure yours don’t have it
```

---
## \#27 Posted by: somaht21 Posted at: 2018-09-04T14:14:30.188Z Reads: 127

```
These values (100A & 200A) are for Dual setups right ? It indicates "only" 60A continuous for single ESC 6.6, which is what Enertion has rated his focboxes =(
```

---
## \#28 Posted by: somaht21 Posted at: 2018-09-04T14:17:34.304Z Reads: 130

```
I've checked it already but nothing on the silicon.

@Mars, Thanks for the info, really intersting. But as you said, unless you have 2 perfect surfaces in contact, you'll need thermal grease or thermal pad right ?
In this case, I'm only using thermal pad for the contact between FETs and Focbox heatsink and Focbox and Alu- plate.
Let's see what the next trial shows. I'll let you guys know.
```

---
## \#29 Posted by: Andy87 Posted at: 2018-09-04T14:18:00.015Z Reads: 131

```
https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink

For the dual it’s 100a per single stated on there website 
🤔 strange sentence 😅
But I think you understood
```

---
## \#30 Posted by: Pedrodemio Posted at: 2018-09-04T14:19:36.832Z Reads: 129

```
You could use the thinnest thermal pad you manage to  find and make a copper or aluminum spacer, this should improve conduction a lot

Just make sure to avoid electrical contact
```

---
## \#31 Posted by: somaht21 Posted at: 2018-09-04T14:29:37.476Z Reads: 128

```
That's weird, Single 60A but one side on a Dual 100A..
I wouldn't trust the 100A then!
```

---
## \#32 Posted by: mars Posted at: 2018-09-04T14:44:11.222Z Reads: 125

```
Yes as I understand it you still need to use a thermal compound.
I haven't used thermal pads. The paste is applied in very thin layers to fill the tiny gaps between the cooler and the IHS or just to make some additional heat conductivity possible if the two surfaces are convex or concave.

So the smoother the surfaces are to start with the better the result.

As @Pedrodemio suggests the thinnest thermal pad a copper or aluminum spacer, avoid electrical contact lol
```

---
## \#33 Posted by: Blitz Posted at: 2018-09-04T14:47:07.899Z Reads: 122

```
So basicly we haven't moved from vesc 4.12.
we need higher voltage Esc's (I know your working one one)
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-09-04T14:47:25.475Z Reads: 122

```
Mosfet case itself is a pin, you need isolating thermal pad or etc stuff
```

---
## \#35 Posted by: E1Allen Posted at: 2018-09-04T19:20:31.827Z Reads: 110

```
If you look at the middle of this ride you can see a 27sec Hill climb where mosfet temps get up to 62c. Battery amps between 35-45a.  This is with the focbox cooling case. So I guess the definition of continuous has to be defined.

https://metr.at/r/1v20t
```

---
## \#36 Posted by: Deckoz Posted at: 2018-09-04T21:44:36.462Z Reads: 102

```
I literally just add aluminum mass.. Evo has no external cooling and an extra 1/4" thick piece of aluminum big enough to rest two Focbox on top off and screw them to the plate. The only cooling issues I run into are with the motor.
```

---
## \#37 Posted by: somaht21 Posted at: 2018-09-05T08:21:39.653Z Reads: 88

```
Really interesting datas.
It's pretty much the same for my focbox. When ppulling 35Amps,  the temp doesn't increase that much but passing 50A it just starts going crazy.
I guess 60A continuous is in the best case scenario with a fan blowing cool air on the heatsink.
I'll try the new thermal pad soon but if it doesn't work out --> Vesc6 !
```

---
## \#38 Posted by: Cobber Posted at: 2018-09-05T08:28:45.299Z Reads: 87

```
I thought around 45a was the focbox ceiling? I know DeckyBro has been running high voltage low amps...
Above 45a you run into temp. prob.
So your observation of >50a overheating sounds right :no_mouth:

as for v4.12 I thought that was max 28-30a

How many Amps are you running @Deckoz?
```

---
## \#39 Posted by: somaht21 Posted at: 2018-09-05T10:09:38.544Z Reads: 87

```
On Enertion's website it's written "60A continuous - 120A Burst". 
For me, "continuous" means that you  could have it run for 10 minutes without reaching the FETs temp limit (so around 80-90°C). From my experience and what I've read, it's just not true.
```

---
## \#40 Posted by: Cobber Posted at: 2018-09-05T10:19:41.353Z Reads: 89

```
No it is not.

& to be honest pushing a prop through water is like trying to ride through quicksand!
So likely you will need to be conservative as compared to a eSk8.

Even with a VESC 6... I'm not sure if you could load it with 80a for 10 minutes without thermal cut-off just because I have not seen anyone do that in the real world, only static tests by Vedder. And then his design has been shown to be limited by thermal transfer hence the proliferation of heatsinks for all designs. No doubt v6 is a big step up from v4 but it still has limitations.

So many variables from battery to loom to speed controller to loom to motor... and everything else in-between.
```

---
## \#41 Posted by: somaht21 Posted at: 2018-09-05T14:34:20.495Z Reads: 84

```
I've ordered the  100A Vesc 4.xx based Maytech Esc. Let's see what it can handle
```

---
## \#42 Posted by: Kug3lis Posted at: 2018-09-05T14:42:40.470Z Reads: 86

```
I wouldn't expect much more than you get now ;)
```

---
## \#43 Posted by: Cobber Posted at: 2018-09-05T14:54:25.749Z Reads: 87

```
i'd rate a focbox above a maytech v4...

there are three levels of adjustment, battery, motor & absolute.

might be a good idea to bone up on vesc settings before you do a (rip) "bigbro" and burn up a hand full of controllers & become the wizards best customer!
```

---
## \#44 Posted by: Dazeto Posted at: 2018-09-05T23:38:05.716Z Reads: 77

```
i run a 12s4p dual motors at batt max 30A (30A each vesc= 60A) and they are fine, no overheating at all. i tried 35A( 70A for both) and even the enclosure got hot, i could touch it and feel the heat on my hand.
 i saw a video of Vedder testing currents and he said vesc 4.1x can take 34A or so continuous.
```

---
## \#45 Posted by: lrdesigns Posted at: 2018-09-06T01:46:18.091Z Reads: 69

```
[quote="somaht21, post:41, topic:66988"]
I’ve ordered the 100A Vesc 4.xx based Maytech Esc.
[/quote]
I don't think anyone here has tested it with such a high load yet. I would be a big surprise if the performance is much better than focbox which is the current king of V4 vescs. 

Are you running in BLDC or FOC? I think BLDC runs a bit cooler. On the focbox you could run 13s and lower amps for similar power. 

Is your prop geared or direct drive? A higher gear ratio is a 100% certain way to lower temps. 
![image|419x303](upload://snvdcdIE39t95xI2Ujw5EThWNms.jpg)
```

---
## \#46 Posted by: Dmaxx Posted at: 2018-09-06T03:14:47.257Z Reads: 62

```
I'm currently running 12s @ 65amp battery max on 170kv 6374 single drive on sensored foc with the new maytech 100amp esc and it has been amazing! Once my new metr pro module shows up I can record a ride and verify temps are stable. I can verify a flawless performance so far ~60miles riding pretty hard and going up big Seattle hills no problem
```

---
## \#47 Posted by: somaht21 Posted at: 2018-09-06T08:09:05.273Z Reads: 57

```
I'm runing in BLDC, no need for the FOC mode.
My prop is direct drive. The idea is to have a really easy setup.
I only need to pull 70A for about 30 seconds, then it should drop down to 40A continuous. But so far, the Focbox can't see 70A continuous without raching 80°C and limiting the Amps pulled.
```

---
## \#48 Posted by: somaht21 Posted at: 2018-09-06T09:04:44.529Z Reads: 56

```
From the datas I've collected here and there, not so many people have tried it out but those who did are really thrilled by the power it can handle.
I'll let you know if it does what it's supposed to and if it can handle 80A continuous like Maytech said.
If so, this coould be a real game changer for many e-mtb riders out there. Capable of climbing walls for the price of a focbox !
```

---

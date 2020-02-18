# When does your bms really balance?

### Replies: 30 Views: 4150

## \#1 Posted by: Hummie Posted at: 2017-11-23T06:26:50.956Z Reads: 220

```
all the ones I've been looking at have the same function where they balance by discharing a tiny amount through a resistor only when the cell hits 4.2.   All the bms I've seen have the balance current of about 68mah.  That's tiny and unless the pack is being charged by a very slow charge a single cell could easily be getting fed more than 68mah so still taking a charge beyond 4.2  

Can you explain everything on the description:
https://bmsbattery.com/bmspcm/733-10s-16s-50a-lipo-bms-system-battery-management-system-bms-pcm.html


I dont understant the over-voltage protection because if the bms were able to stop charging a single cell at 4.2 then there wouldnt need to be a balance function

http://liionbms.com/php/bms_options.php#Digit._balancers
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-23T06:32:13.825Z Reads: 213

```
During the CV stage the current decreases rapidly. 
For instance a 10S pack will hit 42V while charging before the pack is actually 42, if you disconnect the second it hits 42, the pack could easily drop down to 41v. The CV stage starts once the charger hits 42 at constant current, then starts decreasing current at a rate fast/slow enough to maintain the 42v till it hits 10% rate of original charge current and stops charge
```

---
## \#3 Posted by: scepterr Posted at: 2017-11-23T06:37:28.730Z Reads: 207

```
Also, all these BMS are meant to keep new, balanced packs in balance, not balance mixed, aging, drifting packs.
```

---
## \#4 Posted by: Hummie Posted at: 2017-11-23T06:40:19.077Z Reads: 200

```
I believe my power supply works with a constant voltage. I set it to a certain voltage and hook it to my pack and it will charge to that voltage and decrease the current on the way up there.  when it gets near the full charge, lets say 50v, it does slow down the current but if there were a bad cell in the pack how would that play out?  If a bad cell were to hit 4.2 while everything else were even as high as 4 volts, and the power supply is still feeding 8 amps, which is common, and if the discharge balancers only are able to burn off 86mah,...that cell will go much higher than 4.2 unless there's some other feature that comes into play.

bms for only new balanced packs in balance?!  that defeats its purpose though.   eventually a pack will age and drift.
```

---
## \#5 Posted by: scepterr Posted at: 2017-11-23T06:42:13.811Z Reads: 194

```
If you have a pack with a cell .2v apart from all the others, that cell needs to be replaced. These BMS aren't meant for fixing unbalanced packs
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-23T06:42:58.416Z Reads: 190

```
A properly built pack with matched cells will not drift through hundreds of cycles
```

---
## \#7 Posted by: Hummie Posted at: 2017-11-23T06:43:09.122Z Reads: 185

```
so how would it end for a pack with a typical bms that did happen to have a cell with .2v variation?
ive had that happen many times with lipo that I've damaged
```

---
## \#8 Posted by: scepterr Posted at: 2017-11-23T06:43:42.748Z Reads: 181

```
Often times the BMS itself is faulty and burning energy somewhere
```

---
## \#9 Posted by: Hummie Posted at: 2017-11-23T06:46:25.975Z Reads: 175

```
I'm looking for how a bms DOES help and all I'm finding is it's false sense of security and youre adding to that belief

but I'm only talking of the balance function, how will it's other possible functions do something productive in such a case with an unbalanced cell.   Other than damaging a lipo, which is relatively easy to do, there could be cells getting cooked due to how the pack has the cells arranged.  or maybe the cells were soldered badly
```

---
## \#10 Posted by: scepterr Posted at: 2017-11-23T06:50:44.778Z Reads: 174

```
This will do 6A constant, 10A burst active balancing
http://diytechandrepairs.nu/1s-modular-active-balancer-reviewed-and-trashed/
The title is misleading,^ it's good 😋

The guy reviewing is daromer on www.diypowerwalls.com
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-23T06:56:37.700Z Reads: 161

```
In terms of what will happen if a cell goes bad and drifts to the BMS....I imagine the traces for that cell on the PCB would burn up and/or the components on that line
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-11-23T06:57:26.302Z Reads: 159

```
There are also BMSs that start balancing earlier than 4.2v. Mine has configurable settings and I have it set to start balancing at 3.7, so it's ALWAYS balancing. Sure, that may waste a tiny percentage of the power in the balancing, but I don't have to worry about cell drift, like, EVER.
```

---
## \#13 Posted by: Hummie Posted at: 2017-11-23T07:08:49.865Z Reads: 148

```
what bms is that?  I don't understand you saying it would waste more energy in it's always balancing.  the alternative being have a cell that's too high?

maybe I don't understand how a bms works.  Does the high voltage cut-off shut current going to the whole pack and stop the charging if any cell hits that?
that single cell balancer is surprisingly big and expensive considering id does nothing else.   but it's "active" and transfers the overfilled cells to the lower filled and that's ideal. i'm still looking!
```

---
## \#14 Posted by: Eboosted Posted at: 2017-11-23T07:14:43.781Z Reads: 150

```
The more I know about BMSs the less I want to use them on my builds, nevertheless, I'd never recommend anyone to run without one. 

After 1 year riding my Vanguard with bms only for charging I've never seen any of my cells drifting, if the connections are good, they wouldn't drift at least it has worked for me.

I never run them below 3.2v, usually 3.6v before it's connected to the charger.

The overcharge function on my Street Carver kicked in several times, cutting all current supply to to battery during charging at 3A, when one pack peaked 4.3v, as soon as I switched to 2A for charging everything was smooth again
```

---
## \#15 Posted by: MysticalDork Posted at: 2017-11-23T07:26:21.558Z Reads: 148

```
It's an 80a BMS from aliexpress. All the BMS we use for esk8 are passive, so that means every time it balances a cell, it's wasting some energy. Might not be a lot, but my guess is that having the balancing start earlier probably has some small impact on the overall energy lost as waste.

If one cell goes seriously overvoltage (like 4.3 or whatever the maximum overvoltage setting is) then the BMS will shut off until it has balanced that cell down to match the others.

The active balancer has quite a bit of active power control circuitry in it, to step up the cell voltage, send it, receive from another one, and convert that back down to charge its cell, as well as communicate with the other modules. Very sophisticated system. Not really necessary for our small packs, but definitely needed for powerwalls, large EVs, etc, that can be well over 10KWh.
```

---
## \#16 Posted by: deucesdown Posted at: 2017-11-23T07:39:49.981Z Reads: 141

```
Link dammit :)
```

---
## \#17 Posted by: MysticalDork Posted at: 2017-11-23T08:00:58.972Z Reads: 139

```
What, the BMS I have? I warn you, it's pretty large and the shipping can be unpredictable. @stormboard1 has one, and it took him ages to get it. https://www.aliexpress.com/item/36V-Bluetooth-BMS-for-10S-42V-Li-ion-Battery-PCB-board-with-80A-constant-charge-and/32826867315.html
```

---
## \#18 Posted by: lowGuido Posted at: 2017-11-23T10:58:06.682Z Reads: 129

```
[quote="Hummie, post:9, topic:39058"]
I'm looking for how a bms DOES help and all I'm finding is it's false sense of security
[/quote]

finally your eyes are open.
```

---
## \#19 Posted by: TarzanHBK Posted at: 2017-11-23T14:46:03.196Z Reads: 117

```
This forum is like:

_"A BMS is really helpfull and everyone should use one!"_

+one month later+

_"Fug those BMSes, they kill packs!"_

< repeat every month >
```

---
## \#20 Posted by: lowGuido Posted at: 2017-11-23T15:01:48.868Z Reads: 112

```
some people are all "OMG you should only use BMS WTF! DO you want to EXPLODE?!"

and then other people actually understand the electronics in the BMS are like.. uhh yeah they are nice to have. but they aren't magical unicorns that save you batteries from all demons.

they are a board that does 3 things:
make charging 1 plug
bleed resistors on higher voltage cells
FET switching for low volt cutoff

that's all. nothing more.
they are handy. they are not gods. 
and if you are diligent, they are not necessary.
```

---
## \#21 Posted by: TarzanHBK Posted at: 2017-11-23T15:25:25.373Z Reads: 106

```
Amen to that!
```

---
## \#22 Posted by: Hummie Posted at: 2017-11-23T17:41:21.311Z Reads: 105

```
and high voltage cut off too no?  that seems the most important for not blowing up.

looking at the details on this 80amp one from battery support I'm going to annotate it and hope someone can add their own or tell me if i'm wrong or right.

http://www.batterysupports.com/44v-48v-504v-12s-80a-12x-36v-lithium-ion-lipolymer-battery-bms-p-392.html

Technical Parameters:
Balanced current: 60mA (VCELL = 3.90V when)    **starts balancing when a cell over 3.9 with just 60ma**
Balanced for: 4.20 ± 0.05 V
Over-charged Protection: 4.2 ± 0.05 V    **will shut the charging off to all cells if one hits 4.2**
Over-charged Release: 4.05 ± 0.05 V     **?waits till the high cell all the way down to 4.05??**
Over-discharged Protection: 2.9 ± 0.05 V  **shuts down output of all cells at 2.9**
Over-charged delay: 5mS  **whats this 5secs?  till it shuts off?**
Over-current Protecton: 80 A **shuts down power out of battery if over 80 done?**
Supports Max. Continuing Discharge Current: 80A  **?but somehow will do the 80 continuous?**
Static power consumption: less than 200uA
Short-circuit protection function: disconnect the load from the recovery.
 
Dimension: 200mm * 110mm * 20mm (L*W*T) - with Radiating Board
 
The main functions: Over-charged, Over-discharged protection, short circuit protection, over-current protection, with Balancing function.
```

---
## \#23 Posted by: lowGuido Posted at: 2017-11-23T18:06:54.777Z Reads: 98

```
high voltage cut off is usually taken care of by your supply. in the case of a 12S pack you use a 50.4V supply.
4.2V x 12S = 50.4V therefore your supply will not allow you to charge more than 4.2V per cell because it physically can't.
the "protection" will probably shut down if you hook up a supply that too high voltage.
if one cell reaches 4.2V before the others while charging, a bleed resistor is switched across that cell  (presumably @ 60mA ) this happens apparently within 5 milliseconds.

the 80A current refers only to the switching component and is related to the amount of FETs and what they can handle.  
For what its worth the only difference between a 20A BMS and a 100A BMS is the amount of switching FETs and what they can handle.
80A continuous is a bit of a lie if the over current is set at 80A LOL
```

---
## \#24 Posted by: Hummie Posted at: 2017-11-23T18:09:15.427Z Reads: 91

```
my bulk supply will definitely charge individual unbalanced cells higher than 4.2 with my bulk supply at 50v.
I understood that this bms would start balancing at 3.9.  Otherwise, which I've often see, where the balance function starts at 4.2.. that makes no sense if the pack will have a safety over-voltage per cell at 4.2 as well.  no time to balance.  but labels seem to say anything.
```

---
## \#25 Posted by: lowGuido Posted at: 2017-11-23T18:10:44.252Z Reads: 89

```
that's because you bleed resistor can't discharge faster that you can charge.
```

---
## \#26 Posted by: Hummie Posted at: 2017-11-23T18:17:10.836Z Reads: 91

```
i'm saying the supply doesn't do anything other than feed 50v regardless of what the individual cells at.   no safety feature there to protect a cell and that's what the supposed point of the bms is.  
am I right in thinking that the whole pack will stop charging or discharging if any cell hits the low voltage cut off or the high?

how about those many bms that state 4.2 is when it starts to balance...and also when the high voltage cutoff is?  or maybe it's just more empty writing.
```

---
## \#27 Posted by: PXSS Posted at: 2017-11-23T18:26:55.487Z Reads: 88

```
<img src="/uploads/db1493/original/3X/8/a/8a918661270dd37bab7cb9d73de703a59c56a7e2.GIF" width="267" height="200">
```

---
## \#28 Posted by: Hummie Posted at: 2017-11-23T18:33:36.861Z Reads: 84

```
that's disgusting
```

---
## \#29 Posted by: PXSS Posted at: 2017-11-23T18:37:09.653Z Reads: 82

```
I'll try to explain it tonight if I have time
```

---
## \#30 Posted by: Hummie Posted at: 2017-11-23T18:42:15.813Z Reads: 82

```
oo and while youre at it can you tell me if I could modify this

https://www.aliexpress.com/store/product/10S-4-2v-li-ion-balancer-board-li-ion-balncing-full-charge-battery-balance-board/1821822_32728243247.html?spm=2114.12010612.0.0.61c7e4f4s2VAhl

to have greater discharge ability by adding bulbs or different resistors. be cool looking if it had tiny bulbs that I could see through my enclosure.  and I'd also like to reduce the voltage it starts to balance.

ive got a couple 13s versions coming in the mail and assume I'll be about to do 12s
```

---

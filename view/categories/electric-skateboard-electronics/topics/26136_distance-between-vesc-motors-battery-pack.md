# Distance between vesc - motors - battery pack

### Replies: 11 Views: 1233

## \#1 Posted by: banjaxxed Posted at: 2017-06-25T11:43:36.375Z Reads: 172

```
I'm in the process of a Mtb build but still shaping out the design as I go along. From reading threads here I've discovered that distance of vesc to battery is sensitive on 4.12 hardware unless extra capacitors are installed. But I plan to keep the dual vescX's and battery in the same case...so there is not much info on that setup.

It's possible I think but what are the effects on motor response?

Is there any way to combine the six motor cables from the enclosure i.e. 3 cables splitting into 6 cables just before motors?

What are the effects of really long motor sensor cables?

Is a 10s7p Samsung 30q pack enough to drive 6384(3500w) dual motors or should I go to 12s?

Oh and thanks for any replies
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-25T12:21:04.286Z Reads: 174

```
Doing the 3 to 6 split probably won't work out for multiple reasons, main one being the VESCs aren't going to be 100% synchronized and the motors will have their own calibration that will be slightly different (hence the lack of synchronized signal).

Regarding the distance between the batteries and the VESC I haven't had a problem and have pretty long 14ga wires from the batteries to the VESC on a 10S setup, but also curious if you can link to one or two of the places you saw it being talked about as an issue?

Regarding the power delivery just need to look at a few things really, given the wattage and a known voltage you can compute the amperage that needs to flow to fully power those motors... that said the specs are probably rated above what it will actually typically be using... I have a 2200W motor but typically at 40ish Volts I only draw about 6-10A most of the time so usually only hitting up to 400W just because I'm not constantly accelerating or going up a hill.  Once you get up to cruising speed you're typically not drawing much current.  Anyhow you could compute the max current then knowing the resistance of the wires you can calculate the power loss in the wire due to heat and all to figure out what it all works out to in theory then you know assume you have extra losses in reality that aren't accounted for (and VESC efficiency etc.).  Resistance in a material is roughly a constant per unit length so adding double the length basically doubles the ohm value for the resistance but not sure why else that would be an issue regarding distance between the battery and the VESC.
```

---
## \#3 Posted by: mwkeefer Posted at: 2017-06-25T19:35:30.502Z Reads: 128

```
Banjaxxed,

Good catch, it's not just the VESC this presents a problem with but nearly every controller I've tried (RC, EV, eBike, etc) over the last 10 years.  

The technical issues of  long cables in general is two fold... first the long wires as already explained will increase the impedance or resistance of the length thus dropping the voltage and / or heating up so basically it's a garden hose but it's too thin to flow enough power to your pressure washer (in this case the ESC).. the capacitors help on the battery side because they allow the ESC to deliver transient bursts and they prevent or help to prevent the real killer of ESCs on long cable runs, the build up of eddy currents.

Now as far as sensor cables (hall sensor, ntm35 thermal or thermistor), while temperature and "variable" level signals may be attenuated or lose some amplitude over a long cable run, hall sensors are straight up 3 Parallel Bits or just on and off.. since they swing is 0v to 4.7-5v it's very unlikely there would be an issue introduced.

There are a ton of issues I'm skipping here, common sense rules here: Keep all wires as short as possible while being serviceable, use sufficient gauge and quality silicone or ptfe jacketed low resistance wire for power and phase (I use something like 24g silicone for my signal lines just for thermal and short resistance and flexibility, it really doesn't matter as long as the wire you use here won't fracture with vibrations), 

Combine them sure... I head to my auto parts shop and get carbon fiber looking conduit tube... I pass all  6 wires from the enclosure contained in a single cable which splits to a Y within the truck area and each 3 phase side is then passed to the motor in another, thinner conduit tube - I've seen guys use 5/8, 1/4 and 1/8' auto hot rod hose wrapping for effect but you can't combine the phases - two motors, two controllers, 6 phases and 3 each (plus sensors).

Samsung Q30 is 15A maximum continuous discharge in 1P and 3000mah if memory serves, so it's not a matter of can that pack handle the dual 63xx series BLDCs it surely can as 7P it will be 21AH and capable of 5C discharge continuous or 5 * 21 = 105 Amps Continuous, I'm not sure the peak discharge rate but this is fine...  now your voltage is only 37v nominal and while you don't specify your motor kV ... I'm guessing around 190kv so currently the motor can spin up to 37v * 190 = 7030 RPM (this is not 100% accurate since it would be at 100% efficiency, think more like 85% loaded efficiency and that would be 7030 * .85 = 6022.25 RPM actual.  Moving to the 12S would up your maximum motor RPM to 44.4v * 190 = 8436 RPM or at 85% efficiency 7170.6 RPM.

In addition to the higher RPM which obviously translates to higher top speed and likely faster acceleration it also means more power to some extent.. again pulling from thin air, VESC x 2 @ 45A Each Continuous / 100A @ 15 second peak current so your power will go from 37v * 45 Amps * 2 ESCs =  3330 watts continuous power and 37v * 200 A = 7400 watts peak or surge to 44.4 * 45 * 2 = 3996 watts constant (nearly a full HP, 666w constant power upgrade) and burst power of 8880 watts (2 FULL HP MORE PEAK POWER).

To sort speed, if you presently on 10S have a "top speed" (assumes 83mm wheels and 16:36t gearing) of 6022.25 RPM / 336 * 83mm||3.27" / 2.25:1(36t:16t) = 26 TOP SPEED and going to 12S would in theory give you: 7170 RPM / 336 * 83mm}}3.27" / 2.25 : 1(36t:16t) = 31 MPH TOP SPEED

Now even though the 10s7p is fine, if you can go to 12s for a reasonable fee.. do so, the system will run cooler and more efficiently (or can).

I listed the math to calculate speeds, rpm and no-load or loaded kV and RPM to expect so you can adjust to fit your numbers and build.

If I may offer one bit of advice, while yes some in the community have reinvented the wheel... don't, if you stick with a somewhat "standardized" layout with the ESCs located nearest to the motors as possible and the battery other side then keeping your wiring short, neat and efficient should be super easy.

Hope it helps!

-Mike
```

---
## \#4 Posted by: banjaxxed Posted at: 2017-06-25T19:43:11.404Z Reads: 104

```
Thanks for the detail, here's the threads
https://www.electric-skateboard.builders/t/motor-cables-longer-than-1m/17641/8

https://www.electric-skateboard.builders/t/3-foot-long-motor-phase-cable-issues/14640

I will use 10awg silicone cables in a sheath of course, thanks for the explanation of not combining cables, it makes sense
```

---
## \#5 Posted by: banjaxxed Posted at: 2017-06-25T19:45:45.480Z Reads: 94

```
Thanks Mike, that helps, the sensor cables I will have to make, but will use quality cables as advised. 

The motors are kv130
http://alienpowersystem.com/shop/brushless-motors/alien-6384-sensored-outrunner-brushless-motor-130kv-3500w/

I'm now thinking that I will add another 14 cells for 12s since these are VESCs with direct get afaik

Appreciate it Alan
```

---
## \#6 Posted by: wafflejock Posted at: 2017-06-25T19:52:02.318Z Reads: 83

```
Yup just some thoughts since I did have my cables going across a long board initially with the separated setup.  Currently I switched to an old school deck since it got a bit more space between the trucks than a modern board (along with some extra girth) but is obviously smaller than a long board so now the cable length isn't really a problem but good to be aware of.  Also thanks for the details @mwkeefer all sounds reasonable just saw someone using this calc for the equations too http://calc.esk8.it/ seems handy
```

---
## \#7 Posted by: banjaxxed Posted at: 2017-06-25T20:04:41.546Z Reads: 77

```
I tried out the calc with my setup the 10s should hit abiut 26mph weighted (71kg), 12s will get another 4mph bit how I would get there with another 2s would also feel very different I would imagine, probably worthwhile for the cost of another 14 cells food for thought thanks

Calcs made with 9" primos - what I'm thinking
```

---
## \#8 Posted by: mwkeefer Posted at: 2017-06-25T20:16:09.190Z Reads: 77

```
Banjaxxed,

if your at 130kv, yeah brother go for 12S !!!

What size wheels bud?

Direct FET is just a package gimmick, but yes VESC = 12S @ 130kv = No Problems :slight_smile:

Silicone Quality :). I actually use turnigy 8/10/12G power and phase cables and their RC ESC silicone wire (3, 4 and 5 conductor available last I checked) which is like 24awg computer ribbon cable that won't fray..  Some JST connectors for the VESCs soldered on at the ends and whalla :slight_smile:

Another hint, on all my builds (eBikes, eSk8, EVs, etc) I use low temp hot glue (I know oxymoron but its at every Walmart across the country), just a drop on each connector wired up to ensure they stay seated with vibration, etc... nothing more frustrating than an intermittent issue with the controls lets alone a blow ESC.

One last tip, keep all power cables and more importantly all 6 phase wires EXACTLY the SAME LENGTH... it may sound trivial but it can prevent a whole host of issues down the road.

Yeah going to 12S would widen and/or extend the "power band" feeling of acceleration, if your trying to get a "feel" for 12S, you can always increase your motor pulley teeth by 1 or 2 or reduce your driven wheel pulleys a few teeth and achieve close to the same effect without investing in consumables and investing time and money.

9" primos, what wheels?  Haha!!

130kv and 85% efficiency so loaded kV (within rated motor spec for loads) would be 130 * .85 = 110.5 * 37v = 4088.5 RPM, still don't know your reduction (and hate algebra) so assuming 2.25 : 1 again with 9" wheels now works out to 4088.5 / 2.25 = 1817.1 / 336 = 5.408 * 9" = 48.67mph

Wait what am I not getting about your posted setup, what reduction ratio will you be running?

No matter, your on the right track!

-Mike
```

---
## \#9 Posted by: banjaxxed Posted at: 2017-06-25T20:19:53.530Z Reads: 65

```
Cheers pal, motor will probably be 15t or 16t, on the hub the pulley will be somewhere between 60t and 70t, primos are 225mm but starting out with the regular 8" tyres that are on the board I got.

Nice tip on the hot glue I was thinking those connectors could do with a dab
```

---
## \#10 Posted by: Minim Posted at: 2017-06-25T20:55:51.762Z Reads: 58

```
The issue with longer battery wires on the ESC is not resistance but the inductance in the wires when extended. The ESC produce high voltage spikes when it's modulating with PWM and every time it goes OFF, a voltage spike higher than input voltage is generated. The longer the battery wires are the higher this spike is amplified and the higher voltage of the eletronics inside the ESC will get. The input capacitors on the ESC will catch (some of) these spikes but if they get to high they will heat up and kill the caps and voltage spikes will get past them. It can be "fixed" by adding more small capacitors with low ESR and a voltage rating well above your voltage. On a 6S setup I measured 33volt spikes when battery voltage was only 24volts as a pointer.
```

---
## \#11 Posted by: banjaxxed Posted at: 2017-06-25T20:59:50.453Z Reads: 56

```
I thought spikes were the result of long cables between the esc and battery negated by extra capacitors, my setup would have the battery and escs close together in the same enclosure with the motors the distant link...are we talking the same setup? Thanks
```

---

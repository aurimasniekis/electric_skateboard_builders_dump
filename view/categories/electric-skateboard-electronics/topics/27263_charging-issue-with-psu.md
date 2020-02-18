# Charging issue with psu

### Replies: 17 Views: 783

## \#1 Posted by: pau Posted at: 2017-07-10T18:32:31.654Z Reads: 73

```
hey
i just want to charge a 2 x 3s lipo with 8000mAh.
i bought a psu with 120 watt and 24V. I adjust the psu to 25,2V. [PSU - Link]( http://www.ebay.de/itm/DC12V-24V-2A-30A-Netzteil-Trafo-Adapter-Treiber-Power-Supply-LED-Strip-Lampe-DE-/162296585279?var=&hash=item25c9a15c3f:m:m5fnVz9DxDHAxF6ZJYM4NFQ)

but when i charge the battery. the ampere meter just shows 0,0 or 0,3A. But it has to be ~4,5A. [link to Ampere meter](http://www.ebay.de/itm/DC-0-10-A-LED-Digital-Amperemeter-Stromsanzeige-Strommesser-Einbau/222118792852?ssPageName=STRK%3AMEBIDX%3AIT&var=520972127995&_trksid=p2060353.m2749.l2649)

here is my schematic. what is wrong? i know there is a bms missing. i just removed the bms to find the issue.
<img src="/uploads/db1493/original/3X/6/f/6f190a6943b4b28abb3f519d4ee6936ee02715bf.png" width="690" height="272">
```

---
## \#2 Posted by: Challlsss Posted at: 2017-07-10T19:33:02.518Z Reads: 61

```
why is ground connected to the negative end of the batteries?
```

---
## \#3 Posted by: pau Posted at: 2017-07-10T21:07:15.737Z Reads: 52

```
Im Not sure, what do you mean with ground?

The battery negative wire is conncetd to ampere meter. And The ampere meter is conncted to The negative psu lead. 
So all in all. The negative battery wire is "directly" conncted to The neagtive psu.
```

---
## \#4 Posted by: goldenHusky Posted at: 2017-07-10T21:13:41.628Z Reads: 48

```
For me it looks like that your amperemeter is wired parallel to the psu/ batteries.
```

---
## \#5 Posted by: pau Posted at: 2017-07-10T21:40:33.668Z Reads: 49

```
<img src="/uploads/db1493/original/3X/2/6/26af3a851cb32f4975121bc7b369c9803b09a6d8.JPG" width="300" height="300">

Stromquelle = psu
Verbraucher = battery 

I think The ampere meter is seriel
```

---
## \#6 Posted by: goldenHusky Posted at: 2017-07-10T22:03:06.281Z Reads: 45

```
[quote="pau, post:5, topic:27263"]
I think The ampere meter is seriel
[/quote]

Yea, you are right, the supply wire for the amperemeter itself confused me, didn't check the link.
How did you adjust the 24V psu to 25,2?
Did you measure the voltage of the 6s configuration?
Maybe the psu only supplies 25,2V with no load and as soon as there is a load it breaks down to a lower voltages.
```

---
## \#7 Posted by: pau Posted at: 2017-07-11T11:38:13.753Z Reads: 39

```
there is a adjuster on the psu. 
<img src="/uploads/db1493/original/3X/8/7/878dcf937baf187b91040aa98662138a183708f7.jpg" width="500" height="500">

the battries have 22.3 Volt. so there are flat and have to load.

if i adjust the psu to 25,2V the ampere should be 4,7 A. because the psu has 150 Watt. 

is the psu maybee broken?
or are the battries broken?
```

---
## \#8 Posted by: krloz Posted at: 2017-07-11T12:09:41.503Z Reads: 35

```
Leave it a couple of hours connected and check if the batteries charge (voltage riser In  the batteries). If it does rise your ampmeter is bad.  If it doesn't your psu is bad.  Then you can go on from there

This is unless you have a multimeter to check if the pay is actually giving power
```

---
## \#9 Posted by: pau Posted at: 2017-07-11T13:52:35.408Z Reads: 30

```
it is charging but very very slow. 
it charged 0,2 Volts in 2 Hours. I think that is to slow.

i also used a multimeter. instant a ampere meter. the multimeter shows the same value.


so all in all.
is the psu broken?
```

---
## \#10 Posted by: krloz Posted at: 2017-07-11T15:23:20.365Z Reads: 26

```
There you have it.  I'm guessing if you set the psu for exactly 25.2V is because you hooked the multimeter to the psu and measured said voltage.  So your psu is giving voltage but at a ridiculous low amp level.  You could try to hook it to some type of resistive load to check it's the psu not giving and not the batteries not accepting, if that is even a thing.  But I'm rooting for the psu is not working properly.
```

---
## \#11 Posted by: Hummie Posted at: 2017-07-11T15:31:22.113Z Reads: 25

```
I've a wattmeter attached to the power supply so u can see exactly what's happening. They always charge fast when the pack voltage is low and just slight trickle when it's almost full.  If the pack is too low though I get an on and off noise and it's very slow and I have to turn the screw down. Without a wired-in wattmeter it's hard to know what's going on when u turn the screw
```

---
## \#12 Posted by: JdogAwesome Posted at: 2017-07-11T15:46:23.961Z Reads: 23

```
I had the exact same setup for charging, problem was my batteries were drawing to much current the the PSU didnt have any CC/CV functionality so it just turned off. Your PSU could have a soft over current protection were it shuts off and then back on very rapidly so it seems that barely any current is flowing. Why dont you try lowering the voltage on the PSU to just slightly above the battery voltage and then continue rising it until the PSU over current trips. If that is the case then your going to need to use some type of CC/CV converter to monitor the current to the battery.
```

---
## \#13 Posted by: pau Posted at: 2017-07-11T17:22:51.749Z Reads: 20

```
Actually The ampmeter jumps from 0 to 0.3 A Every half Second. And jumps back to 0 ampere.
So Maybee my drawing to much ampere. And The The psu will shut down.

So what Fan i do, to fix that Problem?
```

---
## \#14 Posted by: goldenHusky Posted at: 2017-07-11T17:45:52.948Z Reads: 20

```
Maybe I'm completely off now (never charged with a non CC/CV psu) but isn't there a current flowing equal to the voltage difference (25.2V-22.3V) divided through the wire resistance (some milliohms)? That would be more than the rated 11.2A of the psu. So in my opinion it shuts down and "reboots" periodicially.

You could add a high load resistor to limit the current to your desired 4.7A.
```

---
## \#15 Posted by: JdogAwesome Posted at: 2017-07-11T19:12:34.476Z Reads: 22

```
Yeah I think @goldenHusky is right it's drawing to much current. You could add a resistor but it's going to create a ton of heat and it would be a lot easier to use a cc/cv converter like I use in mine. To test it out like I said turn down the voltage and see if it starts drawing current without shutting down, lower the voltage, lower the current.
```

---
## \#16 Posted by: pau Posted at: 2017-07-12T00:00:27.645Z Reads: 18

```
What is a cc cv Converter? And why do have to use it?
```

---
## \#17 Posted by: JdogAwesome Posted at: 2017-07-12T00:08:18.439Z Reads: 16

```
CC/CV stands for Constant Current (CC) Constant Voltage (CV) and either one does as it says, it keeps the voltage constant by changing the output current or it keeps the current the same by altering the voltage. You need it so that the 25.2V from the PSU is turned down while the board is charging so it only draws, lets say 5A continuously. Lets say at 25.2V input with a dead battery at 22.2V it would try to draw a lot of current probably 20A+ so the converter drops that voltage down to maybe around 22.8V so it doesnt draw as much current, then as the battery is charged more it slowly increases that voltage to keep it charging at 5A. What ive been using is a so called "250W Boost converter" like [THIS](http://www.ebay.com/itm/DC-DC-Step-up-Converter-250W-10A-Constant-Current-Mobile-Power-Supply-LED-Driver-/262812499468?epid=526692992&hash=item3d30d87e0c:g:eHUAAOSwnHZYfr26) one. Its meant for driving LED's buts its what I had on hand and it works, although at 8A it gets pretty hot even with a heatsink and fan. Obviously because its a boost converter it can only step voltage up so I set my PSU to 19V and I have the boost set at 25.2V max and adjusted the current to 8A max.
```

---

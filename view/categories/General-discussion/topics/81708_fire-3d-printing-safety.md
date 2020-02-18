# Fire / 3d Printing / Safety

### Replies: 11 Views: 379

## \#1 Posted by: captclearleft Posted at: 2019-01-22T13:49:34.642Z Reads: 130

```
This just happened to a guy on a cosplay forum.  Not sure all the details as to cause of the fire.  
Stay safe when manufacturing your parts.
![50049717_10219850620715358_5281064827651883008_n|666x500](upload://7STp0Xt12uXnlJRBndY57m8ktA5.jpeg)
```

---
## \#2 Posted by: Itsmedant Posted at: 2019-01-22T13:52:17.376Z Reads: 121

```
It usually due to under speced mosfets on the power switch. Easily upgraded and fixed on mine. I think it was less than $20 for the new mosfet power switch.
```

---
## \#3 Posted by: linsus Posted at: 2019-01-22T13:53:30.696Z Reads: 115

```
Just needs a polish that machine, its fine
```

---
## \#4 Posted by: trelensis Posted at: 2019-01-22T13:57:08.493Z Reads: 121

```
Or also can be a failling thermistor. Controller keep pouring power while hotend/bed does not reach expected temperature. Updated firmware usually includes safety features to prevent this, but it can still happen if you keep stock firmware on cheap printers.
```

---
## \#5 Posted by: murloc992 Posted at: 2019-01-22T14:24:35.139Z Reads: 115

```
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/9176

All I can say, during this morning I was really happy it didn't burn up. :smiley:
```

---
## \#6 Posted by: akhlut Posted at: 2019-01-22T14:33:57.317Z Reads: 108

```
And this is why you don't leave these machines running unattended, especially around other fuel sources (wood, paper,etc).  Anything can and will happen.

Build a chamber for it, preferably one that has a higher melting point than aluminum.


It's full of stuff right now becaue of a move, but here's an example.
![20190122_093042|375x500](upload://ymkV9t2ueLK6jlfoWfq9SOEY4kd.jpeg) 

Extruded aluminum chassis with steel panels.
```

---
## \#7 Posted by: mishrasubhransu Posted at: 2019-01-22T14:53:16.544Z Reads: 87

```
Thermal runaway could be triggered by multiple reasons? Sensor failure, too cold. Do you know which one was it?
```

---
## \#8 Posted by: murloc992 Posted at: 2019-01-22T14:59:00.277Z Reads: 86

```
I think my bed shorted, look at the connectors..

I am amazed that this 15A fuse didn't blow. Just burned a bit.. Still a good fuse...
```

---
## \#9 Posted by: skelstar Posted at: 2019-01-22T17:44:19.847Z Reads: 65

```
I was standing next to my machine 3 days ago when I noticed smoke coming from the 12VDC connector (main input to the board). Will fit the FET that I bought months ago tonight I think.

I _had_ bought a new printer the day before. Perhaps my old printer had heard about it :slight_smile:
```

---
## \#10 Posted by: murloc992 Posted at: 2019-01-22T19:45:43.617Z Reads: 53

```
![42|690x388](upload://fMoDYvC9bKlQEj8PyvWtoZb5368.jpeg) 

After a "tiny bit" of replacements my prusa is chugging again. :smiley:
```

---
## \#11 Posted by: wafflejock Posted at: 2019-01-22T19:52:19.207Z Reads: 53

```
Agree with others here most likely causes are a short on the power connectors from either input power coming loose or shorting stray wires between the screw terminals (have had this happen before and start on fire on me), or could be problems with the MOSFET.  In general the MOSFETs are just going to shut off if they get too hot but they can get hot enough before they shut off to ignite anything with a low enough ignition temperature around them, on my GT2560 controller board the MOSFETs are very voltage sensitive and driving the main power supply voltage too low causes them to cook themselves (in my case this just results in the control board going crazy think becasue overheating mosfet was close enough to serial chip to mess up serial communication enough that it just bails out and terminates).  For my MOSFET issue just upping the voltage on the PS helped a lot and also added a little cooling fan to blast the heatsinks on the MOSFETs (cheaper boards will have MOSFETS just hanging off board with no cooling some other ones expect that the heat will dissipate through the control board PCB).

---

Think worthwhile PSA anyway since more people picking up 3d printers all the time and occasionally people who are having to go cheap on parts/tools here, but would be good to know if you gather any more info on the nature of the failure and how others could avoid (what printer was it?)
```

---

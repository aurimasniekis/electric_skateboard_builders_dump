# 12s4p bms recommendations

### Replies: 16 Views: 734

## \#1 Posted by: jneumann Posted at: 2019-01-16T11:22:41.728Z Reads: 162

```
Hi all I'm building my first battery with Samsung 30q's and I'm looking for recommendations for a bms. I've seen the besttech units but I'm starting to wonder if I need a discharge bms. What are my options for smaller charging and balancing BMS units? Also are there any options that can send data?  And has anyone managed to send cell voltage to there transmitter display? I've used the search function but haven't found much.
```

---
## \#2 Posted by: janpom Posted at: 2019-01-16T12:05:28.523Z Reads: 158

```
[quote="jneumann, post:1, topic:81041"]
Also are there any options that can send data? And has anyone managed to send cell voltage to there transmitter display
[/quote]

[Here's](https://www.electric-skateboard.builders/t/monitoring-individual-cell-voltages/80340) some info you may find relevant.
```

---
## \#3 Posted by: Andy87 Posted at: 2019-01-16T12:05:59.435Z Reads: 154

```
https://www.electric-skateboard.builders/search?q=smart%20bm
```

---
## \#4 Posted by: jneumann Posted at: 2019-01-16T22:45:43.059Z Reads: 131

```
So after researching there doesn't appear to be any standout options. Are discharge BMS's really necessary? With the Besttech BMS units do people get them configured to not charge the battery cells to 4.2V? Id imagine if after you charge your battery fully the brakes would try to recharge the battery and the BMS would cutout? I was hoping for a Besttech where i could monitor cell voltage via an android app but this does not appear to be available. I guess you just have to trust that the BMS is doing what it says it is.
```

---
## \#5 Posted by: Adstars Posted at: 2019-01-16T23:01:41.538Z Reads: 113

```
The Neptune 15 bms has a nice android app, allowing you to continually montitor your cells. It is what I am using in my current build. An expensive option though, but a premium product, and extremely small.
```

---
## \#6 Posted by: mynamesmatt Posted at: 2019-01-16T23:07:45.166Z Reads: 107

```
im pretty sure the DieBieMS works with Bluetooth through the vesc to provide voltage feedback to a phone app...? (someone correct me if I'm wrong here)
```

---
## \#7 Posted by: jneumann Posted at: 2019-01-17T00:11:46.802Z Reads: 102

```
looks like ill just go for a besttech 80a and run with discharge aswell. What settings should i get setup from bestttech? im using for samsung 30q. Will brakes work with this bms? are people getting them set from factory to only charge each cell to say 4.17v so brakes will always work?
```

---
## \#8 Posted by: jneumann Posted at: 2019-01-17T01:38:10.788Z Reads: 93

```
Also for the guys using charge only BMS units what are you doing to detect low voltage so you don't over discharge your batteries?
```

---
## \#9 Posted by: hyperIon1 Posted at: 2019-01-17T02:08:31.395Z Reads: 88

```
For charge- balance only (bypass) bms the over discharge is set in your esc, in the form of  volt limits Hard/soft
```

---
## \#10 Posted by: dareno Posted at: 2019-01-17T03:38:09.626Z Reads: 85

```
http://www.bestechpower.com/htmledit/UploadFiles/201832964539361.jpg

If you are going to run 12s4p then get something with a higher amp rating than 80amp discharge.  The site only has this 90a listed but if you contact them they will configure what you want but going direct you have to buy 2 moq
```

---
## \#11 Posted by: Marsen Posted at: 2019-01-17T10:12:38.742Z Reads: 76

```
I have been using these smart BMS's:
https://www.lithiumbatterypcb.com/product-instructionev-battery-pcb-boardev-battery-pcb-board/ev-battery-pcb-board/smart-bms-of-power-battery/
They are fully customizable so you can change all the parameters and they give lots of info to an android app as well as speed and distance (uses the gps on the phone).
I have been upgrading the Mosfet's to infineon ones as they have less internal resistance and can handle much higher current. The 60A model can be upgraded to handle 4.5Kw of power.
```

---
## \#12 Posted by: Marsen Posted at: 2019-01-17T10:20:33.530Z Reads: 72

```
It has a facility for an e-switch too.
```

---
## \#13 Posted by: jneumann Posted at: 2019-01-17T22:06:08.980Z Reads: 64

```
Hey Marsen,are you getting them upgraded from the factory or doing the upgrades at home? I'm in Perth as well. If you've got any upgraded BMS units would you be willing to sell me one?
```

---
## \#14 Posted by: Marsen Posted at: 2019-01-18T08:05:37.854Z Reads: 58

```
Hi jneumann, I do the modification myself so I know the MOSFET's are genuine, I get them from RS components. I am waiting for the e-switches but I have a load of 10S BMS's and 12S's are on the way. What was you after? They do an 11S which I haven't seen anyone use in an esk8 setup yet.
```

---
## \#15 Posted by: jneumann Posted at: 2019-01-18T22:52:06.000Z Reads: 50

```
Looking for a 12s one. Are the traces equipped to deal with the higher current on the 60a PCBs?
```

---
## \#16 Posted by: Marsen Posted at: 2019-01-19T06:05:34.984Z Reads: 46

```
It has copper busbar soldered to it for the higher current.
```

---

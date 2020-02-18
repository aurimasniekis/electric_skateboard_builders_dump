# Just broke new lipos on the first ride HELP

### Replies: 16 Views: 1343

## \#1 Posted by: Quinlanbrown Posted at: 2016-11-19T21:28:10.462Z Reads: 178

```
i just got new turnigy 4s 6000mah 45c witch is 270a output i programmed my vesc absolute max 200a and battery max 200a, one of the cells was completly dead and the other 2 battery's there where alot of inbalinced cells what do i do?
```

---
## \#2 Posted by: Monte Posted at: 2016-11-19T21:57:09.489Z Reads: 171

```
Send them back?
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-19T22:06:24.651Z Reads: 165

```
You should not have any setting on the vesc at 200a. That's very wrong.
```

---
## \#4 Posted by: Quinlanbrown Posted at: 2016-11-19T22:08:25.069Z Reads: 158

```
but if the baterys can put out 270a why would 200 be bad, what should i use insted
```

---
## \#5 Posted by: flatsp0t Posted at: 2016-11-19T22:09:35.084Z Reads: 157

```
well, the vesc can handle 50
```

---
## \#6 Posted by: Quinlanbrown Posted at: 2016-11-19T22:10:59.403Z Reads: 152

```
it peakes to 240a
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-19T22:27:54.455Z Reads: 153

```
for a couple seconds yes, that's the theoretical max. If you have 200a continuous on your system, you'll easily burn the trace and wires out. Why would you even want 200a, you'll just end up burning the excess energy as heat and have crap battery life. Battery max should be 40-60a in most situations.
```

---
## \#8 Posted by: IDVert3X Posted at: 2016-11-19T22:43:51.654Z Reads: 148

```
Sounds like a faulty battery, return it within 30 days to HK. The problem isn't the 200A setting, you can not pull that much even if you wanted... But ideally, you should limit it to 60A on the battery just to be safe and keep it nice and cool.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-11-19T23:09:34.586Z Reads: 138

```
200a Vesc settings is not too high for the batteries but it is too high for the Vesc and motor.
It is a great idea to run batteries capable of much higher current than you need to avoid voltage sag. 
I'm currently running Turnigy 5.0/ 60c/120c batteries capable of 300a cont and 600a peak. 
It sounds like you may have just over discharged yours. It's a must to monitor the voltage of Lipos while riding and not take them below 3.2 volts per cell under load. 
It's also important to balance charge them. 
You mentioned that they where out of balance. How out of balance where they?
```

---
## \#10 Posted by: Namasaki Posted at: 2016-11-20T04:16:59.007Z Reads: 121

```
I got a bad battery pack right out of the box from HK once. I contacted them and they told me "Do Not Send it Back"
What I had to do was take a picture of the battery connected to a voltage meter showing the voltage of all the cells and the cell with voltage below minimum and the serial number of the pack. Then they told me to dispose of the battery myself and they shipped me a new battery.
```

---
## \#11 Posted by: Mobutusan Posted at: 2016-11-20T16:12:16.351Z Reads: 97

```
What was your battery voltage cutoff set at? I assume your running these in series at 12s?
```

---
## \#12 Posted by: saul Posted at: 2016-11-20T18:02:18.820Z Reads: 89

```
those peak ratings are mostly for the mosfets...pushing components that hard is not a good idea...the current control on vesc still needs time to react. you'll have crazy high current spikes even if only for a few ms...

this setting is there for added protection...you've removed that layer and ruined your lipos....

adjust motor/battery max. not absolute.
```

---
## \#13 Posted by: Quinlanbrown Posted at: 2016-11-21T00:42:55.721Z Reads: 76

```
The battery with the dead cell is at 3.39, 0.00, 3.29, 3.41, I think I broke the cell but I'm still gonna try to return it anyways, the other batterys at 3.21, 3.43, 3.51, 3.39 and the last ones at 3.13, 3.23, 3.24, 3.07 the 2 batterys that are a little unbalanced feel really solid the same as when I got them but the one with the dead sell is a tad bit puffed but barley, after I rod they where a little hot, my venom carger won't charge them for some reason I tryed before I used them to bc batterys come a little under charged, I'm planing on charging with my bms once I wire it will that balance out the cells or do I need to do that before using the bms?   Thanks for the help
```

---
## \#14 Posted by: SORRENTINO Posted at: 2016-11-21T01:22:04.313Z Reads: 67

```
New lipos typically will be out of balance for the first couple of charges / discharges. Either the other one has a completely dead cell or maybe the wire pulled off the cell tab and it wont read that cell imo. Also resting voltage of lipos should be around 3.6. The fact that your resting at 3.2 to 3.1 isnt good since most likely with high loads the battery will sag into the 2 volt range which is not good at all for your cells and will increase IR cells. Over discharging is really bad for lipo cells.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-11-21T02:15:13.956Z Reads: 58

```
I don't know what BMS your using however, I tried to replace one pack in my series of 5 2s packs and it's cells where only around .4v higher than the cells of the existing packs but my BMS would not balance them out and fully charge the pack so I wound up using my hobby balance charger to fully charge each pack individually and then hooked them back up to the bms.
So I recommend balance charging your pack with a balance charger before installing them with a BMS.

As for your bad pack, your best bet is to open a live chat on Hobby Kings website and tell them your pack has one dead cell.
They should give you an email address to send them pics of the pack showing it's serial number and of the pack connected to a Lipo volt meter showing the voltages of cells .
Then if they agree to replace it, they will open an order for a new pack to be shipped to you free of charge and they will tell you to dispose of the bad pack.
They do not want any defective Lipo packs returned to them for obvious reasons.
BTW, anytime you buy a Lipo battery from anyone, check it's voltages with a Lipo meter before doing anything with it.
I suspect that your pack with the dead cell was bad right out of the box.
```

---
## \#16 Posted by: powerhungry Posted at: 2016-11-26T17:33:29.881Z Reads: 38

```
I would first pump my brakes lol, then relize I do not need to pull 200 amps, as stated by others. pushing everything to the max will destroy everything quickly, better to have everything run cool ,might have to over build to get performance and longevity but at least u are not pushing everything to its limits,if that makes sence to you. what I mean is instead of pushing a battery to its max where it is overheating, get a couple batteries to do the same job but they remain cool as load is shared. now if you do this with everything then u have no problems and just the joy of e boarding and not rebuilding everyday .
```

---

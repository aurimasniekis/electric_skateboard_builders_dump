# Battery and bms setup

### Replies: 17 Views: 331

## \#1 Posted by: KranzeKake Posted at: 2018-10-22T22:24:31.817Z Reads: 91

```
Hi. Im building my first electric longboard, and have some questions regarding the setup. I will be using this battery: https://www.eboardsperu.com/product/10s4p-battery-for-loaded-vanguard/ Here are my questions:

1. What BMS would you guys recommend for my battery?

2. Can I disable the BMS for discharge to remove a possible bottleneck ? (a wiring schematic would really help) 

   3 Is there any way to connect the BMS to an Arduino to get charge data?

Thanks for the help guys!
```

---
## \#2 Posted by: dareno Posted at: 2018-10-22T22:30:52.856Z Reads: 80

```
Just ask Alan ( @Eboosted ) to supply the battery complete with bms charge port and indicator etc.  wired for charge only.  Make life so much easier for you.
```

---
## \#3 Posted by: dg798 Posted at: 2018-10-22T22:42:45.777Z Reads: 77

```
If not you can buy one from @JLabs. He has some charge only from bestech
```

---
## \#4 Posted by: Travo Posted at: 2018-10-22T22:43:00.134Z Reads: 75

```
You can purchase a Bluetooth BMS it has some neat features, trying to set mine up now
```

---
## \#5 Posted by: KranzeKake Posted at: 2018-10-22T22:44:36.590Z Reads: 74

```
Yeah I did, he said he did not have time atm
```

---
## \#6 Posted by: Eboosted Posted at: 2018-10-22T22:46:56.577Z Reads: 69

```
I can make the battery with balance leads and BMS wired, you will only need to wire the charging port yourself.

:slight_smile:
```

---
## \#7 Posted by: KranzeKake Posted at: 2018-10-22T22:48:17.655Z Reads: 65

```
The only problem is that I already have an Arduino running on Bluetooth. I am also planning to buy the FOCBOX Unity which has Bluetooth too, don't want more than 2 radios....
```

---
## \#8 Posted by: KranzeKake Posted at: 2018-10-22T22:50:39.759Z Reads: 70

```
That's awesome! Then I just need a schematic for how I wire up the charge port. Do you sell chargers aswell?
```

---
## \#9 Posted by: Travo Posted at: 2018-10-22T22:51:41.073Z Reads: 69

```
So you want a physical screen reading off the inputs? Also the focbox would replace the Arduino Bluetooth wouldn't it.
```

---
## \#10 Posted by: KranzeKake Posted at: 2018-10-22T22:56:05.329Z Reads: 66

```
I want to be able to check the voltage of my cells, and also get a signal when charging is complete. I heard that Enertion was planning on an app for the Unity, maybe that could give me this information, if not I want it sent to my arduino which I use for my remote.
```

---
## \#11 Posted by: Eboosted Posted at: 2018-10-22T22:57:24.926Z Reads: 59

```
Yes. I supply everything you will need, charging port, wires for charging ports, even the heat shirk, antispark switch, bms, on/off switch, XT60s and if course battery and enclosure with bolt kit.
```

---
## \#12 Posted by: KranzeKake Posted at: 2018-10-22T22:58:35.586Z Reads: 54

```
Even the charger itself? If so, what amps is it rated at?
```

---
## \#13 Posted by: Eboosted Posted at: 2018-10-22T23:00:31.762Z Reads: 53

```
Charger too, I don't have it on my website though, I could offer a 2A, 3A or 4A, I suggest the 2A as they batteries will have a longer lifespan and it's better if they ever go out of balance
```

---
## \#14 Posted by: KranzeKake Posted at: 2018-10-22T23:01:13.608Z Reads: 54

```
Thank you so much for your help! Got my enclosures today, love them!
```

---
## \#15 Posted by: Eboosted Posted at: 2018-10-22T23:51:50.547Z Reads: 53

```
[quote="KranzeKake, post:1, topic:72010"]
* What BMS would you guys recommend for my battery?
* Can I disable the BMS for discharge to remove a possible bottleneck ? (a wiring schematic would really help)
[/quote]

1. Bestech has a good reputation around here

2. Here you go:
[img]https://i.imgur.com/oeNLTjn.jpg[/img]
```

---
## \#16 Posted by: KranzeKake Posted at: 2018-10-23T05:42:20.784Z Reads: 41

```
Thank you! So now the batteries will charge trough the BMS, but discharge without it?
```

---
## \#17 Posted by: Eboosted Posted at: 2018-10-23T05:55:55.781Z Reads: 40

```
Correct, just follow the positive and negative line and you will realize it.
```

---

# Fault_Code_Under_Voltage

### Replies: 21 Views: 420

## \#1 Posted by: Wallgreeens Posted at: 2018-07-22T22:44:49.870Z Reads: 110

```
Everything runs fine until get to about 50% battery life the vesc shuts down and give me this fault code. Before 50% battery life the board is running fine.  I don't know what is causing this to happen around the same battery percentage every time.    I'll include the voltage settings, and the error codes.  One image is the board resting at about 40% battery.  If I tried riding the board the vesc would shut down and give me the fault code under voltage.  The other image is during a shut down and the last image is my settings on the master vesc.  Any help would be greatly appreciated.![kaly%20fault%20code|243x500](upload://43xFoFxKhSUpgtGUgUsPQ7M1BFO.png)
![kaly%20voltage%20settings|690x307](upload://lhYMKHWFHlKDYeroXcQbxypy26s.PNG)
![Kaly%20Vesc%20During%20Malfunction|243x500](upload://8W4XUtxqUgUvvEpkNLCmnUTYK2Z.png)!
![vesc%20monitor%20resting|243x500](upload://q2QcPrnK2sXx0PEZUQjUlC5SA89.png)
```

---
## \#2 Posted by: Wallgreeens Posted at: 2018-07-23T00:28:48.553Z Reads: 88

```
Now, I'm getting this fault code that, but my max current is set at 130.   ![abs%20over%20current|243x500](upload://m9WpwGsbEQMj4jHum65HIkjaqU0.png)
```

---
## \#3 Posted by: Martinsp Posted at: 2018-07-23T00:28:57.140Z Reads: 83

```
Id suggest first checking all of your solder joints and connectors. If that all looks good try to measure the voltage of the battery right at the VESC inpuit when the fault is triggered and your VESC keeps shutting off. As far as settings go it seems all ok in terms of voltage. Maybe your BMS (if you use one) is turning off.
```

---
## \#4 Posted by: Wallgreeens Posted at: 2018-07-23T03:21:29.827Z Reads: 76

```
All the connections seem fine, I"m wondering why the errors switched from low volatage to over voltage.
```

---
## \#5 Posted by: Eboosted Posted at: 2018-07-23T03:25:23.157Z Reads: 73

```
You have an issue with your battery pack or with the VESC caps, open your vesc and check for that.
```

---
## \#6 Posted by: dareno Posted at: 2018-07-23T03:29:00.177Z Reads: 73

```
Check all battery banks with a meter but that looks like a bms fault.
```

---
## \#7 Posted by: Wallgreeens Posted at: 2018-07-23T06:09:41.090Z Reads: 69

```
Would a bad vesc cap look fried? Or what would I be looking for?
```

---
## \#8 Posted by: Wallgreeens Posted at: 2018-07-23T06:10:44.493Z Reads: 67

```
Thanks, I'll try that.
```

---
## \#9 Posted by: Martinsp Posted at: 2018-07-23T08:00:11.671Z Reads: 58

```
A broken cap (the cylindrical one) would have a cracked top. If it is broken the pressure will rise inside the aluminium can and the pressure relief will blow on the top side. 

Does it have any repetitive behavior or is it random?
```

---
## \#10 Posted by: Wallgreeens Posted at: 2018-07-23T13:10:57.708Z Reads: 54

```
Very repitiive, every time I hit around 50% battery life this happens, be for that it runs like a champ.
```

---
## \#11 Posted by: Martinsp Posted at: 2018-07-23T13:13:42.482Z Reads: 51

```
Okay that may be an issue with the voltage sensing either firmware issue since it is reading below 8V which triggers the fault, or a problem with the voltage divider. 

When you plug your battery in charged above the 50% you are mentioning, what voltage does the VESC show in real time data? Is the voltage correct? If the reading is the same or reasonably close as your multimeter reading I would try to flash the firmware again. If you want to you can save the XML with your motor configuration, you will have to set up your app config though
```

---
## \#12 Posted by: Wallgreeens Posted at: 2018-07-23T13:30:27.160Z Reads: 48

```
The akmaniacs esc tool seems pretty accurate as for voltage when fully charged. I can crack it open and check it with the multimeter.  I would have to charge it first.  I was trying to replicate the issues, so I kept the battery around 50%.  Where do I plug the multimeter into to determine  the voltage?
```

---
## \#13 Posted by: Martinsp Posted at: 2018-07-23T13:33:53.206Z Reads: 45

```
Well you dont need to charge it. As long as the VESC turns on and gives you a reading it is OK. After that measure the voltage of your battery directly on the connector. It should be all the same within some margin of error.
```

---
## \#14 Posted by: Martinsp Posted at: 2018-07-23T13:37:13.234Z Reads: 44

```
So if all of that is correct I would suggest flashing the firmware, just because it is simple and lowers the number of potential reasons for your VESC to not work.
```

---
## \#15 Posted by: hmgcoa Posted at: 2019-08-11T00:58:00.540Z Reads: 25

```
I have the same issue looked up on the vesc tool. While trying to find the fault that caused this, found that each time I test there was different ERRORS under fault. I had ABS_Over_Current error, undervoltage error and DRV. Essentially now on 44.3 v left in a 50.2 volt 12s set up I can turn on the vesc but when I move like 10m the vesc stops and turns off itself after a few flashes of red light. If I allow it to run without me standing on it it can run further before it stops.
```

---
## \#16 Posted by: Santino Posted at: 2019-08-11T03:06:18.008Z Reads: 22

```
Sounds like something is wrong with your ESC...Maybe something it is fried....
```

---
## \#17 Posted by: Wallgreeens Posted at: 2019-08-11T06:07:37.899Z Reads: 22

```
Mine turned out to be unbalanced cells.  Yours sounds a little different as mine only happened when the board was below 50% battery life.
```

---
## \#18 Posted by: Jansen Posted at: 2019-08-11T20:28:15.203Z Reads: 20

```
Im having this exact issue right now? Is it fixable... I have a 12s3p 30q pack I didn't use for like 6 months. Set up an extra build and it seemed to be working fine but then once I hit 50% or under it will turn off with the under-voltage error. If I turn the board on and off it works again until it turns off and is under voltage. Battery sag right? I am pretty sure my cells are unbalanced to cause some stupid seller on Alibaba sold me 13s charger instead of 12s and i didn't notice till recently so I am pretty sure I was overcharging it at times.... lmk what you did on yours if anything. Thanks, @Wallgreeens
```

---
## \#19 Posted by: dareno Posted at: 2019-08-12T04:58:37.130Z Reads: 16

```
Sounds like the same thing to me.  Cells never go to 0 volts but they do go to 0 %.  On 12s the highest voltage should be 50.4v and the cut off is whatever you set it for.  Vesc tool sets it at 33 -36 I think from memory in the wizard.  Might be out by a volt or 2 but the point still stands the voltage range is not the same as percentage.  As advised a year ago you need to check each p pack for voltage across the bms wiring.  Starting from the first it should climb in increments of around 3.6v judging by the total voltage of the pack.  I'm guessing one pack is way out of line with the others.  @Jansen  You too brother.  Get the multimeter out.
```

---
## \#20 Posted by: Jansen Posted at: 2019-08-13T20:19:34.646Z Reads: 10

```
@dareno thats what Im saying, my multi meter was reading 0.0 v from the xt60 connector so im going to test some other places and the balance leads like you suggested later today. Thanks brotha.
```

---
## \#21 Posted by: dareno Posted at: 2019-08-13T21:59:06.354Z Reads: 9

```
0v from the xt is a main connection issue.  Be very careful because you may have a broken main wire.  Literally just had the same issue on an enertion pack that I was trying to use.  Solder tab (paper thin nickel)  had broken off in the shrink wrap and caused some nasty stuff.
```

---

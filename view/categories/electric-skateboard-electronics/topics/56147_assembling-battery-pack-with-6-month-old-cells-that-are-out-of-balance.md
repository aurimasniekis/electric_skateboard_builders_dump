# Assembling battery pack with 6 month old cells that are out of balance

### Replies: 14 Views: 432

## \#1 Posted by: craj1031tx Posted at: 2018-05-21T03:13:18.731Z Reads: 126

```
Hey all,

I bought some 25Rs that were brand new in November and am only just now getting around to assembling them into a 10S4P flat pack. I bundled together the 10x 4P packs, and noticed that the voltage range is fairly significant: most are at 3.5-3.6v, but there are 2 packs that are at 4.0v each. Is this going to be a problem upon assembly? I have a Bestech BMS that I think is rated at ~150mA balance capability; I know that the 3.5-3.6 variance shouldn't be an issue but I'm worried about the 4.0v packs being wildly out of sync with the others. 

Do I need to discharge them? Is there a recommended range that all packs should be in before assembly? If I am to discharge them, what's the recommended method for doing so? 

Thanks!


Edit: I know it sounds odd that brand new 25R cells would have some wildly different voltages... I think I may have played around with a few individual cells over the last few months so that is where that abnormality stems from. They were all purchased from IMR so they should all be good/authentic.
```

---
## \#2 Posted by: EverBlade21 Posted at: 2018-05-21T03:15:20.289Z Reads: 122

```
So before making your battery pack it would be supppppppeeeerrr beneficial to charge up all of your batteries so that they are all at their maximum and THEN start spot welding and attaching all the cells together. I have no idea how the BMS will interact with what you already have, but thats what I do at step 0. Good Luck!
```

---
## \#3 Posted by: craj1031tx Posted at: 2018-05-21T03:17:20.442Z Reads: 117

```
Well it might already be too late for that as they are already welded together into groups of 4. I do have access to a high-quality benchtop power supply on which I can control voltage and max current so I could try and charge each individual 4 cell pack though. I thought standard procedure was to weld them up when they are in a storage-charge state though - am I wrong? As to prevent any serious discharge issues if you accidentally short them.
```

---
## \#4 Posted by: EverBlade21 Posted at: 2018-05-21T03:20:55.527Z Reads: 111

```
The chances of shorting individual cells is not very likely so I dont worry about that at all,but if you can use your benchtop power supply set it  to 1A and your highest voltage (4V) and charge up the batteries. Just check with a multimeter to see if its goign well and make sure to check the cell temperatures.
```

---
## \#5 Posted by: DougM Posted at: 2018-05-21T03:24:10.727Z Reads: 110

```
If you've already welded the individual cells then I would just go ahead and build it.  That's exactly what the BMS is designed for.  It'll take some time to balance everything out.
```

---
## \#6 Posted by: baxter Posted at: 2018-05-21T03:34:09.539Z Reads: 104

```
I would recommend you do a google search for “bottom balancing” parallel groups of cells.
```

---
## \#7 Posted by: darkkevind Posted at: 2018-05-21T06:33:55.241Z Reads: 98

```
Once you've built it, buy a TP4056 (or several) and use it to charge each parallel pack to full charge through the balance connector... This will take time but also bring all cells in to line. Then use and charge through the BMS as normal.

![20180416_103950|690x335](upload://3V94nRda7SSyojvJUNFTGRPXQnR.jpg)
```

---
## \#8 Posted by: philvanzu Posted at: 2018-05-21T11:58:02.661Z Reads: 81

```
wouldnt it be ok to just sandwich all your packs of four between two copper plates so they are all put in parrallel and let them auto balance that way?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-05-21T12:01:48.000Z Reads: 79

```
This would most likely make a loud bang which couldn’t be good.
```

---
## \#10 Posted by: philvanzu Posted at: 2018-05-21T12:05:06.638Z Reads: 79

```
why? there woulnt be a circuit? just a 1S pack
```

---
## \#11 Posted by: pat.speed Posted at: 2018-05-21T12:16:07.446Z Reads: 72

```
Thank about how they balance, one pack must change the lower packs. When connected straight together there is nothing to limit current flow, so the packs will dump a lot of power all at once trying to bring the others up to the same voltage. Thus a bang and spark, well so I’ve heard.

When the voltages are close it’s different but 4v and 3.5v is a bit of a gap
```

---
## \#12 Posted by: philvanzu Posted at: 2018-05-21T12:17:53.914Z Reads: 71

```
Oh ok that makes sense. I didnt know it would work that way.
```

---
## \#13 Posted by: goldrabe Posted at: 2018-05-22T23:55:27.346Z Reads: 49

```
Hi Kevin,

i have a 10S5P pack which is out of balance. All cells have readings between 3.92 - 3.95V except one parallel group of 5 cells which are between 40 - 41.5V. When i charge the pack through the BMS the charger turns green but the voltmeter only shows 39.5V in total when measuring at the XT60 connector.
Bringing the pack in to balance with a TP4056 seems to be the best solution. Can you elaborate a bit more where exactly to plug the TP4056 and in which order to proceed?
Can i just use a smartphone charging brick?
Your help is really appreciated!
Thanks.
```

---
## \#15 Posted by: darkkevind Posted at: 2018-05-23T15:40:11.047Z Reads: 35

```
Charge it with the TP4056 through the balance connector, as per my photo above...
```

---

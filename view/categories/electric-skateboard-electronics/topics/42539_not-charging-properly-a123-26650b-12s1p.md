# \[not charging properly\] A123 26650b 12S1P

### Replies: 27 Views: 1145

## \#1 Posted by: GreasyGearsWRX Posted at: 2018-01-02T02:34:19.004Z Reads: 133

```
Hey guys, I have been having an impossible time figuring out why my 12S1P A123 26650b battery pack wont balance properly. 

Now to begin when I say 12S1P I mean I have made two individual 6S1P packs that I plan to run in series so that I can use a common hobby charger that can only balance 6 cells. I wanted to just use a balance charger for now so I can iron out my rig before I build my enclosure and call it "finished". 

I started by cycling all my batteries individually and then charged them all up to a voltage of 3.3 before building the pack.

I then welded the cells together via a sunkko 788h and .15mm nickel strips rated for 10-15 amps. to handle the high amperage ability of these batteries I welded 3 of those nickel strips on top of each-other so that I wouldn't have a failure. I then soldered a 7 pin balance connector for 6S to each of the packs on the nickel strips in between each battery. The pattern that they are soldered are as follows: (ground wire:negative lead of first battery) (2nd wire:positive lead of cell one) (3rd wire:positive lead of cell two) (pattern as follows) then (7th wire:positive lead of cell 6).

I have checked the voltages of the cells directly on the leads to confirm voltage and also checked the pins of the balance connector to make sure their voltages accurately correlate with the voltages of the charger. I have used 2 different hobby battery chargers to make sure its not a symptom of a specific charger. 

So, what I am experiencing is when I attempt to balance charge (OR EVEN DUMB CHARGE) all the cells voltages rise proportionally and correctly as expected for the first 30 seconds to 1 minute of charging but then over the course of a few minutes all the cells but one slowly stop charging COMPLETELY and come back to their resting voltages. The one cell in question continues to charge until it reaches 3.6v. Once the one cell reaches this charged voltage the charger stops. What is especially odd is that the whole pack only consumes about 100 mah every time I do this. For one of the two packs, cell 2 is the battery that rises to 3.6 and in the other pack cell 4. 

For all of my testing I have tested these voltages with the multimeter on the leads of each cell so none of these reading are false readings. 

Please someone help me solve this problem it is very frustrating that I cant enjoy my first board!! Thanks!!

Pack 1:
<img src="/uploads/db1493/original/3X/3/c/3cfafb78c03d2b814d18ef806c1b73c47f0891cc.JPG" width="666" height="500"> 
<img src="/uploads/db1493/original/3X/8/9/89e8b74f98818cb4170cbde8b0eaabbfe257d8c7.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/e/a/ea04c0e347acc92dc10f46d26e7326936c6f42ea.JPG" width="666" height="500">

Pack 2:
<img src="/uploads/db1493/original/3X/c/d/cdf7afd512730560db5546b5631f33ff1319ee9c.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/3/636ff2386239db0c218d8905633a64423401a7dc.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/e/cef3720c29d054a730f8a180b01c400b455b634b.JPG" width="666" height="500">
```

---
## \#2 Posted by: scepterr Posted at: 2018-01-02T02:40:54.638Z Reads: 115

```
Possibly bad welds between the layers of nickel 
Have you tried just charging the 6s as a whole?
```

---
## \#3 Posted by: GreasyGearsWRX Posted at: 2018-01-02T02:46:46.771Z Reads: 114

```
yeah man I did try to just charge the whole pack without using the balance leads!
```

---
## \#4 Posted by: scepterr Posted at: 2018-01-02T02:47:47.741Z Reads: 114

```
Then maybe the initial welds aren't good
```

---
## \#5 Posted by: GreasyGearsWRX Posted at: 2018-01-02T02:49:48.463Z Reads: 112

```
yeah I am considering this could be the problem but the overall pack voltage has been fine and it initially charges all the batteries evenly.. its so weird!
```

---
## \#6 Posted by: scepterr Posted at: 2018-01-02T02:51:32.290Z Reads: 102

```
Well that's a sign of bad series connection
You can get a voltage reading but as soon as you put current through it the resistance on the bad links shoots up and you get nothing

If it doesn't charge through the nickel layers or through the first layer but the cells charged fine on their own, it's the series connections
```

---
## \#7 Posted by: GreasyGearsWRX Posted at: 2018-01-02T02:54:02.648Z Reads: 97

```
interesting! okay well I am going to go rebuild one of the packs and hope it fixes it! I really appreciate your help man! If you think of anything else please let me know!
```

---
## \#8 Posted by: scepterr Posted at: 2018-01-02T02:55:02.185Z Reads: 96

```
You'll know if they were bad right now when you pull off the nickel

Post a pic of the cells after you remove the nickel and as you do each layer
```

---
## \#9 Posted by: GreasyGearsWRX Posted at: 2018-01-02T03:24:44.042Z Reads: 92

```
sorry i forgot to man but hey we are on to something! So we think you are right that because of a bad connection it is indicating our voltages as wrong at the charger but not in the actual battery. we just used the multimeter to test the leads of the battery and the bullet connectors into the charger as we were charging it and on the leads of the batteries we got 3.3 and on the bullet connectors at the charger we got 3.5 and at the charger it indicated 3.55....? weird or normal?
```

---
## \#10 Posted by: scepterr Posted at: 2018-01-02T03:29:39.134Z Reads: 88

```
Maybe main lead from charger to battery is bad?
```

---
## \#11 Posted by: GreasyGearsWRX Posted at: 2018-01-02T03:57:32.684Z Reads: 82

```
hmmm ive done some testing and the resistances of my batteries seem a little high. when i first got them they were between 10 and 35 and i just tested one and got around 50.... thoughts? i tried two chargers and different balance leads and different batteries as cross reference.
```

---
## \#12 Posted by: scepterr Posted at: 2018-01-02T04:04:34.249Z Reads: 75

```
Did you remove all the nickel and replace it?
```

---
## \#13 Posted by: GreasyGearsWRX Posted at: 2018-01-02T04:19:50.554Z Reads: 73

```
sort of, i left the positive and negative strips on there and just tested individual cells
```

---
## \#14 Posted by: scepterr Posted at: 2018-01-02T04:22:07.105Z Reads: 73

```
I'm not sure what that means

The nickel to cell connection is bad it needs to be removed and inspected so you can see where it's bad
```

---
## \#15 Posted by: GreasyGearsWRX Posted at: 2018-01-02T04:26:11.207Z Reads: 77

```
sorry i took the nickel strips off and just individually tested each battery and its resistance and it seemed high. but even by testing the individual cells we had weird voltage spikes when trying to charge even at low amperages like 1.5 amps.
```

---
## \#16 Posted by: scepterr Posted at: 2018-01-02T04:33:31.563Z Reads: 81

```
Ahh, well that is wierd, how are you charging them individually?
```

---
## \#17 Posted by: GreasyGearsWRX Posted at: 2018-01-02T04:38:08.224Z Reads: 77

```
just with a cell holder that i 3d printed and on a 1S setting with an imaxb6!
```

---
## \#18 Posted by: scepterr Posted at: 2018-01-02T04:38:50.730Z Reads: 76

```
There might be a bad connection somewhere between the imax and the cell
```

---
## \#19 Posted by: GreasyGearsWRX Posted at: 2018-01-02T04:47:30.329Z Reads: 78

```
i wanted to think that too but i just tried it on another charger with similar results. So the listed resistance of these batteries is around 10 ohms. Sooo do you think my batteries are dead?
```

---
## \#20 Posted by: scepterr Posted at: 2018-01-02T04:49:18.995Z Reads: 74

```
Anything is possible 🤔
```

---
## \#21 Posted by: GreasyGearsWRX Posted at: 2018-01-02T04:57:45.939Z Reads: 68

```
awe damnnnn just twist the knife lol I'll post back when I know more tomorrow. Thanks a lot for your help though man!
```

---
## \#22 Posted by: deucesdown Posted at: 2018-01-03T00:09:36.137Z Reads: 60

```
you have a second 6s, how's that one looking?
```

---
## \#23 Posted by: longhairedboy Posted at: 2018-01-03T01:34:11.227Z Reads: 57

```
hard to tell from the pics but it looks like some of the balance leads may be out of order.
```

---
## \#24 Posted by: GreasyGearsWRX Posted at: 2018-01-03T08:10:26.524Z Reads: 41

```
Hey thanks guys sorry been away from home today! Yes I have two 6s packs wired exactly the same. I wired them the same pattern as I have seen lipos wired for years. Maybe it’s backwards? I don’t believe so though. I am going to finish rebuilding one of the packs in the morning and I may reverse the order of the pins but I believe it’s correct!
```

---
## \#25 Posted by: GreasyGearsWRX Posted at: 2018-01-07T10:11:39.450Z Reads: 32

```
Wanted to make it aware that this issue was resolved! Running as well as can be now!
```

---
## \#26 Posted by: pat.speed Posted at: 2018-01-07T12:07:25.795Z Reads: 26

```
That's great, what was the issue in the end?
```

---
## \#27 Posted by: GreasyGearsWRX Posted at: 2018-01-07T19:21:37.923Z Reads: 22

```
Poor nickel strip connection and poor solders to the nickel strips. I don’t have a high powered soldering iron so I soldered all my wires to the nickel strips before I welded them because when the heat could dissipate into the cells I couldn’t got nice connections!
```

---

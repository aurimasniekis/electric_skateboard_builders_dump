# Anatomy of a speed controler

### Replies: 13 Views: 576

## \#1 Posted by: TheGreekGuy Posted at: 2018-09-17T20:45:15.112Z Reads: 152

```
Hi all, 
I was wondering if there is anyone here with knowledge on electronics.
What I was wondering is if I can change some capacitors / resistors / mosfets etc on my dual hub motor board.
for example:
![s-l1600|500x500](upload://yspIu8m9Oe4LjcSmfZEQPuluUwa.jpg)
what if I change the 2 capacitors (470uF / 63V) on my board with 2 x 1000uF/63V or 2x 470uF/100V
what would that change if anything?

Thanks
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-09-17T20:50:09.003Z Reads: 141

```
@Kug3lis have at it lol
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-09-17T20:52:17.374Z Reads: 139

```
I am no expert at this at all, but why would you like to change the caps in the first place?
```

---
## \#4 Posted by: robthebuilder Posted at: 2018-09-17T20:52:31.622Z Reads: 138

```
I guess the other components on the board would need to be changed for it to handle that kind of power
```

---
## \#5 Posted by: b264 Posted at: 2018-09-17T20:55:39.832Z Reads: 133

```
Upping the caps *could* make the ESC perform *slightly* better but might fry an antispark switch that may be embedded in the ESC itself, or separate.  Unless it has a loopkey, then will be harder on the loopkey.
```

---
## \#6 Posted by: TheGreekGuy Posted at: 2018-09-17T21:03:55.224Z Reads: 128

```
Well my idea is that if the controler with 470uF/63V tops at 63V (burned above that value) with 470uF/100V the controler will be more protected of voltage surges. Is my understanding right?
```

---
## \#7 Posted by: Pedrodemio Posted at: 2018-09-17T21:27:06.825Z Reads: 119

```
Not completely, the caps can survive the large spike, but they wouldn't fail right away with a higher voltage

The other components remain exposed to these higher surge

The only easy modification you could easily do is find the current shunts, probably on the underside of the board and change them to increase the current output. I do not recommend that since the MOSFET's, PCB traces and other componentes were not designed to handle that increased current
```

---
## \#8 Posted by: b264 Posted at: 2018-09-17T21:31:24.145Z Reads: 111

```
[quote="TheGreekGuy, post:6, topic:68339, full:true"]
Well my idea is that if the controler with 470uF/63V tops at 63V (burned above that value) with 470uF/100V the controler will be more protected of voltage surges. Is my understanding right?
[/quote]

Yes

But that won't save an IC or a FET
```

---
## \#9 Posted by: dareno Posted at: 2018-09-17T21:43:15.109Z Reads: 102

```
That esc already works with long battery leads in nearly every application so it shouldn't be necessary.
```

---
## \#10 Posted by: Okami Posted at: 2018-09-19T05:24:35.537Z Reads: 66

```
If u change caps as far as i know they should be low ESR..
```

---
## \#11 Posted by: Nordle Posted at: 2018-09-19T05:53:51.065Z Reads: 62

```
you won’t notice any difference
```

---
## \#12 Posted by: Kug3lis Posted at: 2018-09-19T07:17:32.420Z Reads: 53

```
Uhh sorry I am bit late here. But just changing capacitors, resistors and mosfets will not change how ESC handle higher voltages. Some other devices like regulators and other IC not always work with higher voltages.
```

---
## \#13 Posted by: yuweng Posted at: 2018-09-19T08:53:35.253Z Reads: 42

```
These generic Chinese ESC uses the cheapest but reliable [RU6888R](http://www.ruichips.com/uploads/file/20180818/20180818060920251.pdf). During my ebikes days, we use to mods these by changing the mosfets, higher value resistor for the regulator & modify the shunt. These Chinese ESC doesn't have the shunts, may be they are software based, i donno.

![single%20hub%20ESC|666x500](upload://xOwskYqeyaSSnagVDmsrPJLhfHJ.jpeg) 
RED circle is the 7815 regulator. If you do plan to over volt it then just add a 470 ohm resistor before the input to lower down the input voltage. A watt will do, i think, if its really hot then increase to 2 or 3 watt resistor.

![mosfet|666x500](upload://7InhbtD3AD1yhJ4ktWPLYSV521T.jpeg) 
For ebikes, we use to replace these with [FDP2532](http://www.onsemi.com/pub/Collateral/FDB2532_F085-D.PDF) as it was the best & cheap at that time. You'll need the 100 volt cap for these upgrades. It is a good idea to upgrade the heatsink as well. You can salvage it from a dead PC PSU, most of them are about the same size. After that, you should be able to use 12S, 13S, 16S or may be even 20S ! :sunglasses:

But who would dare to ride on a 20S, safety first in case you really do plan to do these upgrades !
```

---

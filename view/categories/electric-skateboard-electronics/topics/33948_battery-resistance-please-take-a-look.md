# Battery Resistance - please take a look

### Replies: 6 Views: 534

## \#1 Posted by: Nexo Posted at: 2017-09-25T19:24:40.835Z Reads: 94

```
hi there! :slight_smile:

I checked my batteries today, because one of cells in my battery died today (it shows 0,00V) :confused:

so for me, my 4s pack is ruined

but I decided to check resistance of all my lipo packs, and here they are

pack 1: 012, 003, 001, 004
pack 2: 029, 003, 011, 006
pack 3: 009, 002, 002, 002
pack 4: 015, 003, 005, 009
pack 5: 014, 003, 003, 003

Batteries that I use are: Multistar Li-Po 4S 10000mAh 10C

they are working in 3,2-4,2V range according to my FOCBOX settings

Is there something that I should be afraid of?
```

---
## \#2 Posted by: Silverline Posted at: 2017-09-25T19:47:43.174Z Reads: 77

```
Lipo dont like to low voltage. I would not go lower than 3,5v on lipo. On racing quads, we land when the cell voltage is arround 3,8v
```

---
## \#3 Posted by: SilentException Posted at: 2017-09-25T20:17:37.875Z Reads: 68

```
Just curious, what is the procedure you use to get internal resistance numbers?
```

---
## \#4 Posted by: Nexo Posted at: 2017-09-25T20:44:02.071Z Reads: 49

```
SkyRC Imax B6 "Batt Resistance" setting :slight_smile:
```

---
## \#5 Posted by: Martinsp Posted at: 2017-09-25T21:38:18.930Z Reads: 40

```
From what it looks like your charger that you used to measure voltages has something wrong inside it in my opinion. In such low resistance even a not so good solder joint can throw the result off. It seems like your charger detects the first cell (left one in the table) a little too high. Maybe you have a not so good (does not take much to throw off by 1mΩ) somewhere inside the charger or between the charger and battery. 

To confirm or bust my theory, do your batteries get way out of balance? Especially the first cell (left side again) compared to the other 3 cells in the pack.

I think if your resistance readings are correct the would become unbalanced by quite a lot. Reason: the internal resistance of the whole pack is the sum of all cells resistance. If all cells dont have same or very close resistance they will drift because the current would "flow" differently in one of them in this case then in the rest. 
Another reason why I think your readings are incorrect is that manufacturers of these packs match the cells based on their internal resistance so that they dont become unbalanced so easily/quickly.
```

---
## \#6 Posted by: SilentException Posted at: 2017-09-25T21:45:25.827Z Reads: 32

```
Ah :) Well, although it is *a* way to measure internal resistance, the numbers it yields are not that accurate to say at least. Just look at how the first number is much larger than all the other ones... There is a much better way with better results as well but involves some work.

In order to get good internal resistance numbers push some amps through those cells. Don't know what current B6 uses while testing IR but it is charger capable of only 2A discharge which is nothing for our beefy cells :) 8 halogen 20W bulbs, 2s 4p would be discharging about 12A. use 2s 5p for 15A and so on...make a discharger with in-line Amp-meter.

Measure resting voltage of pack / cells after 10min at the constant temperature without load. Best way is just to connect the accurate cell meter on the balance lead and take a picture. Now connect your bulb pack on the LiPo main leads and let it be for couple of seconds. Take a second picture of the cell meter and do some simple math:

( (Vr - Vl) / I ) * 1000

Vr - resting voltage recorded
Vl - voltage under load
I - current in Amps from the in-line Amp-meter

You can do it for the whole pack and each cell.
```

---

# BMS charging new unballenced cell

### Replies: 9 Views: 372

## \#1 Posted by: MaxMalouf Posted at: 2018-03-03T04:59:35.585Z Reads: 70

```
Hi all,

I am using a custom 10s lipo Pac that I made out of 10, 1s packs. 

One of the cells broke so I had to replace it with a new cell. 

Now I'm in a bit of a problem as the new cell is at 3.76v but the remaining 9 cells are at 4.19v 

I tried just charging the board through the bms. But after plugging in my 42v 2a charger, the light doesn't turn red, the light just becomes a brighter green. How do I charge this  new cell to match 4.19v?

By the way the old cells have only been through 2 charges and discharges
```

---
## \#2 Posted by: Namasaki Posted at: 2018-03-03T05:24:50.351Z Reads: 66

```
You'll either need to charge the new cell by itself with an adjustable lab power supply or hobby charger.
Or you'll need to discharge the other 9 cells before connecting the new cell.
If you don't have a lab power supply or hobby charger then the 2nd option is your only hope.
what you could do is disconnect pack from the bms and disconnect the new cell from the pack and discharge the pack until it reaches 3.76v per cell.
you can do this by running board on 9s with the bms disconnected but be careful to monitor the pack voltage while running it so you don't take it down too low. You'll need to adjust the low voltage settings in the Vesc for 9s.
 Once you have the 9s pack down to nominal voltage, reconnect the new cell and reconnect the bms and charge the whole pack.
```

---
## \#3 Posted by: MaxMalouf Posted at: 2018-03-03T05:27:24.323Z Reads: 57

```
Dam yeah I might try the hobby charger. I thought the BMS would balance out the cells.
```

---
## \#4 Posted by: b264 Posted at: 2018-03-03T05:27:40.936Z Reads: 55

```
You can connect the new cell to the pack through a 47 ohm resistor and wait a week or until the voltages match.  Then they should be matched and ready to install.

Keep in mind the pack may be unbalanced and the first time you charge it, they light may not turn red, and it may take an incredibly long time as it's balance-charging at 50mA.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-03-03T05:28:22.018Z Reads: 50

```
Ok, I should have just asked you that first. I could have saved myself a lot of typing.
It's easy to charge a single cell with a hobby charger.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-03T05:35:11.270Z Reads: 47

```
I have experienced the same thing when I replaced a 2 cells in my pack. The bms won't balance if there way off.
```

---
## \#7 Posted by: b264 Posted at: 2018-03-03T05:50:18.750Z Reads: 45

```
It probably will, it just might take an absurd amount of time.  How long did you try for?
```

---
## \#8 Posted by: MaxMalouf Posted at: 2018-03-03T05:57:10.989Z Reads: 44

```
I tried for about half an hour and the voltage was still 3.76v
```

---
## \#9 Posted by: b264 Posted at: 2018-03-03T06:04:08.939Z Reads: 41

```
According to the math, it could charge 160 times slower (as regular 5 amp charging) to balance charge (at 25mA) the P-pack up to the rest of them
```

---

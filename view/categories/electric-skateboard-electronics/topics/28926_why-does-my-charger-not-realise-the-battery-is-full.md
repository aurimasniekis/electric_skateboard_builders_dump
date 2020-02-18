# Why does my charger not realise the battery is full?

### Replies: 7 Views: 418

## \#1 Posted by: Geddi Posted at: 2017-07-28T16:47:52.661Z Reads: 88

```
My charger has an led. Green for not charging/fully charged (means its green when not plugged into the board). And red when it is charging the board.
I use lipo batteries with a 10S Bestech BMS and this [charger](http://www.ebay.de/itm/Hochwertiges-Netzteil-Ladegerat-Ladekabel-42V-2A-fur-36V-Elektrofahrrad-E-Bike-/351890999220?hash=item51ee5687b4:g:gx0AAOSwnbZYE2U~).
I have left it charging for a while after my battery indicator showed 100%, but the light never turns green. I did not wanna let it charge anylonger, because I was afraid it could damage the battery.
Does anyone have any ideas? 
Oh and the board is turned on when charging.
```

---
## \#2 Posted by: mmaner Posted at: 2017-07-28T17:07:39.031Z Reads: 83

```
Its probably balancing the cells.  Check the cells individually and see if they are all at 4.2, I bet you they arent.
```

---
## \#3 Posted by: Tuomalar Posted at: 2017-07-28T17:11:20.086Z Reads: 80

```
Measure voltages from cells if theyre even and where does charger stop. And btw my bms takes forever to charge that last 0.1V
```

---
## \#4 Posted by: rojitor Posted at: 2017-07-29T10:59:58.797Z Reads: 49

```
Out of balance for sure. Leave it plugged for a few hours.
```

---
## \#5 Posted by: Bloop Posted at: 2017-07-29T12:51:05.008Z Reads: 40

```
depending on your indicator. My indicator shows 100% when my batteries are at 41V. So this could be a reason make sure to check with the multimeter the tension in your battery

Also check again the specs of your bms. you should see there at what tension it will stop charging the batteries
```

---
## \#6 Posted by: krloz Posted at: 2017-07-29T12:57:12.280Z Reads: 39

```
I think what your charger is doing is lighting the led green when the amps it is feeding is below a certain value and red when the amps are above that value and thus charging.  So maybe your charger is detecting the idle power consumed by your board as enough to think it is still charging
```

---
## \#7 Posted by: Geddi Posted at: 2017-07-29T14:00:14.990Z Reads: 34

```
I am leaving it to charge for a few hours now and see if it is just balancing. But I thought about what you sayed earlier as well. We will see
```

---

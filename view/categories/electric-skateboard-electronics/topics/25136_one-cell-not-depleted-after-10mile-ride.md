# One cell not depleted after 10mile ride?

### Replies: 12 Views: 702

## \#1 Posted by: SpeedSloth Posted at: 2017-06-11T20:40:13.475Z Reads: 118

```
Hi guys,

So I just took my board out for a 10 mile ride, about 9.5 miles in the VESC battery cut out came on as expected and I pushed the last half a mile back home. It was a very windy day and the board was working hard uphill on the way there and down hill slightly on the way back. 

When I got back to put the lipos on a storage charge they gave some really weird values with one cell being at 4.17V and one being at 2.82! This didn't make much sense to me as all the cells in the pack run in series right? I'd assume that they all would run down relatively evenly. My only thought is that when I push back only one cell got charged? It was the last cell in my 10s pack. Is it possible to balance them when riding?

My setup is a 5000mah combinations of lipos which I charge as two separate 5s batteries.

3s + 2s in series to make 5s with another 3s + 2s or the second. The first 5s was fine voltage wise the second was all over the place. 

Any thoughts or help would be appreciated.

<img src="/uploads/db1493/original/3X/1/e/1e101efc6ee271c434fbe57e772af1cefb5a68e0.JPG" width="375" height="500">
```

---
## \#2 Posted by: anorak234 Posted at: 2017-06-11T21:51:11.233Z Reads: 99

```
This is VERY dangerous. A wire likely came loose inside the battery packaging. You can attempt to balance charge or open it and resolder the wire but I would honestly dispose of the battery ASAP
```

---
## \#3 Posted by: SpeedSloth Posted at: 2017-06-11T21:56:14.672Z Reads: 96

```
I've rebalanced it over a period of about 2 hours and all cells are sitting at 3.7 now. I just don't understand how it could of happened. In a lipo the cells are connected in series so a break to one of the cells would of disconnected the entire pack, a break to any of the balance leads would show 0V on the charger. Neither happened here so I don't think a wire has come loose inside the lipo itself.
```

---
## \#4 Posted by: SpeedSloth Posted at: 2017-06-11T22:02:33.498Z Reads: 91

```
I'm also struggling to believe that the cell wasn't used at some point as I got equal milage to normal on a windy day and according to strava was travelling faster than normal at 40kmh, I think I'd of noticed a power reduction which leads me to believe that pushing with the board still on recharged just one cell.
```

---
## \#5 Posted by: wmj259 Posted at: 2017-06-11T22:07:03.738Z Reads: 89

```
Are all the packs the same mAh and C rating?
```

---
## \#6 Posted by: SpeedSloth Posted at: 2017-06-11T22:19:18.038Z Reads: 84

```
Yep all 5000mah 20C
```

---
## \#7 Posted by: wmj259 Posted at: 2017-06-11T22:26:10.226Z Reads: 81

```
Can you post pictures of the battery wiring.
```

---
## \#8 Posted by: SpeedSloth Posted at: 2017-06-12T08:33:51.433Z Reads: 70

```
<img src="/uploads/db1493/original/3X/a/1/a1d8892bb5a4779c4ccff7d44328c3da1717af78.png" width="666" height="500">
```

---
## \#9 Posted by: Nordle Posted at: 2017-06-12T12:39:44.360Z Reads: 61

```
Also of real world wiring?
```

---
## \#10 Posted by: SpeedSloth Posted at: 2017-06-12T15:53:16.105Z Reads: 46

```
In the current configuration I can't really show it to you in a useful way. It's spread over two separate enclosures and the way the wires are packed in makes it hard to determine what goes where. I checked that the wiring to match the wiring diagram and with a voltmeter before packing it in the case and am confident that it is to the diagram I posted.
```

---
## \#11 Posted by: Dornacht Posted at: 2017-06-12T20:08:14.219Z Reads: 30

```
This also happened to me in the past most likely a nickel strip inside the battery tore and sometime will make contact sometimes not and the arcing will be dangerous take @anorak234 advice
```

---
## \#12 Posted by: SpeedSloth Posted at: 2017-06-13T11:25:05.972Z Reads: 15

```
Will take the advice to keep it safe, thanks both. I still don't understand the how cell would keep it's voltage in the arcing condition? Did you ever look further into the battery to see if this was the cause?
```

---

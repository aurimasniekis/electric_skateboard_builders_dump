# Bypassing Discharge (White square BMS)

### Replies: 12 Views: 1173

## \#1 Posted by: NickTheDude Posted at: 2017-08-17T20:30:29.697Z Reads: 156

```
Hey guys, I got one of these BMSes http://www.ebay.ca/itm/331883424408 
<img src="/uploads/db1493/original/3X/2/c/2cc2bc62205e57a8691f4ed7afbae000a5d9bda1.png" width="500" height="371">

I've looked through a bunch of threads and this seems to be how I would wire it up in order to bypass discharging:
<img src="/uploads/db1493/original/3X/a/4/a416b71343761a03ec6295ddc26196227cd4b571.png" width="553" height="397">

Is this correct? I was just looking for some clarification so I can move forward without accidentally blowing things up :P
```

---
## \#2 Posted by: krloz Posted at: 2017-08-17T20:50:12.124Z Reads: 140

```
Is correct.
missing some kind of sparkswitch/loop key so your vesc isn't always on
```

---
## \#3 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-17T21:04:13.101Z Reads: 136

```
But since "CH+" is connected to the positive of the battery, doesn't that screw things up? 

Say the BMS wants to charge group 5, then it applies power to "B6" and "B5". But if the "CH+" is also connected directly to the battery's positive(through "anode B+") that should screw something up, right?
```

---
## \#4 Posted by: krloz Posted at: 2017-08-17T21:08:22.476Z Reads: 131

```
I dont think I quite understood you there. 
the charge+ is wired directly to the battery and the ch- is wired through the bms to have overcharge protection. ie the bms cuts power from charging port when the battery is full, the balance wires are for the bms to be able to balance each cell group and to measure the voltage of each cell group to be able to provide undervoltage detecion. ie to cut power out of the battery if a cell gets too low. you wont be having this last feature as you are bypassing discharge protection.
nothing screwed up here as long as you properly set minimum voltages in vesc so it wont over discharge your battery
```

---
## \#5 Posted by: mccloed Posted at: 2017-08-17T21:15:33.237Z Reads: 120

```
I have had two of those BMS's. They both killed cells in my 10s packs. I would recommend not using a BMS over using that BMS.
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-08-17T21:16:21.305Z Reads: 116

```
Fantastic... Any idea what the problem was? Was it overcharging cells?
```

---
## \#7 Posted by: mccloed Posted at: 2017-08-17T21:25:02.895Z Reads: 110

```
No idea what the problem was. Two of the cells were drained to zero after riding. I think it's taking power from them when it's not charging.:confused:

I would recommend spending the extra money on a quality BMS.(supower, batterysupports, etc.)
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-23T23:56:14.562Z Reads: 101

```
[quote="NickTheDude, post:6, topic:30919, full:true"]
Fantastic... Any idea what the problem was? Was it overcharging cells?
[/quote]


The problem is simple:
<img src="/uploads/db1493/original/3X/b/4/b42182b48999a3052dbc4d018bf8910ab58e94ff.png" width="217" height="53">
Quality BMS's don't come dirt cheap.
That's my opinion anyway.
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-08-24T02:08:44.184Z Reads: 93

```
Fair enough, I figured it'd be worth a shot since I'm only using it for charging. Once I get a hold of a charger I'll test it for science and report back.
```

---
## \#10 Posted by: rich Posted at: 2017-08-24T14:10:50.633Z Reads: 89

```
I use the same BMS bypassed for charging my 10s 10Ah Lipo since 2 months without problems (not that I recommend it but in my case it works so far, fingers crossed).

But @mccloed is scaring me, did you use this BMS for discharging, too?
```

---
## \#11 Posted by: mccloed Posted at: 2017-08-24T14:30:27.339Z Reads: 89

```
Nope. Just charging. I gave another one a chance on a different board and had the same results but I caught it before it destroyed any of the cells. Sorry to scare you but this was just my experience. Hopefully you don't have any issues.
```

---
## \#12 Posted by: rich Posted at: 2017-08-24T15:04:00.470Z Reads: 82

```
No, thanks for scaring me, think i'll switch to better BMS :sunglasses:
```

---

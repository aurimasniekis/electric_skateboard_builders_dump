# Usable capacity of cells

### Replies: 11 Views: 311

## \#1 Posted by: 12meterkuk Posted at: 2018-07-07T13:22:21.573Z Reads: 134

```
I was looking at the discharge curve of the 30q and noticed that only 2.25ah is used when voltage drops to 3.2v which is what my raptor 2 cuts off at. In what hours that’s only 324wh so I was wondering if that could be the cause of me only getting 20 km with 16wh per km?
```

---
## \#2 Posted by: Randyc1 Posted at: 2018-07-07T13:31:47.727Z Reads: 132

```
What size battery ?,..what kind of board ?
```

---
## \#3 Posted by: Holyman92 Posted at: 2018-07-07T13:45:25.845Z Reads: 126

```
I have a 10s5p and the voltage sag is real... I use it as a daily commuter and halfway through my.ride one way (1.5 - 2 miles) i go from being able to hit 20mph with half throttle (I usually coast at 10-15 tho), to going less than mph 5mph and having to pull over (usually on the way home)and that's from a full charge... for short runs it works great and can go several days without a charge
```

---
## \#4 Posted by: 12meterkuk Posted at: 2018-07-07T13:56:34.959Z Reads: 118

```
30q 10s4p.    

10c
```

---
## \#5 Posted by: karma Posted at: 2018-07-07T14:32:31.975Z Reads: 106

```
The full capacity which cells are rated at is the maximum you could achieve, full charge and down to 2.5V and like 1C. This is however not how you would use the cell. The current at which you discharge also has a large impact on how run time, more current = more losses. Only using SoC of 30-80% (that is, don't fully charge, don't drain it empty)  will make the battery last A LOT longer, like 2-8 times longer. If you want maximum range you should fully charge to 4.2v/cell and discharge to around 3v/cell. 16wh per km is realistic if you bomb som hills, accelerate and break alot.
```

---
## \#6 Posted by: Randyc1 Posted at: 2018-07-07T15:16:37.613Z Reads: 99

```
16 wh/km seems high for urathane wheels. What are other R2 getting in avr range?
```

---
## \#7 Posted by: 12meterkuk Posted at: 2018-07-07T15:27:30.065Z Reads: 94

```
I accelerate and brake pretty hard and go full speed most of the time. I’m also 100kg with my backpack and books and stuff
```

---
## \#8 Posted by: Okami Posted at: 2018-07-07T19:26:27.956Z Reads: 81

```
Cant u put cutoff at 3.0v ? 

Board will probably feel weak but might be able to sqeeze a little bit more out of it..
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-07-09T10:07:48.478Z Reads: 52

```
The board is bypassed which is good but I can’t change the values of the cutoff without flashing new firmware(2.80 r2 firmware is very restricting) and that would also void my warranty
```

---
## \#10 Posted by: bartroosen12 Posted at: 2018-07-09T11:06:17.274Z Reads: 45

```
Only 20km with a 450Wh battery pack seems low for me.
Okey if you fo hills and crazy acceleration.
I have a 350Wh pack (10S) and I get like 30km, but yeah I got not those powerfull hubmotors.
Are you sure the pack is fully charged? And all cells are balanced?
```

---
## \#12 Posted by: 12meterkuk Posted at: 2018-07-09T11:25:37.621Z Reads: 35

```
Yup, fully charged. I think it’s because of the high cutoff. No hills where I live
```

---

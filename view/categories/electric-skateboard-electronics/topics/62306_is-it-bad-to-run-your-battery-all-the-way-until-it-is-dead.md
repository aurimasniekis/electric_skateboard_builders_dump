# Is it bad to run your battery all the way until it is dead?

### Replies: 17 Views: 496

## \#1 Posted by: MarcShane Posted at: 2018-07-19T20:39:47.250Z Reads: 218

```
It is bad for the battery or any of the other electrical components?
```

---
## \#2 Posted by: b264 Posted at: 2018-07-19T20:42:16.736Z Reads: 220

```
"dead" doesn't mean anything.  Are you referring to 0.0 volts per cell?  If so, then yes.  Also, only if it's a lithium-based chemistry.  What chemistry battery?
```

---
## \#3 Posted by: gliz5714 Posted at: 2018-07-19T21:13:40.196Z Reads: 200

```
To expand on b264 - Typically ESCs and VESCs have 'cut off' limits for your battery.  Basically each battery cell holds appx 4.2v and when it 'dies' when connected to a vesc you can set it to die at 3.2v (or something around there) - so technically the battery still has juice in them but it is there to not destroy/ruin the battery.  This is what many here will tell you to set it at at least.  If you set your VESC and put it at 0.0v, then yes, you will harm the battery. 

I also apologize if I am a bit off on the electric numbers, I am not currently in the eskate world, just got out last year and contemplating building again!
```

---
## \#4 Posted by: b264 Posted at: 2018-07-19T21:17:40.583Z Reads: 190

```
I didn't put cutoff numbers on purpose because different chemistries have different ones.  If you used LiFePO4 cutoffs for li-ion, for example, you will damage the cells.  So those numbers above are examples only.
```

---
## \#5 Posted by: MarcShane Posted at: 2018-07-21T13:21:16.751Z Reads: 147

```
Can anyone tell me what the cut off should be for Samsung 30Qs?
```

---
## \#6 Posted by: L3chef Posted at: 2018-07-21T13:28:21.076Z Reads: 144

```
I have mine cutoff to start att 33v and ned at 30v
```

---
## \#7 Posted by: PXSS Posted at: 2018-07-21T14:22:42.227Z Reads: 135

```
Absolute low is 2.5 per cell. What I use: 2.8 per cell. What most use: 3.0 per cell.
```

---
## \#8 Posted by: b264 Posted at: 2018-07-22T01:22:27.423Z Reads: 109

```
[quote="L3chef, post:6, topic:62306, full:true"]
I have mine cutoff to start att 33v and ned at 30v
[/quote]

That's for 10S.  So for 30Q cells that'd be 3.3V or 3.4V start and 3.0V or 2.8V end per cell.  So for 10S, multiply by ten and for 11S multiply by eleven...
```

---
## \#9 Posted by: Holyman92 Posted at: 2018-07-22T01:45:18.868Z Reads: 93

```
On a side note... what's a good start and end cutoff for a 12s3p 30Q pack
```

---
## \#10 Posted by: Ixf Posted at: 2018-07-22T04:16:44.341Z Reads: 90

```
[quote="b264, post:8, topic:62306"]
30Q cells that’d be 3.3V or 3.4V start and 3.0V or 2.8V end per cell
[/quote]

Take those values multiply by the # of S in your pack
```

---
## \#11 Posted by: L3chef Posted at: 2018-07-22T10:00:25.512Z Reads: 81

```
I have no idea why I left that part out :sweat_smile:
Yup that's for 10s
```

---
## \#12 Posted by: sayekim Posted at: 2018-07-22T14:34:53.275Z Reads: 64

```
What is the logic here behind the cut off calculation? Why is it more or less depending on series?
```

---
## \#13 Posted by: AutoItKing Posted at: 2018-07-23T01:45:21.171Z Reads: 59

```
Cutoff keeps the ESC from over discharging your pack (this can damage the batteries).
A 10S pack will have a voltage range of 30 to 42 Volts (10 * 3.0 to 10 * 4.2). Basically total battery voltage is dependent on how many cells are in series (xS*V_batt where x is the # of cells in series). Putting two batteries in parallel just increases the capacity, not the voltage. Think of two square blocks. You can put them on top of each other making a block twice as tall (2x voltage) or next to each other for a wider block with the same height (2x capacity). You cannot increase both without more cells. To double voltage and capacity you need four times the batteries. I hope that makes sense.

Edit: capacity in mAh; capacity in Wh will increase both ways (mAh * voltage).
```

---
## \#14 Posted by: sayekim Posted at: 2018-07-23T09:16:12.033Z Reads: 53

```
Thanks this idiot did not realize that each individual cell would be lower voltage with more cells in series if you kept the cutoff the same as with lower cells in series. 

30/10=3.0
30/12=2.5

So to still be in the safe range I could go with 34 volts cutoff at the least I would say for 12s. 
34/12=2.83
```

---
## \#15 Posted by: AutoItKing Posted at: 2018-07-23T17:43:13.698Z Reads: 41

```
Lithium ion cells have basically no juice left in them below 3V anyways. 2.8V while technically safe will not gain you anything and may shorten your battery's life. I would use 3V per cell as a safe cutoff. You can go lower, just know that you don't gain much.
```

---
## \#16 Posted by: b264 Posted at: 2018-07-23T18:13:16.356Z Reads: 34

```
Setting your cutoff at 2.8V will probably get you ten meters more range than setting it at 3.0V :rofl:
```

---
## \#17 Posted by: sayekim Posted at: 2018-07-23T18:27:20.422Z Reads: 29

```
For sag reasons though 2.8 would be preferred.
```

---

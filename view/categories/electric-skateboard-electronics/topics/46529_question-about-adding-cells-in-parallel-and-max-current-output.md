# Question about adding cells in parallel and max current output

### Replies: 5 Views: 504

## \#1 Posted by: t0m_r1dd1e Posted at: 2018-02-15T20:43:15.493Z Reads: 77

```
Just a quick question to help understand some electrical concepts:

Say I have a 12s2p battery with 30q cells. Each cell has a max continuous output of 15 amps, according to the spec sheet. How do I calculate the voltage, max current, and max power of the whole battery? How does that change if I decided to do 12s3p instead? 

Thanks all
```

---
## \#2 Posted by: cwazy1 Posted at: 2018-02-15T20:52:31.837Z Reads: 77

```
12x 3.6 = your nominal voltage (your s number multiplied by 3.6 for nominal, or 4.2 for max) 

2x 15 = your max continuous amperage (change 2 to 3 for a 3p pack, change 15A to whatever max if you change cell type/model) 

your motor = max wattage

3000mah x 2 = your max capacity of the battery. (mah of cell multiplied by the p count)
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2018-02-15T21:01:30.377Z Reads: 67

```
So let me see if I have this:

12s2p max continuous current = 30 amps
           max power (ignoring esc and motor limits) = 30 x 12 x 3.6 = 1296 watts nominal
                                                                          or     30 x 12 x 4.2 = 1512 watts at full charge (not really real-world possible)

12s3p max continuous current = 45 amps
max power nominal = 45 x 12 x 3.6 = 1944 watts 
or 45 x 12 x 4.2 = 2268 watts full-charge max

Is that correct? 
Does that mean that adding additional cells in parallel (increasing p number) always increases the battery's maximum output current?
```

---
## \#4 Posted by: cwazy1 Posted at: 2018-02-15T21:02:25.570Z Reads: 61

```
bingo, you got it.
```

---
## \#5 Posted by: t0m_r1dd1e Posted at: 2018-02-15T21:04:42.863Z Reads: 57

```
Thanks mate!
```

---

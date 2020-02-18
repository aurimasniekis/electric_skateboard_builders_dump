# How to test a cells resistance?

### Replies: 13 Views: 207

## \#1 Posted by: accrobrandon Posted at: 2019-01-24T15:25:02.067Z Reads: 83

```
Can someone break down how this done? I looked around...I know people mention doing it if they feel like a cell or cells are drifting in a pack but havent seen anything straight forward as to what to do...

and then what values would one be looking for?
do those values change based on the current voltage of the battery.. like 4.2v vs 3.6v?

asking specifically for 18650 in my case.

thanks
```

---
## \#2 Posted by: b264 Posted at: 2019-01-24T15:32:37.335Z Reads: 81

```
The short answer is a nice hobby charger offers that feature.

The long answer is mathematically, you'd have to use Ohm's Law with a known load and calculate all the numbers...
```

---
## \#3 Posted by: accrobrandon Posted at: 2019-01-24T15:34:08.657Z Reads: 81

```
i have a imax b6? i dont use it very often so im not sure of its features...??
```

---
## \#4 Posted by: b264 Posted at: 2019-01-24T15:41:41.579Z Reads: 74

```
I believe that one does have an internal resistance testing feature.
```

---
## \#5 Posted by: Indiangummy Posted at: 2019-01-24T15:45:24.442Z Reads: 66

```
Can you also use a multimeter? most multimeter's have a feature that allows you to see the resistance....no?
```

---
## \#6 Posted by: Mich21050 Posted at: 2019-01-24T15:46:31.709Z Reads: 62

```
You have to put a load on it to get an accurate result so in my opinion no.. :slight_smile:
```

---
## \#7 Posted by: Indiangummy Posted at: 2019-01-24T15:49:33.755Z Reads: 58

```
Well, I guess you are right. if I'm not mistaken the multimeter would put current through the cell and calculate resistance that way, but I guess that would be the resistance with close to no load.
```

---
## \#8 Posted by: Benjamin899 Posted at: 2019-01-24T15:51:04.509Z Reads: 57

```
i used the liitokala lii-500 to show me the internal resistance, but i doubt the accuracy.
```

---
## \#9 Posted by: Vanarian Posted at: 2019-01-24T15:51:41.927Z Reads: 54

```
A hammer and a woodplank or an anvil will cut to the job if you only need to test _resistance_

...Ok I'm out :door:
```

---
## \#10 Posted by: linsus Posted at: 2019-01-24T15:54:30.347Z Reads: 53

```
Generally the hobbychargers dont give you the actual internal resistance, however since the calculation is done the same way per parallell group, any difference in those values will tell you if something is off or not.
```

---
## \#11 Posted by: visnu777 Posted at: 2019-01-24T16:21:45.740Z Reads: 51

```
I have a xtar vp4 dragon which is basically a 4x single cell charger with ir probes.
```

---
## \#12 Posted by: b264 Posted at: 2019-01-24T16:27:07.984Z Reads: 46

```
The way to get the actual internal resistance is to measure the open voltage of the cell, then connect a load with a known resistance, and quickly measure the voltage across the load.  Using Ohm's Law, you can deduce the amount of extra resistance that must be in the cell itself.

So if Vu is unloaded cell voltage and Vd is loaded cell voltage and Rd is the resistance of the load, then Rc (internal cell resistance) can be calculated

Rc = (Rd * Vu / Vd) - Rd

So, for example, if you had a 20 watt resistor that measures 10.0 ohms - and you have a cell that measures 4.01V -- and you connect the resistor to the cell and quickly measure 3.984V across the resistor before you unhook it again ... then you can calculate a (10.0\*4.01/3.984)-10.0 = 65.2mΩ internal cell resistance
```

---
## \#13 Posted by: accrobrandon Posted at: 2019-01-24T17:33:18.351Z Reads: 34

```
and how do we know what is good number for resistance and bad? the lower the better?? is there a particular range to be within which is good vs ok vs bad?
```

---

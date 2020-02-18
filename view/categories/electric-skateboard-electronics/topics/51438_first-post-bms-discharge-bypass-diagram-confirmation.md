# First Post! BMS Discharge Bypass Diagram Confirmation

### Replies: 10 Views: 910

## \#1 Posted by: civic619 Posted at: 2018-04-06T23:06:57.734Z Reads: 180

```
Hi.  First post here.  Awesome site!

Just wanted to get some Esk8 expert confirmation on the wiring diagram that I mocked up.  Based on the many threads I've read related to bypassing the BMS for discharge, this is what I have gathered.  I will be programming the VESCx to maintain the battery packs amperage draw to prevent the cells from over discharging.  The BMS will only be used to balance charge the cells.   ![20180406_155450|582x500](upload://nLT87DcMcu8G3L8A4kMiP66y5QJ.jpg)

Does it look good?  

Thanks!
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-04-06T23:23:59.611Z Reads: 156

```
damn youre a good artist
```

---
## \#3 Posted by: treenutter Posted at: 2018-04-06T23:37:02.151Z Reads: 151

```
@civic619 you could post this in our “beautiful diagrams@ thread.
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-04-07T04:27:12.326Z Reads: 136

```
to answer the question, looks good to me. 

your bms wiring and balance leads look good, you got the voltmeter on the correct end of the loop key so it doesn't stay on indefinitely.

think you're good to go.
```

---
## \#5 Posted by: b264 Posted at: 2018-04-07T04:43:04.598Z Reads: 130

```
[quote="civic619, post:1, topic:51438"]
Does it look good?
[/quote]

No, I don't think so.  Everything except the balance wires is good, except making the lines fatter that need to be 10AWG is helpful, and running a positive to the battery from the charge port and a positive to the battery from vesc/loop key would help to, because one needs to be 10AWG and the other 22AWG.  You don't want 10AWG wire on your charge port.

But the balance wires I don't think are correct.  I don't know what BMS you are using, but I have a bestech D190 here I am looking at and it's as follows:


B0 is B-
B1 would be what you have labeled 7
B2 would be what you have labeled 6
B3 would be what you have labeled 5
B4 would be what you have labeled 4
B5 would be what you have labeled 3
B6 would be what you have labeled 2
B7 would be what you have labeled 1, same potential as B+


Electrically it's the same, but I tend to advise putting the loop key on the negative line because the wiring ls less confusing.  Then everything hooks up to battery positive and it's only the negative side that's switched.  Instead of some switched negatives and some switched positives.
```

---
## \#6 Posted by: civic619 Posted at: 2018-04-07T06:03:25.382Z Reads: 114

```
Thanks for the input and suggesting using the appropriate gauge wires.  For reference, I have attached the diagram that I received with my BMS.  I think I followed it correctly despite I don't know how to read Chinese.![BMS|526x499](upload://jrauoWz2NQqCSmZebpugCmXklLL.jpg)
```

---
## \#7 Posted by: civic619 Posted at: 2018-04-07T06:03:52.198Z Reads: 107

```
Thanks everyone who also responded.  I appreciate it!
```

---
## \#8 Posted by: b264 Posted at: 2018-04-07T06:27:08.515Z Reads: 104

```
So then you should have 8 balance wires, where B1 is B- and B8 is B+

Some BMSs omit the first one because they can get the same potential from B- wire but yours appears to have both.  So all the wires in the BMS photo would be 22AWG high strand-count silicone-insulated tinned copper wire and the load on the far left would be absent
```

---
## \#9 Posted by: Namasaki Posted at: 2018-04-07T13:41:06.759Z Reads: 92

```
Good eye @b264
You are correct. 
@civic619 
The cells are numbered correctly but the balance wires are reversed in this diagram. 
 You would have cooked your bms if wired that way.
```

---
## \#10 Posted by: pedro Posted at: 2018-08-09T13:38:13.999Z Reads: 54

```
Some one know if this "BMS" is working like Bypass?
Becouse i buyed and i think is not safe for discharge.
I want to be safe!!

![bms|448x500](upload://bBDUe6E38r337h9a7hLq5c67eKR.JPG)
```

---

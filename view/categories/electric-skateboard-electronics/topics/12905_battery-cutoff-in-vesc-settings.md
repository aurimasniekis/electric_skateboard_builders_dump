# Battery cutoff in vesc settings

### Replies: 5 Views: 1101

## \#1 Posted by: jak Posted at: 2016-11-11T22:42:02.785Z Reads: 155

```
hey guys just a quick question in the BLDC program.  Im running (4) 4S @ 5k mah batteries in series and then in parallel to make 8s @ 10k mah.  i was told the recommened cuttoff to start at 3.4v and end at 3.2v but to be safer use 3.6v and 3.4v respectively. my question is when setting my cutoff for the battery do i need to double those values because of adding the batteries together? also what would be the recommended batt min (regen)? it is currently set at -10.00
 
thanks Jak
```

---
## \#2 Posted by: JuniorPotato93 Posted at: 2016-11-11T23:18:18.608Z Reads: 149

```
Those are the values _**PER CELL**_ of the battery.

You're going to be using 2 X 4S for a total of 8 cells so you actually multiply these values by 8, not 2. You're starting cut off and cut off is going to be-using the non conservative values- 27.2V and 25.6V, respectively. Using conservative values, 28.8V and 27.2V, respectively.   

You do not have to double these vales because you are running the batteries in parallel either.

You'll have 4 batteries total from what I'm reading here, 2 sets of series, in parallel, but that also doesnt affect how you multiply the cut off values. Just the total number of cells your system runs at, the series part, is what determines that. So your system will still function with the setting above.
```

---
## \#3 Posted by: jak Posted at: 2016-11-11T23:26:38.911Z Reads: 138

```
makes perfect sense thanks! any idea on the battery min regen? i figured -10.00 would be a conservative setting.
```

---
## \#4 Posted by: JuniorPotato93 Posted at: 2016-11-11T23:57:43.753Z Reads: 125

```
I think it's probably a reasonable amount. I remember someone once posted the range -7.00 to -15.00 depending on your set up was acceptable. I used -10, had some issues and brought it down to  -7.5V if I remember correctly and that seemed to fix it. I was also running dual vescs so it was actually -15V going back into the battery.
```

---
## \#5 Posted by: jak Posted at: 2016-11-12T00:02:43.096Z Reads: 115

```
sounds good. thank you. i am running single drive so i will try it @ -10.00
```

---

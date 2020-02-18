# Batterie min help

### Replies: 13 Views: 320

## \#1 Posted by: Devilmycry Posted at: 2018-06-04T14:46:39.140Z Reads: 125

```
Hi everyone 
Hi have questions 
I run 12s7p 30Q 
What the max battery min I can make 
 I run each vesc at -15 and my motor at -60 
I think what I know is each cell can get 4A 
4*12=48 
For my 2 vesc6 i’m At 30A full brake 
Is look like I can go 18A more (bc if I can go higher it will be brake better when I go fast ) 

Can you tell me what is the best for me for not domage my battery 
Thank you
```

---
## \#2 Posted by: rey8801 Posted at: 2018-06-04T17:01:50.261Z Reads: 108

```
The batt min is calclulated on the capacity. So 30Q are 3000mAh battery. 7p x 3A = 21A...I would suggest tot start with 2c for batt min so -41A total / 2 vesc = -20A each vesc... Batt min will mainly affect brake at higher speep so try it out carefully.
```

---
## \#3 Posted by: Hummie Posted at: 2018-06-04T17:18:25.299Z Reads: 107

```
can you increase the regen without increasing the braking power?
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-04T17:22:00.824Z Reads: 101

```
I think the only way is to reduce the braking curve later on in the ppm signal
```

---
## \#5 Posted by: deucesdown Posted at: 2018-06-04T17:38:17.559Z Reads: 94

```
Actually OP is correct, samsung specs .5c (1.5a) for standard charge, 4a for rapid charge.

So 4a per cell, 7 cells per group, means 28a total charge rate within mfg's rapid charge spec. The safe number for batt min per vesc is -14a.

You can likely set more, but you would no longer be °safe°.

Note, the number of series groups does not affect amperage.
```

---
## \#6 Posted by: rey8801 Posted at: 2018-06-04T17:43:05.584Z Reads: 86

```
I gave 2c as general value but it's of course correct ot check the cell specs. Thank yuo for the input.
```

---
## \#7 Posted by: Devilmycry Posted at: 2018-06-04T17:57:25.041Z Reads: 85

```
Ok I see 
Thank you everyone
```

---
## \#8 Posted by: Devilmycry Posted at: 2018-06-04T17:59:32.599Z Reads: 86

```
Ok thank you more P I have more I can get my battery min 
Thank you 
And about the vtc6 
It will be the same
```

---
## \#9 Posted by: Devilmycry Posted at: 2018-06-05T01:49:01.888Z Reads: 76

```
What is the C and where I can find it thank you
```

---
## \#10 Posted by: Hummie Posted at: 2018-06-05T03:38:17.910Z Reads: 69

```
It'll be dubbed c rating if lipo or peak discharge and continuous discharge on ion.
```

---
## \#11 Posted by: deucesdown Posted at: 2018-06-05T03:49:01.084Z Reads: 64

```
[quote="Devilmycry, post:9, topic:57777"]
What is the C
[/quote]

"C" is the capacity of the battery in amps. 30Q is 3000mah, 1C for 30Q is 3000ma (aka 3 amps).

Often the charge and discharge rates are stated as some proportion of C. A good rule of thumb for modern lithium batteries is 1C max charge rate. 30Q is unusual in the the manufacturer actually recommends 0.5C charge rate.
```

---
## \#12 Posted by: Hummie Posted at: 2018-06-05T05:46:31.695Z Reads: 54

```
c rate reveals the stated discharge ability.  multiply the c rate by the capacity.  often exaggerated with lipo and rare on ion cells and more often on ion cells I read an actual amperage of charge or discharge
http://www.datasheet39.com/PDF/951041/INR18650-30Q-datasheet.html

   when the discharge  or charge is pushing the cells limits then the voltage will sag (decrease) and the cell will get warm and that damages it leading to less ability to store energy.
```

---
## \#13 Posted by: rey8801 Posted at: 2018-06-05T06:35:24.690Z Reads: 46

```
@Hummie @deucesdown gave a full explanation. Thx guys!
```

---

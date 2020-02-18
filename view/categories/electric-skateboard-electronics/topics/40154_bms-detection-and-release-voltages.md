# BMS detection and release voltages?

### Replies: 6 Views: 1578

## \#1 Posted by: richardx Posted at: 2017-12-05T02:42:53.266Z Reads: 100

```
Hi all, I'm going through the process of getting a Bestech BMS ordered (D528V1 if anyone's wondering) and I have absolutely no idea what the detection and release voltages are. Can someone explain how I should get these set? Also, I'm planning a 10S4P pack of Samsung 30Q cells, so if anyone could share their parameters that'd be great too. Thanks!
```

---
## \#2 Posted by: krloz Posted at: 2017-12-05T07:58:26.106Z Reads: 90

```
Assuming detection and release of overvoltage protection.  Detection is the voltage at wich your overvoltage protection its triggered, blocking any more input power from charging.  Release is the voltage at which the protection is turned off and the bms allows charge input again.  
You could go 4.2v per cell for detection maximun and 4.1 to 4.15 for release.
```

---
## \#3 Posted by: rich Posted at: 2017-12-05T10:26:45.782Z Reads: 79

```
I ordered from bestech last month and wanted to change some settings, too. The overcharge settings were not adjustable (not like I wanted) but the over discharge detection and release voltages I set to 3V because I use them for Lipo and Li-ion. But in your case you could buy it with the standard settings, it's already set for Li-ion.

BTW the shipping from china to my flat in europe was 1 day :laughing:
But you'll have to pay tax.
```

---
## \#4 Posted by: richardx Posted at: 2017-12-06T22:54:33.785Z Reads: 59

```
Why 4.2V? Wouldn't the balancing fail then? The standard cutoffs as Bestech have provided are:

Overcharge detection: 4.25V
Overcharge release: 4.05V

Overdischarge detection: 2.70V
Overdischarge release: 2.90V

Will this work for me? Also, what should I set the two overcurrent limits to?
```

---
## \#5 Posted by: krloz Posted at: 2017-12-07T08:51:35.281Z Reads: 46

```
The higher you stop charging the batteries the sooner they will die. I don't charge over 4.2v
```

---
## \#6 Posted by: composites_r_awesome Posted at: 2018-05-29T19:32:20.051Z Reads: 32

```
Hey Thanks for the input!  
  
One question tho, what shipping did you have? Last time I ordered from MayTech I used DHL  and they marked the shipping value under 22€ which made it through customs then. It still was like 70€ for shipping but came out cheaper without taxes<:P
```

---

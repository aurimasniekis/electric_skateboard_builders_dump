# Question about 12S battery with JST-XH 7 pin balance wires

### Replies: 8 Views: 300

## \#1 Posted by: billappleton Posted at: 2018-11-14T00:33:48.344Z Reads: 70

```
Hi all,

I have a Chargery charger which will do 12s. Here is a picture of the pins on the charger and the balance cable connection diagram for the 12S battery. Please look at how we are hooking up the 12S cells to the two JST-XH 7pin connectors. Does this look right?

Thanks in advance



![bms_design|579x500](upload://zlct82xz7hlryYIGPoHTld15fQm.jpeg) ![bms_pins|650x500](upload://nKlB9WGGf783xrLYW3TcKZeK0gT.jpeg)
```

---
## \#2 Posted by: Jumpman Posted at: 2018-11-14T00:43:07.144Z Reads: 60

```
Without knowing anything about the charger, or your battery, it seems like you may have the connectors labelled the wrong way around.  Bottom connector 1-6, and top connector 7-12.
```

---
## \#3 Posted by: billappleton Posted at: 2018-11-14T01:01:37.046Z Reads: 54

```
Thank you for helping with this. The battery is a 12S4P 18650. The Chargery charger is really nice but with limited instructions. I definitely want to get the right JST-XH in the right connection.
```

---
## \#4 Posted by: billappleton Posted at: 2018-11-14T03:20:29.976Z Reads: 53

```
so is this diagram correct?  Thanks

![bms_design2|579x500](upload://tQ4ygwIGMqXcYfjxhi72k8VLWiH.jpeg)
```

---
## \#5 Posted by: Jumpman Posted at: 2018-11-14T11:12:32.874Z Reads: 48

```
Yes, this looks correct now, but always follow the charger instructions.  If you are unsure about anything you can always contact the manufacturer directly for their advice.
```

---
## \#6 Posted by: rich Posted at: 2018-11-14T16:21:41.232Z Reads: 36

```
Just to make it more clear

![diagrEdit|579x500](upload://eRTPLkFEpPVn1uufyA1WAMoBJzJ.jpeg) 

I guess you have to connect the main power leads of the battery as well with this serious charger.

It should be this one, you can find manuals for every charger there.
Am I the only one using google? :wink:

http://chargery.com/C4012B.asp

EDIT: the diagram above is only right if the charger is charging the whole 12s battery at once. If it's supposed to charge 2x 6s batteries at once it's a different and more complicated story.
```

---
## \#7 Posted by: janpom Posted at: 2018-11-14T16:37:16.731Z Reads: 32

```
Checking the voltage between the wire 0 and 13 would be worthwhile. It should be 40-50V. If it's not, check that you don't have the two sets of balance leads swapped.
```

---
## \#8 Posted by: billappleton Posted at: 2018-11-14T16:56:06.264Z Reads: 28

```
Thanks all you guys are awesome. I have the chargery manual but it is not very clear on this.

The charger is a beast.
```

---

# External charging port help!

### Replies: 4 Views: 1657

## \#1 Posted by: Pablo_702 Posted at: 2016-06-15T17:55:26.193Z Reads: 196

```
i finally started receiving my parts next ill be ordering vesc from ollin, i have a 6374 149kv and 3 x 3S1P 30C 8000mah in series for a 12S and in their website toward the bottom of the vesc page you can choose the connectors that you want in the vesc i was thinking 4mm on the motor and 5.5mm on the battery but my main goal is to be able to charge it from an external port with out having to remove the enclosure so i read xt30-xt60-xt90 i dont know what they are forbut i understand i should pay attention to this in order tho achieve my main goal, anyone can help with this????
```

---
## \#2 Posted by: Jinra Posted at: 2016-06-15T18:01:37.534Z Reads: 194

```
I'm assuming you meant to say you have 4 x 3S1P packs as 3 x 3 only gets you 9S. Connector won't matter since you'll need to solder on a charge port in the layout as well. Though it might be easier to just plug the cells to charge since you'll need to balance charge them. You can also make a VGA charger like this http://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242
```

---
## \#3 Posted by: Pablo_702 Posted at: 2016-06-15T18:15:38.311Z Reads: 186

```
yes i meant times 4 (X4) yeah i was looking into that last night,taking the cells out of the skate is not an option i seen some of the guys here they have 2 ports the balance port and then the other port mounted on the outside of the enclosure
```

---
## \#4 Posted by: oriol360 Posted at: 2016-06-15T19:25:47.205Z Reads: 166

```
So i've been looking into more options for my customers who want to set up a simple charger for 12S.
I always recommend getting a BMS but I understand not many people want to incorporate more bulk to their build.

If you have a charger like this: http://www.hobbypartz.com/75p-1220-charger.html

You can wire a VGA connection to balance 12S. it will be taking up all the pins on the VGA so I only recommend charging at up to 3Amps, to not overload the pins.
13Pins for the Balance Leads and 2 Pins for the Charge leads.

However, a BMS will allow you to charger faster. and they are very slim to they fit great on most builds.
```

---

# How to test lipos?

### Replies: 7 Views: 177

## \#1 Posted by: Lucajo16 Posted at: 2018-11-28T13:21:23.239Z Reads: 77

```
Hay ive been riding for a few months and i use a 5s 4000mah turnigy battery. Now up until recently they charged to a full 21volts but now there just a few thousandth away from 21. Does that mean there dying? Should i try to charge again? How do i check with my charger? Also what do i look for in my charger to gauge there death?
```

---
## \#2 Posted by: telnoi Posted at: 2018-11-28T13:30:00.467Z Reads: 74

```
Internal resistance increases the older the Lipos get. You'd have to track IR from the very beginning for this to be of some use. Some chargers calculate IR, others don't and the value between different chargers can be vastly different, so no point in comparing these values with those others give you. IR as measured by chargers is inaccurate and should only be used to track deterioration. 

If the lipos are dying, it will no longer output the same amount of Ah. For example, my 8000 zippy went from 6000 till 3.7v to 4000 till 3.7v. Balancing also took considerably longer and a few cells will drop voltage 0.3v when charging is stopped. I'd consider these practically dead.
```

---
## \#3 Posted by: Lucajo16 Posted at: 2018-11-28T13:36:35.630Z Reads: 68

```
Ok. :frowning: i guess im not doing lipos anymore! XD i cant afford to spend 180 every 2 months to ride....now the question is how to kill the pack safely?
```

---
## \#4 Posted by: Jalapeno Posted at: 2018-11-28T14:24:53.293Z Reads: 62

```
@Lucajo16 what was the exact model?
How many Kms did they last you?
I'd say fully discharge them with a charger, and then use a lightbulb ( https://rogershobbycenter.com/lipoguide/ )
The salt water method seems okay-ish since the conductivity is relatively low and can be controlled both by the ammount of salt and the distance the battery leads are from one another. But then again lithium reacts with water https://youtu.be/Vxqe_ZOwsHs

@telnoi, same how many Kms before they dropped to 4000mAh?
```

---
## \#5 Posted by: marsrover001 Posted at: 2018-11-28T14:45:45.682Z Reads: 56

```
Lightbulb or wire wound resistor (heating coil from an old heater? It's winter, might as well use that energy)

When pack reads 0v, it's dead. Drop it in your nearest battery recycle bin.
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-11-28T14:48:32.858Z Reads: 56

```
Normally lipos will charge all the time to the top voltage if charger charges it to the top voltage but it will not hold that additional charge as "range" and drop after some time. In cold temperature internal resistance changes which can also influence voltage range and other parameters. There are so many factors which can affect IR in Li-Ion batteries :)
```

---
## \#7 Posted by: Hummie Posted at: 2018-11-28T20:09:09.760Z Reads: 30

```
using a charger and noticing only the slightest lower voltage at full charge being thousandths of a volt lower full the full pack could be almost anything or nothing. That’s an insignificant voltage difference and I’m guessing it would be slightly unbalanced cells causing it and the bms is catching up to the charger and draining the highest cell.  It’s not saying anything about the pack deteriorating with what he’s experiencing.

If u speed charge a battery the last bit won’t get in there and the pack voltage will drop further when off the supply compared to slow charge too
```

---

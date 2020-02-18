# My BMS kept being warm after unplugging the charger

### Replies: 13 Views: 229

## \#1 Posted by: filipandre95 Posted at: 2019-03-22T12:16:42.660Z Reads: 82

```
I got concerned when I found out that my BMS kept being warm after unplugging the charger and waiting for a while. So i unplugged the balancing leads and waited for it to cool down. When it was cold I plugged it back in and it didnt warm up. Is this normal ???
I have my BMS wierd up only for charging.
Does the BMS still balance even after its been unplugged?

I checked the pack with my Fluke multimeter:
4,19v 8,38v 12,57v 16,77v 20,96v 25,15v 29,34v 33,5v 37,7v 41,9v
```

---
## \#2 Posted by: filipandre95 Posted at: 2019-03-22T12:20:48.515Z Reads: 76

```
This is the BMS
https://www.banggood.com/37V-42V-10S-45A-Li-ion-Battery-Protection-Board-BMS-PCB-System-p-1177351.html?rmmds=search&cur_warehouse=CN
```

---
## \#3 Posted by: rojitor Posted at: 2019-03-22T14:03:34.022Z Reads: 67

```
How Hot? It is normal to be how while balancing. No need to be plugged.
```

---
## \#4 Posted by: threebysix Posted at: 2019-03-22T14:21:33.601Z Reads: 63

```
Those P packs' voltage values are all over the place, which is probably why the bms is super warm.

edit: My bad, I read it wrong.
```

---
## \#5 Posted by: filipandre95 Posted at: 2019-03-22T14:23:56.268Z Reads: 62

```
I know, but is it normal that its still hot 10 minutes after unplugging the charger even that I'm blowing on it with a fan. It only cooled down when I unplugged the balance cable.
```

---
## \#6 Posted by: taz Posted at: 2019-03-22T14:24:48.099Z Reads: 60

```
Why do you say that?
I am seeing 4.19-4.20V for every p-group.

Edit: There is one p-group with 4.16V
```

---
## \#7 Posted by: threebysix Posted at: 2019-03-22T14:28:41.192Z Reads: 54

```
Nvm, you were right. I read it wrong. My bad.
```

---
## \#8 Posted by: rojitor Posted at: 2019-03-22T15:00:54.057Z Reads: 52

```
Yes. It is normal. Balancing can take hours. Unless the bms goes above 40° celsius i wouldn't worry. You do the right thing noticing the heat. It could be troublesome. 
As soon as the pack is fully balanced your bms should remain cold after charging.
```

---
## \#9 Posted by: thisguyhere Posted at: 2019-03-22T16:43:37.928Z Reads: 42

```
bms temp during balancing:

![image|629x500](upload://tQoXFJfS3p8bH3HjA0B71DAxhyo.jpeg) 

250f or 121c, and this is normal.

this is why it's not good to place the bms directly on the battery.  but i digress.

bms should NOT remain hot when charge stops.

as a test, take P group voltages, jot it down.  then plug balance leads back on, connect to battery but DON'T charge it.  leave it for...hours, come back and take P group voltage readings again.  if there's a difference, you got a bms problem.

i've had bms that had slow drains on them.

failure rate is low, but not uncommon.
```

---
## \#10 Posted by: goldrabe Posted at: 2019-03-22T23:56:53.177Z Reads: 27

```
Is 121°C really a normal figure during charging? 
With how many amps did you charged to reach that temperature? 
I had my BMS placed on one P group and it killed the P group in the course of one year of frequent charging. However I checked the pack several times by hand and didn't noticed any heating during charging. My BMS was also wired for discharge and I noticed that the pack got hot twice in the area where the BMS was placed.
```

---
## \#11 Posted by: thisguyhere Posted at: 2019-03-23T03:19:54.206Z Reads: 22

```
it always get this hot, and it's using a 1.5a charger.

but the heat isn't coming from the charger.  the tiny resistors are draining an entire P group at like 250mAh.  so, a 4p group is 12Ah, being discharged at 250mAh with a tiny resistor - so that's working full time trying to drain a giant charge.

anyway, yea it gets hot.

with yours, maybe your pack is perfectly balanced so it doesn't kick into balance charge?  i mean, you said it's discharging too so it may be keeping it balanced at all times.  this is the potential issue with bypassing the bms.
```

---
## \#12 Posted by: goldrabe Posted at: 2019-03-23T03:31:14.790Z Reads: 21

```
Thanks! Now I understand better. I think my BMS just controls overcharge and under voltage, it shut down my pack because the P group came out of wack completely. But having the potential that something can heat up to 120°C in my enclosure makes me anxious. Could every BMS get that hot or are there better ones in this regard?
Now I know it's a good idea to check my packs and BMS's on the end of the discharge!
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-03-23T03:54:18.180Z Reads: 20

```
bms balance through bleeding charge with resistors - resistors convert energy into heat - so i think all bms' will get hot.

so yea, there's something that is way above boiling point hanging out inside the enclosure, kinda scary.
```

---

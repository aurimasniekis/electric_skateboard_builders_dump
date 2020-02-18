# Charge/Discharge vs charge only bms

### Replies: 9 Views: 248

## \#1 Posted by: JoelMatousek Posted at: 2019-08-04T02:46:43.517Z Reads: 48

```
This may have been answered somewhere else, but I can't find anything. I currently have a 10s4p 30q with a charge only bms. I have been worried about a pack discharging too far, so I only go to about 37/38 volts (I've only discharged it once and charged it twice) eventually I will discharge it more, but for now I'm just testing. Does a charge/discharge bms also balance the cells while discharging? Or does it just limit amp withdraw?
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-08-04T04:14:08.422Z Reads: 44

```
Assuming you're using a vesc or derivative thereof, it has settings to prevent overdischarge For a 10s battery you should be safe going as low as 30-33 volts.

Most BMS' (either charge only or both) only balance when charging - specifically when mostly charged - the first cell that hits, say, 4.2 volts will begin to be bled down by the internal resistors of the BMS until it matches the next cell. When those two hit 4.2, they are both bled down until they match more cells, and the cycle continues until all the cells have hit the same voltage, and the overall pack voltage has hit the 100% mark.

The main advantage of a two-way BMS is that it has authority to stop the cells from discharging if, for example, you leave your board on overnight (or for a week while you're out of town, etc) and the quiescent current draw of the electronics would otherwise drain your pack below what the vesc is set to stop at, or if the vesc fails and you end up with a short or other electrical drain that doesn't stop on its own.

There are some BMS models that will do bottom end balancing or whatever you want (I have one on my ebike project) but they're the exception rather than the rule.
```

---
## \#3 Posted by: JoelMatousek Posted at: 2019-08-04T04:17:32.795Z Reads: 41

```
So it's unlikely that any one of the individual cell packs will discharge below 3.0 while the rest are at like 3.3 or above?
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-08-04T04:24:37.612Z Reads: 40

```
Correct, **assuming** they are balanced and well matched in capacity first. (You should be fine since your pack is made of  - I assume - new 30Q cells.) Usually a pack made of new cells that's been balanced once will only drift between a couple and a dozen millivolts throughout the whole discharge.

If you're nervous you can always check the individual cell voltages with a multimeter while you're discharging them.
```

---
## \#5 Posted by: JoelMatousek Posted at: 2019-08-04T04:26:55.944Z Reads: 37

```
Also, considering it has a 12mah capacity. I doubt leaving it on over night will kill the battery, especially considering I don't plan on leaving it with a voltage below 3.3 for a long time because of that reason
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-08-04T04:27:31.459Z Reads: 34

```
True. I'm just listing hypotheticals.
```

---
## \#7 Posted by: JoelMatousek Posted at: 2019-08-04T04:29:50.632Z Reads: 31

```
They were all brand new with a voltage of 3.42 volts. Except one was at 3.41, but that shouldn't be an issue. I just wanted to double check. I've seen the horror stories of these packs blowing up, so I wanted to do my research and make sure that nothing will go wrong, and that I can get the most out of my battery pack. Thank you!
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-08-04T04:30:31.611Z Reads: 30

```
Glad to help.
```

---
## \#9 Posted by: JoelMatousek Posted at: 2019-08-04T04:30:54.365Z Reads: 30

```
My bad not 12mah, I meant 12Ah
```

---

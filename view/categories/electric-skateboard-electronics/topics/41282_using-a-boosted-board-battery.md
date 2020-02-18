# Using A Boosted Board Battery

### Replies: 5 Views: 1183

## \#1 Posted by: A-lone-tenno Posted at: 2017-12-17T20:55:23.288Z Reads: 165

```
making a new thread because i assume this could help other BB fanboys like myself. is it possible to take their battery system (with charging, a switch, etc.) and connect it to the vesc/vescs we use? for instance: 

https://i.ebayimg.com/images/g/oS8AAOSwjM5aLy72/s-l1600.jpg

I don see how it would connect (only the one cable) but hypothetically would it be possible? if so, could save a lot of people some trouble (some are selling them because of the new battery)

i couldn't find this topic so sorry if it exists already

Thanks!
```

---
## \#2 Posted by: MrHappy Posted at: 2017-12-17T21:00:56.126Z Reads: 163

```
Yeah, If you find the right pins, they're using a 12s1p.
```

---
## \#3 Posted by: BoostedBuilder Posted at: 2017-12-17T21:16:49.373Z Reads: 155

```
No, you won't be able to use it with a VESC. 

The stock BMS is connected to their ESC via that cable (most likely a CAN connection) so if you use it with a different ESC, the battery will give you an error signal (yellow or red light).

You can open the pack, salvage the cells and use a different BMS in that case (but most likely you won't be able to do that since it's around 3mm and not many 12s LiFePo4 BMS's are that small). 
<img src="/uploads/db1493/original/3X/2/1/21bc37588d5491a2e6b0405007a8d15248241510.JPG" width="375" height="500">

Or you could just use their case and fit 20 (18650) cells in there with any Li-ion BMS, comme ça:
<img src="/uploads/db1493/original/3X/7/2/7281af142e2f9e436d330681612fb68203d74b36.jpg" width="690" height="444">
```

---
## \#4 Posted by: A-lone-tenno Posted at: 2017-12-17T22:03:03.036Z Reads: 135

```
And I assume there's no way to buy their esc? 
Also they have double motors, don't they have 2 esc's?
```

---
## \#5 Posted by: Pantologist Posted at: 2017-12-17T22:33:06.645Z Reads: 120

```
They do not sell it. 

Basically a set of ESCs on one PCB.
```

---

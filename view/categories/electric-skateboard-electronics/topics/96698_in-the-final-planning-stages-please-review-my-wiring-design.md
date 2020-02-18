# In the final planning stages, please review my wiring design!

### Replies: 11 Views: 191

## \#1 Posted by: cubed Posted at: 2019-06-16T03:28:03.675Z Reads: 55

```
Wiring show below via simple photo-shopped file, sorry if its not clean looking this was the easiest way for me to visualize it.

Anyways to the design!

1) A123 26650 batteries in a 6s5p config. I am going to get this built by @psychotiller (if its approved) but I just want to make sure my understanding of how battery packs are wired is right.

2) DieBieMS - connections via molex and input power from batteries

3) Output to female xt60, then goes into a male xt60 to dual female xt60 output

4) FocBox male xt60 input

5) 10 inch wide hub motor; 24v input, 600W power

6) Another xt60 splitter (one for usb charging, the other output for future led lighting)

7) Step down converter to dual usb charging ports (input 8-22v, output to 5v)
 
8) Barrel connector

9) Boosted board charger (outputs 100-240v, 50-60hz) I figured it would work as boosted uses the same cells.

Any input is appreciated! My few concerns are if the pack can properly power the motor, I calculate it will output about 20V so I hope undervolting a 24V motor is okay. 


![esk8circuit|500x500](upload://6muTvvt26RC5VfF2bD2nfQczKrc.jpeg)
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-06-16T04:19:07.350Z Reads: 46

```
6s a123 is only 21.9v fully charged (3.65v per cell)

[quote="cubed, post:1, topic:96698"]
Boosted board charger (outputs 100-240v, 50-60hz) I figured it would work as boosted uses the same cells.
[/quote]

It will but if your bms does not cut off at 21.9v than your battery will overcharge and probably explode...

Boosted boards uses 12s A123 I believe which is 43.8v fully charged (charger voltage ends at 43.8v)
```

---
## \#3 Posted by: cubed Posted at: 2019-06-16T04:24:58.953Z Reads: 43

```
Thanks! Im using the DieBieMS and will probably throw in a fuse between the charging port and bms, do you think that would help?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-06-16T04:25:44.082Z Reads: 42

```
Fuse won't help with anything unless it's a short circuit...

Getting a proper charger is not expensive.

Just sayin if that diebiems is not configured properly or it it does not cut off charge than the boosted charger will charge your 21.9v pack to 43.8v which = 🧨🧨🎆
```

---
## \#5 Posted by: cubed Posted at: 2019-06-16T04:26:59.567Z Reads: 40

```
Gotcha, Ill look into one that matches the pack. I wasnt sure how to determine which one to buy.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-06-16T04:28:58.854Z Reads: 39

```
If @psychotiller is building you're pack I'm sure he can find you a proper charger.
```

---
## \#7 Posted by: cubed Posted at: 2019-06-16T04:29:38.365Z Reads: 40

```
Ya I will double check everything with him as well. One more thing, do you have experience in undervolting a motor?
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-06-16T04:30:45.132Z Reads: 39

```
Well you cant exactly undervolt a brushless motor 😂

Brushless dc motors can run at almost any voltage, it's just that if the voltage was super low it won't have enough torque.
```

---
## \#9 Posted by: cubed Posted at: 2019-06-16T04:32:17.231Z Reads: 37

```
:thinking: very true, Im just unsure if I will be supplying it with enough juice to even move me :sweat_smile:

Here's the motor in question

https://www.peipeiscooter.com/10inch-10-inch-10x6-00-5-5-wide-tyre-brushless-gearless-dc-wheel-hub-motor-balance-scooter-hub-motor-hally-motor-phub-188.html
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-06-16T04:32:50.233Z Reads: 36

```
Onewheel build?

I don't think 6s a123 is enough. It won't have enough torque that is.
```

---
## \#11 Posted by: cubed Posted at: 2019-06-16T04:35:40.251Z Reads: 35

```
Not really a onewheel build :sweat_smile: more of a three wheel build 

https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/7/f708bbcbce3e09599d3e0d78a89b1176d01ac10d.jpeg
```

---

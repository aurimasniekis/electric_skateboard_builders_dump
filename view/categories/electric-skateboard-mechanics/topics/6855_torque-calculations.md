# Torque calculations

### Replies: 9 Views: 5700

## \#1 Posted by: Bender Posted at: 2016-07-30T12:14:36.547Z Reads: 390

```
Does anyone know of a calculator, or easy way to calculate the torque increase/decrease for change in gear ratio

I'd like this to be for the esk8 community and be as simple as possible to understand (like the top speed calculators)

Obviously I can feel this when I change things on my board, but I think it would be helpful to a lot of people to calculate BEFORE ordering parts

There seems to be a few calculators for top speed, but I'm really interested in a balance between speed and torque (a lot of hills by me and I'm a big guy)

Factors that I think should be included:
Motor pulley teeth
Wheel pulley teeth
Motor kv
Wheel diameter 
Battery voltage 
Motor size?
Dual/single motor?
Am I missing anything?

Thanks!
```

---
## \#2 Posted by: Hillso Posted at: 2016-07-30T13:30:35.705Z Reads: 373

```
heh I just thought about this idea. maybe you need to know the wattage, if so max continuous amp limit (motor / battery / esc / bms... whatever)
```

---
## \#3 Posted by: devin Posted at: 2016-07-30T15:07:50.811Z Reads: 365

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#4 Posted by: devin Posted at: 2016-07-30T15:13:28.444Z Reads: 335

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: PB1 Posted at: 2016-07-30T16:18:32.538Z Reads: 329

```
Every motor has a torque constant,  Kt.   It tells you how much torque per amp it produces.  
It's related to the Kv.  Kt=1/Kv. 

Then you need to calculate how many amps go trough your motor.  Lots of discussion here already.  

I'm preparing a spread sheet for all of that already and can add torque.  

Regarding gearing you can use the same figures as for RPM.  

However in the end it's Watts that propel the rider.  Torque is mainly used when accelerating.
```

---
## \#31 Posted by: Bender Posted at: 2016-07-30T17:34:04.031Z Reads: 315

```
@torqueboards @jacobbloy @lowGuido @longhairedboy @psychotiller @cmatson Can a mod split this thread

I actually really like listening to @devin and @Hummie 
But this has derailed a bit
```

---
## \#59 Posted by: devin Posted at: 2016-07-30T22:08:06.798Z Reads: 318

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-31T12:59:03.832Z Reads: 270

```
52 posts were split to a new topic: [Hummie vs Devin (Volts conversion to amps)](/t/hummie-vs-devin-volts-conversion-to-amps/6910)
```

---
## \#60 Posted by: EnderWiggin Posted at: 2016-11-23T01:06:59.646Z Reads: 270

```
So I had the same question or a very similar one when I was designing my Mountain board so I have spent too much time making this spread sheet. Let me know what you think and if it helps with understand the torque speed relationships.

I still need to account for gear ratios for the graphs but this should help a lot. 

http://www.electric-skateboard.builders/t/google-spreadsheet-for-easy-and-fast-calculations/13337
```

---

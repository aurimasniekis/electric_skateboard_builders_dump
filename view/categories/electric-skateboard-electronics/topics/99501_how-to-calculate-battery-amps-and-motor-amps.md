# How to calculate Battery amps and Motor amps

### Replies: 4 Views: 294

## \#1 Posted by: Stan8 Posted at: 2019-07-31T22:02:07.370Z Reads: 85

```
Hello, recently after trying to understand how batteries work, I've been trying to find how to calculate the different Amps for my Electric Mountainboard. I will have a 12s4p in Sanyo NCR20700B 4250mAh - 15A max discharge with a 10A continuous charge. 

So with this formula, I was trying to calculate the Amps that my motors will pull on the battery: 
Volt * Amp = Watts 
Watts / Amp = Volt
and Watts / Volt = Amp

So I have a 12s4p: (12x3.6)(4x10) which makes it 1728 
But then if my motor pulls let's say 30 Volts I get a result of 57.6
Is there something wrong with this formula? Or have I done anything wrong?
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-07-31T22:16:31.663Z Reads: 78

```
@Stan8  Motors don't "pull" amps or volts. They're passive devices. The motor controller controls (Ha, it's in the name) the amount of power and thus current that goes to the motors. 

Your math about battery current is also wrong: Adding more cells in series (the 12s part of your pack) increases the *voltage*, but doesn't affect the amperage at all. Similarly, adding cells in parallel (the 4p part of your pack) increases the *current* your pack can produce, without increasing the voltage at all. 

Since you've got a 12s battery, that means the nominal voltage is  (12x3.6) = 43.2 volts.

Since it's a 4p, the output current is (15x4) = 60 amps.
```

---
## \#3 Posted by: Stan8 Posted at: 2019-07-31T22:27:06.837Z Reads: 73

```
Thank you :).
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-07-31T22:31:42.481Z Reads: 70

```
@Stan8  Basically you went wrong by mixing unrelated units - Charge current has no bearing on your maximum discharge current, so that has no place in the equation - should have used 15 instead of 10.
Voltage has no bearing either, so the 12 and the 3.6 are both irrelevant.

If you want watts, then it's the discharge times the cell voltage times the number of cells in series and parallel ((12x4)x3.6x15) = 2592 watts.

If you want total energy in the pack, then it's the capacity of each cell, times the voltage of each cell, times the number of cells in the pack. ((12x4)x4.25x3.6) = 734.4 watt-hours.

If you want capacity, then it's the cell capacity times the number in parallel. (4x4.25) = 17 amp-hours.

And hey, because math is commutative, once you've figured out a couple of these, you can figure the rest by combining them! - 734.4 watt-hours divided by 43.2 volts gives us our 17 amp-hours!
2592 watts divided by 43.2 volts gives us 60 amps!
```

---

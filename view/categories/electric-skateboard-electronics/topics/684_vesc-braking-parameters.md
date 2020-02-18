# VESC braking parameters

### Replies: 8 Views: 1320

## \#1 Posted by: tomtnt Posted at: 2015-12-08T22:01:37.619Z Reads: 182

```
I'm running CarVon Single Hub motor with VESC and 8s/8000mah lipos..  I've read you should only charge lipos at 1c or 2c max - that would mean 16A.  Does that mean I can only set braking current on the VESC to -16A?  the braking is really weak at 16A but I don't want to risk overcharging the lipos.
```

---
## \#2 Posted by: onloop Posted at: 2015-12-08T22:23:02.900Z Reads: 185

```
I suggest setting the brakes to what you consider a safe and practical level for your riding ability & body weight.

The max regen braking setting you define in the VESC is not a constant flow of current, it's the peak at which your regen current can reach. Normally this peak is sustained for only a fraction of a second, as you slow down the back current also weakens.

If you are on a *very-very-long* steep hill that takes an hour or more to descend and your brake is on maximum the entire time & your speed is still high during braking at you might damage the battery due to charging at too high a charge rate. But this is very unlikely to ever happen.
```

---
## \#3 Posted by: SirBo Posted at: 2017-09-29T14:56:34.010Z Reads: 89

```
Mmmmh, i'm curious about it. I run a setup with 5000 mAh. So my "Batt min (regen)" value should be around 5 Amps. Set it to 20 Amps to get a reasonable brake means be 4 times over....

Do you onloop, or anybody has experience if its fine for the batteries?

Regards!
```

---
## \#4 Posted by: florensvb Posted at: 2017-09-29T16:31:11.968Z Reads: 85

```
I charge at my 8000mah lipos at 2c. so my battery min (regen) is at 16ah. but theres also the settings for motor min which is essentially your brake power at low to mid level speeds. i am not an expert, not sure where the extra energy really goes, but it will never charge the batteries above 16ah. i think beyond that its just more heat in the motor and vesc because the energy needs to go somewhere. so try making the motor min to about the same as your motor max and watch your brake increase
```

---
## \#5 Posted by: SirBo Posted at: 2017-09-29T17:02:11.115Z Reads: 77

```
Yeah, my "motor min (regen)" is at about -60 A (Motor max is at 80A). But when i set Battery (min) to 10 Amps (what in my case would be 2c) then the brakes are muuuuuch to weak for me. At least i need 20 A for "battery min (regen)" for a reasonable brake power.  

I refer to the suggestion of onloop "setting the brakes to what you consider a safe and practical level for your riding ability & body weight." Wondering if his statement finds any confirmation by other builders or by an trustable source.

Or is it possible to kind of bypass the regeneration while braking completely? 

Regards!
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-09-29T17:45:42.702Z Reads: 68

```
You should be able to set the Regen current to zero. IIRC I have my battery min set to 5 amps per motor (dual) and the motor min set to 80, and the brakes are good enough to chuck me off if I'm not careful.
```

---
## \#7 Posted by: florensvb Posted at: 2017-09-30T01:15:24.735Z Reads: 63

```
does this generate a lot of heat or no problems?
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-09-30T01:18:22.803Z Reads: 59

```
my only problem is that when I have a nearly full battery and I go down a long hill, sometimes the vesc will reach its overvoltage cutoff and the brakes will fail for a second or two. It's a little unnerving.
```

---

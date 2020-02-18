# VESC brake settings plus hardware idea

### Replies: 6 Views: 738

## \#1 Posted by: craj1031tx Posted at: 2018-01-21T18:19:53.052Z Reads: 133

```
So I know that the batt min setting is the regen setting for recharging your batteries during braking, but what happens to all of the surplus energy that is captured if you're braking at a higher current than your regen setting is set to (braking at the 'motor min' setting, which most people usually set much higher than the batt min setting). Is this excess energy just stored/buffered into the capacitors before being trickled back into the batteries or used for future acceleration events?

If there is some sort of limit to this amount of energy (as in, you've 'filled up' the capacitors), does the VESC revert to a braking force that is equal to your batt min settings, as it has now where else to throw the extra energy?

I know this would require some sort of special hardware support, but for an imaginary future VESC, would it be feasible to dump (excess) braking energy into some sort of large resistor (think blow dryer or space heater heating element, which typically operate at around 1500 watts) and then just radiating that energy out as heat to the environment? I have a space heater sitting right next to me that has a 1500 watt coil that looks like it wouldn't even need to have a heatsink attached to it if were to be used for this purpose - as long as you could isolate it and mount it in a safe position, you should be able to throw 10 seconds of 1500 watt heat into it without it breaking a sweat.
```

---
## \#2 Posted by: krloz Posted at: 2018-01-21T19:30:14.966Z Reads: 119

```
[quote="craj1031tx, post:1, topic:44275"]
you’re braking at a higher current than your regen setting is set to
[/quote]

I dont think that's possible. The max you are going to brake is determined by the limits you set in min battery and motor
```

---
## \#3 Posted by: ugothakd Posted at: 2018-01-21T21:30:09.282Z Reads: 96

```
I read somewhere that what you're talking about is implemented in some commercial eboards. As for what happens when that energy has no where to go.. shutdown and loss of brakes I think
```

---
## \#4 Posted by: craj1031tx Posted at: 2018-01-21T22:24:27.502Z Reads: 81

```
Interesting, so what is the point of the motor min setting in bldc?
```

---
## \#5 Posted by: krloz Posted at: 2018-01-21T22:51:10.165Z Reads: 72

```
Motor min and battery min are related by the duty cycle. Just as in motor max and battery max.  At least in current control modes
```

---
## \#6 Posted by: Namasaki Posted at: 2018-01-25T02:23:46.836Z Reads: 42

```
http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---

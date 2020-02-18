# What does green led indicate on my vesc?

### Replies: 3 Views: 1095

## \#1 Posted by: Rions Posted at: 2017-02-04T10:57:10.304Z Reads: 106

```
I recently tried a different battery with my setup and vesc has blue and green lights on it.In bldc iv tried changing voltage to match new battery but doesn't seem to be liking the new settings as a red light continues to blink until i change back to previous config.Im getting no movement from control to motor.When i plug in original battery all is back working well.New battery is a lithium 21.6vdc/8.8ah/190.08wh.Is it suitable ?any suggestions please ?
```

---
## \#2 Posted by: flatsp0t Posted at: 2017-02-04T11:05:34.382Z Reads: 106

```
What settings did you change exactly?
If it was MAX_INPUT_Voltage and MIN_INPUT_Voltage, dont change them, they should stay at stock settings.
see http://www.electric-skateboard.builders/t/vesc-faq-limit-output-voltage-according-to-motor-maximum-specs/683/11?u=flatsp0t for reference
```

---
## \#3 Posted by: Rions Posted at: 2017-02-04T23:33:49.277Z Reads: 78

```
Yes i was aiming to try changing from 57v but as i mentioned it just kept blinking red.i previously had 10s space cell battery on it so am unsure if this new battery is ok to use.Do you know what green indicates -i was looking for a voltage fault but doesnt seem to read one in realtime.I can see it is picking up batt volt at 25.2v but thats it.i dont really want to fiddle around too much these vescs are easily fried
```

---

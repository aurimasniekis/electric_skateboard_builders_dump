# How to test motors&hellip;?

### Replies: 3 Views: 294

## \#1 Posted by: kchxaz Posted at: 2019-01-27T21:49:44.652Z Reads: 84

```
Hi All,

Wondering if there is a way to test motors for functionality? I received several used motors from a friend (he works at an R/C shop) but he is unsure as to the working condition of them. The motors do not have the typical blue/green/yellow wires protruding from the motors so my question is do the color of the wires actually matter? I could guess that maybe the colors indicate which is forward vs reverse but I don't know, which is why I thought I's ask the forum...? Oh, the motors have the small gauge hall sensor wires too, if that matters...Any ideas how to test these three wired motors to see if they work properly?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-27T21:55:50.040Z Reads: 80

```
The order of your phase wires matter as depending on the order the motor will turn forwards or backwards.
You can just swap 2 phase wires or set the invert signal in the vesc tool in case your motor spins in the wrong direction.
To check if you don’t have shorted phase wires you can use this method 
https://www.electric-skateboard.builders/t/not-sure-if-you-have-shorted-phase-wires-here-is-how-to-test-them-without-frying-your-esc/78693?u=andy87
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-01-27T22:19:36.243Z Reads: 61

```
Measure the resistance between each of the phases, and from each phase to the case. The resistance between all the phases should be equal, and there should be no connection between the phases and the case. If that all checks out, then you can also do the drill test as shown above. If you have equal resistances and equal voltages, then you have a good, happy motor.

If you have a way to measure the RPM of the motor accurately while preforming the drill test, then you can also determine the KV of the motor. If the KV is significantly higher than it should be according to the label, then the magnets may be damaged by heat - weaker magnets increase the motor's KV. (BLDC tool/vesc tool also has a KV measurement option in there somewhere IIRC, you can check that as well.)
```

---

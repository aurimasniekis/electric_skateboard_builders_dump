# VESC &#124; What kind of control is BLDC?

### Replies: 2 Views: 727

## \#1 Posted by: chibby Posted at: 2016-03-29T08:37:08.584Z Reads: 52

```
I am trying to figure out the difference in control between BLDC or FOC on the VESC. FOC is obviously field-oriented control, however is BLDC some sort of scalar control?
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-29T11:06:08.687Z Reads: 45

```
Trapezoidal commutation, in sensorless mode I think the rotor position is estimated by sensing the zero crossing of back EMF.
Here's an interesting video of the technique:
http://youtu.be/szgVUfyX8JM
```

---

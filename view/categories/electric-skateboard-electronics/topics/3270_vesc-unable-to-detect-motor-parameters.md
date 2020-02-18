# VESC &#124; Unable to detect motor parameters

### Replies: 2 Views: 1023

## \#1 Posted by: chibby Posted at: 2016-05-14T16:54:17.771Z Reads: 109

```
I have trouble running the motor detection in BLDC-tool. I am getting "Bad motor detection". I am able to spin the motor with the arrow keys and it gives noise when trying to detect. 

In BLDC-mode it's not spinning up, barely steps, resulting in bad motor detection. In FOC-mode I detect a very high resistance (7 ohm), but the inductance seems alright (11 uH). However it fails to detect any flux linkage.

Reflashed the VESC, with both new and older firmware. Running from a labsupply (30 V with 10 A), all pins are disconnected. Tried with two different motors. 

Anyone with an idea of what could be causing this or how I should proceed in my troubleshooting?
```

---
## \#2 Posted by: laurnts Posted at: 2016-05-14T20:26:44.531Z Reads: 96

```
It could be that lab power supply were not good enough (mine didnt work well VESC + PSU). Try with lipo / battery also fine.
```

---

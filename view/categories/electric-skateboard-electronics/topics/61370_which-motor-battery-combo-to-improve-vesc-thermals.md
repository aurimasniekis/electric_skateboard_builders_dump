# Which motor/battery combo to improve VESC Thermals?

### Replies: 3 Views: 191

## \#1 Posted by: TheFluffiest Posted at: 2018-07-09T18:39:13.119Z Reads: 53

```
Currently, I have two configuration options for a single drive board. Right now, it is a KEDA 6364 190kv motor running on  three 4s 20~30c 5000mah batteries to make 12s. I am having a problem where the torque cuts out significantly within a mile of riding, and stays that way until I stop for a bit. After doing some research, I believe this is due to the VESC overheating, and I have ordered heatsinks to help with that.

The other option is a TB 6355 260kv motor sensored. I would run it off four of the same 4s batteries to make it 8s2p. I am thinking about changing over because the KEDA is pretty beat up, and both options are easily available to me. Plus I am sure sensored would be nice. I assume the 8s2p setup would allow for more range, less voltage sag, and less possibility of the VESC overheating because less watts would be pulled.

Thoughts anyone?
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-09T19:10:31.791Z Reads: 46

```
Find a way to cool your vesc better.  Going 8s is only going to increase amps required to get you going especially with 260kv motor.  More amps, more heat. What's your current settings on your vesc and what kind of it?
```

---
## \#3 Posted by: TheFluffiest Posted at: 2018-07-09T19:27:48.099Z Reads: 42

```
Off the top of my head, I think its 55a motor max and 80a battery max. I thought it was wattage that made it hotter? Less volts, same amps means less watts? It's a 4.12 vesc.

I could also rewind the motor in a delta configuration to reduce kv in the other motor...
```

---

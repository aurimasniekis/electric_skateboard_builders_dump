# Is there anyway to check a BMS voltage before plugging my batteries in?

### Replies: 4 Views: 99

## \#1 Posted by: CrimzonGryphon Posted at: 2019-08-11T11:56:08.149Z Reads: 28

```
If you plug a BMS into a battery that it's not rated for you're going to kill that battery.

Is there anyway of checking the BMS balance voltages before plugging it into a battery?
```

---
## \#2 Posted by: butt_stallion Posted at: 2019-08-11T13:22:55.231Z Reads: 25

```
If you have the balance wires soldered you can use the voltage meter probes and stick them into the pins of the balance connector.  So keep the ground on the ground pin of the connector and then you can put the positive on each pin and you should see the voltage.
```

---
## \#3 Posted by: CrimzonGryphon Posted at: 2019-08-11T14:47:17.500Z Reads: 20

```
Wouldn't this just be checking the voltage of the battery? Maybe I'm misintepretting you.
```

---
## \#4 Posted by: wafflejock Posted at: 2019-08-11T16:02:22.261Z Reads: 18

```
I guess the question is why would you use a BMS for batteries or voltages it isn't designed for, if you can't trust the spec sheet you probably just shouldn't be use the BMS.  No easy way I know to simulate the battery "load" here since the BMS will probably expect cells to be at least 2.5 or 3.0V before attempting to charge.
```

---

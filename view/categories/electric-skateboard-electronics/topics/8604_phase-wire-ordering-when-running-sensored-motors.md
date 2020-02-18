# Phase wire ordering when running sensored motors

### Replies: 6 Views: 934

## \#1 Posted by: dinodave Posted at: 2016-08-29T21:26:17.728Z Reads: 136

```
I'm using @chaka's 170kv sensored motors, and Enertion VESCs, and thought I would attempt to use the hall sensors given I would like nice smooth operation at low speeds.

So I have a question, I assume the order of the sensor wires connecting to the VESC is important, I found this post where @Jinra showed how to connect them, and am doing something very similar. http://www.electric-skateboard.builders/t/ollinboardco-om5065-200kv-sensored-motor/3409/397?u=dinodave

But is the ordering of the 3 phase wires connecting to the VESC also important? And if so, what's the order? The Ollin motors come with phase wires colored red, yellow, and black.

Thanks!
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-29T21:29:06.883Z Reads: 134

```
+5v and GND cables (red and black) are important, but the 3 sensor wires doesn't matter as long as you do detection and set it correct on the sensor table on BLDC tool.
```

---
## \#3 Posted by: dinodave Posted at: 2016-08-29T21:31:04.018Z Reads: 130

```
Thanks, but perhaps I'm using the wrong terminology, I meant the 3 wires that carry the voltage and drive the motor, is their order important?
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-29T21:32:29.379Z Reads: 123

```
gotcha, those are typically called phase wires. Just make sure they're spinning the right way, order doesn't matter. There will be 3 combinations that will make it spin 1 way and 3 that will make it spin the other way. As long as the hall sensor table is correct, you'll have no problems.
```

---
## \#5 Posted by: dinodave Posted at: 2016-08-29T21:37:35.252Z Reads: 115

```
Awesome, many thanks! Hoping to get this all wired up and configured today... fingers crossed.
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-29T21:38:18.197Z Reads: 111

```
if you throttle and it looks like the motor is cogging, do NOT put more throttle/current to it, or you can blow something.
```

---

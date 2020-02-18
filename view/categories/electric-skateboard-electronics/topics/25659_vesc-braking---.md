# Vesc braking___

### Replies: 11 Views: 409

## \#1 Posted by: Vampiresquid64 Posted at: 2017-06-19T05:19:50.472Z Reads: 101

```
so how long can I brake without damaging my vesc? is it possible to use the battery to brake on long hills after the capacitors of the vesc are full? I'm a vesc nube so if I said something wrong please correct me.
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-19T05:28:07.244Z Reads: 100

```
There's no issue with braking unless you exceed max voltage (default 57v) from the generated BEMF.
```

---
## \#3 Posted by: Vampiresquid64 Posted at: 2017-06-19T05:30:02.744Z Reads: 100

```
oh ok. I heard a rumor somewhere that once the capacitors were full the brakes stopped working.
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-19T05:32:57.584Z Reads: 98

```
capacitors fill up and discharge extremely quick, that's what they're meant for. You probably heard that once the battery is full it can brake. I haven't experienced this myself, and have only heard it in limited occasions. I have a feeling it may be another factor (such as overvoltage) that's causing the issue.
```

---
## \#5 Posted by: Vampiresquid64 Posted at: 2017-06-19T05:33:27.997Z Reads: 90

```
ok good to know
```

---
## \#6 Posted by: gee Posted at: 2017-06-19T06:26:41.787Z Reads: 81

```
you're saying that if i have maximum voltage in the battery and I go downhill, it charges my battery and as a result it will over charge it and therefore overvoltage and possibly affect the vesc.
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-19T06:28:06.667Z Reads: 81

```
depends on your battery, though most likely you'll just damage the battery. You'll likely never overvolt the VESC if you leave the default max voltage value alone.
```

---
## \#8 Posted by: gee Posted at: 2017-06-19T06:52:04.702Z Reads: 75

```
so I shouldn't charge the battery 100%? I don't have the usb 2.0 cable so I can't configure the vesc yet.
```

---
## \#9 Posted by: Jinra Posted at: 2017-06-19T06:54:48.985Z Reads: 78

```
You should be fine in 99% of scenarios. One in which you might have issues is if you're charged 100% and immediately bomb a downhill going faster than your top speed and brake, causing you to potentially overcharge your batteries and damage them.
```

---
## \#10 Posted by: Vieo Posted at: 2017-06-19T11:24:08.889Z Reads: 50

```
In theory. Is there a way around this issue? Would there be a way to disperse the power generated via going down hill when the batteries are 100%
```

---
## \#11 Posted by: Alanhunt123 Posted at: 2017-06-19T12:47:55.961Z Reads: 40

```
The best way I've found to avoid this issue is to either run the board for a minute before going downhill (the voltage quickly drops at the start of discharge), or to only charge up to 4.1v per cell, which doesn't actually reduce the range by much on larger packs, and extends the cycle life of the battery.
```

---

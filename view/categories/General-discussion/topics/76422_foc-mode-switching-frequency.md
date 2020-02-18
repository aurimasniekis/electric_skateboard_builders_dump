# FOC mode switching frequency?

### Replies: 6 Views: 142

## \#1 Posted by: Jmding Posted at: 2018-11-28T21:43:23.740Z Reads: 61

```
Anyone know roughly what the switching frequency for FOC mode is?

In BLDC its just motor_phases * voltage * Kv since the MOSFETs only switch once per phase

In FOC, I imagine its MUCH higher, something like 4-5 switches per phase? Anyone know?
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-11-28T21:53:17.040Z Reads: 61

```
You can set it in Vesc tool
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-11-28T21:54:01.265Z Reads: 59

```
AFAIK bldc is also switching through each phase.

It has to modulate each phase using something PWM-esque to vary the voltage. That's how you get variable drive speed.
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-11-28T21:54:32.663Z Reads: 57

```
FOC maybe?

[quote="TowerCrisis, post:3, topic:76422"]
AFAIK bldc is also switching through each phase.
[/quote]
```

---
## \#5 Posted by: TowerCrisis Posted at: 2018-11-28T21:56:18.197Z Reads: 52

```
No, BLDC is most certainly modulating each phase to limit voltage.

FOC is switching much more frequently to output a smooth sine wave. (I'm not an expert)

EDIT: see @Pedrodemio 's explanation for something that makes more sense.
```

---
## \#6 Posted by: Pedrodemio Posted at: 2018-11-28T21:59:16.830Z Reads: 45

```
In BLDC the switching frequency is variable and as you said depends in RPM

In FOC is a fixed number, the defaults is 20 kHz, but some motors are pretty noisy at that value, you can up that to 30 kHz and be truly silent

The fixed frequency is due it using PWM to form a sinewave
```

---

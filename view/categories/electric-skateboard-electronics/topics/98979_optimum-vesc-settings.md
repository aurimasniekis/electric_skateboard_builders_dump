# Optimum Vesc settings?

### Replies: 2 Views: 131

## \#1 Posted by: DaFunkyMonkey Posted at: 2019-07-23T16:27:01.043Z Reads: 41

```
Looking for anyone's advice on Vesc settings for my build. I am running two Racestar 5065 200kv motors (max current: 46A), two flipsky vescs (4.12, 50A continuous / 240A peak), a 10s3P battery and an Evolve AT kit.

Here is what I got so far:

Settings (per vesc)
Motor Max: 30A
Motor Min: -12A
Battery Max: 30A
Battery Min:-10A

Unfortunately I do not know what amps my battery can supply as i got it free second hand with no info. All I know is that it's 10s3p. It looks old so most likely not 30Q.

Just looking for some advice to get me started without frying my Vesc/battery.
```

---
## \#2 Posted by: DaFunkyMonkey Posted at: 2019-08-19T22:05:55.044Z Reads: 20

```
Removing the shrink wrap revealed the cells to be:

* BFN ICR18650 2000 2000mAh 3.7V
MH60385 17F19

Which have the following specs:

* Standard Charge: CC/CV,0.2C5A,4.20V
Standard Discharge: CC,0.2C5A, 3.00V
Quick Charge Current: 2000mAh @1.0C
Quick Discharge Current: 4000mAh@2.0C
Max Discharge Current: 10000mAh@5.0C

To summaries what information i have gathered from the forums so far:

* **Motor Max**  (Motor Current Max): Set to 30A
This is the MAX amps you want inside your motor (i.e. it controls low end acceleration).
This setting needs to be below the max current of the motors (i.e. 46A).
It also needs to take into consideration the limit of the VESC (i.e. 50A).
With my 4.12 HW VESC (with no heat sink), I should set motor max between 30 and 40A.
Hence I should start with a low setting of 30A, and depending on how the acceleration is I can later increase it up to 40A, and if I am feeling really adventurous I could even set it as high as 60a or 80A.
* **Motor Min**  (Motor Current Max Brake): Set to -20A
This is the max amps I want inside the motor during braking (i.e. it controls break force at mid to low speeds).
This setting should be approx. 10A below motor max.
* **Battery Max**  (Battery Current Max): Set to 15A
This is the max current draw from the battery.
This setting is based on the limit of the battery, however for VESC HW 4.12, this setting should be no more than 35A regardless of the battery type.
Also, motor amps should always be greater than battery amps.
For my battery cells, the ‘max constant current’ is 10A.
10A x 3P = 30A. For a dual setup 30A / 2 = 15A.
* **Battery Min**  (Battery Current Max Regen): Set to -9A
This is the max regen-charging current I want to flow into the battery whilst braking (i.e. controls break force at high speeds).
This setting is based on the limit of the battery.
For my battery cells, the ‘Quick charge current’ is 2Ah.
2Ah x 3P = -6. For Duel setup -6/2 = -3A.
However, at this setting the “Battery Current Max Regen” will limit the brake power at nearly all speeds because it is too low.
Max charge current ratings are only for continuous charge and not for short bursts, which take mostly not longer than 5 seconds.
Therefore it can be set to 20% of Motor Max setpoint which is -6A, plus a 10% buffer = -9A.

Please could someone help me and confirm if the settings above makes sense, in particular the motor min. setpoint as I am not sure if this parameter is also limited by the battery?
```

---

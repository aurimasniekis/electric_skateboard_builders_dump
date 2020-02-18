# Wattage of motor calulated via battery volt x battery amp or battery volt x motor amp?

### Replies: 9 Views: 562

## \#1 Posted by: Brad Posted at: 2018-04-20T14:24:52.464Z Reads: 145

```
Hello

Wattage is volts times amp would be the obvious calculation.

I'm aware that motor amp is higher than battery amp due to the stator in the can spinning which is why battery amp is set lower than motor amp in the VESC.

Is the actual wattage for torque calculated off battery voltage and battery amp or off battery voltage and motor amp?

I also assume that amp rating limit for motors set by factories is based off total motor amp instead of just amps being drawn into the motor from the battery?
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-04-20T14:29:13.990Z Reads: 142

```
[quote="Brad, post:1, topic:52903"]
battery voltage and battery amp
[/quote]

:kissing_heart:
```

---
## \#3 Posted by: professor_shartsis Posted at: 2018-04-20T14:29:18.841Z Reads: 139

```
Battery current * pack voltage = electrical wattage

((pack voltage * duty cycle %) - back emf voltage) / winding resistance = motor current

motor current * (pack voltage * duty cycle %) = electrical wattage
```

---
## \#4 Posted by: Brad Posted at: 2018-04-20T14:30:22.222Z Reads: 133

```
Thanks for clearing that up for me.

Nice, easy for me to put that equation into my spread sheet :brain:
```

---
## \#5 Posted by: Chewie Posted at: 2018-04-20T21:17:13.970Z Reads: 113

```
Batter volts times Motor amps, it's all marketing and marketing is about having the biggest number you can come up with in this case.
```

---
## \#6 Posted by: Brad Posted at: 2018-04-21T01:10:47.917Z Reads: 104

```
Well you stated "Battery current * pack voltage = electrical wattage" and then stated "motor current * (pack voltage * duty cycle %) = electrical wattage", so when talking about wattage for motor torque, which one of the two is it? 

I understand what duty cycle is, but at 100% or near there times the higher motor amp would give a different answer.

Also Chewie says battery volts times motor amps (unless it was just a simple mistake and he meant battery amps). 

See why I have to ask in an attempt to understand where the wattage for motor torque is as the calculation would give different answers.:thinking:
```

---
## \#7 Posted by: Namasaki Posted at: 2018-04-21T02:42:55.878Z Reads: 93

```
P=IE
Power = current x voltage
Ohm's Law
```

---
## \#8 Posted by: professor_shartsis Posted at: 2018-04-21T03:24:06.944Z Reads: 85

```
[quote="Brad, post:6, topic:52903"]
Also Chewie says battery volts times motor amps (unless it was just a simple mistake and he meant battery amps).
[/quote]


only when the duty cycle is %100 can you use either battery or motor amps * pack volts because the motor amps and battery amps will be the same at 100% duty. also at 100% duty cycle, the effective voltage of the controller is the same as the battery pack voltage. (but the max duty cycle of a vesc is 95%...)

when the duty cycle is anything less than 100%, than the correct answer is battery amps * battery volts = electrical watts (not motor amps * pack volts for electrical watts unless 100% duty)

[quote="Brad, post:6, topic:52903"]
when talking about wattage for motor torque, which one of the two is it?
[/quote]

motor torque is directly proportional to motor current.

KT * motor current = torque in newton meters

KT = 60 / (2 * pi * kv) = torque in newton meters per motor amp
```

---
## \#9 Posted by: Chewie Posted at: 2018-04-23T16:44:27.050Z Reads: 62

```
Like I said, any wattage rating listed is marketing propaganda.  They're going to take the largest number they can come up with, which in this case will be motor amps, times volts, and not worry about duty cycle in the least.

I may have a very low opinion of marketing ;)
```

---

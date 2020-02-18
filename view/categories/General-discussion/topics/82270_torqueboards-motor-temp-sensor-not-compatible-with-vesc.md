# Torqueboards motor temp sensor not compatible with VESC?

### Replies: 6 Views: 427

## \#1 Posted by: Pedrodemio Posted at: 2019-01-27T15:57:57.688Z Reads: 88

```
Anyone run into this issue? I was measuring it to determine the beta factor and realized that the NTC sensor is connected between V+ and Temp, and the VESC requires it to be between GND and temp

I really wanted to avoid having to open it and put a new sensor, but sens like there is no other way

@torqueboards 

![image|612x500](upload://dkSUSmSLC70Tjcj33Hk80fSIm9g.jpeg)
```

---
## \#2 Posted by: FullMetal_Machinist Posted at: 2019-01-29T16:05:49.311Z Reads: 52

```
Checked the 4.12 schematics on my end and sensor needs to be connected to GND inside the motor. If it is connected to +3.3v or +5v it will not work. Sensor type is NTC 10kohm.
Torqueboards list their motors as compatibile with vesc on theor website - you certain that sensor is connected to positive supply (pin 1 of connector)? It should be between pins 2 and 6 of 6-pin connector. You can check it easily with multimeter set to 20kohm range. Pay attention which pin is number 1 - it should be marked with small triangle or number 1 on connector. Hope i could help.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2019-01-29T16:18:35.854Z Reads: 51

```
Yeah, checked and is connected to the 5v, looking forward to what Dexter will say the reason is

And it's not that the overall polarity  is wrong since since the hall sensors are working

In the end I've added my own NTC and also took the opportunity to measure the beta factor for it, better to put only the sensor in the oven than the entire motor

![IMG_7112|666x500](upload://yPjEojY7fUptjy3epY3VvyuE0cu.jpeg)
```

---
## \#4 Posted by: Tijmen Posted at: 2019-06-25T21:12:16.170Z Reads: 31

```
Can you explain how you added a temperature sensor yourself and how it's wired? I'd also like temp data from my torque motors
```

---
## \#5 Posted by: Pedrodemio Posted at: 2019-06-25T21:18:33.567Z Reads: 30

```
Sure

First you have to buy a NTC thermistor, should be found in any electronic components store or online

On your motor sensor PCB you have to find the black wire, solder on leg of the sensor to it, the other leg you have to solder a new wire to it and connect on the place of the original white wire
```

---
## \#6 Posted by: mishrasubhransu Posted at: 2019-06-26T08:07:12.030Z Reads: 23

```
buy a 10K NTC thermistor.
```

---

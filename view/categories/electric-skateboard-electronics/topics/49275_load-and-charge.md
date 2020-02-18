# Load and charge

### Replies: 15 Views: 698

## \#1 Posted by: saybot Posted at: 2018-03-16T11:55:55.241Z Reads: 163

```
Hi, i building some devices and need advice. Ive got this 7s bms
![image|281x499](upload://wbeX6NFXXp7JH303j2I7xdDG8lO.jpg)



 can i charge and discharge from the same wires? Negative from bridged c- and p-, positive from battery so i the end Ive got one socket for charge/discharge?
```

---
## \#2 Posted by: Ishayc Posted at: 2018-03-16T12:50:41.947Z Reads: 137

```
Battery minus goes to B-, C- from BMS goes to charger plug minus and P- goes to ESC minus.
```

---
## \#3 Posted by: Deckoz Posted at: 2018-03-16T12:55:30.103Z Reads: 135

```
That little box called charge

Is the charge plug... The negative end goes to BMS. The positive goes to the battery positive

The box called load is your ESC. The positive of your vesc goes to the battery positive. The negative to -p of BMS


The little boxes make it look confusion...
```

---
## \#4 Posted by: saybot Posted at: 2018-03-16T13:09:39.594Z Reads: 114

```
yes i understand, all the bms i connected like you says, but now i have different situation and would like to make one socket for load and discharging like on this pic below. Can i make it like this?
![Untitled|690x475](upload://5bcrJr87C588oLmg6kBqR0PZLGG.png)

When i want to charge i plug XT to charger, when i wan to load ill disconnected from charger and connect to the motor.
Its nor for electric longboard i building battery for another purposes.
```

---
## \#5 Posted by: Acido Posted at: 2018-03-16T18:06:21.749Z Reads: 83

```
Are you sure that this bms can be used for eskate and discharge?
```

---
## \#6 Posted by: saybot Posted at: 2018-03-16T18:48:40.685Z Reads: 72

```
My question from the begining is about if i can make it like this. I dont know,just asking
```

---
## \#7 Posted by: Acido Posted at: 2018-03-16T18:55:11.668Z Reads: 72

```
check the specs of it
see how many amps it can discharge
```

---
## \#8 Posted by: pat.speed Posted at: 2018-03-16T21:47:20.098Z Reads: 54

```
Check the back side of the pcb, if there is a trace that connects both conection pads together I would say you can do what your asking. If not I would not attempt to do it
```

---
## \#9 Posted by: saybot Posted at: 2018-03-17T00:16:03.175Z Reads: 47

```
Hard to say.
![image|375x500](upload://gzaQEq8cRmkZEWdqzMAstsKUxhy.jpeg)
```

---
## \#10 Posted by: Namasaki Posted at: 2018-03-17T19:54:13.485Z Reads: 37

```
Is your load going to draw less current than what that bms is rated for?
```

---
## \#11 Posted by: saybot Posted at: 2018-03-17T20:47:26.700Z Reads: 36

```
Yes. Bms got max 35A continous but i will use 30A motor and before motor 30a fuse
```

---
## \#12 Posted by: Namasaki Posted at: 2018-03-17T20:52:49.683Z Reads: 33

```
The motor max can be higher than 30a.
It's the Batt max that limits the battery current.
You could set the motor max at 60a and the batt max at 30a but I would not put a 30a fuse inline.
The reason is that the bms will handle current spikes higher than 30a but the fuse will blow and you will either be thrown off the board when it suddenly looses power while your accelerating or will find yourself going fast with no brakes.

The bms will provide short protection so there is really no need for a fuse anyway.

As for connecting the P- and C- in parallel.
I'm using Bestech bms's and both C- and P- show full battery voltage when the bms is on so it appears that they are already in parallel.
Also charging through the P- pad with Regen braking doesn't cause any issues so I don't see why you shouldn't be able to do what your wanting to do.
Still, whatever you do that is different from the standard wiring, you do at your own risk.
```

---
## \#13 Posted by: saybot Posted at: 2018-03-17T21:06:01.901Z Reads: 31

```
We loose the subject. My question was if i can bridge p- i c- in this bms. Battery with bms is for another purpose not for eboard.
```

---
## \#14 Posted by: Namasaki Posted at: 2018-03-17T21:06:46.051Z Reads: 31

```
Please read the rest of my edited reply
```

---
## \#15 Posted by: saybot Posted at: 2018-03-17T21:23:16.691Z Reads: 27

```
I buildng Underwater scooter battery for a diver. So no need of regen etc. I just asking if i can work with just one socket for 2 purposes load/charge. But ok i will make like it should be so i put 3pin out
```

---

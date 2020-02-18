# 12s2p LIPO BMS worth it?

### Replies: 12 Views: 608

## \#1 Posted by: notepad Posted at: 2018-06-29T18:04:13.400Z Reads: 135

```
Finally getting around to doing the electronics for my 34" ( I know its kinda short) MountainBoard.

MultiKv - 192 & 168.
Vesc v6 and Focbox repectively.
12s2p Turnigy Graphine 8000mah 
2.4 Ghz dual receiver for redundency.

But I am at a crossroads with the batteries.   Which battery setup should I use, and is it worth adding a bms for loverly one point charging?

I beleive I can run the vescs in series, if so that means a 12s2p is possible.   But if not I could always go with a 12s1p x2. one for each vesc.

Incase the first one is used how would I wire up the 12s BMS.  I understand that the cells in series would auto balance, so would I use the back, or the front balance wires on the Lipo for the BMS in this case.
OR
If I have to go with two, 12s1p loops and I would want a BMS(s), is there any way to get a single charging port to charge both loops, or would I have to have two ports and charge both independently?


I do appologise if these are pretty newbie questions, what can I say, its my first time making a dual vesc setup.
anyway, thanks for reading!
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-06-29T18:08:23.432Z Reads: 126

```
12s2p is not going to be fun. you will run out of juice quick. go for a 4p and use bms. you can use a bestech unit w/ built in antispark. and it wasnt that bad on build. definitly read as much as you can and look @ the pics of other builds
```

---
## \#3 Posted by: wafflejock Posted at: 2018-06-29T18:09:18.226Z Reads: 123

```
Each VESC needs the same voltage so you'd be wiring them off the battery bank in parallel so they each get the same voltage.  Basically doesn't make sense to treat them separately you don't want one to run out while the other still has charge and if they are in parallel then effectively the VESCs aren't affecting each other aside from the strain they put on the batteries when drawing amps/power.
```

---
## \#4 Posted by: notepad Posted at: 2018-06-29T18:21:50.083Z Reads: 118

```
How come im not going to get much range.  My curent setup is 12s1p. it is 16,000Ah with a single vesc, but I get about 50km per charge. so wouldnt with having two vescs just give me 25Km at double the performance?
```

---
## \#5 Posted by: wafflejock Posted at: 2018-06-29T18:25:34.886Z Reads: 112

```
Typically when people are doing parallel it's assumed you are using 18650s if you don't say otherwise so was probably thinking 2.5-3Ah per cell.  Regarding splitting power if you are using the same power through two motors you should get roughly the same range you're just adding to torque basically the top speed will stay the same you've only lost in extra friction in the shaft/motor bearings.
```

---
## \#6 Posted by: notepad Posted at: 2018-06-29T18:31:25.564Z Reads: 103

```
That good to know then, Was getting confused with if having them in parallel would mean having 22v instead of 44v for each vesc. so was just tring to get my head around if I would actually loose performance. But alteast if the torque goes up the acceleration is more.
And if the range is the same, it means I still have a 50Km pack, which is nice
```

---
## \#7 Posted by: wafflejock Posted at: 2018-06-29T18:44:28.068Z Reads: 97

```
Yup if you are actually using more power (accelerating harder or climbing hills faster) then you will bleed off more power but in general if you were putting 800W into one motor and you're now putting 400W into two motors at a given speed/grade then the same energy is consumed in the same time.

Needing to deliver less current to each motor is good too since loss is computed with a square of the amperage times the resistance so anything you can do to reduce amperage helps significantly.  Example 10A at 40V is 400W of power, say we split this between two motors now it's 5A at 40V per motor (still 400W total, 200W each), the loss in the first case is 10^2 * R or 100R, for the second case it's 2 * (5^2 * R) or 50R where R is the fixed resistance of the load.

Anyone feel free to correct me if I went wrong somewhere there but believe this all to be the case.
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2018-06-29T18:54:31.402Z Reads: 94

```
Also voltage sag can be unsettling when trying to mob especially with dual motor. It can be scary. I had issues on both my 12s2p. How much u weigh brah
```

---
## \#9 Posted by: notepad Posted at: 2018-06-29T21:05:19.438Z Reads: 86

```
Luckily only 65Kg ish. so on the light side.
```

---
## \#10 Posted by: notepad Posted at: 2018-06-29T21:08:50.929Z Reads: 83

```
Do you know how I should set up the bms then.  would I plug the balance wires into the bms from the back of each 2p or the front? as I beleive each 1s2p should self balance between each other - please correct if im wrong.
```

---
## \#11 Posted by: wafflejock Posted at: 2018-06-29T21:48:00.145Z Reads: 81

```
Cells in parallel will self balance, regarding how to wire I'm not much help there since I've not used a BMS.
```

---
## \#12 Posted by: notepad Posted at: 2018-06-29T22:49:08.728Z Reads: 74

```
Cheers for the help anyhow.  Time to finally finish the build so I can finally finish testing my mounts
https://www.electric-skateboard.builders/t/yin-yang-3d-printed-dual-mtb-motor-mounts-development/43438?u=notepad
```

---

# Batteries dead after board turned off for few hours

### Replies: 6 Views: 461

## \#1 Posted by: freeh18 Posted at: 2017-08-29T21:33:59.151Z Reads: 98

```
Hey there,

I'm currently building my first board. After i've assembled all the electronics, I was extremely proud to see it all working correctly. After some initial dry runs, I've left the board turned off for a couple of hours. After that, I've turned it back on again but the voltmeter doesn't even turn on and the LEDs on the VESCs only shimmer very lightly.
So, today I tried to charge the batteries but after two hours the result is still the same.
I'm hoping, that I haven't killed the batteries yet :|

Does anyone know what can cause these symptoms?

Attached you can find a drawing of my circuit and the documentation of the BMS I use (because somehow I assume the mistake is hidden in its wiring)

Many thanks for your help in advance :)

<img src="/uploads/db1493/original/3X/6/8/68e42f9e5584e4dd038bc15f4245d45aa001acf2.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/d/2/d24f15ebfe772dd888927e0cab74d113558abfbd.png" width="689" height="362">
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-08-29T21:57:58.576Z Reads: 87

```
Get a multimeter and check each cell in the batteries.
```

---
## \#3 Posted by: esk8guy Posted at: 2017-08-29T22:07:41.794Z Reads: 86

```
take out all the extra stuff like the volt meter and anti spark. plug one esc into one battery and one motor and see if it works and go from there. good luck
```

---
## \#4 Posted by: sl33py Posted at: 2017-08-30T00:06:15.609Z Reads: 78

```
Remove the BMS as well and charge direct via lipo charger.  Eliminate complexity and then slowly reintroduce until you figure out where it's drawing your power and killing cells.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-09-04T03:23:04.228Z Reads: 46

```
What charger are you using?
And as @GrecoMan suggested, first thing I would do is check individual cell voltages to see if any are below minimum voltage of 3.0v
If any are below 3.0v then I would replace that pack.
```

---
## \#6 Posted by: freeh18 Posted at: 2017-09-07T20:44:11.372Z Reads: 27

```
Thanks for all your input. The cells are all at 4.09v, so they seem to be fine. After some 'debugging' I bypassed the BMS and everything worked as I wish for.
Do you have an idea how the BMS could be harmed simply by being in 'standby'?
```

---

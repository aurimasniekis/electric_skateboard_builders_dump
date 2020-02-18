# DC input too low Error

### Replies: 9 Views: 1690

## \#1 Posted by: benslmn Posted at: 2017-06-13T14:26:55.165Z Reads: 40

```
I am using a SKYRC imax B6AC version 2 to charge my 5000maH 4S 20C Zippy Lipo battery and every time I attempt to charge my batteries, after about 10 seconds of charging, I get an error message saying my "DC input is too low." 

I have the charger on balance charge mode, the balance cable is plugged into the 4S balance socket with correct polarity, and I am using a normal wall socket. 

How can I fix this problem?
Thanks for your help.
```

---
## \#2 Posted by: chaka Posted at: 2017-06-13T14:34:01.852Z Reads: 34

```
Lower your charging rate or increase the size of your dc power adapter. Your dc adapter can only output a certain wattage, my guess is you are trying to charge at a higher wattage than the adapter can handle.
```

---
## \#3 Posted by: benslmn Posted at: 2017-06-13T14:34:57.546Z Reads: 34

```
Right now I am using the power cable that came with the charger @chaka do I need to buy a new one?
```

---
## \#4 Posted by: chaka Posted at: 2017-06-13T14:37:15.958Z Reads: 29

```
No, you just need to lower your charging rate. 

Can you list the specs on your ac/dc adapter? Also, how many amps are you charging at?
```

---
## \#5 Posted by: chaka Posted at: 2017-06-13T14:46:04.584Z Reads: 22

```
Ok I see, the b6ac has an intigrated converter but it is only good up to 80 watts.  This means you can only charge at a rate of roughly 5 amps at 4s.... maybe less.

Of course it could be something else but this is my best guess.
```

---
## \#6 Posted by: benslmn Posted at: 2017-06-13T14:47:18.647Z Reads: 22

```
DC adapter is 7A and 125 Volts. I was told to charge at whatever your batter amperage is so that is 5A and my voltage is set at 14.8V since it is a 4S battery.
```

---
## \#7 Posted by: chaka Posted at: 2017-06-13T14:54:47.619Z Reads: 22

```
Try charging at 2 amps and see if it still logs the low DC input error.
```

---
## \#8 Posted by: benslmn Posted at: 2017-06-13T14:59:28.903Z Reads: 21

```
That seems to be working. How long do you think it will take to fully charge? Thanks for your help.

Also could I try to charge at 3 or 4 amps or would that be an unnecessary risk?
```

---
## \#9 Posted by: chaka Posted at: 2017-06-13T15:13:01.536Z Reads: 20

```
Charging at 1/2 the capacity is easier on your cells, a little over 2 hours.

 You can try charging at 4 amps and increasing incrementally until it throws a low voltage fault again. This way you can find your "actual" max on that charger for fast charging.
```

---

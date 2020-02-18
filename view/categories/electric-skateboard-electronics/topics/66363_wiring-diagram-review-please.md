# Wiring diagram review please

### Replies: 7 Views: 311

## \#1 Posted by: Matrom Posted at: 2018-08-28T16:48:16.919Z Reads: 116

```
Hello! 
Could somebody please take a look over my BMS diagram? Sorry it’s so messy!
![image|666x500](upload://mSjTTrI7hTmCCzEa7UVJ8tHzOp9.jpg)
```

---
## \#2 Posted by: Namasaki Posted at: 2018-08-28T19:04:41.525Z Reads: 92

```
What is the maximum discharge current of your bms?
If it’s not at least 60a, you’ll need to bypass the bms on the discharge circuit.

Also, connect the red wire from battery B to balance port 4. 
Not the ground wire from battery A
```

---
## \#3 Posted by: Matrom Posted at: 2018-08-28T19:33:29.473Z Reads: 77

```
It’s only rated for 15A discharge, thanks for taking a look. Is this better?
![image|666x500](upload://6cyTqlZF4ZGw65ncBW3ZuYQYx80.jpg)
```

---
## \#4 Posted by: Namasaki Posted at: 2018-08-29T00:00:25.897Z Reads: 60

```
Looks good now. 
Only thing now too many connectors in my opinion. 
I prefer hard wiring the batteries together and to the bms. 
Less chance of connectors rattling loose and less circuit resistance.
```

---
## \#5 Posted by: Matrom Posted at: 2018-08-29T00:04:00.937Z Reads: 57

```
Thank you, is it possible for me to connect the black balance wire from battery B to B- instead of the large gauge battery cathode wire?
```

---
## \#8 Posted by: b264 Posted at: 2018-08-29T05:22:52.544Z Reads: 43

```
Yes, the wire going to B- does not need to be 10AWG like the wire going going to the ESC.  You can use the balance wire for that if you're not running the ESC current through the BMS like the second diagram

The balance and charge wires can be 18AWG to 22AWG and the voltmeter leads can be any size, preferably 22AWG not because of current-carrying capacity, but because of vibration resistance of the thicker wire
```

---
## \#9 Posted by: Namasaki Posted at: 2018-08-29T12:01:52.166Z Reads: 28

```
@b264 is correct but only if the bms is bypassed for discharged. 
So you could connect the balance ground wire of battery B to B- and run the  main ground wire of battery B straight to the Vesc.
```

---

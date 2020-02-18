# How did I reach 26km/h on flat on my board?

### Replies: 4 Views: 400

## \#1 Posted by: Clonkex Posted at: 2017-09-12T23:04:38.556Z Reads: 76

```
Ok that's the question... how did I reach 26km/h on flat on my board? Here's the important numbers:

6S lipo
192Kv
14T motor pulley
30T wheel pulley
63mm wheels
110kg rider

The [esk8 calculator shows](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":192,"system-efficiency":85,"motor-pulley-teeth":14,"wheel-pulley-teeth":30,"wheel-size":63}|) a maximum theoretical top speed of 23.62km/h. Is there anything that could make that calculation inaccurate other than going downhill?
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-12T23:11:32.656Z Reads: 71

```
The calculator calculates 6s as 22.2v which is nominal and lover than fully charged 25.2v, the efficiency should be set to 93 %, i dont know why is it so low as default. Enter 7s battery to get a speed calculation on your full battery. Then you get 25.63 km/h
```

---
## \#3 Posted by: Clonkex Posted at: 2017-09-12T23:33:54.783Z Reads: 59

```
Oh truuuue I'm an idiot, I forgot about the calculation's voltage! Thanks, that makes perfect sense now because I was on full charge! :D
```

---
## \#4 Posted by: Rinzler Posted at: 2017-09-12T23:50:14.124Z Reads: 53

```
Happens to the best of us :wink:
```

---

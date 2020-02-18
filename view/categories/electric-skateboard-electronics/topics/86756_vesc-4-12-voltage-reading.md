# Vesc 4.12 voltage reading

### Replies: 6 Views: 291

## \#1 Posted by: Wilsonliang777 Posted at: 2019-03-10T10:28:40.409Z Reads: 69

```
Hi guys.  I have a question about flipsky 4.12 vesc.   I have a  board  with single  6364 190kv motor on 10s lipo with a flipsky 4.12 vesc. I bypass my bms for discharge.   

 My question or problem is the voltage reading on the mobile phone app.  On my phone the vesc tool voltage reading is 41.00 volt. Is that normal on a full charged 10s lipo?   I tested my battery with a voltmeter and it reads 42.23v.  I also have a lcd battery display connect to the battery out put just b4 the vesc and it reads 41.7v.   Could the vesc and led voltage meter cause the reading difference?   

Battery 42.23v -> lcd voltmeter b4 the  vesc 41.70v---> vesc tool app 41.00v
```

---
## \#2 Posted by: taz Posted at: 2019-03-10T11:27:46.765Z Reads: 62

```
The flipsky esc is known to give inaccurate voltage values.
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-03-10T12:11:51.997Z Reads: 56

```
Like Taz said, they slightly inaccurate. Unfortunately, with lipos, each little tick of voltage is important in maintaning healthy lipos. 
Just adjust your cutoff voltage by the difference and you should be fine
```

---
## \#4 Posted by: Rzkyyy Posted at: 2019-03-10T18:22:17.691Z Reads: 38

```
Just curios, is it safe to charge without bms by using only vesc flipsky or focbox? @Sn4pz @taz
```

---
## \#5 Posted by: taz Posted at: 2019-03-10T18:26:46.529Z Reads: 37

```
I am not sure what you mean.

The vesc has nothing to do with the charging of the battery except for regenerative braking.

The only time it is safe to not use a BMS is if you are using a hobby charger with a balancing function.
```

---
## \#6 Posted by: Rzkyyy Posted at: 2019-03-10T18:29:18.983Z Reads: 35

```
Thank you for your ecplanation
```

---

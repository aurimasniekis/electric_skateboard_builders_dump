# Need help w Vesc settings on Lacroix board build

### Replies: 7 Views: 409

## \#1 Posted by: Atxraider Posted at: 2018-07-30T09:51:36.100Z Reads: 116

```
Would like some advice on what settings I should setup my dual FOCBOXs, mainly on the first motor tab. Here are the specs:

10s6p 30Q
Dual sensored 6374 230kv
8-in tires
5M 72T/16T

I’m currently running it in FOC, and have the ERPM limit set to 60000/-60000, as well as under the app tab I have it set to 53000 and 55000. I’m a big guy, 6’2” 230lbs.  

Any help/advice would be appreciated. 
Thanks
```

---
## \#2 Posted by: linsus Posted at: 2018-07-30T12:02:01.851Z Reads: 101

```
Never owned an F-box so bit unfamiliar with how sensitive they are. guessing you're looking for max and min current values? The default values wont do any harm. But since you got a bick pack you can increase max min quite abit. 

If you experience alot of electrical noise from your motors you can play abit with the "Switching frequency" on the advanced tab. 29-32k is usually the golden spot to make them less noisy. If you're using NRF and have Cruise Control you might have to fiddle abit with the PID values. Think the default values are suited after BV's prefrences but can be altered if you're heavier/leaner then he is, also depends on terrain etc.
```

---
## \#3 Posted by: Atxraider Posted at: 2018-07-30T12:06:13.750Z Reads: 91

```
I’m currently running defaults, except for motor max set at 50A and the ERPM settings bc the motors are 230kv.
```

---
## \#4 Posted by: linsus Posted at: 2018-07-30T12:10:00.546Z Reads: 88

```
Try monitor your current draw and see if you ever Close in on any current tresholds. Since its dual you're pretty much covered with 50A per motor. But I dont see any problem with increasing it a little
```

---
## \#5 Posted by: Devilmycry Posted at: 2018-07-31T04:02:23.537Z Reads: 77

```
What A is your bms 
You can do 60 -60 for motor and
Battery max 40 min -12 
If your bms is 60A 
Make battery max 30
```

---
## \#6 Posted by: Atxraider Posted at: 2018-07-31T22:59:45.170Z Reads: 59

```
I was told by the person who made my battery pack (shout-out to @Brando), “It actually allows bursts up over 100A.” and also suggested 50A for battery max on each FOCBOX.
```

---
## \#7 Posted by: Brando Posted at: 2018-07-31T23:21:24.031Z Reads: 57

```
I have found that 50A always works best for me. The VESC is the bottleneck for most systems and will throttle itself due to heat when nessesary so the battery max setting doesn't actually matter too much. If you have issues just lower the value.
```

---

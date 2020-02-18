# Driving motors with higher voltage than recommended

### Replies: 7 Views: 631

## \#1 Posted by: jmapark91 Posted at: 2018-03-12T18:31:25.506Z Reads: 107

```
Hi,

I was wondering about the output signal from an ESC.
Is the amplitude of the output of the ESC always the same and it's only the frequency that ever changes regardless of the input voltage?

For example, if my ESC can work with 6S and 12S, if I power the ESC with 6S vs 12S, will the amplitude change? Or does the amplitude remain the same, but the 12S just allows my ESC to increase its output frequency to allow the motor to spin more quickly?

I ask because my motor's suggested voltage is 24-36V. Does this translate to 6S to 9S?
What would happen to my motors if I fed 12S to it, provided my ESC can handle 12S? Will 12S damage the motors? Or it just means my motors will be less efficient?
```

---
## \#2 Posted by: Acido Posted at: 2018-03-12T19:07:48.820Z Reads: 96

```
36v is 10s
I do not think that there will be any damage to it
But im not am expert to this
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-03-12T19:10:14.600Z Reads: 93

```
If it is a brushless dc motor you should be all good. The extra voltage will make your motor spin faster and be able to output more power/watts.
```

---
## \#4 Posted by: lrdesigns Posted at: 2018-03-13T01:16:21.224Z Reads: 67

```
You can run any voltage a standard esc can use with a brushless motor. They are not sensitive to voltage, it just results in higher rpm. 

They **are** sensitive to load/amps and heat, so if the rpm is higher than recommended you need to use a higher gear reduction to reduce the load on the motor. 

As long as you keep the motor from getting too hot, all will be fine.

Additionally on 12s you should use a motor with a KV lower than 270, or the rpm may be too high for the esc to handle and your gear ratio starts to get ridiculous with a huge wheel pulley and tiny motor pulley.
```

---
## \#5 Posted by: mmaner Posted at: 2018-03-13T01:57:09.356Z Reads: 56

```
270kv at 12s?  My 1st inclination is to ask in what universe but I assume you are using a crazy bgear reduction to keep from hitting the ERPM barrier or a non-VESC ESC.
```

---
## \#6 Posted by: lrdesigns Posted at: 2018-03-13T02:06:52.214Z Reads: 48

```
Ok yeah 190kv or lower is better on 12s. Currently using 140kv

I did in the past use a 270kv motor on 12s with vesc4 97mm wheels, had to use the 4:1 ratio 12t - 48t gearing and have eprm software limited to 60k. It would only hit the 60k limit on the bench though. It it was not a good setup due to the small motor pulley wearing out super fast, and the large wheel pulley being close to the ground. It did have kick ass torque though and really strong brakes.
```

---
## \#7 Posted by: Cobber Posted at: 2018-03-13T02:39:43.888Z Reads: 44

```
Keep an eye on your bearings as well... at higher rpm they are more likely to seize

I re-lube mine periodically
```

---

# Flipsky 6354 190kV motors / wrong kV rating / 170kV

### Replies: 7 Views: 673

## \#1 Posted by: Marsl187 Posted at: 2018-10-18T19:21:10.852Z Reads: 165

```
Hey there,
I have the 6354 motors from flipsky. They are looking pretty awesome but the KV rating is wrong. 
As you can see in the picture I get rougly 44.000 ERPM which means at 37V 170KV. 
So their motor is labled wrong.
Just wanted to ask if somebody as a similar experience with motors from them?
Also would be nice to see a screenshot of one that really has the 190 KV.
![43115209_2705977642761298_5364413233580998656_n|666x500](upload://nj5GLfzmjopXJ7grDCzkmCxlLmL.jpeg)
```

---
## \#2 Posted by: Hummie Posted at: 2018-10-18T19:22:28.111Z Reads: 156

```
but ur at 95% duty cycle not 100. So pretty close
```

---
## \#3 Posted by: Marsl187 Posted at: 2018-10-18T19:29:18.901Z Reads: 152

```
The VESC is just capable of 95% duty cycle. 
When I plug in my 270KV motors it gives me the right ERPM..
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-10-18T20:28:04.967Z Reads: 144

```
https://www.electric-skateboard.builders/t/realistic-kvs-and-you/23346?u=jc06505n
```

---
## \#5 Posted by: Namasaki Posted at: 2018-10-18T21:24:49.468Z Reads: 127

```
I have Alien HEV 190kv 6355 and 200kv 6374. Four motors and all tested at 170-175 kv
This is a common situation.
```

---
## \#6 Posted by: dareno Posted at: 2018-10-18T21:35:45.560Z Reads: 117

```
Same with my sk8 and sk3.
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-10-19T13:57:17.061Z Reads: 98

```
were you in FOC mode for the kv test? the FOC waveform means the top speed of the motor could be lower in FOC than BLDC.

if you were in FOC can you repeat the test in BLDC mode to see if the results change?

if you’re already in bldc:

40.7v times 94.9% duty is 38.62v effective volts to the motor leads.

44005erpm divided by 7 electrical revs per rev is 6286.4 rpm.

6286.4rpm divided by 38.62v effective is 162.77rpm per volt

so assuming the test was done in BLDC mode the kv looks to be about 162.7kv. all this means is you are getting a bit extra torque per amp and you can achieve the same top speed as a 190kv motor with a slightly lower gear ratio (multiply the intended 190kv gear ratio by 0.85)

also you would have to spin the motor a little bit faster than it will go on its own with outside energy to overcome the bearing resistance, etc until the motor current measures 0a at 100% duty cycle to get the true kv reading. also the motor leads have some voltage drop so the actual voltage to the motor is even lower still.
```

---

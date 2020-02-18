# Vesc thinks I&rsquo;m going double the speed that I&rsquo;m actually going?

### Replies: 8 Views: 229

## \#1 Posted by: Ariehh Posted at: 2019-05-27T06:31:26.595Z Reads: 99

```
Hi,

I installed a Metr Pro last week and when trying it out I was going super slow. I played around with profiles and came to the conclusion that I only had to change the max speed/ERPM to actually go faster or slower.

With GPS I know my top speed is 45km/h, while the Metr app shows ~90km/h.
If I set the max speed to 50 with the Metr app, I'm only going 25km/h etc...

What would be the cause of this? I checked the gearing settings and wheel diameter and those are correct.

My setup is:
- Flipsky Dual Vesc 6.6
- 10S4P
- TB 6355 190kv
- 14T/36T
- 90mm wheels
- Running Sensored FOC mode
- Both the Vesc and Metr are up-to-date

Any tips? Thanks in advance.

Ninja edit: Someone mentioned that it **could** be related to having a dual vesc?
```

---
## \#2 Posted by: mackann Posted at: 2019-05-27T06:37:15.998Z Reads: 92

```
Its because you have wrong settings in metr, go: Settings>Motor and select correct wheel size and gearing
I suggest you also go to battery and choose correct Voltage your battery have.
```

---
## \#3 Posted by: Ariehh Posted at: 2019-05-27T07:03:30.197Z Reads: 80

```
Well, I think you are right. I remember setting it correctly but the gears were both on 1 instead of 14 and 36 but it probably didn't save?

I hope this is the simple fix, I can test when I get back from work.
```

---
## \#4 Posted by: Ariehh Posted at: 2019-05-28T05:33:35.529Z Reads: 51

```
Unfortunately that was not the fix. It still happens.

Dumb question maybe; under Settings>Magic I have "Dual data" turned on. Should that be on if I have a dual VESC instead of 2 seperate ones?
```

---
## \#5 Posted by: mackann Posted at: 2019-05-28T06:18:35.781Z Reads: 41

```
I think so, but best is to ask @rpasichnyk
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2019-05-28T07:09:53.577Z Reads: 37

```
What did you put for the setting "Motor poles"? It should be 14 for your motor
```

---
## \#7 Posted by: Ariehh Posted at: 2019-05-28T07:44:31.635Z Reads: 34

```
It is set to 14 poles indeed.
```

---
## \#8 Posted by: Ariehh Posted at: 2019-05-28T17:02:13.855Z Reads: 12

```
Turning off dual data did the trick, speed is normal now.

Thanks @mackann and @ARetardedPillow for your input.
```

---

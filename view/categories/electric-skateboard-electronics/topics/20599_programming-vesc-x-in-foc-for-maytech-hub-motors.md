# Programming Vesc X in FOC for Maytech hub motors

### Replies: 12 Views: 1303

## \#1 Posted by: on1y Posted at: 2017-04-08T09:05:50.075Z Reads: 221

```
So I got the sensor wire adapters and have it all plugged in correctly. 
1. Since this motor is only 22A what should I set the motor max to? About 15-16A? What about motor min? Does battax/min stay same? 
2. What do I need to know when switching to FOC? Is it really quieter? Pros? Cons?
3. How do I program the sensor values/settings? 
4. How pussy is this thing going to be on hills compared to dual r spec 6355?
5. I just recently purchased the 12mm pulley kit for the R-Specs, any truck modification required?
Thx Y'all. 
6. Looking for a set of Abec 11 Flywheel authentic 90mm. (Found on evolve Australia but shipping is ridiculous)
```

---
## \#2 Posted by: sayreul Posted at: 2017-05-24T15:57:35.182Z Reads: 174

```
hello 
have you tried FOC with this hub motor ? any feedback on your settings ? 

cyril
```

---
## \#3 Posted by: on1y Posted at: 2017-05-24T22:25:35.723Z Reads: 159

```
yes. it runs great. the website ways they are only 24A but Alien power systems rates them at 50A so i raised the motor max to 45A and they run great, way more power. the wheel euro are pretty hard but that was expected.. i would look into the torque boards hubs personally though, they look to be more efficient.
```

---
## \#4 Posted by: sayreul Posted at: 2017-05-24T22:44:26.561Z Reads: 157

```
Nice ! 
Do you use sensors ? 
I m waiting for 2 Vesc x to try this setup 
I need to finish my battery pack ...

I have bought this hubs to ride while waiting carvon v3
```

---
## \#5 Posted by: on1y Posted at: 2017-05-24T22:57:56.319Z Reads: 151

```
the carvon v3 are going to come with custom abec 11 liquid attack trucks specially designed for his direct drive motors.. he sent me a picture, they look bad ass now. stoked also
```

---
## \#6 Posted by: Penny_Pincher Posted at: 2017-06-02T04:41:35.861Z Reads: 131

```
@on1y How was your performance with the maytech hub motors? did you use the 70mm or 90mm motors? I'm looking into buying a set of 90mm motors but I want to know if i'll be able to get the speed and hill climbing ability that I want.
```

---
## \#7 Posted by: on1y Posted at: 2017-06-13T13:03:13.529Z Reads: 111

```
i sold em cuz they are not very great for hills. the website says they're only 24A but I've heard u can put them up to 50A.. on APS site, they say 50a.. also the PU on the wheels are pretty hard. Also, the front two wheels didn't match the same color as the hubs
```

---
## \#8 Posted by: adman Posted at: 2018-01-01T04:46:39.094Z Reads: 72

```
https://youtu.be/kpQbfUXkfY0
```

---
## \#9 Posted by: Berlad180 Posted at: 2018-04-18T15:55:03.962Z Reads: 53

```
Hi man,
So are you sure its ok to set the min and max motor current to 50 Amp ?
Will it burn the motor eventually ? 
Thanks or the review!
```

---
## \#10 Posted by: adman Posted at: 2018-04-19T17:55:25.499Z Reads: 48

```
50 for max is fine.   50 for min would be a very hard breaking.   start min at 25 and work up to confort
```

---
## \#11 Posted by: Berlad180 Posted at: 2018-04-22T10:45:18.499Z Reads: 42

```
[quote="adman, post:10, topic:20599"]
or m
[/quote]

Thanks! ill try it
```

---
## \#12 Posted by: composites_r_awesome Posted at: 2018-07-10T15:19:08.388Z Reads: 26

```
Hi

How are Maytechs holding up so far? Do they overheat much with double the rated cont current?
```

---

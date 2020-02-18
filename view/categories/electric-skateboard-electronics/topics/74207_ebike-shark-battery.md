# Ebike &ldquo;shark&rdquo; battery

### Replies: 21 Views: 842

## \#1 Posted by: venom121212 Posted at: 2018-11-10T22:06:14.577Z Reads: 227

```
US EU No Tax Hailong 36V 13AH Electric Bicycle Battery 36V 12.5Ah Li-ion Battery Pack for Bafang BBS01 350W 500W Motor
 https://s.click.aliexpress.com/e/crImt7ok

Anyone use these shark type batteries on a board? Pretty sleek looking and supposedly good quality cells. I guess China has singles day going on and there's some good deals on batteries
![Screenshot_20181110-170709_AliExpress|281x500](upload://dWSn4mddDRm6nGugfgL0ukFAwtl.jpeg)
```

---
## \#2 Posted by: Grozniy Posted at: 2018-11-10T22:22:43.416Z Reads: 205

```
You would have to change the BMS. 20a is too little. Also there is no info about cell discharge nor their model. 
And how would one mount this bulky battery? Only top mount somehow
```

---
## \#3 Posted by: venom121212 Posted at: 2018-11-10T22:35:18.979Z Reads: 198

```
Yeah I'm looking into top mount. The bms was the real limiter. So what's the factor that sets the continuous rating needed? Is it the motor combined with what voltage the battery is determining regular amp draw?
```

---
## \#4 Posted by: Grozniy Posted at: 2018-11-10T22:40:57.489Z Reads: 178

```
In theory you would need as much as your motor needs. More is always better to limit voltage sag. If you would go  10s5p 30q, would get 75a continuous.
For single drive 10s3p 30q is good, 10s2p is acceptable but big sag, low range and less battery life.
```

---
## \#5 Posted by: venom121212 Posted at: 2018-11-10T22:56:45.595Z Reads: 156

```
So bare with me here :
Motor is 65A, rated for 60A. That battery I listed is outputting 75A continuous (they claim its Samsung LG or Panasonic) but the BMS only supports 20A. So is it only acceptable for low wattage motors that can't pull that many Amps?
```

---
## \#6 Posted by: Grozniy Posted at: 2018-11-10T23:00:40.901Z Reads: 146

```
It will work on flat road. Uphill might not work at all.
Chinese hub boards use 18a per hub with 10s2p30q and they don't do hills
```

---
## \#7 Posted by: venom121212 Posted at: 2018-11-10T23:01:55.388Z Reads: 135

```
I didn't realize the BMS had that much of an effect on discharge. I thought it was meant to handle cell balancing /charging only.
```

---
## \#8 Posted by: Grozniy Posted at: 2018-11-10T23:03:13.124Z Reads: 128

```
If it's a charge only BMS it will be fine. But it looks like it's not bypassed
Where did it say it's 75a discharge?
```

---
## \#9 Posted by: venom121212 Posted at: 2018-11-10T23:04:58.275Z Reads: 118

```
I thought that was provided by you in reference to 10s5p configuration.
```

---
## \#10 Posted by: Grozniy Posted at: 2018-11-10T23:05:40.654Z Reads: 116

```
If it was 30q battery. But it's not because 30q are 3000mah each
```

---
## \#11 Posted by: venom121212 Posted at: 2018-11-10T23:06:36.996Z Reads: 105

```
Ah I see, in reference to c value. Thank you for your info and patience!
```

---
## \#12 Posted by: Sn4pz Posted at: 2018-11-10T23:16:05.934Z Reads: 104

```
I thought it was 10a from each hub?

your point still stands :laughing:
```

---
## \#13 Posted by: silaczdotoalet Posted at: 2018-11-11T00:17:09.402Z Reads: 103

```
Which motors do you use 36V or 48V?
```

---
## \#14 Posted by: venom121212 Posted at: 2018-11-11T01:11:48.005Z Reads: 99

```
It's my understanding that brushless motors don't have a set voltage rating. It's rpm per volt supplied. These are the motor specs though ![Screenshot_20181110-175310_Chrome|281x500](upload://fy8FBwOZ9RLbSC0xSZoSSgvkiX7.jpeg)
```

---
## \#15 Posted by: pat.speed Posted at: 2018-11-11T01:40:20.546Z Reads: 89

```
That is correct they don’t have a set voltage, well until a certain point, I don’t think it would like having 100v pumped through it
```

---
## \#16 Posted by: venom121212 Posted at: 2018-11-11T01:47:26.227Z Reads: 89

```
Challenge accepted!
```

---
## \#17 Posted by: Grozniy Posted at: 2018-11-11T06:45:35.599Z Reads: 79

```
Maytech are one of the best motors
```

---
## \#18 Posted by: venom121212 Posted at: 2018-11-11T12:08:39.268Z Reads: 70

```
These seem to carry a pretty solid reputation, thanks! @psychotiller
```

---
## \#19 Posted by: psychotiller Posted at: 2018-11-12T03:53:02.309Z Reads: 57

```
Can't wait to see the 24s build!
```

---
## \#20 Posted by: venom121212 Posted at: 2018-11-12T12:28:43.375Z Reads: 34

```
I'm going to assume that doesn't void the warranty?
```

---
## \#21 Posted by: Acido Posted at: 2018-11-12T14:31:25.771Z Reads: 27

```
100v but not with 80A maybe 30-40A pretty sure they would handle it
```

---

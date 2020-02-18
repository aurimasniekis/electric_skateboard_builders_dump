# 12S BMS with 10S pack

### Replies: 28 Views: 627

## \#1 Posted by: Fede6686 Posted at: 2019-03-01T19:41:48.258Z Reads: 122

```
Hi everybody!! I'm at my first esk8 and i have a question: I would build a 10s3p battery but with the possibility of upgrade to 12s4p in future. Can I use a 12s BMS connecting 10/12 cables or I must get a 10S BMS and upgrading it too? If yes which do you suggest? And both in charge and discharge or only charge?
Thanksssss
```

---
## \#3 Posted by: pat.speed Posted at: 2019-03-01T20:59:21.417Z Reads: 108

```
No it does work like that. @Fede6686 you can certainly bet a 12s bms and connect just the first 10/11 wires depending on the bms. Any normal bms will allow you to do this, however smart bms modules won’t. 

I’ve done this myself as 12s bms are hard to get cheaply so I used a cheap 13s ebike one
```

---
## \#4 Posted by: Indiangummy Posted at: 2019-03-01T21:06:00.603Z Reads: 93

```
Yup as @pat.speed said you can just plug in the first 10 cells. Someone actually found this out not to long ago. @thisguyhere can confirm
```

---
## \#5 Posted by: StefanMe Posted at: 2019-03-01T21:08:34.940Z Reads: 86

```
🤦🏻‍♂️😂

10 Char
```

---
## \#7 Posted by: TowerCrisis Posted at: 2019-03-01T21:13:34.845Z Reads: 77

```
The BMS may be able to do that, BUT your cells may not.

Upgrading from 10s3p to 12s4p is really not possible if you plan on using the came cells. Lithium cells "age" and it's important to keep the same average age group between the S groups.

You can mix and match old and new cells within a P group (cells connected in parallel) but you cannot mix old and new between cells in series.

So you could upgrade from 12s2p to 12s3p or you could upgrade from 10s2p to 10s3p. But you cannot upgrade from 10s to 12s.
```

---
## \#9 Posted by: TowerCrisis Posted at: 2019-03-01T21:17:20.015Z Reads: 69

```
The BMS doesn't monitor the overall voltage. It only monitors individual cell voltages.

So as soon as any P group reaches the cutoff voltage (like 3.2V) then it will go into protection mode. Or if any group reaches 4.2V it will be trying to burn off that voltage (if charging) or if it exceeds 4.2 it will cutoff incoming power.
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-03-01T21:17:54.087Z Reads: 67

```
How bout on a discharge bms?

Also I've alawys thought that the bms monitor's overall voltage

But I guess I missed that thread
```

---
## \#11 Posted by: TowerCrisis Posted at: 2019-03-01T21:20:30.575Z Reads: 64

```
Yeah, all of what I said applies to both charge and discharge.
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-03-01T21:21:18.317Z Reads: 63

```
Yeah still don't get it, I do but I still can't believe it as bms are designed for a certain voltage
```

---
## \#13 Posted by: Indiangummy Posted at: 2019-03-01T21:24:45.580Z Reads: 61

```
Look on the spec sheet for any bms. It list charge and dischrage voltage for each cell not the total pack voltage.
```

---
## \#14 Posted by: TowerCrisis Posted at: 2019-03-01T21:26:47.490Z Reads: 59

```
Most simple BMS's work like this.

There are two partitions. The first half of the BMS is designed to be able to turn the main power on and off. This is what the negative lead of the battery goes through.

The other half is just for the balance leads.

If you look close, all of these components for the balance leads are rated for low voltage, usually 5V max.

That is because there are "channels" to each balance wire. Between each wire there is a "channel" that will ground the components on the lower voltage lead, and receive power from the higher voltage lead.

These channels do not communicate to each other. They do a few key things:

-burn off power once 4.2V is reached
-monitor cell voltage
-send out a distress signal if the voltage goes above 4.2 or below 3.3

This distress signal goes directly to the other partition of the BMS, the part that does the switching. And if it received this signal then the pack turns off. Simple as that.
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-03-01T21:26:57.314Z Reads: 52

```
Erm they state 37v bms 🤣

And yeah I do understand
```

---
## \#16 Posted by: Indiangummy Posted at: 2019-03-01T21:28:10.145Z Reads: 52

```
Link? They might be able to acomadate 10 cells but the charge and discharge rating it self will be per cell. You are not looking at the spec sheet.
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-03-01T21:29:12.855Z Reads: 55

```
Yeah I know, also kinda weird because my bms wouldn't charge without all cells plugged in
```

---
## \#18 Posted by: janpom Posted at: 2019-03-01T21:29:34.479Z Reads: 58

```
[quote="pat.speed, post:3, topic:85774"]
@Fede6686 you can certainly bet a 12s bms and connect just the first 10/11 wires depending on the bms. Any normal bms will allow you to do this, however smart bms modules won’t.
[/quote]

With the LLT Power smart BMS it won't work out of the box but it can be easily configured for 10-15S.
```

---
## \#19 Posted by: thisguyhere Posted at: 2019-03-01T21:31:05.731Z Reads: 56

```
@scepterr said it works:

https://www.electric-skateboard.builders/t/bms-hunting-no-more/49040

don't do this if you're discharging through bms since voltages will be way different.

but charge only...it maybe doable...but i'd test the SHIT out of it before putting into production.
```

---
## \#20 Posted by: Indiangummy Posted at: 2019-03-01T21:32:07.756Z Reads: 55

```
The Neptune smart bms depend on this idea. They only sell 15s bms and then sell apapters to acomadate 10-14s.
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-03-01T21:39:16.621Z Reads: 54

```
[quote="thisguyhere, post:19, topic:85774"]
don’t do this if you’re discharging through bms since voltages will be way different.
[/quote]

Ha I knew it I knew I wasn't bugging out 😀
```

---
## \#22 Posted by: Fede6686 Posted at: 2019-03-01T22:19:25.733Z Reads: 49

```
Thanks everybody !! So can someone suggest good 12s3p/4p BMS for single and dual 6374?
```

---
## \#23 Posted by: deltazeta Posted at: 2019-03-01T22:28:23.019Z Reads: 47

```
http://www.ti.com/product/BQ77905
I've seen a couple bms's use this chip for voltage detection and controlling the charge/discharge mosfets. The spec sheets shows undervoltage faults are only triggered if there is a cell voltage is above 1.2V and below 3V(depending on undervoltage threshold). So you can just short pins together that aren't being used, since the reading would be 0V.
```

---
## \#24 Posted by: Fede6686 Posted at: 2019-03-01T22:28:35.099Z Reads: 44

```
Better under $50-60
```

---
## \#25 Posted by: AlanZhou Posted at: 2019-03-01T22:32:31.708Z Reads: 44

```
Litechpower

Distributer of bestech bms 

http://www.litechpower.com
```

---
## \#26 Posted by: pat.speed Posted at: 2019-03-02T01:29:41.821Z Reads: 41

```
Why would it not work when discharging through it? I use the bms for charge only and then have the led display connected to the bms output that way it will turn off letting me know my batteries hit the cutoff without cutting out my main power
```

---
## \#27 Posted by: TowerCrisis Posted at: 2019-03-02T07:04:16.060Z Reads: 36

```
You're right to question that.

If it works for charge it WILL work for discharge. (Mileage may vary, I'm talking about dumb BMS's like supower)
```

---
## \#28 Posted by: pat.speed Posted at: 2019-03-02T08:18:16.862Z Reads: 33

```
I agree, I don’t see how voltage is accurate enough to balance to 4.2v but not cut off at 2.8
```

---
## \#29 Posted by: TowerCrisis Posted at: 2019-03-02T08:32:26.834Z Reads: 32

```
Yeah, and it's completely nonsensical to say that a BMS would look at overall voltage.

The entire point is to look at each P group individually. Looking at the entire pack overall would be just a protection circuit, not a BMS.
```

---
## \#30 Posted by: pat.speed Posted at: 2019-03-02T08:58:29.447Z Reads: 31

```
We already have he vesc to look a pack voltage anyway. 

To sum all this up, yes a 12s bms will work with a 10s battery
```

---
## \#31 Posted by: Fede6686 Posted at: 2019-03-03T08:09:49.501Z Reads: 27

```
Really thanks everybody!
```

---

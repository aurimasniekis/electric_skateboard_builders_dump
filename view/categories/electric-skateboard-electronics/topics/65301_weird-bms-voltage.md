# Weird BMS Voltage

### Replies: 7 Views: 212

## \#1 Posted by: Brontech Posted at: 2018-08-18T22:33:19.145Z Reads: 64

```
I've Been Riding my board reliably for a few months, but when on a ride the other afternoon, my board completely shut down.
I restarted the board and it worked completely fine on the way home.
However, the day after that, my board shut down and wouldn't turn on..
When I tried to power back on, the battery meter went from 4% to 0% slowly. 
However, when I tried to power it back on after the the fifth time, with my board upside down, my board shut on, and went back to 74%. But shortly after, my board shut down again, doing the same thing...

I went to go open up my board, and I measures the battery pack's voltage, 47.2V, okay.
Then I went go go measure the B- port on my bms, and that, too, read 47.2V. But, when I went to the P- port, the voltage read 3.3V..
I'm thinking the bms has a problem, but I cannot flip the BMS upside down due to how its secured to the enclosure.
But, if I have to, I will take the BMS out.
Do you guys think the BMS is toast? Or should I take the BMS out and see if anything is burnt, because from the top (Heatsink side), It looks okay.
Any advice is greatly appreciated! :slight_smile:
```

---
## \#2 Posted by: Ishayc Posted at: 2018-08-19T13:21:59.100Z Reads: 46

```
What battery and what BMS are you using?
I'd start with looking for cold/loose soldering joints.
```

---
## \#3 Posted by: SageTX Posted at: 2018-08-19T17:23:44.366Z Reads: 35

```
I agree. Sounds like a loose connection. Especially considering the upside down board "test". Check solder joints in xt60/90 if you are using them. Check at the bms connection too.
```

---
## \#4 Posted by: Brontech Posted at: 2018-08-19T18:21:41.899Z Reads: 32

```
I'm using 2x 8000Mah Lipo batteries in series.
I do agree that a cold/loose solder could be the issue, but when I measured the B- (input) terminal and the positive end of my battery, I got a voltage reading of around 47V, but when I measured the P- (Output) terminal of my bms, it read about 3V.
So I think the issure is between the B- terminal and the P- terminal, and the BMS is right in between those..
I am going to go re solder the B- and P- connections later today and see if that solves the issue, if not, I'll take out the bms to inspect it.
I have a 80Amp Bestech BMS. (Not Bypassed)
```

---
## \#5 Posted by: Ishayc Posted at: 2018-08-19T18:35:20.472Z Reads: 29

```
I assume its the one with the build in switch so you need to turn on the board in order to see the voltages in the P-.
```

---
## \#6 Posted by: Brontech Posted at: 2018-08-19T18:49:02.299Z Reads: 25

```
Ah you are right, the more you know..
I'll turn on the board next time and measure the voltage :sweat_smile:
```

---
## \#7 Posted by: Brontech Posted at: 2018-08-21T19:30:15.798Z Reads: 17

```
Alright I fixed it, for now...
I found out that when I put pressure on the bms wires, which were on top of the bms, my board would cut power.

I moved the bms wires because they were right on the bms and I think that the sharp solder joints from the bms were puncturing the wires.

So I just moved and re arranged the order of the wires in my enclosure and boom its fixed I guess. :joy:

I'll update this thread if the issue comes back tho, thanks for the help!
```

---

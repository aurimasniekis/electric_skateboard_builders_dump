# HELP DIAGNOSE a problem somewhere in the charging system!

### Replies: 20 Views: 258

## \#1 Posted by: reiko Posted at: 2018-09-16T11:17:59.096Z Reads: 86

```
I have charged and discharged my battery successfully about 20 times. When I plugged in the charger today, the LED on the charger did not turn red. 

My charging setup is show on this diagram I drew and also posted a few weeks back![BMS%20DISCHARGE%20BYPASS|424x500](upload://fFMHBvBAgAoleGg23KBeMuJ5JDw.png)

I measured voltage in every possible place and I can't figure out what is going on.

 - The charger is constantly putting out 25.2 volts
 - The leads leaving the charge port are still carrying 25.2 volts
 - P- is 25.2 V
 - B- is 25.2 V
 - Negative battery terminal is 25.2 V.

If I connect the positive charge port lead to the battery positive terminal nothing happens. The voltage read from the battery leads is 21.3 V and the charger stays green. In some cases after completing the circuit, the voltage measured in various places starts fluctuating anywhere between 2 V and 20 V. This is what confuses me the most. I suppose it is possible that just the green LED on the charger is faulty and the board is actually charging, but I can't wrap my head around this weird voltage. Granted, I am not the most experienced in electronics...

Anyways, what do you think? Where do you think the problem might lie? If you have any additional questions I will try to answer quickly, I really just want to get back on the road.

Thanks a lot for taking the time to read this post!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-09-16T11:51:20.091Z Reads: 68

```
Have you thoroughly checked all wire to make sure they aren’t loose, I’ve had a bms wire break off during riding before and my board wouldn’t charge
```

---
## \#3 Posted by: reiko Posted at: 2018-09-16T11:57:17.592Z Reads: 67

```
Okay, I will do it right away. Do I need to check the balance wires as well? Even though unconnected balance wires would be bad for the battery it shouldn't stop it from charging, right?
```

---
## \#4 Posted by: pat.speed Posted at: 2018-09-16T12:00:54.973Z Reads: 62

```
It depends, some bms module won’t allow the battery to charge with a disconnected lead, just unplug the connector and measure the voltage on all connector pins. The voltage should rise by about 3-4 volts per pin
```

---
## \#5 Posted by: reiko Posted at: 2018-09-16T12:50:03.667Z Reads: 53

```
Just finished checking all wires and no problems on that end. This is what the setup looks like atm. All connections are visible and nothing seems to be out of order. The balance wires are also all properly set up. The battery doesn't charge :confused: 

https://scontent.fhen1-1.fna.fbcdn.net/v/t1.15752-9/s2048x2048/41903788_2154254167941331_2276274856620195840_n.jpg?_nc_cat=0&oh=4e34bdb938055d6784aa4c73dab73767&oe=5C210D85

Here are two additional pictures where I check if B- and P- are connected as well, because these are the only connections I didn't rip apart.

B-:
https://scontent.fhen1-1.fna.fbcdn.net/v/t1.15752-9/s2048x2048/41897976_1695394363921013_3727504667685421056_n.jpg?_nc_cat=0&oh=a2a01dd69e9593ae05eb9c23abf699b9&oe=5C152B3D

P-:
https://scontent.fhen1-1.fna.fbcdn.net/v/t1.15752-9/s2048x2048/41801962_311050632961213_1071369601893269504_n.jpg?_nc_cat=0&oh=6b5562a4cf76671822b2de2e4c885a57&oe=5C33F89C

Sorry if I am bothering someone with posting pics of me measuring voltage, but since I do not feel confident in this field, I'm thinking maybe the pictures show something that I am doing wrong and could help solve this whole charging issue.
```

---
## \#6 Posted by: reiko Posted at: 2018-09-16T14:11:13.280Z Reads: 39

```
I will be leaving the house for a few hours and just to make sure the charger's LED is showing green correctly I'll leave the charger plugged in. I hope it will charge so I know exactly what the problem is.
```

---
## \#7 Posted by: reiko Posted at: 2018-09-16T17:25:40.901Z Reads: 40

```
Back home now and the battery was not charging as expected.

I did however find something interesting about the fluctuation. When the charger is plugged in and I'm measuring voltage from the negative battery terminal and the positive lead from the charging port, that's when I get the fluctuating voltage. It was between 9 V and 13 V in this case.

Is this normal? If not, what could it mean?

If anyone has any ideas, I will read them happily. I'm lost on this one.
```

---
## \#8 Posted by: L3chef Posted at: 2018-09-16T17:59:31.287Z Reads: 35

```
that's wierd. Measure the output from the charger
```

---
## \#9 Posted by: reiko Posted at: 2018-09-16T18:03:26.255Z Reads: 34

```
Output straight from the charger is constant 25.2 V as it should be. Sometimes it flicks to 25.3 V but I assume this is the error margin for the multimeter.
```

---
## \#10 Posted by: L3chef Posted at: 2018-09-16T18:06:01.261Z Reads: 34

```
Hmm. So your battery voltage is ok. Your charger is ok. Your chargin plug is ok. Wires are ok. That leaves the bms..
```

---
## \#11 Posted by: reiko Posted at: 2018-09-16T18:10:38.873Z Reads: 31

```
Is there any way to make sure it's the BMS? It sure seems so, but the 25.2 V goes through the BMS module, which sounds like it should still be able to charge the battery.

Would something awful happen if for a short time I connect the charge port leads straight to the battery? So if it starts to charge, I know for sure the BMS is the problem.
```

---
## \#12 Posted by: L3chef Posted at: 2018-09-16T18:15:17.147Z Reads: 30

```
Could be some protection on the bms that triggered and won't let it charge the battery. Look for burnmarks on the bms. Other then that I don't know about. 

Don't connect that charger straight to the battery.
```

---
## \#13 Posted by: mmaner Posted at: 2018-09-16T20:24:38.688Z Reads: 27

```
[quote="reiko, post:11, topic:68195"]
Would something awful happen if for a short time I connect the charge port leads straight to the battery? So if it starts to charge, I know for sure the BMS is the problem.
[/quote]

Nope, I have a 10s3p 30q back that has no BMS, charge and discharge through the Sam port. I couldn't even guess how many charge cycles but it's still balanced as of Friday night (last time I checked the cell groups). 

The need for a BMS is real, but it's for catastrophic failure that it's real value comes into play. 

Don't discharge past 3.4 per cell and only charge to 4.1 per cell and you will "likely"  be good for months and months. Likely is the key word here. It's all fun and games till someone looses an eye right 😄.
```

---
## \#14 Posted by: reiko Posted at: 2018-09-16T20:29:21.607Z Reads: 25

```
Thanks @mmaner! I'll only use it once though to check if the battery charges without a BMS. 

Out of curiosity, how do you check that you don't go past 4.1 per cell? I guess cutoff below 3.4 can be configured with the VESC, but how does the 4.1 part work?
```

---
## \#15 Posted by: mmaner Posted at: 2018-09-16T20:32:52.152Z Reads: 24

```
Mine is a 10s pack, full charge is 42.  I use a lab power supply that allows me to set the voltage and amperage and cutoff. I charge at 1.5a to 41v.
```

---
## \#16 Posted by: mmaner Posted at: 2018-09-16T20:37:10.381Z Reads: 24

```
This is lab power supply I'm using. It was $80 when I bought it. 

KORAD KA6003P - Programmable Precision Variable Adjustable 60V, 3A DC Linear Power Supply Digital Regulated Lab Grade https://www.amazon.com/dp/B00AXL7UJA/ref=cm_sw_r_cp_apa_p7RNBbSSQC6NZ
```

---
## \#17 Posted by: reiko Posted at: 2018-09-16T20:42:11.982Z Reads: 21

```
Nice, I just found something similar in a local electronics store that goes to 50V, 3A for 100€. I probably don't need one, but I really like it!
```

---
## \#18 Posted by: mmaner Posted at: 2018-09-16T20:45:34.571Z Reads: 21

```
There's a lot of 30v units, be careful you don't get one if those. I like the 60v so I can charge anything with it. 

I have the memory buttons set for 41v x 1.5a, 42v x 3a, 50.4 x 2a and 50.4 x 3a. 

It's nice to have at home where I keep my boards, but too bulky to carry around.
```

---
## \#19 Posted by: reiko Posted at: 2018-09-16T20:50:01.057Z Reads: 21

```
Yea I figured. As a proud owner of a single entry level board, I think a brick charger works for now :slight_smile:

btw, I just hooked the charger straight into the battery and the red charger light turned on. Time to order some parts... 

Thanks again!
```

---
## \#20 Posted by: mmaner Posted at: 2018-09-16T20:51:13.715Z Reads: 22

```
No worries, glad to assist. 

Yeah, lab power supplies are pricey so mostly only valuable when you want lots of control and/or have multiple boards.
```

---

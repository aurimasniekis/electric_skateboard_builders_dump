# 10s3P batteries

### Replies: 12 Views: 1195

## \#1 Posted by: NewbieBoardBuilder Posted at: 2017-07-01T02:59:43.092Z Reads: 155

```
Batteries can be set up in series or parallel, but some are cells are connected in series, and the set of series connection are connected in parallel. For example 10s3P. What are the advantages to that over just having them in series?
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-01T03:02:54.406Z Reads: 151

```
Discharge potential is directly related to parallel cells. More cells in parallel, more power delivery
```

---
## \#3 Posted by: JLabs Posted at: 2017-07-01T03:03:16.670Z Reads: 151

```
Come on man, this is like your 3rd or 4th thread about the same thing. Were happy to help, but the information is out there! 

The 10S gives you 36v and the 3p gives you 3x the amount of range. 

If you connected them all in series you would have a 30s1p battery that would not work for an eSk8.
```

---
## \#4 Posted by: NewbieBoardBuilder Posted at: 2017-07-01T03:15:39.967Z Reads: 141

```
[quote="JLabs, post:3, topic:26480"]
that would not work for an eSk8
[/quote]

Why?😂I'm a beginner
```

---
## \#5 Posted by: wmj259 Posted at: 2017-07-01T03:18:20.379Z Reads: 137

```
You would turn the VESC into a marshmallow
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-01T03:18:24.011Z Reads: 135

```
https://learn.adafruit.com/all-about-batteries/overview

Suggest reading above and/or watching below:

https://www.youtube.com/watch?v=m4jzgqZu-4s

Need to get a general gist of what the difference is between voltage (potential difference in charge) vs amperage (speed of the flow of electrons).  The combination of potential (voltage) and speed of charge (amperage) is Watts (power and/or heat).  Based on Ohm's law you should know if you increase V but keep the resistance or components in a circuit the same you increase the amperage flow.  Beyond this various components like capacitors on the VESC or any ESC have Voltage limits and heat dissipation limits (max current basically).

---

The max voltage of components is basically the max safe voltage before something internally shorts or breaks down and the component stops working in an ideal way (usually either shorts closed making a circuit as though the component is just a wire or open, like a break in the circuit, depending on the component type and nature of the failure).

The VESC has a few major components involved, the high level overview is it takes in power through a capacitor bank, to help deal with when it needs a lot of amps to deliver to the motor it doesn't have to come all the way from the battery for short bursts.  There's also voltage regulators that drop and control the voltage input for the STM32F ARM based microprocessor (it needs regulated 3.3 V most likely).  When dropping the incoming voltage for components like the microprocessor some energy is burned off as heat... if it's too much you get marshmellows like @wmj259 said.  After the power goes by the capacitors it goes through the MOSFETs controlled by the DRV8302 chip ( the STM32F does the main processing but hands off the fast firing of the MOSFETs to the DRV chip).  So basically need to look at all these components and their max V and see whatever is lowest is what your limit is, for the VESC this is around 12S I'm pretty sure.
```

---
## \#7 Posted by: oyta Posted at: 2017-07-01T06:05:24.494Z Reads: 109

```
If you look at the illustration here: http://www.electric-skateboard.builders/t/8s-4p-battery-help/25062/2?u=oyta
That shows how it is calculated.

There are many designs. I use 10s3p. If I expand to 10s4p I would increase the range by about 33%. That is for my battery type, LG HG2, going from 3x3Ah=9Ah to 4x3Ah=12 Ah.

For the voltage, you need to put batteries in series. 10x3.6V=36v which suits esk8 well. However it depends on your application.
```

---
## \#8 Posted by: NewbieBoardBuilder Posted at: 2017-07-02T04:31:44.076Z Reads: 83

```
<img src="/uploads/db1493/original/3X/1/2/127aa51b41249d439281a3ff69052a9e4af7c5c4.PNG" width="375" height="500">so what are the differences I'm looking for when buying two 6S batteries in series
```

---
## \#9 Posted by: NewbieBoardBuilder Posted at: 2017-07-02T04:38:54.522Z Reads: 78

```
What mah do people use for Eboards (mono) 12S
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-02T04:57:01.809Z Reads: 77

```
Regarding differences basically the difference in LiPos is Ah capacity and C max amperage as explained here http://www.electric-skateboard.builders/t/s-and-c-ratings/26110/2

With a 12S if you have a high Ah then the C rating can be relatively low and still means high max Amps output.

Example

    5Ah * 20C = 100A
    10Ah * 10C = 100A

Regarding how much is enough it's just the tradeoff of weight and volume of the batteries vs range it will pull you.  I have 5Ah on a 10S can go 12miles, on 12S would expect to go a little further but not linearly further since higher speed means more friction and wind resistance.
```

---
## \#11 Posted by: NewbieBoardBuilder Posted at: 2017-07-02T12:57:07.074Z Reads: 65

```
So what's the difference between 5000Mah 30C 6S1P and 5000Mah 30C 6S... would you recommend either?
```

---
## \#12 Posted by: wafflejock Posted at: 2017-07-02T17:09:41.193Z Reads: 58

```
no difference between what you wrote except the 1P but that doesn't mean anything 1S or 1P is just a cell by itself 2S is two cells stacked butt to head (negative to positive in a line, voltage increase same amps flow through both) 2P is two batteries next to each other negative to negative positive to positive (each supplies half the amperage for the total amperage out of the pair). 1P is not a thing ( a thing, battery in this case, cannot be parallel with nothing you need at least 2 things for them to be parallel | |  <-- see)
```

---

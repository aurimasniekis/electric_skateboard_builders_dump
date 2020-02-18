# Is there a way to measure battery voltage while charging?

### Replies: 14 Views: 4721

## \#1 Posted by: Hillso Posted at: 2016-07-15T14:15:26.330Z Reads: 112

```
Continuing the discussion from [Landyachtz Canyon Arrow | Lipo 8s2p 10A | VESC | BMS Charging](http://www.electric-skateboard.builders/t/landyachtz-canyon-arrow-lipo-8s2p-10a-vesc-bms-charging/4299/11):


Is there a way to measure battery voltage while charging, or will will measure the charging voltage?
battery chargers and BMS know the voltage, but I don't think they can help me to measure the voltage.
```

---
## \#2 Posted by: PB1 Posted at: 2016-07-15T14:32:27.460Z Reads: 112

```
Of course you can measure the voltage of your battery while charging. Use a volt meter in parallel or a Watt meter in series. 

What sort of charger are you using? My Lipo charger shows the voltage the battery pack is at the moment. With the balance lead connected it also shows the voltage of each cell. 

It is true that in theory every measurement influences the result, but I think we can neglect this effect here.
```

---
## \#3 Posted by: Hillso Posted at: 2016-07-15T14:37:51.137Z Reads: 108

```
Thanks for the answer.  I'm using a BMS and power supply, here is my circuit:
<img src="/uploads/db1493/original/2X/1/15d6ec8a5f96f154fde4c8bff3b90c6cd55c2c64.png" width="419" height="500">

<img src="/uploads/db1493/original/2X/4/497d80194fe0dd2cd65bd1542512a392ac05f24d.png" width="580" height="500">
```

---
## \#4 Posted by: PB1 Posted at: 2016-07-15T14:54:00.656Z Reads: 96

```
Sorry mate, I don't get your wiring diagram. 

If I'm not mistaken your batteries will eliminate themselves. Your Volmeter will read 0V. 

What are you trying to achieve? Or am I too stupid to understand your diagram?
```

---
## \#5 Posted by: Hillso Posted at: 2016-07-15T15:03:47.615Z Reads: 92

```
It's ok, I know the diagram is not so clear.

I'm trying to get the voltmeter work only when board is on or when charging.
I got a suggestion to use a npn transistor.
```

---
## \#6 Posted by: PB1 Posted at: 2016-07-15T15:11:35.688Z Reads: 93

```
I'm more worried about how you want to connect your batteries. 

I'm not even talking about the voltmeter. 

You connected your batteries the following way:  (+   -) this is one battery
(+   -)(-   +)(-   +)(+   -) 

What do you want to achieve here? Have you wired this already? Is your board working?
```

---
## \#7 Posted by: Hillso Posted at: 2016-07-15T15:15:25.293Z Reads: 87

```
I'm trying to connect 2 in parallel and 2 in series.

I haven't connected the electronics yet.

so if I connect the batteries like this I will short them?  
Thanks.
```

---
## \#8 Posted by: PB1 Posted at: 2016-07-15T15:23:27.185Z Reads: 80

```
Don't do it this way!!!

You will not short the batteries, but they will eliminate themselves. 

There is a whole section here with wiring diagrams or google how to wire them properly. You need to buy or make a parallel harness. 

And please don't burn down your house, lipos can be very dangerous when not treated properly.
```

---
## \#9 Posted by: Hillso Posted at: 2016-07-15T19:53:19.764Z Reads: 77

```
Is it ok now? 
Thanks.

<img src="/uploads/db1493/original/2X/3/3abc23143abfc75e1f6ad6d81cea547f2e37affc.png" width="416" height="500">
```

---
## \#10 Posted by: PB1 Posted at: 2016-07-15T20:15:21.990Z Reads: 66

```
Charger, BEC and voltmeter looks good.
One input: the VESC BEC is also the PPM input (input from the receiver) so you will have to soldier a custom wire or buy an Y-cable and cut it. 

Batterie also looks good. The drawing is somewhat unusual, but it should work. 

Btw. your charger needs to be able to charge 8s (33,6V end voltage).
```

---
## \#11 Posted by: PB1 Posted at: 2016-07-15T20:34:34.722Z Reads: 67

```
This is how I would connect 4 batteries in series and in parallel. 
<img src="/uploads/db1493/original/2X/d/df2f0da82ae297291731b363d3398d1c034f3d8e.jpg" width="666" height="500">

Using the Anderson Power Poles makes them very flexible and I can easily take the whole pack apart and charge them individually. 
If you are using other connectors you have to buy / make a harness or soldier. 

This would be the corresponding diagram (on the back of an envelope :-) )
 <img src="/uploads/db1493/original/2X/e/e7057cba9730e36d53947712b951e629a3d51532.jpg" width="666" height="500">
```

---
## \#12 Posted by: Hillso Posted at: 2016-07-15T21:05:35.422Z Reads: 62

```
now i understand why my battery diagram is weird.

any idea how to connect the voltmeter so it will work also when charging?
```

---
## \#13 Posted by: devin Posted at: 2016-07-15T22:49:14.052Z Reads: 60

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#14 Posted by: Hillso Posted at: 2016-07-18T19:19:36.073Z Reads: 48

```
This circuit has been suggested to me: <img src="/uploads/db1493/original/2X/6/6e18432e02d3c7f11b36ea983c4873f3f01b62b2.png" width="526" height="500">

I worry that the transistor base voltage will lower the voltage of the system.

Also, is it safe that the board (ESC circuit) will be on while charging?

Thanks.
```

---

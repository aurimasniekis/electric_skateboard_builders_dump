# APS 6384S Motor Problem

### Replies: 10 Views: 799

## \#1 Posted by: RyuX Posted at: 2018-05-29T15:14:43.445Z Reads: 142

```
Hey Guys

I bought an APS 6384S Motor with Hall Sensors.
When I installed it I was never able to Detect the hall sensors and always got Unknown Hall Error 255.
I tried all different Phase Wire combinations and Duty Cycles - no luck.

Then I decided to run the Motor without Sensors and I have to say it almost is as good from the start as my older Maytech 6374 Motor.
One thing that is strange is that even though I didnt connect the Hall Sensor / Temp Plug to the VESC I still got Temperature Readings from the VESC and the Board threw me off at around 28 km/h due to Motor Overheating Error.
I was able to "Run it out" and didn't fall so I was lucky.
I then just increased the Thermistor Value to an insanely high value to keep that from happening - but why does it get readings in the first place ?

So anyone has any experience regarding this hall sensor problem and or had similar experiences running sensorless and getting those temp readings ?

Thanks again
```

---
## \#2 Posted by: Kug3lis Posted at: 2018-05-29T15:19:34.169Z Reads: 137

```
VESC mcu, runs ADC calculation which produces some kind of number depends on circuit so it can be super high or super low, if you have enabled thermal protection or something then yeah it triggered it then read random value overshoot limit :)
```

---
## \#3 Posted by: RyuX Posted at: 2018-05-29T15:21:04.372Z Reads: 132

```
Where can I disable the thermal protection ?
```

---
## \#4 Posted by: RyuX Posted at: 2018-05-30T13:58:34.742Z Reads: 106

```
So today I decided to swap out the Hall Sensor PCB. I took the one from my other Motor which uses Honeywell 43A Hall Sensors.
I had to modify the PCB but now my Hall Sensor detection worked flawlessly on the first try :slight_smile:

Can only recommend those Honeywell Hall Effect sensors (compared to the No Name ones which have been on my APS Motor)..

![grafik|487x500](upload://xoaZgmgH8Aqjlr4IR743RBBRAR8.jpg)![grafik|690x392](upload://v4O2QGLwMysgKurEx2uNY8tb8tC.jpg)![grafik|470x499](upload://b86AbDFobu7sNClvpYXiybpU78K.jpg)![grafik|690x421](upload://qcpFNtGmllXRTwnFFr8u0vGtInq.jpg)![grafik|503x500](upload://cBM4rkaGgrbUkD0jYhCYFkfKiRl.jpg)
```

---
## \#5 Posted by: Deckoz Posted at: 2018-05-30T15:05:21.115Z Reads: 93

```
@banjaxxed I forgot where you posted it but can you share the repin out of the APS Halls?
```

---
## \#6 Posted by: RyuX Posted at: 2018-05-30T15:06:52.846Z Reads: 95

```
There you go
![grafik|583x499](upload://wF2uv4uQQoPYUo3D50UfNsueaIM.jpg)
```

---
## \#7 Posted by: Deckoz Posted at: 2018-05-30T15:07:11.645Z Reads: 94

```
https://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579/968?u=deckoz

Found it...
```

---
## \#8 Posted by: RyuX Posted at: 2018-05-30T15:10:04.576Z Reads: 89

```
Just a good feeling - now it works every time.. those standard APS Halls are crap (imho)
![grafik|466x142](upload://rK4itDQCp6U4F2vJjErgii9jO9M.png)
```

---
## \#9 Posted by: chocol4te Posted at: 2018-05-30T15:17:28.994Z Reads: 86

```
Damn, I bought an 8072S, should I look into replacing them with something better?
```

---
## \#10 Posted by: RyuX Posted at: 2018-05-30T15:27:13.290Z Reads: 79

```
I guess they don't only have one supplier.. I would try the motor first..
```

---

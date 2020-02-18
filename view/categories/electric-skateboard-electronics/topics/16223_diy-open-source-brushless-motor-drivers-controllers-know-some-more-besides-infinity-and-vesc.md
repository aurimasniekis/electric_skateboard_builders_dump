# (Diy / Open Source) Brushless motor drivers (controllers).. Know some more besides Infinity and Vesc?

### Replies: 7 Views: 1239

## \#1 Posted by: Okami Posted at: 2017-01-17T21:03:07.645Z Reads: 102

```
Hi there! I started this discussion because today I saw something very interesting!

One guy had built a simple **-Brushed-** motor controller just out of one mosfet and an arduino.. His ''schematics'' looked really simple.. almost like anyone could build at home lol!

What was even more interesting - he limited his maximum amp output to 8amps. - just to make the motor cooler cause it could not tolerate such heat, if the motor were fed over 10amps.. 20amps would have cooked it from what the author of the video said..

---

I know that Brushed and Brushless motor controllers might be a completely different thing.. but anyways - I wanted to make a little ''review'' or summary, of all the available ''diy/open source'' brushless motor controllers, just in case I dont know one yet and perhaps it is there!
```

---
## \#2 Posted by: IDVert3X Posted at: 2017-01-17T21:08:14.648Z Reads: 95

```
Its super easy to control brushed motor, the same cant be said about the brushless.

For brushed, just a mosfet and simple MCU for PWM control will work, it will suck in a voltage control mode tho... :/

Also, brushed motors tends to heat up more and for the same power, they are bigger. Standstill torque is the only good thing about them.
```

---
## \#3 Posted by: Okami Posted at: 2017-01-17T21:09:30.302Z Reads: 90

```
Hi - I think the guy in video had duty cycle control. this way the amps were controlled

ah yeah, I assume so.. :) though, it was really fascinating for me how easy it is to control brushed motor.. versus the brushless one I assume haha
```

---
## \#4 Posted by: IDVert3X Posted at: 2017-01-17T21:11:41.313Z Reads: 86

```
You can control amps using shunt ( current feedback ) connected to the ADC of MCU and adjust the PWM ( voltage ) so that you have desired current. But yeah... Its still a brushed motor. There is a reason why we dont use them.
```

---
## \#5 Posted by: Okami Posted at: 2017-01-17T21:22:34.105Z Reads: 74

```
Well, the ''old eboards'' did  use the.. even some chinese and ''fiik'' still uses them..

I think even first gen evolve used them.. :D they're still around

--

You are correct about the current feedback part! Good electronics knowledge you have.. :D Will post the video later.. - just for the inside look on brushed motor things..
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-01-18T15:02:05.069Z Reads: 44

```
you can´t tell us things like that and not provide a link to the video :D
```

---
## \#7 Posted by: Okami Posted at: 2017-01-18T15:04:02.294Z Reads: 43

```
Sorry forgot about this thread.. the guy looks quite smart commenting, know some rc things before hand it seems :slight_smile:

https://www.youtube.com/watch?v=fbG35z_UZa0&t=451s 

The title probably says it all lol.. :d I was - ''Holy crap, we are paying up to 100usd for a motor and this guy takes 15$ worth one and turns it into an electric longboard :D

You will see the details later on, if you watch it.. non the less, he was doing just fine with max of 8 amps for the motor..

He also said 30kph or so is too fast for him :D (or at least for his son)
```

---

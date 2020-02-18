# Measuring sensorless motor temperature with TCR( Temperature coefficient of resistance)

### Replies: 11 Views: 844

## \#1 Posted by: Rinzler Posted at: 2018-04-27T11:33:23.771Z Reads: 105

```
So i got an idea after smoking my sensorless motor on a hill. Powered up the hill and noticed smoke coming from my board, the motor is toast. So my idea is to measure the motor winding temperature without sensors via VESC and its ability to measure motor winding resistance, using the following formula for temperature coefficient of resistance. Would like everybody to chime in and start the discussion to see if this is even possible, thanks!
![image|502x277](upload://q78bLGgVyMPfU2sbmThmpaKgTAv.png)
![image|600x497](upload://qXvrgsTSrT2NTbNgI4ndAoRyQrA.jpg)

Here are some links:
http://www.resistorguide.com/temperature-coefficient-of-resistance/
https://www.allaboutcircuits.com/textbook/direct-current/chpt-12/temperature-coefficient-resistance/

The things i dont know are:
1. Is the VESC able to measure the motor resistance while it is commutating the stator
2. Does the VESC have enough processing power to do the calculations 

What should this be used for:
It would be cool to integrate this into the many variations of Android and IOS VESC telemetry/monitor apps @Ackmaniac . There are a lot of folks here that have unsensored motors, and i think it would be nice to know the temperature of the motor. If the VESC cant measure motor resistance while riding it would still be useful if it could measure it when you stop.
```

---
## \#2 Posted by: lock Posted at: 2018-04-27T12:06:40.261Z Reads: 87

```
Apologies if this was your post...

[Motor temperature via winding resistance](https://vesc-project.com/node/185)

> I have done some testing with this as it would be very useful, but so far I only got it working reasonably at low speeds. That was without signal injection though. When I spend more time on signal injection for position estimation at 0 speed for salient motors I will have another look.

Have no personal input on this, well outside my expertise.
```

---
## \#3 Posted by: banjaxxed Posted at: 2018-04-27T16:05:21.528Z Reads: 77

```
A thermocouple sensor lead/chip can do ths? essentally that's what a 3d printer uses

Along with an ardruido and the relevant libraries along with some code

https://www.banggood.com/MAX6675-Sensor-Module-Thermocouple-Cable-1024-Celsius-High-Temperature-Available-p-1086406.html?rmmds=search


Or maybe you can leave out the ardruno & go drect to the vesc but i dunno on that
```

---
## \#4 Posted by: Rinzler Posted at: 2018-04-27T17:07:16.836Z Reads: 67

```
@banjaxxed Yes, that is an easier solution but again it is not practical. The sensor would require excellent thermal contact to the stator which would require some manual work. My idea is to have everything plug and play without sensors and extra wires, and using the potential of the vesc to its fullest. Sadly i dont know how to code so i hope that guys that have the skill chime in.

@lock Benjamin wrote that in 2017-10-27 so maybe he quit the project or he cant make it work. I guess he has a lot of work on his hands. Dont know how realistic is of me to expect for someone from this forum to implement this in the vesc, usually that work is done by Benjamin.
```

---
## \#5 Posted by: b264 Posted at: 2018-05-01T02:01:50.540Z Reads: 61

```
Benjamin has done almost all the heavy lifting as far as code is concerned.  The code in the VESC firmware is exceptionally complicated compared to any of these phone apps or ESC tools or anything.
```

---
## \#6 Posted by: Rinzler Posted at: 2018-05-01T18:04:58.114Z Reads: 47

```
@b264 Guess we will have to wait a while for Benjamin to work his magic.
```

---
## \#7 Posted by: b264 Posted at: 2018-05-01T18:06:42.378Z Reads: 46

```
He might not put a whole lot of effort into it if enertion is just going to steal it.  Let someone else do it
```

---
## \#8 Posted by: mmaner Posted at: 2018-05-01T18:08:40.744Z Reads: 49

```
ease up, enertion is stealing anything.  ben is not willing to work with anyone but Frank.
```

---
## \#9 Posted by: b264 Posted at: 2018-05-01T18:12:04.926Z Reads: 52

```
enertion has stolen it -- on 2018 January 16 they have denied my request per the GPLv3 software license to have the source code for their tool.  This is not legal.
```

---
## \#10 Posted by: Acido Posted at: 2018-05-01T18:19:46.615Z Reads: 52

```
i think i might have their FB firmware and tool code somewhere(there was a download page on their site for something some time ago)
```

---
## \#11 Posted by: b264 Posted at: 2018-11-16T07:33:53.169Z Reads: 35

```
They released it now

https://www.electric-skateboard.builders/t/raptor-2-focbox-source-files/74888/3?u=b264

https://www.electric-skateboard.builders/t/measuring-sensorless-motor-temperature-with-tcr-temperature-coefficient-of-resistance/53641/9?u=b264
```

---

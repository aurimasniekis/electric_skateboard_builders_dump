# SK 3 FOC sensorless start up

### Replies: 13 Views: 620

## \#1 Posted by: cypa9904 Posted at: 2018-04-13T18:59:59.626Z Reads: 155

```
Hi. 
I spent a few hours searching for any video that shows SK 3 FOC start up.
Is there sb who has SK 3 FOC and would tell me if the start up is smooth (and starting from the place is possible without moving/pushing/whatever board)  or I should buy sensored motor?
Thanks for all the answers!
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-04-13T19:26:43.136Z Reads: 142

```
Low kv, high voltage(, Low rider weight) = no Problem
```

---
## \#3 Posted by: Yecrtz Posted at: 2018-04-13T19:34:55.694Z Reads: 138

```
On my old board, 10s single belt drive 192kv it had no problems from a standstill with my 60kgs. However on my Trampa with 2x 149kv 12s with th directdrive from Jenso it works besf if I give it a little push.

With little resistance it should be no problem.
```

---
## \#4 Posted by: cypa9904 Posted at: 2018-04-13T19:41:47.895Z Reads: 134

```
Did you use FOC? Could you also tell me your Trapma reduction? :)
```

---
## \#5 Posted by: Yecrtz Posted at: 2018-04-13T19:50:40.415Z Reads: 120

```
Yea always use Foc. It is a 5:1 if I'm correct. Don't have the new fancy helical gears
```

---
## \#6 Posted by: linsus Posted at: 2018-04-13T20:48:25.557Z Reads: 106

```
"I spent a few hours searching for videos"..

Did you even try Bens own channel? Where he tries FOC on the exact motor you're looking for?..

***Rewokes internet licence***

here you go : https://www.youtube.com/watch?v=ISzeSLpZWbM
```

---
## \#7 Posted by: cypa9904 Posted at: 2018-04-13T21:19:05.595Z Reads: 97

```
Yup. 
Saw this one but this video isn't enough for me.

I read that sensorless startup is not smooth; there's also instruction how to add sensors to sensorless motors for smoother start up so it is not that clear for me.

There are also things like bad terrain, grass etc. Sometimes even slight slope may cause problems, that I want to prevent.

I need sth more than 1 video on flat surface.

btw this is why I am asking for your experience with SK3 FOC.
```

---
## \#8 Posted by: linsus Posted at: 2018-04-13T21:24:46.869Z Reads: 84

```
The detectionless start of the motor works by trying to figure out where the stator is correlated to the rotor, that by trying to step the motor slightly in order to make a more accurate activation of w/e phases are next. 
That beeing said. If you have some spin on it, it wont stutter. But if you're on a complete stop. trying to push full throttle over a lawn that hasnt been mowed for months. Then yes, you wont get an instantaious start. 

there are sevral settings you can play with in order to make the motor more tolerant to w/e surfaces you're planning to adventure on. However every fix has its compromises. So if you really value having the most smooth startup as every possible then the short answer is: Yes. you will want sensors.
```

---
## \#9 Posted by: telnoi Posted at: 2018-04-14T05:49:24.584Z Reads: 64

```
Did not have issues...in my living room. No cogging. 
SK3 149kv 
10s 
5:1   
Trampa, 110 kg.

Since FOC braking was not what I wanted I switched back to bldc.  I am in the process of adding sensors to my SK3. FOC is noticeable better at sensorless startup.
```

---
## \#10 Posted by: Silverline Posted at: 2018-04-14T06:05:54.556Z Reads: 59

```
How are you planning to ad sensors to sk3 ?
```

---
## \#11 Posted by: telnoi Posted at: 2018-04-14T06:13:15.250Z Reads: 55

```
![15236862977572912008323459221298|375x500](upload://i651OKoh9IbYIv2FXyqsuEekQTl.jpg)

You can get something similar here. 
http://e0designs.com/products/hall-effect-sensor-board/
```

---
## \#12 Posted by: Silverline Posted at: 2018-04-14T06:15:06.959Z Reads: 53

```
So the PCB is sitting outside the motor ?
```

---
## \#13 Posted by: telnoi Posted at: 2018-04-14T06:17:14.113Z Reads: 54

```
Yes. Nothing to worry about imo. Properly designed case and silicone spray will protect it better than most internal sensors.
```

---

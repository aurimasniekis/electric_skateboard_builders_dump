# Split ppm one motor faster

### Replies: 15 Views: 144

## \#1 Posted by: yanggatang Posted at: 2019-01-05T23:09:17.433Z Reads: 64

```
I'm currently running split ppm with two diyelectric motors, but one starts before the other and seems to be running faster. Is there anyway to fix this? All the VESC motor settings are the same.
```

---
## \#2 Posted by: Indiangummy Posted at: 2019-01-05T23:10:36.047Z Reads: 62

```
How can you tell one is faster? Would be pretty hard to eyeball it, I would  think. Are you running sensored?
```

---
## \#3 Posted by: Skunk Posted at: 2019-01-05T23:21:53.705Z Reads: 59

```
I imagine this is during a bench test?
Or do you actually feel like you're getting more pull from one motor when accelerating while riding?
```

---
## \#4 Posted by: yanggatang Posted at: 2019-01-05T23:28:53.176Z Reads: 55

```
it is noticeable eyeballing it
```

---
## \#5 Posted by: yanggatang Posted at: 2019-01-05T23:29:02.378Z Reads: 54

```
I'm running unsensored
```

---
## \#6 Posted by: yanggatang Posted at: 2019-01-05T23:29:43.244Z Reads: 53

```
So for the input wizard in the VESC, the two motors differed by quite a bit in terms of center, min and max for the remote. Do you think that could be the case?
```

---
## \#7 Posted by: DeathCookies Posted at: 2019-01-05T23:35:32.057Z Reads: 50

```
Under no load (bench test) you will notice a difference in rpm with almost every build. Even if you connect can and activate traction control it will only kick in after x rpm. 
Thats the case because there are always some differences. Difference in Motor kv, vesc measurements/wizard, Phase wire Length, battery cable Length,....


**As you told maybe the pwm settings are different? Adjust one and copy the settings to the other?** 

But in real life you will not notice a big difference in rpm. Only if something is really fucked up :smiley:

So please test it while Riding and Report back :)
```

---
## \#8 Posted by: yanggatang Posted at: 2019-01-05T23:36:41.495Z Reads: 46

```
alright. will do
```

---
## \#9 Posted by: DeathCookies Posted at: 2019-01-05T23:37:10.025Z Reads: 44

```
I just edited a pwm Part for you
:)
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-01-06T02:23:21.930Z Reads: 31

```
I think what your trying to say for the people that don't understand is.

motors wont spin at at the same time but shouldn't be noticeable in rides, even if connected in can-bus.
```

---
## \#11 Posted by: DeathCookies Posted at: 2019-01-06T02:31:03.943Z Reads: 31

```
[quote="AlanZhou, post:10, topic:80037"]
motors wont start up at the same time but shouldn’t be noticeable in rides, even if connected in can-bus.
[/quote]

No where near i talked about motors that start up at the same time or not.

I just talked genereally why two identical motors would not spin with the same rpm. Not every aspect is important but good for research or error hunting.
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-01-06T02:32:11.448Z Reads: 28

```
i should edit that, but anyways you get the point, theres no way two motors can spin at the same rpm except if you have some nasa like esc precision
```

---
## \#13 Posted by: skatardude10 Posted at: 2019-01-06T02:35:28.759Z Reads: 25

```
I have this. dual via can, and just the minor difference in belt tightness and debris accumulation will cause one to spin, and much faster before the other, depending.
```

---
## \#14 Posted by: DeathCookies Posted at: 2019-01-06T02:36:04.020Z Reads: 26

```
[quote="skatardude10, post:13, topic:80037"]
I have this. dual via can
[/quote]
Did you activate traction control and adjusted the value?
```

---
## \#15 Posted by: skatardude10 Posted at: 2019-01-06T02:39:10.134Z Reads: 25

```
Yep. Off completely, and on with ranges varying from 500-8000erpm. Regardless there's always some difference in each wheels RPM when bench testing... Unless you really have things dialed in. As someone else said before, all the electrical differences combined with mechanical differences, it all adds up and it's totally normal for one wheel to spin faster than another.... *On the bench*

Offtopic, I don't do traction control anymore cause burnouts aren't *as* spectacular. /offtopic
```

---

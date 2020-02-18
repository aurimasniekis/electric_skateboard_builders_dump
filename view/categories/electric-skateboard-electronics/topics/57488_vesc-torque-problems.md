# VESC torque problems

### Replies: 6 Views: 309

## \#1 Posted by: Mathieu Posted at: 2018-06-01T15:11:00.896Z Reads: 89

```
Hello,

i am building a small electric scooter with a VESC. The motor is a turnkey sk3 63mm 193kv and a 10S4P battery. The problem I'm having is after a while there is no power anymore. The first 2-3 minutes I am able to go full throttle without a problem but after a while (mostly after going full power) I can't get any power out of the system, it is really slow and doesn't go as fast as is should. The VESC settings are in the pictures.
![Knipsel|690x348](upload://bnMQm4oBrNLTZfm32BLvEL5zoO8.PNG)![Knipsel 3|690x358](upload://7e43wa7HO5PfjoTlcD7GhnmrcPI.PNG)![Knipsel 2|690x347](upload://9VXGn5qj131rrQJDScjWDhQ5OsF.PNG)
```

---
## \#2 Posted by: Kug3lis Posted at: 2018-06-01T15:15:40.734Z Reads: 79

```
You miss so many key points, like what receiver or control mechanism you use, maybe motor/vesc overheats? How do you transfer power from motor to wheel and etc ;) Also which VESC.

P.S. Your currents without decent cooling is kinda pointer here 85A on 4.12/focbox without a cooling is like burning it and definitely can trigger temp cutoff
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-06-01T15:16:11.686Z Reads: 77

```
yea what he said^^^

I bet it’s thermal throttling
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2018-06-01T15:17:25.967Z Reads: 80

```
Why is your battery cutoff at 0v.,,.

Edit: if you are running 10s it should be at least at 33start and 30end
```

---
## \#5 Posted by: Mathieu Posted at: 2018-06-01T15:49:57.455Z Reads: 63

```
I’m running a htd5m 15mm setup with 20t-60t. Vesc is 4.12, but shouldn’t i have fault in the terminal when i hit top high temperatures? The terminal doesn’t show any faults after when i hook up the Vesc after the problem occurs? I am controlling the vesc with a thumb throttle and e brake trough an Arduino and programmed the Arduino to give a servo output
```

---
## \#6 Posted by: Mathias Posted at: 2018-06-01T17:54:12.826Z Reads: 48

```
[quote="Mathieu, post:5, topic:57488"]
but shouldn’t i have fault in the terminal when i hit top high temperatures?
[/quote]

Nope, it is a soft cut-off starting at 80°C. When you reach that temperature, the VESC will gradually start to reduce power, so exactly what you are describing. This will not produce an error. The hard cut-off is at 100°C, which is what the soft one keeps from happening. 
If you want more continuous power you can heat-sink the FETs. There are a couple of good examples how to do it around the forum.
```

---

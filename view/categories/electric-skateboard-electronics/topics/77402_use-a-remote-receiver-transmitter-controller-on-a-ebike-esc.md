# Use a remote receiver/transmitter controller on a ebike esc

### Replies: 14 Views: 276

## \#1 Posted by: H69pc Posted at: 2018-12-08T02:35:35.292Z Reads: 74

```
Hello guys i am planning to use some hoverboard wheels to build a skate i need 71v to have decent speed on them but the vescs usually don’t go above 60v , i was planning to use a ebike controller but they only support wired throttle anyone heard a way to connect a wirelless receiver to a ebike esc maybe some convertion board that let me connect the receiver to the ebike throttle input…
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-12-08T03:51:32.935Z Reads: 69

```
there are hoverboard wheels that can handle 71v...? jesus christ
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-12-08T03:55:58.635Z Reads: 66

```
id be asking maybe on endless sphere
```

---
## \#4 Posted by: b264 Posted at: 2018-12-08T03:57:03.662Z Reads: 65

```
[quote="H69pc, post:1, topic:77402"]
use a ebike controller
[/quote]

This sounds super scary.  I'd be very careful the brakes don't toss you off at high speed
```

---
## \#5 Posted by: rojitor Posted at: 2018-12-08T10:42:37.168Z Reads: 38

```
Take a gun and shoot yourself, it will be faster and less painful. 
Seriously dude don't do it. It's a suicidal build.
```

---
## \#6 Posted by: bartroosen12 Posted at: 2018-12-08T11:01:19.568Z Reads: 33

```
I don't think 72V will be dangerous, there are enough E-vehicles which work on 16S-20S but you need to check the sensor wires because maybe they have a different wire position.
Ebike controllers normaly have regenerative breaks so that should be nice.

Can't you just plug in a receiver? I know the throttle wire have 3 wires red white and black.
Maybe it just works with a normal receiver
```

---
## \#7 Posted by: Friskies Posted at: 2018-12-08T11:05:10.224Z Reads: 34

```
In what world would you need 72v?? Vesc has regenerative brake by default.....
```

---
## \#8 Posted by: bartroosen12 Posted at: 2018-12-08T11:06:02.301Z Reads: 33

```
These hubmotors have a very low Kv so you need higher voltage to get  decent speed.
```

---
## \#9 Posted by: Friskies Posted at: 2018-12-08T11:10:05.721Z Reads: 35

```
Let's assume that the motors won't overheat or break at the required speeds you are looking for and stop for and second and think....

If you can afford the high end hardware and battery required to drive a system at this spec why not just build with the much cheaper already available parts?
Most of us here use 10-12s with a list of success and speed and torque. 

I want to be positive about this but you are honestly setting yourself up for failure and I don't want to recommend you doing this with the high likelihood of injury ot causing a fire....
```

---
## \#10 Posted by: H69pc Posted at: 2018-12-08T11:10:53.019Z Reads: 34

```
These motors have very low rpm to have a decent speed you need to overvolt them... its not the same like doing it on a regular skt hub motor :-), some ppl report getting to 40 km/h on 72v...., may it works connecting the reciever directly but i think its a long shot i dont know if its the same /compatible signals...., the esc have to have regen ovcourse, its only a project , if you guys have any positive information about these i apreciate it...
```

---
## \#11 Posted by: Friskies Posted at: 2018-12-08T11:19:07.976Z Reads: 30

```
Just don't do this....

https://youtu.be/1y4zh5mAdzA
```

---
## \#12 Posted by: bartroosen12 Posted at: 2018-12-08T11:27:10.100Z Reads: 32

```
Do you have found a better way to put those hubmotors on the trucks?
Maybe they fit on the meepo style back trucks?

I think if you found a more reliable esc that works with higher voltages this would be a fun project.

The ebike controller is maybe a bit to difficult to work with a wireless remote.
```

---
## \#13 Posted by: H69pc Posted at: 2018-12-08T11:41:02.097Z Reads: 29

```
Yes i have those kind of trucks and will try to fit 2 motors on them.... , first i will try with a vesc but i dont know how high voltage can i use withouth burning them... , maybe 52v ...
```

---
## \#14 Posted by: bartroosen12 Posted at: 2018-12-08T13:47:29.761Z Reads: 25

```
12S won't be a problem for the motors. I should try with max 12S (50.4V) for a vesc.
And keep the current low, 10A per motor.
```

---

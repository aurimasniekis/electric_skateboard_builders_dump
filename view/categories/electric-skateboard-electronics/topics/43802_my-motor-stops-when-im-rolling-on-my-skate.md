# My motor stops when I&rsquo;m rolling on my skate

### Replies: 10 Views: 366

## \#1 Posted by: Hansg Posted at: 2018-01-15T20:06:23.881Z Reads: 77

```

Now I have traveled a good distance in my skate. My motor is failing when I am in a course, it stops, even a few days ago it stopped completely and I was going 25 km. I almost fell, but I hurt my foot, after the motor performs this action, I try to accelerate, but I accelerate with the remote control and the engine does not respond, I have to stop it and accelerate it again to make it work.

I need your help to know if it is the VESC configuration or possibly my engine is harmful :frowning:
```

---
## \#2 Posted by: abenny Posted at: 2018-01-15T20:07:38.500Z Reads: 74

```
a) theyre motors not engines
b) what controller are you using? have you set up a failsaife to coast if your reciever loses connection?
and is it just stopping power? or completely locking up?
edit: by controller i meant RC transmitter + remote btw...just realized it could have been interpreted as what speed controller
```

---
## \#3 Posted by: Hansg Posted at: 2018-01-15T20:14:33.721Z Reads: 67

```
I currently use the mini controler remote
https://www.ebay.com/itm/2-4GHz-Transimitter-Radio-Remote-Controller-With-Receiver-for-Skateboard-OS917/311939830787?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

i dont undertand the question: **have you set up a failsaife to coast if your reciever loses connection?**

the motor stops completely and then in the course it continues presenting the same fault
```

---
## \#4 Posted by: abenny Posted at: 2018-01-15T20:16:08.514Z Reads: 63

```
does the motor stop as if you are braking? or  as if youve let go of the trigger
```

---
## \#5 Posted by: Hansg Posted at: 2018-01-15T20:18:22.065Z Reads: 54

```
it is a sudden braking as if the engine will be completely braked.
```

---
## \#6 Posted by: abenny Posted at: 2018-01-15T20:19:30.301Z Reads: 51

```
and its just for a moment? like you'll be cruising along and suddenly it will brake for a second, then return to normal function?
```

---
## \#7 Posted by: Hansg Posted at: 2018-01-15T20:26:30.775Z Reads: 48

```
If, but after the first time happens the same thing happens during the whole tour
```

---
## \#8 Posted by: laurnts Posted at: 2018-01-15T20:27:10.455Z Reads: 47

```
Few things that can happen here. 1st Motor jammed physically.
2nd It could be VESC power cutoff due to malfunctions or incorrect configuration.
3rd If your phase cable is shorted (that means the 3 cables running from motor to VESC for some reason due to vibration connect with each other).

Most of the time heatshrink broke, small vibration join both phase cable = sudden braking. VESC cut off the power and resume power when phase cable shorts are not happening. Please check your wires.
```

---
## \#9 Posted by: abenny Posted at: 2018-01-15T20:27:39.686Z Reads: 46

```
hmmm...im not too sure then...hopefully the questions i asked plus some more can help someone diagnose your issue...do you have any other parts you can try? like a different receiver? or a different motor?
```

---
## \#10 Posted by: Hansg Posted at: 2018-01-15T20:52:25.450Z Reads: 37

```
I have checked the physical connections and they are well, what comes to my mind would be a bad configuration in the VESC.

On the other hand I have a different remote control to do tests.
```

---

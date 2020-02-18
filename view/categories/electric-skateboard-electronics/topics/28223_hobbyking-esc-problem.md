# Hobbyking esc problem?

### Replies: 19 Views: 2296

## \#1 Posted by: colossalbreacker Posted at: 2017-07-21T21:32:24.480Z Reads: 107

```
So im working on my first eboard and i got the electronics wired up, but when I pull the trigger on the quantum transmitter nothing happens. I've pared the transmitter and the receiver , but i did notice that the hobbyking esc's light is purple,and im not sure if thats normal.
<img src="/uploads/db1493/original/3X/d/9/d9ae2bfc0a9b6346dc0190126b619bdfbcee3563.jpg" width="375" height="500">
here are the parts, any help would be greatly apreciated.
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html

diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/

https://hobbyking.com/en_us/quanum-2-4ghz-3ch-pistol-grip-tx-rx-system.html
```

---
## \#2 Posted by: pat.speed Posted at: 2017-07-21T21:38:44.587Z Reads: 89

```
I have that esc and usually it is purple when the remote hasn't connected to it yet. Have you don't the throttle range on the esc? If not hold down the little button on the soft switch on the esc near the on switch. Turn on the esc while holding down this switch and wait for the light to turn green then push the remote trigger to full brake and wait for a beep, then full forward and wait for a beep, then neutral and wait for a beep. The esc should turn of just turn the same switch off then on and it should go great
```

---
## \#3 Posted by: lowGuido Posted at: 2017-07-21T21:44:34.250Z Reads: 83

```
as @pat.speed just said. you need to calibrate the controller.

although i thought it was full forward first, then full brake.. RTFM.
```

---
## \#4 Posted by: pat.speed Posted at: 2017-07-21T21:47:03.400Z Reads: 83

```
@lowGuido Yes I think you are right I can't quite remember it's still too early here. Just test it and if it's the wrong way do it again the other way
```

---
## \#5 Posted by: lowGuido Posted at: 2017-07-21T21:50:29.923Z Reads: 77

```
oh, and hook those wires up properly. that is a short waiting to happen.
the amount of times people do something like this:
<img src="/uploads/db1493/original/3X/0/9/0986708a2913059eae20958691114f6430052317.jpg" width="255" height="160">
and then wonder why their ESC blew up. 
It is such a bad practice. this is high current we are working with here..
```

---
## \#6 Posted by: colossalbreacker Posted at: 2017-07-21T21:56:34.258Z Reads: 68

```
i was holding them apart when i was testing it, but yeah i know it should be mounted. Great news is the motors turning now, bad news is it doesn't seem to have reverse or brake.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-07-21T21:59:26.661Z Reads: 66

```
usualy for reverse you have to pull back twice first pull is brakes, second pull is reverse. reverse wont engage untill you are fully stopped.
did you do the calibration correctly?
```

---
## \#8 Posted by: colossalbreacker Posted at: 2017-07-21T22:02:06.538Z Reads: 64

```
yeah, i know some escs have options to turn reverse off, but it dont know how to change it if this one does.
```

---
## \#9 Posted by: darkkevind Posted at: 2017-07-21T22:05:00.755Z Reads: 63

```
HobbyKing normally have a PDF manual on their site along with the listing of the product. You can probably program it with a series of throttle movements and listening for specific beeps.

Alternatively you may be able to order a programming card for this ESC from HK.

EDIT: Here's the manual from their site: [Manual](https://hobbyking.com/media/file/264719761X1465900X55.pdf)
```

---
## \#10 Posted by: darkkevind Posted at: 2017-07-21T22:08:48.560Z Reads: 63

```
According to the manual it has brakes, although the modes available don't mention brakes, just reverse.

<img src="/uploads/db1493/original/3X/8/c/8c90d42fab975e7965edfa0f03fdb8391d08f587.png" width="576" height="500">

I imagine Brake mode may be Running Mode: 1
```

---
## \#11 Posted by: lowGuido Posted at: 2017-07-21T22:15:31.751Z Reads: 58

```
mode 1 is forward and brake.
mode 2 is forward brake then reverse.
mode 3 I have never used... sounds dangerous :smirk:
```

---
## \#12 Posted by: colossalbreacker Posted at: 2017-07-21T22:16:10.451Z Reads: 56

```
thanks for the help, any idea on how to actually program the settings? im looking online right now and i dont see much.
```

---
## \#13 Posted by: darkkevind Posted at: 2017-07-21T22:17:03.007Z Reads: 60

```
Read the manual. It tells you just above that chart....
```

---
## \#14 Posted by: lowGuido Posted at: 2017-07-21T22:19:32.530Z Reads: 59

```
I feel that every question in this thread could be answered by reading the manual.
```

---
## \#15 Posted by: Cobber Posted at: 2017-07-21T22:25:31.360Z Reads: 57

```
The force is strong with this one

https://www.youtube.com/watch?v=11IABg1un6A
```

---
## \#16 Posted by: colossalbreacker Posted at: 2017-07-21T22:27:16.822Z Reads: 57

```
Based on the manual i would assume i need to buy the programming card, the only thing related to programming i see above the chart is throttle range calibration.
```

---
## \#17 Posted by: darkkevind Posted at: 2017-07-21T22:34:13.787Z Reads: 55

```
It does mention programming by LED at the beginning...

Features:
● Enhanced throttle response, excellent acceleration, linearity and driveability
● Using advanced PC interface to set up or update the firmware
● **Using both of LED and LCD program card to make adjustments.**
● Adjustable BEC output 6.0V/8.4V
● Multiple protection features: Low voltage cut-off protection, over-heat protection and throttle
signal loss protection
● Compatible with NOVAK, LRP , ORION brushless motor
```

---
## \#18 Posted by: lowGuido Posted at: 2017-07-21T23:09:39.473Z Reads: 51

```
I have only ever used the LED programing card, however default settings work well for the most of it.
only thing I ever change is to maybe set initial acceleration lower for beginners. and timing higher for top speed.
```

---
## \#19 Posted by: pat.speed Posted at: 2017-07-22T02:59:58.555Z Reads: 52

```
Also buy the LCD programming card don't get the led one because lots of people have had it not work
```

---

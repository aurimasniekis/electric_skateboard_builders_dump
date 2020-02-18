# My motor is wrong

### Replies: 15 Views: 357

## \#1 Posted by: Hansg Posted at: 2019-03-20T16:27:10.943Z Reads: 155

```
Hello team,

On Monday I was riding my skateboard, but in a moment it stopped, I touched the engine and it was hot. I want to ask you about it, I do not know if I can fix my motor or I need a new one, I have attached video for your help. I want to make sure that the error is the motor and not the VESC.

https://photos.app.goo.gl/zowp16V6YCo9faDA8
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-03-20T16:32:02.323Z Reads: 149

```
BLDC motors have issues starting smoothly from a standstill, but that doesnt seem to be your issue here....

Please post your vesc settings if you want proper help


e: oh yeah crushing it. :+1:
```

---
## \#3 Posted by: olestra Posted at: 2019-03-20T18:29:04.928Z Reads: 129

```
check the resistance of all three coils, it looks like one is shorted
```

---
## \#4 Posted by: Hansg Posted at: 2019-03-20T20:29:52.414Z Reads: 108

```
could let me to know some manual how I can validate the check the resistance of all three coils?
```

---
## \#5 Posted by: b264 Posted at: 2019-03-20T20:31:22.137Z Reads: 105

```
@Dareno do you have that procedure saved?
```

---
## \#6 Posted by: mikenyc Posted at: 2019-03-20T20:45:26.423Z Reads: 97

```
can you turn the motor by hand easily?
```

---
## \#7 Posted by: Hansg Posted at: 2019-03-20T20:52:17.042Z Reads: 91

```
yes but it sounds weird
```

---
## \#8 Posted by: mikenyc Posted at: 2019-03-20T20:56:56.347Z Reads: 85

```
without power? everything shut down?
```

---
## \#9 Posted by: Hansg Posted at: 2019-03-20T21:21:48.077Z Reads: 85

```
I do not understand your question, but if you want to say when I remove the battery from the speed control, yes, the engine shuts down.
```

---
## \#10 Posted by: olestra Posted at: 2019-03-20T21:46:27.916Z Reads: 81

```
use a multimeter, measure resistance from wire 1 to 2, 2 to 3, and 3 to 1. each measurement should have very close to the same small resistance. the amount of resistance you should expect can be found on the motors specifications
```

---
## \#11 Posted by: dareno Posted at: 2019-03-24T03:21:57.855Z Reads: 58

```
[quote="b264, post:7, topic:69843"]
Disconnect the motor from everything and disregard the sensor cable, if present.

Connect phase A to phase B and verify by hand spinning that there is choppy braking
Connect phase A to phase C and verify by hand spinning that there is choppy braking
Connect phase B to phase C and verify by hand spinning that there is choppy braking
Connect phase A to phase B to phase C and verify by hand spinning that there is strong, smooth braking

If any of the first 3 brakes feel different, the motor has an issue. They should feel *identical* . The last brake should feel smooth and not be cogging.
[/quote]

This is a surefire way of checking the motor status.
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-03-24T05:18:47.978Z Reads: 51

```
@Hansg Do what @olestra and @dareno have said. 

You can also try to spin the motor with nothing connected to it. It should spin smoothly and with little noise. If there is noise or resistance, you may have a bad bearing.
```

---
## \#13 Posted by: Hansg Posted at: 2019-03-28T03:07:39.548Z Reads: 27

```
Hello friends, I was doing the validations and in the 4 ways it works well.

A-B braking Connect 
A-C braking Connect 
BC braking Connect 
ABC is strong, smooth braking

in this case, it may be the VESC that is damaged, I'm not sure which of the components has problems.
I was looking at the VESC and I can program it well, I even put it to change the direction of the motor and take the change
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-03-28T03:52:27.936Z Reads: 23

```
Does it spin smoothly with no wires connected?
```

---
## \#15 Posted by: Hansg Posted at: 2019-03-29T02:59:19.188Z Reads: 14

```
yes it spin smoothly with no wires connected
```

---

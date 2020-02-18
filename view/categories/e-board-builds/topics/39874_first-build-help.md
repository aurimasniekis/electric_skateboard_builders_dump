# First build.Help!

### Replies: 23 Views: 1130

## \#1 Posted by: Timg Posted at: 2017-12-01T16:09:29.892Z Reads: 96

```
So i m a 15 year old Romanian who d like to build his first board. I allready built my deck with a hydraulic press i made and would like to make it electirc.
These are the parts i was looking for:

Battery 2 6s 8000mah: https://hobbyking.com/en_us/turnigy-nano-tech-8000mah-1c-lipo-battery-xt90.html. i want to desolder the cells and lay them on flat across the board
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html
For the wheels i m asking for some suggestions. Some Flywheels would be best.
Vesc: https://hobbyking.com/en_us/turnigy-sk8-esc-for-electric-skateboard-conversion.html ( i don t know if it s good enough)
And all the other bits and pieces also from HK that i allready have.
Hoping for some sugesstions from more experienced builders in this category. thx
(sorry if my spelling wasn t quite correct)
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-12-01T16:36:02.122Z Reads: 77

```
Are you planning to go with the two 6s batteries in series, or parallel?
```

---
## \#3 Posted by: Timg Posted at: 2017-12-01T16:37:14.437Z Reads: 72

```
I m planning to go in series
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-12-01T16:39:23.430Z Reads: 69

```
Your motor is too high KV then. For 12s, you need 170kv or less.
```

---
## \#5 Posted by: Timg Posted at: 2017-12-01T16:40:37.523Z Reads: 68

```
So can you estimate the speed if i go with 190kv?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-12-01T16:42:31.002Z Reads: 68

```
A 245kv motor would do well with 6s. 
And with 16ah You would have decent range. 
You could just put the batteries in parallel
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-12-01T16:42:44.878Z Reads: 66

```
The calculation is: number of cells (12)* full charge cell voltage (4.2)* number of pole pairs in the motor (7)* the kv of the motor. You want the result to be less than 60000. 170kv gives ~59900.
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-12-01T16:43:16.825Z Reads: 66

```
Also what namasaki said.
```

---
## \#9 Posted by: Timg Posted at: 2017-12-01T16:48:07.370Z Reads: 63

```
thx i used this calculator and it resulted in 45~ km/h wich is fast if you need it, but i m pretty sure you re right: http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":240,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":48,"wheel-size":80}|. Also,is that vesc any good?
```

---
## \#10 Posted by: MysticalDork Posted at: 2017-12-01T16:50:00.556Z Reads: 60

```
It's nothing spectacular, but it's okay. I wouldn't run FOC with it, but it should hold up fine.
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-12-01T16:52:32.377Z Reads: 61

```
Remember that you can change your speed by changing your pulleys as well. You aren't stuck with just the battery and motor.
```

---
## \#12 Posted by: Timg Posted at: 2017-12-01T16:56:17.378Z Reads: 61

```
What is FOC? And also, i m pretty light and where i live,there aren t any hills, so i guess i could wire them in paralell, get more range and change the gear ration for a bit more speed than torque cause i don t relly need it
```

---
## \#13 Posted by: FredrikHems Posted at: 2017-12-01T17:00:50.792Z Reads: 58

```
You dont Get more range If you have them in parallell. Also, use the search tool; you will Get lots of information
```

---
## \#14 Posted by: Timg Posted at: 2017-12-01T17:03:44.989Z Reads: 56

```
well than why is paralell better?
```

---
## \#15 Posted by: A-lone-tenno Posted at: 2017-12-01T17:20:44.550Z Reads: 56

```
Yes you do. 6s2p is double the range of 12s1p. You have double the capacity.
```

---
## \#16 Posted by: E1Allen Posted at: 2017-12-01T17:38:17.413Z Reads: 54

```
Double amp discharge as well. Not that it matters with those batteries.
```

---
## \#17 Posted by: egzplicit Posted at: 2017-12-01T17:48:14.808Z Reads: 58

```

[quote="Timg, post:12, topic:39874"]
What is FOC?
[/quote]

To see what FOC is, see http://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/3002 . You can't use it on that VESC anyway, you need much better ones that can handle FOC. But for BLDC it should be ok.
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-12-01T18:23:20.326Z Reads: 54

```
No you don't. You get twice the capacity at half the voltage. Same number of watt-hours either way.
```

---
## \#19 Posted by: FredrikHems Posted at: 2017-12-01T18:42:25.731Z Reads: 52

```
In my experience you will get even more range in 12s1p compared to 6s2p. As you will pull double the amps in 6s, you will generate more heat. Heat=energy
```

---
## \#20 Posted by: A-lone-tenno Posted at: 2017-12-01T18:52:48.040Z Reads: 54

```
Well I've been living a lie, goddammit, what's the point in going parallel than?
```

---
## \#21 Posted by: E1Allen Posted at: 2017-12-01T19:01:14.611Z Reads: 47

```
Higher amp draw and more mAh
```

---
## \#22 Posted by: MysticalDork Posted at: 2017-12-01T19:24:57.288Z Reads: 45

```
You can run higher KV motors, because it can sometimes be hard to find low enough ones for 12s, especially smaller (6355, 5065, etc) ones. 

Also you can use ESCs that can't handle 12s.
```

---
## \#23 Posted by: egzplicit Posted at: 2017-12-01T20:43:33.734Z Reads: 44

```
[quote="MysticalDork, post:22, topic:39874"]
Also you can use ESCs that can't handle 12s.
[/quote]


I was about to say this. Don't use 12S on a hobbyking cheap vesc, I don't think it will survive for long. Go 6S and a higher KV motor (like the 245kv that you listed).
```

---

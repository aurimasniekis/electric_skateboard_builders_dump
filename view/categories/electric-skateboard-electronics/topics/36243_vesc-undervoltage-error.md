# VESC undervoltage error

### Replies: 9 Views: 903

## \#1 Posted by: aaron Posted at: 2017-10-23T06:09:08.116Z Reads: 110

```
Hi, i recent built a board and its been a amazing experience riding it around. However, I'm encountering a problem that i cant solve.

After riding the board for a few minutes, it would, seemingly at random, cut power for a few seconds. Not a gradual decrease that can be attributed to overheating, but a instant cut that leaves me with no power or, more importantly, brakes for a good 5-10 seconds. Afterwords, I would have very low power for a few seconds before everything returns to normal.

looking at the fault codes for the VESC, I get a under-voltage error. with the voltage reading in the mid-high 7 volt range. this is with the battery at 39V. I've checked for shorts, and nothing obvious comes up. all my solder joints are fine, and the temps are in the mid 40's when it errors. 

My battery is a 10s3p enertion space cell, and my vesc is from @chaka so there shouldn't be a problem with those two. I have a sk3 6364 190kv motor with a 15/36 reduction. and 80mm wheels

my best guess for the problem is that my wires are too long since i have two separate enclosures, and soldering on more capacitors will solve the problem. but that is just a wild guess. anyone have any other ideas?

Here are my settings:
https://gyazo.com/d491f52df82439abaf7ff890391ffccd

https://gyazo.com/635d77a99fb9be2e303edec97c1400bd

thanks in advance,
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-23T06:15:12.322Z Reads: 101

```
Pictures of your setup, connections, etc please
```

---
## \#3 Posted by: aaron Posted at: 2017-10-23T06:28:47.110Z Reads: 102

```
https://gyazo.com/e7425f3e820984136cfe3d6786f39145

https://gyazo.com/2c588dc052893b4835d89abb9ae3a4da

sorry about the terrible quality. i dont have the board on me right now and these are all I have. I'll try to get better ones tomorrow.
```

---
## \#4 Posted by: esk8 Posted at: 2017-10-23T08:51:10.806Z Reads: 86

```
Your problem was, that you have making the Battery cut off start to high 37 Volt.
The best setting was by the 18650 cells,
Minimum input Voltage 28V
Maximum input Voltage 57V 
Battery cutoff start 32V
Battery cutoff end  30V
When your Battery have 39V and you calculated the Volt sag the you
came under the 37V and then reducing the Vesc the power from the motor.

And by the setting for the motor:
Motor max 40A was enough 
Motor min -40A 
Batt max    40A
Batt min   -12A
Absolute Max 120A

Regard Attila
```

---
## \#5 Posted by: aaron Posted at: 2017-10-23T09:03:37.957Z Reads: 82

```
Hmm. that does make sense. I'll give it a try tomorrow and get back to you with results. Although I am still somewhat skeptical because in the terminal, it says my voltage dropped to 7.8V, not slightly under 37. 

As for the motor settings, I live in a fairly flat place, but there are one or two extremely steep hills so I need the power for the 10-20 seconds that I am climbing or braking on them. I've tried with 40A, and I cant make it up them. 

Is there a negative effect from having it that high that i should know about?
```

---
## \#6 Posted by: esk8 Posted at: 2017-10-23T09:24:10.046Z Reads: 79

```
The Vesc can continues 50A
Your Battery max 60A when it was charged full
Your Motor working with max 65-70A
When you mean that´s 40A was not enough you can going higher.
Try it with 50A,-50A, 50A
Wich SK3 6364 motor was that ? 190,213 ore 245KV 18, 16 and 14 Turns 
Don´t forget the ERPM limit, not that you kill your Vesc.
I think that under Load the Voltage breaks down.
```

---
## \#7 Posted by: esk8 Posted at: 2017-10-23T09:27:09.051Z Reads: 74

```
Sorry i see now that was a 6364 with 190KV = 18 Turns 
With this motor you have by 42V over 70.000 ERPM.
```

---
## \#8 Posted by: Silverline Posted at: 2017-10-23T09:55:28.466Z Reads: 73

```
Are you sure that sk3 190 have  9 pole pairs ?
Or what do you mean by '18 turns?

I get under 50.000erpm's 

I have the same motor on 10s, thats not a problem at All
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":83}|
```

---
## \#9 Posted by: esk8 Posted at: 2017-10-23T13:31:49.736Z Reads: 57

```
Sorry i have making a mistake 
you are right with 7 pole pairs

left 6374 200KV right SK3 6364 190KV

<img src="/uploads/db1493/original/3X/5/3/5389fbd02953d21d307512dad7a068be9a3f3614.JPG" width="375" height="500">
```

---

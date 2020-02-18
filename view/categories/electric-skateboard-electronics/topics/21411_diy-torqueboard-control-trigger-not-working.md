# Diy torqueboard control trigger not working

### Replies: 12 Views: 843

## \#1 Posted by: willpark16 Posted at: 2017-04-20T05:21:45.291Z Reads: 84

```
So I'm helping my friend with his longboard setup and he has the vesc x paired setup but his torquevoard mini controller trigger isn't working and instead it's the wheel on the side that spins the motor any ideas? Also may need help with some ideal vesc setting for 10s 190kv single
```

---
## \#2 Posted by: Eboosted Posted at: 2017-04-20T05:22:52.352Z Reads: 84

```
You need to connect the channel 2 instead of channel 3 on the receiver. You will have to disassemble the enclosure to do that
```

---
## \#3 Posted by: Namasaki Posted at: 2017-04-20T05:49:21.389Z Reads: 80

```
If I'm not mistaken channel 
1 is the steering wheel
2 is the trigger
3 is open
4 is binding
```

---
## \#4 Posted by: willpark16 Posted at: 2017-04-20T05:54:57.391Z Reads: 76

```
Ahhh thanks @eboosted I'll give her a fo
```

---
## \#5 Posted by: willpark16 Posted at: 2017-04-20T06:16:17.850Z Reads: 71

```
Can anyone recommend some good settings for 190kv 10s4p
```

---
## \#6 Posted by: Eboosted Posted at: 2017-04-20T13:56:23.565Z Reads: 54

```
Motor max 80A
Motor min -80A
Battery max 40A
Battery min - 10A
Absolute max 130A
Curoff start 30V
Cutoff end 28V
```

---
## \#7 Posted by: willpark16 Posted at: 2017-04-20T14:01:16.023Z Reads: 49

```
And for braking when I turn his controller off it spins at top speed
```

---
## \#8 Posted by: Eboosted Posted at: 2017-04-20T16:51:29.983Z Reads: 39

```
It mean you din't set PPM settings correctly.

You needto set PPM settins rab to 50% when rremote is off
```

---
## \#9 Posted by: willpark16 Posted at: 2017-04-20T16:54:03.497Z Reads: 40

```
alright will do
```

---
## \#10 Posted by: flatsp0t Posted at: 2017-04-20T17:00:58.668Z Reads: 38

```
You need to rebind it and remove the bind plug before poweroff to set the failsafe.
https://www.electric-skateboard.builders/t/please-help-when-turning-off-my-controller-the-motor-goes-full-speed/17001/3?u=flatsp0t
```

---
## \#11 Posted by: willpark16 Posted at: 2017-04-20T17:20:05.866Z Reads: 35

```
haha that didnt pop up when I looked for that issue Thanks bro
```

---
## \#12 Posted by: flatsp0t Posted at: 2017-04-20T17:21:09.896Z Reads: 34

```
Well, the search around here can be difficult sometimes.
I only found it because i knew it had to be there ^^.
```

---

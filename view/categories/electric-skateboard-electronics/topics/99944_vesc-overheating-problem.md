# Vesc overheating problem

### Replies: 8 Views: 147

## \#1 Posted by: Klaxs Posted at: 2019-08-08T09:48:12.062Z Reads: 59

```
Hello everyone,

I am having problems with my off road configuration. When the road conditions are extreme, with stones and climbs, the vesc begin to cut the energy more and more, and I have to wait a few minutes to regain total power. I have tried to put some small heatsinks and make some holes in the vesc box and it has a better results, but it is not a complete improvement. Any ideas to solve this problem? These are the features:

126p Samsung 30q battery
8 "Trap Wheels
Ratio 1: 6 12 teeth -72 teeth
2 engines 6374 250 Kv
2 vesc Maytech 4.14
Vesc tool configuration:
     Current max motor: 50
     Current max brake motor: -50
     Battery current max: 30
     Battery current max regen: -12

Thanks!!!
```

---
## \#2 Posted by: JoelMatousek Posted at: 2019-08-08T14:06:53.661Z Reads: 44

```
Maybe you could get a 5v fan and power it with the vesc so it turns on with the board
```

---
## \#3 Posted by: JoelMatousek Posted at: 2019-08-08T14:07:44.941Z Reads: 42

```
The ppm port has a 5v, ground, and signal wire. If you spliced it to the 5v and ground wire it should turn on and off with the board
```

---
## \#4 Posted by: JoelMatousek Posted at: 2019-08-08T14:15:44.252Z Reads: 35

```
Or do you have a 3d printer?
```

---
## \#6 Posted by: Klaxs Posted at: 2019-08-08T14:59:11.737Z Reads: 32

```
No, sorry

I can try with a 5 v little fan. Where y can buy?
```

---
## \#7 Posted by: olestra Posted at: 2019-08-08T15:27:02.679Z Reads: 30

```
https://lmgtfy.com/?q=5v+fan
```

---
## \#8 Posted by: Klaxs Posted at: 2019-08-08T15:42:27.439Z Reads: 30

```
Tenías ganas de soltar la gracia de turno
```

---
## \#9 Posted by: danielz Posted at: 2019-08-08T18:41:23.557Z Reads: 27

```
Mines a similar configuration as yours. I never see more than 45c in the following configuration 
https://danielz.uk/vesc-mods/
```

---

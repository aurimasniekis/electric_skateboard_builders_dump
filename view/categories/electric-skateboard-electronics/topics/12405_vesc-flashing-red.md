# VESC Flashing Red

### Replies: 9 Views: 723

## \#1 Posted by: tonys Posted at: 2016-11-03T18:45:26.766Z Reads: 104

```
I am running 2 VESC connected to 2 motors. They are powered by 2 5s LiPo's in series. Was working fine until I recharged the batteries. Batteries are charged at 4.2v with a balance charger. One VESC stays flashing red, the other is blue. When I disconnect one of the batteries both VESC's operate and control the motors properly. Does anyone know what the problem is? Each battery operates the 2 VESC's properly when connected separately but when connected in series the red light on one of the VESC's flashes and will not operate. Do I need to change the settings on the VESC? I don't believe the batteries are faulty because meter shows they are properly charged.
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-03T18:51:33.447Z Reads: 97

```
What did you set your Max Voltage to? You should leave it at 57
```

---
## \#3 Posted by: tonys Posted at: 2016-11-03T18:57:37.548Z Reads: 95

```
Hi chinzw, I set max input voltage at 42v. Heres all my settings <img src="/uploads/db1493/original/3X/2/d/2d9872ef4686a4421ea956f2a6ce9e2d244b1557.jpg" width="690" height="355">
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-11-03T18:59:49.544Z Reads: 89

```
Don't modify the input voltage values, they are just there to protect the VESC from Voltage spikes. Set max input Voltage to 57V and your problems will be gone.
```

---
## \#5 Posted by: chinzw Posted at: 2016-11-03T19:01:23.871Z Reads: 88

```
That's your problem, set max input voltage back to 57. Im not sure why people keep changing this value.

If your batteries are full, its possible that instead of charging to 4.2v per cell it charged one or more cells to 4.21 or higher, so that would trigger the protection.

Max input voltage is to protect the VESC nothing else, and the VESC is rated for 60V so just leave that 57V alone and youll be fine.
```

---
## \#6 Posted by: elkick Posted at: 2016-11-03T19:02:42.705Z Reads: 79

```
If Jacob Bloy is not taking that false advice out of his YT tutorial we will have this kind of problems for the next 100 years.

I tried to convince him not only once, but he sticks to his false opinion. And of corse, others have to solve it now. Not very funny!
```

---
## \#7 Posted by: tonys Posted at: 2016-11-03T19:05:48.422Z Reads: 71

```
Cool, Thanks so much everyone! I'll change the setting and let u know how it worked. I took my settings from this video (link) as I'm sure many others have. https://www.youtube.com/watch?v=5HLZaMcYRuY
```

---
## \#8 Posted by: tonys Posted at: 2016-11-03T19:37:07.054Z Reads: 66

```
That solved my problem! Thanks so much! You guys are AWESOME!!!
```

---
## \#9 Posted by: flatsp0t Posted at: 2016-11-06T14:09:25.598Z Reads: 42

```
Well, it is not only his videos, but it will be a good start to remove it there.
```

---

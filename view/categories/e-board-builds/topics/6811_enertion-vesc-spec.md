# Enertion VESC Spec

### Replies: 5 Views: 963

## \#1 Posted by: Vermontstig Posted at: 2016-07-29T07:50:36.102Z Reads: 101

```
Will the Enertion VESC work for a 12s 44.4v battery or will it fry it anyone know?
```

---
## \#2 Posted by: Skitzor Posted at: 2016-07-29T07:59:43.714Z Reads: 100

```
It'll work. Just put the right voltage settings in it.
```

---
## \#3 Posted by: makevoid Posted at: 2016-07-29T08:32:55.431Z Reads: 93

```
make sure you have the version with capacitors rated for 60V
```

---
## \#4 Posted by: Vermontstig Posted at: 2016-07-29T08:42:39.828Z Reads: 89

```
I didn't know there was a difference from the reg to platinum lucky I got the platinum. Thanks guys.
```

---
## \#5 Posted by: makevoid Posted at: 2016-07-29T08:47:01.790Z Reads: 85

```
platinum is the warranty, to find out which capacitors do you have they sit on top of the vesc near where you plug the battery, in general there are 2 or 3 and they look like this: https://sc01.alicdn.com/kf/HTB1XZxILXXXXXXQXpXXq6xXFXXXM/382LX473M050B062VS-Aluminum-Capacitors-47000UF-50V-20-382LX.jpg_200x200.jpg

You an see this is a 80V one, if you have the 60V you are fine, if they are 50V because you use 12S voltage you need to replace them with 60V ones (12*4.2V = 50.4V, exceeds the max rated voltage of the 50V ones, also not counting possible voltage spikes)
```

---

# Motor cogging?Is there a setting that can eliminate this?

### Replies: 7 Views: 246

## \#1 Posted by: helpmebuild Posted at: 2019-03-29T22:01:16.944Z Reads: 99

```
Hey guys so at low speeds in grass or pavement mostly grass my motors cog.Im wondering if their is a way to set it up for smoother acc.Its 8085 170kv sesored motors on a 11t-50t 225mm wheels.Trampa vesc6 esc.Could this issue be the kv is too high to run at slow speed?
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-03-29T22:24:30.518Z Reads: 94

```
Post your vesc settings
```

---
## \#3 Posted by: Saturn_Corp Posted at: 2019-03-29T22:28:44.762Z Reads: 91

```
Are you running sensorless in the vesc tool instead of sensored or hybrid?
```

---
## \#4 Posted by: rich Posted at: 2019-03-29T23:42:19.423Z Reads: 76

```
You have to run sensored FOC, there is cogging in sensored or hybrid BLDC mode.
```

---
## \#5 Posted by: mishrasubhransu Posted at: 2019-03-29T23:47:00.682Z Reads: 73

```
I have this annoying cogging now too after the latest firmware update. I am not sure which firmware caused it though but 3.47 maybe
![Screenshot_20190329-194634|281x500](upload://puWOd8HDqnctL0gllIWPvnzKCe0.png)
```

---
## \#6 Posted by: RedBaron Posted at: 2019-03-30T05:26:00.901Z Reads: 55

```
Your gearing seems a little off for such a large tire diameter, I could be wrong. Another thing that could be the cause of the cogging is a failed hall sensor. If your motorplates aren't aligned or off a little in the wrong way, the can rubs against the sensors and breaks them. This happened to me on a 6374 170kv from improper alignment. I desoldered 2 of the 3 sensors and replaced them.
```

---
## \#7 Posted by: helpmebuild Posted at: 2019-03-30T23:57:22.902Z Reads: 35

```
sorry guys for the late reply i will show my settings when i get off work.Its foc sensored with halls
```

---

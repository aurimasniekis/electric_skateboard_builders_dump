# Harming the motor when off throttle?

### Replies: 6 Views: 500

## \#1 Posted by: Pafrican Posted at: 2017-04-19T03:21:58.487Z Reads: 88

```
Hey.
If im cruising and decide to let go of the throttle and coast..will this hurt the motor or ESC?
What if the battery dies? Is it safe to manually ride the board?

Thanks
```

---
## \#2 Posted by: Smorto Posted at: 2017-04-19T11:12:39.945Z Reads: 63

```
[quote="Pafrican, post:1, topic:21339"]
What if the battery dies? Is it safe to manually ride the board?
[/quote]

I believe so yes, as long as you keep your board on but only kick push. Also cruising is ok as well. Anyone feel free to correct me if I am wrong.
```

---
## \#3 Posted by: Nordle Posted at: 2017-04-19T12:13:21.014Z Reads: 49

```
Everything fine!
Except using brakes when no battery is connected. If battery is empty but connected no problem.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-04-19T12:22:54.291Z Reads: 45

```
If you´re pushing, motor is a generator, that needs to go somewhere. So if you have an empty or not full battery connected, your Vesc can put it in there. If nothing is connected, Vesc gets all the energy and absorbs it as heat, but this ability is very limited, so you´ll kill it with a certain amount of energy.
Also don´t shut your board off! Leave it on, so Vesc can do it´s work.
```

---
## \#6 Posted by: Pafrican Posted at: 2017-04-19T12:36:19.629Z Reads: 41

```
Does regen braking have to be enabled?
Also, I'm assuming this doesnt apply to when the battery dies because the VESC is no longer powered?
```

---
## \#7 Posted by: Nordle Posted at: 2017-04-19T12:44:11.232Z Reads: 36

```
If regen braking is disabled cant brake anyways?
The vesc will be powered as long as a battery is connected. Only if the battery is at low voltage you will get under voltage cutoff when trying to accelerate. But no problem in charging it while braking.
```

---

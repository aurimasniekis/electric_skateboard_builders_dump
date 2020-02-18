# 6s on vesc issues?

### Replies: 8 Views: 558

## \#1 Posted by: Izzet Posted at: 2017-08-15T20:03:27.342Z Reads: 63

```
I've read a couple times advice agaisnt using a vesc when running 6s because somehow the amps are too high for the vesc. But now I wonder, is this bs or is it true. If it's true, how does that work? Is it that with a lower voltage the motor draws more amps?

Next question : I'll be running a 15/36 gearing ratio with 6s (possibly). Atm I'm using 70mm wheels but when I'll have more money I'll be using 93mm. Then I wonder if I use a 245kv motor will I have enough torque? Or should I go with a 190kv motor (I live in a city with just a bit of hills)
```

---
## \#2 Posted by: Decdog Posted at: 2017-08-15T20:31:58.544Z Reads: 56

```
I run 6s and vesc with no issues.
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-08-15T20:35:21.312Z Reads: 55

```
Same here, 6s 245kv never had a vesc problem
```

---
## \#4 Posted by: mmaner Posted at: 2017-08-15T20:35:26.939Z Reads: 51

```
I run 6s on 2 boards, no worries.
```

---
## \#5 Posted by: mmaner Posted at: 2017-08-15T20:38:31.430Z Reads: 47

```
[quote="Izzet, post:1, topic:30736"]
Atm I'm using 70mm wheels but when I'll have more money I'll be using 93mm. Then I wonder if I use a 245kv motor will I have enough torque? Or should I go with a 190kv motor (I live in a city with just a bit of hills)
[/quote]

245 is not going to give you a lot of torque, but 6s on 190kv is gonna be really slow.  With 70mm wheels 245kv is probably a good middle ground, but when you move to 93mm you will loose a substantial amount of torque.

<img src="/uploads/db1493/original/3X/0/b/0b95db4368e49cc0bf8ad4a5ff71a9405d746f3f.png" width="690" height="362">
* http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":245,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":70}|
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-08-15T20:42:09.668Z Reads: 44

```
Power (Watts) = A * V

If you lower voltage, to output the same amount of power you need to increase amps. Whether you are on 6S or 12S, the amp limit of the VESC doesn't change. So the 12S setup will have double the power of the 6S setup.

Generally you want to avoid the upper limits of your components, so in order to keep amps low, you can use a higher voltage battery and you won't be stressing the VESC as much for the same amount of power.
```

---
## \#7 Posted by: Izzet Posted at: 2017-08-15T22:31:20.248Z Reads: 31

```
thanks for the replies.

so what should I do for the motor? 245kv or 190kv, I'm probbaly gonna upgrade to 93mm pretty quick.
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-08-16T00:13:49.758Z Reads: 25

```
6s and 245kv on 90mm wheels with 15/36 gearing is about the top you will get. 93mm or 97mm are just to large and will cause heating issues. You say there are hills so even 90mm wheels are a stretch and you may end up goons down to 83mm to avoid thermal shutdown. If you want larger wheels or more speed you will have to move to a 8s or 10s setups. There are no miracles or ways around this.
```

---

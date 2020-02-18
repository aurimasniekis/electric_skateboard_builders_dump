# Manual speed controller

### Replies: 12 Views: 1323

## \#1 Posted by: ninja Posted at: 2016-07-14T21:28:53.851Z Reads: 116

```
Hi! I was wondering if it's possible to control speed without esc? I mean use some kind of device connected with some cable to battery and motor.
```

---
## \#2 Posted by: Stevemk14ebr Posted at: 2016-07-14T22:10:21.479Z Reads: 107

```
No it's not. Brushless motors need an esc to controll which copper coil on the inside receives power. If the wrong coil gets power at the weong time the motor will not spin. The esc is needed to do high speed calculations to make sure it powers the proper coil, it is unavoidable.
```

---
## \#3 Posted by: anorak234 Posted at: 2016-07-14T23:39:32.403Z Reads: 94

```
It is if you have one of those sketchy drill E-boards :laughing:
Nah, the ESC is basically the brain of the electronics.
What is a human without a brain? Useless. Same goes for e-boards.
```

---
## \#4 Posted by: ninja Posted at: 2016-07-15T05:00:22.269Z Reads: 76

```
Ok, thanks for answer
```

---
## \#5 Posted by: ninja Posted at: 2016-07-15T05:08:41.852Z Reads: 72

```


Yes, I understand now.
```

---
## \#6 Posted by: ninja Posted at: 2016-07-18T21:02:31.849Z Reads: 51

```

But this guy in this video at 3:27  https://www.youtube.com/watch?v=PWYBtbleH08, he is using some manual speed controller, maybe becauce those motors are not brushless?! Any ideas?
```

---
## \#7 Posted by: clpjan Posted at: 2016-07-18T21:06:22.018Z Reads: 48

```
i dont think he uses a manual speed controller. his "remote" just isn´t wireless 
he still needs a esc / vesc
```

---
## \#8 Posted by: ninja Posted at: 2016-07-18T21:16:36.019Z Reads: 49

```
O.k. i see! Thing is why i'm so afraid those esc is: when i was younger my hobby was making rc boats, and i remember that sometimes esc were going nuts, like for an example- full speed with no controll, or unexpected brake to unexpected full speed, an so on. So when that kind of things happening on esk8 it can lead to big problems. Thing is that i do not trust esc at all. Maybe these days esc are trustable, are they?
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-07-18T21:30:14.538Z Reads: 40

```
Guess you can say the problems still exist but it isn't a rampant problem ....
```

---
## \#10 Posted by: Maxid Posted at: 2016-07-18T21:51:34.499Z Reads: 35

```
The cheap mechanical ones from the early days suffer from this issue way more than the electronic ones we use today.
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2016-07-19T00:40:12.583Z Reads: 28

```
It's more of a remote control issue. Transmitters use to be a am signal with telescope antenna so when the signal was lost it would lead to full throttle. Remotes now are 2.4ghz that are very reliable when set up correctly. When remote is turned off it has a fail safe so it goes to neutral.
```

---
## \#12 Posted by: anorak234 Posted at: 2016-07-19T00:49:23.019Z Reads: 24

```
The ESC's aren't 100% trustable today, but it's not impossible to make a failsafe. Many people use anti-spark loops that could cut power to the motor very quickly in the event of a failure. @FLATLINEcustoms even put his loop on the top of the board using the drop-through to his advantage. It would be very easy to reach down and cut the circuit in the event of an ESC rampage
```

---

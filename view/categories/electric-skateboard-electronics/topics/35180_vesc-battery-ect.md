# Vesc, Battery ect

### Replies: 8 Views: 468

## \#1 Posted by: Benjamin899 Posted at: 2017-10-09T14:52:44.034Z Reads: 97

```
Hi Guys, i have a couple of questions regarding Vesc:

I know that the Vesc is able to control the current it asks of the battery, but my question is.
 How big can you make your battery? Since there has to be some kind of limitation or can you just built a battery with 300+ Amps and just limit it in the settings and all is good?
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-10-09T15:12:41.485Z Reads: 91

```
This is a common misunderstanding with electronics in general, people are worried there battery will "push" out to many amps when that's just not how it works. It doesn't matter if you have a AAA battery or car battery connected to your motor as long as there the same voltage the motor will DRAW the same amount of current. You see battery's don't push current your load simply draws it. Anyways to answer your question simply no it doesn't matter how big your battery is all that matters is the voltage.
```

---
## \#3 Posted by: Benjamin899 Posted at: 2017-10-09T15:30:36.485Z Reads: 77

```
thank you very much for that crucial peace of information. Guess thats why normal ESC are not that popular on eboards, since we are pushing a lot of load (humans).
```

---
## \#4 Posted by: Namasaki Posted at: 2017-10-09T21:26:45.962Z Reads: 52

```
And, when it comes to batteries, bigger is better.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2017-10-09T22:41:56.913Z Reads: 47

```
even when using rc esc? think they work in voltage control or something.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-10-09T23:31:23.424Z Reads: 40

```
RC ESC's work in duty cycle mode which means that as you increase throttle, they increase voltage to the motor.
```

---
## \#7 Posted by: Benjamin899 Posted at: 2017-10-22T02:11:13.519Z Reads: 26

```
so i am guessing that if the load stays the same, while using a rc esc, and i use a bigger battery and also with a higher c rating but the same voltage it would draw more current since the batteries are able to provide it or is it going to be roughly the same.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-10-22T04:15:23.337Z Reads: 22

```
With duty cycle esc's, the motor current increases as the load increases if you hold the throttle in one position maintaining constant voltage to the motors.
If you increase throttle when the load increases, you are increasing voltage to the motors and then less current is required to produce the wattage needed.

If you use a battery with a  higher  discharge rate, the result will be less voltage sag  which in turn will cause less current to be required.

If the load stays the same and the voltage remains constant, the motors will not draw more current regardless of how high the battery's discharge rate is.
```

---

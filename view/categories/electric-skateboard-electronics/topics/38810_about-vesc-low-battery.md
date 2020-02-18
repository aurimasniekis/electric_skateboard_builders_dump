# About vesc low battery

### Replies: 15 Views: 663

## \#1 Posted by: Bloop Posted at: 2017-11-20T12:29:51.327Z Reads: 65

```
Hey i was thinking if there is any setup on vesc (or external idk) that when the battery is low it will stop the acceleration but keep the vesc on only for breaking ?? and so if you ran low battery you can push to home but still have to breaking if needed or if you get a hill to regen some battery?

Also i saw some posts but im still not sure about this. What will happened if my board is turned off and i kick push it ? Or if i go down a  hill or something ? The current produced by the motor would damage the vesc or not ? And if the vesc is turned on and i kick push the board would this be any different ?? 

Or all the current will go back to the battery even if i dont break ?? 

Thank you.
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-20T12:34:36.427Z Reads: 59

```
Just don't use the throttle and push when you hit cutoff start...
```

---
## \#3 Posted by: Bloop Posted at: 2017-11-20T12:38:26.694Z Reads: 57

```
true that but if i give my board to a friend or something cant tell him hey if you drop that much dont use the throttle. I would like to make it safe for anyone and make sure no one can (unintentional) damage the board
```

---
## \#4 Posted by: scepterr Posted at: 2017-11-20T12:39:30.640Z Reads: 52

```
Well that's what the cutoff end is for

Also, if you like your board, don't give it to anybody, especially a friend 😋
```

---
## \#5 Posted by: Bloop Posted at: 2017-11-20T12:45:47.575Z Reads: 48

```
[quote="scepterr, post:4, topic:38810, full:true"]
Also, if you like your board, don't give it to anybody, especially a friend 😋
[/quote]

Hahaha they wont be friends with me if i dont let them play with this new TOY.

Maybe i dont really understand the cutoff settings. but when it gets to cutoff start it will only reduce the power when accelerating and cutoff stop will stop the board when it gets to that value right ? 
How do i detect when it gets to cutoff start ?
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-20T12:48:59.848Z Reads: 41

```
Its not a toy, it's an electric vehicle, treat it like a car, how many people would you let drive that?

Depending on cells used, 3.4ish volts * S count for start, 3.1-3.3 for end
```

---
## \#7 Posted by: Bloop Posted at: 2017-11-20T12:51:38.623Z Reads: 38

```
yeah i have the values but what is going on with the vesc when it gets to that point 

i have 3.1 start and 2.9 for end  (i like to push it for days when i need that little bit more to get home) 

(When i give it to friends i limit the power so for them will be only kinda toy :joy:. )
```

---
## \#8 Posted by: scepterr Posted at: 2017-11-20T12:53:00.479Z Reads: 37

```
It's what you said it does
If you're on lipo that's really not good for them btw
```

---
## \#9 Posted by: Bloop Posted at: 2017-11-20T12:54:09.916Z Reads: 36

```
And there is no way to stop someone from accelerating when it gets to cutoff start .. so is not really an option.

but again i dont understand what is going on when the board is of (or on with low power) and you push. is this 100% safe or magic smoke will be there.
```

---
## \#10 Posted by: Bloop Posted at: 2017-11-20T12:54:59.456Z Reads: 36

```
li ion samsung 25R  - but only 2 times i really had to get them to 0% rest i discharge them to 20 30 or so 4p is getting me far
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-20T12:55:53.430Z Reads: 36

```
It's safe to push at start or end. Acceleration will be reduced when start is triggered and no acceleration at end
```

---
## \#12 Posted by: chaka Posted at: 2017-11-20T14:21:23.924Z Reads: 25

```
If you ride your board till the throttle cut-off engages from low voltage you will still be able to use your brakes on a hill, let me explain.

If we take our boards and coast down a hill the VESC will allow the motors to raise the voltage through power generation and you will have use of your brakes. The motors generate power anytime they are spinning and connected.

The main problem with this scenario is the act of running your battery low on regular basis. It isn't good for battery health and you could lose control of your brakes due to unpredictable operation.
```

---
## \#13 Posted by: Bloop Posted at: 2017-11-20T14:25:48.330Z Reads: 23

```
Alright but when my battery is low as cutoff end the vesc is powering off (or maybe is from bms not sure did not try with higher cutoff from vesc)

SO you are saying that if i set the cutoff end to 3.2V when the battery gets there the vesc will cut all acceleration but wont turn off ? I will have to test this out. When i got my battery low my vesc turned off but that might be the bms.
```

---
## \#14 Posted by: chaka Posted at: 2017-11-20T14:35:13.928Z Reads: 21

```
The VESC never turns off unless it has no power source, the cut-off is only for throttle function. When we coast the voltage will rise if we are going fast enough. I don't recommend relying on this function but it is how the VESC will behave.
```

---
## \#15 Posted by: Bloop Posted at: 2017-11-20T14:43:12.049Z Reads: 20

```
Alright this make sense now thank you @chaka and @scepterr.
```

---

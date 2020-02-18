# Disconnection Problem

### Replies: 8 Views: 437

## \#1 Posted by: Truckster Posted at: 2017-10-19T18:05:56.792Z Reads: 67

```
Hi Everyone,

bit of a weird problem. I can ride for about 2km and then the controller starts to disconnect or the VESC makes problems. I can't really determine where the problem is located. In the BLDC tool I get no failures. 

My setup is a VESC-X (or FOCBOX now) and a Nano-X controller. 

Anybody knows this problem and what it causes? Really annoying to go for 2km and then it disconnects continuously.
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-19T18:06:53.961Z Reads: 65

```
Faults are cleared when you power off and on, are you making sure you keep it on when you get back to check BLDC tool for faults?
```

---
## \#3 Posted by: Truckster Posted at: 2017-10-19T18:19:43.101Z Reads: 58

```
yes, i kept it on. but at home it worked flawless. very weird
```

---
## \#4 Posted by: Jinra Posted at: 2017-10-19T18:24:27.513Z Reads: 53

```
What are the symptoms? Does it completely turn off? or does the remote just act like it turned off?
```

---
## \#5 Posted by: Truckster Posted at: 2017-10-19T18:31:35.160Z Reads: 46

```
it disconnects. then auto-breaking goes on. turned that off that I at least roll out. It disconnects usually for a second or so and a couple of times in a row. After disconnecting the VESC from the batteries it goes fine for some time and then happens again.
```

---
## \#6 Posted by: Martinsp Posted at: 2017-10-19T22:33:52.915Z Reads: 36

```
Isn't it temperature? From what you said it could be, the vesc does not shut down it just stops sending power to the motor.
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-10-20T00:04:42.840Z Reads: 24

```
try rebinding radio
```

---
## \#8 Posted by: Truckster Posted at: 2017-10-20T04:18:25.474Z Reads: 17

```
Thanks for the help so war. Rebinding I already did. Over temperature I also thought as we have here mainly over 30 degrees Celsius. I opened the cover a bit more for airstream to cool it. But had also no real effect. Obviously can’t rule that out completely. 

Is there anything setting wise to keep the VESC cooler? Reducing amps or something like that?
```

---

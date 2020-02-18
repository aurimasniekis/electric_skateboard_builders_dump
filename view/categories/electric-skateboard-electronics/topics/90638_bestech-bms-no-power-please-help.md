# Bestech BMS - no power? PLEASE HELP!

### Replies: 11 Views: 195

## \#1 Posted by: MrDGOrman Posted at: 2019-04-15T17:03:59.115Z Reads: 59

```
Hi everyone,

I'm building my own battery and have completed it (I'll post pictures at another time). I go to turn it on using my Bestech BMS eswitch (HCX-D596LI12S80A-02) and according to my voltage meter it jumps from 40.x volts to 5 volts. It happens in a split second. The FOCBOX turns on and then off again.

I have a feeling the BMS is dead but I'd like someone to clarify that for me.

Thanks,
Daniel
```

---
## \#2 Posted by: RedBaron Posted at: 2019-04-15T17:26:10.286Z Reads: 51

```
Did you make sure your balance leads are in the proper order? We'd need to see a good picture to really help you. But yeah it sounds like its fried from what you're saying.
```

---
## \#3 Posted by: MrDGOrman Posted at: 2019-04-15T18:53:26.765Z Reads: 48

```
Hey thanks for the reply.

So here's the testing I've done:
- 42v when testing the cells them self
- 4.5v when eswitch is off and multimeter terminals are testing through the BMS
- 28-38v when eswitch is turned on but then drops down to 4.5-5v a split second afterwards
- all balance wires are in the correct format. For some reason there's a left over wire which has no resistors connected to it etc so I joined that with B12. There's 2 connectors - one with 11 wires and the other with 2. The one with 2 wires is, in my understanding, B12 and "B13" if it existed.

My guess is that the BMS has died. Is there a way for me to test if before ordering a new one?
```

---
## \#4 Posted by: MrDGOrman Posted at: 2019-04-15T19:08:58.722Z Reads: 42

```
I've done some further testing.

When connecting the positive end of my multimeter to the positive of the battery and then working my way from B1 to B12 I have the following voltage readings:

B1 - 42v
B2 - 38.5v
B3 - 35v
B4 - 31.5v
B5 - 28v
B6 - 24.5v
B7 - 21v
B8 - 17.5v
B9 - 14v
B10 - 10.5v
B11 - 7v
B12 - 3.5v

Progressively reducing by 3.5v.

I'm guessing this is correcr. Is there a way for me to test the BMS itself or is it not worth the trouble?

Thanks,
Daniel
```

---
## \#5 Posted by: RedBaron Posted at: 2019-04-15T19:28:06.498Z Reads: 38

```
Are you trying to connect a 10s battery to a 12s bms? If so thats your problem right there. 

For 10s there are 11 balance leads. B1 goes to the main negative terminal, and every lead after goes to the remaining positive terminals for a total of 11 balance wires where the last lead is on the main positive terminal. 

Same goes for 12s except there are 13 balance leads.
```

---
## \#6 Posted by: MrDGOrman Posted at: 2019-04-15T19:59:31.150Z Reads: 35

```
No I've got a 12s6p pack and am using a 12s BMS from eskating.

So are you saying the balance wires should be on the positive end and not the negative end? I always thought it was negative cell ends!

Will it make a difference which side it's on?
```

---
## \#7 Posted by: RedBaron Posted at: 2019-04-15T20:51:58.199Z Reads: 33

```
Im not to sure about that, but I've always put B-1 to the main neg terminal where the leads come out for the vesc and every balance lead after to the positive terminals all the way to b+. So yeah im pretty sure your leads are wrong.
```

---
## \#8 Posted by: MrDGOrman Posted at: 2019-04-15T20:57:52.036Z Reads: 33

```
Okay, I'll do some multimeter testing tomorrow to see what voltage I would get if I shifted them all along one.

It's so frustrating that there isn't a solid "do it this way" guide. I swear there's some seasoned battery builders on here that could help?

I will definitely look into what you've said though. The last thing I want to do is strip it all down again and redo it!
```

---
## \#9 Posted by: MrDGOrman Posted at: 2019-04-16T20:55:25.523Z Reads: 25

```
You were correct RedBaron.

I should of paid closer attention to the schematics! Either way, all working as expected now. Thanks!
```

---
## \#10 Posted by: RedBaron Posted at: 2019-04-16T22:20:15.687Z Reads: 25

```
Glad you got it sorted out! Enjoy!
```

---
## \#11 Posted by: MrDGOrman Posted at: 2019-04-17T08:05:02.766Z Reads: 16

```
Cheers mate!
```

---

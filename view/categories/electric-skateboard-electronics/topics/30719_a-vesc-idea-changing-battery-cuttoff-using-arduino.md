# A vesc Idea: Changing battery cuttoff using arduino?

### Replies: 6 Views: 368

## \#1 Posted by: onepunchboard Posted at: 2017-08-15T16:27:27.538Z Reads: 63

```
Hi,
I have 2 set of batterits 6s 6ah and 10s 5ah.
So I thought if I can change voltage cut off using Bluetooth via arduino, I can swap to small battery in case big one dies. Do you think it's possible?
board like boosted has slow and fast mode, so same concept, but not sure if vesc can be programed like that
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-08-15T16:55:43.357Z Reads: 54

```
I don't know where you get those commands, but in theory it should be doable. But why not just use a regular Voltage meter or use the Arduino for that?
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-08-15T17:43:41.643Z Reads: 46

```
okay, I first tired to figure out via Bluetooth connection to phone, but Im not sure if u can change voltage cut off. and if I can eliminate taking out the phone opening app wait for connection so on. It's just a thought. XD
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-08-15T17:59:28.804Z Reads: 37

```
I get ya, tinkering is always the most exciting. You can send a lot of different serial commands via Bluetooth to the VESC, but you would probably need a custom app or serial monitor for this. Look for the Vesc Uart Library for Arduino, this will be a good starting point.
```

---
## \#5 Posted by: saul Posted at: 2017-08-16T03:39:20.292Z Reads: 24

```
it can be done.
but I don't think that part of the uart protocol was implemented by anyone yet. so you'd have to write that up on your own.

just the write config method i think. haven't look at vesc code for a while...
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-16T03:42:29.576Z Reads: 21

```
I don't know a single code about uart protocol 😂
```

---

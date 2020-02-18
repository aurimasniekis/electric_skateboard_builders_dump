# HELP! Motor issues?

### Replies: 12 Views: 419

## \#1 Posted by: John_Doe Posted at: 2017-12-05T20:22:39.419Z Reads: 69

```
Firstly, I would suggest turning down your volume before you check out the video below. (2 are VERY loud, I apologize for that)
The setup:
12S5P Samsung 30Q's Hooked up to a BESTECH BMS
2 Maytech 60A VESC
2 Maytech 170KV (6374) motors
FLYSKY Receiver and transmitter

The issue: The motors are not rotating when the remote sends a signal. 
I'm not exactly sure what I did wrong in setting up the VESC's but here's how I troubleshooted. 
I checked to see if the VESC was receiving the signal correctly from the remote ([This is loud](https://streamable.com/hiang))
Next I checked to see if the VESC was working correctly([Not loud](https://streamable.com/ll79e))
And this is what happens when I attempt to control the motor with the remote ([Loudest](https://streamable.com/kdysg))
Any advice would be greatly appreciated.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-12-05T20:34:05.517Z Reads: 61

```
First of all, it looks like your throttle is reversed. The small slide switch (there are two) on the remote board will reverse that.

It also looks like you haven't set your PPM endpoints.

I'd guess you didn't apply the motor detection results after doing the detection. If you don't click "apply" and then "write configuration" you haven't done anything to the settings.
```

---
## \#4 Posted by: John_Doe Posted at: 2017-12-05T20:43:41.688Z Reads: 49

```
I have applied the motor settings, I just did the detection again for demo purposes to show that it is working. Thanks for the tip on the remote though.

Also could you explain what you mean when you say PPM end points? Thanks :)
```

---
## \#5 Posted by: John_Doe Posted at: 2017-12-05T20:48:27.204Z Reads: 48

```
nvm, you were write i guess i didnt apply the settings, thanks :)
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-12-05T20:51:10.363Z Reads: 46

```
The signal coming from the receiver is a series of pulses. The length of the pulses is used to tell the vesc what to do. You have to program the vesc with the "endpoints" of the remote, as in, at full throttle the pulse will be X long, and at full brake the pulses will be Y long. Good starting values are 2000ms and 1000ms. You can use the BLDC tool to read what the vesc is actually receiving, and adjust accordingly.
```

---
## \#7 Posted by: John_Doe Posted at: 2017-12-05T20:54:32.840Z Reads: 41

```
How would I go about reversing the direction of the motor?
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-12-05T20:56:50.544Z Reads: 41

```
<img src="/uploads/db1493/original/3X/e/4/e439fbdabde2c06754c6d5c11239f3fdfbfe12e8.jpg" width="690" height="370">

Flip the switch marked "reverse throttle."
```

---
## \#9 Posted by: John_Doe Posted at: 2017-12-05T21:00:27.147Z Reads: 38

```
When I hit reverse throttle it just flips the transmitted value not the direction of the motor.
```

---
## \#10 Posted by: MysticalDork Posted at: 2017-12-05T21:01:51.948Z Reads: 34

```
That's what you want. To reverse the motor direction, swap any two of the three wires going to it.
```

---
## \#11 Posted by: John_Doe Posted at: 2017-12-05T21:03:57.107Z Reads: 32

```
thanks that worked :)
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-12-05T21:06:05.819Z Reads: 29

```
Glad to help. I'll be unresponsive for a while, lunch break is over. I'll check back later if you have any questions.
```

---
## \#13 Posted by: Big_belly_sean Posted at: 2018-10-26T10:39:11.097Z Reads: 12

```
hi i need help picking a motor i am 100 kg i have had a 200kv motor but it makes weird sounds when i go faster any help
```

---

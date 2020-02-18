# VESC Configuration: Only full throttle or off. Please help

### Replies: 16 Views: 2302

## \#1 Posted by: kampfhahn Posted at: 2016-07-16T17:48:26.220Z Reads: 219

```
At the moment i´m trying to configure my VESC. Unfortunately it doesn´t work well.

Setup: 5S / Alien Power Systems 190 KV 6355 sensorless / Winning Micro Remote

I ran the motor detection and applied the correct detected settings to the "sensorless - commutation mode" area in the BLDC tool. Also the remote is set perfectly to match 0-50-100%.

When i start to accelerate, the motor immediately runs up to the 5S max ERPM of about 25k. I can´t dose the amount of power, only on/off.

Can anyone help?
```

---
## \#2 Posted by: GhettoFab.rictation Posted at: 2016-07-16T18:03:08.512Z Reads: 216

```
Use a voltmeter to test your circuit board, then if that checks out maybe ask whoever you purchased it from to help vise versa.
```

---
## \#3 Posted by: kampfhahn Posted at: 2016-07-16T18:05:37.499Z Reads: 210

```
I think it´s just a setup issue. I can set every ERPM i want in the control section of the BLDC tool just not with the remote. I also tested an other RC-Remote with the same result.
```

---
## \#4 Posted by: devin Posted at: 2016-07-16T18:35:42.360Z Reads: 197

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: GhettoFab.rictation Posted at: 2016-07-16T19:01:31.693Z Reads: 186

```
If you're bench testing it, there should be a programed button that tests the motor in your bldc
```

---
## \#6 Posted by: mccloed Posted at: 2016-07-16T19:07:47.574Z Reads: 183

```
@devin is correct. Once you install the motor and VESC on your board and put load on it the VESC will act different.
```

---
## \#7 Posted by: onloop Posted at: 2016-07-17T01:06:09.350Z Reads: 175

```
Is this result when bench testing or riding? Do you have "current control" selected?
```

---
## \#8 Posted by: cmatson Posted at: 2016-07-17T02:40:23.775Z Reads: 165

```
bench testing will make the motor go full forward with only 5% throttle. 

once you step on it though, it will be much more progressive!
```

---
## \#9 Posted by: kampfhahn Posted at: 2016-07-17T07:52:11.536Z Reads: 152

```
Thanks everyone. Riding the board the VESC works as desired. Now im angry that i spent about an hour for this. Is it a bug or a feature?
```

---
## \#10 Posted by: GhettoFab.rictation Posted at: 2016-07-17T09:08:43.641Z Reads: 147

```
I think it's just the way a brushless motor is set up to make it run this way, that's why amp and kv play very important roles. The amount of wire and "poles" and type of wire are getting a little more in depth about it. Efficiency wise these brushless are the way to go. I don't think it has anything to do with the vesc. Someone correct me if this is wrong though.
```

---
## \#11 Posted by: kampfhahn Posted at: 2016-07-17T13:40:11.452Z Reads: 134

```
Thanks for the explanation. But why is it possible to set any ERPM in the control section of the BLDC tool without load then?
```

---
## \#12 Posted by: Nordle Posted at: 2016-07-17T13:45:24.697Z Reads: 129

```
Select ''Duty cycle'' instead of ''Current'' in your PPM tab. Then you should can do what you desire.
```

---
## \#13 Posted by: kampfhahn Posted at: 2016-07-17T14:03:53.950Z Reads: 127

```
I'll give it a try. Do i have to change it back to current before riding then?
```

---
## \#14 Posted by: Nordle Posted at: 2016-07-17T14:04:34.851Z Reads: 128

```
Dunno exactly, i think u can ride it.
```

---
## \#15 Posted by: onloop Posted at: 2016-07-17T14:57:57.182Z Reads: 122

```
The VESC electronic speed controller uses current to control the motor speed. However, if there is no load on the motor a small amount of current will make it easily spin up to maximum rpm.

If you are cruising along flat ground at a steady speed with the trigger at 80% throttle & you maintain that 80% and start up an incline your speed will slow but the motor current will stay the same. Because the trigger controls the current.

Therefore to maintain speed up the incline you would need to apply more throttle/current to counter the load.

With hobby grade esc, if you have your trigger at 80% throttle and approach the same incline as above your esc & motor will actually try to maintain your original speed. If the incline increases more, more current will automatically drawn to maintain that speed. Most hobby esc don't have current limits though so tend to fail if you keep pushing them hard as they just keep pulling current.

With the vesc if you don't increase the throttle and the load increases enough you will slow down and eventually stall the motor.

Vedder has said current controll seems more intuitive. Not sure I agree with that 100% but either way current control is nothing to be concerned about. The end result is basically the same.
```

---
## \#16 Posted by: mcfly777 Posted at: 2016-07-17T15:03:16.547Z Reads: 114

```
I think the reason Vedder believes current control is more intuitive is that it parallels a regular car throttle. To go up a hill you have to push harder. I haven't tested which setup is smoother for acceleration though...might make a difference.

Leo
```

---

# VESC ABS over current

### Replies: 15 Views: 2805

## \#1 Posted by: Emerson Posted at: 2017-03-21T17:13:05.816Z Reads: 304

```
Hey everyone,
   I have a TB Vesc that is acting up.  Currently running FOC and I can run low speed for a little while just fine but then it just drops the power completely...seems to reboot the vesc then start again.  Any reason why I would hit an over current?  I'm running Bat and Motor max at 70.  

Board Specs:
10s3p battery from the last US group buy (with BMS)
Vesc from TB (With Ack's firmware)
Enertion 6372 motor/mount
Benchwheel Remote
97mm wheels

I can post my vesc settings if that would help.  Any advice?



<img src="/uploads/db1493/original/3X/1/8/1833301a92acf5e366452244be304c5cdc740159.png" width="281" height="500">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-21T17:37:29.399Z Reads: 281

```
Sounds like you have your battery current set too high. 70a seems too high for battery current.
Drop it down to 40 or 50 and try it
```

---
## \#3 Posted by: PXSS Posted at: 2017-03-21T23:41:33.223Z Reads: 268

```
Can you post your VESC settings?
As Namasaki said, your power settings are most likely wrong.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-03-22T02:07:06.030Z Reads: 262

```
I guess you set "Absolute max" in the motor settings also to 70.
Set it to 130 A. And also enable "Slow absolute max".

But just post screenshots of your settings from the Motor, FOC, Advanced and the remote tab.

Cool that you use my app.
```

---
## \#5 Posted by: Emerson Posted at: 2017-03-22T11:38:56.853Z Reads: 245

```
<img src="/uploads/db1493/original/3X/b/5/b5d009af2b58c838473025291873083d3face63d.JPG" width="690" height="447"><img src="/uploads/db1493/original/3X/b/7/b7fd9f9c83e83823570b446f00c134b1f5f25569.JPG" width="690" height="448"><img src="/uploads/db1493/original/3X/3/3/33b02938039a675477582616f5316541dbd6042c.JPG" width="690" height="448"><img src="/uploads/db1493/original/3X/e/b/eb3e78c3c50bf116e8f8c4bff4f6bec6ac313bd5.JPG" width="690" height="449"><img src="/uploads/db1493/original/3X/4/6/462c42326dd5df7e0a5b38179cf7a3fc160a43b4.JPG" width="690" height="447">
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-03-22T11:43:30.887Z Reads: 210

```
If you´re running a 10s3p with 25r cells you should trim that battery max down! 70A is too much for them.
25r are able to deliver 20A max, so 3x 20A are 60A max. But you should leave room, so get that down to 40A to be safe or 50A if you really need that punch.
```

---
## \#7 Posted by: Emerson Posted at: 2017-03-22T11:45:44.342Z Reads: 213

```
Totally makes sense...I don't know what I was thinking with 70.  Dropping that down to 40 for sure...I'll just create a profile at 50 using the @Ackmaniac App to see the difference.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-03-22T11:59:14.355Z Reads: 211

```
Set your battery cutoff start to 30V and the cutoff end to 28V for your 10S li-ion Battery.

But it doesn't make sense that you get a Overcurrent Error with 130 A as absolute max. Because the current when the error happened was below 130. So did you change it in the settings back to 130 A or was it at 130 A when the error happened?
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-03-22T12:02:57.522Z Reads: 204

```
there was a case like this before if i remember correctly that you have errors sometimes if you run high, identical bat/motor settings. So 70A Bat and 70A motor could have caused that problem.
@Emerson try it pls with the new settings and report back here.
```

---
## \#10 Posted by: Montiey Posted at: 2017-03-22T12:25:16.829Z Reads: 200

```
ABS Max is key for letting the VESC handle hard brakes of accelerations. It will adjust it's power and control where the current flows to make sure that the battery nor the motor exceeds set limits, but that doesn't happen instantly, and current spikes can occur at random- ABS max needs to be high enough so the VESC's current ramping has a good ceiling to work under.
```

---
## \#11 Posted by: Pimousse Posted at: 2017-03-22T12:33:35.131Z Reads: 185

```
I already had this error pushing high the current limit too.
It was on bench when I triggered it, so really no load but I hit a peak of 132A.
Since I came back to 50A, I never had this problem again. ;)
```

---
## \#12 Posted by: Emerson Posted at: 2017-03-22T12:55:15.895Z Reads: 177

```
It was always set to 130.  I'll give the new settings a try and report back.
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-03-22T14:21:36.052Z Reads: 175

```
Right, it's just there to protect the VESC from spikes or when something goes wrong. So this definitely should be higher than Motor max.
130 is a good value.
When you **enable** "Slow absolute max" then it throws a error when **Current filtered** is above absolut max.
When you **disable** "Slow absolute max" then it throws a error when **Current** is above absolut max.
And when the error is logged it detects again the actual current. So it could be a bit off (<1ms) to the moment when the error happened.
```

---
## \#14 Posted by: Emerson Posted at: 2017-03-22T14:39:32.096Z Reads: 169

```
Fun fact:  When I had most of the settings in BLDC instead of FOC the error required power reset in order to control the board.  While in FOC the error will occur but then only drop the receiver for a few seconds.
```

---
## \#15 Posted by: Ackmaniac Posted at: 2017-03-22T14:55:02.549Z Reads: 164

```
Just lower the currents that you use and see if it get's better. And also enable "Define Max Watt" and set max watts to 36V * batter max.

So if battery max is set to 40A then it would be 36V * 40 A = 1440W

But to me it seems that your VESC has issues to detect the actual current correctly. So just by lowering the values it will get better. And i recommend to not use FOC as long as you have these issues.
```

---

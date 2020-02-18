# Motor Throttle Help

### Replies: 13 Views: 736

## \#1 Posted by: nadir35 Posted at: 2017-03-26T17:50:30.325Z Reads: 83

```
Hi guys,

I am currently doing my first build and I am experiencing the following problem:
The motor throttle seems to burst randomly, especially at low throttle values. (video: https://drive.google.com/file/d/0B5qHMcrmYIvbalFQQTFqYlpLRkE/view )

My Setup:

* SK-3 6364 245kv
* Hobbyking X-Car Beast 120A
* Arduino Nano + Bluetooth as receiver for ESC (code: http://pastebin.com/MmBQbXGj)

I have doublechecked the values transmitted to and received by the arduino, but these do not show any irregularities.
Does anyone have a clue what could be going wrong here? Much obliged.
```

---
## \#2 Posted by: JLabs Posted at: 2017-03-26T18:01:41.828Z Reads: 77

```
Are you expirencing the same problem with a normal rc remote and receiver?
```

---
## \#3 Posted by: nadir35 Posted at: 2017-03-26T18:02:40.579Z Reads: 77

```
sadly I don't own a normal set, so I can't tell
```

---
## \#4 Posted by: JLabs Posted at: 2017-03-26T18:03:36.310Z Reads: 71

```
I would buy the cheapest thing you can find or borrow a friends to test. If it works good with a normal rc remote than the arguing code is the problem.
```

---
## \#5 Posted by: nadir35 Posted at: 2017-03-26T18:05:08.806Z Reads: 68

```
yeah I figured that that would be a next step. I will try to hook up a potentiometer instead of the bluetooth communication tomorrow and see if the problem persists
```

---
## \#6 Posted by: Sander Posted at: 2017-03-26T18:48:37.404Z Reads: 57

```
The code is wrong.
```

---
## \#7 Posted by: Sander Posted at: 2017-03-26T18:52:35.921Z Reads: 56

```
Change the code with SoftwareServo.  
SoftwareServo is inbuilt already, i think. If not [download it here.](https://www.dropbox.com/sh/vak0vhc9efa2pry/AABCaS4pIFS0CW1-BlZzkpcma?dl=0)
> (hashtag)include "SoftwareServo.h"
> SoftwareServo ESC;

> void setup(){
> ESC.setMinimumPulse(800); //800
> ESC.setMaximumPulse(2000); //2000
> }

Here you change the values, you need to have the softwareservo refresh thing.
> ESC.write(value);
> SoftwareServo::refresh();
```

---
## \#8 Posted by: nadir35 Posted at: 2017-03-26T19:27:37.562Z Reads: 48

```
thanks, I'll give it a try
```

---
## \#9 Posted by: Sander Posted at: 2017-03-27T08:44:33.288Z Reads: 39

```
and the values are from 0-180 i believe
```

---
## \#10 Posted by: nadir35 Posted at: 2017-03-27T14:57:35.281Z Reads: 36

```
I've tried to make it work yesterday  with the SoftwareServo library yesterday to no avail ( ESC wouldn't set the min. throttle properly, probably should try with other values than 800)  and after reading a little bit about the reliability problems of self-made bluetooth solutions I've decided to go forward with a conventional car remote. I guess the app + Arduino setup was more for testing purposes anyways, don't think that riding around with a smartphone in hand would be a good idea :smile: 

Thanks for the fast replies.
```

---
## \#11 Posted by: Sander Posted at: 2017-03-27T17:49:36.393Z Reads: 26

```
Hehe, but did you calibrate your ESC?
```

---
## \#12 Posted by: nadir35 Posted at: 2017-03-27T18:57:54.941Z Reads: 21

```
During calibration I could set the max throttle while transmitting 2000, but when setting the min throttle of 800 the esc wouldnt take it and just did nothing.
```

---
## \#13 Posted by: Sander Posted at: 2017-03-28T09:02:47.825Z Reads: 14

```
 hange the values? from 2000 to 3800?
```

---

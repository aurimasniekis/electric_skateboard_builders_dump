# Help Smoothing Out R-Spec with VESC

### Replies: 14 Views: 2304

## \#1 Posted by: lilracerboi Posted at: 2016-05-14T03:31:42.476Z Reads: 144

```
I just got the VESC yesterday and have been playing around with it, but I can't seem to get it to the point where I can take off smoothly as well as transition from forward to backward smoothly. Similar to the Boosted Board, if that's even possible.

I still don't quite get how the parameters work.

Edit: It can actually take off from a stop, but it's not particularly great at it.
```

---
## \#2 Posted by: Blasto Posted at: 2016-05-14T03:50:47.212Z Reads: 144

```
I don't have the exact answer to your question, but those who do, will want to know your motor setup, battery setup, pulley setup etc... Oh and the type of remote you're using
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-05-14T05:52:45.779Z Reads: 132

```
Have you read:

 http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980?u=michaelinvegas


[quote="evoheyax, post:1, topic:2980"]
VESCNow, onto the configuring itself. Here is an article explaining what you need to modify to get your vesc running.
[/quote]
```

---
## \#4 Posted by: lilracerboi Posted at: 2016-05-14T06:19:02.922Z Reads: 128

```
Here's my setup:
Motor: Enertion R-Spec 2.0 6355
ESC: VESC HW 4.12 FW 2.16
Batteries: 6S 20C Zippy Lipos

@Michaelinvegas Yeah, I've been referring myself back to that thread since I got my VESC and it's helped out a lot.
I mean, the VESC is already way smoother from a stop than say, the HobbyWing 120A ESC, but can it get any more smoother? Can it be Boosted Board smooth?
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-05-14T06:21:09.016Z Reads: 116

```
You gotta get a vesc/r-spec person that has a simlar setup to see if they have it tuned in
```

---
## \#6 Posted by: lilracerboi Posted at: 2016-05-14T06:28:18.779Z Reads: 113

```
I found a configuration file for the R-Spec 6355 in the mc_configurations folder located [here](http://vesc.net.au/BLDC-TOOL/Firmware/Motor%20configuration/).
It's not much different than my original setup, though it did allow me to use FOC since my motor detection in FOC is not working (not giving a lambda value).
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-05-14T06:32:02.829Z Reads: 110

```
This is beyond me...

Hopefully someone will chime in on this and help you get some diffrent settings
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-05-14T06:34:20.241Z Reads: 113

```
Just modified the title mate...make it a little clearer
```

---
## \#9 Posted by: lilracerboi Posted at: 2016-05-14T06:35:31.236Z Reads: 110

```
Hey thanks. Yeah, it was pretty unclear.
```

---
## \#10 Posted by: Iceni Posted at: 2016-05-14T09:33:18.160Z Reads: 100

```
Not sure about the specs of the boosted, but it might run sensored motors (correct me if I'm wrong) which helps tremendously with startup smoothness.

The r-spec is unsensored, which makes it a little less smooth on start from a standstill compared to a sensored setup.
My recommendation is to kick-start, to reduce the strain of the components.
```

---
## \#11 Posted by: evoheyax Posted at: 2016-05-14T17:46:39.843Z Reads: 82

```
I'm not sure about the r-spec, never ran it with the vesc in FOC. What I can say is, in FOC, you can get great start up. With hummies motors in FOC, I can start from stop with great power.

But the boosted has that initial punch due to the motors being sensored. It will always be hard for a not sensored motor to compete with a sensored motor in start up, but he vesc in FOC is your best choice, and should get you pretty darn close.
```

---
## \#12 Posted by: lilracerboi Posted at: 2016-05-14T21:10:36.431Z Reads: 76

```
Right, I forgot to factor in sensored and sensorless motors.
Makes a lot for sense now.

I don't really like to use FOC at the moment since the motor detection in FOC mode isn't working. To get it to work, I have to use the preconfigured XML configuration for the motor and I've noticed it isn't better at start up than BLDC.
```

---
## \#13 Posted by: EnertionSupport Posted at: 2016-05-14T22:33:32.379Z Reads: 72

```
The setup will never be Boosted smooth due to the lack of sensors. 

That said, if you just give the motor enough power (rather than barely pressing the throttle and watching the motor jitter) it will start right up. Without the sensors it has a harder time starting at a really low creep as @evoheyax mentioned. But what the R-Spec lacks in sensors like Boosted, it more than makes up for in overall torque. 

But remember, one little push would solve all of your issues, not to mention it's easier to balance with a simply push off- much like riding a bike,  initial rolling momentum can help a lot!
```

---
## \#14 Posted by: lilracerboi Posted at: 2016-05-14T23:32:43.888Z Reads: 63

```
Even though I have the VESC now, I still push to put less strain on the components.
The power to not have to push at really low speeds is helpful when, for whatever reason (sidewalk traffic, etc.), I have to slow down. In some situations with no room to push.

How does a Boosted Board compare to a sensored setup?
```

---

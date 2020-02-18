# Constant speed setting for VESC

### Replies: 10 Views: 304

## \#1 Posted by: murdomeek Posted at: 2019-02-16T08:26:11.433Z Reads: 74

```
Still new with VESC's and I cant seem to find anything regarding my specific problem.  

I longboard dance, and I would like to make an electric dancer build.  When I am dancing, it is difficult to keep the speed constant controlling with the throttle while flinging my arms about and shifting my center of gravity drastically on the board.  It would be easier to keep the throttle at max.  But obviously I cant dance at 40km/h.  

Is it possible in the VESC settings to set the motors to go at a constant speed at max throttle? (10km/h = ~25% of max speed)  And when the voltage dips throughout, it stays at 10km/h until the voltage is too low to physically support that. 

This scenario doesn't need to account for hills, because dancing is usually on flat ground anyways.

I have only had experience with the generic chinese esc's with the "4 mode remote".  However, even with "mode 2", the speed decreases proportionally with the voltage level as time goes on.  

Thanks!
```

---
## \#2 Posted by: b264 Posted at: 2019-02-16T08:31:52.862Z Reads: 69

```
I do know the "PID Speed control" VESC app contains the functionality you want, but I don't know anything about it because I've never used it.
```

---
## \#3 Posted by: Friskies Posted at: 2019-02-16T09:04:41.543Z Reads: 62

```
If you have Metr you could make a profile with speed limited to 10kmh and then switch to it when you are dancing. Then all you need is to full throttle.
```

---
## \#4 Posted by: amazingdave Posted at: 2019-02-16T09:28:07.551Z Reads: 57

```
Second the metr suggestion... it is stable at holding the speed at whatever you like... I use it for my kids, a different speed for each.
```

---
## \#5 Posted by: rich Posted at: 2019-02-16T09:34:05.910Z Reads: 54

```
[quote="murdomeek, post:1, topic:84350"]
electric dancer build
[/quote]

Haha great, you should change the thread name to this :grinning:

I also think modes are the way to go, so you can ride faster if needed and change to the "dancing mode" on the fly.

The new Vesc-Tool mobile app has modes, too where you can limit to e.g. 10km/h.
```

---
## \#6 Posted by: rich Posted at: 2019-02-16T09:51:30.259Z Reads: 52

```
[quote="amazingdave, post:4, topic:84350"]
it is stable at holding the speed at whatever you like… I use it for my kids, a different speed for each.
[/quote]

Wait.... now I'm interested, too. That sounds like almost real cruise control. If you set it to e.g. 20km/h does that mean if you ride uphill the motors turn faster to stay at 20km/h? 
Also the throttle is like a dead man switch if you release full throttle.
```

---
## \#7 Posted by: amazingdave Posted at: 2019-02-16T13:23:56.300Z Reads: 41

```
Yes to the speed hold up a hill, as you release the throttle it doesn’t slow until the throttle passes the speed limit set in metr...
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-02-16T13:45:05.019Z Reads: 38

```
If you are using any arduino based remote you can assign any button to be cruise control, it will keep the speed no matter what
```

---
## \#9 Posted by: murdomeek Posted at: 2019-02-16T17:17:38.368Z Reads: 30

```
thanks for all the suggestions guys! :slight_smile:
I'll definitely look into all those!
```

---
## \#10 Posted by: deucesdown Posted at: 2019-02-16T17:20:39.529Z Reads: 30

```
[quote="murdomeek, post:1, topic:84350"]
dancing
[/quote]

https://www.electric-skateboard.builders/t/esk8tube-video-thread/47/2029?u=deucesdown

Of coure @rich is already in the thread :)
```

---

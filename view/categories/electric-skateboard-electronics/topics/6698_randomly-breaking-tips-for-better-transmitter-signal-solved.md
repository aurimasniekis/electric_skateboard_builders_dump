# Randomly Breaking. Tips for better transmitter signal? (SOLVED)

### Replies: 12 Views: 1341

## \#1 Posted by: Brando Posted at: 2016-07-27T15:43:37.867Z Reads: 112

```
I have been having loads of fun riding my week old board around, but every so often, the board will just start breaking. I'm fairly confident that this is an electrical problem, and not a mechanical jam somewhere because I can hear the motor's breaking sound when it randomly slows down. I'm using the winning mini remote purchased [here](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/). I'm surprised because I heard good things about this remote's signal. could it be my esc overheating and automatically breaking? [This is my ESC](diy-electric-skateboard-kits-parts/single-motor-120a-6s-esc/) and it has a fan constantly running so that seems less likely.
Also, the receiver that came with my remote doesn't have a antenna, which seems uncommon as most receivers have an external antenna.
FYI I live in a suburban area where every house has WiFi most likely transmitting.
```

---
## \#2 Posted by: Stevemk14ebr Posted at: 2016-07-27T15:46:09.460Z Reads: 115

```
If two motor wires short together the motor will brake. Check all your motor wire connects and make sure they are insulated
```

---
## \#3 Posted by: Brando Posted at: 2016-07-27T15:46:43.612Z Reads: 116

```
Thanks. I'll look and upload some pictures
```

---
## \#4 Posted by: elkick Posted at: 2016-07-27T15:54:26.620Z Reads: 111

```
That's a very common problem with the winning remote: the default "fail safe" is sometimes set to full brake in case of loosing connection and that's not good! Did you test the fail safe function yet? 

Here are some steps I collected a while ago: 

Please test the fail-safe functionality (like moving the transmitter as far away from the board and checking if the motor shuts down if out of reach). If the motors doesn’t shut down or applies brakes, please perform the following steps for binding and calibrating:


1.     Check and make sure all the wires are connected and that the REMOTE is OFF. Insert the bind plug into CH3(Bind) on the RECEIVER.

2.     With the REMOTE OFF: switch on the ESC to power up the RECEIVER, the red LED light will flash.

3.     PRESS and HOLD the bind button on the REMOTE and then turn the REMOTE ON.

4.     You should notice the REMOTE and RECEIVER LED light go from flashing red to solid red.

5.     Once you see a solid red light, the binding process is complete. Then without turning the REMOTE OFF or touching the THROTTLE pull the bind plug out (for the receiver to record the throttle mid point, neutral, to engage the fail safe)

6.     Then you can test it again by turning OFF the REMOTE and the RECEIVER LED should flash. By turning the REMOTE ON the RECEIVER LED should go back to solid red.

7.     Before riding, it's better to test the fail safe functionality again. Leave the board powered on and switch the REMOTE off: if the motor isn’t moving, the fail safe function is working, if the motor is moving fast or abruptly braking while throttle is applied: you have to repeat step No.1- No.6
```

---
## \#5 Posted by: Brando Posted at: 2016-07-27T16:02:42.994Z Reads: 97

```
Thanks so much for the detailed instructions! I'll do that now. I have tested the fail safe by just turning off my remote and the motor indeed breaks. I had no idea I could set the fail safe to just coast.
```

---
## \#6 Posted by: Maxid Posted at: 2016-07-27T16:07:18.552Z Reads: 91

```
Does that apply to a GT2B as well? My motor goes into reverse when the transmitter is shut off before the board is turned off.
```

---
## \#7 Posted by: elkick Posted at: 2016-07-27T16:10:20.731Z Reads: 89

```
Probably yes, at least it's worth to try fail safe functionality with every new remote you connect. There are some specific YT videos out there for GT2B fail safe procedure, but I remember it being quite similar to the winning remote.
```

---
## \#8 Posted by: Brando Posted at: 2016-07-27T16:18:27.105Z Reads: 80

```
@elkick Thanks so much! the fail safe is set to neutral now.
```

---
## \#9 Posted by: elkick Posted at: 2016-07-27T17:21:11.699Z Reads: 77

```
@torqueboards, maybe you should copy the above text and paste it into your product description. :slight_smile:  

It's sort of a dangerous default setting which needs to be known by the customers - did the same on my HP :wink:
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-27T17:28:26.987Z Reads: 77

```
I don't know about torqueboards, but the controller I got from @Kaly has paper with instructions on how to rebind and calibrate.
```

---
## \#11 Posted by: Justin Posted at: 2016-07-27T18:15:03.754Z Reads: 70

```
So people do experience connection problems with the Winning remotes? That on its one is a thing to worry about. Also don't want to be a nitpicker but don't you guys mean 'braking'?

https://www.youtube.com/watch?v=ZpUYjpKg9KY
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-27T18:17:08.959Z Reads: 66

```
I've noticed this a million times on here and the r/electricskateboarding subreddit. Not sure why so many people mix up 'braking' and 'breaking'. I was started to question my own definition of the word :smile:. I haven't used it extensively yet, but so far it seems to be good. Jason from Enertion has been using it with his personal Raptor and is about to start selling it, so I'm assuming it's reliable enough.
```

---

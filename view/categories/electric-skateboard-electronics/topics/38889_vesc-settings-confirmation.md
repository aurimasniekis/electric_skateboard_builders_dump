# VESC Settings Confirmation

### Replies: 5 Views: 823

## \#1 Posted by: maxhost4 Posted at: 2017-11-21T08:43:43.517Z Reads: 109

```
Hey all,

I'm currently in the final stages of completing my first build. The final step this evening was to configure the VESC, and I think I've done it correctly (I think). I would love some feedback/affirmation on my settings before I attempt to ride the board tomorrow. 

I'm currently using:
-A single 6374 190 kv motor from torqueboards
-A 10s2p LiPo battery pack composed of 4 5s, 20C, 3Ah LiPo cells
-VESC from torqueboards (V. 4.12 w/ firmware 2.18)
-Torqueboards Nano remote (2.4Ghz).

If any of my settings look horrendous or even could be improved slightly, I'd love to hear y'all's thoughts. If you need more screenshots or other info, please let me know. Additionally, if there's anything I should watch out for/keep an eye on with my set-up, I'd very much appreciate any words of wisdom.

I promise I'll get a full post about this build up soon. As always, any and all thoughts, comments, concerns, etc. are greatly appreciated.

-MH

<img src="/uploads/db1493/original/3X/0/0/002e07b12585fbb10dbcffd084198fb9d02ee961.png" width="690" height="387"><img src="/uploads/db1493/original/3X/5/5/558823e113d83c4e551ced49d76309afaeb89246.png" width="690" height="387"><img src="/uploads/db1493/original/3X/0/e/0e031c8e0a09ee9c71ae20b2fc55e2a551a5f03f.png" width="690" height="387"><img src="/uploads/db1493/original/3X/b/7/b7e37f163116dca0c1b71aeef8261b66067245e7.png" width="690" height="387"><img src="/uploads/db1493/original/3X/a/2/a29748657c1bdd83f9cc3031b85a438d8dd49e83.png" width="690" height="387">
```

---
## \#2 Posted by: lasplaner Posted at: 2017-11-21T10:47:55.128Z Reads: 80

```
Relatively good!

Is your Minimum/Maximum Pulsewidth set by yourself, or default? If default, switch the setting to "Disabled", write configuration, and click the check box in "Display". Then make sure your remote is connected, and adjust the Min/Max, as you rock your controller from the forward position to the backwards position. Then set back to current control with brake, and write configuration again.

Batt min looks awfully low. For this pack, you could afford to probably increase to 12A (2C), unless the battery specific states it cannot be charged at this rate.

Also in your Motor Configuration, check the checkbox for Soft RPM limit, and change the ERPM limit start and ERPM limit end to 55,000 and 60,000 respectively. Don't kill your DRV Chip!

I notice that your hall sensors are not on. Use them! For BLDC (the mode you are using), this how to set it up: (Optional)

1. Connect the Sensor wires (if it doesn't connect to VESC you need an adapter).
2. In BLDC tool, detect the motors again, and copy the detection results for the Hall sensors into the Hall Sensor table.
3. Click _"Hybrid"_ on the top left, and change Sensorless ERPM (hybrid mode) into a value in the neighbourhood of 3000-5000 ERPM.
<img src="/uploads/db1493/original/3X/f/0/f0c033bd6e534eea2a237f1cc602f4cda463911f.png" width="690" height="359">

Also, you have the capability of using FOC mode, but run with BLDC for 50-100km or so, before you switch. Especially considering that you are running a high voltage (10S).

ALSO, I do not take responsibility for these settings. If you get it wrong, no harsh feelings, not my fault! That being said, you should be ok with these adjustments.

-lasplaner
```

---
## \#3 Posted by: maxhost4 Posted at: 2017-11-21T16:17:36.563Z Reads: 65

```
Thanks so much for the tips- I was trying to figure out how to adjust the controller settings. And I do have the Hall sensors- the plan is to get an adapter and run in hybrid sensors/senseless mode. Until I get an adapter however, it’s sensorless. Thanks again for the advice. 

-MH
```

---
## \#4 Posted by: lasplaner Posted at: 2017-11-21T20:12:12.835Z Reads: 54

```
[quote="maxhost4, post:3, topic:38889"]
I was trying to figure out how to adjust the controller settings.
[/quote]
Do you know now? It is the PPM part.

Also, sensored motors run much better at lower speeds. Give it a try!
```

---
## \#5 Posted by: maxhost4 Posted at: 2017-11-21T22:51:18.087Z Reads: 46

```
I got everything figured out. Thanks again man.
```

---

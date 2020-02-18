# FOCBOX Motor Detection Issue: Motor not responding, Bad detection results received

### Replies: 1 Views: 276

## \#1 Posted by: eshnell Posted at: 2018-09-14T03:25:43.118Z Reads: 81

```
Hey Everyone!

I apologize, there are many similar topics on the site; however, none of the solutions I have found have worked.

A few days ago I setup my 2 new focboxs for a dual board.  I successfully completed each setup and calibration using the enertion BLDC tool then linked the two via CAN bus.  After doing that, I went to test the setup untethered before adding it to the board, but only the slave motor would run when I throttled the remote (even then it would only pulse and then cut off until I released the throttle and applied it again).  I took it all apart and could not find a issue so I decided to redo the setup and motor detection to see if that would help.  This is where the real problem started.

After resetting the master to its default configuration I began motor detection under the FOC tab (sensored) but every time I went to measure R and L the FOCBOX would disconnect and the tool said "port disconnected".  It kinda looked like the FOCBOX was crashing as, while the green and blue light stayed lit, after a few seconds from disconnecting, the 3 red blinks that normally signal it turning on would flash.  I tried this multiple times and then also tried the hall sensors detection which gave feedback in the form "Bad detection results received" with no response from the motors.  I tried re-flashing the board and also tried setting it up BLDC, sensored and unsensored, but kept getting "bad detection results received" and no response from the motors when I tried any form of motor detection (though it would still only disconnect if I tried FOC R and L).  There are no shorts (board, wires, or motor), no signs of damage on the board, and all the solders look fine. I tried it on a different motor with no success.  The battery cutoffs are correct and I used the slave FOCBOX (which is working perfectly) to test everything hardware and software-wise.

I then downloaded the VESC tool, flashed their firmware, and tried the setup through there.  When I got the the FOC sensored detection and did R and L it would actually give me numbers but the motor would not make any noise, and when I detected lambda it also gave me a number without spinning.  These numbers were way too large to make sense (an order of magnitude or 2 so).  When I detected hall sensors or did a BLDC detection I would get a similar message to that of the Enertion BLDC tool, the "bad detection received".

I have tried modifying the BLDC- ERPM, Current, and duty values, tested it on multiple motors, tested the batteries and tested the same settings on another FOCBOX (which works).  I have provided pictures of the board in case you can see something I can't, and I can provide pictures of the settings if need be.  Any clue what may be wrong?

Some general specs:
Controllers:  Enertion Focboxs
Receiver: Enertion Nanox
Battery: 12S 2P (18650)
Motors: BRH5065 (Racestar) 200 KV  (no temperature sensor so you will notice that pin 5 on the focbox sensor input it missing)


Thanks in advance!

![20180913_195604|375x500](upload://8ickho4WDixX9DYTPAvRbd4N5FY.jpg)
![20180913_195545|375x500](upload://5ictLasQ9920O9JlgeouagXcYop.jpg)
```

---

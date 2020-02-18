# VESC ISSUES? Not responding but no DRV error

### Replies: 2 Views: 299

## \#1 Posted by: yakerman Posted at: 2017-06-11T12:06:49.169Z Reads: 46

```
Whilst riding my board yesterday it just lost power. At first I thought it may have been an issue with the receiver but when plugging it into bldc tool the motor still doesn't spin up. 

There are no errors showing in the real time tab or when I type faults into the terminal. At this point the pulse width display also still showed the receiver was working.

I updated the VESC firmware and tried to do motor detection in BLDC mode. Nothing happened and it said bad detection. Weirdly I can't seem to pair the receiver now either (nothing showing in pulse width display). The arrow keys don't spin the motor.

Can anyone help shed some light on this? I'm guessing my VESC might be broken but could it be the motor instead?  I think the cause of this could be from upgrading from 8s to 10s yesterday. Maybe I missed something when setting the board up. Although it ran fine for around 3 miles before this issue. I was running in FOC originally. I don't have a spare vesc or motor to test unfortunately.

Here's a screen shot from BLDC Tool <img src="/uploads/db1493/original/3X/2/1/21ceeedacfc1a30b9a5310db83ce7dd3c9ef0f2d.png" width="690" height="431">
```

---
## \#2 Posted by: Blasto Posted at: 2017-06-11T12:26:58.950Z Reads: 37

```
Is your max input voltage set at 57v?

Could your batteries been low when you were riding? Hit the low cut off?
```

---

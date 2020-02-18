# VESC - FAULT_CODE_DRV8302 - Cause?

### Replies: 6 Views: 779

## \#1 Posted by: ajsberger Posted at: 2017-05-18T20:49:14.230Z Reads: 80

```
Using the information in this forum, I built an electric longboard.  I am using a Spacecell Pro3 (10SP3) from Enertion and a 6355 190KV motor and VESC BLDC Speed Controller from http://.  I road 40 miles or so and then, earlier this week, the remote (torqueboards nano) just stopped responding.  I took the board apart and used the BLDC tool to see what was going on and found after typing "fault" into the terminal I was getting the DRV error.  I am working with  to see if they can help but I was hoping someone could look at my settings and see if I made an obvious error.  Nothing looks burnt on the board.<img src="/uploads/db1493/original/3X/b/5/b5b39b6f82e91d436f46eeb8d0ae42b4c9a2cf7c.jpg" width="690" height="386"><img src="/uploads/db1493/original/3X/4/4/44fa778611e619fab7f3d4ebb9f4490474583e85.jpg" width="690" height="312"><img src="/uploads/db1493/original/3X/d/0/d043d2efa4ba3666da68f9419ddd3cb540225c65.jpg" width="690" height="354"><img src="/uploads/db1493/original/3X/5/d/5da0b6624db73c6a2fb7f2121eada4a4b2f87be7.jpg" width="690" height="62">
```

---
## \#2 Posted by: ajsberger Posted at: 2017-05-20T03:47:38.538Z Reads: 52

```
anyone see anything off?
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-20T04:03:48.777Z Reads: 52

```
Can you post pictures of your vesc?
you might have a hardware issue and not a software issue.

Although, I'm not sure about running motor min at -80A  especially when your only outputting -6a to the battery.
```

---
## \#4 Posted by: ajsberger Posted at: 2017-05-20T04:45:29.694Z Reads: 50

```
I sent the vesc back to  http:// this morning, they are going to take a look since the vesc comes configured for my setup according to their website.  

Based on your comment, what would be a better value for the motor min?  I think this may be a hardware issue but i wanted to rule out an obvious setting issue.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-05-20T05:01:38.547Z Reads: 51

```
Well I'm not really qualified to give optimum settings for the Vesc, I just recall reading that the motor min and batt min should not be too far apart. I don't know if that theory still holds or not.
I run my motor max at 80a and motor min at -40a and batt min at -10a
I mostly use my brake to control speed or come to a gradual stop. I run my belts pretty loose which keeps me from slamming the brakes anyway.
Really I'm not even sure that your motor min setting could be causing any issues. And I didn't notice anything else wrong with your settings.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-20T05:04:16.730Z Reads: 51

```
When I said it could be a hardware issue, I meant that there could be a short somewhere on the vesc that caused the DRV fault. Motor phase wires shorting together can also cause a DRV fault.
```

---

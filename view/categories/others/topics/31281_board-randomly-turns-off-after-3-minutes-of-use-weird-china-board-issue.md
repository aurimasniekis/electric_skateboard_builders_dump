# Board randomly turns off after 3 minutes of use (weird China Board issue)

### Replies: 5 Views: 1311

## \#1 Posted by: frickingphil Posted at: 2017-08-22T20:06:54.137Z Reads: 101

```
Hi esk8 builders! 

I got a little Chinese penny board to mess around on\* and it's been a blast these past few weeks, but now it's got this completely random issue that I'm wondering if anyone's ever encountered before.

Here's the issue: **the board shuts off 3 minutes after I power it on, every time, regardless of what I'm doing with it for the duration of those 3 minutes.**

I've noticed that the auto-shutoff for when the board is idle is also exactly 3 minutes, so something must be not communicating to the ESC that the board is actually being used.

Things I have tested:

* Thought it was something to do with the power button, so I unplugged it while the board was on and running. Still turned off.
* Unplugging the hall sensor while running just causes the motor to seize, so I left that plugged in.
* The board has two speed modes, and neither have an effect on the issue.
* Tried known-good batteries in the remote, still no effect on issue. The board beeps constantly when the remote connection is lost, anyway.
* The board's battery charge level has no effect on the issue.
* Double-checked every connection to the ESC and made sure nothing conductive is shorting or touching the PCB.

It's almost like the board thinks it's idle the entire time and auto-shuts off, even if I'm riding it or not.
The board is, from what I can tell, a "Haitral"-brand board. Pic of ESC attached to bottom of post.

Figured I'd throw this out there in the off-chance that someone has actually had this same issue and/or had a fix.

<img src="/uploads/db1493/original/3X/8/4/8444e357227be352a4b9b5d7002017104504b92c.jpg" width="375" height="500">

\* = Yeah, I know, false economy, etc...I impulse-bought the thing for $65 on craigslist, so I'm not too beat up over the fact that it's acting up now. After a bit of research, I was most likely going to end up picking up a Meepo Penny Dual soon anyway, or building my own small cruiser based off a Landyachtz Dinghy deck, but figured I'd see if any ESC gurus were lurking here and could troubleshoot this odd (and kinda funny) issue.
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2017-08-23T16:28:22.375Z Reads: 66

```
it may not be worth your time to fix. alternatively you could swap the unit out with a more common esc and redo the wiring.. id salvage the motor and board w/battery, and redesign it.. could be fun!
```

---
## \#3 Posted by: frickingphil Posted at: 2017-08-23T17:55:22.291Z Reads: 58

```
True that. Are there any common ESC's that have integrated BMS (charging) and controller / receiver? Or are most of the DIY things all piecemeal? I've read up on the VESC and it seems like a great solution but a little overkill for a board that's probably going to get replaced soon...
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2017-08-23T18:28:02.128Z Reads: 49

```
look at diyelectric skateboards shop.. measure your cavity.. go with a vesc if you have the space..
if the deck is good, keep using it.. try to keep your costs down, then plan a really nice build, that wont be your first experiment.. (first time usually things go horribly awry and mistakes will be made)
```

---
## \#5 Posted by: Frankegold Posted at: 2018-09-26T17:28:21.763Z Reads: 19

```
I’m having the same problem. Did you find a solution? My thought is to get a new esc/controller and swap it out.
```

---

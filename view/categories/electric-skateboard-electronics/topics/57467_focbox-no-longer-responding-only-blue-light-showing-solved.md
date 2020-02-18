# FOCBOX no longer responding. Only blue light showing (Solved)

### Replies: 21 Views: 621

## \#1 Posted by: TinnieSinker Posted at: 2018-06-01T12:07:23.675Z Reads: 168

```
Hi folks, I'm at a bit of a loss here.

I finished my esk8 build two weeks ago and for the most part everything has been working fine. (build thread coming at some stage :smiley: ) 
Today while trying to get bluetooth to work, one of my two FOCBOX's stopped responding and is no longer recognized by the PC.
When powered, the blue light comes on, the red light flashes once faintly and no green light.
Its not recognized in the Device manager but in know the cable and everything else works because the other FOCBOX connects just fine.

I have spent a few hours reading but can't seem to find any other threads with this problem

Any help would be greatly appreciated
```

---
## \#2 Posted by: longhairedboy Posted at: 2018-06-01T13:40:17.052Z Reads: 158

```
I've seen this before. Not sure what caused it but it ended up in the @JohnnyMeduse bin.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2018-06-01T13:55:13.531Z Reads: 154

```
Is the Bluetooth still connected? 

Also, which firmware are you using?
```

---
## \#4 Posted by: TinnieSinker Posted at: 2018-06-01T15:04:58.833Z Reads: 140

```
BT is disconnected. I first noticed the problem after removing the cable.
the other focbox has been fine with the module

look like 3.38
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2018-06-01T15:09:59.727Z Reads: 139

```
Hummm... I think It could be a firmware Issue, you might need to reflash your vesc using a st-link.
```

---
## \#6 Posted by: trancejunkiexxl Posted at: 2018-06-01T17:43:04.576Z Reads: 123

```
Other ones poor smoke
```

---
## \#7 Posted by: jadatmag Posted at: 2018-06-01T20:31:37.241Z Reads: 119

```
I've had this kind of issue with my Raptor 2. Only under 50% battery though. Does battery percentage have anything to do with your issue?
```

---
## \#8 Posted by: CarlCollins Posted at: 2018-06-02T07:53:06.682Z Reads: 106

```
@TinnieSinker

Just want to know: your other FOCBOX connects to Windows without any issue?
Your other FOCBOX also have 3.3xx FW?
Your other one shows green light?
Have you connected them via CANBUS?
Have you disconnected the CANBUS once without removing it from both of the FOCBOX together?
```

---
## \#9 Posted by: TinnieSinker Posted at: 2018-06-02T12:16:03.992Z Reads: 101

```
Thats a Yes for all everything. They have both been working perfectly for 2 weeks.

Regarding the canbus. It was hot glued in place on both ends. I've only removed one end while trying to diagnose this problem. It's still plugged into the one that works, is that a bad thing?
```

---
## \#10 Posted by: TinnieSinker Posted at: 2018-06-02T12:16:42.170Z Reads: 96

```
Thanks, I'll look into that
```

---
## \#11 Posted by: CarlCollins Posted at: 2018-06-02T14:32:02.159Z Reads: 91

```
@TinnieSinker

OHHH! Man I think you just fried CAN transceiver of one of the FOCBOX.
It must be the one on which CANBUS cable stay connected.
@JohnnyMeduse What do you think?
```

---
## \#12 Posted by: egzplicit Posted at: 2018-06-02T14:36:43.163Z Reads: 91

```
I just did a firmware update to 3.102 and unplugged the can bus connector from slave while leaving it plugged into the master. Unplugged the receiver from master then upgraded firmware on master, redid motor detection. Turned it off, replugged the receiver and did the app / ppm settings. Then connected usb to slave, did the detection and slave app. Then turned everything off and reconnected the cable coming from master into slave. Started everything up again and all good. Did a test for 10 miles, all ok.

Why would a can cable connected to a focbox but not connected to the other fry the can bus? Makes no sense.

As far as I know what you don’t want is a can cable connecting two focboxes while only one is powered. A cable that is not terminated shouldn’t fry a can bus chip.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-06-02T15:14:23.613Z Reads: 89

```
No... if it was a blown, nothing will even light up. That sound more like a firmware issue
```

---
## \#14 Posted by: TinnieSinker Posted at: 2018-06-02T16:13:34.529Z Reads: 86

```
Neither CANBUS where removed before the problem occured. (i have had the connection drop out while riding though, even with hot glue holding them in)

There's a chance that the buad rate for the BT was not changed to match the module, if that helps?
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-06-02T17:33:20.375Z Reads: 85

```
@JohnnyMeduse
it happens with one of the customer, I am not tech Junkie, not aware of the technicalities but I think he Might blew something which have 5V. 

For software, I just read the whole thread now, Sounds like it's FW issue.
He need to use ST link to flash it back to default one
```

---
## \#16 Posted by: Jebe Posted at: 2018-06-02T18:58:09.385Z Reads: 78

```
sounds like canbus chip. did you have one box disconnected to power while still connected by canbus?
```

---
## \#17 Posted by: TinnieSinker Posted at: 2018-06-04T13:51:40.949Z Reads: 66

```
nah. the way i made the parallel adapter is too annoying to disconnect them.
```

---
## \#18 Posted by: TinnieSinker Posted at: 2018-06-04T13:55:24.737Z Reads: 66

```
@JohnnyMeduse @CarlCollins

I have ordered an st-link and read the walk through about it. I'll let you know how that goes.

thanks for the help.
```

---
## \#19 Posted by: TinnieSinker Posted at: 2018-06-06T10:16:18.127Z Reads: 59

```
@CarlCollins @JohnnyMeduse.

Good news, everyone! Flashing with st-link worked.

took longer to find the firmware and crimp up some wires than fixing the brick lol

Many Thanks!
```

---
## \#20 Posted by: CarlCollins Posted at: 2018-06-06T10:16:56.748Z Reads: 59

```
@TinnieSinker

Great! Now you should mark this thread as solved :slight_smile:
```

---
## \#21 Posted by: TinnieSinker Posted at: 2018-06-06T10:17:45.014Z Reads: 54

```
beat ya to it =P
```

---

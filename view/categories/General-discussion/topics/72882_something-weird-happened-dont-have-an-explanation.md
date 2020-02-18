# Something weird happened don&rsquo;t have an explanation?

### Replies: 14 Views: 199

## \#1 Posted by: ksfacinelli Posted at: 2018-10-31T04:25:59.261Z Reads: 80

```
Running dual Foxbox,  canbus between esc providing power to dual 6374 TB motor with a Nano remote....Went out on ride and lost control in first mile. Turned on and off remote and one motor powered and road home.  Charged remote and next day both motors power as normal.  Does anyone have any idea what may have happened?
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-10-31T04:47:39.487Z Reads: 69

```
Hard to tell without more info about what specifically happened when you say “lost control”
```

---
## \#3 Posted by: ksfacinelli Posted at: 2018-10-31T04:49:58.864Z Reads: 66

```
Board totally shut down.... recycled remote and one motor came back??? Did not power down board...
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-31T04:50:53.906Z Reads: 62

```
Check your connections and plugs.
Charge your remote (what you already made 😉)
And if it happens again or you can somehow recreate it don’t switch off. Connect to the vesc tool and check if there any faults.
If you have a Bluetooth module than check there if some faults poped up from the focbox.
```

---
## \#5 Posted by: ksfacinelli Posted at: 2018-10-31T04:52:50.022Z Reads: 52

```
Thanks did not crack open because next day all was good and back to normal......I thought I blew a Foxbox but not the case as everything was back next day.... ??? Just weird...Also was not pushing board at all....
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-31T04:55:19.818Z Reads: 50

```
If you have drop outs better to check your stuff.
Even if it works now. You don’t want that shit happen again when you are at full acceleration.
Safety first 😉
```

---
## \#7 Posted by: ksfacinelli Posted at: 2018-10-31T04:56:27.801Z Reads: 46

```
Agree... will crack open and and run ack tool and see if I can figure out anything...do you think a low power situation on remote could cause this situation.  Just trying to piece things together... as I charged remote over night as it was a bit a low. Just don't understand how this could be the cause because was running canbus.
```

---
## \#8 Posted by: dareno Posted at: 2018-11-01T02:26:35.511Z Reads: 28

```
[quote="ksfacinelli, post:7, topic:72882"]
low power situation on remote could cause this situation.
[/quote]

Hell yeah.  Total shutdown is usually due to bad connection to the battery or remote disconnection.  
Battery is unlikely but remote is far more common. Bad battery in the remote?  Bad connection to the receiver.  Check the master ppm cable connection.  
Reading this I'm not sure if you had charged it prior or charged it after and the problem went away.
```

---
## \#9 Posted by: ksfacinelli Posted at: 2018-11-01T02:27:46.010Z Reads: 29

```
Charged and prob went away...just weird as I was running canbus
```

---
## \#10 Posted by: dareno Posted at: 2018-11-01T02:30:56.327Z Reads: 26

```
No the little nano will cut off if low as will most remotes.  Canbus doesn't matter if there is no power at the remote.
```

---
## \#11 Posted by: ksfacinelli Posted at: 2018-11-01T02:36:29.283Z Reads: 22

```
But why when turned on and off remote did only one wheel engage?
```

---
## \#12 Posted by: dareno Posted at: 2018-11-01T02:53:14.255Z Reads: 19

```
Really need to stop speed reading.  sorry.  Could have been a weak signal dropping out during comms.
It still works as a master slave set up.  The master receives and sends via canbus.  If the signal is interrupted and weak then maybe the signal did not reach the slave.  
_

Disclaimer;  this is pure speculation_
```

---
## \#13 Posted by: ksfacinelli Posted at: 2018-11-01T02:54:16.916Z Reads: 18

```
Yea just one of the wired things if it happens again will did into it deeper...
```

---
## \#14 Posted by: Jake2k17 Posted at: 2018-11-01T02:56:14.185Z Reads: 18

```
Well, it is Halloween...
```

---

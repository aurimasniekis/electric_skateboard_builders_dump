# Changing from 6s to 9s with a single 260 kV motor

### Replies: 4 Views: 689

## \#1 Posted by: sandrewvdv Posted at: 2016-10-14T13:55:03.515Z Reads: 78

```
Hi all,

I've made my own E-Board a few months ago and it has served me very well during the summer. I once did a test ride while measuring my speed with an app ( can't recall wich one). My top speed was 39 km/h. This was on a 6s battery. 15/36 ratio (Enertion pulleys) and 260 kV motor.

Ive dialed my specs in this calcuator and found out these numbers ( http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":260,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}| )

It says my max weighted speed should be 30 km/h. So good news, I can go faster with this board. (even though I don't know how it's possible, maybe the app wasnt correct enough. It definitely felt way faster then 30km/h.)

Now I want to go even faster, so I was thinking about adding one 3s cell in series giving me a 9s battery. this would give me these speeds http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":9,"motor-kv":260,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|

45 Km/h weighted speed, fast enough if you ask me.

**

## Now for the real question.

**
I have "programmed" my VESC a few months ago, so I havent hooked it up on a PC for a while.
I have read on this forum about a VESC fault if you write new information on it. Does this also affect me when I just set other voltage limits and maybe adjust my braking force a little? Also, someone else with this setup and can give me some feedback on how it rides? :slight_smile:


Thanks in advance everyone!

EDIT: on 9s my ERPM is 60606 = sweet spot?
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-14T15:07:20.064Z Reads: 62

```
You'll actually be at about 65k erpm at full charge. May error out and break your components.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-10-14T21:46:23.033Z Reads: 42

```
Will it be ok if he sets the erpm limit at 60k in bldc tool?
```

---
## \#4 Posted by: Jinra Posted at: 2016-10-14T21:47:56.090Z Reads: 41

```
I believe he has to set the soft eRPM limit in app config. I heard setting the limits on the motor tab causes the VESC to shutdown or brake. I always setup for a <60k eRPM so I never messed with that to know for sure.
```

---

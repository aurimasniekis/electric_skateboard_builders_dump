# Mini Remote Roxxy 9120 Error

### Replies: 6 Views: 390

## \#1 Posted by: GloStix Posted at: 2017-09-30T15:41:53.730Z Reads: 61

```
Using the Mini Remote for 12S Roxxy 9120 Escs

Forward, Reverse and Neutral work fine on the remote but when I turn the transmitter off, the motors will rotate at some predetermined speed not max power.

I went through the programming steps a few times but maybe I messed up?

I would prefer it for safety reasons if I turn off the transmitter or it loses power for some reason that the motors go to neutral instead of what appears to be 1/3 power.
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-30T15:51:16.922Z Reads: 55

```
Setup the failsafe in vesc settings
```

---
## \#3 Posted by: GloStix Posted at: 2017-10-01T00:03:53.419Z Reads: 39

```
Its not a vesc but thanks I will get some for another project later.
```

---
## \#4 Posted by: pat.speed Posted at: 2017-10-01T06:56:28.570Z Reads: 28

```
If they are heli or plane escs this will most likely happen and I don't know if there is a solution
```

---
## \#5 Posted by: benjammin Posted at: 2017-10-01T08:54:36.418Z Reads: 24

```
I setup a board recently with roxxy ESCs and GT2B controller with no issues. Could it be something to do with the throttle trim, or range perhaps? I'm still pretty new to this, but if everything's setup correctly the motors shouldn't continue to spin without signal.
```

---
## \#6 Posted by: GloStix Posted at: 2017-10-08T22:49:14.292Z Reads: 15

```
Finally figured out the issue, apparently the receiver I received was not correctly built, a cheap knockoff was placed in a different housing.

Obviously to save money, as the housing had a bind button and fail safe button, but they also included a bind loop key, and the instructions stated to use the loop key (a red flag, I surprisingly didnt pick up on).

So I cut open the black plastic housing only to reveal that both the bind button and fail safe button didnt connect to anything!

Obvious chinese scam, so will get a couple more to be safe from another supplier, might as well get another transmitter too.

Think I spent 2 hrs over the course of a week or so diking around before finally just taking a dremel to that case lol 

Anyways, thanks for the help.
```

---

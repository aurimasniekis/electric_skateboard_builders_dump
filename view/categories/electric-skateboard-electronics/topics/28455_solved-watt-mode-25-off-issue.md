# \[SOLVED\] *Watt mode* 25% off issue

### Replies: 2 Views: 344

## \#1 Posted by: adseguy Posted at: 2017-07-24T07:50:35.600Z Reads: 93

```
Hi everyone, I've been lurking on the forum a few months and finally got my setup together:

New Enertion VESCX
Torque boards 6355 190kV (80amp max) 2,550Watts
10S6P Li-ion Batteries (60amp cont. 120amp max)

My issue is that in Watt control mode it's almost exactly 25% off.  What I mean is if I have the settings to
M Max: 80
B Max: 80
Watt: 250Watts

and I punch it, at no time will I get over about 184 Watts on Akamaniac's android app.  Set at 500Watts I see about 376Watts in the Control panel.  I was OK with this until I realized That hitting the 80Amp limit (if it's still following this 25% rule) is about 60Amps and sure enough you can see the Video, I'm limited here to about 60-62amps.  You can see my settings in the top left.  So what's going on?  I tried to set to 90Amps on the motor current and I get 71amps max in the display.  I don't know what to trust...

Also, I set this up tonight in Watt mode with reverse.  I noticed that when I turn off the controller first, the motor spins backwards.  I guess that's for the safety braking, but why backwards, shouldn't it just request negative amps without going in reverse?  Anything I can do about that too?

Thanks!

https://youtu.be/IgEzmu-fMss
```

---
## \#2 Posted by: adseguy Posted at: 2017-07-25T07:29:18.047Z Reads: 49

```
So I was thinking about this more and thought about the controller maybe not giving full range here.  Indeed that was the issue after looking at the App Configuration -> PPM section.  I would full throttle and it would only show me about 90%.  I used the Median Filter Auto Wizard to correct this.  I then had full range.

New problem....TOO MUCH POWER!  HAHA, I'm slipping the belt, I love it.  Great problem to have.
```

---

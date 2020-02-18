# Help me diagnose&hellip;bad BMS?

### Replies: 5 Views: 125

## \#1 Posted by: Skatejitsu Posted at: 2019-10-14T13:49:52.246Z Reads: 27

```
Last winter I built a 10s8p battery (sony VTC6) to replace a stock Evolve BGT battery.  I swapped the Evolve ESC for a Unity, used a Bestech D140 charge only BMS, custom enclosure, and everything was running great.

Due to the size of the battery, even though I rode it a "decent amount", I honestly probably never charged it more than a dozen times.  

The last time I rode it, it was running oddly.  It was stuttering and the battery reading on an LCD I had installed was showing it was very low even though I had just charged it.  I tried charging the board and it was not charging to a full voltage before the charger would turn green on me indicating it was done.

I opened everything up and tested the voltage on each BMS wire and everything was good up to bank # 9.  The 8 batteries in bank 9 had ZERO voltage...nothing.  

Fast forward to now - I've done surgery to remove the bad bank of 8 batteries.  Testing that pack alone still indicating absolutely no voltage at all.  I disposed of them immediately since they were run down to zero, so I'm assuming permanently damaged.  The remaining 9 banks of batteries all have a 4.2 voltage/ea.

My original thought was that I must have had a cell that went bad and brought down that pack.  I wired 8 new  batteries in place of the bad bank, thinking once I hook everything back up, the BMS would allow that pack to come up from 3.5 to 4.2 to match the rest of the batteries. It only charged for a couple of minutes and the charger turned green.  Voltage on pack #9 is still only 3.5.

ALL this info to lead me to this question - was it not a bad cell, and is this just a bad BMS?  I don't see anything visually burned up on the BMS itself.  It appears it's just not allowing anything in bank #9 to be charged.  The leads are run properly to the BMS and indicate the same voltages as if I probe the packs themselves, I just don't know if there's anything else I can do myself to test the BMS.  

Also, if this was just a simple failure in the BMS, is there a better quality one I should be using?  I went with Bestech because that seemed to be what everyone recommends, but I have a pretty big enclosure and can fit just about anything.  I'm ok with spending more on a higher quality one if it means less potential of having to go through something like this again!
```

---
## \#2 Posted by: JoelMatousek Posted at: 2019-10-14T15:10:44.821Z Reads: 15

```
Just be very careful with this, running into issues like this can very easily cause fires. I would suggest running a new lead from #9 pack to the bms. It seems like there could be an issue with wiring. If not, I would suggest getting a new bms. I have a bestech and I have no issues with it
```

---
## \#3 Posted by: Tinp123 Posted at: 2019-10-14T15:21:45.281Z Reads: 15

```
You have to charge new group to same voltage like old groups! Bms just can't balance voltage difference of 0.75v (assuming new cells are on 3.45v and old on 4.2v). If you have normal 1s or adjustable charger and you have possibility to connect crimps as charging connectors, you can charge only that new group while still in pack. But be extra careful not to short anything. If you don't feel comfortable doing this, disconnect new group from other groups and charge it then. When you charge new group to the same voltage as others, connect it back on pack and bms and leave everything overnight. Check voltage on each group every few hours if possible. If you spot heat on bms or you see that bms is draining that one group,disconnect bms and smash it with hammer.
```

---
## \#4 Posted by: Skatejitsu Posted at: 2019-10-14T16:16:44.842Z Reads: 12

```
Thanks! I wasn't 100% sure if the BMS could/should bring up the lagging pack to 4.2 or not.  What you described was exactly my other idea.  I'll pick up a 4.2v charger and charge that new bank of batteries while they are still in the pack and then monitor everything closely once I get the entire thing up to 42v.
```

---
## \#5 Posted by: Skatejitsu Posted at: 2019-10-14T16:19:22.314Z Reads: 11

```
That's not a bad idea.  The wire looks good and reads the same voltage at both ends.  I can plug it into the BMS and test voltage on the board and it gives the proper reading, so I don't think it's a bad wire or connector, but I may do just that to be on the safe side.
```

---

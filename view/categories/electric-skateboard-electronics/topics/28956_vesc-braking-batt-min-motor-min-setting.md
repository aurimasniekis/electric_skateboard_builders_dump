# VESC Braking - Batt Min / Motor Min Setting

### Replies: 2 Views: 555

## \#1 Posted by: jaykup Posted at: 2017-07-28T18:18:13.071Z Reads: 155

```
I've got a 12s4p pack with Samsung 25r cells in it.

Datasheet shows 4A max charge per cell for "rapid charge".

So my VESC is configured as follows:

Motor Min: -60
Batt Min: -16 (4x4)

The problem is my brakes aren't strong enough at higher speeds.  Ideally I should be able to brake hard enough to lock up the rear.  I noticed my data logs are only showing -40 to -50 motor min in practice, and I believe it's because of the large difference between Motor Min and Batt Min.  At high duty cycle, the 44A difference needs to be dissipated by heat (i think) in the VESC, causing an over temp error (and brake failure), or just weak brakes.

I want to increase my Batt Min to say -32 to give somewhere for this energy to go.  This is nearly twice the recommended rapid charge rate on a Samsung 25r.

So the question is, how bad is it to charge 18650 cells for short periods of time (<30 seconds) at 2-3x the rapid charge rate?  Is temperature of the cell a driver for these 4A specs?  Or does it cause physical damage to the cell even before it reaches max temperature and results in a loss of capacity?
```

---
## \#2 Posted by: RiGo Posted at: 2017-11-01T03:17:46.567Z Reads: 107

```
Puling up an old thread I found when searching as I have the exact same question.

Could someone who knows better please provide some insight into this?

Thanks!
```

---

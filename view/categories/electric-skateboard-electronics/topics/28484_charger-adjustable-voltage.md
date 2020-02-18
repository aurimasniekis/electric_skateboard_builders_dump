# Charger adjustable voltage

### Replies: 13 Views: 1229

## \#1 Posted by: banjaxxed Posted at: 2017-07-24T12:22:16.690Z Reads: 136

```
Decided to open a new thread for this rather than derail a closed GB for 12s charger.

Essentially I bought this charger when originally planning a 10s setup, while I may still run a board in 10s almost certainly I will be doing a trampa ATB in 12s, in which case I either need to be ablre to mod this charger or buy a 12s one.

Here is the charger I have
https://banggood.app.link/lc17oCsKNE

Here is the guts to check for a potentiometer, not clear to my eyes , can anyone help with identifying?
https://www.electric-skateboard.builders/uploads/db1493/original/3X/a/9/a9123a452b6c32c5e1f5900b066b79e34ff3a01d.JPG

Thanks
```

---
## \#2 Posted by: jmasta Posted at: 2017-07-24T12:38:15.336Z Reads: 131

```
I see three potentiometers, which is typical of many voltage regulators. See the little blue boxes with the small screw on top? One of them should be for voltage output, one for max current, and the other I'm not sure...

Look on the PCB for labels. My guess is the voltage pot is one by itself on the right side near the power cord. Hook up a power meter first so you know what you're changing before turning any potentiometer screws
```

---
## \#3 Posted by: banjaxxed Posted at: 2017-07-24T12:40:51.927Z Reads: 123

```

thanks for this, I wasn't sure if they were what I was looking for, will try that (carefully)
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2017-07-24T12:44:20.923Z Reads: 116

```
Hopefully someone with proper knowledge will answer this specifically for you. 
My thinking is that if it's a 10s charger then you are only going to be able to adjust the voltage slightly in an around the 42v mark. Like adjusting the voltage a bit lower for example 4.1v per cell to extend the life of your battery. Just thinking out loud.
You might be better off selling this to someone who can use it as is and buying the proper charger for your 12s setup. This is the safest bet.
```

---
## \#5 Posted by: Silverline Posted at: 2017-07-24T12:50:48.161Z Reads: 107

```
Sorry for offtopic. But i`m looking for a 10s charger for my Bestech 10s BMS. This charger looks nice. But how do you know when the batteries i charged ? It don`t look like there is a diode or something ?
```

---
## \#6 Posted by: jmasta Posted at: 2017-07-24T12:58:31.493Z Reads: 100

```
It's not the safest idea (nor is building your own electric skateboard...), but it honestly might work.  

I have the 12S adjustable charger from the group buy linked above.  It was supposed to be 12S 5A, like the identical-looking 10S 5A chargers.  But it is actually only 4A at 12S.  Why is this significant? Because I suspect it is just a 200W charger with adjustable voltage and current.  My power meter has always shown 200W or less charge current, which is roughly equivalent to what you'd also get from a 10S 5A charger

Be very careful while adjusting the charger, since it needs to be open and powered on.  Don't increase the voltage without also decreasing the current output.  I'd recommend balancing the power output such that `P=V*I` remains constant pre- and post-adjustment
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-07-24T13:10:41.570Z Reads: 90

```
Interesting and thanks. So it's quite possible they tune the voltage for different outputs and slap the appropriate stickers on it.
```

---
## \#8 Posted by: rpn314 Posted at: 2017-07-24T13:24:31.569Z Reads: 90

```
Yeah. It's either been made to get it in the general ballpark for a 10s, and then the potentiometers just tune it exactly to account for slight variations in components (I'd probably tune it down to 41v for longevity's sake) or it's completely generic and the potentiometer can change it between 10s+/- a few (maybe 8s up to 12s?). My guess is it's just to account for slight variations, but you may get lucky!

Take it slow, with just a multimeter (Not plugged into your board!), and see what happens. Risk is pretty low. Turn one potentiometer a little, see if the voltage changes. If it doesn't, turn it back to where it was and try another. Either way, keep track of how it is now so you can revert if necessary :slight_smile:
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-07-24T19:09:06.133Z Reads: 80

```
Yeah everyone so far has probably been right, though do be careful and make sure at least the capacitors have a voltage higher than whatever your adjusting it to. 

@Silverline you could probably use this charger with it, and the way you know it's done charging is either when the batteries stop drawing any current, or if theres a charge indicator LED on there, it will let you know.
```

---
## \#10 Posted by: banjaxxed Posted at: 2017-07-24T19:19:03.110Z Reads: 75

```
Thanks for the advice all, the Banggood charger has a led status but I went and bought a second charger for 12s linked by @TranxFu in the GB, eBay €20 offer accepted , €13.50 delivery
```

---
## \#11 Posted by: SilentException Posted at: 2017-07-24T19:25:24.956Z Reads: 75

```
Probably for the best and good for you. Playing with mains voltages while screwing with pots is not good if not sure what you're doing. It could go well but it could also go very terribly wrong.

As a funny coincidence, there was a recent video by GreatScott!, awesome guy, very knowledgeable in electronics who wanted to turn PC PSU into variable output PSU. He have up in the end for the same reasons.
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2017-07-24T19:47:43.938Z Reads: 73

```
so no extra use for those pc power suplies laying around...damnn was hoping i could use them at some point
```

---
## \#13 Posted by: banjaxxed Posted at: 2017-07-24T20:00:07.644Z Reads: 71

```
In case anyone else is looking for a safe adjustable voltage charger look here
https://www.electric-skateboard.builders/t/10s-and-12s-adjustable-charger-from-china-groupbuy-worldwide/17287/15
```

---

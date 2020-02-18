# Soldering your own VESC

### Replies: 17 Views: 1070

## \#1 Posted by: uigiroux Posted at: 2018-01-04T07:49:56.613Z Reads: 189

```
So I was looking this topic up online and came across a few threads where this has been done, but I then got curious about something that I've asked before and was told the VESC was the limiting factor.  I'd I wanted to run a motor with a 14s battery pack, could I do that IF I soldered my own VESC and put in higher resistors or whatever it is that makes them fry if the power goes over voltage?  Is there some modification that can be made to already built VESC's that would allow this as well?
```

---
## \#2 Posted by: willpark16 Posted at: 2018-01-04T07:55:15.617Z Reads: 188

```
Most of the components would require smd and a heat bed, soldering is only good for a few components and I'm pretty sure that it is not in fact possible, roughly every component of the vesc would have to be upgraded. @JohnnyMeduse would know best
```

---
## \#3 Posted by: b264 Posted at: 2018-01-04T07:56:34.296Z Reads: 185

```
Firstly you'll need to upgrade the MOSFETs at the minimum, and most of the components at the maximum.  I really don't recommend this, there are other ESCs on the market that can do higher voltages (ebike controllers).  It's more useful to add two VESC controllers and two motors and/or bigger motors, than trying to run the circuit at a higher voltage, unless you know **exactly** what you're doing.  The reactive load of motor windings will ensure that the voltages your circuit will endure need to be higher than the supply voltage, as well.  Technically the vesc can handle 14S but not when you add that in.
```

---
## \#4 Posted by: uigiroux Posted at: 2018-01-04T08:03:21.642Z Reads: 172

```
Good points, well figured it was worth at least asking! Thanks guys :)
```

---
## \#5 Posted by: SOICDIP Posted at: 2018-01-04T08:04:16.638Z Reads: 167

```
A fully charged 14S pack is 58.8V, which is too close to the max operating voltage (60V) of the DRV8302/1.

If you go downhill and use regen breaking, you'll easily exceed 60V and even the absolute max supply voltage of 65V. 

Sure you can get higher rated capacitors but you wouldn't be able to use the DRV8302/1, which is the core of a VESC4/6.

You'll need to design your own ESC with dedicated MOSFET drivers like this:
http://www.electric-skateboard.builders/t/daily-driver-v2-0-35-holypro-trampa-vertigo-trucks-aps-6384s-170kv-4kw-custom-directdrive-12s-custom-esc/36560/14

If you must go 14S, something like this should work:
https://hobbyking.com/en_us/turnigy-dlux-250a-hv-14s-60v-esc.html
```

---
## \#6 Posted by: uigiroux Posted at: 2018-01-04T08:12:18.100Z Reads: 145

```
There are some engines I've wanted to use that day they can go up to 14s.  I've never understood when someone is doing a build and they have a great motor and then run it at like 6s or 8s.  Even 10s I don't get, it seems like people are underpowering their motors if they aren't running the max 12s..?
```

---
## \#7 Posted by: SOICDIP Posted at: 2018-01-04T08:16:38.228Z Reads: 137

```
[quote="uigiroux, post:6, topic:42729"]
Even 10s I don't get, it seems like people are underpowering their motors if they aren't running the max 12s..?
[/quote]

You also have to watch out for the kV rating of the motor, as if it's too high (over 200kV) running it at 12S may exceed the 60k ERPM limit with VESCs.

You might also want to go that fast; personal preference.
```

---
## \#8 Posted by: uigiroux Posted at: 2018-01-04T08:19:14.550Z Reads: 126

```
Lol no I just want to do 50, maybe 60mph tops. I'll use 107mm wheels though!
```

---
## \#9 Posted by: SOICDIP Posted at: 2018-01-04T08:23:57.359Z Reads: 125

```
[quote="uigiroux, post:8, topic:42729, full:true"]
Lol no I just want to do 50, maybe 60mph tops. I'll use 107mm wheels though!
[/quote]

50-60mph sounds scary, maybe it's just me. 

https://www.youtube.com/watch?v=7uo7Ek9JZbE

Use this calculator to guide you through building one:
http://calc.esk8.it/
```

---
## \#10 Posted by: uigiroux Posted at: 2018-01-04T08:35:12.352Z Reads: 117

```
Ouch, that looks painful, but not too bad as long as your wearing the proper protective gear.  I've had similar motorcycle accidents where I slid like that from a tight turn and walked away from it cause I had leathers on and good helmet.  Just sore the next few days /well, lol.  No I don't actually want to go that fast, I would like to be able to do about 40mph realistically.
```

---
## \#11 Posted by: Acido Posted at: 2018-01-04T12:37:29.784Z Reads: 98

```
You will die unless you are riding in the world of sponge
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2018-01-04T14:32:38.680Z Reads: 93

```
[quote="uigiroux, post:6, topic:42729"]
I've never understood when someone is doing a build and they have a great motor and then run it at like 6s or 8s.  Even 10s I don't get, it seems like people are underpowering their motors if they aren't running the max 12s..?
[/quote]

The Vesc was originally built for around 6s to 8s setup, most of the component are ratted for 50V to 60V MAX on the original Version which should be 25% to 30% higher than the Maximum voltage allowed... Why did you think everyone was blowing up their Vesc at 10S and 12S? But since then Companies like Enertion and Ollin as upgrade most of the 50V part (which were mostly CERAMIC Capacitor) up to 100V, But still the DRV Can only go up to 60V or else it will most likely blow.  The Only reason a FocBox could go up to 13S (which I really don't recommend), is because there is a TVS diode that blocks the excess voltage over 53V (if I remember correctly).

If you want to go higher than 12S, you need to find another ESC type.
```

---
## \#13 Posted by: uigiroux Posted at: 2018-01-04T18:59:31.286Z Reads: 73

```
Is it possible to upload Vedder software too one of these other ESC for bikes?
```

---
## \#14 Posted by: FredSaberhagen Posted at: 2018-01-04T19:36:21.171Z Reads: 68

```
not unless those bike ESCs were also designed around the VESC project (same ST micro Coretex M4 etc)
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-01-04T19:56:28.319Z Reads: 62

```
Yes, it is, but you have to look at projects that are base on the Vedder Project. 

Like this one 

http://vesc-project.com/node/144

And unlike the Vesc they are far from cheap.
```

---
## \#16 Posted by: uigiroux Posted at: 2018-01-04T20:31:50.299Z Reads: 54

```
Whoa, 200 hp vesc, that's insane!
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-01-04T20:43:12.731Z Reads: 54

```
Isn't what you where looking for ??? :grin:
```

---

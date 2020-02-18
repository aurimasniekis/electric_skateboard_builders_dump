# VESC 6 Brake Over-ride

### Replies: 5 Views: 241

## \#1 Posted by: Everglase Posted at: 2019-04-10T23:01:25.174Z Reads: 76

```
Hi all.

First time poster. :slight_smile:

I'm converting my partners Razor E300 over to using a BLDC motor and I want to use the VESC6 controller.

I have a twist throttle that will run via ADC and I plan to use a thumb throttle for regen braking. But we still want to keep the mechanical brake there for when it is needed (holding on hills, emergency ect).

Is there a way that I can use the brake switch that is on the brake lever to tell VESC to not to apply throttle? That way the motor isn't trying to be powered as the mechanical brack is activated?

TIA 

Jeff
```

---
## \#2 Posted by: district9prawn Posted at: 2019-04-11T04:07:42.090Z Reads: 59

```
Hi,

The simple way would probably be to use the switch to short the throttle signal to ground.
```

---
## \#3 Posted by: Everglase Posted at: 2019-04-11T04:30:30.299Z Reads: 54

```
I was thinking about using it to interrupt the signal. But I didn't know if there was a way to do it in vesc.

Thanks :slight_smile:
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-04-11T14:56:42.981Z Reads: 33

```
probably the vedder forum have lots and lots of info. on this

http://vedder.se/forums/viewtopic.php?f=6&amp;t=230&amp;sid=061a9d947abfe31633308c4ddbd7cf89

for the mostpart (99%) we rely on the regen braking which is why we show up in A&E frequently
```

---
## \#5 Posted by: Everglase Posted at: 2019-04-13T07:26:51.791Z Reads: 13

```
I am planning on using regen braking but would also like a mechanical brake. If I end up putting my partner in the emergency room she would never let me live it down :laughing:
```

---

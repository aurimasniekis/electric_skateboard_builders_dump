# Sensored versus Unsensored: Louder motor?

### Replies: 6 Views: 999

## \#1 Posted by: jackw Posted at: 2016-10-23T15:30:02.749Z Reads: 205

```
I've been skating my new build around for a few weeks and have been having a lot of fun. No real problems with the VESC and it all seems to be working really well.

I did however have a small amount of cogging from a standstill start, nothing major - just what I imagine is the VESC figuring out which way is forward before giving you smooth acceleration. I would always make sure I was moving forward slightly or give a little push when starting off, but wondered if connecting up the sensor wires would make any difference.

My motor is a 190kv 6355 from Torqueboards, which has the small type sensor connector so I wired up an adapter with a larger pin pitch that fits the VESC and gave sensored motors a go.

I now have awesome smooth acceleration from a complete stop, and seem to have smoother performance overall when braking or quickly punching the throttle while already moving to get up to speed.

I do however seem to have gained louder motor running noise? I don't understand the in's and out's of exactly how the VESC controls motors (I know the basics, BLDC/FOC having differing "styles" of telling the motors what to do...) but how could BLDC with or without sensors make a difference?

Before without sensors, the motor had that tell-tale BLDC whine, but now with the sensors added there now seems to be a louder lower pitched groan in there too, especially when braking. It has made me much more conscious of it when riding around the city compared to before.

Anyone else noticed a difference after they added sensors?
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-23T15:33:12.634Z Reads: 199

```
There shouldn't be a louder noise, mine is the same sensored and unsensored. Make sure you use hybrid mode, that way it goes sensorless after a certain erpm.
```

---
## \#3 Posted by: jackw Posted at: 2016-10-23T19:39:16.626Z Reads: 162

```
Ahh good thinking, now that you mention it I am unsure if I set it to sensored or hybrid mode...

I'll whip out the usb cable and report back!
```

---
## \#4 Posted by: Michael319 Posted at: 2016-10-23T22:12:05.342Z Reads: 137

```
What did it say?
```

---
## \#5 Posted by: jackw Posted at: 2016-10-24T01:26:00.956Z Reads: 124

```
Well I'll be damned, from my testing at the workbench, seems like that was the problem! I'll take it out tomorrow for a proper test at speed and in normal circumstances to confirm though :)

Thanks to @Jinra, gotta love it when a problem is just a slight oversight and is fixed almost instantly!
```

---
## \#6 Posted by: FlashNova Posted at: 2016-10-24T08:19:19.761Z Reads: 104

```
Does anybody know if using hyrbid mode will effect your top speed?
```

---

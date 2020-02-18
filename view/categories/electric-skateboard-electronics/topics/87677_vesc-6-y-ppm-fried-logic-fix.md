# VESC 6 Y PPM fried logic fix?

### Replies: 3 Views: 149

## \#1 Posted by: goffzh Posted at: 2019-03-19T22:11:42.204Z Reads: 42

```
Had 2 Trampa VESC 6+ running off separate channels of a receiver cause I need independent speed control of 2 motors. After doing some no load wheels up testing one of the VESC's is now dead, no lights. Digging through documentation and forum posts I'm guessing the 5V pins I had connected together could've caused the failure. Also possibly having common ground through the PPM port seems frowned upon based on some forum topics. Been doing this stuff for decades and its kinda ridiculous the logic rail is so frail and unprotected on these supposedly high-end controllers but I digress to the point of this topic being what might have failed and need replaced in this sort of fault? I don't know much about VESC hardware. Is this potentially an easy repair replacing a regulator chip or is there going to be a lot of dead components needing days of troubleshooting? Going forward I'm putting optoisolators inline the PPM cables to block any sort of troublesome ground loops like what mature r/c controllers do.
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2019-03-19T23:09:50.293Z Reads: 30

```
[quote="goffzh, post:1, topic:87677"]
Is this potentially an easy repair replacing a regulator chip or is there going to be a lot of dead components needing days of troubleshooting?
[/quote]

You can always check if you still have a 5V output on the damage VESC, if not you most likely have killed the DRV, which have an integrated 5v regulator.
```

---
## \#3 Posted by: goffzh Posted at: 2019-03-19T23:34:23.989Z Reads: 22

```
Yeah I assumed the 5V was dead since no LED's were lit.
```

---

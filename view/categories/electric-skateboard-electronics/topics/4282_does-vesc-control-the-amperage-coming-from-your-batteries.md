# Does VESC control the amperage coming from your batteries?

### Replies: 3 Views: 733

## \#1 Posted by: Pyrax Posted at: 2016-06-05T12:07:52.122Z Reads: 96

```
If I am running two 6S 10,000 mAh 10c batteries in series will the Enertion VESC be able to handle the amount of amps coming from the batteries (maximum of 100A). The VESC is capable of handling up to 12s so it is fine voltage wise however It is only rated for 50 A continuous so I was wondering whether or not the VESC would automatically control the amperage coming from the batteries or whether anything else would be needed to do this.
Thanks-
Current Rig:
2X Multistar High Capacity 6S 10000mAh
Turnigy SK3 192kv Outrunner Motor
Enertion VESC
Enertion Motor Mount, Trucks and Wheels
```

---
## \#2 Posted by: Maxid Posted at: 2016-06-05T12:12:24.010Z Reads: 91

```
When you turn on the lights in your house are you also worried about them using the full current your grid can offer?

The VESC will take the current it currently needs to drive the motor - not what the batteries can supply.
It is not like there are constantly running 100A through the ESC - where would all that energy go otherwise?
```

---
## \#3 Posted by: lowGuido Posted at: 2016-06-05T12:47:28.217Z Reads: 81

```
Yes. the VESC is almost infinitely programmable. current is one of the many things it can control.
```

---

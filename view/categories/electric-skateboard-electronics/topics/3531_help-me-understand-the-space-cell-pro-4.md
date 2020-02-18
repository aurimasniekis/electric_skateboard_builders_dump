# Help me understand the Space Cell pro 4

### Replies: 3 Views: 965

## \#1 Posted by: Jinra Posted at: 2016-05-20T02:17:00.399Z Reads: 119

```
I'm reading up on the pro4 specs and it states it has the ability to draw 80 amps (which makes sense 4p x 20a) but has a 40a fuse for protection and the pack should be used on "2400w motors or less!". With these specs the max the battery can output before the fuse blows is 1680 watts; and between two motors that's 840 watts each So..

1. Does that mean dual motors (assuming 2400w motor) have 1560 worth of unusable watts?

2. The VESC should be programmed with a motor max of 40a (20a with dual)?
```

---
## \#2 Posted by: paragon Posted at: 2016-05-20T02:30:11.821Z Reads: 115

```
I think the 40a fuse can handle higher voltage spikes. If it blows, you can probably just put a higher rates one in.
```

---
## \#3 Posted by: shred Posted at: 2016-05-20T07:44:33.614Z Reads: 90

```
I think what you are saying is correct! 
Not so sure what you could configure as motor max. 

You might be interested in this one:
http://www.electric-skateboard.builders/t/bypassing-bms-of-space-cell-to-pull-more-amps/2204
```

---

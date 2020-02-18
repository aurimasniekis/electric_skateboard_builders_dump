# VESC may or not be broken, need help

### Replies: 3 Views: 653

## \#1 Posted by: robskie Posted at: 2016-09-14T15:09:11.917Z Reads: 53

```
Hi there, I'm very close to completing my board, the my VESC isn't cooperating.
I'll start by giving some basic information.

Enertion VESC (ordered about a month ago, received 2 weeks ago)
Motor:
http://alienpowersystem.com/shop/brushless-motors/alien-5065-outrunner-brushless-motor-270kv-2200wa/

Batery: http://www.hobbyking.com/hobbyking/store/__8851__ZIPPY_Flightmax_3000mAh_3S1P_20C.html
(I know these batteries won't last long, but my priority is for them to take the least amount of space possible since I have a pretty flexy deck.

Now, for the actual question.

Whenever I try to do my motor detection it doesn't work (The motor does actually nudge a bit when I power it, it also nudges during motor detection)
and when I go to the realtime data tab and I try to use my remote I get the infamous 'drv8302' fault.


This is the way i have my VESC connected to my motor, I know this is not at all an optimal connection, but I have no proper connectors yet (i'll just solder everything in place when I know it works)
nor do I have access to any connectors atm, since I pretty much drained my bank account by buying all the parts (I guess some of you know the feeling? :D)

Could this be causing the issues I'm having, or is the VESC faulty for sure?

<img src="/uploads/db1493/original/3X/1/5/15180f0e791102f58d83ed7813a44be0212944e4.jpg" width="669" height="500">

Also, has anyone ever used the motor I'm using, I haven't found the perfect settings yet as the settings could probably be causing the issues aswell I suppose.

I'd really like to get some help since I'm looking forward to riding this board A LOT.

Thanks guys
```

---
## \#2 Posted by: ra.rend Posted at: 2016-09-14T16:18:33.691Z Reads: 39

```
Drv chip needs to be replaced. Contact enertion support. They'll probably tell you to buy the 1 year warranty, then send it to be repaired (they might just send you a new one instead)
```

---
## \#3 Posted by: chinzw Posted at: 2016-09-14T16:51:24.921Z Reads: 34

```
Did you set your motor step ramp value before doing the motor detection? I've been seeing a lot of problems with that value defaulting to 50 and also writing x10 the value to the vesc.
```

---

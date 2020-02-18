# See realtime data from two VESCs

### Replies: 4 Views: 651

## \#1 Posted by: rmrf Posted at: 2016-09-04T10:58:52.642Z Reads: 96

```
Is it possible to see realtime data (voltage, current, rpm) in BLDC_Tool for several VESCs? If yes, can I see it all at the same time, or do I need to switch between CAN ports? Or maybe I can run two BLDC_Tool apps at the same time?
```

---
## \#2 Posted by: Monte Posted at: 2016-09-04T14:46:40.588Z Reads: 66

```
I only have one mono Board and never tested it with two, but i think it should work if you connect your vescs with cables on an Laptop at the same time and use BLDC with diffrent Com ports
```

---
## \#3 Posted by: Skitzor Posted at: 2016-09-04T17:55:54.355Z Reads: 52

```
Someone correct me if I'm wrong but if you enable the can fwd the realtime data should be from both vescs...
```

---
## \#4 Posted by: rmrf Posted at: 2016-09-04T19:34:44.222Z Reads: 37

```
That's what I am trying to figure out. Can not test it right now, because don't have two VESCs but looking at BLDC_Tool code https://github.com/vedderb/bldc-tool/blob/master/packetinterface.cpp `PacketInterface::processPacket` does not check where the packet comes from. I think it is only possible to specify which VESC you want to communicate with, but it does not work to receive packets from all VESCs at the same time
```

---

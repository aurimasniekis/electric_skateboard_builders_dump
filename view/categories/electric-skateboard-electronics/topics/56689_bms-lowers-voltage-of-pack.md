# Bms lowers voltage of pack?

### Replies: 4 Views: 163

## \#1 Posted by: Brontech Posted at: 2018-05-25T01:58:42.755Z Reads: 41

```
I am currently wiring two 6s lipos in series to a 12s bms. What is weird though, is that when I go to measure the B- one the bms, I get a readout of 44.9, but on the P- output, I get a readout of 44.1. Not exactly sure what is causing this, any insight would be very appreciated! :slight_smile:
Also, is this something I shouldn't really worry about, or is it an issue that has to be resolved?
```

---
## \#2 Posted by: mmaner Posted at: 2018-05-25T02:53:52.484Z Reads: 34

```
The BMS requires a load, or draw, to actually discharge correctly. Until it's connected a system that makes a significant draw you won't get accurate measurements with a multimeter.
```

---
## \#3 Posted by: Brontech Posted at: 2018-05-25T02:55:45.269Z Reads: 31

```
Ok, thanks for the help! :slight_smile:
```

---
## \#4 Posted by: mmaner Posted at: 2018-05-25T02:56:25.128Z Reads: 28

```
No worries. Just connect a vesc and motor to it and it'll look right I expect.
```

---

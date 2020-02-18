# Where do I connect the reciever to my VESC

### Replies: 3 Views: 480

## \#1 Posted by: codes Posted at: 2016-10-14T18:42:13.574Z Reads: 82

```
Just bought 2 vescs from enertion, not the new one, and am planning on connecting them via can bus connector. Where do I connect the receiver for controller?
```

---
## \#2 Posted by: jespers101 Posted at: 2016-10-14T19:02:25.722Z Reads: 76

```
This may not help with dual vesc ( I only have experience with 1) but your receiver connects to the 3 pin plug on your vesc capacitor side. You may have pins or you may just have solder pads. It depends on who you bought it from.
```

---
## \#3 Posted by: Blasto Posted at: 2016-10-14T19:16:30.101Z Reads: 73

```
do a search using "CAN bus VESC" you should find clear instructions

unclear instructions:
one vesc is your master, he will have the ID 0 and you will connect the servo wires to this one. He will be driving the show. the other vesc is your slace, he will have the ID 1, he listens to the master and takes commands or he will be punished.
```

---

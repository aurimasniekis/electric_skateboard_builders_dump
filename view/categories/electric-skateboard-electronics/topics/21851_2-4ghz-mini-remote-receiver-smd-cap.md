# 2.4Ghz Mini Remote Receiver: SMD Cap?

### Replies: 4 Views: 404

## \#1 Posted by: whitepony Posted at: 2017-04-26T20:23:24.176Z Reads: 61

```
jojo guys,

think my antenna got loose on my 2.4Ghz mini remote receiver, so I tried to open the enclosure to re-solder it. sadly its well sealed, so I had to break it open and while doing that I damaged the SMD capacitor (see picture). can anyone tell what kind of cap it is? there is nothing printed on it, dimension seems to be 3.2 x 1.6mm (just about, cant tell exactly really).

<img src="/uploads/db1493/original/3X/a/8/a8f7e05b571b112147737495a12edfae2523a361.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/3/d/3de2c4bb8cac24a428b258d4417fdb6688129296.JPG" width="375" height="500">
```

---
## \#2 Posted by: Blasto Posted at: 2017-04-26T20:27:45.783Z Reads: 56

```
just looks like a decoupling cap (on gnd and 5V rail), 2.2uf 16V should be good (0805 size???)

it will probably work without it... but also good to have it, you have a tantalum cap that's there for the lower frequencies, that one would take care of the higher frequencies
```

---
## \#3 Posted by: whitepony Posted at: 2017-04-26T20:36:21.181Z Reads: 51

```
hm, I have no clue about these things - all I can do is hold a soldering iron and do some minor soldering work. from the size table this seems to be a 1206 size apparantly. is bigger = better for low passing? should I look for anything above 5V and large capacity?
```

---
## \#4 Posted by: Blasto Posted at: 2017-04-26T20:39:53.871Z Reads: 46

```
16V is good, the receiver is 5V. 1206... man that is a big cap.... if i had to guess... 4.7uF to 22uF
```

---

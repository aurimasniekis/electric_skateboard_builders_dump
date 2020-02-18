# Using different 2 different motors/escs in one build?

### Replies: 4 Views: 274

## \#1 Posted by: ih8Darian Posted at: 2018-07-18T04:19:11.661Z Reads: 76

```
I have a N5055 (http://www.diyeboard.com/270kv-n5055-outrunner-motor-1400w-for-diy-electric-skateboard-p-539.html) diyeboard motor welded to a Caliber truck and a diyeboard esc. If I bought a torqueboards 6374 motor alongside with a VESC, would all of those parts work together? I want to make a Frankenstein build because I already have some parts.
```

---
## \#2 Posted by: JazzAmsterdam Posted at: 2018-07-18T07:54:40.985Z Reads: 58

```
I don't see how you can use the same remote for both ESC and VESC. Even if you were to use 2 seperate remotes at the same time, you still would need to gear them to have the exact same rpm and acceleration curve etc. Otherwise one would go faster than the other. Does not seem like a good idea to me, perhaps you can use the parts you already have to make a 2nd/backup board.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2018-07-18T13:23:02.713Z Reads: 42

```
two different motors and escs totally work together, check out @lowGuido ´s build.
Problem with your case is the diyeboard esc because of the build in receiver. You would need that signal somehow on your vesc, which is not possible to get as far as i know.
```

---
## \#4 Posted by: pennyboard Posted at: 2018-07-18T14:08:30.714Z Reads: 34

```
My advice is ditch the diyeboard one and do a single motor with the vesc. The diyeboard esc will just interfere with the vesc and make the ride quality worse. 
It is possible to run both of those but one will always be pulling more power than the other and you'll need 2 remotes or build one yourself.
```

---

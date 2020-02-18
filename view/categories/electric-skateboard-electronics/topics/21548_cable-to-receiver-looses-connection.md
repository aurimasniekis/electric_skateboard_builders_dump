# Cable to receiver looses connection

### Replies: 7 Views: 280

## \#1 Posted by: faaailix Posted at: 2017-04-22T10:27:06.482Z Reads: 63

```
Hi,
I'm using a build with a VESC and a standard 2.4 Ghz transmitter with receiver. The connection cable between VESC and Receiver (3pin servo cable), however, sometimes looses connection on the receiver side - I guess due to vibrations. On the receiver side it's just hold in place via a plug. This is quite dangerous at high speed. Did someone have the same problem? How did you solve it? Directly soldering to the pins of the receiver?
```

---
## \#2 Posted by: lowGuido Posted at: 2017-04-22T10:35:40.426Z Reads: 60

```
solder EVERYTHING.
plugs and sockets are not designed for skate vibrations.
```

---
## \#3 Posted by: faaailix Posted at: 2017-04-22T10:44:48.394Z Reads: 54

```
@lowGuido I agree. But would you solder it directly to the pins? Do you maybe know of an example photo or youtube video where someone solders it in a correct manner?
```

---
## \#4 Posted by: lowGuido Posted at: 2017-04-22T12:47:57.519Z Reads: 47

```
I would. solder it to the pins and put heatshrink over each wire.
my first board that I built had the standard PWM plug on the ESC and after a few hundred km of riding it just dropped off. I was about 13km from home and I had no tools with me to open my box up.
after that Day I solder everything or at very minimum glue the PWM plugs in.
```

---
## \#5 Posted by: faaailix Posted at: 2017-04-22T14:08:24.811Z Reads: 39

```
Instead of soldering it to the pins, I desoldered the pins and soldered the link cable directly on. Thanks for the advice.
```

---
## \#6 Posted by: Mrmoonlight Posted at: 2017-04-22T14:41:50.276Z Reads: 35

```
I had an issue where I'd lose connection when the outside temp dropped below freezing. Soldered everything and everything is now good.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-23T04:30:17.785Z Reads: 22

```
Soldering the wires to the vesc would definitely be the fool proof solution.
However, I just got some zip ties and put them around the signal wires and the vescs and I have been running it that way for a long while  now with no problems.
<img src="/uploads/db1493/original/3X/e/0/e0f5369cb8c476afdd7b3b8b7398055c7dae264b.png" width="490" height="499">
```

---

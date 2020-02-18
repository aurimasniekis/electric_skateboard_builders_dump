# FOCBOX Documentation

### Replies: 8 Views: 735

## \#1 Posted by: Olloxan Posted at: 2017-11-02T18:52:32.980Z Reads: 180

```
Hi everyone,
I would like to build my own Eskate using enertions FOCBOXES. I was looking around for a detailed documentaion of all its Pins but could not quite find one. I would like to use cruisecontrol and was wondering, if I can implement this in the FOCBOXES or if I would have to program the remote to give a continous signal. Furthermore I would like to use the 5V 1A pin on the FOCBOX to put some LEDs on. Would it be possible to control this pin with the remote like an ON/OFF Switch? Alternatively would it be possible to control all this using the RX/TX Serial communication Pins on the FOXBOX? It would be awesome if you could help me or point me to any tutorials I may have missed.

Cheers
```

---
## \#2 Posted by: Acido Posted at: 2017-11-02T18:56:05.067Z Reads: 172

```
Depends on your remote channels for that, think g2b has some channels you can use for that kind of stuff
```

---
## \#3 Posted by: Olloxan Posted at: 2017-11-02T19:11:08.025Z Reads: 163

```
Do I have to program the remote myself, like the signals, it is sending? How do I know, what signals the FOCBOX needs to do something?
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2017-11-02T19:19:33.097Z Reads: 154

```
[quote="Olloxan, post:1, topic:37202"]
I was looking around for a detailed documentaion of all its Pins
[/quote]


mmmmm this??
<img src="/uploads/db1493/original/3X/e/7/e7c2aad4ffa8048c65ce66e0c40bfe4b87c0d22d.PNG" width="477" height="500">
```

---
## \#5 Posted by: Olloxan Posted at: 2017-11-02T19:25:59.393Z Reads: 135

```
Cool, thanks a lot. Now I have to look for tutorials on how to properly use those pins:)
```

---
## \#7 Posted by: PI3RR3 Posted at: 2018-03-27T17:15:12.306Z Reads: 88

```
Did you finally find a tutorial and manage to program light? i am interesting in using the comm pins of the FOCBOX.
```

---
## \#8 Posted by: b264 Posted at: 2018-03-27T17:18:30.599Z Reads: 85

```
[quote="Olloxan, post:1, topic:37202"]
I was looking around for a detailed documentaion of all its Pins but could not quite find one.
[/quote]

This forum is exactly that.

[quote="Olloxan, post:1, topic:37202"]
I would like to use cruisecontrol and was wondering, if I can implement this in the FOCBOXES or if I would have to program the remote to give a continous signal.
[/quote]

in the FOCBOXes

[quote="Olloxan, post:1, topic:37202"]
Furthermore I would like to use the 5V 1A pin on the FOCBOX to put some LEDs on.
[/quote]

That's 5 watts maximum, minus whatever your radio receiver uses...  They won't be bright, or you might burn up your DRV8302 chip

[quote="Olloxan, post:1, topic:37202"]
Would it be possible to control this pin with the remote like an ON/OFF Switch?
[/quote]

No; you are limited to one RC channel.

[quote="Olloxan, post:1, topic:37202"]
Alternatively would it be possible to control all this using the RX/TX Serial communication Pins on the FOXBOX?
[/quote]

Yes; if you write C99 code.
```

---
## \#9 Posted by: Olloxan Posted at: 2018-03-30T07:46:59.846Z Reads: 44

```
I haven´t continued building yet because I am still waiting on some parts from Enertion and I am still looking for a proper BMS ;) But yeah, once the parts arrive, I will go on with the build, thx for the answers anyway, thats very helpful :)
```

---

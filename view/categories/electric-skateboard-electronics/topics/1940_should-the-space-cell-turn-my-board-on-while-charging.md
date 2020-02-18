# Should the space cell turn my board on while charging?

### Replies: 8 Views: 1135

## \#1 Posted by: evoheyax Posted at: 2016-03-23T21:04:45.671Z Reads: 88

```
I've just started using my space cell recently, and I noticed when I charge it, the fan and lights, which are powered by the receiver turn on.

Is this normal?

I would prefer for the board to stay off while charging if possible, as my fan is a bit whinny sounding. It's kind of obnoxious when I'm charging it during class.
```

---
## \#2 Posted by: EnertionSupport Posted at: 2016-03-24T02:05:52.636Z Reads: 84

```
Yes, when you charge the battery it has the same affect as turning it on. 

It works this way with most BMS modules.
```

---
## \#3 Posted by: longhairedboy Posted at: 2016-03-24T13:13:56.113Z Reads: 67

```
It has to do with the fact that you're supplying power to the mains on the ESC side of the integrated soft switch in the BMS.

Every time i charge my space cell based board i have to also turn on the receiver. This is because not only do the VESCs power up and wait for a PPM signal, they start to think that my 2.4GHz WiFi is some sort of ppm signal and it tries to interpret it as that and starts twitching the motors. 

The only way to get around this without redesigning the BMS to have a soft switch AFTER the charging leads are tapped in would be to add in your own high current soft switch, such as the one on , and then remove the switch from the BMS after permanently shorting the leads so that it is always on. 

This behavior has sort of stopped me from looking for a BMS with an integrated power switch to use with my own packs. I'd rather start making or buying my own soft switches.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-03-24T15:39:48.324Z Reads: 57

```
I was thinking about using dyi's switch. I have one but was going to use it on another build. But may end up having to use it here. The other solution I was thinking of was using 5v switches to turn the fans and lights on and off
```

---
## \#5 Posted by: cmatson Posted at: 2016-03-24T17:06:13.125Z Reads: 50

```
ya, I was going to go with a BMS on my latest pack, but ended up just reverting back to the tried and true loop key. 

Plus, I don't really mind using a standard balance charger- a laptop style charger is nice, but not a necessity in my opinion.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-03-24T17:24:28.274Z Reads: 48

```
i really really like the convenience of not having to pay any attention at all to my charger, so i'm totally going to be using BMSs from now on if i can find some i like. right now i have to go check on my 6S charger like every 30 minutes or so because it's doing its safety thing and will just stop charging after 35 minutes and say its at capacity despite not being anywhere near capacity. I'm going to fiddle with the settings a bit but i'm certain i'll still have to babysit it. I don't have time to babysit a balance charger unfortunately, so i'm trying to get away from them completely if i can.
```

---
## \#7 Posted by: onloop Posted at: 2016-03-24T21:43:53.830Z Reads: 43

```
[quote="longhairedboy, post:3, topic:1940"]
This behavior has sort of stopped me from looking for a BMS with an integrated power switch to use with my own packs. I'd rather start making or buying my own soft switches.
[/quote]

The new SPACE CELL PRO have the switch circuit after the BMS & Before Esc ... so this behaviour won't exist anymore. You can charge the battery & the ESC will not see any power.

<img src='/uploads/db1493/original/2X/7/7f1e75ff995d952cefa05f6196a7b8240ea89da7.jpg'>
```

---
## \#8 Posted by: evoheyax Posted at: 2016-03-25T00:04:28.140Z Reads: 35

```
Looks beautiful. I just hope the shipping crisis can be solved.
```

---

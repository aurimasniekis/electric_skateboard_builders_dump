# Which GT2B mod has enough space for additional arduino nano, hc-05 module and 0.96&rdquo; oled display

### Replies: 12 Views: 900

## \#1 Posted by: laikiux Posted at: 2017-02-05T18:48:55.732Z Reads: 169

```
So I want to build controller with telemetry for vesc.
There should be enough space for arduino nano, hc-05 module and 0.96" oled display. Maybe any of you have modified one of the gt2b cases? Or there already exists one?
```

---
## \#2 Posted by: lox897 Posted at: 2017-02-05T20:08:24.438Z Reads: 159

```
That is a BadWolf V2 case. It can be found on thingiverse
```

---
## \#3 Posted by: num3a Posted at: 2017-02-10T20:58:13.834Z Reads: 132

```
I want to do the same but I don't know how to power gt2b and arduino with the same lipo ...
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2017-02-10T21:07:45.187Z Reads: 131

```
voltage step-down converter?
```

---
## \#5 Posted by: ron Posted at: 2017-02-10T22:26:54.123Z Reads: 121

```
3.3v step down / buck converter.

I'm also going to build a GT2b mod (Sparkle) with Arduino, BT module and OLED display. Need to order a GT2b battery and get a Vesc first ...

Hope it fits in the sparkle GT2B mod...
```

---
## \#6 Posted by: laikiux Posted at: 2017-02-11T07:44:37.466Z Reads: 113

```
Arduino pro mini is suitable for this application.
```

---
## \#7 Posted by: saul Posted at: 2017-02-11T08:08:58.164Z Reads: 114

```
why not just use the nano and bt or nrf for control?
dual radio is overkill...
```

---
## \#8 Posted by: RogerD Posted at: 2017-02-11T10:06:55.563Z Reads: 113

```
Battery for gt2b = hobbyking 2s 800 Mah pack split in half :-)
```

---
## \#9 Posted by: num3a Posted at: 2017-02-11T15:38:06.684Z Reads: 102

```
I've already printed a sparkle too :)

How do you think I can wire all the things ?

Lipo 3.7V  wired to the gt2b and the arduino in parallel (including a step down converter on the arduino side) ?

Sorry for my english ...
```

---
## \#11 Posted by: num3a Posted at: 2017-02-20T15:23:31.230Z Reads: 96

```
Find out that you can use a channel port, they have a 3.3V output.
Which means that the GT2B will power the arduino. The benefits are that you can use the gt2b charge part :slight_smile:
```

---
## \#12 Posted by: Montiey Posted at: 2017-02-24T01:20:26.652Z Reads: 72

```
[THIS](http://www.thingiverse.com/thing:1713157) one has lots of room inside, but the standoffs are too thin and snap off with any rough tightening of the screws. Otherwise, it's comfortable. I'm working on a Sparkle now, it's probably similar.
```

---
## \#13 Posted by: okp Posted at: 2017-02-24T06:36:05.768Z Reads: 65

```
awesome. keep me posted if you want me to make little adjustment to the SPARKLE.
```

---

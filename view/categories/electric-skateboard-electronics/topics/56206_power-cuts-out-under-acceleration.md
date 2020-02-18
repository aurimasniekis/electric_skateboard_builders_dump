# Power cuts out under acceleration

### Replies: 7 Views: 445

## \#1 Posted by: BadleyBoarding Posted at: 2018-05-21T15:45:04.370Z Reads: 93

```
I recently replaced one of the VESC's (hobby king 4.12) as I blew one up, completely my fault. After this it has developed an issue where when accelerating the motors cut out, usually happens after a couple seconds of acceleration which is accompanied by flashing red lights on the VESC. I can get it to do the same thing when unloaded lying on its back but only if I floor it from a standstill.

The settings are exactly the same as I was using before, 45amp max 50amp absolute max with voltage cutoff starting at 36v and ending at 33v on a 10s lipo pack (2x turnigy graphine 5s lipos), VESC's are not connected rather the receiver is split into both. The issues also seems to be more pronounced when the board is fully charged. 

After reading some advice on here I tried straightening the receiver cable and moving it away from the VESC's but didn't make a difference. I ruled out that: it was a temperature issue as it starts happening immediately and doesn't get worse with time, that it was an over amperage issue as its a dual motor config and happens on flat though is slightly worse on hills, that it's a voltage sag issue as it seems to get better as the battery discharges not worse.

Any ideas much appreciated as I'm completely lost at this point, thanks
```

---
## \#2 Posted by: Michaelj1 Posted at: 2018-05-21T15:50:52.910Z Reads: 85

```
I had a similar issue however mine with just an antenna shorting out in my remote. Have you checked for faults on the vesc terminal? Next time it happens, DO NOT turn your board off. Plug your vesc in, go to the terminal and type “faults.” Let me know what it says
```

---
## \#3 Posted by: BadleyBoarding Posted at: 2018-05-21T15:53:12.035Z Reads: 80

```
I haven't, didn't know you could do that will try it when i get home. Currently procrastinating in the library when i should be revising for university finals lol
```

---
## \#4 Posted by: Michaelj1 Posted at: 2018-05-21T15:54:48.243Z Reads: 78

```
If feel you haha. The only time I’ve had the identical issue that you’ve described was after my first version of my board was hit by a car. One of the phase wires for the motor was practically broken and was shorting out or something, the board would randomly slam on the brakes and the Vesc’s would blink red, so if there aren’t any faults it might be your motors.
```

---
## \#5 Posted by: amazingdave Posted at: 2018-05-21T18:21:34.171Z Reads: 59

```
Sounds like your absolute max is too low..... as far as I’m aware it should be 130A. maybe someone more knowledgable will chip in.
```

---
## \#6 Posted by: BadleyBoarding Posted at: 2018-05-21T21:41:04.509Z Reads: 52

```
Yeah I’m getting an over current error, but in the dark as to how Max and absolute max work? Will it only allow absolute max for a few seconds or what’s the difference ?
```

---
## \#7 Posted by: pat.speed Posted at: 2018-05-21T22:36:26.659Z Reads: 40

```
Absolute max must be 130a. Batt max should be between 25 and 50a depending on your battery. Motor max should be between 30-80a. 

Post up your settings if you need some more help
```

---

# I dun goofed today :( ESC dead need new one (EDIT: FIXED it&hellip; So happy)

### Replies: 11 Views: 1059

## \#1 Posted by: irexjr Posted at: 2016-10-29T14:58:30.663Z Reads: 140

```
It was raining today and I was gonna miss the last bus home. I had to ride it out in the rain. I had been preparing my board to be splash proof over the past week getting a waterproof box, filling up holes with water proofing filler etc but it failed me....

RIP my HK 150A Car ESC. The ESC still accepts power and there doesn't seem to be burn marks on the PCB that I can find without desoldering the top PCB from the bottom, its just glitchy. Can't throttle calibrate properly. Motors don't initialize. etc

Was thinking of getting this:
http://www.hobbywing.com/goods.php?id=354&filter_attr=5417.5599

Any one used this before?

I'll be running these with my Benchwheel motors.

http://www.electric-skateboard.builders/t/completed-benchwheel-rebuild-hobbyking-150a-fs-gt2b-6s-lipo-cut-deck/10465
```

---
## \#2 Posted by: thisrealhuman Posted at: 2016-10-29T15:09:13.037Z Reads: 126

```
Are you sure it's the esc and not the receiver?
```

---
## \#3 Posted by: irexjr Posted at: 2016-10-29T15:23:28.373Z Reads: 114

```
I plugged my HKSS programming card into the ESC. Can't get the menu's up either.
```

---
## \#4 Posted by: smudgeUK Posted at: 2016-10-29T15:36:45.413Z Reads: 109

```
Might be an idea to leave it somewhere nice and warm for a while? Could be damp still causing the glitches ... its worth a shot before giving up with it?
```

---
## \#5 Posted by: irexjr Posted at: 2016-10-29T15:41:41.893Z Reads: 102

```
I've already taken it apart and blow dried everything. I'm 100% sure everywhere is dry.
```

---
## \#6 Posted by: JLabs Posted at: 2016-10-29T15:56:00.236Z Reads: 95

```
I have the 6s 120a FVT esc in stock and ready to ship. Only **$55**
https://electric-skateboard.market/product/fvt-6s-120a-esc-sensored/
```

---
## \#7 Posted by: irexjr Posted at: 2016-10-29T17:23:40.902Z Reads: 85

```
Been playing around with the HK ESC and now suddenly allows me to throttle calibrate. After calibration, turn it off and back on. It should start beeping and initializing with the motors but when I turn it back on it just sits quiet. Fan running, nothing happening. HKSS program card has no response either. Looks to me like its the ESC for sure. Not my RX.
```

---
## \#8 Posted by: irexjr Posted at: 2016-10-29T19:20:46.692Z Reads: 74

```
I did it!

I found out what was wrong.... After hours of diagnosing.

I noticed how when I turned the ESC on, it would always go straight into orange light (that's usually calibrating light)
It wouldn't calibrate though even in the orange light unless i hit that reset button again. This lead me to some thinking. The reason why it wouldn't arm the motors nor would the programming card display any menus was because the ESC was going into reset/throttle calibration mode everytime it turned on..

I realised that the ESC switch was obviously broken from water damage. 

De-soldered the red, black and white wires from the switch and I hooked up the red and white wires to a new switch. Just an average small switch you can get from a local hardware store. I then isolated the black wire for future use. And everything works now! 

However, if I ever were to perform throttle calibration again, all I need to do is to touch the black wire onto the other red and white wires.
```

---
## \#9 Posted by: smudgeUK Posted at: 2016-10-29T20:29:59.501Z Reads: 62

```
Good job ! Perseverance pays off.
```

---
## \#10 Posted by: thisrealhuman Posted at: 2016-10-29T20:39:35.625Z Reads: 57

```
Yay SCIENCE!
```

---
## \#11 Posted by: Namasaki Posted at: 2016-10-31T03:25:23.222Z Reads: 31

```
Maybe you can find another 3-way switch to hook it up as before.
```

---

# VESC failure after reverse polarization

### Replies: 19 Views: 871

## \#1 Posted by: Zdzichu Posted at: 2017-09-13T19:30:00.628Z Reads: 130

```
I made a battery where wrong polarity. When I connected the battery to Vesc, the connectors were blown. After that I made the correct polarization, but the radio control does not work. When I power the Vesc up, the red LED flashes three times, then blue and green (on top) remains on. When I plug in my transmitter and pull the trigger, Vesc does not respond, but when I connect Vesc to my computer and click on the "Start detection" button, the motor starts to spin. What should I do to solve this problem if possible?
```

---
## \#2 Posted by: Martinsp Posted at: 2017-09-13T19:38:20.954Z Reads: 129

```
Does the receiver power on? some LED or something on it should turn on when it gets power
```

---
## \#3 Posted by: Zdzichu Posted at: 2017-09-13T19:53:11.777Z Reads: 126

```
Yes. The receiver is working correctly. 
    https://www.youtube.com/watch?v=-YRLD_pi5qY
```

---
## \#4 Posted by: Martinsp Posted at: 2017-09-13T19:54:41.843Z Reads: 119

```
Have you tried to look at it in the BLDC tool in the PPM tab? it might not get the input...
```

---
## \#5 Posted by: Zdzichu Posted at: 2017-09-13T19:59:17.218Z Reads: 112

```
No, becouse I don't know where i can do this. I don't know the BLDC Tool yet.
```

---
## \#6 Posted by: Zdzichu Posted at: 2017-09-13T20:01:36.816Z Reads: 104

```
But i wrote the default configuration, and everything should work.
```

---
## \#7 Posted by: Zdzichu Posted at: 2017-09-13T20:06:16.875Z Reads: 102

```
And yes, in the PPM tab there ins't any input signals
```

---
## \#8 Posted by: Martinsp Posted at: 2017-09-13T20:08:53.994Z Reads: 100

```
When you go to the PPM tab there is a check box and it says display... it displays the PPM input ...signal as the VESC sees/processes it
If you have it set up right it should be showing 50% when you dont pull the trigger
```

---
## \#9 Posted by: Zdzichu Posted at: 2017-09-13T20:12:58.720Z Reads: 97

```
It is showing  50%, but when I pull the trigger it isn't react.
```

---
## \#10 Posted by: scepterr Posted at: 2017-09-13T20:16:21.093Z Reads: 97

```
Did you turn on ppm? Default only has uart turned on
```

---
## \#11 Posted by: Zdzichu Posted at: 2017-09-13T20:21:59.730Z Reads: 87

```
OMG. I'm so stupid, thanks for help, it is working now.
```

---
## \#12 Posted by: Silverline Posted at: 2017-09-13T21:12:31.570Z Reads: 82

```
So you are telling us, that the VESC and receiver actually survived wrong polarity :flushed: ?
```

---
## \#13 Posted by: Zdzichu Posted at: 2017-09-13T21:37:32.566Z Reads: 73

```
Yes, the VESC survived wrong polarity from 6s 60A battery pack. I'm very lucky guy. This is connector who were take the wrong polarity: <img src="/uploads/db1493/original/3X/c/d/cd899c7ed38b64600b86fbabd8bc5d6ef44fb26f.jpg" width="281" height="500">
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-13T21:38:30.322Z Reads: 72

```
Lucky it was that connecter, an xt60/90 wouldnt have melted that quick and fried the vesc
```

---
## \#15 Posted by: Deckoz Posted at: 2017-09-13T21:57:34.616Z Reads: 63

```
Xt60 and deans are both 60a & 100a burst rated..

Xt90 is 90/150
```

---
## \#16 Posted by: GrecoMan Posted at: 2017-09-13T22:03:34.964Z Reads: 63

```
I’ve done the same thing before, billowed out the magic smoke for a good 5 seconds before I burned my fingers and unplugged the battery.  That vesc is still working to this day.  The battery however...

Edit:  mine had xt60s the only thing that happened other than the connectors melting, was that both of my lipos now have cells at .34 volts 😬
```

---
## \#17 Posted by: Clonkex Posted at: 2017-09-14T02:57:25.036Z Reads: 56

```
Whoa that's pretty amazing that they can survive that. Not that I intend to test it myself, but it always feels like if electronics don't have reverse polarisation protection they'll instantly die from it. Apparently not, though :O

That closest I've come to reversing my battery leads so far has been accidentally attempting to plug in a 2 x 3S to 1 x 6S adapter the opposite way to the discharge leads. It made a big fat **_CRACK_** with a blinding flash and burnt one of the JST connector pins but everything is still fine and the battery cells don't seem hurt, so all is well :P

Needless to say I jumped three feet in the air despite being seated...
```

---
## \#18 Posted by: Nordle Posted at: 2017-09-14T10:33:50.685Z Reads: 40

```
[quote="scepterr, post:14, topic:33074, full:true"]
Lucky it was that connecter, an xt60/90 wouldnt have melted that quick and fried the vesc
[/quote]

nope, i vaporised a xt60 in exact the same way, vesc was still working
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-09-14T11:34:16.590Z Reads: 38

```
Oh believe me, I jumped about 10 feet then froze. That’s why I took so long 😂
```

---

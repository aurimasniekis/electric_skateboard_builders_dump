# Converting wireless remote to wired

### Replies: 11 Views: 1634

## \#1 Posted by: jango955 Posted at: 2017-08-17T16:09:36.838Z Reads: 120

```
Hello all! Second post here, second post based on controllers.

So i'm a primitive caveman who thinks wireless is work of the devil and will sooner remove my own scrotum with a teaspoon, than use a wireless controller.

Therefore, does anyone have any info on converting say, a 2.4ghz controller to wired? ( IE - Running the Transmitter output through the ESC bec output instead )

The other option i'm fond of is using a wired wii nunchuck, however i have 0 experience with arduino.

If anyone has anything useful to share, i'd appreciate it...just no more questions on why i'm not fond of wireless remotes... otherwise i'll pray bad things for your children ^_^
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-17T16:12:52.899Z Reads: 120

```
Haven't done it myself, but I imagine you'd just directly connect the potentiometer directly to the servo pins. 

I personally feel that this is more dangerous as it has more room for error. A wire dangling and moving around all the time is under much more stress and can fray faster than a stationary one. There's also the danger of accidentally breaking it with your leg or other environmental variables. Having to bail on your board while holding (or even not holding) your remote will probably cause damage to the cable and remote.
```

---
## \#3 Posted by: velox Posted at: 2017-08-17T16:27:54.352Z Reads: 111

```
I've used a wired connection to communicate via UART when I started building my first board. The problem was that the cable and the connectors gets damaged quite easily by pulling/dragging etc like Jinra describes. Also the cable may be a problem if you need to jump off the board. Luckily there is an emergency timeout option in BLDC tool. Better go for a wireless remote. I'm using BLE modules now and so far I haven't had any problems.
```

---
## \#4 Posted by: Jedi Posted at: 2017-08-17T16:30:50.199Z Reads: 105

```
Use the wired nunchuck. The VESC has a built in wiiceiver, so plug n play. 

And once you realize how silly it is to have a wired controller, simply swap out for a wireless nunchuck.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-08-17T16:38:34.120Z Reads: 98

```
[quote="Jedi, post:4, topic:30899"]
The VESC has a built in wiiceiver, so plug n play.
[/quote]

The vesc does not have a built in wiiceiver. It has code to work with the wii nunchuck, but it does not have a receiver or transmitter in itself. You need to wire a receiver for the wireless one, I'm not sure about the wireless one though.
```

---
## \#6 Posted by: bmcm Posted at: 2017-08-17T17:12:38.537Z Reads: 93

```
Right now I use a wired nunchuck but replaced the cable with a longer cat5e, and a jack that plugs into the UART port. I also have a wireless nunchuck whose receiver also plugs into that cat5 jack for easy swapping.
```

---
## \#7 Posted by: jango955 Posted at: 2017-08-17T17:35:08.930Z Reads: 86

```
Any chance you could provide further information to how with works? does the nunchuck plug into an arduino board and then the esc? or have you a similar set up?
```

---
## \#8 Posted by: bmcm Posted at: 2017-08-17T17:40:53.335Z Reads: 88

```
If you're asking me, my current setup just has the nunchuck plug directly (with a cat5e male + female jack in between) into the VESC. However, yes, I do plan on having it (wired or wireless) plug into an arduino board over i2c, then convert to PPM into the VESC, and also have the arduino board read from the VESC over UART to then power an OLED either on the deck or in the controller.
```

---
## \#9 Posted by: jango955 Posted at: 2017-08-17T18:02:35.163Z Reads: 79

```
I don't suppose you could send me some details images of your wiring? specifically from the bec --> cat5 and then into the nunchuck itself
```

---
## \#10 Posted by: bmcm Posted at: 2017-08-17T18:14:55.491Z Reads: 75

```
I'll see what I can do (when I get home from work).
```

---
## \#11 Posted by: bmcm Posted at: 2017-08-18T02:03:14.039Z Reads: 62

```
You can find wiring diagrams for connecting the wireless receiver or the wired controller to the I2C port of the VESC. And it doesn't matter which wires you map to in the cat5e cable - as long as they're the same on both ends. There are 8 wires and you only need 4 (5V, GND, SCL, SDA), leaving 4 for future use (like an OLED :slight_smile:)

 <img src="/uploads/db1493/original/3X/f/8/f8e5380d0c5a25d1755dee7cfd2f9d21eb0dd0e8.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/8/4806de5d7123a239aa17d7d3206bf7aa4ccce268.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/2/523a9b626c4e88c14b2af4e4cdf20af68ccb72a8.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/0/a/0adf751bbe955b24aa67b76b43689635cfcbd370.jpg" width="374" height="500">
```

---

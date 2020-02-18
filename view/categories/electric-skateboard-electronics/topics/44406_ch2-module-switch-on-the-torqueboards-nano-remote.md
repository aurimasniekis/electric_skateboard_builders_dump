# Ch2 module switch on the torqueboards nano remote

### Replies: 13 Views: 1221

## \#1 Posted by: Leo31016 Posted at: 2018-01-23T03:44:15.000Z Reads: 134

```
so I have a nano remote from torqueboards, and I'm trying to figure out what exactly the ch2 extension switch can do. Does anyone know what can I do with it?![image|379x500](upload://eOFhLUB3xHixntlabi6ehdOzoci.jpg)
(stole the picture from this [thread](http://www.electric-skateboard.builders/t/nano-v2-full-review/25159/12) because I lost my manual lol)
```

---
## \#2 Posted by: Blasto Posted at: 2018-01-23T03:54:59.811Z Reads: 125

```
![image|281x500](upload://zfmJSnLbgW4tFNm02BxiFWbjhia.jpeg)

Hold this switch for 5 secs or so, it will toggle ch2 on and off. It’s not a ppm signal but a 0-5V signal

You cant use this signal to drive leds, but you can use it to drive a transistor that drives leds
```

---
## \#3 Posted by: Leo31016 Posted at: 2018-01-23T04:00:00.104Z Reads: 117

```
[quote="Blasto, post:2, topic:44406"]
leds
[/quote]
 thanks man, but I have a question completely irrelevant to this topic
what is cruise mode?
```

---
## \#4 Posted by: Leo31016 Posted at: 2018-01-23T04:00:42.119Z Reads: 116

```
I know what it is, but doesn't know how to switch it on
```

---
## \#5 Posted by: Blasto Posted at: 2018-01-23T04:02:57.638Z Reads: 114

```
No cruise on this remote
```

---
## \#6 Posted by: Deckoz Posted at: 2018-01-23T04:03:44.408Z Reads: 115

```
[quote="Blasto, post:2, topic:44406"]
Hold this switch for 5 secs
[/quote]

Dude.. I always wondered why mine didn't do shit... I wasn't holding it long enough haha thanks dude
```

---
## \#7 Posted by: Bensaida Posted at: 2018-01-23T04:35:16.356Z Reads: 110

```
how would you connect LEDs such as this: https://www.ebay.com/itm/WS2812B-5050-RGB-LED-Strip-30-60-144-LEDs-M-ws2812-IC-Individual-Addressable-5V/262452005540?hash=item3d1b5bcaa4:m:mkMwXOyKYoE3TxVrA-ee05w to the remote?
```

---
## \#8 Posted by: Deckoz Posted at: 2018-01-23T04:41:04.974Z Reads: 108

```
Well...you can't "control" those LEDs from this remote...

But you could use a RC switch to control the on/off of the power source of those LEDs 

https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html
```

---
## \#9 Posted by: Bensaida Posted at: 2018-01-23T04:44:56.283Z Reads: 109

```
so i just buy any LED strip, plug it into the switch, then i can turn them off/on with the remote?
```

---
## \#10 Posted by: Deckoz Posted at: 2018-01-23T04:47:36.291Z Reads: 108

```
Not quite..
Ws2812b LEDs requires a digital.control signal... If you buy the led strip with a controller.. or make an Arduino to control them... You could them use the rc switch to turn on or off the 5v power supply to the LEDs.. effectively turning the LEDs on and off..

But ws2812b will not light up without a Digital controller
```

---
## \#11 Posted by: Bensaida Posted at: 2018-01-23T06:07:15.291Z Reads: 100

```
do you know any bike/skateboard lights that could use that tranciever?
```

---
## \#12 Posted by: Deckoz Posted at: 2018-01-23T06:12:43.377Z Reads: 100

```
Any of them can? You just put that in between the light and the battery... It's like a power switch... Positive from the battery goes to one red wire..comes out the other red wire.mmthe servo lead goes to the receiver... When it's on it connects the two red wires for power to pass through...
```

---
## \#13 Posted by: lambievu0916 Posted at: 2018-03-04T19:16:32.352Z Reads: 77

```
so the button is there just so u can toggle another future u can add on the board correct? Also can anyone explain the led or have a visual of it because I'm still kind of confused on how to add LED.
```

---

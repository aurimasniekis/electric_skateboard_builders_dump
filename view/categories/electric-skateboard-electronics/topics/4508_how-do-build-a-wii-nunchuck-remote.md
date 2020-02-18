# How do build a Wii nunchuck remote?

### Replies: 25 Views: 5859

## \#1 Posted by: Airmacx Posted at: 2016-06-10T08:11:17.974Z Reads: 359

```
I've seen a few that have been self made, I think @jacobbloy 's channel and he had one that he was able to program himself. But I'm looking at controller options, I want a wireless bluetooth whatever it is, and the Wii one seems to look the best, really not into the RC car controllers. I was wondering can I just buy a normal Wii nunchuck from the shops, and just modify it, put a chip in it or something. And how much will it cost?
```

---
## \#2 Posted by: zk8_builder Posted at: 2016-06-10T08:17:58.478Z Reads: 361

```
You could do something like https://m.youtube.com/watch?v=zaTskMjpXtA this
```

---
## \#3 Posted by: zk8_builder Posted at: 2016-06-10T08:18:05.109Z Reads: 356

```
At the end
```

---
## \#4 Posted by: Paulf Posted at: 2016-06-11T15:40:03.316Z Reads: 320

```
A friend of mine gave me a wii nunchuck and after removing most of the plastic and circuit board inside the nunchuck I managed to fit in a 1s tiny lipo (~300mah, which is ridiculously too much, I haven't been charging the remote for a month now and still got juice!), an atmega328 which I've programmed and an nrf24l01. 
This implies the need for another atmega or arduino like board as well as another nrf24l01 in the skateboard. I've been riding this setup for a few months and it seems very reliable. 
Tell me if you're interested in doing what I did, I would be very happy to help you
<img src="/uploads/db1493/original/2X/d/d7157717491a158e3dbf7b42aaec24473d99bddd.jpeg" width="669" height="499"><img src="/uploads/db1493/original/2X/7/73484c9ed113f1e05536e81bd1cd1f2659019c4d.jpeg" width="373" height="500"><img src="/uploads/db1493/original/2X/4/426e0317a834f0dc7c9a5db1e412feb45894f0b0.jpeg" width="669" height="499">
(We can't see the nrf24l01 on the pictures)
```

---
## \#5 Posted by: Airmacx Posted at: 2016-06-11T15:57:03.293Z Reads: 286

```
Looks great. The parts needed won't take up a lot of space on the board right? Including the cost of a nunchuck how much is the build of this.
```

---
## \#6 Posted by: Paulf Posted at: 2016-06-11T16:10:52.347Z Reads: 283

```
No, it doesn't take much space on the board at all. 
Without the nunchuck and the small lipo in the nunchuck (which I'm sure you can buy for very cheap) I'd say it costed me less than 10€
Let's add 10€ for the lipo and small bms for it and you're done for 20€ -> cheapest controller ever (it still needs quite a bit of time to build it)
I don't know how much is a nunchuck if you ain't got one already but its gotta be cheap
```

---
## \#7 Posted by: Airmacx Posted at: 2016-06-11T16:21:32.356Z Reads: 272

```
Alright cool. Probably anywhere from $10-$20 where I'm from. Could you tell me how you did this?
```

---
## \#8 Posted by: Paulf Posted at: 2016-06-11T16:25:05.486Z Reads: 269

```
Yeah of course
Just give me a little bit of time so I can write a good post with pictures, the code for the controllers, the wiring and links to the different parts :slight_smile:
```

---
## \#9 Posted by: Airmacx Posted at: 2016-06-11T16:29:28.251Z Reads: 256

```
Looking forward to it 😊.  It's 2am for me now so I gotta sleep, but I'll check first thing in the morning.
```

---
## \#10 Posted by: XIII Posted at: 2016-06-11T18:48:35.568Z Reads: 253

```
Would try it aswell with a good guide !
```

---
## \#11 Posted by: Nordle Posted at: 2016-06-11T18:58:53.965Z Reads: 246

```
Hey @Paulf, which code do you use? Is it your own or someones from E-S forum maybe? I'd like to build similar remote (preferably with Rolinggeckos code, cause it's UART has cruise control, reverse, led indikators for remote & board battery, and an oled wich i would skip). But I really could need some help also.

A good guide would be a great tribute to the community!
```

---
## \#12 Posted by: XIII Posted at: 2016-06-11T19:38:11.725Z Reads: 234

```
I had the same question, does your nunchunk also feature the cruisecontrol function? 
And maybe other functions?
```

---
## \#13 Posted by: Paulf Posted at: 2016-06-11T20:01:11.505Z Reads: 225

```
The code is mine, it has cruise control
Atmegas/arduinos does support uart so, I think that I can easily tweak the code in order to make it uart compatible
However my remote ain't got all the other features (battery LEDs and screen)
(The remote battery is more than big enough so that i never have to worry about and I mounted a led on the top of my board which I can always see while riding and  which blinks according to the boards battery level )
By the way, have you got a link to the remote/code you're talking about? Seems interesting
I'm happy to help you with all the electronics/code questions you have
```

---
## \#14 Posted by: Paulf Posted at: 2016-06-11T20:02:54.688Z Reads: 213

```
My remote features cruise control and I can  also change the color of the led strips under my board with one button on the remote
```

---
## \#15 Posted by: Paulf Posted at: 2016-06-11T20:04:42.273Z Reads: 209

```
Ok guys, I'm definitely doing a detailed guide soon! but please give me a bit of time cause I got a lot of exams to prepare these days :confused:
Hope you understand
```

---
## \#16 Posted by: Nordle Posted at: 2016-06-11T21:40:51.470Z Reads: 209

```
[quote="Paulf, post:13, topic:4508"]
By the way, have you got a link to the remote/code you're talking about?
[/quote]
[Rollonggecko](https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812&hilit=rollinggecko) github link in the first post there. Required Vesc code for this project is already merged into VESC firmware!
```

---
## \#17 Posted by: kyo Posted at: 2016-12-27T11:50:09.849Z Reads: 173

```
Hi @Paulf. Would please you do a turtorial on this please?
```

---
## \#18 Posted by: K.kris Posted at: 2017-01-09T15:44:06.094Z Reads: 170

```
He Paul! I Just ordered All the parts you Lister above here and I want to try to build this controller. But could you post a link too your code. Or tot a tutorial. Code would be good enough I love to experiment with my projects and learn while doing but only if I get it eventually.
```

---
## \#19 Posted by: Paulf Posted at: 2017-01-09T20:56:50.176Z Reads: 170

```
I'm sorry guys I really can't find the time to do a proper tutorial now but my code is always up to date here https://github.com/PaulFl/Arduino
I've been making another of these remotes not long ago, it works well <img src="/uploads/db1493/original/3X/9/1/911fac88ef62fdc8dc1882621a8b831b0d808331.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/3/4350198bd22c4fd75c5c56226aef3240555db9ae.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/7/a764ed5ade796f7c555fc3fc59197634b3fa1721.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/8/b/8b370729bec3579514bc8fa070b252a96b4d8dc3.jpg" width="374" height="500">
The code you wanna check is esk8_v2_remote for the remote and esk8_v2_sensitive for the remote
Although I don't have the time to write a full tutorial, I would be very happy to help you whenever you have a doubt or a question
```

---
## \#20 Posted by: K.kris Posted at: 2017-01-11T19:08:08.826Z Reads: 160

```
NO worries!
Thanks for the code tho! 
Its atleast something. If you ever get the time do the tutorial let is know. 
Thanks man!
```

---
## \#21 Posted by: MadPatch Posted at: 2018-11-16T16:21:58.575Z Reads: 71

```
I know I am a bit late, but @Paulf do you have a schematic?
```

---
## \#22 Posted by: Paulf Posted at: 2018-11-16T16:33:53.525Z Reads: 71

```
I currently don't but I might be able to do one for you if I find time in the week-end
```

---
## \#23 Posted by: MadPatch Posted at: 2018-12-16T14:47:30.166Z Reads: 64

```
If you still have time to make a quick schematic that would be greatly appreciated!
```

---
## \#24 Posted by: MadPatch Posted at: 2018-12-21T19:30:03.173Z Reads: 50

```
I cant find a pinout of the joystick in the remote, how did u determine it?
```

---
## \#25 Posted by: Paulf Posted at: 2019-01-12T22:03:18.968Z Reads: 44

```
Sorry for the very late reply but I finally found some time for a schematic, here it is:  https://github.com/PaulFl/Arduino/blob/master/esk8_v2_remote/Eks8_remote.pdf
For the joystick of the remote, for each axis, you do have 3 pins, the middle one is the analog signal and the ones on the sides are for VCC and GND
```

---

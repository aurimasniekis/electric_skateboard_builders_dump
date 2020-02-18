# Arduino VESC Nunchuck controller (Emulates NRF controller)

### Replies: 6 Views: 1992

## \#1 Posted by: boards Posted at: 2016-08-03T03:28:26.640Z Reads: 227

```
https://www.youtube.com/watch?v=4HWATHOKTzU

https://www.youtube.com/watch?v=1ozh3tdX8kM

You can communicate with VESC like NRF nunchuck with arduino. It's pretty simple the struct is in bldc tool, but keep in mind you have to calculate an additional CRC (separate from one calculated on chip). Just got it working this morning and as soon as I did I got a DRV8302 fault... Fortunately I have another VESC coming later this week. I also ordered 10 DRV8302 chips and 5 DRV8301(Though hopefully I won't need them with 6.0) chips through work so I won't have that problem anymore :p 

The DRV8302 fault is probably because I was spinning the motor without motor detection (Had to reflash the vesc firmware a few times with a custom build  to add some debugging info to terminal.)

All you need is arduino, nunchuck, 2 RF24 modules (You can get 10 for like 3-4$ on ebay). I also used a disassembled usb battery for power (Thinking of swapping it with lipo so I can fit in nunchuck). I'll post code later when I make it work with unmodified VESC firmware and maybe a small guide.
```

---
## \#2 Posted by: mason Posted at: 2016-08-03T03:30:49.864Z Reads: 197

```
video is private
```

---
## \#3 Posted by: boards Posted at: 2016-09-03T05:10:58.001Z Reads: 163

```
Some updates on this. I added some data for the best to return with the keep alive packets. Unfortunately on first test I did a little backroll off the board (wear your helmet folks) because one of the shitty wires had snapped. This also cracked the display.

 Resoldered it up and ordered some more oled displays. Thinking about adding a microsd writer to log data. 

<img src="/uploads/db1493/original/2X/4/4d5dbe643fb585652d505c6d4d550b8f5547d981.JPG" width="690" height="388"><img src="/uploads/db1493/original/2X/a/ad74741fe1da7afbaf4411adb6f8c6fcf5729fc5.JPG" width="666" height="500">

Almost thinking about diving into kicad and designing a nice board to stick in a real case, but iunno, i'm no ece.

I kinda even wanna make a board with a nRF52832, it's a pretty expensive soc, but it does everything and could sync data to a phone. Some of these chips you can probably make a remote you never have to turn off (listen for keep alive packets at very low rate).

----------
```

---
## \#4 Posted by: Patate Posted at: 2016-11-29T17:43:50.604Z Reads: 109

```
Wow impressive build ! I am currently programming a similar remote with Nunchuck + Arduino 32U4 + RF24, and I would love to build up on your code if you have a Github repository :)
```

---
## \#5 Posted by: m.kicker Posted at: 2018-07-09T08:17:56.801Z Reads: 46

```
HI! I planned to connect an arduino to the VESC built-in NRF chip. But I can't even receive alive packet. Do you mind sharing your code ?

Thanks !
M
```

---
## \#6 Posted by: relations99 Posted at: 2019-03-30T03:04:12.326Z Reads: 22

```
@boards Could you show how to setup the vesc to directly connect the NRF to the vesc? Also the arduino code, do you have an example? I can try to figure out the rest! Thanks so much for your work bud
```

---

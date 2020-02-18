# FVT 120A esc beeping on start up

### Replies: 12 Views: 282

## \#1 Posted by: Harp Posted at: 2018-07-26T05:06:12.536Z Reads: 72

```
I've been using the FVT 120A esc for a while now and it's given me no problems except for a minor issue that I hope someone can help answer. Every time I power on the board the esc makes 5 long beeps followed by the regular tune that plays on startup. Does anyone who has owned this esc know what these 5 beeps mean? The manual doesn't have any info on this. It might be important to mention that this esc is connected to an Arduino instead of a receiver for a controller and it is powered by 18v instead of 6s.

Edit: I meant to say 5 beeps instead of 3.
```

---
## \#2 Posted by: Silent_bob52637 Posted at: 2018-07-26T10:16:30.952Z Reads: 60

```
Mine has always behaved that way on startup from the day I first used it
```

---
## \#3 Posted by: pat.speed Posted at: 2018-07-26T11:23:56.534Z Reads: 55

```
It might be low voltage, try connecting it to a 24v psu and see if something similar happens
```

---
## \#4 Posted by: Silent_bob52637 Posted at: 2018-07-26T13:47:08.967Z Reads: 46

```
Mine was connected to an Arduino aswell I think it has to do with the Arduino taking time to boot after the Rx cable gets power
```

---
## \#6 Posted by: Harp Posted at: 2018-07-28T05:03:01.291Z Reads: 24

```
Shouldn’t the Arduino already be booted if the RX cable is sending power?
```

---
## \#7 Posted by: Harp Posted at: 2018-07-28T05:16:48.019Z Reads: 21

```
I just tried 24 volts but the esc still produces those 5 initial beeps.
```

---
## \#8 Posted by: pat.speed Posted at: 2018-07-28T05:33:22.528Z Reads: 21

```
Ahhh, yep that’s just the sound it makes on startup signally how many cells are connected, 1 beep = 1 cell, 3 beeps = 3cells and so on. 

I’m not sure why it didn’t do this before, but my Xcar beast esc does this on start up
```

---
## \#9 Posted by: Harp Posted at: 2018-07-28T06:13:39.493Z Reads: 21

```
Alright, I guess I'll have to buy the USB programming link and disable this sound. Ty for the help.
```

---
## \#10 Posted by: 2Old2Sk8 Posted at: 2018-07-28T06:16:48.345Z Reads: 20

```
Can I ask where you found the manual?  The only one I can find on the FVT site is called "FVT'S manual for Electronic Skateboard ESC" and can't be opened in Word 2016 or Wordpad.  Is there another one available somewhere?
```

---
## \#11 Posted by: Silent_bob52637 Posted at: 2018-07-28T10:56:19.442Z Reads: 18

```
I meant the ppm cable has been powered up
```

---
## \#12 Posted by: pat.speed Posted at: 2018-07-28T11:38:17.992Z Reads: 19

```
I don’t think the noise can be disabled, well at least on the Xcar it couldn’t be disabled
```

---
## \#13 Posted by: Harp Posted at: 2018-07-28T21:43:46.807Z Reads: 13

```
Manual:
https://img.banggood.com/file/products/20151109031117FVT%20ESC%20Manual_141227.pdf
```

---

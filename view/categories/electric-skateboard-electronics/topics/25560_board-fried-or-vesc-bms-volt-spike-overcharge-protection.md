# Board Fried? Or VESC/BMS volt spike overcharge protection?

### Replies: 12 Views: 925

## \#1 Posted by: 1tczx Posted at: 2017-06-17T07:47:25.035Z Reads: 96

```
Hi I just got a board went down hill with full battery. Board suddenly shut off and refuses to turn on again. However, whenever I press the power button, power light comes on, but when I remove finger, power light goes off

Board refuses to turn on. It doesnt seem like theres any electrical component fried from the picture. 
<img src="/uploads/db1493/original/3X/5/3/536870a5b28964295e37ba39f9ed468600be85eb.jpg" width="374" height="500">
Therefore, I am guessing it is a software problem where my vesc has voltage surge protection on? How do I reset VESC?

Help needed and thanks in advace

Cheers
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-06-17T22:13:07.050Z Reads: 75

```
My first though is why you would go down hill with a battery charged fully at 4.2 volts per cell? Can you read any error codes off the VESC?
```

---
## \#3 Posted by: 1tczx Posted at: 2017-06-17T22:48:44.058Z Reads: 68

```
Thanks for your reply @chuttney1 How do u know if it is 4.2V per cell just from the picture? 

I havent got a VESC to usb cable yet, this board was pre-made. Should I get a cable or is there other ways to remedy?
```

---
## \#4 Posted by: chuttney1 Posted at: 2017-06-17T23:30:45.697Z Reads: 66

```
[quote="1tczx, post:3, topic:25560"]
Thanks for your reply @chuttney1 How do u know if it is 4.2V per cell just from the picture?
[/quote]

The photo doesn't show it, but this is common knowledge one you understand what a cell's maximum and minimum voltage. Absolute max voltage of a lithium cell is 4.2 volts unless otherwise stated by the manufacture. I don't know how many cells in series your battery is. You said you "went down hill with full battery," this says 4.2V per cell to me.


[quote="1tczx, post:3, topic:25560"]
I havent got a VESC to usb cable yet, this board was pre-made. Should I get a cable or is there other ways to remedy?
[/quote]

Well, that explains what is in the photo. Who made it? With pre-made, this is a different story and does not use a VESC controller unless stated by seller.  I own a premade regarding experience. If the ESC doesn't have an usb connection port there's not much I know you can do unless you're good at diagnostics stuff with an oscilloscope, but that's for experts. I will have others chime in so it is not help from one person. They might know something that I don't.

Just for reference, VESC uses a USB mini-b cable which I think you have if you have a stockpile of old cables.
```

---
## \#5 Posted by: 1tczx Posted at: 2017-06-18T01:08:58.342Z Reads: 58

```
@chuttney1 It has no usb jack whatsoever. I thought I could hook it up with the 4pin  connector or something. Looks like I do need some special help then
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-18T03:11:10.348Z Reads: 57

```
I experienced this problem where you push the button and the power comes on but when you release the button the power goes off. 

I'm betting you  have a faulty button switch.

I'm currently using this one and it has been dependable. 
https://www.amazon.com/dp/B00YS25ZEM/ref=cm_sw_r_cp_apip_G5WX4QilR1THS
```

---
## \#7 Posted by: 1tczx Posted at: 2017-06-18T07:14:05.727Z Reads: 52

```
@Namasaki thanks for your input bro. But I doubt it is a faulty switch? if it is so then I would able to connect to it while holding the button down and keeping light on. However, with light on and button held down, board is not technically on as I cant connect to it too
```

---
## \#8 Posted by: 1tczx Posted at: 2017-06-19T18:52:02.595Z Reads: 45

```
@Namasaki @chuttney1 Hi my board is the Onan  here: https://www.onan-booster.com/product-page/onan-x1-electric-skateboard-booster-w-93mm-dual-motor-wheel 

  Any help on this?
```

---
## \#9 Posted by: sl33py Posted at: 2017-06-19T19:07:46.509Z Reads: 43

```
@1tczx - this looks really similar to Landwheel, but not a simple re-badge.  

Your best bet is to contact Onan for support.  You likely have a warranty, and messing with it too much might void it.  I would go through troubleshooting they walk you through, and not mess with it otherwise.

It's not a VESC, at least what i read on site, and see in the picture above.  VESC is specific to Vedder's ESC = VESC.  Just an ESC  (electronic speed controller).

Good luck!
```

---
## \#10 Posted by: 1tczx Posted at: 2017-06-20T06:19:33.242Z Reads: 35

```
Thanks for the help guys appreciate it!
```

---
## \#11 Posted by: TarzanHBK Posted at: 2017-06-20T13:43:13.120Z Reads: 30

```
You can see the ESC in the picture. This is not a Vesc and I think you just overcharged your batteries and the ESC has some sort of over voltage protection. So as soon as you try to switch it on, it´s switching off to prevent any damage.
Best would be to hook you batteries on an Multimeter and see whats going on.
```

---
## \#12 Posted by: 1tczx Posted at: 2017-06-20T17:39:15.347Z Reads: 26

```
@TarzanHBK thanks for the tips. Should'nt I be hooking my multimeter to the ESC instead of the battery?  I have tried draining the battery a little too will that help?
```

---

# Reintech Rt 60c2 Chinese esc substitute info

### Replies: 14 Views: 1191

## \#1 Posted by: Cieszyn Posted at: 2018-10-05T06:05:03.895Z Reads: 151

```
Hi everyone 
I have just built my first cheap setup. I thought I have bought the typical chinese esc substitute
https://img.staticbg.com/thumb/view/oaupload/banggood/images/0E/99/08009779-d370-4244-966c-57cf255e88e7.JPG
 but instead I received this funny red one
https://cbu01.alicdn.com/img/ibank/2017/894/611/4380116498_199196347.jpg

I have managed to get it running but I have a problem. 
it accelerates very slowly and when I let off the gas it builds up speed almost from the 0, so it's nearly impossible to slow down a bit before traffic light and zip through cross roads, typically I end up rolling slowly in the middle of the cross roads... Which is kind of dangerous. it also reaches top speed of 25km/h at 36v.

How to boost the acceleration? Is It the signal from the remote (change remote for newer one), is it esc (buy another Chinese substitute, more legitimate this time)? Can I somehow modify the existing esc?

If you have some info on this controller, please also give it here
Best
Tomasz
```

---
## \#2 Posted by: telnoi Posted at: 2018-10-05T06:20:58.734Z Reads: 138

```
Why not contact the reseller for support?
Seems like a few people did not get what they paid for. I'd send it back.
```

---
## \#3 Posted by: dareno Posted at: 2018-10-06T22:30:35.834Z Reads: 115

```
Presumably you have checked the speed switch on the remote?  Don't mean to sound obvious but sometimes its the simple things....
```

---
## \#4 Posted by: Cieszyn Posted at: 2018-10-07T02:59:14.038Z Reads: 102

```
Yes, the problem is i haven't recognized the wrong product from the beginning and. Had to hot glue it all over to work reliably. Now it's done deal.
On low speed its 15km/h on high speed its 25km/h
```

---
## \#5 Posted by: Cieszyn Posted at: 2018-10-08T05:11:09.828Z Reads: 87

```
The question is: would the board accelerate faster if I changed to newest remote controller?
```

---
## \#6 Posted by: yuweng Posted at: 2018-10-11T15:50:47.302Z Reads: 80

```
No it won't, it will only accelerate faster when you increase the voltage, modded my generic Chinese ESC to 16S, all you need is swap a smd resistor for that :sunglasses: 

Take a high res photo of your board where the 6S & 7S is, attach it here & i'll guide you, hopefully its the same. In the mean time, you can also try increasing 1S at a time, no worries, it won't blow up, the wheels will only stop spinning when the voltage gets too high. Eg. Yours is 10S, add another 18650 = 11S & so on & so forth. i think it'll stop working when voltage is above 48 Volts.
```

---
## \#7 Posted by: Cieszyn Posted at: 2019-02-04T02:33:08.055Z Reads: 69

```
Hi, it wasn't that easy messing up with baterries, since I have a pretty strange setup not easy to add or remove cells.

However I bought flipsky dual and my main problem is gone. I can set the throttle curve, I think it accelerates much faster on the same setup, and most importantly it's much safer since it accelerates instantly while cruising (that was the biggest issue with the old one, it didn't pick up the speed when already cruising, it accelerated fine only from stop). 

In my opinion reintech Rt 60c2 has all the features needed for esc for decent price, but with firmware I had its very dangerous and unrideable.
```

---
## \#8 Posted by: bogas Posted at: 2019-04-28T06:50:43.186Z Reads: 54

```
Hello.
 I have an Archos SK8 board, but I do not have a remote control for it.
 ESC is Reintech RT-60D, 7S power supply.
 The board does not connect to the standard 2.4GHz RC apparatures.  I see NRF24L01 on the ESC.
 Does anyone have knowledge of how the remote control would pass with it or where on the ESC to look for a place to connect pwm?

Greetings,
Mateusz

[20190425_171308_resize_23|243x500](upload://wtPMyf01sHoocOfL36H007hdCN9.jpeg)
```

---
## \#9 Posted by: Cieszyn Posted at: 2019-04-28T23:15:06.258Z Reads: 48

```
I have seen spare remotes on ebay, I don't know if it would work with reintech though. Can't find one right now. They come without receiver and it says on auction they work only with esc substitute like reintech and alike.
Best
TC
```

---
## \#10 Posted by: bluegreen Posted at: 2019-04-29T04:54:14.265Z Reads: 41

```
I have an onan x1 and it accelerates the same way. Almost certain it is not the remote, it is the software in the ESC to make sure that you are not thrown off by sudden acceleration.

But as you mentioned, and I agree with you, it is probably more dangerous because you cannot get going when you need to. It's the main reason I'm using VESC, the ability to control these things.
```

---
## \#11 Posted by: Schanilong Posted at: 2019-05-14T19:35:53.858Z Reads: 30

```
where can i get this controller reintech rt60 c2 v1.2? on my board only one motor is working, i think i destroyed the controller riding in wet conditions, so i want to buy a new one. if i chage the motors, the other one is running, so motors are good, battery is good. BR
```

---
## \#12 Posted by: Windsongdj Posted at: 2019-07-24T18:15:03.403Z Reads: 23

```
Hi I'm new here where did you get that board and controller because I need one?
The search I did brought me here.
```

---
## \#13 Posted by: Cieszyn Posted at: 2019-07-24T18:59:39.313Z Reads: 20

```
Ebay: esc substitute - that's where I got it from
There were different versions of it.
```

---
## \#14 Posted by: Draomian Posted at: 2019-07-25T15:39:11.823Z Reads: 12

```
Hi everyone, im brand new here.

I bought a chinese eléctric sk8 with reintech 60 C2 v1.2.

It worked fine several months, but suddenly, days ago, it stops randomly. When i begin to acelerate, it stops and it turns off.

I find that i cannot connect vía Bluetooth for vesc controling, or i don't know how to do it.
Motors are ok 

Any ideas for repairing this issue?

![IMG_20190725_115416007|281x500](upload://9uEaTJDXJAH9stl2ZSpiCHk5Qct.jpeg)
```

---

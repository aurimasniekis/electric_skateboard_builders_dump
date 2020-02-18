# ISO Vesc with bluetooth capabilities

### Replies: 28 Views: 324

## \#1 Posted by: RealaPolarBear Posted at: 2019-01-22T06:09:34.348Z Reads: 114

```
So currently, I have a torqueboards VESC working with my build and I originally hoped to use a Bluetooth module I got from Jared at Build Kit Boards. I recently learned that the torqueboards VESCs do not have Bluetooth capabilites. Does anyone have any suggestions of VESCs that have Bluetooth capabilities while being the same size as the torqueboards vesc if not smaller(I am working in tight quarters and need it to be able to fit on it’s side, there’s is just enough room for the Vesc I have now in my enclosure) ? And if possible on the cheaper side but something reliable (I know, cheap = not reliable, but I’ll see). I’d like it to be reliable in FOC and be able to be reliable especially when climbing hills (and some varient of 4.12 with ble capabilites). Thanks.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-22T06:12:22.552Z Reads: 109

```
How can a VESC based esc don’t support Bluetooth? 
Don’t get it.
```

---
## \#3 Posted by: RealaPolarBear Posted at: 2019-01-22T06:16:43.930Z Reads: 102

```
I don’t know man 😂, I even contacted them questioning it. Apparently it’s because they “have no need for it”. I don’t me to bash torqueboards, don’t get me wrong I love their products and they’re great, but this is my only complaint. (I still use their products on my builds though).
```

---
## \#4 Posted by: Holyman92 Posted at: 2019-01-22T06:26:28.239Z Reads: 95

```
Their 4.12 escs are meh... almost caught my board on fire.... but I still use their motors and other products, just not their esc's

As for their 12s esc that's not a vesc
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-22T06:27:59.097Z Reads: 89

```
maybe i´m wrong, but there is an uart port on the tb vesc and they run the usual firmware. there is no reason why a bluetooth module shouldn´t work!
```

---
## \#6 Posted by: J0ker3366 Posted at: 2019-01-22T06:32:32.806Z Reads: 83

```
Bluetooth should be capable on TB vesc. I'm about to find out for myself. And I know I've seen a couple of builds here with TB and BT
```

---
## \#7 Posted by: RealaPolarBear Posted at: 2019-01-22T06:35:48.284Z Reads: 82

```
Lemme know what you find because I know they have the correct port, but they said it doesn’t support it, also if it does support it then what am I doing wrong, I have set the module up on my phone, I have set the module to 9600 and have the VeSC setting to ppm and uart so I don’t know what would be wrong.
```

---
## \#8 Posted by: J0ker3366 Posted at: 2019-01-22T06:39:06.291Z Reads: 72

```
@Andy87 was it just early focbox that the rx and tx had to be swapped?
```

---
## \#9 Posted by: Andy87 Posted at: 2019-01-22T06:51:14.786Z Reads: 69

```
like @J0ker3366 said, try to swap rx and tx on the jst plug.
should work after.
```

---
## \#10 Posted by: RealaPolarBear Posted at: 2019-01-22T15:02:35.554Z Reads: 61

```
I can’t really swap the cables as they are set solid in the 6 pin connector, but I’ve checked and rx on the ble module goes to the tx on the VeSC, and vice versa, this is correct right?
```

---
## \#11 Posted by: Pedrodemio Posted at: 2019-01-22T15:04:41.305Z Reads: 58

```
Yeah, that’s right 

They should work, what phone and what app are you using?
```

---
## \#12 Posted by: b264 Posted at: 2019-01-22T15:05:25.016Z Reads: 53

```
"Can't" is a word which is not frequently found on a DIY forum.
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-22T15:05:28.606Z Reads: 57

```
You can lift up the fixation a bit and take out the pin from the jst.
```

---
## \#14 Posted by: RealaPolarBear Posted at: 2019-01-22T15:05:34.497Z Reads: 59

```
I have an iPhone 7 running iOS 12 and I am using the Xmatic app
```

---
## \#15 Posted by: RealaPolarBear Posted at: 2019-01-22T15:07:23.953Z Reads: 55

```
@Andy87 Alright I’ll try, thanks.

[quote="b264, post:12, topic:81691, full:true"]
“Can’t” is a word which is not frequently found on a DIY forum.
[/quote]

Yeah, 😂 I realized my mistake
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-01-22T15:10:22.148Z Reads: 58

```
[quote="RealaPolarBear, post:1, topic:81691"]
I recently learned that the torqueboards VESCs do not have Bluetooth capabilites.
[/quote]

They do have Bluetooth capabilities, I'm using a TB vesc with a bluetooth module right now, it's just that the TB agents, Alex and Ralph don't know anything, Dexter definitely knows how to set it up and it's quiet easy.

@torqueboards -Dexter 

For the @mccloed modules from @psychotiller you only need to use 5 of the 6 pins, I'll upload a picture when I get home from school😂
```

---
## \#17 Posted by: RealaPolarBear Posted at: 2019-01-22T15:27:15.819Z Reads: 54

```
Ok, cause I have a ble module from buildkitboards
![image|375x500](upload://6iH38xArjpE0mlVudBeW3TMCFFJ.jpeg) 

And I do put it in this port right
![image|375x500](upload://aQ3fONpQuvbF3HU6rDKfHGaXX5Z.jpeg)
```

---
## \#18 Posted by: legend27 Posted at: 2019-01-22T17:04:26.980Z Reads: 51

```
Looks good to me. Should have 7 pins. Bluetooth works fine on my TB vesc.

![IMG_3890|666x500](upload://pjN0hVGPr4CF0TxbHa9veKjwN40.jpeg)
```

---
## \#19 Posted by: legend27 Posted at: 2019-01-22T17:06:03.672Z Reads: 51

```
Remember to set the setting in the vesc (can't remember where) to "PPM+UART" and set the baud rate to "9600"
```

---
## \#20 Posted by: RealaPolarBear Posted at: 2019-01-22T18:44:58.378Z Reads: 49

```
I’ve tried setting the app setting to ppm and uart before and have been sure to set my baudrate to 9600. I don’t know why it isn’t working, in the app, it just says connecting to VESC forever. Usually this is a baudrateproblem but I don’t know. Could this be a Ble module problem because otherwise everything is correct right? What apps and phones do you guys use? Could it be a problem with one of the rx/thx pins not fully in?
```

---
## \#21 Posted by: JLabs Posted at: 2019-01-22T18:53:18.595Z Reads: 46

```
I saw the TB recently dropped the price of the ESC’s. If they are now saying it dosnt work for the new batch my guess is that they removed some of the UART components to reduce the cost as they aren’t required for basic function. Just my 2 cents

To preface this, I hand flashed the new firmware on these modules, and tested each one before sending. The only problems people have had were with recent TB VESC and Flipsky 6.6.
```

---
## \#22 Posted by: AlanZhou Posted at: 2019-01-22T19:12:41.111Z Reads: 40

```
It's was proobly Ralph or Alex that said that, they didn't even know how to setup the Bluetooth modules on any vesc lol.
```

---
## \#23 Posted by: RealaPolarBear Posted at: 2019-01-22T19:18:59.947Z Reads: 39

```
I have on of the "older" TB vescs, I got mine in june-ish of 2018, I don't know if that would have an impact but...
```

---
## \#24 Posted by: legend27 Posted at: 2019-01-22T19:22:54.042Z Reads: 39

```
Have you tried to restart your phone and check for app updates?


edit: @twan any suggestions?
```

---
## \#25 Posted by: twan Posted at: 2019-01-22T21:02:10.931Z Reads: 32

```
may or may not be my app. try the new update :smiley:
```

---
## \#26 Posted by: AlanZhou Posted at: 2019-01-22T21:48:41.139Z Reads: 33

```
![IMG_20190122_164654|375x500](upload://qlaFZ4KWGDtQPyrIcdP1tkB8TfY.jpeg)
```

---
## \#27 Posted by: legend27 Posted at: 2019-01-24T06:41:08.803Z Reads: 23

```
Did you solve the issue?
```

---
## \#28 Posted by: RealaPolarBear Posted at: 2019-01-24T15:49:33.699Z Reads: 22

```
Not yet, I’m working on it
```

---

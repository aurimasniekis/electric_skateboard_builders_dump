# VESC polarity components

### Replies: 50 Views: 3079

## \#1 Posted by: zblad Posted at: 2016-07-21T02:29:33.433Z Reads: 146

```
Hello,

Next week I should be getting all the parts to build my first VESC I have one major concern and that is I am not sure what components do the polarity matter on.  Does anyone have a list or images that show what components to make sure are the right way or direction.  Is there any other tricky things I should prepare for.  I made my own solder oven and I ordered my boards and stencil from dirtyPCB.
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-21T02:41:43.102Z Reads: 143

```
Look at the pictures on vedder's github. I think there is an arrow or the name is in a special place (top left maybe) for the polarity.
```

---
## \#3 Posted by: zblad Posted at: 2016-07-21T02:51:41.634Z Reads: 136

```
The only thing I see is the line on the edge...
<img src="/uploads/db1493/original/2X/c/cf1638866413b2eb18ea505ec9b0d2efd3c5efdb.png" width="690" height="487">
```

---
## \#4 Posted by: lox897 Posted at: 2016-07-21T03:16:06.165Z Reads: 122

```
Maybe ask this on vedder's forum. You might get some better answers.
```

---
## \#5 Posted by: Blasto Posted at: 2016-07-21T04:33:34.044Z Reads: 121

```
What component are you asking about? The component placement seems pretty clear.
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-21T05:52:44.074Z Reads: 113

```
He is asking about the orientation of the components. Do they have to be in a certain orientation so they don't short? How do you know which way to solder them.
```

---
## \#7 Posted by: zblad Posted at: 2016-07-24T21:26:22.328Z Reads: 93

```
Yes that is what i am asking or at least how many of them does the orientation matter.
```

---
## \#8 Posted by: chuttney1 Posted at: 2016-07-24T23:43:28.728Z Reads: 83

```
The LEDs do. Your smartphone should have a high magnification to see the markings of the SMD LED.
```

---
## \#9 Posted by: zblad Posted at: 2016-07-25T01:36:44.172Z Reads: 81

```
alright i figured the LEDs, Schotty Diode, and im sure there are other was just hoping someone had a picture with them high lighted i noticed some of the parts on the image i posted previously some parts have a black line on the edge of them not sure why though.
```

---
## \#10 Posted by: Stevemk14ebr Posted at: 2016-07-25T01:48:50.748Z Reads: 80

```
I bet ya @chaka can help you out.
```

---
## \#11 Posted by: zblad Posted at: 2016-07-25T01:52:36.984Z Reads: 75

```
I hope someone can i have the next two days off and got all the parts I need and really dont want to mess this up...
```

---
## \#12 Posted by: lox897 Posted at: 2016-07-25T02:42:54.603Z Reads: 70

```
I'd be interested to know this as well because I am about to build an Arduino Spot Welder. @chaka @Blasto
```

---
## \#13 Posted by: Blasto Posted at: 2016-07-25T03:17:09.098Z Reads: 70

```
Diodes-
Component: line marks the cathode
Silkscreen: could diode symbol or just a plain line to mark de cathode

Led-
Component: check the component datasheet, usually green dot on the bottom marks the cathode
Silkscreen: same as diode

Tental capacitor-
Component: line on component marks the positive side
Silkscreen: thick line marks positive

Intergrated circuits-
Component: little dot in the corner of the component marks the pin 1
Silkscreen: a dot should mark pin 1

Connectors
Component: this one is tricky, depends on the manufacturer, usually pin 1 is marked
Silkscreen: usually the component pin 1 pad is square, or can have a dot

For the other components, fets, shunts and voltage regulator... Well you should figure that one for yourself

https://sites.google.com/a/eng.ucsd.edu/quadcopterclass/labs/lab-7-solder-practice/smd-component-identification
```

---
## \#14 Posted by: chuttney1 Posted at: 2016-07-25T04:10:58.432Z Reads: 65

```
I forgot to mention which side for the LEDs on the VESC. Its not silkscreen on the pcb. I had to check the comments on Vedder's blog of the VESC to find the direction of the LEDs.

The ground is toward the side with the mosfets.

Check to make sure.
```

---
## \#15 Posted by: cjoliver Posted at: 2016-07-25T04:32:19.635Z Reads: 63

```
You're about to solder your own VESC but don't know polarity of some components, seems kinda backwards logic
```

---
## \#16 Posted by: lox897 Posted at: 2016-07-25T05:32:42.809Z Reads: 63

```
Some people like to have goes at things they haven't done before. Asking a question about something you don't know isn't bad.
```

---
## \#17 Posted by: zblad Posted at: 2016-07-25T21:16:20.753Z Reads: 60

```
Alright so i finished the board today but havent got to test it out yet i have a couple concerns....

when i put the board in my soldering oven some of the components move so i had to straighten them out with my regular soldering gun and i home i didnt over heat them or anything.  Another issue is there is bridges all over the place in the small processor and motor driver.  See images.  also on the fets it looks like they might be shorted across the pins does anyone know if this will cause issues and can i try flash the firmware on it or will that mess it up?

<img src="/uploads/db1493/original/2X/a/ad12a558f715975c8d6a9522609f2308acd0e752.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/e/eb44f8bf89b74620a9d1b563bda26168585c00cb.JPG" width="375" height="500">
```

---
## \#18 Posted by: Blasto Posted at: 2016-07-26T01:20:40.671Z Reads: 54

```
Clean that board up with some wick, no chance in hell it will work looking like that. Go ez on the paste on the next one
```

---
## \#19 Posted by: zblad Posted at: 2016-07-26T01:28:36.198Z Reads: 54

```
Already clean it all up looks good and yeah first time ever using a stencil and there was a couple other issues i had with my homemade oven.  Going to try flash it tomorrow morning crossing my fingures it works...  Does anyone know if a 50v 1000uf capacitor on the battery wires will work instead of the 60v 2200uf?
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2016-07-26T02:37:01.437Z Reads: 52

```
what battery are you using?? and better luck next time, to find the right temperature curve. :smiley:
```

---
## \#21 Posted by: zblad Posted at: 2016-07-26T03:05:01.119Z Reads: 51

```
I am going to use a battery out of a hoverboard for testing... its it 10s battery.  The crappy thing is half the stuff soldered it was almost like half the oven didnt reach the right temp.  Another question does anyone know if the LEDs are indicator lights or if they are in backwards will something not work?  I am fairly certain i put them in the right direction but one of them was extremely hard to tell if there was a little circle...
```

---
## \#22 Posted by: zblad Posted at: 2016-07-26T03:08:09.075Z Reads: 52

```
and should i put a fuse in line with the battery wires... And if i should home many amps would you go with?  Thanks for all the help really hoping this board turns out.
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-07-26T05:17:09.914Z Reads: 54

```
[quote="zblad, post:21, topic:6404"]
LEDs are indicator lights
[/quote]


yes, the blue is for the power, the red and green for operation with the drv. And next time for the LED look at the pads before placing them. 

[quote="zblad, post:22, topic:6404"]
and should i put a fuse in line with the battery wires
[/quote]

Yes, and around 40amp to 60amp
```

---
## \#24 Posted by: chuttney1 Posted at: 2016-07-26T05:26:07.720Z Reads: 52

```
Don't you have a 12V battery to confirm it works. Done to limit the amount of current otherwise you could kill the DRV8302. Proceed with caution until you are confident it won't die.

Capacitor voltages its okay to have ones rated higher than the intended voltage, but never below. Capacitance is of question in regards to capacitor size and either one or two. Its done to deal with ripple current and has been talked among the RC people. 50V is okay for 10S.
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2016-07-26T06:05:05.032Z Reads: 50

```
[quote="chuttney1, post:24, topic:6404"]
Done to limit the amount of current otherwise you could kill the DRV8302
[/quote]


NO, this is totally false and misleading. It won't brake the DRV8302 (half of the problem have there root with other part than the DRV, but lead to DRV failure, like burnt MCU and CAN tranceiver). 

But it is true, you should use low current 12V to check if all part are working, and program the MCU, before putting a big load and running motor detection.

And you should go with the 63V capacitor, because the maximum rating of the VESC is 60V.
```

---
## \#26 Posted by: zblad Posted at: 2016-07-26T11:54:06.005Z Reads: 46

```
Alright i do have a small 12v i can use instead so i will give that a shot...
```

---
## \#27 Posted by: zblad Posted at: 2016-07-26T13:28:01.309Z Reads: 46

```
So the instant i hook up the stlink2 to my vesc all the light go off on the stlink2 and I cant see it under lsusb in ubuntu so im guessing something is shorted or not connected :(  when i run make upload i get "This adapter doesn't support configurable speed".  I also dont get any lights on the VESC.
```

---
## \#28 Posted by: zblad Posted at: 2016-07-26T13:42:43.839Z Reads: 45

```
Alright so i checked some solder joints and now the lights stay on the stlink2 and the blue light on the VESC comes on but i get this weird error init mode failed in procedure 'transport'.
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2016-07-26T14:19:22.018Z Reads: 45

```
I think, you will need to get the Multi-Meter out, and check for short, because you may have a solder bridge under one of the chip. Also check if you have the 5v from the drv a the 3.3v from the regulator.
```

---
## \#30 Posted by: elkick Posted at: 2016-07-26T17:00:48.618Z Reads: 42

```
You need to uncomment the line 273 and comment line 274 with a # in the make file before doing the make upload.
```

---
## \#31 Posted by: zblad Posted at: 2016-07-26T17:13:11.813Z Reads: 40

```
How do i edit the make file is that the config one?
```

---
## \#32 Posted by: elkick Posted at: 2016-07-26T17:30:58.464Z Reads: 39

```
No, it's in the top folder like the config one and it's called "makefile".

Just comment the part for the discovery board in there and uncomment the STLink part.
```

---
## \#33 Posted by: zblad Posted at: 2016-07-26T17:42:09.611Z Reads: 38

```
Alright will although my patience got the best of me and i wrecked the board.  Kinda my fault and the merchant i bought the parts from.  The small processor had a bunch of bent pins so i tried straightening them out myself this made the processor solder down not perfectly straight so i did the best to correct it but ripped some of the copper of the board in the process...  Now I need to decide if i should say screw it and buy one or try make one myself again.
```

---
## \#34 Posted by: zblad Posted at: 2016-07-26T17:44:53.201Z Reads: 39

```
Alright so i changed the code but i think its a little to late really sucks I should have waited for someone to comment back :frowning:
```

---
## \#35 Posted by: chuttney1 Posted at: 2016-07-26T18:15:35.808Z Reads: 40

```
Welcome to the predicament I am still in. Really weigh your options if it still worth the cost of building another one or ones already made.
```

---
## \#36 Posted by: JohnnyMeduse Posted at: 2016-07-26T18:33:24.711Z Reads: 40

```
[quote="zblad, post:33, topic:6404"]
but ripped some of the copper of the board in the process
[/quote]


do yo have a picture ?
```

---
## \#37 Posted by: Blasto Posted at: 2016-07-26T18:44:37.816Z Reads: 40

```
Where are you located?
```

---
## \#38 Posted by: zblad Posted at: 2016-07-26T19:02:59.647Z Reads: 41

```
Thief River Falls, Minnesota.  Crazy thing so after i changed that code i hooked it up for shits and giggles and it started to compile but eventually errored out which i knew it would since half the pins are busted now.  Why did you want to know where i live?
```

---
## \#39 Posted by: zblad Posted at: 2016-07-26T19:09:38.887Z Reads: 40

```
Only reason im still considering building my own is because i bought everything to build them lol i have 9 boards left, i have the flashing board stlink2, I have a laptop with ubuntu, I have a homemade surface mount oven, and i like to build my own stuff haha. 

<img src="/uploads/db1493/original/2X/f/fc525d7a0c9e90dc461957388a217aacd519f466.JPG" width="375" height="500">
```

---
## \#40 Posted by: JohnnyMeduse Posted at: 2016-07-26T20:13:40.551Z Reads: 38

```
Well I don't there is any possibility to repair this board, Better luck with the 9 other board. :confused:

What solder paste did you use, and did you use flux when doing your repair ? Also what is your temperature curve on your oven ?
```

---
## \#41 Posted by: zblad Posted at: 2016-07-26T21:00:12.897Z Reads: 39

```
My oven is using some code i found online for an arduino so not exactly sure...  Yeah this board is SHOT o well learning expierence.  Solder paste is chipquik smd291ax whatever that means its in like a syringe.  It also says sn63/pb37 no clean t3 solder paste.  Flux yes i did well I tried.  Where i did the most damage was trying to straighten pins with my soldering iron.  Alot of the issue was the pins being bent when i got the processor so it didnt set the processor correctly when i tried using the oven.
```

---
## \#42 Posted by: JohnnyMeduse Posted at: 2016-07-26T21:41:22.528Z Reads: 36

```
Check for the code, because if it operate for EU standard, that mean it made for LeadFree Soldering, and melting point are different than Leaded Soldering, like the one you use. Also, you may want to straighten the pin before soldering it. Finally, if you don't use a stencil be careful with the amount of paste you put.
```

---
## \#43 Posted by: zblad Posted at: 2016-07-26T21:49:54.988Z Reads: 37

```
I did use a stencil i just dont have it down snug enough... Also what side would you solder first.  I did the back side maybe i should do the front first.
```

---
## \#44 Posted by: JohnnyMeduse Posted at: 2016-07-26T21:57:34.016Z Reads: 40

```
You should do the side, with the MCU and DRV last, because you don't want to expose them to too much heat. 

And Use these with your stencil, for removing the excess  <img src="/uploads/db1493/original/2X/d/d6d1dd366cc064bef77d15fb64fab9660aeb482c.jpg" width="375" height="500">
```

---
## \#45 Posted by: zblad Posted at: 2016-07-26T23:22:13.455Z Reads: 40

```
Ok so yeah i did it in the right order and i did use one of the but i think my stencil wasnt down tight enough so it pushed some solder paste under the stencil if that make sense...  Idk hopefully in a week or two ill get a chance to give it another go.
```

---
## \#46 Posted by: lox897 Posted at: 2016-08-17T11:14:10.371Z Reads: 38

```
For anyone interested in knowing this, this page helped me a lot: https://learn.sparkfun.com/tutorials/polarity

If you are building the arduino spot welder and don't know what the markings mean, this also helps.
```

---
## \#47 Posted by: zblad Posted at: 2016-08-22T19:53:58.340Z Reads: 26

```
Successfully made a VESC today and flashed it.  Ordered the bullet connectors and wire today so now just waiting on that.  I was wondering if a regular 12v battery would work for testing or should i try hook up the 10s hoverboard battery right away?  Also i plan on using an rc remote for now but does anyone know if the VESC will power the remote controls receiver? Thanks
```

---
## \#48 Posted by: mason Posted at: 2016-08-22T21:20:56.233Z Reads: 25

```
Yes, it will power the receiver.
```

---
## \#49 Posted by: zblad Posted at: 2016-08-22T22:15:08.869Z Reads: 22

```
Sweet thank you...  Do you think testing it with a 12v is the way to go or does it really matter?
```

---
## \#50 Posted by: zblad Posted at: 2016-08-23T21:48:43.403Z Reads: 20

```
Problems i hooked power to my vesc today and i got a blue light only i couldnt get it to cennect and now the blue light went out and does nothing???  what the heck could be the issue.
```

---

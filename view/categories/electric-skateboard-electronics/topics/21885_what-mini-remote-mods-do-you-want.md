# What Mini remote mods do you want?

### Replies: 5 Views: 828

## \#1 Posted by: saul Posted at: 2017-04-27T07:35:15.164Z Reads: 221

```
Started a mini remote mod a few months back, abandoned it in favor of a full custom arduino nrf remote.
But now I have 2 mini remote pcbs and 3-4 enclosures about 90% done.


Seem like there are more mini remotes being used now so I want to finish it up and get it out there but what do you all want out of the mod?

Size:
[poll type=multiple min=1 max=3 public=true]
* Make it as small as possible.
* Give it more features.
* Make it work for huge banana hands.
* Just gimme!
[/poll]

Control style
[poll name=poll2 type=multiple min=1 max=3 public=true]
* ps3 Thumb stick
* stock trigger style
* stock thumb style
[/poll]
Complete or diy?
[poll name=poll3 type=multiple min=1 max=4 public=true]
* Completed mod
* printed case and extra componets
* printed case only
* .stl only
[/poll]

This is latest version, about 110mm tall, 50mm wide at the top, 36mm at the base. and 32mm deep.
li ion battery about 500mah, micro usb charger, trinket 3.3v (buck and power meter) + rgb leds.

<img src="/uploads/db1493/original/3X/c/b/cb4e345b5954fc745b52b594410469b572d406b6.png" width="369" height="500">
<img src="/uploads/db1493/original/3X/1/c/1c2211d0cfeaf434884cda444ccdd0ca4de33079.jpg" width="648" height="500">
```

---
## \#2 Posted by: Okami Posted at: 2017-04-27T11:53:01.448Z Reads: 192

```
How are the leds working?

If the ''new enclosure'' accomodates state of charge indicator for remote that would be nice.. 

Replacing batteries for mini remote on the go is not always easy, as you need a screwdriver and carry somewhat bulky 2X AA batts.

So taking care of these ''old generation'' AA batteries is a nice step forward. Especially because a few times they just ''die'' quickly and there''s no real way on seeing how much voltage there still is as to opening the compartment and measuring it manually.
--
Not sure if possible but I personally was thinking was it possible to mount little volt meter in the old case (original one) of the mini remote, to see the voltage.. but then again, a ''mod'' with rechargable battery is way better, as you can always just top it up after a few days or so.. without the need to monitor it all the time.

--

As about the trigger (control style) - im not entirely sure which one is the better one, I just know that I didnt like the short trigger play I had on the original setting, so I made a cutouts in the plastic for the trigger to go a bit more deeper into the enclosure..

This need to be adressed, so that the remote is not super sensitive and offers a ''firm grip'' of control.
```

---
## \#3 Posted by: saul Posted at: 2017-04-27T12:42:05.172Z Reads: 172

```
[quote="Okami, post:2, topic:21885"]
state of charge indicator for remote that would be nice..
[/quote]

got it. the trinket/attiny85 reads the battery voltage with 10bit analog and displays red/orange/blue/green on the leds to indicate charge level.
I could add an oled display for actual voltage, but thats overkill so i'm saving it for the Arduino and vesc data...
no more changing batteries was my reason for starting it.

[quote="Okami, post:2, topic:21885"]
This need to be adressed, so that the remote is not super sensitive and offers a ''firm grip'' of control.
[/quote]

for the control I've been using the ps3 style joystick because it works well for other uses.

the alternative is to use the stock steering pot and add a wheel or throttle attachment.
a longer throttle = more travel = better control (hopefully)
```

---
## \#4 Posted by: Okami Posted at: 2017-04-27T12:57:37.897Z Reads: 180

```
[quote="saul, post:3, topic:21885"]
displays red/orange/blue/green on the leds to indicate charge level.
[/quote]

yeh, these sort of levels sound very good, if you manage to mount 4tiny leds in there, all ok!

Otherwise was a bit afraid, it will be just 1 dual color led, with green/red light for example :D 
--
[quote="saul, post:3, topic:21885"]
could add an oled display for actual voltage, but thats overkill
[/quote]


Agree, oled / other displays are not that needed then, unless u plan to integrate speedo or board's voltage there.

[quote="saul, post:3, topic:21885"]
the control I've been using the ps3 style j
[/quote]

So how is the control with thumbstick? I used to play video games but im not super sure how sensitive it might be in this application.. I know people use them on nunchuk remotes but i havent had the chance to see for myself how sensitive / responsive they are..

One thing for sure, it looks like the way evolve made their ''joystick'' on their newer gen boards.. sucks ass, because people have been putting foam to dampen the sensitivity of the whole potentiometer.

--

So yes, longer travel distance is advised, that''s for sure :) less space for error to happen with accidental movements etc
```

---
## \#5 Posted by: SageTX Posted at: 2017-04-27T18:32:24.027Z Reads: 153

```
Keep throttle finger control trigger.  Add thumb trigger using steering pot so @Ackmaniac 's  mod is usable for cruise. Recess (or enclose) trim pots so they don't get bumped.  
More robust on /off switch.  
Personally I love the size. I can use it with wrist guards. 
Batteries - whatever. The AAs have lasted over 150 miles. I changed them just because to lithium but the tabs are WEAK. So maybe rechargeable would be better.  

Just my 2¢ for the perfect mod.
```

---

# Aps80mm motor issues using etoxx aps80mm direct drive

### Replies: 27 Views: 894

## \#1 Posted by: gibbsc16 Posted at: 2018-11-07T16:04:35.211Z Reads: 159

```
Hello everyone,

I recently bought the alien aps 8055 70kv 6000m motors and etoxx/ jens kappels aps80mm direct drive motor mounts. I'm running 2 vesc six configured with 2 6s zippy compact 40c 6200 mah lipo batteries per vesc running dual rear direct drive. Im lost and starting to lose hope in this build as my motors won't turn without giving them a push. The wires that come off the motor i believe are to small for the power which they are rated at and are copper wires coming straight from the magnetos with heat shrink tubing and no bullet connectors, seems like a poor design to me. Is my problem with the way the vest are configured or is it with the way that the motors are designed? Am i using to low kv motor? Should I be using 165kv or even 250kv motor? Also, is my battery setup with the mah to high or to low for the setup?  Does anyone have any experience running this setup? Is there any other motors that would be recommend to use with the motor mounts i already have? Any help is greatly appreciated!!!!!
```

---
## \#2 Posted by: Klaerke91 Posted at: 2018-11-07T16:09:31.283Z Reads: 148

```
you need sensored motors otherwise there is always start problems when starting from 0.

I have these motors - https://alienpowersystem.com/shop/brushless-motors/c8085-sensored-outrunner-brushless-motor-170kv-6000w/
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-11-07T16:14:34.234Z Reads: 141

```
The kV of the motors are really low, but this should only be good for strart-ups. As said, you’ll need sensors to get really smooth start-ups. Could you please take some pictures of the motor wires? Didnt quite understand..
```

---
## \#4 Posted by: gibbsc16 Posted at: 2018-11-07T16:20:12.160Z Reads: 131

```
Im not sure if you are familiar with Jens kappel but he has a website called e toxx where he sells direct drive mounts and i bought two of the aps 80mm direct drive motor mounts which, if I'm not mistaking, can only be used with the aps model motors. The motors that I'm looking at getting now is the "APS8072S Sensored BLDC motor 165KV 6000W" or "APS8072S Sensored BLDC motor 250KV 6000W"
```

---
## \#5 Posted by: gibbsc16 Posted at: 2018-11-07T16:21:34.438Z Reads: 126

```
![53%20AM|655x500](upload://rnp10iC5Y7wiwLxfvKo6m3nIG5y.png)
```

---
## \#6 Posted by: gibbsc16 Posted at: 2018-11-07T16:23:13.359Z Reads: 125

```
 https://alienpowersystem.com/shop/brushless-motors/aps8055-sensored-bldc-motor-50kv-4500w/

this is the link to a similar motor just different kv and watt. I can't even find the same kv and watt motor that I have and just bought from alien power systems a couple months ago. Makes me wonder if they have had problems with this particular one?!?!
```

---
## \#7 Posted by: Klaerke91 Posted at: 2018-11-07T16:23:33.930Z Reads: 121

```
you dont want 250kv that to high. 
I have the drives from jens and he told me to get the c8085 sensored motors and not to go over 200kv
```

---
## \#8 Posted by: telnoi Posted at: 2018-11-07T16:27:01.150Z Reads: 120

```
Missing allot of information. Did you even run motor detection? What do you mean with motor needs a push? Unsensored will usually cog with load, but should turn fine without load.

As for KV, for 5:1 149kv-200kv will be OK. Below 149 will severely impact top speed. Above will decrease torque the higher you go.
```

---
## \#9 Posted by: gibbsc16 Posted at: 2018-11-07T16:28:21.364Z Reads: 118

```
So you have the same motor mounts that I do? I guess I'm still a little confused as to why the bigger 80mm motors have smaller wiring and just heat shrink tubing around them where as the 60mm motors have bigger wiring with a lot better insulation and bullet connectors already soldered. When I clicked on the link to the c8085 motors there is a shaft coming out of both ends why is this? Also, is there anyway you could post a picture of your motor setup with the motor mounts.
```

---
## \#10 Posted by: gibbsc16 Posted at: 2018-11-07T16:36:45.834Z Reads: 113

```
Ran motor detection and detected them perfectly fine. I have to kick of the board as I'm mashing the throttle button in order to take off. I was playing around the other day with the throttle on my remote and If you push the throttle ahead VERY slow it works fine but if you just try throttling at a normal push on the joystick it cogs and jitters until you spin the motor then it takes off. I also have a 1:4 helical gear ratio. I figured using the low, 70kv, would provide good torque and take off to do those wheelies :joy:
```

---
## \#11 Posted by: telnoi Posted at: 2018-11-07T16:38:18.922Z Reads: 101

```
Foc or bldc?
```

---
## \#12 Posted by: gibbsc16 Posted at: 2018-11-07T16:40:40.565Z Reads: 102

```
the motors are bldc I configured them in foc mode
```

---
## \#13 Posted by: gibbsc16 Posted at: 2018-11-07T16:53:34.066Z Reads: 100

```
@telnoi the motors are bldc I configured them in foc mode
```

---
## \#14 Posted by: gibbsc16 Posted at: 2018-11-07T16:54:29.807Z Reads: 96

```
[quote="gibbsc16, post:9, topic:73829, full:true"]
So you have the same motor mounts that I do? I guess I’m still a little confused as to why the bigger 80mm motors have smaller wiring and just heat shrink tubing around them where as the 60mm motors have bigger wiring with a lot better insulation and bullet connectors already soldered. When I clicked on the link to the c8085 motors there is a shaft coming out of both ends why is this? Also, is there anyway you could post a picture of your motor setup with the motor mounts. @Klaerke91
```

---
## \#15 Posted by: telnoi Posted at: 2018-11-07T16:56:52.382Z Reads: 92

```
See if bldc does a better job. Would at least confirm if this is hardware or software related.

Redo motor detection.
```

---
## \#16 Posted by: gibbsc16 Posted at: 2018-11-07T17:35:26.099Z Reads: 94

```
@Klaerke91 I just ordered the c8085 motors with reworked shaft including

 * shaft external length = 30mm
* shaft external diameter = 10 mm

* keyway length = 25mm
* keyway size = 3mm
* keyway distance from end shaft = 2.5mm
```

---
## \#17 Posted by: Klaerke91 Posted at: 2018-11-07T17:45:35.171Z Reads: 92

```
nice. i have the 12mm shaft and i dont use a keyway. i use locktite - https://www.henkel-adhesives.com/us/en/product/retaining-compounds/loctite_638.html

Just dont get it in your motor. 

and just so you know. i haven't finished my board yet, so take that in to account. I can screw up just as much as you
```

---
## \#18 Posted by: gibbsc16 Posted at: 2018-11-07T17:48:12.642Z Reads: 89

```
Oh pooooppppp....does the motors atleast fit on the motor mounts and on the hanger mounted to the deck? Or have you not got that far yet @Klaerke91
```

---
## \#19 Posted by: Klaerke91 Posted at: 2018-11-07T17:50:56.906Z Reads: 89

```
if you got the motor i linked to they will fit with 10 and 12 mm shaft. You need to cut off the shaft on the back and some in the front to make it fit the mounts, but its easy if you take it slow and measure before cutting
```

---
## \#20 Posted by: gibbsc16 Posted at: 2018-11-09T03:31:56.452Z Reads: 82

```
Sweeeettttttt i sent aps the information based off the ones i already have that fit so they can do the cutting and they're cutting the other end off that isn't needed. How do you feel about the quality of the wires coming out of the motor? I sent aps an email regarding the wires and if they could upgrade them to heavier gauge wire and bullet connectors like come on there 60mm motors. When do you think you'll be testing? Cant wait to see!!
@Klaerke91
```

---
## \#21 Posted by: Klaerke91 Posted at: 2018-11-09T09:45:52.087Z Reads: 79

```
The wires coming out is the copper windings in the motors so that cant be changes unless you use another kv setting in the motor. Bullet connector you can solder yourself, its not that hard :-).
If all goes well i will have my first run this weekend .-)
```

---
## \#22 Posted by: gibbsc16 Posted at: 2018-11-10T05:08:54.173Z Reads: 78

```
@Klaerke91keep me posted on how everything goes. As far as the wiring on the motors goes I guess what my man concern is when you look at the 63mm motors aps provides they don't just have heat shrink tubing around the wires they have some kind of black wire loom around it that looks like it can with stand heat a lot better than just heat shrink tubing. ![Aps%202|690x373](upload://rSiDaRBC2fUrs0XYvpPe5sFpq8o.png) ![aps%201|690x371](upload://b6XtlTbqhf2uiu9y5yp7ctjLCCQ.png)  these are the motors I have ordered and that you have Im not sure if its like the 80mm I already have but if it is then its just heat shrink tubing


![aps%200|690x397](upload://m8NWz5GKqDEcSvfqp8kR00c4SMZ.png) 
This is a picture of aps 63mm motors.. just looks like to me the 63mm wiring is of better quality then the 80mm
```

---
## \#23 Posted by: gibbsc16 Posted at: 2018-11-14T19:38:05.195Z Reads: 69

```
I've been talking with aps about the motors I just ordered and they have addressed my concerns and are wrapping the wires just like they do on the 60mm motors and also adding bullet connectors
```

---
## \#24 Posted by: gibbsc16 Posted at: 2018-12-18T22:28:33.281Z Reads: 65

```
@Klaerke91how is your board coming along? My motors have finally come in I'm just trying to figure out what color wires on the sensor cable corresponds to what feature on the vesc. Example, red wire is v+ black wire is ground etc. but I'm not sure what they are.
```

---
## \#25 Posted by: Klaerke91 Posted at: 2018-12-20T18:54:46.278Z Reads: 58

```
The other wires goes to your hall sensors and temp sensor if there is one installed.
The pinout is different depending on you Vesc.

Had my board up and running and its a beast but i haven driven more that a few kilometers as its winter.
Right now its disassembled and waiting on new parts. (Hubs and BMS)
```

---
## \#26 Posted by: gibbsc16 Posted at: 2018-12-21T20:41:27.260Z Reads: 45

```
@Klaerke91 I've finished my board and the new motors with 10 gauge wiring done the trick along with the sensors I'm doing more testing today. Im finding out though that the steering is to stiff for any turning but yet at the same time not stiff enough to eliminate wobbling
```

---
## \#27 Posted by: Andy87 Posted at: 2018-12-21T21:03:18.071Z Reads: 43

```
Elastomer damper 
https://www.e-toxx-shop.com/trampa/elastomere-damper/#cc-m-product-10002752170
Or steering damper could solve that issue.
```

---

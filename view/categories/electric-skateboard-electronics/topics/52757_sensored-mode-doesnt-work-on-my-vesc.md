# Sensored mode doesn&rsquo;t work on my vesc

### Replies: 24 Views: 777

## \#1 Posted by: flaviuschris4 Posted at: 2018-04-19T05:54:17.849Z Reads: 93

```
hello everyone so I used to run sensored mode on my vesc on bldc mode and then one day I wanted to try sensorless mode and the start isn't as good so I switched back and I tried it on sensored mode again nothing happenes but when I put it in foc mode on sensored mode it works but very high pitched can anyone help me!
```

---
## \#2 Posted by: myreala Posted at: 2018-04-19T06:25:48.113Z Reads: 89

```
Run foc motor detection again for both motors.
```

---
## \#3 Posted by: Exiledd_Top Posted at: 2018-04-19T06:33:46.165Z Reads: 85

```
I have done the same what ends up happening and why I think u didn't like sensorless was because u never redid the parameters on detection as stated so when you switch from sensor to nonsensor u have to run motor detection again , I personally make everything default again in motor detection page and run it again .
```

---
## \#4 Posted by: flaviuschris4 Posted at: 2018-04-19T06:35:14.758Z Reads: 82

```
I do run the motor detection its just still very compared to sensored
```

---
## \#5 Posted by: flaviuschris4 Posted at: 2018-04-19T06:36:34.591Z Reads: 80

```
what do you mean and is it safe to run in foc mode? is there anything I should do?
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-19T06:40:02.855Z Reads: 77

```
The 255 255 255 255 tab changes when you run sensord but if just switched back to sensorless then those numbers stay the same such as 98 255 78 190 but should be default 255  , I had that problem motors were really eh at start,  for me personally I do not like sensors I run foc but on 4wd it's too smooth I can't feel anything you know , I don't get a sense on weather it's safe or not it rises to good lol. Start is good but ride just make a me feel so riding blind I like to feel the raw power I cruise at 30mph usually
```

---
## \#7 Posted by: flaviuschris4 Posted at: 2018-04-19T06:42:52.986Z Reads: 72

```
I run a single motor on 9s and its 190kv 6355 is there any way to make foc safer?
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2018-04-19T06:44:24.688Z Reads: 65

```
[quote="flaviuschris4, post:5, topic:52757"]
safe to run in foc
[/quote]

Foc is known not to be user friendly and not alot of vesc out there can handle foc but company's say u can but just for advertising.  So we see a  first timers buy a vesc and try foc and end up frying it but it also depends on what motor kv and voltage , usually a 190kv u want to run 10s for foc and try at own risk 12s , but I only recommend a focbox  for foc endless u want to pay big money for a ves6 200-360$
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-04-19T06:47:08.417Z Reads: 59

```
Which ESC you are using?
```

---
## \#10 Posted by: flaviuschris4 Posted at: 2018-04-19T06:47:51.869Z Reads: 59

```
the 99$ vesc from diy electric
```

---
## \#11 Posted by: Exiledd_Top Posted at: 2018-04-19T06:49:11.039Z Reads: 57

```
I mean those are known not to be foc friendly and most people fry the vesc on just putting it in foc get a focbox has upgraded components, but yet again u are running 9s on 190v , but yet again one could say single drive foc can stress the motor alot. Anyways to make it safer ? Have safe motor settings such as motor min and battery min
```

---
## \#12 Posted by: CarlCollins Posted at: 2018-04-19T06:50:35.997Z Reads: 56

```
Those are popular for not handling the FOC. 
I hope you VESC is not burnt. Please check the PCB of the VESC from both side
```

---
## \#13 Posted by: flaviuschris4 Posted at: 2018-04-19T06:52:43.538Z Reads: 55

```
its not burned since it still works in both modes also I just can't get it to work in sensored mode in bldc the motor doesn't spin the vesc light turns on when I give it throttle but idk whats wrong
```

---
## \#14 Posted by: CarlCollins Posted at: 2018-04-19T06:53:33.599Z Reads: 53

```
What are the L & R values in BLDC tool?
```

---
## \#15 Posted by: flaviuschris4 Posted at: 2018-04-19T06:54:21.072Z Reads: 52

```
im not sure where do I check that?
```

---
## \#16 Posted by: CarlCollins Posted at: 2018-04-19T07:01:28.415Z Reads: 49

```
Read configuration first before doing it 
https://www.screencast.com/t/sYwsl07ia
```

---
## \#17 Posted by: flaviuschris4 Posted at: 2018-04-19T07:08:44.542Z Reads: 50

```
I dont think its a good idea running in foc mode though
```

---
## \#18 Posted by: CarlCollins Posted at: 2018-04-19T07:13:08.270Z Reads: 49

```
You already ran it in FOC mode, (you've indicated it above)
```

---
## \#19 Posted by: flaviuschris4 Posted at: 2018-04-19T07:14:33.140Z Reads: 49

```
yea but I just did for a few min im afraid If I do for more ill burn it haha
```

---
## \#20 Posted by: CarlCollins Posted at: 2018-04-19T07:15:50.808Z Reads: 48

```
Then try reflashing the Firmware to get default values back 
And do BLDC detections again.
```

---
## \#21 Posted by: flaviuschris4 Posted at: 2018-04-19T17:28:58.677Z Reads: 37

```
how do I reflash the firmware?
```

---
## \#22 Posted by: flaviuschris4 Posted at: 2018-04-19T17:34:47.263Z Reads: 34

```
I can't find any reflashing options on the vesc program how do I reflash the firmware? plz help
```

---
## \#23 Posted by: flaviuschris4 Posted at: 2018-04-19T17:43:04.541Z Reads: 34

```
![29 AM|690x372](upload://fwNSXtRXuSpr6S03vTiTeVR9jRX.png)
thease are what my settings are on bldc and nothing is happening when I give it throttle on sensored mode but senseless works fine
```

---
## \#24 Posted by: CarlCollins Posted at: 2018-04-20T10:04:54.334Z Reads: 32

```
@flaviuschris4
Download BLDC tool from DIY electricskateboard website and use that application to reflash the firmware.( Firmware files muse be included with the BLDC). 

If you got any error initially (on the connection of VESC)
Then you have to find a way to downgrade the firmware of VESC.
```

---

# FSESC 6.6 strange sound on start&hellip; normal?

### Replies: 9 Views: 232

## \#1 Posted by: StefanMe Posted at: 2018-12-21T18:11:06.399Z Reads: 55

```
Hey guys, ist just hooked up my FSESC 6.6 on my single 6474 motor and have some strange sound in FOC at the beginning before turning... after that it starts smoothly... I didn't have this sound with my FOCBOX. Is this normal? It sounds a bit like there is no sensors attached, but the start is smooth...
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-21T18:16:18.331Z Reads: 55

```
Mine are super silent with belts from the start up.
Maybe you can upload a video with the sound?
```

---
## \#3 Posted by: StefanMe Posted at: 2018-12-21T18:28:15.576Z Reads: 47

```
https://youtu.be/72utVzW2cVA
```

---
## \#4 Posted by: Blasto Posted at: 2018-12-21T18:39:44.013Z Reads: 42

```
Check your ppm settings, sounds like the brakes are being applied
```

---
## \#5 Posted by: StefanMe Posted at: 2018-12-21T18:43:01.711Z Reads: 38

```
No that looks fine... I pushed the throttle slightly forward... looks normal. When I push backwards there is no sound at all, but breaks are working normal/

![18|690x432](upload://1N82Z2cl4qYOw6Z7CypjNbQk6DH.png)
```

---
## \#6 Posted by: Andy87 Posted at: 2018-12-21T19:29:36.504Z Reads: 30

```
Which remote you use?
If you accelerate the throttle goes up smoothly?
Did you already make a second run for the motor detection?
Can you hear if the sound comes only from one or from both?
```

---
## \#7 Posted by: StefanMe Posted at: 2018-12-21T19:39:05.840Z Reads: 27

```
I use my own remote... ([FeatherRemote LINK](https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084))

Yeah looks quite smooth. 

 but as I said before... didn't got these problems with a FocBox... Thats why I am wondering. Is 5V the correct setting for the HALL SENSORS? Anyway makes no difference.

I got only one motor installed.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-21T19:43:24.410Z Reads: 27

```
5V is right.
It’s based on the firefly right?
Just today one guy had problems with his firefly that with 5% throttle he already got like 100% acceleration or so. Thought maybe it could be a similar problem, but if you say it’s smooth ramping up than it’s probably not the case.
```

---
## \#9 Posted by: StefanMe Posted at: 2018-12-21T19:46:35.036Z Reads: 24

```
No not really... code and hardware is very different. But thanks... all thoughts are welcome! Maybe its just normal...  I don't know... I also think that the startup accelerations is a bit crapy. But this is maybe just because of the 105mm wheels and 15/38 gearing. The motor pulls just 5-8A from battery while Motor is taking 45A... my limits fare at 25battery and 60 battery. I ll swap it out for my Focbox these days. thanks
```

---

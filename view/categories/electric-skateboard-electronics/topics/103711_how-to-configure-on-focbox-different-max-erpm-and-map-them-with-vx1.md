# How to configure on FOCBOX different max erpm and map them with vx1

### Replies: 16 Views: 255

## \#1 Posted by: Pura-Vida Posted at: 2019-11-07T18:23:46.819Z Reads: 79

```
Hi all,

New French regulation requires us to restrict speed of our engine. 
* Sidewalk: 6kph (green vx1 mode)
* cycle line/road/street: 25kph (yellow vx1 mode)
* outdoors and private zone: no restriction (red vx1 mode)

I know it is possible to configure one  MAX ERPM to limit globally max erpm to a target value, but is it possible to configure different max erpm and map them with vx1 mode?

The objective is to go from home to off-road zone using public road and cycle lane as defined by regulation.

Configuration FOCBOX 23.44, vx1
```

---
## \#2 Posted by: mackann Posted at: 2019-11-08T11:30:47.275Z Reads: 70

```
No, the vx1 does only change acceleration. It have no functions to change any erpm settings.
You could get a Bluetooth module and make different modes with erpm limit and change between them with your mobile
```

---
## \#3 Posted by: Pura-Vida Posted at: 2019-11-08T12:35:49.020Z Reads: 67

```
Hi mackann,
Can you detail, as your solution seems to fit to my expectation, even it it requires to login thru BT from my phone, it will let me ride from my home to the outdoor zone (6km downtown and cycle lane).
So if you can identify components to buy, and settings to apply I will be the happiest Esk8 novice builder/rider.
My configuration is FOCBOX unity 23.44 and vx1 module
```

---
## \#4 Posted by: mackann Posted at: 2019-11-08T15:27:15.468Z Reads: 61

```
Buy this:
https://metr.at/shop

![app|230x500](upload://wf067uqz504lIrJsJBHsbIEs1ro.jpeg)
```

---
## \#5 Posted by: NullReference Posted at: 2019-11-08T15:36:11.454Z Reads: 49

```
I love my Metr.Pro. I also love the app.

Don’t use the app to configure profiles.

The only App you should ever use to write configurations to your ESC is either the VESC app for normal VESCs or FocBoxUI for a Unity. Anything else is playing with fire.

Reading configurations and stats is fine.

FocBoxUI does not support eRPM caps. The only way I can think of to configure one is to write a command to the terminal. Do not use the terminal unless you fully understand what you are doing.
```

---
## \#6 Posted by: mackann Posted at: 2019-11-08T17:21:53.647Z Reads: 46

```
Their is no problem using metr to set settings on Unity. You can even do motor detection, remote calibration, erpm limit. Its not playing with fire using unity and metr to change settings.
```

---
## \#7 Posted by: Pura-Vida Posted at: 2019-11-08T18:28:26.714Z Reads: 44

```
Hi all, thanks a lot, but for a newbie, a step by step roadbook is mandatory.
Is Metr replacing VX1 BT module?
where do I plug it (no no, please it is not a joke)?
which parameter do I have to configure? 
can somebody prepare a tutorial?
```

---
## \#8 Posted by: NullReference Posted at: 2019-11-08T19:39:09.798Z Reads: 41

```
Ask @longhairedboy how well Metr works for setting eRPM limits on a unity.

The app is fantastic for logs and the module works great, don’t write configuration with it.
```

---
## \#9 Posted by: mackann Posted at: 2019-11-08T20:07:50.009Z Reads: 42

```
I do it every day and have probebly done it on 60 different boards without any problem
```

---
## \#10 Posted by: Pura-Vida Posted at: 2019-11-09T00:09:29.088Z Reads: 40

```
Hi as you've posted that install metr is a daily task for you, please can you take and share some pictures when you will install next one? Steps from end to end
```

---
## \#11 Posted by: Anubis Posted at: 2019-11-09T09:16:37.507Z Reads: 40

```
The metr and vx1 reciver both plug into 1 vesc. The metr allows you to change the top speed and the vx1 modes how fast you can reach it.

These wont actually help you comply with the law. Your board would have to by design be limited i.e be a 6s board with slow gearing, or at least ive been told that software speed limiters arent enough.  The best solution is to get a max speed 25kmh sticker and slap it on the bottom and if you are seen over 25 claim it was a downhill or you push assisted it higher
```

---
## \#12 Posted by: mackann Posted at: 2019-11-09T15:54:38.697Z Reads: 33

```
https://media.giphy.com/media/eKCrMsVRbow2d2974s/giphy.gif
```

---
## \#13 Posted by: Pura-Vida Posted at: 2019-11-09T17:22:15.621Z Reads: 28

```
Hi Markus alias @mackann,
Thanks a lot for your tutorial, it is exactly what I was expecting.
I have some questions: 
Q1) how to upgrade metr firmware before to plug it into Focbox as noticed [here](https://www.bioboards.se/en/focbox-unity-motor-controller-settings/)?  
Q2) does Focbox UI application still continue to be operational after swapping between original and metr?

Now let back to French driving regulation. As usual, members of French assembly and senators did the job by 80%: No standard are defined, only vehicules will have to be limited to 25kph by conception, and Vehicules that will bypass this restriction using jailbreak (DIY is an alien concept for 70 y.o. assembly members) will be outlaws... Nowhere they are speaking about 6S...
```

---
## \#14 Posted by: Pura-Vida Posted at: 2019-11-10T19:08:20.234Z Reads: 21

```
[quote="Anubis, post:11, topic:103711"]
The metr allows you to change the top speed and the vx1 modes how fast you can reach it.
[/quote]

Hi Anubis, are you sure that metr can manage ERPM thru different  pre-registered and customized settings or only is able o manage MAX voltage and Ampere delivered? that is not exactly the same?
```

---
## \#15 Posted by: mackann Posted at: 2019-11-18T13:11:42.287Z Reads: 13

```
![app|230x500](upload://gMTPGv7Uriqn8yIElTHSkdUCuSS.jpeg)
```

---
## \#16 Posted by: skatardude10 Posted at: 2019-11-18T18:40:07.308Z Reads: 8

```
I can confirm that Metr pro works great to limit speed to ERPM. 

I used to use Ack fw + ESC monitor + HM-10, limiting the speed used to work and stopped working for some reason so I upgraded to Metr pro, now it's flawless. In expert mode, you can change literally every setting from VESC tool directly from the phone app, including detecting PPM range, hall sensors, and motor detection... it's scary awesome... and it even works on my modified ackmaniac 3.102 firmware as well as TCP bridge to use the desktop tool over WiFi/bluetooth
```

---

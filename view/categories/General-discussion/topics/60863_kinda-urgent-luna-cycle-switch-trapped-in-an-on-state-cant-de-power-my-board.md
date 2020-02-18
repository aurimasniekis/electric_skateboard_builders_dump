# \[kinda urgent\] Luna cycle switch trapped in an on state, can&rsquo;t de-power my board

### Replies: 13 Views: 796

## \#1 Posted by: osbor Posted at: 2018-07-04T06:29:23.971Z Reads: 142

```
this guy right here
https://lunacycle.com/remote-on-off-solid-state-switch/
a really great anti spark, fuse, and power switch all in one
except now it's trapped in the on state.

i brushed against the exposed leads for the power switch extension cable, and boop the board turned on without the actual physical switch even present. Now there's no way to de-power the board except to unplug the xt90 connectors entirely, and as soon as they're plugged back in the board is alive. it's like the solid state switch is stuck in the on state forever.

Note how the switch is un-depressed which should mean it's off but...

![IMG_20180703_232715|374x500](upload://7o9ZhKlLt60BbF1M16ZuU2oyc6m.jpg)

![IMG_20180703_232733|374x500](upload://t9UdJHOcBBGDM6Uq344x1vLyem6.jpg)

what do?
```

---
## \#2 Posted by: Maxid Posted at: 2018-07-04T06:44:32.174Z Reads: 129

```
You MOSFETs are damaged and failed as open - that's common. You need to get a new switch.
```

---
## \#3 Posted by: Eboosted Posted at: 2018-07-04T07:03:58.688Z Reads: 119

```
Damn, I had high hopes for that switch.

I even placed an order online today. 

@goldenhusky are the only switches alive now.
```

---
## \#4 Posted by: osbor Posted at: 2018-07-04T07:06:26.939Z Reads: 117

```
oh come the F on
this build is cursed at this point, so many annoying setbacks all the time, ugh
```

---
## \#5 Posted by: Maxid Posted at: 2018-07-04T07:29:48.403Z Reads: 109

```
Well I just ordered one from @Martinsp that looks quite nice (comes with a small aluminium plate as heatsink). Haven't tried it yet but maybe you can give him a shot as well... he's in Slovakia though.

Edit: and when looking at this http://electricskateboard.repair/index.php?id_product=41&controller=product it seems like I ordered too early - damn it! :D
```

---
## \#6 Posted by: TarzanHBK Posted at: 2018-07-04T08:33:10.376Z Reads: 95

```
That´s freggin awesome! Good find!
@Martinsp get some updates flowing!
```

---
## \#7 Posted by: Martinsp Posted at: 2018-07-04T09:59:14.080Z Reads: 85

```
Hi guys,

@Maxid Thank you for the mention! :slight_smile:

I have a working test unit but it looks far from presentable so right now I am waiting for PCBs to be manufactured and some mouser&Farnell deliveries. I should have the switches ready at the end of next week, both the regular ones and the push to start. The push to start will still have an option to add a button to disable the push to start feature. And after probably 1 minute of not riding the board will turn off. What are your thoughts about the time after which it should turn off?

Martin.
```

---
## \#8 Posted by: TarzanHBK Posted at: 2018-07-04T12:35:08.557Z Reads: 64

```
Thats awesome!

I think the time differs from person to person. One Minute could be too short for a heavy crowded traffic light, so your board shuts down and you don't recognize it when you wanna start again. After that the vescs need a Short period to boot again before they are ready again. This could throw some people of, if you're not prepared. 
I personally think 5min is optimal for me.
```

---
## \#9 Posted by: Martinsp Posted at: 2018-07-04T12:49:51.811Z Reads: 62

```
Thank you for the feedback! I will probably create a thread when I have at least pictures to show people and create a poll to find the sweet spot. The switch will have a small MCU on board so the timing will be controlled in the firmware so I could change it if someone would want some custom period of time.
```

---
## \#10 Posted by: Battosaii Posted at: 2018-07-04T12:57:00.160Z Reads: 61

```
A way for the user to adjust it to their liking would be best.
```

---
## \#11 Posted by: Martinsp Posted at: 2018-07-04T13:05:32.766Z Reads: 53

```
I thought of that actually but I have not implemented that in the hardware since that would ideally need some kind of readout and adding like a display is not worth it I think, that would drive the cost and physical size up :/ I will try to add some simple way of adjusting the timing
```

---
## \#12 Posted by: Jc06505n Posted at: 2018-07-04T13:27:57.478Z Reads: 56

```
Will the switch be momentary ? Been trying to find one that’ll allow custom inputs , such as a slight push displays battery %, a long Push turns on the board :turn off etc.
```

---
## \#13 Posted by: Martinsp Posted at: 2018-07-04T13:30:40.432Z Reads: 56

```
I have actually designed and made a switch with a momentary pushbutton. It had an attiny13 on board but I never actually put it up for sale. 

I dont want to steal a thread like this, I am sorry. I will create a new one in a moment

https://www.electric-skateboard.builders/t/push-to-start-switch-coming-soon/60879
here is the new thread, if any of the mods see this, please move the replies that are of topic to there. Thank you. :)
```

---

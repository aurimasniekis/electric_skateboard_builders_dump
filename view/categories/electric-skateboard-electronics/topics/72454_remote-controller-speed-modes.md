# Remote controller speed modes

### Replies: 15 Views: 510

## \#1 Posted by: JensSjogren Posted at: 2018-10-26T20:17:49.516Z Reads: 149

```
Hi! So i just finnished my Trampa build and i'm very very happy with the result! My only real concern is that i'm only able to use one speed mode, the controller i use is the 2.4 Ghz nano controller from Torqueboards and it has a switch that should allow me to have 2 speed modes. However there is no difference in power when i flip the switch. i'm not sure if this has to be configurated in the VESC tool but i cannot find anything about speed modes in the tool. The ESC's i'm using are Focboxes. basicly, is it possible to configurate two different speed modes on a DIY board? The insane power i get atm is definitly not needed most of the time and it would be great to have a cruising mode to save some power 

Best regards//Jens
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-27T11:30:19.865Z Reads: 129

```
If I remember it should change acceleration curve or maybe it is just top speed. @torqueboards might be able to help
```

---
## \#3 Posted by: Komamtb Posted at: 2018-10-27T11:48:18.122Z Reads: 117

```
Did you do your ppm detection while the remote was in the higher mode?
```

---
## \#4 Posted by: JensSjogren Posted at: 2018-10-27T12:02:42.609Z Reads: 115

```
[quote="pat.speed, post:2, topic:72454, full:true"]
If I remember it should change acceleration curve or maybe it is just top speed. @torqueboards might be able to help
[/quote]

Yeah i want it to change the acceleration curve, one mode for more casual cruising but still get to the same top speed and one "sport/dirt trial" mode with insane acceleration. Ive seen that i can modify the acceleration curve in the vesc tool but that doesnt solve the speed mode problem
```

---
## \#5 Posted by: JensSjogren Posted at: 2018-10-27T12:03:50.098Z Reads: 107

```
[quote="Komamtb, post:3, topic:72454, full:true"]
Did you do your ppm detection while the remote was in the higher mode?
[/quote]

Hmm never paid attention to that, it is highly possible that it was in the high mode, should that not be the case?
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-27T12:10:31.887Z Reads: 102

```
If you adjust it in the low speed, your low speed will work like high speed and your high speed like high speed too.
😅 hope that was not more confusing 😅
```

---
## \#7 Posted by: JensSjogren Posted at: 2018-10-27T13:32:14.693Z Reads: 95

```
[quote="Andy87, post:6, topic:72454"]
If you adjust it in the low speed, your low speed will work like high speed and your high speed like high speed too.
[/quote]

i think i got it, so basicly i need to do the PPM detection again and make sure that the switch is set to high speed? Is there anything else i have to do in the vesc tool or should the low speed mode work after that?
```

---
## \#8 Posted by: Andy87 Posted at: 2018-10-27T13:54:15.324Z Reads: 86

```
I don’t know about any speed settings in the vesc tool. You can make it via remote or app only I think.
Yap try to do the ppm confit in the high mode. The low mode should be work than. I hope.
```

---
## \#9 Posted by: JensSjogren Posted at: 2018-10-27T13:58:36.162Z Reads: 84

```
thank's i'll try this out right away!
```

---
## \#10 Posted by: JensSjogren Posted at: 2018-10-27T16:29:08.174Z Reads: 75

```
Didnt seem to make any changes at all sadly, guess ill try to contact torqueboards.
```

---
## \#11 Posted by: dareno Posted at: 2018-10-27T19:04:16.509Z Reads: 71

```
Set the ppm calibration in slow mode.  then set it again in high.
```

---
## \#12 Posted by: SecrIT Posted at: 2018-12-14T10:46:25.032Z Reads: 56

```
I seem to have the same issue.

I have a Benchweel remote + Flipsky vESC 4.12a.

I run the PPM wizard in low mode, and then when i try to use high the board just dies out when accelerating.

When i re-run the PPM wizard in HI mode then LO mode doesnt really work.

I want the same outcome as @JensSjogren .  I'd like low to be simple acceleration and hi to be more sporty.

If this is possible can someone be more explicit on how to configure this.

My steps are below that gave me a poor outcome.
-Run PPM wizard in lo mode and apply config
-Run PPM wizard in hi mode and apply config
(basically the last mode i ran the wizard in, is the only mode that works on the controller) 

thx
```

---
## \#13 Posted by: JensSjogren Posted at: 2018-12-14T14:15:00.723Z Reads: 47

```
I managed to solve the issue, i thought that i had set the PPM calibration in high mode since it seems logical for me that the remote is in high mode when the switch is facing upwards. This was not the case on my remote, the lower position is "fast" mode and the higher position is "slow" mode and thus i had set the pulsewidthlenght that was showing on slow mode. That's the reason why both modes was the same. 

When i set the pulsewidthlenght in high mode and then switched over to slow mode i could see in the VESC tool that throttle only went up to 70% on full throttle. So my TB nano remote seems to have slow mode preset to 70%, dont know if this is changeable. In real testing i barely notice any difference in acceleration between 100 and 70%. Top speed is also the same so it would be nice to havr slow mode at 50%. 

Not sure if that madr any sense at all 😅
```

---
## \#14 Posted by: SecrIT Posted at: 2018-12-14T14:49:34.501Z Reads: 40

```
It does make sense now.

It is my misunderstanding.

I thought that both modes would need to be calibrated, and that the remote would somehow limit the amperage.

But really what it seems that the procedure should be:
-Calibrate in HI mode only
-Low mode is only a fractional percentage of HI mode so you will only get 50-70% of what HI offers

thanks!
```

---
## \#15 Posted by: JensSjogren Posted at: 2018-12-14T15:27:22.592Z Reads: 31

```
That is correct, i suppose that different remotes has different setups for the speed modes. You will see in the pulsewidthlenght setup that the slow mode gives a different percentage value on full throttle once you set it up in fast mode.
```

---

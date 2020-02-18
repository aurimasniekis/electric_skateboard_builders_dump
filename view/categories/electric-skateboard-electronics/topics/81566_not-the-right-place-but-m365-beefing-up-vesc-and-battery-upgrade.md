# Not the right place BUT - M365 Beefing UP &ldquo;Vesc and Battery Upgrade&rdquo;

### Replies: 14 Views: 1270

## \#1 Posted by: AlanZhou Posted at: 2019-01-21T01:48:40.902Z Reads: 133

```
Hey so i have a segway es4 and 20mph is not quite fast enough for me (limited by firmware), so I was thinking of getting an m365 and modding the hell out of it, "talking whole new battery and heatsinked vesc", but I have a few concerns, how would I get the rear light (rear light blinking) and the throttle connected? and how do I get the 4 indicator lights on the dash to work? oh was also thinking of adding an extra 10s4p along with a 10s3p inside the m365

Ps - there was nothing on the internet, so I thought you guys would know how to do this :rofl:

![M365%20MOD1|640x360](upload://vXXlw6IckZD05moD4085JDnnJOt.jpeg) ![m365%20MOD2|690x460](upload://1rPjR6v4Xj7O6hhC9WcBpFT54ZY.jpeg) ![M365%20MOD3|480x485](upload://kiXHcqDRTKftgxGkFfVLii8oEqw.png)
![m365%20MOD4|690x325](upload://rje8EiOgIgimpHg793CLvlnzEK5.jpeg)
![m365%20Mod5|690x326](upload://klUSvnrTObLQSRnma53Z13vFCJl.jpeg)
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-01-21T02:12:30.532Z Reads: 118

```
Does nobody on the internet know how to do this kinda stuff :sob:
```

---
## \#3 Posted by: Eboosted Posted at: 2019-01-21T05:46:47.515Z Reads: 115

```
I think there are some unicycle modders out there who could help you with these questions, as you said this might not be the best place
```

---
## \#4 Posted by: ninTHIENdo Posted at: 2019-01-21T06:03:14.168Z Reads: 107

```
With the 365, you would just need to flash the old firmware to get the crazy speed originally on it.
```

---
## \#5 Posted by: AntiumOne Posted at: 2019-01-21T08:41:02.932Z Reads: 94

```
This is definitely in the realm of possible. You won't be able to make everything work super easily but anything is possible with microcontrollers, sensors, and a little but of software. I currently have a m365 and I have been planning to mod it as well.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-01-21T15:17:37.266Z Reads: 73

```
[quote="ninTHIENdo, post:4, topic:81566, full:true"]
With the 365, you would just need to flash the old firmware to get the crazy speed originally on it.
[/quote]

I arleady know that I'm trying to install a vesc

[quote="Eboosted, post:3, topic:81566"]
as you said this might not be the best place
[/quote]

All my questions were related to vesc which experts on here should be able to answer
```

---
## \#7 Posted by: linsus Posted at: 2019-01-21T15:25:56.628Z Reads: 70

```
Might want to look on the VESC forum if you need more technical answers. 
My guess would be that you need a few free I/O pins from the MCU, think there are 2-3 on the 4.12 if thats what you're using. Prob not routed on the PCB however. After that you'd need to write some code to make it all work. Think BV had some LED strips controlled as brakelight and even turn signal in combination with the NRF..but that was years ago. 

Regarding the battery gauge its probably voltage dependant, so if you stay in the same range as the meter, it should work pretty much plug n play. Else you'd need a new gauge or do a voltage divider net or smthn.

Not sure what the throttle is but PPM is a high possibility since its usually the cheapest.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-01-21T15:29:54.581Z Reads: 62

```
[quote="linsus, post:7, topic:81566"]
Regarding the battery gauge its probably voltage dependant, so if you stay in the same range as the meter, it should work pretty much plug n play
[/quote]

It's actually my another pcb that also connects to the brake (that controls the rear light) and throttle and has it's own microcontroller that controls what mode the scooter is on (on the stock esc) so that's why I'm just gonna plunk down a davega on top of the dashboard and hook it up to the vesc

And the throttle is ppm

**Worst case senro I don't have rear lights and battery gauge and throttle is not working
```

---
## \#9 Posted by: linsus Posted at: 2019-01-21T15:32:43.726Z Reads: 60

```
Is there a MCU on the throttle/batterygauge/brake PCB? If so it probably does avraging of the battery voltage to not illustrate sag on the LED gauge. You could try find the interface to the LED gauge and see if its of any use at all.
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-01-21T15:35:06.677Z Reads: 59

```
![jpg_640x640|500x500](upload://gGaLpul0M7Sy7I8cBG2OZiXr3Sj.jpeg) 

The m365 actually has two Modes on the stock esc, Eco and normal.

The mcu also controls the headlight on off along with the power button



All other hacks on the m365 use 3 pins out of 4 on the dash mcu to install a dashboard displaying speed and range left, on a lcd dispaly
```

---
## \#11 Posted by: sami Posted at: 2019-01-21T15:41:54.394Z Reads: 59

```
Following... I have m365 too. Want to see what you make and copy :stuck_out_tongue_winking_eye:
```

---
## \#12 Posted by: linsus Posted at: 2019-01-21T15:46:16.080Z Reads: 57

```
Looks like that MCU on there does some magic after all. Is it only 2 leads(cables) to the battery gauge, or several?
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-01-21T16:03:25.338Z Reads: 55

```
[quote="linsus, post:12, topic:81566, full:true"]
Looks like that MCU on there does some magic after all. Is it only 2 leads(cables) to the battery gauge, or several
[/quote]

Theres a mcu on the esc and the bms too lol, and actually there are 4 led lights soldered on the pcb that the mcu is on and one of the lights turns green on eco
![M365%20MOD7|300x300](upload://rCpgKKC4cNatClvUn8Z01SE6GYI.jpeg)
```

---
## \#14 Posted by: sami Posted at: 2019-01-28T08:34:29.126Z Reads: 33

```
https://vesc-project.com/node/325

this might help you...
```

---

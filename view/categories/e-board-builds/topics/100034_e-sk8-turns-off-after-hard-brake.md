# E-Sk8 turns off after hard brake

### Replies: 27 Views: 359

## \#1 Posted by: E-Sk8er Posted at: 2019-08-10T08:48:03.310Z Reads: 112

```
Heyy guys

I have some problems with my new build diy e-sk8. I am using dual VESC 4.12 from Torque boards, dual Hobbyking sk3 5055 280kv motors and a 10s3p Battery from diyeboard.com. The Problem is that the board often turns off after a hard brake. Not sure what to do. Btw I'm using the BLDC-tool. 
Hope that someone can Help me(:
```

---
## \#2 Posted by: L3chef Posted at: 2019-08-10T08:53:06.484Z Reads: 105

```
Start by posting your settings.. 10s and 280kv motor is not the best idea since you will have too high erpm with 4.12
```

---
## \#3 Posted by: E-Sk8er Posted at: 2019-08-10T10:21:48.259Z Reads: 99

```
![IMG_3081|666x500](upload://b3PveqpNpRjyFoOuiC6jM4ZwXUB.jpeg)
```

---
## \#4 Posted by: E-Sk8er Posted at: 2019-08-10T10:22:33.821Z Reads: 92

```
![IMG_3083|666x500](upload://zFD9O1SZrUzaZkUBhQuFwfzKNq7.jpeg)
```

---
## \#5 Posted by: E-Sk8er Posted at: 2019-08-10T10:23:11.031Z Reads: 89

```
![IMG_3085|666x500](upload://4WLaYUcF2dgg9A7lijplOisWYPT.jpeg)
```

---
## \#6 Posted by: E-Sk8er Posted at: 2019-08-10T10:23:49.836Z Reads: 87

```
![IMG_3087|666x500](upload://bfmG1N8LFGljJhz5SUchI8yaXBo.jpeg)
```

---
## \#7 Posted by: E-Sk8er Posted at: 2019-08-10T10:24:04.922Z Reads: 81

```
![IMG_3088|666x500](upload://e4HYVqASH5cJhzL4DPDRLkZNWP5.jpeg)
```

---
## \#8 Posted by: L3chef Posted at: 2019-08-10T10:49:52.229Z Reads: 81

```
Jeesus you are teying to pull 99amp from a china battery with 3p.. Most likely fake cells.
And then charge it with 60a...

Have you changed the erpm value? 4.12 should be 60k and -60k if it's not a upgraded 4.12
```

---
## \#9 Posted by: taz Posted at: 2019-08-10T10:53:46.475Z Reads: 79

```
No he is not.
The battery amps will be limited by the motor amps.
```

---
## \#10 Posted by: L3chef Posted at: 2019-08-10T10:58:54.139Z Reads: 78

```
Yeah you're right. Still it's a high number since he doesn't know what cells are in use.
```

---
## \#11 Posted by: E-Sk8er Posted at: 2019-08-10T11:21:11.486Z Reads: 76

```
What could be the problem to cause the VESC to turn off
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-08-10T11:28:16.046Z Reads: 75

```
No its probably the bms just tripping overcharge protection
```

---
## \#13 Posted by: E-Sk8er Posted at: 2019-08-10T11:29:13.909Z Reads: 75

```
How much amps should i set for regen.
```

---
## \#14 Posted by: L3chef Posted at: 2019-08-10T11:30:16.415Z Reads: 72

```
Depends on what cells you have. Any idea?
```

---
## \#15 Posted by: E-Sk8er Posted at: 2019-08-10T11:31:53.982Z Reads: 70

```
They are 18650 Cells
```

---
## \#16 Posted by: L3chef Posted at: 2019-08-10T11:34:02.246Z Reads: 69

```
Yes but what brand?
```

---
## \#17 Posted by: E-Sk8er Posted at: 2019-08-10T11:39:37.809Z Reads: 71

```
I have no Idea and on diyeboard.com they dont name any brand):
```

---
## \#18 Posted by: visnu777 Posted at: 2019-08-10T11:42:35.468Z Reads: 71

```
Absolutely. Its still -73A altogether in this dual setup, I'm also sure that its overcharge protection. Limit battery current max regen to -10 per VESC and try it out.
```

---
## \#19 Posted by: E-Sk8er Posted at: 2019-08-10T11:43:29.084Z Reads: 71

```
Thx for the help(:
```

---
## \#20 Posted by: Voxu Posted at: 2019-08-10T12:30:11.872Z Reads: 69

```
![Screenshot_20190810-142736_Samsung%20Internet|690x237](upload://sWVfCmcSCHZ8ovIQy7UsndPgdXg.jpeg) ![Screenshot_20190810-142722_Samsung%20Internet|690x139](upload://8hUU1fr6Qtd1AzeGEbRiGTjIzS8.jpeg)
```

---
## \#21 Posted by: Voxu Posted at: 2019-08-10T12:30:32.003Z Reads: 67

```
Samsung 22p
```

---
## \#22 Posted by: visnu777 Posted at: 2019-08-10T12:42:24.339Z Reads: 66

```
uhhh... Then your whole pack can deliver 30A continuous and charging is at 6A max. Your settings are way out of specs. Limit battery current to 15A per VESC and battery regen to -5A per VESC.
The BMS is still a possible factor too...
```

---
## \#23 Posted by: Voxu Posted at: 2019-08-10T12:46:40.128Z Reads: 63

```
They have a built in BMS in their battery packs. Probably not bypassed and some shitty discharge rate that triggers the BMS with your settings.
```

---
## \#24 Posted by: MiniChopper4Me Posted at: 2019-08-10T19:40:20.519Z Reads: 54

```
This.

I had a pack custom made in China, asked for bypassed discharge, and they STILL put it discharge protected.
```

---
## \#25 Posted by: Waiboard Posted at: 2019-08-10T23:10:23.763Z Reads: 50

```
I am having a similar problem but in my case I get cuts accelerating and also braking. I have tried many configurations.

My battery is 10s4p Samsung 25r with BMS of 100A continuous for charging and discharging. Two Flipsky 6354 190KV engines and a VESC 4.20 dual Plus.

I currently have the VESC-Tool configuration in: Motor: 15 / -10 (very weak brakes); Battery: 15 / -4

With this configuration I am getting much less cuts than with higher value settings, but still cutting.
I don't know where I can have a problem anymore. But my doubt is if the BMS may be causing a cut even though it admits 100A continuous and 200A peak.

I would appreciate your feedback.
```

---
## \#26 Posted by: visnu777 Posted at: 2019-08-11T07:42:20.008Z Reads: 41

```
If you are capable of soldering you can bypass you BMS for discharge, at least for testing that. You can charge with 4A per cell without problems, meaning 16A@4p and -8A per VESC. Discharge can be 80A total, 40A / VESC. The motor settings are almost independent from this, so you could just run the new detection for values close to the real specs of the motors. Try setting 50/-50A motor.
Cutouts might also be caused by bad connections / cabling. WIth max discharge you are in the 10AWG domain ;)
```

---
## \#27 Posted by: Ryian Posted at: 2019-09-05T07:14:00.359Z Reads: 20

```
If the battery is full charged , esc auto shut it off to avoid overcharging,
```

---

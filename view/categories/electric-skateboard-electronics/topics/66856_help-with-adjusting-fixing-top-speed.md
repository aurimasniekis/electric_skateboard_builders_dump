# Help with adjusting/fixing top speed

### Replies: 21 Views: 432

## \#1 Posted by: Taliesin Posted at: 2018-09-02T18:48:25.598Z Reads: 129

```
My board is finally up and going but it feels really slow (roughly 10mph tops) and I’m assuming/hoping it has to do with my vesc settings.

I weigh 205lbs

12s4p 30q battery going to a bestech BMS 

Dual 6374 190kv 3200W motors to dual ESCapes with ppm splitter


In vesc tool:

FOC mode

Motor current max: 60
Motor current max brake: -60

Battery current max: 80
Battery current Max Regen: -12

I have my ERPMs reduces from 100,000 to 60,000 for + and -

Hall sensors work fine and it passes all the setup wizard tests with no issues.

Any help or suggestions?
```

---
## \#2 Posted by: linsus Posted at: 2018-09-02T18:52:44.151Z Reads: 123

```
What BMS is it? Charge only or Charge and discharge?
Do you get any fault codes when benchtesting? (red lights from FOC boxes)

Try switching to BLDC mode and see if you have same behavior

**Edit dont forget voltage tresholds, (over and under voltage etc) not only current that needs to be put in
```

---
## \#3 Posted by: Taliesin Posted at: 2018-09-02T19:49:23.701Z Reads: 114

```
It’s the HCX-D596 bms
```

---
## \#4 Posted by: linsus Posted at: 2018-09-02T19:50:54.312Z Reads: 114

```
[quote="Taliesin, post:3, topic:66856, full:true"]
It’s the HCX-D596 bms
[/quote]

Assuming its connected [properly](https://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14), you should have alot of juice running thru without a problem then. What about the other parts? Can you show us a dump of your vesc tool settings?
```

---
## \#5 Posted by: mccloed Posted at: 2018-09-03T04:43:30.271Z Reads: 95

```
I’m not so sure it would be the BMS. Those usually cut out,not slow down. Maybe try adjusting the ERPM back up to 100000? What do you have the voltage cut-offs set to?
```

---
## \#6 Posted by: Taliesin Posted at: 2018-09-03T04:46:34.092Z Reads: 92

```
My battery wasn’t charged....

My voltage meter wasn’t setup/connected properly to the battery so it was reading 100% even though it was actually at 0%.

It’s all good and the board is fast as fuck now.

I’ll get the voltage numbers though regardless.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-03T06:01:46.711Z Reads: 90

```
[quote="Taliesin, post:1, topic:66856"]
Battery current max: 80
Battery current Max Regen: -12
[/quote]

Take care with your battery max setting.
If you run 80A for both escapes than all good and ignore my comment.
If you set 80a in every escape than please split it to 40a on each escape.
your battery can´t handle 160a and I guess the escape could fry over 60a too. ;)
```

---
## \#8 Posted by: Taliesin Posted at: 2018-09-03T06:52:55.759Z Reads: 86

```
Thank you for that. I will go back and adjust them to 40
```

---
## \#9 Posted by: Winfly Posted at: 2018-09-03T10:26:56.864Z Reads: 74

```
Also reduce that Regen to -8A if you don't wanna ruin your cells
```

---
## \#10 Posted by: Andy87 Posted at: 2018-09-03T11:22:17.412Z Reads: 69

```
if he don´t plan to constant break a 3km hill he should be fine with
24A in total too. the break current appears usually just for some seconds.
the q30 should handle this.

side mark:
I don´t think it´s true, but when I blow my first vesc the guy how sold me his 4.12 vesc said that my settings (dual -6A) on the vesc was too low and the break current resulted in heat up the drv....
If somebody can say if it´s right or just bullshit, it would be interesting for me
```

---
## \#11 Posted by: Nordle Posted at: 2018-09-03T11:25:57.296Z Reads: 64

```
i’m no expert, but less amps = more heat sounds like bs...
```

---
## \#12 Posted by: Andy87 Posted at: 2018-09-03T11:36:54.809Z Reads: 61

```
let´s say like this:
the breaking current depend not only from your bat min settings, also from your motor min setting. If to set the motor min to -45 and the bat min to -6A
the break energy need to go somewhere. that´s the -6a back to the battery and the rest into heat of the motor and maybe also the vesc somehow.
but this I don´t know. would like to know if the break energy also transform into the heating of the vesc?
the thing is, that I would assume that in my specific case the vesc should not blow, but shut down because of overheating. there was no overheating, so I don´t understand how it could cause the blown drv.
```

---
## \#13 Posted by: Nordle Posted at: 2018-09-03T11:45:52.609Z Reads: 58

```
that sounds logic, but then only fets should heat up and that should just result in thermal shut down sooner than later, like you said.
```

---
## \#14 Posted by: Taliesin Posted at: 2018-09-03T17:24:40.737Z Reads: 51

```
Well here’s what I have set now. (Dual ESCapes so I reduced to 40 on bat current max like Andy said.)

Should I keep the bat current regen at -12 or go to -8?

![image|374x500](upload://vnz6bnSkfSFMiaJFqVQnCim8iLV.jpeg)
```

---
## \#15 Posted by: Taliesin Posted at: 2018-09-03T17:25:34.416Z Reads: 53

```
And here’s my voltage thresholds someone asked for (I think?)

![image|374x500](upload://dtfwRGno3KI2XMDeAdAtFzSwCK4.jpeg)
```

---
## \#16 Posted by: Newby Posted at: 2018-09-03T22:21:43.314Z Reads: 46

```
There isn't really a set answer for that question. Consider how long you brake for, gradient, hills etc. If you're not slamming on the brakes you might only be using half your regen max anyway.  But anyway it's a vesc pick the safe option first and you can always change it
```

---
## \#17 Posted by: Taliesin Posted at: 2018-09-03T23:58:50.489Z Reads: 43

```
Would -12 or -8 be considered the safe option?
```

---
## \#18 Posted by: Namasaki Posted at: 2018-09-04T02:56:25.265Z Reads: 38

```
Find out what the safe fast charge limit is for your battery and divide by 2 for dual Vescs.
Thats where you set the Battery Min.
The Motor Min can be higher. 
I run my Motor Min at -40 and Battery Min at -12  for My Lipo build that is capable of 25a fast charge according to manufacturer.
```

---
## \#19 Posted by: MaxMalouf Posted at: 2018-09-04T04:51:50.112Z Reads: 31

```
Um so your board was going 10mph at low battery? what?
```

---
## \#20 Posted by: Namasaki Posted at: 2018-09-04T04:53:28.032Z Reads: 29

```
Probably activated the Vesc low voltage start which is a soft back off strategy.
```

---
## \#21 Posted by: Andy87 Posted at: 2018-09-04T05:05:16.507Z Reads: 26

```
You can save set your battery cut off start to 3V per cell and cut off end 2.8V.
Will give you a bit more of range 😉
LiIon can discharge till 2.5V, so with 2.8V you still have a good buffer.

With LiPos it’s a different story, there you need to cut off at 3.5V per cell.
```

---

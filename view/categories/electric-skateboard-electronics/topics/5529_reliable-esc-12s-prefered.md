# Reliable ESC (12s prefered)

### Replies: 22 Views: 2709

## \#1 Posted by: Stevemk14ebr Posted at: 2016-07-03T22:53:52.047Z Reads: 189

```
I just got all if my board parts about a week ago and have had quite a few issues with the TB 12s esc's. I had the first esc's bec blow out after using the board twice. The esc still worked so i bought an external bec and hooked it up. That worked for one ride and then the OTHER esc completely died and isn't powering the motor at all, nor being recognized by the programmer. Im experienced in electronics and went over all the components on the pcb and nothing obvious is fried and the ic is still functioning fine so idk what's up.

 Tldr; both of the esc's i bought are garbage so im looking at geting two new ones. I'd like to run at 12s for efficiency but im wiling to go to 6s if needed. Im looking at the mamba monster 2 escs if i were to go 6s, can anyone vouche for these? 

Are there any other good choices for a 12s esc?

Parts: 
2x 230kv  tb motor
Tb v4 mount, motors, wheels, etc
2x 25c 5000mah zippy in series
Loaded vanguard deck
Custom abs enclosure
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-03T23:00:00.022Z Reads: 183

```
The VESC. Have you got a refund from @torqueboards ?

EDIT: Why are you running 230kv with 12S?
```

---
## \#3 Posted by: torqueboards Posted at: 2016-07-03T23:03:15.672Z Reads: 183

```
Only other 12S option would be VESC atm. Surprising this has happened. Kinda weird that has happened and I haven't experienced that before.

If your ESC's aren't totally trashed as in you swapped the connectors, etc. I'll replace it. If it happens again it might be a setup issue.
```

---
## \#4 Posted by: Stevemk14ebr Posted at: 2016-07-03T23:04:28.198Z Reads: 174

```
From what i understand the vesc @12s with 230kv motors would be over the erpm limit? Plus i kind of want the vesc 6.0 as i like that he controls the fets directly without the drv chip that people fry all the time. 

Tb offered to replace the esc with the blown bec for $30 but then i had the other esc blow out and im reconsidering
```

---
## \#5 Posted by: torqueboards Posted at: 2016-07-03T23:07:38.611Z Reads: 169

```
I am interested to know how it failed almost immediately. You can tell by the design and quality of construction that the ESC is of quality. I'll replace both for the price + shipping. If you happen to re-consider.. I'm definitely interested to know what happened. Failure rate is pretty low if not non-existent.
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-03T23:07:39.231Z Reads: 163

```
It will be over the ERPM limit. Why are you using 230kv with 12S? 149-170 would be way better.
```

---
## \#8 Posted by: torqueboards Posted at: 2016-07-03T23:10:22.501Z Reads: 163

```
Couldn't be amp draw. I run it perfectly fine. :confused:
```

---
## \#9 Posted by: Stevemk14ebr Posted at: 2016-07-03T23:22:52.095Z Reads: 163

```
This is how everything was hooked up, the little black thing attached to the 9v battery is a linear regulator pumping out 5v @1A. This is the external bec i used once the integrated one blew on the first esc. Before the integrated bec blew i had it hooked up just as you recommend with only the y splitter <img src="/uploads/db1493/original/2X/9/9e22cc8fb9a6f6ae0f64b6c97903685abcebc7bb.jpg" width="281" height="500"> 

 i ran 230kv as ive seen others go as high as 270ish? The amp draw should have been fine on the bec, i measured the amp draw of all the parts hooked to the bec and it was only 50mA total (@5V) so that was likely just a faulty part. As for why the other esc failed i have no idea, i spent two hours measuring each component on the pcb and nothing was wrong. I also found that the esc uses the si labs C8051F31x chip and did a hardware reset as the manual posted and that didnt fix it either. 

@torqueboards the escs are still all together i just took off the covers to get to the pcb. The one has a blown ubec but other than that stil functions. And the other that didnt have a ubec is dead afaik. What would be the total arrangment if i were to exchange them?
```

---
## \#10 Posted by: torqueboards Posted at: 2016-07-04T00:06:59.788Z Reads: 154

```
@Stevemk14ebr I emailed you some details steve.
```

---
## \#11 Posted by: Stevemk14ebr Posted at: 2016-07-04T00:20:15.444Z Reads: 152

```
@torqueboards Thanks, ill do all that tomorrow and have them shipped out aswell if the post office is open. 

Im curious though has anyone tried out the mamba monster esc's i mentioned?
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-07-04T00:30:14.803Z Reads: 147

```
It's the 🇺🇸 4th of July.....(unless ur not in the US) Banks and post is closed....but I hear they have some great sales tomorrow! Lol
```

---
## \#13 Posted by: willpark16 Posted at: 2016-07-04T00:35:40.916Z Reads: 147

```
Try Miami boards he does testing on each esc before shipping
```

---
## \#14 Posted by: thisrealhuman Posted at: 2016-07-04T02:04:02.758Z Reads: 144

```
You blew out the BEC on an ESC advertised as OPTO, meaning that it has no BEC. I must be missing some info.
```

---
## \#15 Posted by: torqueboards Posted at: 2016-07-04T02:07:02.650Z Reads: 139

```
@thisisrealhuman. There are 2 versions. One w/ a BEC and one that is OPTO. He had one of both. Blew out the one w/ BEC.
```

---
## \#16 Posted by: barajabali Posted at: 2016-07-04T05:00:33.833Z Reads: 133

```
im my experience the @torqueboards esc without the BEC is bullet proof. 

not sure about that new one though.
```

---
## \#17 Posted by: lox897 Posted at: 2016-07-04T07:29:39.536Z Reads: 130

```
Same as @barajabali
```

---
## \#18 Posted by: Stevemk14ebr Posted at: 2016-07-04T11:41:21.110Z Reads: 113

```
I hope i have a better experience with the replacement parts then! I bought these esc's as i heard good things too
```

---
## \#19 Posted by: Menwaylo Posted at: 2016-07-04T13:51:53.446Z Reads: 112

```
I have also had some issues with my TB 12s esc I have one with the bec and one w/o. I Am working with TB now but nothing is helping so far,they do not operate at the same speed. If I cannot get them to work I will have to change my setup to 8s 😭  Which one did you get for a replacement? With ubec w/o ubec?
```

---
## \#20 Posted by: Stevemk14ebr Posted at: 2016-07-05T00:07:50.615Z Reads: 101

```
The motors are going to spin at different speeds since the controllers don't talk to each other. As long as your controllers actually spin the motors then yours are working just fine.
```

---
## \#21 Posted by: exnor Posted at: 2016-07-14T20:36:03.334Z Reads: 85

```
I have the mamba! Do ask me anything you want, I fucked up gluing the enclosure so at the moment I can't connect it to the pc to update settings but it's pretty configurable, right now, I have the brake curve too aggressive maybe.
```

---
## \#22 Posted by: Stevemk14ebr Posted at: 2016-07-14T22:02:36.707Z Reads: 77

```
What all does it let you adjust? How hot does it get? Is it loud at all? Is it constructed well? How long have you had it, and how much has it been used, as well as your personal opinion on its quality. Thanks!
```

---
## \#23 Posted by: exnor Posted at: 2016-07-18T00:02:02.156Z Reads: 65

```
I couldn't test it much but it lets you adjust accelaration curves, brake curves, max speed, reverse mode, and a couple things that are for RC cars and don't make sense in a skateboard. What do you mena loud? The construction is awesome and it's waterproof. I've had it for a month and a half by now, not much. I'd have to adjust its settings somehow better but I glued the case so I can't connect it to the PC anymore and for now don't wanna break the case haha, but with a little steeper accel. curve and a not so brake curve I think it'd be pretty great. Have to test the VESC someday to compare though... See you!
```

---

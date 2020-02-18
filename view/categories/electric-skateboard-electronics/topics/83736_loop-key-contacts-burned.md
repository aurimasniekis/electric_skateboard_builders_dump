# Loop key contacts burned

### Replies: 25 Views: 323

## \#1 Posted by: High-roller Posted at: 2019-02-09T18:56:36.072Z Reads: 98

```
Can someone help me with this? I was going to start running motor detection, all the wires were properly connected. When I plugged in my key there was a small 'pop' and then nothing. The vesc doesn't turn on, or the reciever. There doesn't seem to be any visible damage to the vesc or other components, just the loop key socket:  
![image|281x500](upload://5H4dExCfqGlDyln01fG1NRKquhH.jpeg)
Both it and the key were new. There was a little bit more resistance than I expected when pushing the plug all the way in, but there wasn't any debris blocking full contact. 
On my previous build I rode once for about twenty minutes with the key not all the way in and that just caused it to burn out and melt (no other damage thankfully. lesson learned) so what happened here?  
I replaced the burned socket and tried again, with the same results.  
Ideas anyone? Thanks
```

---
## \#2 Posted by: Fraserrazor Posted at: 2019-02-09T19:01:36.939Z Reads: 99

```
Was the loop key an antispark xt90? Did it have a resistor connected on a short circuit band to prevent initial spark occurring?

I'm talking about the image below where the green marking indicates an antispark connector
![image|565x414](upload://75AqFAbXdU3kGptlIsBt5lBKQxM.jpg)
```

---
## \#3 Posted by: dareno Posted at: 2019-02-09T19:01:56.914Z Reads: 96

```
You using an xt90s anti spark?  lol this :point_up_2:
```

---
## \#4 Posted by: High-roller Posted at: 2019-02-09T19:04:09.993Z Reads: 92

```
Yes I am using an anti spark one.
Here's the loop set up, is this correct? It's what I did for my last build.
![IMG_20190209_210243|375x499](upload://cCRn2Spxo7Xnqkj0a0v0RvXLMY.jpeg)
```

---
## \#5 Posted by: ShutterShock Posted at: 2019-02-09T19:05:33.988Z Reads: 93

```
That looks right to me.  I had a friend who had a popping anti-spark too.  There's some possibility that the antispark could have just been a bad one

What brand is it?  I always get the Amass ones and have never heard one pop
```

---
## \#6 Posted by: Fraserrazor Posted at: 2019-02-09T19:05:43.972Z Reads: 91

```
Check there isn't a short in the anti spark which bypasses the resistor
```

---
## \#7 Posted by: High-roller Posted at: 2019-02-09T19:09:21.145Z Reads: 91

```
@ShutterShock I got them from hobbyking so they should be fine.
@Fraserrazor I didn't any damage on the key either. I tried both the one I made for this and the one for my other board, with the same result.
![15497393868344739573030856221241|666x499](upload://oPC3SAMwWhlFc9E4Bz3dq1JdmVm.jpeg)
```

---
## \#8 Posted by: ShutterShock Posted at: 2019-02-09T19:10:37.562Z Reads: 88

```
Ah okay.  Very odd.  I wonder if there's any chance the resistor is a bit loose inside?  Honestly weird
```

---
## \#9 Posted by: Fraserrazor Posted at: 2019-02-09T19:14:42.189Z Reads: 88

```
The only reasons for a spark occurring when using an anti spark connection is from a short between the anti-spark terminal and the circuit terminal or the resistor is blown/faulty but is still allowing current to flow or has made a spark gap.
```

---
## \#10 Posted by: Fraserrazor Posted at: 2019-02-09T19:15:53.023Z Reads: 88

```
what capacitors are you using in your vesc/esc?
```

---
## \#11 Posted by: High-roller Posted at: 2019-02-09T19:16:11.886Z Reads: 84

```
I don't think so. I just tried both keys in my other board and It powered up perfectly.
I did find this in another thread:
[![|45x45](https://www.electric-skateboard.builders/user_avatar/www.electric-skateboard.builders/deathcookies/45/144819_1.png)](https://www.electric-skateboard.builders/u/DeathCookies)

[DeathCookies](https://www.electric-skateboard.builders/u/DeathCookies)

[Apr '16](https://www.electric-skateboard.builders/t/xt90-s-loop-key-short-circuit/2383/29?u=high-roller)

Today I rechecked my wiring and did find the mistake… I just soldered it like the wiring you have Seen before. Exactly like the wiring diagramm and that was my mistake.

[![|479x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/2X/7/7e282727778eecae40ff5fbf95f60c1f66e747b0_1_479x500.PNG)
2677600ddb451bf7ea5cb112584e83df8ee9e82a.PNG555x579 5.43 KB
](https://www.electric-skateboard.builders/uploads/db1493/original/2X/7/7e282727778eecae40ff5fbf95f60c1f66e747b0.PNG)

In that wiring the polarity of the xt90-s loop key will be wrong! In the diagramm there is a Red positive cable to the left and the black negative on the right. But when we Look at the Battery cables they go the other way to the Esc… So i changed the polarity and blow my xt90-s.
Thanks for the Input! I really appreciate this forum :wink:
Here's my full wiring:
![15497398102111377008072528432844|375x499](upload://jWP0E4VjZgIyPEFeO0qrsSnqXdV.jpeg) 
@Fraserrazor they're minivescs from flipsky so 3x 220uF
```

---
## \#13 Posted by: High-roller Posted at: 2019-02-09T19:19:02.318Z Reads: 72

```
I haven't yet, that wasn't the problem here.
```

---
## \#14 Posted by: ShutterShock Posted at: 2019-02-09T19:19:03.328Z Reads: 73

```
BRO that wheel wtf lol that looks insane!

As far as I know, the loop key doesn't have polarity?
```

---
## \#15 Posted by: Fraserrazor Posted at: 2019-02-09T19:19:27.986Z Reads: 71

```
Yh sorry replied wrong person :sweat_smile:
```

---
## \#16 Posted by: Battosaii Posted at: 2019-02-09T19:19:56.603Z Reads: 69

```
You have positive and ground hooked up to the antispark plug. This happened to me once and and I blew 2 Focboxes. 

You may have damaged something. 

Loop key should be ground to ground or positive to positive. Never positive to negative.
```

---
## \#17 Posted by: High-roller Posted at: 2019-02-09T19:25:17.729Z Reads: 61

```
Damn. Alright, I'll switch it and report back, I really hope I got lucky, I don't want to have to replace a vesc at this late stage.
@ShutterShock interesting that you call it insane. Check out the build thread :wink:
```

---
## \#18 Posted by: rich Posted at: 2019-02-09T19:37:28.779Z Reads: 64

```
The "loop key" in the special charging diagram above cuts the serial connection for charging 2x 6s batteries with 2x 6s balance charger simultaneously. It has nothing to do with a normal loop key which would be between battery and vesc.

But maybe it still works this way with the XT90S, no idea tbh, the connection isn't wrong.

I have yellow XT90S and black XT90 (like in your picture) from hobbyking and I recognized that yellow on yellow fits perfect but the yellow XT90s female doesn't fit well into the black male XT90, it's very tight. I'm just thinking loud, maybe this is a problem, too.
```

---
## \#19 Posted by: dareno Posted at: 2019-02-09T19:44:02.437Z Reads: 58

```
Yeah shit dude you only cut the negative or positive.  Never both.  Amass only and if you got the hk then make sure its the amass.  They sell cheaper versions.
```

---
## \#20 Posted by: skatardude10 Posted at: 2019-02-09T19:46:20.216Z Reads: 58

```
Yup made that mistake ![20190203_143015|690x335](upload://xuJ3dkh9QpchRyoxl7RIUlpgXiI.jpeg)
```

---
## \#21 Posted by: dareno Posted at: 2019-02-09T19:47:11.680Z Reads: 57

```
I have a drawer full of my mistakes.  Its a fucking big drawer.
```

---
## \#22 Posted by: skatardude10 Posted at: 2019-02-09T19:48:09.764Z Reads: 55

```
😬🤯🤑

10char
```

---
## \#23 Posted by: High-roller Posted at: 2019-02-09T20:13:21.094Z Reads: 51

```
Guess I'll start my own collection too. 
_Mental note: put a big sign above my soldering station that says "check your effing polarity dumbass!"_
```

---
## \#24 Posted by: dareno Posted at: 2019-02-09T20:21:56.556Z Reads: 49

```
My friend I have wired a battery wrong.  Not wrong in the sense of a misplaced wire, I mean the xt90 round the wrong way.  Late night.  Plugged it in and boom!  Bms is toast.  Easy to do.  Shit when it happens.
```

---
## \#25 Posted by: High-roller Posted at: 2019-02-09T20:26:31.024Z Reads: 48

```
Very true.
Okay, I've resoldered the loop. The good news is:
![IMG_20190209_221807|375x499](upload://md5UhAAaSNTnPNL6WV1PsKPCY3c.jpeg) 

The bad news is:
![IMG_20190209_221824|666x500](upload://9mQDvGDmUn6C8PDojS0bMrFhtaq.jpeg) 
...and of course I don't have a STlink programming card in case I mess it up. I love technology 🙄
```

---
## \#26 Posted by: dareno Posted at: 2019-02-09T22:43:28.446Z Reads: 37

```
You won't its a simple process.  Just ID your vesc in the left window and update the latest from the right.  
If you have a simple vesc ie a focbox or tb or hk then choose 4.12.  The left window will display the options.  Then click on it and the right window will tell you what to update to.  Click and update away.  If it does not give you the option then the vesc does not have the bootloader installed and only then would you need the st link.  This is only my own experience based on my own fuck ups so take it as you will.
```

---

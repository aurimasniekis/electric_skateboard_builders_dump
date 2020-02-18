# VESC over_voltage error when braking

### Replies: 28 Views: 661

## \#1 Posted by: TheFluffiest Posted at: 2018-06-24T21:40:33.309Z Reads: 126

```
My vesc won't break at high speeds (15-20+mph), but does around 10 or less. It's running ackmaniac 3.10 firmware, but I doubt that's the problem. I hooked it up to the console and got over voltage errors when braking. I have a single drive 190kv setup with a 12s lipo setup. Max volts is set to 57v. 

I put Regen breaking at 1.5a, and it doesn't over volt anymore, but braking is almost non existent at that point. 

From what I've read, I don't see why a 12s setup would ever go over 57 volts unless braking downhill. But it happens when bench testing and no load, seemingly regardless of battery levels (tested between 4.2-3.8v per cell). 

Any ideas on how to fix this? Would adding capacitors help? I know they are used to negate voltage spikes. Battery wires aren't more than a 3-4 inches, so I don't think that would cause such huge voltage spikes. There aren't any coils either. My mini remote seems to be working fine, so I don't think it's the remote either. Thoughts?

BLDC
PPM with UART (mini remote and h10 Bluetooth for on the fly adjustments)
Motor Max: 60a
Motor min: -60a
Bat Max: 130a
Bat min (Regen): 1.5a
Max volts: 57v
Min volts: 8v (I will bump this up later for 12s)
Battery cutoff start: 42.8v
Battery cutoff end: 40v
```

---
## \#2 Posted by: Silverline Posted at: 2018-06-24T21:53:56.064Z Reads: 115

```
Do you use a BMS for discharging ?
```

---
## \#3 Posted by: Benjamin899 Posted at: 2018-06-24T21:57:23.985Z Reads: 112

```
Highspeed braking is mostly influenced by battery regen, the lower the value the stronger the braking force, yours is quite high
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-06-24T22:36:21.346Z Reads: 101

```
No I don't. I use a balance charger for charging though
```

---
## \#5 Posted by: TheFluffiest Posted at: 2018-06-24T22:37:08.072Z Reads: 97

```
Really? I had the brake all the way on and it barely did anything. Can you explain more?
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-06-24T22:44:39.442Z Reads: 91

```
i had the same problem when i first got my vesc. Well look at it that way. Braking with the motor generates amp flow back to the vesc, but the capacitors are not endless, so where does all the current go....to the battery it goes, so the more the vesc is allowed to feed back into the battery the better it can brake...to an extend. What battery do you have? Type and capacity?
```

---
## \#7 Posted by: TheFluffiest Posted at: 2018-06-24T23:04:49.491Z Reads: 89

```
I have three 4s 5000mah lipo batteries wired in series to create a 12s battery. 

So you are saying that if make battery Regen a positive number it could fix it?
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-06-24T23:07:02.433Z Reads: 88

```
no. regen stays negative. what is the max charge current the battery can take? i guess 2C?
```

---
## \#9 Posted by: TheFluffiest Posted at: 2018-06-24T23:07:38.077Z Reads: 86

```
Yes, as far as I know.
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-06-24T23:12:35.306Z Reads: 82

```
Since you have a 5Ah Battery with 2C charge current max you get 10 amps max charge current. And you can add a bit extra so around 13-14 amps regen. So -13/-14 amps in setup.  It gets confusing here. Some people use the right terminoligy, like in math and others describe the number in context...confusing.
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-06-24T23:21:46.035Z Reads: 79

```
just remember single drive will always be weaker on the brakes, depending on belt, driver weight and decline/incline
```

---
## \#12 Posted by: Ackmaniac Posted at: 2018-06-24T23:34:35.953Z Reads: 74

```
Guess you have a BMS in the discharge cycle. Kick it out and only use it for charging with a power supply.
```

---
## \#13 Posted by: TheFluffiest Posted at: 2018-06-24T23:48:46.249Z Reads: 74

```
I don't have a BMS at all. I use a balance charger seperate from the board to charge the batteries, but nothing regulating discharge.
```

---
## \#14 Posted by: TheFluffiest Posted at: 2018-06-24T23:51:16.778Z Reads: 72

```
If I put it any lower than -1.5a, I get the over voltage error. I got confused. So if I go -2 or further the error is triggered.

I'm planning on upgrading to dual asap, this is my second board because the first one was destroyed. I've definitely seen the light :joy:
```

---
## \#15 Posted by: Benjamin899 Posted at: 2018-06-25T00:02:09.390Z Reads: 71

```
it would be best if you can post screenshots of your settings
```

---
## \#16 Posted by: TheFluffiest Posted at: 2018-06-25T00:13:07.703Z Reads: 69

```
Putting it to 10a seems to have solved it. I'm not entirely sure what the difference between now and then was, but I will go for a quick ride and see if it works under load. If it doesn't work, I will post the screenshots.
```

---
## \#17 Posted by: Benjamin899 Posted at: 2018-06-25T00:13:43.243Z Reads: 67

```
wowowowo wait what
```

---
## \#18 Posted by: Benjamin899 Posted at: 2018-06-25T00:15:28.936Z Reads: 68

```
you set battery regen to 10a? or -10a?
```

---
## \#19 Posted by: TheFluffiest Posted at: 2018-06-25T00:18:09.235Z Reads: 69

```
-10a sorry. Yeah it works now, brakes about as good as they can be with a single motor setup. Very strange indeed.
```

---
## \#20 Posted by: TheFluffiest Posted at: 2018-06-25T00:38:33.882Z Reads: 70

```
Nevermind, it's doing it again. These are my settings.

Motor Current
![Motor%20current|690x373](upload://8pdH3lCtZBMq0lJEYFNVNuACVUC.png)

Motor Advanced
![Motor%20advanced|690x387](upload://3r30CGuF0OGAmVWG8dAnKiTaoL9.png)

Motor General
![Motor%20general|690x374](upload://yXeaLUei2n7M1t3OyPed9E4YBuM.png)

PPM
![ppm|690x375](upload://mkb65Xy5STkKwMzlwZbqXN5JKvb.png)
```

---
## \#21 Posted by: Ackmaniac Posted at: 2018-06-25T00:40:34.789Z Reads: 68

```
Check for loose wire.
```

---
## \#22 Posted by: TheFluffiest Posted at: 2018-06-25T01:15:51.585Z Reads: 64

```
Hmm. Hadn't thought of that. I will when I get back home
```

---
## \#23 Posted by: itsmikeholland Posted at: 2018-06-25T02:04:04.761Z Reads: 64

```
dont get discouraged with a single drive! I ride a balance-discharge 10s 149kv single drive with an Ollin Vesc for 3 years now and take it up and down steep hills daily without problem. Only "issue" I have is a mental thing where I'm used to releasing the trigger when I'm coasting, and I sometimes accidentally do this when going down hills :joy: otherwise I've had no issues except for when the wheel cant grip the ground
```

---
## \#24 Posted by: lrdesigns Posted at: 2018-06-25T02:10:17.599Z Reads: 62

```
Check the caps are connected properly. Might have broken from vibration.
```

---
## \#25 Posted by: TheFluffiest Posted at: 2018-06-25T03:54:24.163Z Reads: 59

```
@Ackmaniac was right. Soldered the hell out of multiple leads, checked everything, all is well again. Thanks everyone!
```

---
## \#26 Posted by: TheFluffiest Posted at: 2018-06-25T04:55:19.552Z Reads: 54

```
I definitely have love for single drives! I just love duals too 😂😂 sounds like a great setup!
```

---
## \#27 Posted by: Benjamin899 Posted at: 2018-06-25T12:04:38.177Z Reads: 53

```
Battery Current 90A is too much, also motor current is a tad much.
Focbox and others like it can take 50a continuous but to be safe i wouldn't set it higher than 40a, but thats my opinion. But 90a is something i haven't seen so far, except normal esc
```

---
## \#28 Posted by: Jordan12 Posted at: 2019-07-10T17:57:22.694Z Reads: 16

```
I’m having this problem, which wires should I check. All the wires on my vesc appear fine
```

---

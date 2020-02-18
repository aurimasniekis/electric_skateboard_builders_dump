# Reccomended Batteries

### Replies: 29 Views: 1230

## \#1 Posted by: nikolas Posted at: 2017-08-14T01:14:48.780Z Reads: 114

```
@darkkevind 

Hi! After about a month of riding on my new board, I had many people telling me that I should upgrade my batteries. However I do not have any knowledge on batteries.

I am currently running two 5000 mah 3s1p 20c lipo batteries. I want to understand what these numbers mean in terms of distance or how fast the board will go. I want to increase my speed while maintaining my distance. Please let me know if two 5000 mah 6s 25 c lipos connected in series would work, or if I need more c rating to up my speed etc.


Here are my parts:

6355 190kv motor from diyelectricskateboard (diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/)

TORQUE ESC VESC ® BLDC Electronic Speed Controller diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

TorqueBoards 2.4ghz Nano Remote Controlle diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/





Thank you in advance!
```

---
## \#2 Posted by: willpark16 Posted at: 2017-08-14T01:18:07.241Z Reads: 106

```
Simple add more lipos in series or change to li ion cells
```

---
## \#3 Posted by: darkkevind Posted at: 2017-08-14T01:21:11.862Z Reads: 106

```
Yes, what @willpark16 said. You need more cells in series to up the voltage which will in turn up your top speed.

However, you must check your motor can handle the extra voltage by checking the specs. 12s (12 x 4.2v = 50.4) may be too much for it.
```

---
## \#4 Posted by: nikolas Posted at: 2017-08-14T01:37:43.985Z Reads: 93

```
Would you reccomend li-ion or lipo?
```

---
## \#5 Posted by: nikolas Posted at: 2017-08-14T01:39:14.622Z Reads: 88

```
Here are my motors max:
Max Power: 2500 Watts
Max Amps: 80 Amps
Max Volts: 12S

Could you tell me if a 5000 mah 6s 25 c lipo would work. Also what does c rating and mah do. Sorry for all the questions.
```

---
## \#6 Posted by: darkkevind Posted at: 2017-08-14T01:40:21.547Z Reads: 83

```
I'd go with Li-po for cost, and AMP output if you're happy charging the batteries individually. You could get a BMS for them if  you want to charge them all together.

I'd go for Li-ion for longevity, safety and ease of charging (through just a power brick by using a BMS). They're quite a bit more expensive than Li-po's though!
```

---
## \#7 Posted by: nikolas Posted at: 2017-08-14T01:42:19.797Z Reads: 77

```
Ok, I will stick to lipo. As for the max for the motor will the other specs do?

Here are my motors max:
Max Power: 2500 Watts
Max Amps: 80 Amps
Max Volts: 12S\

In addition I am using a parralel charger for my lipos
```

---
## \#8 Posted by: darkkevind Posted at: 2017-08-14T01:53:49.347Z Reads: 70

```
Yes, your motor is fine for 12s
```

---
## \#9 Posted by: nikolas Posted at: 2017-08-14T01:57:58.512Z Reads: 70

```
OK, by the way, thank you for all your help on this topic and all my other topics.

Also, what c rating and mah should I get, and what do they mean.
```

---
## \#10 Posted by: willpark16 Posted at: 2017-08-14T02:19:11.476Z Reads: 65

```
Li ion my friends
```

---
## \#11 Posted by: nikolas Posted at: 2017-08-14T02:21:36.716Z Reads: 62

```
I think that in my case, a lipo is better, I have all wires needed and a lipo charger already.
```

---
## \#12 Posted by: willpark16 Posted at: 2017-08-14T02:27:42.179Z Reads: 61

```
Go for it then
```

---
## \#13 Posted by: nikolas Posted at: 2017-08-14T02:30:20.638Z Reads: 60

```
Yes, I am just confused with the c rating and mah.
```

---
## \#14 Posted by: nikolas Posted at: 2017-08-14T02:40:33.049Z Reads: 58

```
I found this on hobbyking https://hobbyking.com/en_us/zippy-compact-5000mah-6s-25c-lipo-pack.html, it seemed good. Is this ok, if so what kind of cables are those red and black ones, they look like bullet connectors. Thank you for your help.
```

---
## \#15 Posted by: jammin Posted at: 2017-08-14T02:46:18.722Z Reads: 57

```
It says they are 5.5 bullet connectors on the description page. I've read (but not seen / experienced) issues with 190kv and 12s (eRPM errors only at top speed). I'm running 10s and 190kv with zero issues.
```

---
## \#16 Posted by: nikolas Posted at: 2017-08-14T04:04:33.020Z Reads: 49

```
How fast are you able to go on your current setup, also what is your mah and c rating.
```

---
## \#17 Posted by: jammin Posted at: 2017-08-14T04:18:44.623Z Reads: 53

```
I'm running 10s1p with 5000mAh, 20c for each battery (5s). I probably should've gone with a higher C rating, but I live in a flat area and I weigh 160 lbs.

I've been able to get my board to 20+ mph pretty easily (not full throttle) and I'm using Kegels with 16/36 gearing. My build:
https://www.electric-skateboard.builders/t/first-time-build-10s-190kv-vesc-superglider/27366
```

---
## \#18 Posted by: nikolas Posted at: 2017-08-14T04:22:02.983Z Reads: 47

```
What does the c rating do, will it affect speed or distance?
```

---
## \#19 Posted by: jammin Posted at: 2017-08-14T04:22:57.327Z Reads: 46

```
tldr it's the max current you can pull out of your batteries. There's a bunch of threads on this forum about it, I'd look it up
```

---
## \#20 Posted by: nikolas Posted at: 2017-08-14T04:23:59.467Z Reads: 47

```
OK, and i'm guessing that your batteries have 5.5 bullet plugs? If so, which connector are you using to have them in series.
```

---
## \#21 Posted by: jammin Posted at: 2017-08-14T04:25:24.065Z Reads: 43

```
4mm bullets. I replaced them with XT90 (overkill) and made my own XT90 series connector with a XT90s switch.
```

---
## \#22 Posted by: nikolas Posted at: 2017-08-14T04:27:26.915Z Reads: 42

```
So do you have 5.5 mm bullet connectors or the 4 mm bullet connectors? Thanks for all the help so far
```

---
## \#23 Posted by: jammin Posted at: 2017-08-14T04:27:58.576Z Reads: 40

```
4mm bullets! https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html
```

---
## \#24 Posted by: nikolas Posted at: 2017-08-14T04:28:56.869Z Reads: 42

```
Ohhhhhh OK sorry, I am new to electric boards.
```

---
## \#25 Posted by: jammin Posted at: 2017-08-14T04:34:35.920Z Reads: 42

```
no prob, are you planning on staying with 6s or do you wanna go bigger (10/12s)? Also you should spend some more time looking up RC / electronics basics before you start building ;)
```

---
## \#27 Posted by: nikolas Posted at: 2017-08-14T04:37:37.225Z Reads: 39

```
I think I am going to go with two 4000 mah 5s 30c lipo batteries connected in series. Also could you explain what the batteries c rating does in terms of speed, distance, safety or anything else it may affect. 

Thanks!
```

---
## \#28 Posted by: jammin Posted at: 2017-08-14T04:41:36.461Z Reads: 36

```
again there's info on that already on this forum and beyond. Just do a google search, I'm feeling like a broken record! :sweat_smile:

If you're feeling lazy it's how much the battery will support a continuous current draw. In your example, you'll have 4000mah * 30C -> 4 * 30 -> 120A continuous, which should be fine.
```

---
## \#29 Posted by: nikolas Posted at: 2017-08-14T04:42:53.588Z Reads: 37

```
Ok, thank you for your help!
```

---
## \#30 Posted by: Proxy Posted at: 2017-12-03T05:17:21.680Z Reads: 14

```

Poor nikolas just wants to know what the c rating does. I respect your patients. Me on the other hand feel like pulling my hair out because of this electronic stuff.
```

---

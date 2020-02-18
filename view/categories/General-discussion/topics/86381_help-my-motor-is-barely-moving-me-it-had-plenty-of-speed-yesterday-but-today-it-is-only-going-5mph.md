# HELP. My motor is barely moving me. It had plenty of speed yesterday but today it is only going ~5mph

### Replies: 65 Views: 819

## \#1 Posted by: buildityourself Posted at: 2019-03-07T01:29:27.278Z Reads: 240

```
I have a 10s5p battery with a 6374 192kv motor. I took it out last night and it went plenty fast. Took it inside and looked at the vesc software and I am guessing it somehow reset everything. My motor settings are max: 70A, min: -60A, Battery max is 40A and min is -12A. The voltages are 34, and 31. Ive spent all day trying to figure this out and can't.

This is the remote settings: ![2019-03-06|690x387](upload://wc5VJLaUaxvElpeM3eDSkzl0jtv.jpeg)
```

---
## \#2 Posted by: rusins Posted at: 2019-03-07T01:54:14.580Z Reads: 230

```
Is your battery charged? You can check the voltage in Vesc tool:
https://www.electric-skateboard.builders/t/how-to-use-the-vesc-tool-to-read-voltage/86326/2?u=rusins
```

---
## \#3 Posted by: KaramQ Posted at: 2019-03-07T01:59:01.194Z Reads: 226

```
Check your wire connectors, same thing happened to me
```

---
## \#4 Posted by: buildityourself Posted at: 2019-03-07T02:09:06.849Z Reads: 228

```
Which wires?
```

---
## \#5 Posted by: buildityourself Posted at: 2019-03-07T02:12:22.937Z Reads: 228

```
woah thats cool. Im getting 30v through it and this is the current: ![2019-03-06%20(1)|690x387](upload://tRVBgK0Vlm9E9r3QzOgTe98Xmfk.png) 

does this look normal?
```

---
## \#6 Posted by: rusins Posted at: 2019-03-07T02:29:37.868Z Reads: 213

```
Well if your cutoff voltage is 31V, and you're getting 30.9V from your battery, then it seems like you're out of power :smiley:

Charge up your battery, it should be 42.0V when fully charged :slight_smile:
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-03-07T02:43:54.030Z Reads: 208

```
Get ready to wait... That 2a charger takes quite a second to charge it fully
```

---
## \#8 Posted by: buildityourself Posted at: 2019-03-07T04:32:10.228Z Reads: 195

```
Oh maybe thats why, I charged it for about half an hour just to test if it was the charger and it didn't do anything. But this brings me to another conclusion, my LED always states that my battery is at 100%
```

---
## \#9 Posted by: dareno Posted at: 2019-03-07T04:38:00.679Z Reads: 192

```
Your led on the charger or your battery meter?
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-03-07T04:43:20.977Z Reads: 192

```
Yeah you have the same issue I did. You got the wrong lcd display / you have it programmed wrong

Not sure which one you have, and if I did, I wouldn't be much help anyways. What I did was swap the reader over to volts and then just got used to reading it as 42v is topped off, and 30 is lowest I would ever go
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-03-07T04:49:04.077Z Reads: 187

```
Plug the charger in, let it go from red to solid green and you're all set

Make sure the charger isnt covered, they get kinda hot
```

---
## \#12 Posted by: buildityourself Posted at: 2019-03-07T05:22:20.143Z Reads: 178

```
Battery meter, attached to my board. It reads 40 volts all the time
```

---
## \#13 Posted by: dareno Posted at: 2019-03-07T05:27:01.557Z Reads: 170

```
On the back is a micro switch.  Press it and it will allow you to set the series count of your battery.  ie 10s.  Then you can see where you are.
```

---
## \#14 Posted by: buildityourself Posted at: 2019-03-07T05:39:46.743Z Reads: 163

```
The tiny black button? I pressed it, held it, pressed it while holding the screen button but nothing happened
```

---
## \#15 Posted by: dareno Posted at: 2019-03-07T05:48:12.444Z Reads: 159

```
turn off the battery then hold down the black switch while you turn the battery back on.  It should flash and allow you to scroll using the front buttons to set it to 10s.
```

---
## \#16 Posted by: buildityourself Posted at: 2019-03-07T05:53:48.135Z Reads: 155

```
Okay it looks like I pick a letter between L, F and P and then select a 2 digit number. I have a 10s5p battery. I was not sure what the letters meant but I put 10 in
```

---
## \#17 Posted by: dareno Posted at: 2019-03-07T05:55:34.529Z Reads: 157

```
Choose L because that stands for lithium then select 10s

good to go brother!!
```

---
## \#18 Posted by: buildityourself Posted at: 2019-03-07T06:05:12.524Z Reads: 154

```
Thanks a ton man! It showed 2%, then 100% and then 99% and now it still says 100% but i'll keep on fiddling with it to try and figure it out. I really appreciate it though. I hope my battery was just out and that is why I was having a really weak motor originally
```

---
## \#19 Posted by: dareno Posted at: 2019-03-07T06:08:57.460Z Reads: 148

```
At 30v it should be reading the 2% mark which is why the board was not moving.  Get it set and hopefully everything is hunky dory.  Remember the 10s should read 42v on max charge.
Don't let the battery get that low again either.  If it gets too low you will struggle to charge it with a 2a charger and it can get damaged.  Good luck!
```

---
## \#20 Posted by: buildityourself Posted at: 2019-03-07T06:20:24.920Z Reads: 147

```
Noted!! Thanks so much
```

---
## \#21 Posted by: marsrover001 Posted at: 2019-03-07T11:41:30.134Z Reads: 136

```
Adding to this. When I let my battery get that low, my BMS decided it's not worth charging. So I would plug my charger in, it turns green instantly, and the pack stayed "dead".

Ended up having to bypass the bms and charge direct into the discharge lead for an hour before swapping back to using the bms to balance out and finish the charge. Checked the specsheet for my bms and sure enough, this cheap chinese bit of junk won't charge my battery if the cells drop below 3.3v (was at 3v, yea I know but I wasn't about to push home)

Everything is fine now, but if your charger light isn't turning red, try bypassing the bms for a bit.
```

---
## \#22 Posted by: rusins Posted at: 2019-03-07T16:10:54.764Z Reads: 123

```
What do you guys recommend then for complete cutoff voltage? Looking at graphs of 30Q discharge it would seem that 3.1V would be a good point to stop. (Many on this forum use 3.2V)
```

---
## \#23 Posted by: dareno Posted at: 2019-03-07T17:52:30.162Z Reads: 113

```
Thats a preference thing.  the higher the safer and better for the battery but how often do you run your board till it stops?  I don't personally.  Battery anxiety is a real thing. lol
```

---
## \#24 Posted by: Sn4pz Posted at: 2019-03-07T18:04:23.836Z Reads: 113

```
[quote="dareno, post:23, topic:86381"]
I don’t personally. Battery anxiety is a real thing.
[/quote]


Dont personally what? Either you mean the battery anxiety = range anxiety, or you mean the overall health of a cell :thinking:
```

---
## \#25 Posted by: dareno Posted at: 2019-03-07T18:17:25.020Z Reads: 107

```
[quote="dareno, post:23, topic:86381"]
how often do you run your board till it stops?
[/quote]

Was I texting in turkish again?  I do that sometimes
```

---
## \#26 Posted by: buildityourself Posted at: 2019-03-07T20:12:47.898Z Reads: 103

```
Damn. I think this is happening to me. Could you speak a little more about how you bypassed the bms? Should I disconnect the bms all together and then charge it and then reconnect the bms?
```

---
## \#27 Posted by: marsrover001 Posted at: 2019-03-07T21:21:53.123Z Reads: 102

```
So I run charge only bms. (Hence the 2 output options) Since you have charge/discharge on the same connector I would just unplug the battery to bms connection and send the charger power direct into the battery. Bms would be disconnected at this time.
```

---
## \#28 Posted by: buildityourself Posted at: 2019-03-08T01:22:14.422Z Reads: 101

```
So this is my BMS, how would you use these wires to bypass it? ![IMG_4209|375x500](upload://qiTMcLARjkoHFPVnzYhxwGnjwM0.jpeg) ![IMG_4210|666x500](upload://w3XFgqqXZBhmohwmNUqNnqsmjD8.jpeg) ![IMG_4211|375x500](upload://vyzGj9MLldQnb1VzgPjeyNLAdun.jpeg)
```

---
## \#29 Posted by: rusins Posted at: 2019-03-08T01:38:56.271Z Reads: 94

```
Looks like the red (assuming positive) wire of the battery is connected directly to the cells, so it's the thick black wire (assuming negative) that is going through the BMS. You'd have to solder the 2 thick black wires together temporarily to charge your battery, but I'm not sure if it's safe to leave everything else in place while you do that. Someone more experienced with BMSs and this scenario should step in and guide you. (i.e., don't take my word for it, wait for someone else to chime in as well.)
```

---
## \#30 Posted by: buildityourself Posted at: 2019-03-08T01:57:21.145Z Reads: 94

```
So in that last picture it is actually after I have soldered the thick wire. The thick wire is the boards power, where the thin wire is the charging cable. I disconnected both of those from the bms and connected them directly to the other side and it seemed to work but now the charger is showing green as if it is fully charged again
```

---
## \#31 Posted by: buildityourself Posted at: 2019-03-08T03:12:44.406Z Reads: 87

```
What did you have to fix exactly?
```

---
## \#32 Posted by: KaramQ Posted at: 2019-03-08T03:13:34.919Z Reads: 88

```
It was just my phase wires but you have a battery issue, and I have absolutely no knowledge on batteries
```

---
## \#33 Posted by: buildityourself Posted at: 2019-03-08T03:17:38.348Z Reads: 87

```
I am still not sure what issue I am having. Was it the soldering of your phase wires or was it something else? I soldered my phase wires to the vesc wires instead of getting connectors.
```

---
## \#34 Posted by: KaramQ Posted at: 2019-03-08T03:19:14.420Z Reads: 84

```
That might be your problem, I really have no clue though
```

---
## \#35 Posted by: buildityourself Posted at: 2019-03-08T03:22:45.940Z Reads: 84

```
What was wrong with your phase wires?
```

---
## \#36 Posted by: KaramQ Posted at: 2019-03-08T03:27:49.006Z Reads: 81

```
One was disconnected
```

---
## \#37 Posted by: buildityourself Posted at: 2019-03-08T03:57:41.410Z Reads: 82

```
Sorry to keep harping on this but was it 100% disconnected or just partially?
```

---
## \#38 Posted by: KaramQ Posted at: 2019-03-08T04:09:41.918Z Reads: 81

```
Partially attached
```

---
## \#39 Posted by: buildityourself Posted at: 2019-03-08T06:27:39.507Z Reads: 80

```
So when I get on the board and try it, it says 100% before I accelerate, but once I begin the battery percentage continuously goes down to ~5% within about 5-10 seconds. Does this sound like the same battery problem to you?
```

---
## \#40 Posted by: dareno Posted at: 2019-03-08T06:30:43.054Z Reads: 77

```
Thought I'd got rid of you!!!!   How long was it on charge for? Did the battery indicator rise to 100 Did the charge light go from red to green?  Does the board work?  Lolz
```

---
## \#41 Posted by: buildityourself Posted at: 2019-03-08T08:38:05.594Z Reads: 71

```
Haha i wish you would have. At least 2 hours. The board still does not ride as normal. The light has turned green even though the problem continues. I have tried to bypass the BMS and still nothing. Times are tough
```

---
## \#42 Posted by: dareno Posted at: 2019-03-08T09:35:44.953Z Reads: 66

```
I'm doing my best here my friend.  You could have some out of whack cells.  I would leave it on charge for a few more hours or overnight.  Do this outside of your house.  Can't be too careful but with a 2a charger when you leave it on it will slowly balance the cells via the bms even if its green.
I think you over discharged it.  What is the battery?  25r 30q?
```

---
## \#43 Posted by: pat.speed Posted at: 2019-03-08T12:16:59.901Z Reads: 65

```
Looks like lg hg2 the 3000mah ones, judging by the brown wrap on em.

@buildityourself Do you have a voltage meter? If yes can you check the voltage of the battery leads going to the bms. The the lead from the bms to the discharge plug. Also check each cell voltage.
```

---
## \#44 Posted by: buildityourself Posted at: 2019-03-08T19:42:34.583Z Reads: 62

```
The battery and the discharge plug both say 41.7. Do you think it could be a wiring problem somewhere else down the line?
```

---
## \#45 Posted by: buildityourself Posted at: 2019-03-08T19:43:45.931Z Reads: 62

```
So i charged it through the night last night. I’m going to try and resolder some wires where I may have done a poor job and see what happens
```

---
## \#46 Posted by: dareno Posted at: 2019-03-08T20:05:57.834Z Reads: 56

```
Now i would get a meter and check the overall voltage of the pack.
```

---
## \#47 Posted by: Sn4pz Posted at: 2019-03-08T20:07:21.319Z Reads: 60

```
To clarify

The battery was balanced and  then ran down to 40v when I sent it, not sure why it would be behaving like this 😱
```

---
## \#48 Posted by: dareno Posted at: 2019-03-08T20:20:30.634Z Reads: 59

```
Ah it all becomes clear.  @Sn4pz sold you a dodgy battery
Hit the solution button our work here is done  :stuck_out_tongue_winking_eye:
```

---
## \#49 Posted by: Sn4pz Posted at: 2019-03-08T20:38:42.740Z Reads: 56

```
No I promise 😭😭😂

If I were to ever sell a battery again, it would be good to prove that everything is in working condition. Is there a way to test a pack without opening the wrapping?
```

---
## \#50 Posted by: buildityourself Posted at: 2019-03-08T21:16:42.218Z Reads: 57

```
The voltage looks fine, its at 41.7. I still don’t know if it is the battery that is the problem.
```

---
## \#51 Posted by: buildityourself Posted at: 2019-03-08T21:17:02.156Z Reads: 56

```
It says 41.7 volts
```

---
## \#52 Posted by: dareno Posted at: 2019-03-08T21:21:34.345Z Reads: 57

```
More or less there then.  You could check the p groups but thats not enough of a drop to really worry.   Put it back together and have a ride.  Check the voltage against the meter when you get back.  Did you get the meter working?
God i hate that bloody blue screen that tells you off for replying too many times.
```

---
## \#53 Posted by: Sn4pz Posted at: 2019-03-08T21:23:43.383Z Reads: 55

```
I know flipsky VESCs have had issues with reading voltages, what brand of VESC do you have?

I think i remember you talking about having a TB VESC, which of the (probably) hundreds if not thousand units sold, hasnt had a track record of reading voltages incorrectly... :thinking:

I have to get out of my habit of using commas and ellipses ;-; sorry for all the post-post editing, but I feel like it should be readable xd
```

---
## \#54 Posted by: dareno Posted at: 2019-03-08T21:27:58.140Z Reads: 58

```
You can extremely carefully check the voltage with a meter at the xt connector. 
 
_Disclaimer_
I have killed 2 multi meters doing this so now I do this.

Best to have a male pigtail connected to a meter and then plug it in. I have a set of leads with crocodile clips soldered on and after I clip them to the pigtail I insulate with electrical tape to be safe.
```

---
## \#55 Posted by: buildityourself Posted at: 2019-03-08T22:22:21.806Z Reads: 55

```
So i do have a flipsky and the voltage reading is accurate. I’m starting to think its my shitty soldering skill that did me in. I’m going to resolder and test it when I get home
```

---
## \#56 Posted by: buildityourself Posted at: 2019-03-08T22:26:48.602Z Reads: 55

```
Oh whoops, i already tested the voltage there and it looked good and luckily didn’t screw up the multimeter 🤔  I don’t know why the battery gauge acts really strange when riding though, it just rapidly lowers the battery percentage
```

---
## \#57 Posted by: dareno Posted at: 2019-03-08T22:36:19.846Z Reads: 55

```
Just got to be careful of arcing.  Sounds like you have a faulty meter.  I've got one that flashes between volts and percentage.  No idea why.
```

---
## \#58 Posted by: buildityourself Posted at: 2019-03-08T22:58:06.533Z Reads: 55

```
I hope so. Yeah thats weird, yours sounds like it senses the button being pressed nonstop.
```

---
## \#59 Posted by: buildityourself Posted at: 2019-03-10T06:39:47.605Z Reads: 54

```
@dareno @Sn4pz Sorry to waste everybody's time and energy but I found the solution... and it was a really stupid mistake. I think the biggest factor was the fact that my enclosure did not allow the XT90 loop key to fit all the way together. After a long test the loopkey smoked and smelled so I looked it up and it just needed to be fully inserted to get the full power going. I feel dumb. But happy. But dumb.
```

---
## \#60 Posted by: dareno Posted at: 2019-03-10T06:42:51.014Z Reads: 56

```
That is the best outcome of any issue.  Most of mine are down my own silliness.  Cool man  Pleased for you.  You can ask a mod to shut it down now if you want to keep things tidy.
```

---
## \#61 Posted by: TowerCrisis Posted at: 2019-03-10T15:49:24.147Z Reads: 56

```
That's really interesting, was it an antispark xt90? That would explain the low speed, but I would have expected it to smoke up much faster. I've definitely set them on fire before.
```

---
## \#62 Posted by: buildityourself Posted at: 2019-03-11T19:56:59.268Z Reads: 51

```
Yep it was. I guess my test runs were too short to tell but then after changing a bunch of things and testing it another 50 times i got frustrated and pulled the trigger and let it run for ~30 seconds and it smoked and STANK
```

---
## \#63 Posted by: AMek Posted at: 2019-05-17T07:43:42.721Z Reads: 41

```
Hey man can I get a parts list with links if possible for your build, also can you tell me if the board holding up?
```

---
## \#64 Posted by: buildityourself Posted at: 2019-05-20T23:00:57.876Z Reads: 31

```
Hey, I will look for the same parts if i can even find them but currently having some vesc (probably DRV chip) issues and ive had a pretty serious issue with connecting my small gear to my motor. If you can wait, I plan on working thoroughly on testing things and bettering the design (while keeping it cheap). Once it works consistently I'll post everything
```

---
## \#65 Posted by: buildityourself Posted at: 2019-06-20T23:27:15.725Z Reads: 18

```
Hey, I got my board back to working condition. Did you still want that part list?
```

---

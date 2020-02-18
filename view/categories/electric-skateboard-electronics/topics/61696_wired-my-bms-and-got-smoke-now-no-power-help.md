# Wired my Bms and got smoke, now no power. Help

### Replies: 28 Views: 963

## \#1 Posted by: J95hicks Posted at: 2018-07-12T21:33:26.069Z Reads: 170

```
Edit 2.... So i wired everything up according to the info given, But i mightve screwed up... I checked all my balance wires once they were connected to the battery, but before wiring the bms up. i checked each balance and read 3.875V +/- .001V increase to a final 46.40V(12s). As i was connecting, i saw smoke come off the bms(very little but i was watching for in just in case) i immediately disconnected bms. I realized iconnected my pos/neg in the Wrong order and i think that mightve caused smoke but would this cause my bms to short or something?? and if so is it a lost cause now? nothing looks burnt or wrong, still shiny new.... Also extra info, i have bulit in battery capacity indicator. When i connect bms without the balance wires connected to bms, my indicator flashes and turns off. When i have the balance wires connected i get nothing and no power thru. Can anyone help

Edit 1** As per the advice given(loop key moved bt P-and Xt90 Neg), does this look correct? ![20180713_104957|374x500](upload://xGhCASz1rWYIjtUMYcLoG4oGTDj.jpg)
```

---
## \#2 Posted by: rojitor Posted at: 2018-07-12T21:52:06.048Z Reads: 157

```
![IMG_20180712_234934163264426793093749|666x500](upload://ws2FMnp6Gx2eKzYIoNZkO3bAGkJ.jpg)
That's not so weird. Look at my bms. I guess the purpose for several wires is to distribute the power among the shunts and fets.
```

---
## \#3 Posted by: J95hicks Posted at: 2018-07-12T22:15:39.084Z Reads: 148

```
Soo, how would i wire this? I thought itd be more clear, but im seeing extra of some terminal and none of the other like C
```

---
## \#4 Posted by: rojitor Posted at: 2018-07-12T22:21:48.228Z Reads: 150

```
Just solder the wires between the cells as usual. How many parallel are you doing? If it's 4p you got there 3 spots.
C (charge) does not need several wires. Only P and B
```

---
## \#5 Posted by: J95hicks Posted at: 2018-07-12T22:47:39.676Z Reads: 143

```
Well im using the NESE modules to avoid welding and soldering. Theyre 8P.. i can solder if i must...but im not asking about where the balance wires go.. its about the leads and charging connection. So i just dont use 4 of the leads, 2black and 2yellow un used. And do i just place my charging port off of the P-?
```

---
## \#6 Posted by: rojitor Posted at: 2018-07-12T22:57:13.347Z Reads: 138

```
I am not familiar with the nese method.
I guess It is ok if you just solder the 3 wires to a thicker wire and use It as usual.
C- is the charging negative you take the positive from main positive
b- goes to main negative
P- goes to discharge negative and you take the positive from the main positive.
Connect the balance wires carefully and you are good to go.
```

---
## \#7 Posted by: J95hicks Posted at: 2018-07-12T23:18:52.165Z Reads: 129

```
I do not have a C- on mine. Thats my issue. Iether its not there or i cant find it. Also, the 3 leads are already 10awg, i dont think i want to solder to a thicker wire
```

---
## \#8 Posted by: rojitor Posted at: 2018-07-12T23:51:03.620Z Reads: 122

```
No C-???? That's not possible. You DO NOT have hvc without It. If C- is not present one of the P- has to do that job. Ask the seller for a diagram and ask particulary about the C-
About the 10awg no problem...solder to another 10awg
```

---
## \#9 Posted by: J95hicks Posted at: 2018-07-12T23:58:35.170Z Reads: 121

```
Okay thank you, i thought i was crazy. That is exactly my issue, i can not identify it. I will ask the seller
```

---
## \#10 Posted by: J95hicks Posted at: 2018-07-13T03:06:48.904Z Reads: 111

```
So i messaged the seller and they said it does not have a C-? How is this possible?
```

---
## \#11 Posted by: DeathByBacon Posted at: 2018-07-13T03:28:44.673Z Reads: 104

```
Use one of the P- as your C-
```

---
## \#12 Posted by: rich Posted at: 2018-07-13T08:31:33.325Z Reads: 101

```
Please don't connect anything before you fully understand how batteries and BMS work. All the needed information is in the link of your OP. Discharge/charge (-) is same port, there is no C-.

There are different BMS out there, some have 
P- and C- (discharge/charge different ports)
P- (discharge/charge same ports)
I also have BMS with P- and C- but discharge/charge is both connected to C-

Also there are BMS which have B- as first cable of the balance leads and some start with B1+.

This is the reason why it's not a good idea to copy a wiring diagram of someone else, too many differences.

Just a short story, once I helped a member because he didn't understand BMS at all. I PM'd him a wiring diagram how he should connect his complete electronics including BMS. Well the next day he wrote me that after connecting he fell asleep and woke up in the night with smoke in the room. The BMS was burnt black and sizzling hot. He claimed me that my wiring diagram was wrong. A couple of PM's later he asked me if it is really important to connect the balance leads in correct order. After checking he found out that his balance wires were connected in the wrong order WTF! 

What a lucky guy that he woke up! I write this story as reminder that batteries and BMS are really dangerous if they are connected the wrong way and can lead to death in worst case, that's no joke thing.
```

---
## \#13 Posted by: rojitor Posted at: 2018-07-13T08:54:58.233Z Reads: 92

```
That Seller doesn't even know what he is selling. 
Your bms has a shared port. Charge and discharge are the same port. Doesn't make any sense to have 3 wires in that case. One of the P- must be used as charge negative and you take the positive from the main positive.
Again does not make any sense that It has a 10awg wire for charge.
Bms with 2 ports are very common but not with so many wires. I never buy a bms without a diagram. Even a crappy sketch is helpful.
```

---
## \#14 Posted by: J95hicks Posted at: 2018-07-13T13:47:53.269Z Reads: 96

```
I wont be connecting anything till im 100% sure. I understand the danger and also it would be an expensive screw up. I have tried to educate myself the best i can. I did read what the seller said of just using a P- as my Charge negative but [quote="rojitor, post:13, topic:61696"]
does not make any sense that It has a 10awg wire for charge.
[/quote] i do agree with this, tryng to use a 10awg wire as my charge negative seems un-ideal and also [quote="rojitor, post:13, topic:61696"]
Bms with 2 ports are very common but not with so many wires.
[/quote] this. Also does it matter which P- i use for charge then?
```

---
## \#15 Posted by: thisguyhere Posted at: 2018-07-13T16:09:00.693Z Reads: 92

```
are you using this bms for charge and discharge, or just charge only?

here's a charge only (discharge bypassed) diagram:

https://www.electric-skateboard.builders/t/warhorse-2-custom-hollow-core-integrated-build/53428/13
```

---
## \#17 Posted by: J95hicks Posted at: 2018-07-13T16:46:55.362Z Reads: 88

```
My intention is charge and discharge,seeing as i payed the extra money for a high Amp discharge rated bms... what makes you ask? Is my wiring incorrect?
```

---
## \#18 Posted by: J95hicks Posted at: 2018-07-13T17:00:16.997Z Reads: 101

```
This looks VERY similar to mine, except i have the loop key on the B- Negative lead. This post mentions the Bms is NOT bypassed. Which is what i want, bc i have a 150A capable bms. 
https://www.electric-skateboard.builders/t/bypass-bms-with-overcharge-detection-how-that-works/22582/12?u=j95hicks
```

---
## \#19 Posted by: thisguyhere Posted at: 2018-07-13T17:11:15.654Z Reads: 97

```
ok, if you only have a P- and B- port, then this diagram should be right:

http://www.esk8life.com/bestech-d140-10s
```

---
## \#20 Posted by: b264 Posted at: 2018-07-13T17:43:02.520Z Reads: 92

```
Don't group all the balance wires together like that.  A lot of BMS wiring problems are the balance wires being off by one or backwards.
```

---
## \#21 Posted by: J95hicks Posted at: 2018-07-13T17:45:25.216Z Reads: 88

```
I will, my main concern were the leads, crappy schematic was just for my sanity
```

---
## \#22 Posted by: J95hicks Posted at: 2018-07-13T17:58:22.233Z Reads: 84

```
So im pretty close. But according to this, should i use the same P- wire for the charger - and the load -  .. i ask Bc my bms has 3 seperate P- wires, do i use one or two or does the not matter at all?
```

---
## \#23 Posted by: thisguyhere Posted at: 2018-07-13T19:20:42.986Z Reads: 76

```
i bet those three wires are all connected to the same rail in the pcb so anyone should be fine, look underside of the pcb and it should all be connected

just looked at your diagram, don't put your loop key where you have it now.  if it's on the B- line you'll have to power up your board to charge.

instead, put the loop key on the P- line so that your esc is isolated via the loop key, while the battery + bms circuit is complete when charger is plugged in.

hope that made sense.
```

---
## \#24 Posted by: J95hicks Posted at: 2018-07-13T19:47:33.142Z Reads: 73

```
Okay, they do seem connected as far as a can tell rn. And yes that makes sense, so move the loop key to between the P- and the Xt90/Vesc connect so i can charge without the loop key in but still have secured power between Vesc, correct?
```

---
## \#25 Posted by: thisguyhere Posted at: 2018-07-13T20:03:24.385Z Reads: 76

```
yup, you got it.
```

---
## \#26 Posted by: J95hicks Posted at: 2018-07-26T16:55:21.302Z Reads: 68

```
Thisguyhere Hey man, sorry to bring you back here lol. But after i wired my bms like suggested, im getting a different voltage off my bms than what my battery is. ![20180724_164059|374x500](upload://jZ0vSOgwKMdYKdZsucsYK5SNYaH.jpg) ![20180724_164018|374x500](upload://itFMTi3bVm7ESX1MxsaYfLHGtHg.jpg) ![Cells%201-6|500x500](upload://z3xolZ2cdLxuLUdCLMSGaGM4915.jpg) ![Cells%207-12|500x500](upload://sQHtEVC9A5fSeBnBrNjUOtFcB7q.jpg). 
I saw a lil smoke off the bms at one point before i got these readings, and maybe it did something to bms, but i see absolutely no damage, signs, or easonwhy it wouldnt be working correctly. i checked all my balance wires several times.....any advice or insight(already contacted seller and they havent been much help lol.
```

---
## \#27 Posted by: thisguyhere Posted at: 2018-07-26T17:26:13.361Z Reads: 57

```
i'll take a look at this later tonight, at work atm...
```

---
## \#28 Posted by: mccloed Posted at: 2018-07-26T20:12:00.292Z Reads: 52

```
This is probably an instance where there needs to be load on the BMS to filly trigger it. I know the switched 10s BMS from Bestech works this way.
```

---
## \#29 Posted by: J95hicks Posted at: 2018-07-27T02:57:18.814Z Reads: 43

```
that might make sense but why would my Bms being reading a false voltage without a load? ...ill give it a try later though.
```

---

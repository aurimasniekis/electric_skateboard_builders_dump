# Question to those who built their own batterypack

### Replies: 19 Views: 1241

## \#1 Posted by: nordlicht Posted at: 2018-04-18T11:45:48.971Z Reads: 183

```
So I just finished my spotwelder using a car battery, a 500A 12V relais for car things and an arduino with a mosfet to shortcircuit it roughly 30ms. Works surprisingly well.

I bought 50 of the samsung Q30 and am planning for 8s6p. I'll probably do 2x 8s3p parallel since the space under the board is limited. I'll include a BMS of course.

I'm a mechatronic student in the 6th semester, still here are my question(s) to you DIYers:

* what in general should I look out for? I'll clean the batteries and the nickel strips first with isopropanol.

* Did you shrink wrap your battery pack? If so, how did you do that? If not, why didn't you? Did you secure your battery pack somehow else or just built a water/dust proof enclosure?

* Is there something you regret afterwards or would do differently?

* What kind of media can you recommend? I'm watching the YT channel of damian rene and find it helpful, can you recommend good sources besides YT?

Thanks for your time,

Ricky

Edit1: I'm only using 8S since the VESC cant have more electric turns per minute with a 130KV HUB as I asked in this thread: http://www.electric-skateboard.builders/t/torque-hubs-with-130kv-and-12s-50v/50420
Thanks for your concerns tho!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-04-18T11:55:08.847Z Reads: 171

```
I haven’t built a battery but am wondering why you chose 8s6p, why not 10s5p or 12s4p?
```

---
## \#3 Posted by: Genghis_Kuan Posted at: 2018-04-18T12:05:58.597Z Reads: 170

```
Ayy Im a fellow mechatronics student, yeah wondering why you went with 8s6p as well, It could be good dependent on your motor and how fast you want to go but most people typically go 10s or 12s for performance. 

As for the battery Ill post the one I made (soldered mine) but basically I arranged my cells in my P group and siliconed them between the gaps using neutral cure silicone (Anti corrosive) then electrical taped the top and bottom followed by kapton tape, some people also recommend a fishpaper layer to prevent wear. Then I made my connections to a busbar (I used cell level fusing) and then heatshrank the whole thing.![27906288_1555573477811581_1183500653_o388x690](upload://lhjKLIMPMnWn8Ru1BBszg9hTHno.jpg)
@Funktapus I saw heatshrank the top and bottom of his p cell groups. 

Most people from what I see try to seal their battery best they can from dust and then just add a water resisting strip to their enclosure which keeps out the majority of the dust anyway.
```

---
## \#4 Posted by: nordlicht Posted at: 2018-04-18T12:51:15.978Z Reads: 147

```
I edited my OP in order to explain why 8s6p.

Have to ask that stupid: What is a "P Group"?
```

---
## \#5 Posted by: DeathCookies Posted at: 2018-04-18T12:57:33.221Z Reads: 141

```
[quote="nordlicht, post:4, topic:52640"]
What is a “P Group”?
[/quote]

P = Parallel Group
S = Series Group

e.g. 10S2P = 10 in series and each series has 2 in parallel
```

---
## \#6 Posted by: DeathCookies Posted at: 2018-04-18T12:59:07.487Z Reads: 136

```
[quote="nordlicht, post:4, topic:52640"]
I edited my OP in order to explain why 8s6p.
[/quote]

Because of the space?
I would rather go 10S4P or 12S4P for better Performance. Budgetwise it is cheaper to go 8S
```

---
## \#7 Posted by: Quezacotl Posted at: 2018-04-18T13:44:40.556Z Reads: 137

```
-Try to triple-check everything.
-secure the wires so nothing can cut them. For example balance wires from sharp nickel stripes.
-Search for battery fail threads for more pitfalls.
```

---
## \#8 Posted by: Deckoz Posted at: 2018-04-18T14:06:05.503Z Reads: 130

```
I haven't seen anyone mentioned this yet. Which is the biggest key to building. Listed in bold

- you may lay your pack out. Batteries all over. Mixed of positive and negative. Whatever

 - **But EVERY Series connection you make. As you build the battery from cell "1" to however many S you make. You should solder a balance lead, and then COMPLETELY cover that series connection with either kapton or fish paper or a mixture of the two so that it is ISOLATED, and there is no chance of you dropping material, tools, or accidentally touching a previous series connection with a future connection. ONLY then should you weld or solder the next series joint so there is NO chance of shorting.**
```

---
## \#9 Posted by: briman05 Posted at: 2018-04-18T17:11:57.581Z Reads: 120

```
Listen to what @Deckoz says.  There are plenty of guys on here who build there own battery you could ask. @scepterr made mine and is very knowledgeable. I would go with a 10s of 12s because you can always limit the erpm in the bldc tool.
```

---
## \#10 Posted by: nordlicht Posted at: 2018-04-19T10:49:43.780Z Reads: 104

```
Thanks for so many advices!
I will definetly triplecheck everything before giving it a go. Also I'll isolate the parts which are already soldered and see that there comes no longterm damage to the cables.

I am wondering, that you guys advise me to build a 12S batterypack, even though the motor only needs 8s. To make it absolutely clear:

 **Is there a difference in efficiency when I supply the VESC with 12S and the motor only needs 8S? Will I be able to drive the same distance with it when limiting the ERPM to 75.000 on 12S compared to unlimited 8S?** 

Cheers, you were very helpful already!
```

---
## \#11 Posted by: koralle Posted at: 2018-04-19T11:02:15.544Z Reads: 100

```
higher Series -> higher Voltage means fewer amps through all your components for roughly similar performance. This means less heat and all that ensues.
That's a main reason why people go for 10-12s. 

Concerning the welding: Make sure you apply lots of physical pressure to the weld while you press the button. If your nickel strips aren't forced to properly touch whatever is underneath, you can blast shit apart.

![IMG_20180325_005850 (1)|375x500](upload://xzEX3uJXhLn9Qg1IYEwqKiZsWO6.jpg)
```

---
## \#14 Posted by: Quezacotl Posted at: 2018-04-19T11:19:55.805Z Reads: 93

```
For example 1100W motor usage with 33,6V(8S) has 33A while 42V(10S) has 26A. It's not much, so i wouldn't worry about it unless you are constantly using the motor at maximum power.
```

---
## \#15 Posted by: pat.speed Posted at: 2018-04-19T11:56:51.133Z Reads: 90

```
I don’t think the way the battery is configured would make any difference to the space it will use. It will still be 48-50 cells either way
```

---
## \#16 Posted by: nordlicht Posted at: 2018-04-20T11:20:08.546Z Reads: 73

```
Alright guys, I started building it.
I'll do 2x 12S2P, because my BMS is very large and fits well an that format. Its also really flat than.

Here are pictures of the first 12S2P pack. I did only do 1 parallel connection yet because I want you opinion on the welding spots. I especially dislike those on the positive pole on the batteries. This one parallel connection is utter garbage. I melted the plastic isolation. In the future I'll go on the positive poles directly.

I'm shurtcircuiting the battery for 50ms right now. I could increase that time slightly, to 60 - 80 and re-weld it.They do stick to the pole tho, when I try to level a bit with a screwdriver the welding resists.

So before I do the parallel connections, do you guys have anything to add, advises for the other half of the pack?

![IMG_20180420_124945|666x500](upload://bDGfeDU5aYm24pwTBOWE70ZMSTy.jpg)![IMG_20180420_124941|666x500](upload://7i9KzYHVlQk04jBA8MQS7k7qHQw.jpg)![IMG_20180420_125846|666x500](upload://4d9uVZqUuXRZSqoHIyHEN8ObsrB.jpg)![IMG_20180420_124949|666x500](upload://qaAclT98pLrRvfFycmVbJgaaxeY.jpg)![IMG_20180420_124954|666x500](upload://dXdkbhlPOLCx5kuAmTq1qxBcxPK.jpg)![IMG_20180420_125849|666x500](upload://nTkSxzkeQunJxeFWzCg6qxOKIl.jpg)
```

---
## \#17 Posted by: koralle Posted at: 2018-04-20T13:00:23.003Z Reads: 68

```
Mate sry to only tell you now after the fact but you are in clear violation of §1.2 in the Battery pack building Lawbook.

> **§1.2** Thou shalt use fishpaperzz on your positive poles before welding!!!

![IMG_20180324_184315|666x500](upload://o16tWrOmLg6mU1LbVzHTet4eave.jpg)

See the dark green circles - they make sure, the nickel strips can not rub through the pink heat shrink, thus shorting with the negative body of the cell.

https://www.aliexpress.com/wholesale?catId=0&initiative_id=SB_20180420050346&SearchText=18650+insulation

You get them with different hole sizes, according to the width of your nickel strip. (@Blitz  I know there is a joke in there somewhere) There are also ones with a small latch on the side to lie underneath your bms connections.

How sticky are your welds? Can you tear them back off? If they leave these tiny pieces of weld behind, you can remove that with some sandpaper or _carefully_ with a file, making sure you don't short anything.

If they are good welds, they should definitely stick properly and tear small holes into the strip when you tear it off with pliers.
```

---
## \#18 Posted by: koralle Posted at: 2018-04-20T13:25:51.942Z Reads: 68

```
![Positive and Negative Insulation (Small)|400x300](upload://m3OqxhDMTkFFs3P47XnAm7HaJ0J.jpg)
```

---
## \#19 Posted by: PartyPoison Posted at: 2018-04-20T13:32:40.471Z Reads: 70

```
man those are dangerous stuff, you should put insulator at the + side like @Deckoz  did to his pack, he put kapton on whole + side of the before spot weld, you look to his thread http://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411 i ask him how did he made his pack, courteously he made a simple tutorial with pics, awesome dude.
```

---
## \#20 Posted by: Deckoz Posted at: 2018-04-20T13:52:08.510Z Reads: 67

```
Hey thanks for the shout here is the  direct post link to that :slight_smile:
https://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411/81?u=deckoz
```

---
## \#21 Posted by: nordlicht Posted at: 2018-04-20T14:16:40.683Z Reads: 61

```
I thought they are unnessecary since the Q30 has already an isolation ring integrated (the white plastic).
And yes, when ripping the strip off, it does tear holes into it.

@koralle where can I find this "Battery pack building Lawbook" for projects in the future?
```

---

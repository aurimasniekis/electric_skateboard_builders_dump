# Best solution to a On/Off switch

### Replies: 57 Views: 2512

## \#1 Posted by: nikoli280 Posted at: 2018-03-29T13:09:24.628Z Reads: 378

```
Hi i am a bit confused. I am looking for a way to turn on and off my board. I know of these options, 

- XT90 Loop key
- Vedder anti spark
- BMS E switch

I would like to avoid the XT 90 switch since i think its very unpracticable. I have a 10S 60A bms from batterysupport system but without the switch, so im unsure if i can modifie it my self. and then i heard somewhere that the vedder switch can fry my electronics because the fuse is on the positive line. Which i dont quite understand.

Help is greatly appreciated
```

---
## \#2 Posted by: Acido Posted at: 2018-03-29T13:13:50.470Z Reads: 367

```
I would recommend getting a BMS with an eswitch or xt90

Vedders fail with big batteries
```

---
## \#3 Posted by: nikoli280 Posted at: 2018-03-29T13:21:13.837Z Reads: 356

```
I have a 10s4p pack
```

---
## \#4 Posted by: Acido Posted at: 2018-03-29T13:23:25.373Z Reads: 358

```
by big i mean how many amps it can deliver, when you are connecting electronics there's always a big spike in power and that's what fucks up the vedders switches especially if they are high C lipos

I'm not an expert on this, this is just what i remember from what i have read on here

I just found LHBs switch and he says it doesnt fail, so if your getting a switch, get his
https://longhairedboy.com/collections/all/products/12s-bare-bones-eswitch
```

---
## \#5 Posted by: Deckoz Posted at: 2018-03-29T13:26:22.505Z Reads: 337

```
AS150

![IMG_20180309_215427|666x500](upload://m5ZVECCMpumnehhlX3cXYzIu3yp.jpg)![IMG_20180309_215456|666x500](upload://w27nZbk3PSUHeZr2aWOztLled7s.jpg)![IMG_20180309_231122|374x499](upload://2jocjdR4PbI6Rv0eSOuWC6zFNe7.jpg)
```

---
## \#6 Posted by: nikoli280 Posted at: 2018-03-29T13:31:27.180Z Reads: 329

```
Do you attach the negative or positive to the as150?
```

---
## \#7 Posted by: PartyPoison Posted at: 2018-03-29T13:34:08.532Z Reads: 330

```
I second @Deckoz on AS150 
Got that on my carver but not as innovative as his
Mine is an old school pull plug
![DSC_1028|690x388](upload://9SqdDDKVgq4sugLq9EvcUVVa7UO.JPG)
```

---
## \#8 Posted by: nikoli280 Posted at: 2018-03-29T13:46:00.130Z Reads: 320

```
and how did you make the 90 degree angle connector
```

---
## \#9 Posted by: Deckoz Posted at: 2018-03-29T14:05:21.337Z Reads: 322

```
https://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411/160?u=deckoz
```

---
## \#10 Posted by: Alex.Scheff Posted at: 2018-03-29T14:08:40.171Z Reads: 314

```
I will use [this](https://m.de.aliexpress.com/item/32644133837.html?pid=808_0003_0109&spm=a2g0n.search-amp.list.32644133837)
```

---
## \#11 Posted by: Nordle Posted at: 2018-03-29T14:23:44.039Z Reads: 310

```
This will work, but inside there will be a spark like when you plug 2 gold connectors together. The spark, everytime it occurs, will eat away a small bit of the contacts. After given number of switches it will be gone.
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-03-29T14:27:50.678Z Reads: 301

```
That will probably work just fine for a while. 

How many amps are you planning to run typically? For 60 amps or less mine work fine, I use them in conjunction with a 60 amp BMS. 

One scenario that made them fail was when a 250 pound dude was regualrly doing 40mph on it, but 99% of the time they last a while. 

We're in the process of testing the 300 amp Flyer eswitches and they seem to be holding up really well under decent loads at 13S. We need something for much bigger dudes, and that seems to fit the bill. 

The BMSs that are worth a shit that have built in temp sensor switches that can be used as on-off triggers don't come in a form factor that I like, so that's why i have both. 

I'm in the process of building a board with that new open source BMS that's been produced by members of this forum as well, that should reveal enough for us to know if we're going to go in that direction this year. I'm hoping we are. It will solve a lot of issues if it works out.
```

---
## \#13 Posted by: Quezacotl Posted at: 2018-03-29T17:47:54.331Z Reads: 259

```
What is the difference in your eswitch compared to vedder design? I see one extra resistor there.
```

---
## \#14 Posted by: b264 Posted at: 2018-03-29T17:52:19.658Z Reads: 261

```
[quote="nikoli280, post:6, topic:50559, full:true"]
Do you attach the negative or positive to the as150?
[/quote]

Technically it doesn't matter, but to stay with the BMS pattern, the negative lead
```

---
## \#15 Posted by: Acidfie Posted at: 2018-03-29T18:40:04.206Z Reads: 246

```
i heard something about the positive one. thats what @esk8 said to me, so i did the positive.
```

---
## \#16 Posted by: b264 Posted at: 2018-03-29T18:41:03.461Z Reads: 241

```
That should work fine
```

---
## \#17 Posted by: nikoli280 Posted at: 2018-03-30T00:15:17.783Z Reads: 225

```
Do anyone know of how to rewire a BMS to have eswitch
```

---
## \#18 Posted by: b264 Posted at: 2018-03-30T00:19:46.948Z Reads: 224

```
Just add an antispark eswitch, don't rewire the BMS
```

---
## \#19 Posted by: nikoli280 Posted at: 2018-03-30T01:06:00.907Z Reads: 218

```
How would you "just add" an eswitch?
```

---
## \#20 Posted by: b264 Posted at: 2018-03-30T01:08:51.974Z Reads: 217

```
If you propose a circuit diagram, myself or someone else can tell you if it has any problems.  Other than that, searching this forum is a good start
```

---
## \#21 Posted by: nikoli280 Posted at: 2018-03-30T01:09:57.484Z Reads: 200

```
I have searched the forum and that is why I write here. I have no idea of how to add a eswitch to my existing bms
```

---
## \#22 Posted by: b264 Posted at: 2018-03-30T01:12:34.129Z Reads: 196

```
Draw how you think you might and put it here and we will tell you if it's okay.
```

---
## \#23 Posted by: nikoli280 Posted at: 2018-03-30T01:13:35.945Z Reads: 201

```
I have no idea. I ask to see if people have done it before. I have contacted sunpowersyste. But they are very slow to answer
```

---
## \#24 Posted by: b264 Posted at: 2018-03-30T01:15:21.871Z Reads: 193

```
https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/53?u=b264
```

---
## \#25 Posted by: nikoli280 Posted at: 2018-03-30T01:21:38.973Z Reads: 186

```
That's the setup for ant spark switch. I'm asking about BMS e dwitch
```

---
## \#26 Posted by: b264 Posted at: 2018-03-30T01:24:17.054Z Reads: 189

```
Nobody is going to tell you how to do it.  If you propose something, you might get someone to say if it's good or not good.  There is an entire thread I linked with tons of information.  We have no idea what you have.

Alternatively, you can buy an electric skateboard already made
```

---
## \#27 Posted by: nikoli280 Posted at: 2018-03-30T01:28:39.116Z Reads: 187

```
I'm sorry I don't understand d your post. I know it's possible and some have done it. I have no idea how so I ask for holp
```

---
## \#28 Posted by: Deckoz Posted at: 2018-03-30T01:42:10.797Z Reads: 187

```
I put the AS150 on the positive side,which leaves everything grounded when off.  But either way is fine.
```

---
## \#29 Posted by: Jebe Posted at: 2018-03-30T01:42:35.366Z Reads: 187

```
Solid state relay
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-03-30T01:43:08.581Z Reads: 188

```
At the moment I just pull off non AS XT90 from battery :D
```

---
## \#31 Posted by: longhairedboy Posted at: 2018-03-30T01:44:49.071Z Reads: 185

```
[quote="Quezacotl, post:13, topic:50559, full:true"]
What is the difference in your eswitch compared to vedder design? I see one extra resistor there.
[/quote]

The mosfets i'm using are rated at a higher voltage and fail less.
```

---
## \#32 Posted by: Kug3lis Posted at: 2018-03-30T01:49:05.634Z Reads: 177

```
If you want good handling stuff, pick a block mosfets they are like 30-50£ but they handle 300-500A and high current. Plus they are not like to220 package which can't handle quick temp rises :)

https://www.mouser.co.uk/datasheet/2/427/vs-fc420sa10-1110749.pdf
```

---
## \#33 Posted by: Nordle Posted at: 2018-03-30T07:00:38.345Z Reads: 170

```
The one linked is 20€, that seems worth a try.
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-03-30T16:00:25.848Z Reads: 167

```
Here is my mock up :P

![image|690x474](upload://xAaoMgCIVPLGuRI04HCnIUMfccR.jpg)
```

---
## \#35 Posted by: Acido Posted at: 2018-03-30T16:22:45.970Z Reads: 163

```
did you order a bms from me?
```

---
## \#36 Posted by: Alex.Scheff Posted at: 2018-03-30T18:06:13.016Z Reads: 156

```
The only problem, regenerative braking would not work
```

---
## \#37 Posted by: Kug3lis Posted at: 2018-03-30T18:09:35.587Z Reads: 157

```
how it would not work? :)
```

---
## \#38 Posted by: nikoli280 Posted at: 2018-03-31T00:24:01.794Z Reads: 144

```
No unfortunately not I have a sunpowersystem BMS laying around that I would like to use. If nothing works I guess I have to look for a group buy
```

---
## \#39 Posted by: nikoli280 Posted at: 2018-03-31T00:24:26.910Z Reads: 144

```
How is this connected?
```

---
## \#40 Posted by: Kug3lis Posted at: 2018-03-31T00:36:26.013Z Reads: 145

```
Battery + goes into one side, Load + goes another, and there is a simple toggle button, which you need to sort to Battery + to turn it on :)
```

---
## \#41 Posted by: nikoli280 Posted at: 2018-03-31T01:32:21.779Z Reads: 129

```
How do you connect the switch to the mosfet. And wouldn't it decrease the voltage after using the mosfet?
```

---
## \#42 Posted by: Nordle Posted at: 2018-03-31T04:58:30.618Z Reads: 132

```
Off:
![image|690x287](upload://6c8Y285msBbAbGXDOTdtVq9iWhY.png)
On:
![image|690x287](upload://rrCsUr0xEk1LON3jSNXuc1gxJxA.png)

There will be a small drop in voltage after the mosfet cause everything has a resistance (except superconductors), but power fets have very low resistance so probably nothing to care about.

Braking will just work fine...
```

---
## \#43 Posted by: Alex.Scheff Posted at: 2018-03-31T08:12:03.300Z Reads: 123

```
![20180331_101304|690x441](upload://fjFsW7hSyd1bqYH9FZgghtpIVp9.png)

There is a diode inside and it will just let electricity trough in one direction.
```

---
## \#44 Posted by: ARetardedPillow Posted at: 2018-03-31T08:39:22.564Z Reads: 116

```
Does anyone know how prebuilt eskates like Evolve and Boosted do their switches?
```

---
## \#45 Posted by: Nordle Posted at: 2018-03-31T09:27:40.098Z Reads: 115

```
This is the symbol for a mosfet, the orientation of the diodes say if it's N or P channel.
```

---
## \#46 Posted by: Kug3lis Posted at: 2018-03-31T17:05:53.233Z Reads: 107

```
It goes reverse, the normal flow. So for e.g. You turn off the mosfet but you can still move current backwards like regenerating braking :)
```

---
## \#47 Posted by: nikoli280 Posted at: 2018-04-01T03:14:30.876Z Reads: 93

```
But how would you connect a switch
```

---
## \#48 Posted by: nikoli280 Posted at: 2018-04-01T03:17:01.339Z Reads: 93

```
And what about using something like the HY4008W it can handle 200a isswnt that plenty. It's also cheaper
```

---
## \#49 Posted by: Nordle Posted at: 2018-04-01T06:06:31.484Z Reads: 97

```
[quote="nikoli280, post:47, topic:50559, full:true"]
But how would you connect a switch
[/quote]
Dunno what is wrong with some of you guys on here
![image|404x500](upload://h5seM8LkBVdQN1QzHyfJmsdoHbN.jpeg)
```

---
## \#50 Posted by: b264 Posted at: 2018-04-01T07:43:51.319Z Reads: 94

```
[quote="Nordle, post:49, topic:50559"]
Dunno what is wrong with some of you guys on here
[/quote]


Some people are here because they want a cheap electric skateboard and aren't here for the "DIY" part.  If you're one of those folks, I will give you a tip: these are better, not cheaper.
```

---
## \#51 Posted by: nikoli280 Posted at: 2018-04-01T10:07:11.703Z Reads: 81

```
Sorry i did not see that but is this schematic the same as the one for the 400A mosfet?
```

---
## \#52 Posted by: Nordle Posted at: 2018-04-01T10:29:18.189Z Reads: 80

```
It‘s the same, some components ratings may change with other mosfets.
```

---
## \#53 Posted by: nikoli280 Posted at: 2018-04-01T10:43:19.239Z Reads: 85

```
Have you down this in practice? If so can you share pictures
```

---
## \#54 Posted by: Nordle Posted at: 2018-04-01T11:31:07.741Z Reads: 83

```
I did, this is not mine but looks similar. Mine is already shrinked and in use.
![image|600x450](upload://gFV4YGg6OOK5abItYv3dk3rFUYL.jpeg)
```

---
## \#55 Posted by: nikoli280 Posted at: 2018-04-01T12:24:41.591Z Reads: 80

```
Interesting, 2 question I can't see a psycical switch here. And where do you ground the mosfet? Just on the negative wire?
```

---
## \#56 Posted by: Nordle Posted at: 2018-04-01T12:29:22.822Z Reads: 83

```
You also don‘t see a battery or an esc/motor cause its further away and not shown in pic

If you can‘t read and understand the schematic you should buy a finished switch..
```

---
## \#57 Posted by: nikoli280 Posted at: 2018-04-01T12:48:34.769Z Reads: 81

```
Please try to answer. I'm no expert in electronics and I am trying my best to learn but it's hard if I can't ask questions
```

---

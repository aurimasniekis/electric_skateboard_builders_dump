# Esk8 that can go up hill and travel in plane

### Replies: 53 Views: 4002

## \#1 Posted by: Trans-amers Posted at: 2016-07-15T09:24:01.719Z Reads: 323

```
I am new to esk8, even for skateboard too. I want to build one that could go up in steep hills but I can take it with me in plane. Here's my plan
5000-6000 mah 18650 6s
TorqueBoards 120A 6S ESC
6374 motor x1 (since I live in China so I wanna and have to buy something cheap)
wheels :83mm
belt: 5M270

But then I found out that 6s might not be able to drive the 6374
Basically I think I am building a boosted replica, that it could climb hills and put on planes.
I can't really find the spec of Boosted as reference so do you guys have any suggestion for me?
```

---
## \#2 Posted by: quinnyt2015 Posted at: 2016-07-15T10:01:57.000Z Reads: 305

```
Don't quote me but boosed has a 99Wh = 12S1P battery using 26650 batteries. Wh = Number of cells in series * Voltage Per Cell * Amp Hours, so 3.3V * 2.5A * 12 Cells = 99Wh which is the maximum size battery you can take on a plane.
```

---
## \#3 Posted by: Dedbny Posted at: 2016-07-15T10:12:40.275Z Reads: 295

```
Get a new label made up with 99wh
```

---
## \#4 Posted by: Photorph Posted at: 2016-07-15T10:23:25.002Z Reads: 289

```
On something like the raptor, or any board with a removable battery... You can travel with the board and ship the battery seperately to your destination.
```

---
## \#5 Posted by: torqueboards Posted at: 2016-07-15T10:26:25.493Z Reads: 280

```
@Trans-amers - We also do have 12S1P A123 same style pack as Boosted does as well. As @quinnyt2015 mentioned it is 99wh!
```

---
## \#6 Posted by: Dedbny Posted at: 2016-07-15T10:30:39.335Z Reads: 273

```
Do you want your space cell lost in mail.  Easier to get sticker. I think this battery issue is over the top with the airlines.. Or just find a hobby shop in place of destination.and buy a new battery.
```

---
## \#7 Posted by: quinnyt2015 Posted at: 2016-07-15T10:43:52.287Z Reads: 270

```
Can you post a link please?
```

---
## \#8 Posted by: cmatson Posted at: 2016-07-15T12:00:22.560Z Reads: 271

```
You can take your battery on board as long as it looks professional, and says something like "20v 4.4ah"

That way, when the airport security guys ask the wathours, you tell them; they can then verify it by doing the math if they know what they're doing.

Haha when I was flying air new Zealand the guy was determined to find out the "mega hertz" of my battery, and I kept insisting that didn't exist- I kept saying the watt hours of the pack, and that the flight rule was that it must be under 100 watt hours.

Basically to sum things up I got stopped at every airport, and each time all the security folks would get together, consult their sheet of rules, and then take my battery to the back office for 10 minutes. They'd either calculate the watt hours themselves, or just ask me, and then let me on my way.
```

---
## \#9 Posted by: torqueboards Posted at: 2016-07-15T23:32:18.430Z Reads: 245

```
@quinnyt2015 - diy-electric-skateboard-kits-parts/12s1p-a123-26650-epower-electric-skateboard-battery/

The current batch which we received is rated for 40a/80a so you'll need an external on/off switch. We're going to get these packs made again except the on/off switch will be built in.

They have 1,000+ life cycles compared to 18650 cells which are rated for about 300-500 life cycles.
```

---
## \#10 Posted by: Rasha Posted at: 2016-07-15T23:39:49.379Z Reads: 239

```
I really wonder why there's no "99wh battery" sticker template floating around on here.
```

---
## \#11 Posted by: anorak234 Posted at: 2016-07-16T04:13:47.841Z Reads: 229

```
The most you can go if you want it to be airplane legal is 6s 4500 mah
```

---
## \#12 Posted by: RunPlayBack Posted at: 2016-07-16T04:25:18.951Z Reads: 216

```
I think 12s1p is a great choice if you frequently travel. It's small, compact and rather than trying to game the system with a sticker, you'll actually be within TSA rules. Not only that but the chemistry of LiFePO4 is very stable and can withstand punctures, high temps and shorts without safety issues. Just a little piece of mind when your 39,000 feet in the air.
```

---
## \#13 Posted by: torqueboards Posted at: 2016-07-16T05:08:36.013Z Reads: 204

```
12s (3.3v * 12 = 39.6) * 2.5ah = **99wh for A123 26650 12S1P 2500mah** or **6S 4500mah 99.9wh**.
```

---
## \#14 Posted by: rubz Posted at: 2016-07-16T09:25:53.207Z Reads: 202

```
I was just looking at your website and saw this pack
diy-electric-skateboard-kits-parts/electric-skateboard-battery-epower-pack-6s2p/

It says:
> Our latest 6S2P EPOWER Pack provides 96 Watt Hours.
> To be legally able to bring your Electric Skateboard on an airplane or travel with it. You need a battery pack which is less than 100wH.
> Our 6S2P solves this problem.

>6S2p 18650 Battery Pack with LG HE4 18650 cells

This doesn't really check out, it's not really 96Wh. 6*2*2,5Ah*3,6V = 108 Wh.
```

---
## \#15 Posted by: torqueboards Posted at: 2016-07-16T09:57:25.902Z Reads: 199

```
This 6s2p is actually a 2000mah cell. Samsung 20R. Need to fix that. Thanks for catching that.
6s4ah = 22.2*4 =  88wh
```

---
## \#16 Posted by: Trans-amers Posted at: 2016-07-16T11:07:46.116Z Reads: 198

```
Since I am just 67KG, I think I can make one with single 6374 and a 12s1p battery, can I?
Also I never know what does P means in 12s1p, I do know that 12s = 12 cell in series which the voltage adds up. 
Will a 12s1p overkill one 6374?
```

---
## \#17 Posted by: lox897 Posted at: 2016-07-16T11:31:24.846Z Reads: 196

```
P means parallel. Parallel increases amp hours. Look at the specs of your motor on the hobbyking page to find out if it can accept 12S.
```

---
## \#18 Posted by: Dedbny Posted at: 2016-07-16T11:31:32.046Z Reads: 193

```
Ok. I have the best solution for getting any eboard battery on a plane. Just make sure the battery is dead. Bring a voltage tester to show security its dead. If your got a space cell even better. Just turn your battery switch on to show its not working. Has been tested with local airline here in Aus, so should be the same for other airlines around the world. See how you go.
```

---
## \#19 Posted by: lox897 Posted at: 2016-07-16T11:33:16.557Z Reads: 184

```
Haha, nice idea? What do you mean by the battery dead though? Like 0v or nominal?
```

---
## \#20 Posted by: Dedbny Posted at: 2016-07-16T11:34:23.500Z Reads: 185

```
0.  Less than twenty characters zero.
```

---
## \#21 Posted by: lox897 Posted at: 2016-07-16T11:37:51.731Z Reads: 176

```
On percentage? I don't think that changes a lot, the batteries still have power in them.
```

---
## \#22 Posted by: Dedbny Posted at: 2016-07-16T11:48:16.150Z Reads: 171

```
You can try it. It has worked.
```

---
## \#23 Posted by: lox897 Posted at: 2016-07-16T12:02:58.544Z Reads: 177

```
It worked with a percentage monitor or actual voltage meter?
```

---
## \#24 Posted by: Trans-amers Posted at: 2016-07-17T11:41:47.366Z Reads: 173

```
Do I have to use two esc for two 6056?
```

---
## \#25 Posted by: lox897 Posted at: 2016-07-17T21:48:31.637Z Reads: 163

```
Yes. You have to use one ESC per motor.
```

---
## \#26 Posted by: Trans-amers Posted at: 2016-07-18T05:19:41.719Z Reads: 156

```
The only battery I found near me is a 9s1p 18650 3ah
It cheaper to buy i here yet the battery has a lower 9x3.7= 33.3V
They claim that the highest voltage is 4.2V and thus the maximum is 9x4.2= 37.8V
While boosted has a higher 12 x 3.3 = 39.6V. 
Can climb hills with 9s1p 18650 3ah and dual 6065?
```

---
## \#27 Posted by: lox897 Posted at: 2016-07-18T05:21:13.383Z Reads: 154

```
Depends on the kv of the motor. I can climb hills on 6S so you should be fine.
```

---
## \#28 Posted by: Trans-amers Posted at: 2016-07-18T07:02:40.444Z Reads: 148

```
How about a 270 kv 5065?
```

---
## \#29 Posted by: lox897 Posted at: 2016-07-18T07:14:52.954Z Reads: 143

```
Are you using VESC? For 9S I would go for 200kv. 270kv is a bit too much.
```

---
## \#30 Posted by: Trans-amers Posted at: 2016-07-18T08:05:03.906Z Reads: 140

```
nah I am using TorqueBoards 120A 6S ESC
I don't think the ESC can control the system.
How is your set up of 6s which can go up hill?
```

---
## \#31 Posted by: lox897 Posted at: 2016-07-18T08:15:45.545Z Reads: 144

```
I have a 6S 190kv geared 15/36. It has really good torque. Haven't tested it on long hills but I have tested it on steep short hills.
```

---
## \#32 Posted by: NAF Posted at: 2016-07-18T13:21:52.260Z Reads: 149

```
99WH rule is just pure nonsense.... this wont give enough range for traveling :)  ...that's why I've passed on 99wh battery and I'll be trying to take 10s3p battery where ever I go. The thing with me is that I always carry a lot of equipment with me. Two professional camera's + big lenses, laptop, chargers, sometimes small lighting. I even used to bring IMAC 21'5" in special  backpack and I was always fine. Of course sometimes they take me to this secret room with more scanners and do some additional search, but usually it's always fine. 

 I'll be making 10s3p - 320 wh pack that looks like SPACE CELL, but it will have two USB hubs additionally. On the cover I'll make super nice big sticker saying " External Usb Power Bank" . My  iphone will be pluged in while I pass the TSA scanner. I should be fine. 

TSA agents are always ok dudes if you tell them that you are professional with a lot of equipment.
```

---
## \#33 Posted by: VladPomogaev Posted at: 2016-07-19T09:17:12.489Z Reads: 148

```
I'm not sure about the states, but in Canada the rules are no electric skateboard with the battery inside. I had to travel recently with my e-board, and I took out the battery. Since I was using two 55.5Wh batteries I was safe from the 100Wh rule, and they just let me carry the batteries on the plane.

Basically, you can always split your battery pack into two ;)
```

---
## \#34 Posted by: DilatedPupils Posted at: 2016-07-19T09:33:47.757Z Reads: 145

```
So, you can bring more than one "99 Wh" battery on the plane?
```

---
## \#35 Posted by: VladPomogaev Posted at: 2016-07-19T09:41:22.053Z Reads: 143

```
Yup, that's what happened to me.
```

---
## \#36 Posted by: kampfhahn Posted at: 2016-07-19T09:43:31.030Z Reads: 136

```
Yes. That´s why a good setup for travellers is 10S using 2x5S 5000 Lipos. Total of 180 Wh, but you can easy take the batterys (90 Wh each) on a plane.
```

---
## \#37 Posted by: jrpwit Posted at: 2016-07-19T10:21:00.658Z Reads: 136

```
Ayyy u just make an account? I saw your vids on youtube they were pretty decent!
```

---
## \#38 Posted by: jrpwit Posted at: 2016-07-19T10:23:48.405Z Reads: 136

```
The official rule is that you can only bring two 99wh batteries on a plane.
```

---
## \#39 Posted by: VladPomogaev Posted at: 2016-07-19T10:28:00.665Z Reads: 138

```
Lol thank you :) I have had the account for a long time now, and I'm going to be uploading my newest carbon-fiber e-board there. Here's a [link](https://www.youtube.com/user/comsa42) for anyone who's interested.

Edit. Woops, thought you meant the YouTube account! No, I made this account an hour ago haha.
```

---
## \#40 Posted by: jrpwit Posted at: 2016-07-19T10:43:12.169Z Reads: 136

```
Lol nice to see u on the forum! You should link this website in your vids tho. More people on this forum is for the best and we are always happy to help people! Also try the vesc it the best esc for electric long boards.
```

---
## \#41 Posted by: VladPomogaev Posted at: 2016-07-19T10:48:29.612Z Reads: 131

```
Yeah maybe. I had a lot of mixed feelings about this site because it promoted expensive kit components so much. With a little bit of Googling and a soldering iron, you can make some really cool stuff and save yourself a lot of money. But I digress, the people on this forum have been extremely friendly and nice, and I'm going to start posting a lot here :) 
Also, I tried to build the VESC while it was in it's beta stage. The components seemed so expensive; I have no idea how they got the price down so quickly.
```

---
## \#42 Posted by: DilatedPupils Posted at: 2016-07-19T12:07:40.003Z Reads: 128

```
Good to know thanks. I'm planning on building my "travel" board soon. So, you check in your board, and you carry on your batteries, right?
```

---
## \#43 Posted by: jrpwit Posted at: 2016-07-19T12:26:24.020Z Reads: 130

```
99wh really isnt that much as many said above. Fortunately it seems that you can take larger batteries without too much of a problem. I looked it up and this article says that spare batteries can only be carry-on baggage. Here's the link if u want to read up on it https://www.faa.gov/about/initiatives/hazmat_safety/more_info/?hazmat=7
```

---
## \#44 Posted by: kampfhahn Posted at: 2016-07-19T12:27:19.025Z Reads: 133

```
Yes, the batterys have to be in your handluggage. Tape the connectors to avoid shorts and use Lipo-Safebags and put the batterys out of the bags in the security check that the officials don´t have to do.
```

---
## \#45 Posted by: VladPomogaev Posted at: 2016-07-19T12:42:11.222Z Reads: 135

```
[quote="jrpwit, post:43, topic:6142"]
tely it seems that you can take larger batteries without too much of a problem. I looked it up and this article says that spare batteries can only be carry-on baggage. Here's the link if u want to read up on it
[/quote]

Don't try to hide your batteries either. They will know :sweat_smile:
```

---
## \#46 Posted by: Hummie Posted at: 2016-07-19T17:43:41.170Z Reads: 135

```
U can carry 3 batteries.  One in the device up to 100wh and two others up to 160wh.   Just break ur pack apart into three batteries. 

According to what I just read from faa linked above
```

---
## \#47 Posted by: itsmikeholland Posted at: 2016-07-19T18:42:57.590Z Reads: 126

```
You can take 3x 99wh batteries, they just need to be seperated.
```

---
## \#48 Posted by: Hummie Posted at: 2016-07-19T20:21:08.734Z Reads: 125

```
it says up to 160wh
```

---
## \#49 Posted by: jrpwit Posted at: 2016-07-20T00:59:22.487Z Reads: 124

```
[quote="Hummie, post:46, topic:6142"]
U can carry 3 batteries.  One in the device up to 100wh and two others up to 160wh.   Just break ur pack apart into three batteries.
[/quote]

Keep in mind this is per person so should be a problem if you travel with someone.
```

---
## \#50 Posted by: DilatedPupils Posted at: 2016-07-20T06:02:09.002Z Reads: 117

```
You can carry your esk8 with you as a carry on?
```

---
## \#51 Posted by: Jinra Posted at: 2016-07-20T06:04:31.232Z Reads: 120

```
I've heard of success with this, though some airlines (in the US at least) have clear restrictions on bringing boards as carry on. I imagine if you remove the trucks and stow them in your luggage/carryon you can convince them to let you bring a flat piece of wood onboard as it takes up virtually no extra space!
```

---
## \#52 Posted by: jrpwit Posted at: 2016-07-20T06:06:24.679Z Reads: 122

```
I have brought a normal skateboard on board as a carry-on before.
```

---
## \#53 Posted by: composites_r_awesome Posted at: 2018-07-10T10:08:22.559Z Reads: 47

```
Hi

Can you tell, If my 6x / 12x <100Wh battarias what will look and are labeled professional, have voltage and temperature meters, safety caps on all contacts for transport, enclosed and sleek  (think like larger laptop battery) with carried in enclosed aluminium 'gun cases' for the flight: could I get airport passes in beforehand? Through e-mail or with the aid of local airport 'inspection' results?
Could they reject randomly tho having a green light before?

Thanks!
```

---

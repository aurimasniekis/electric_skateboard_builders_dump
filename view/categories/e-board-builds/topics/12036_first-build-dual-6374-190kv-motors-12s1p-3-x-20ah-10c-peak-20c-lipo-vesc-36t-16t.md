# First Build - dual 6374 190kv motors - 12s1p - 3 x 20ah 10c peak 20c LiPo - vesc - 36t/16t -

### Replies: 12 Views: 2995

## \#1 Posted by: delduked Posted at: 2016-10-27T23:40:55.123Z Reads: 330

```
Hello everyone,

This is my first time posting in any forum and would like the help from the community to confirm if my math and ideas are correct before I start buying parts and building the electric long board. That being said, Ill list my parts below. The purpose of this post is just to see if all my logic is sound so if you find any errors or irregularities please I am open to criticism.

2 * Electric Skateboard Motor 6374 190KV 3150W
1. Max Amps: 80 Amps
2. Max Volts: 12S
3. 12S 120A-150A
4. 150mm silicone 12AWG 5.5mm Gold Bullet Connector Female

3 * 4S 20000mAh (overkill)
1. discharge 10c peak 20c
2. 14.8v

2 * vesc
1. 5v BEC
2. 8V - 60V
3. 50a continuous 240a 5sec

1 * dual motor Mechanical electrical kit
1. 36/16T
2. 63mm spacing
3. Rear mount

So with the specs all out of the way I think I'll start with the batteries.
When I started I knew I didn't want to make an electric skate board just to see if I could do it ( I still don't). But if I did I'm going to make a darn good one. Which is why I wanted my batteries to last forever. with 20ah I knew the board could go for a long time however I didn't know all about the technical math side of batteries. I found out that I could reach peak performance if I use 12s to match the cap of the vesc. So I decided to get 3 20ah in series. So instead of 4s1p I would get all three batteries working as one for 12s1p. The Discharge rate was low which I was concerned at first but then I found out that having a big battery meant I could get a big discharge because discharge = 10c * 20ah = 200a discharge per hour. This matched up good because the VESCs has continuous amperage of 50a with a peak of 240a. I could keep the amperage at 50a by configuring the vesc. and at the same time the VESCs limit for voltage was 8v-60v where the batteries in series would mean the voltage would equal 14.8 * 3 = 44.4v. Which would also mean 44.4v * a continous 50a would equal 2220w. Which my motors were 3150w each (that's if im using the right formula, hence this post).

My next thought was how am I going to charge these since my battery chargers had a limit of 6s charging and in series my batteries are 12s. So I thought I would charge them parallel. 

I made a drawing of how this works, (I'm still un sure of myself when it comes to the charging part since I don't know the proper units of anything to charge the batteries).


<img src="/uploads/db1493/original/3X/0/d/0d7b0d2cf590af0c9655bb31fdcd34dad50fec67.jpg" width="666" height="500">

After that drawing I decided to learn about gear ratios on the belt. I found that a wider belt is generally better. From the diy electric skateboard website they had either a 36t-13t or 36t-16t. The latter would be faster but the former would have more torque (I think). But then I thought the two motors have enough torques anyway so just go with the 36t-16t anyway. I think I have decided on 36t-16t.

I then started considering what kind of hardware I would need. The batteries use a xt-90 with 5.5mm 10awg cables and JST to connect to the charger. The motor has 12awg cabling but still has 5.5mm cables with bullet connectors on the end. So I think i'm just going to buy a ton of 10awg cable,heat shrinks and xt90 connectors.

The next thing was how am I going to solder everything since I have never done that before. It turns out that a guy on youtube named Barnes'd had some really videos showing him doing a lot of really nice solder work.  link below.
https://www.youtube.com/watch?v=ADl67Fe2Fnk

As for actually setting up all these things I thought how to connect the to VESC to work together. I found out that it was by a jst cable that run to-and-from eachother. All I had to do was remember to setup them up in Master/Slave mode with all the different peaks for all the different electrical units.

I then started to question if the two motors would actually fit on the mounts because the pictures on diy electric skateboard have to 50mm motors and they look a little too snug. And yet the website says you can get the 63mm motors but it sure doesn't look like that to me.

With all that I decided to figure out the speed of all these parts if they did indeed work together magically somehow.

with 16t-36t, voltage of 44.4v, 190Kv, tire diameter of 83mm I could travel a speed of 59km/h or 36mph. Holy cheese balls batman.

I started to play with the gear ratios and found out that my 16t-36t wasn't as fast as a 18t-36t which was 66km/h or 41km/hr. However I don't know where to get those in canada.

Oh, and this is all going on either a Sector9 Sentinel II or a Loaded vanguard.

I think that's the end of my rant. If anybody has any critiques please post a reply or comment or something that is constructive. I look forward to hearing from the community.
```

---
## \#2 Posted by: ajaynagra Posted at: 2016-10-27T23:55:33.546Z Reads: 279

```
Are you aware you need to go diagonal drive
```

---
## \#3 Posted by: delduked Posted at: 2016-10-27T23:58:52.956Z Reads: 285

```
I know what diagonal drive is but I don't know why I would need it in this build.
```

---
## \#4 Posted by: Jinra Posted at: 2016-10-28T00:07:01.078Z Reads: 289

```
Good choice nearly all around. Just keep in mind, as @ajaynagra said, you'll need to go dual diagonal unless you find extra wide trucks. If you're not very heavy (<200lbs) you can use 6355 motors and fit them both on the same truck. You won't have any torque issues at 16/36 with 6355's. I use 16/36 with 5065's in dual diag and they fly up any hill I ride. 

If you want to build the "best" skateboard you can, go with 18650 cells. While Lipos are easy, slim, and generally cheap, they're not as energy dense as li-ion cells and are not as safe. 18650's are a more elegant solution in my opinion. You can also throw in a BMS (you can do this with your lipos as well) for easier charging without having to take out the batteries. If you buy a 12s BMS you can charge just as you would charge a laptop, a single plug.

Soldering isn't too hard to learn, but don't cheap out and get a $25 iron. A good iron goes a long way. I suggest investing in a ~$100 soldering station. Hakko and Weller are good brands. I use [this kendal one](https://www.amazon.com/gp/product/B00W6FK8IG/ref=oh_aui_search_detailpage?ie=UTF8&psc=1) myself and it's been great. It comes with a heat gun for hot air soldering and heat shrinking which is a great bonus.
```

---
## \#5 Posted by: delduked Posted at: 2016-10-28T00:15:31.314Z Reads: 265

```
Thanks, thats good advise. Im 190lbs btw. I went with the 6374 motor because its seemed to have a higher watt rating but with this build I dont see this board going over 3150w. Do you think its over kill? or could I get the same or similar result witht eh 6355s?
```

---
## \#6 Posted by: Jinra Posted at: 2016-10-28T00:22:44.663Z Reads: 254

```
Yea I'd say just go 6355's, theyre lighter and consume less power anyway. Invest more into your battery instead.
```

---
## \#7 Posted by: e-Octo Posted at: 2016-10-28T00:31:13.099Z Reads: 250

```
[quote="delduked, post:1, topic:12036"]
3 * 4S 20000mAh (overkill)1. discharge 10c peak 20c2. 14.8v
[/quote]

Are those the multistar 10Ah 10c packs?  I've heard that their rating for constant discharge is very suspect.  So i would be  concerned that they can supply ample amps to power your board in series.  In parallel will lessen the burden on them.  If pushed hard i'd expect shorter pack life, or even damage (puffy cells) possibly.  If you haven't purchased them i might go another direction?

Do you really need 20Ah range?  Even 10Ah range?
```

---
## \#8 Posted by: delduked Posted at: 2016-10-28T00:41:50.987Z Reads: 240

```
I thought to myself, "can I actually have 20ah in a board? I probably could......Ok ill do that."

and yes https://www.hobbyking.com/en_us/multistar-high-capacity-4s-20000mah-multi-rotor-lipo-pack.html

The alternative batteries were these https://www.hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html

However @Jinra suggested 18650s might be better... So I am considering that now.
```

---
## \#9 Posted by: e-Octo Posted at: 2016-10-28T00:45:37.576Z Reads: 237

```
I'd suggest 20 or 30c lipos if you go that route.  Or 18650 like @Jinra suggests.  Another advantage of the 18650 cells is longer life vs lipo.  It's all in your constant amp draw and how much you heat them.  Heavy use and big voltage sag is not good for any cell - lipo or 18650.  heat is the killer.
```

---
## \#10 Posted by: Eboosted Posted at: 2016-11-23T09:02:48.273Z Reads: 198

```
How did it go with you build? I'm planing the same build on the same Vanguard Deck. 

Did you get the dual 6355 190kv 2500W motors with the DIY skateboards mechanical kit?
```

---
## \#11 Posted by: delduked Posted at: 2016-11-24T01:24:16.163Z Reads: 197

```
Unfortunately I am still waiting on the company that is making the motor mounts from a CNC. I have tried many companies but I haven't seemed to get any business until now. Even the guys i'm talking with currently are taking forever. In the mean time I have been trying to find shaft collars that can clamp on my trucks. I also got a sheet of aluminum for the motor to mount to, then I will mount the aluminum sheet to the collar that will be clamping on the trucks. Once I have made sure that everything will mount properly I'm going to buy the the gears and use a chain belt.
```

---
## \#12 Posted by: Eboosted Posted at: 2016-11-25T03:39:49.061Z Reads: 182

```
I don't understand why you did go CNC route, it usually takes forever and you won't see the final result.

These motor mounts are perfect for 190kv 6355 2500w motors in dual rear wheel setup:

diy-electric-skateboard-kits-parts/v4-63mm-motor-mount/

I don't like the idea of a diagomal setup, I like it to be aesthetically ballanced all around.
```

---

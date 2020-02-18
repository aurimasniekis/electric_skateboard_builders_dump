# Question about building a custom 12s BMS power supply

### Replies: 91 Views: 1741

## \#1 Posted by: dg798 Posted at: 2018-01-07T17:48:14.985Z Reads: 146

```
I am building a custom charger for my batteries. It’s a 12s setup and I ordered a drok cc cv step up module. I will be using a 12v power supply as input and output will be 50.4v. My question is how will I know when all the cells are charged and balanced?
```

---
## \#2 Posted by: dg798 Posted at: 2018-01-07T17:57:34.936Z Reads: 137

```
This is what I ordered: DROK Numerical Control Regulator DC 8-60V to 10-120V 15A Boost Converter, Constant Step Up Module Adjustable Output 48V 24V 12V DC Power Supply with LED Display https://www.amazon.com/dp/B01GFVI6R6/ref=cm_sw_r_cp_api_f8LuAb5X0WA6W
```

---
## \#3 Posted by: vishal_tejwani Posted at: 2018-01-07T19:16:57.488Z Reads: 130

```
I am curious about this answer too, after cc cycle usually the Amp goes down, that might be the indication. I may be completely wrong but, if anyone has done this can answer better, 

Eev blog has video on this i guess
```

---
## \#4 Posted by: Genghis_Kuan Posted at: 2018-01-07T19:35:28.854Z Reads: 119

```
Im doing something similar, @Hummie suggested I use an inline watt meter. If you set a constant voltage when your battery comes to full charge (At that voltage) there will be little to no potential difference between the supply and the battery therefore current will drop to a very small amount. 

Just dont set your voltage too high (I.e 4.2v per cell) and leave it on full charge for a long time as it might be bad for the cells. Read here: https://endless-sphere.com/forums/viewtopic.php?f=14&t=83043&hilit=trickle+charg%2A
```

---
## \#5 Posted by: dg798 Posted at: 2018-01-07T19:47:29.105Z Reads: 105

```
What if I use a 12v power supply with a light on it. Will the light turn green at 12v or will it turn green or whatever color when the cells are all balanced for a total of 50.4v??
```

---
## \#6 Posted by: dg798 Posted at: 2018-01-07T19:50:03.740Z Reads: 103

```
Or maybe just keep a multimeter in the xt60 and when it reaches 50.4, stop it. Just throwing out ideas.
```

---
## \#7 Posted by: Genghis_Kuan Posted at: 2018-01-07T20:07:25.426Z Reads: 103

```
You can do the light thing, but that would require a separate circuit (Either design or buy) and Im not going to bother. I'll charge my cells with me beside them so I can monitor them, one day Ill build a cutoff but for now its good enough. 

Most of the time you wont be charging from a flat battery (Or atleast I wont be) so waiting beside them shouldnt be too bad...
```

---
## \#8 Posted by: dg798 Posted at: 2018-01-07T20:09:39.274Z Reads: 98

```
do you know how I would build a cutoff for each cell
```

---
## \#9 Posted by: Hummie Posted at: 2018-01-07T20:40:02.819Z Reads: 87

```
There's single lipo cell chargers 
 but never have I seen one that did a decent current.  U could do one of those going into each cell's balance leads and the other sides all in parallel into some power supply.  U could have it all off the board and just a 13 prong plug into the board.
```

---
## \#10 Posted by: dg798 Posted at: 2018-01-07T20:41:37.080Z Reads: 84

```
is there a way for the drok module to cutoff at a certain voltage
```

---
## \#11 Posted by: dg798 Posted at: 2018-01-07T20:54:28.792Z Reads: 76

```
I read this on the questions section of amazon, someone wrote this as an answer to something:
This is a constant voltage & constant current converter. Which means it will supply the regulated current value until the constant voltage is reached. Thus if the voltage is set properly it will not overcharge an AGM battery. Just be aware that the battery will likely have to be isolated in some manner while charging or you will create a feedback situation where the converter runs & runs but never gets any charge to the battery. For a 145AH battery heed the note to provide additional cooling (a fan) when operating over 100W

does this mean I can just wait until the voltage is reached and the module will shut off automatically?
```

---
## \#12 Posted by: Hummie Posted at: 2018-01-07T21:15:27.145Z Reads: 72

```
Regardless of if it shuts off or not it doesn't matter. Similarly a psu without the drok thing will not shut off as it never gets quite to the voltage its set to
```

---
## \#13 Posted by: dg798 Posted at: 2018-01-07T21:28:43.393Z Reads: 68

```
so what do you recommend I do so I don't overcharge my packs??
```

---
## \#14 Posted by: Hummie Posted at: 2018-01-07T21:33:20.506Z Reads: 66

```
Just get the bulk power supply that does 8amps and adjustable 0-60 with the golden knob n has aoltage screen. Amazon or eBay .  set it so ur cells only hit 4.15 to be safe, n balance on the side at any time w "lipo discharge balancer". This is the cheapest and fastest charging method. No bms. N rely on the vesc low voltage cut-offs.
```

---
## \#15 Posted by: dg798 Posted at: 2018-01-07T21:35:03.757Z Reads: 66

```
the problem is I already ordered the drok thing and I have a BMS. What should I do??
```

---
## \#16 Posted by: Hummie Posted at: 2018-01-07T21:36:11.822Z Reads: 64

```
U have a power supply to go w drok?
```

---
## \#17 Posted by: dg798 Posted at: 2018-01-07T21:36:42.299Z Reads: 61

```
yes I have a 12v power supply which I will up with the drok
```

---
## \#18 Posted by: Hummie Posted at: 2018-01-07T21:39:40.571Z Reads: 61

```
U have nothing to worry about. Just don't overcharge any cells. Even if u set the supply to put 4.2 and the cells sit on that for days that's not a danger. It's not trickle charging and its a misunderstanding. Think it's float.    its the same as if the cells are at 4.20 n not on a charger
```

---
## \#19 Posted by: dg798 Posted at: 2018-01-07T21:41:06.331Z Reads: 62

```
it doesnt supply to each cell, you just set it to the total voltage no?
```

---
## \#20 Posted by: Hummie Posted at: 2018-01-07T21:43:26.997Z Reads: 63

```
Yea it just does the full pack n the bms likely does discharging of any cell that hits 4.2 simultaneously. 
Danger there is all the bms I see have a very low n slow discharge current when balancing so maybe slowly charge to full voltage the first time.
```

---
## \#21 Posted by: dg798 Posted at: 2018-01-07T21:44:18.727Z Reads: 51

```
well I bought a BMS for charge only.
```

---
## \#22 Posted by: dg798 Posted at: 2018-01-07T21:45:03.140Z Reads: 50

```
also when the drok sees it reached 50.4v total it will stop supplying voltage
```

---
## \#23 Posted by: Hummie Posted at: 2018-01-07T21:45:36.242Z Reads: 51

```
Yea and when it balances cells it likely is discharging the cells that hit 4.2

Don't know what j asking if anything else. Maybe the drok does cut off I don't know but typical from what I use is the current tapers way down n never gets to it
```

---
## \#24 Posted by: dg798 Posted at: 2018-01-07T21:47:23.237Z Reads: 51

```
is there a way to set it so that it doesn't discharge the cells when they reach full voltage
```

---
## \#25 Posted by: Hummie Posted at: 2018-01-07T21:49:06.491Z Reads: 54

```
Don't use a bms. But its just discharging so they stay lower than 4.2. Some are adjustable
```

---
## \#26 Posted by: dg798 Posted at: 2018-01-07T21:49:27.790Z Reads: 56

```
I already ordered one
```

---
## \#27 Posted by: dg798 Posted at: 2018-01-07T21:49:51.555Z Reads: 55

```
I have the bestech d140 12s BMS
```

---
## \#28 Posted by: dg798 Posted at: 2018-01-07T21:50:36.965Z Reads: 53

```
is there a way to set cutoff voltage from the drok itself maybe?
```

---
## \#29 Posted by: Hummie Posted at: 2018-01-07T21:56:15.100Z Reads: 54

```
don't know but what's the point if it's not harming the cells while it's slowly trickling to get to the 4.15 or whatever?
```

---
## \#30 Posted by: dg798 Posted at: 2018-01-07T21:58:10.045Z Reads: 53

```
no im just afraid it will overcharge the cells if im not constantly watching the voltage of each cell
```

---
## \#31 Posted by: Hummie Posted at: 2018-01-07T22:02:46.989Z Reads: 52

```
if you want to be personally watching each cell when charging that's beyond what people normally want to do and most people just trust the bms is doing it's thing correctly.   you can watch the cells come up using a multimeter or with the lipo balancer thing but the bms will discharge anything that gets too high and that's it's point.    
if you really want to be safe just charge so each cell should hit 4.1 max or something.   why don't you trust the bms?
```

---
## \#32 Posted by: dg798 Posted at: 2018-01-07T22:03:31.658Z Reads: 54

```
is there a way to calculate how long it would take to charge it at say 4 amps
```

---
## \#33 Posted by: Hummie Posted at: 2018-01-07T22:06:41.908Z Reads: 52

```
you can figure it but the level the pack is at would be a variable and getting it to do a constant 4amps till full charge doesn't seem to happen as all the supplies I've seen reduce their output when they get close to the set voltage.  you can get a close guess though, how many amp hours is your pack? why do you have worries?  are you planning to charge for long periods while you wont be there or something?
```

---
## \#34 Posted by: dg798 Posted at: 2018-01-07T22:07:58.314Z Reads: 51

```
the pack is 5.2 amp hours. sometimes im not home watching it all the time
```

---
## \#35 Posted by: Hummie Posted at: 2018-01-07T22:14:31.229Z Reads: 53

```
id get a steel filing cabinet and charge in that with it completely closed if youre not going to be around and check everything is good before you leave and trust that it'll be trickling with the constant voltage supply and constantly balancing with the bms.  charging while not around is frowned upon but if you set it up so the fire would be contained seems good enough to me.  
4 amps for 5.2 amphour dead battery I'm guessing would take like an hour.  5,2 amp hour...be 5.2 hours to charge at one amp rate roughly
```

---
## \#36 Posted by: dg798 Posted at: 2018-01-07T22:17:33.537Z Reads: 51

```
OK so im not usually away for long, like I might be how but forget its charging, but that's a good idea. Just one more question, can I use a multimeter and put it through the xt60 to see how much the pack is at?
```

---
## \#37 Posted by: Hummie Posted at: 2018-01-07T22:18:55.740Z Reads: 49

```
yea.........rythtrh
```

---
## \#38 Posted by: dg798 Posted at: 2018-01-07T22:20:05.390Z Reads: 51

```
OK thanks so much for your help, really appreciate it.
```

---
## \#39 Posted by: dg798 Posted at: 2018-02-15T14:28:54.423Z Reads: 47

```
Is there anyway to have the module shut off automatically once it’s done charging. The problem is I don’t have any red or green light telling me when it’s charging or when it’s full
```

---
## \#40 Posted by: Hummie Posted at: 2018-02-15T16:09:03.765Z Reads: 48

```
I don't know about the drok and maybe it could be never seen a power supply that does.  if you get one with the lcd screen (I have one that's new I can sell you in the usa) that will tell you the voltage youre at.  a wattmeter wired on is even better, but still wont shut off just end up putting out a hair's worth of amps once it reaches full charge.  actually it never reaches full charge and just ends up doing a very very small trickle charge while it sits on the supply but from what I read that's ok.   charge to 4.1 or 4.15 to be safe
```

---
## \#41 Posted by: dg798 Posted at: 2018-02-15T17:48:59.757Z Reads: 43

```
@Hummie It has an lcd. How many amps will it put out once it’s done. I put the voltage at 50v charging at 5 amps.
```

---
## \#42 Posted by: Hummie Posted at: 2018-02-15T18:19:31.959Z Reads: 44

```
U mean the drok I think and I'm not sure cause I don't have one but the bare pcu will get to 49v and then be forever tricking it in ...never hit 50v but get close.
```

---
## \#43 Posted by: dg798 Posted at: 2018-02-15T18:20:04.158Z Reads: 42

```
So what do I set the voltage for
```

---
## \#44 Posted by: dg798 Posted at: 2018-02-15T18:21:28.145Z Reads: 47

```
I have a 10s liion Charger which has an led. If I connect it to the drok will it turn green once it reaches 10s capacity or when it hits 50v through the module?
```

---
## \#45 Posted by: getyorma Posted at: 2018-02-15T18:25:12.913Z Reads: 45

```
I have created a video about this topic - i have a working DIY 6S balance charger using TP5000 modules, which are capable of 2A. [Link to video](https://www.youtube.com/watch?v=i8_XV5Yn7_s)
Do note that the video demonstrates the proof of concept of this idea with tp4056 modules. A 6s version follow up coming soon.
It is a really elegant way to balance charge large packs. The TP5000 modules have excellent efficiency and properties, it charges to 4.2v really precisely. Do note that this will probably be a bit more expensive compared to a BMS, BUT you can fix it if something goes wrong - it is very future proof and you could charge any amount of cells in series. Ie if you have a 3s drone, then you can use that to charge it via the balance lead.

Since i have a 12s board that is soon finished - i will be making a 12s version, also with a video update.
```

---
## \#46 Posted by: dg798 Posted at: 2018-02-15T18:25:56.685Z Reads: 41

```
I have a BMS already
```

---
## \#47 Posted by: getyorma Posted at: 2018-02-15T18:30:47.604Z Reads: 43

```
If you are going to use a boost converter with a BMS, you should look into low level arduino coding(unless you want to babysit the charger when it starts finishing). All you need to do is - measure the amperage going into the pack, once it gets low enough, the arduino just has to trigger a relay or a mosfet in order to stop charging. Leaving your battery floating on a charger is really dangerous and also degrades battery life a lot. A little read for you about charging lithium cells: [Link](http://batteryuniversity.com/learn/article/charging_lithium_ion_batteries)
```

---
## \#48 Posted by: Hummie Posted at: 2018-02-15T18:30:50.278Z Reads: 41

```
I don't know bout ur question w the psu and drok. I imagine the drok will override the psu setting.  If it were me I'd plug it in and see what happens. Use a multimeter to check.
```

---
## \#49 Posted by: dg798 Posted at: 2018-02-15T18:30:57.542Z Reads: 38

```
Gotta run to class, keep replying and will be back soon.
Thanks
```

---
## \#50 Posted by: Hummie Posted at: 2018-02-15T18:35:47.488Z Reads: 36

```
Can u link the specific details on the danger in float or trickle charging.  (Forget the term and are different).  I think there's confusion and as long as the voltage of the lithium cell doesn't go into a high voltage for too long and therefore be continuous plating its fine.  A cell at 4.2 is at 4.2 regardless of if connected to a power source and same risk so I read.
Plating or stalagmites or whatever they're called happen based on voltage and charge rate.  Trickle charging at 4.1 should be good all day
```

---
## \#51 Posted by: getyorma Posted at: 2018-02-15T18:46:06.162Z Reads: 37

```
[quote="Hummie, post:50, topic:43088"]
the danger in float or trickle charging.  I think there’s confusion and as long as the voltage of the lithim cell doesn’t go into a high voltage for too long and continuous plating its fine.  A cell at 4.2 is at 4.2 regardless of if connected to a power source and same risk so I read
[/quote]

Putting 4.2v indefinitely to a cell will destroy or damage it. Eventually, it will plate out and will burst into flames. I do not have a link for you but i can assure you it is not a good thing. Normal plating is fine, but when left floating on a charger the process will get faster, and by faster i mean a lot faster. Even if they dont explode, a similar pack that is charged normally will last longer and give better performance. In the end you will just lose more capacity and life from your pack - most if not all lithium ion chargers do this for a reason.
```

---
## \#52 Posted by: Hummie Posted at: 2018-02-15T18:52:19.627Z Reads: 33

```
If u can link evidence cause after discussion on endless sphere there was a diff conclusion.  And 4.2 is 4.2 regardless.
```

---
## \#53 Posted by: getyorma Posted at: 2018-02-15T19:21:47.709Z Reads: 35

```
Let's say you have used the cells with the charger for 6 months and no issue has occurred. But do note that lithium cells do not hold their original 4.2v full charge voltage when they get older, its going to be 4.16-4.19 volts depending how well the pack is kept in condition. Now if you are floating the cells 24/7 at 4.2 volts is going to be okay right? Wrong - the cells will start to heat up a tiny amount, but if combined with an enclosure it can get wild quick. The heat will make the chemical reaction even faster - therefore decreasing its life. [Link to a thing i googled up.](http://dolgin.net/Charging%20Lithium-Ion%20Batteries.html) It would be actually cool to make a video about this topic.
```

---
## \#54 Posted by: dg798 Posted at: 2018-02-15T20:26:24.979Z Reads: 34

```
Can you provide some more info on how to wire the arduino into the module? Is there a link where you found this idea. Seems like a really good one.
```

---
## \#55 Posted by: dg798 Posted at: 2018-02-15T20:28:30.348Z Reads: 38

```
And how would I know how many amps are right for when it’s done charging?
Also @Hummie, I want to test your theory as it would make life a lot easier but I don’t want to test something that may not work on my BMS and batteries. Is there any other way to test your theory?
```

---
## \#56 Posted by: getyorma Posted at: 2018-02-15T20:39:46.590Z Reads: 39

```
You will have to do the research yourself. You just need to make an arduino "amp meter" and combine that with a "relay switch" when the amperage gets low enough. I do not know when to cut off, but with the amp meter you can measure the amperage - babysit it the first time and keep an eye on the amperage, if it looks full write that amperage value down somewhere and use that in the code. Just turn the relay off (that disconnects the boost converter) if it detects the measured amperage - simple but genious. You could also measure voltage with it and report it on an lcd :smiley:
```

---
## \#57 Posted by: Hummie Posted at: 2018-02-15T21:15:11.172Z Reads: 36

```
in a situation where the batteries were old more so what happens in my experience is they get to the supplied voltage more quickly.  are you saying an older battery will not hold this 4.2 or even 4.1 and it will be turned directly to heat? 
https://endless-sphere.com/forums/viewtopic.php?f=14&t=83043&p=1218248&hilit=float+charging+lithium#p1218248
```

---
## \#58 Posted by: getyorma Posted at: 2018-02-15T21:30:26.692Z Reads: 33

```
I made an extreme case cenario. It could happen eventually though. A cell has to be really bad to heat up noticeably. 

As mentioned in that link you posted - they never got an answer that it is reccomended to do it. All the datasheets state that it has to be cut off in the end of the charging. You will need to find a research paper to prove this otherwise.

Some current will flow and it is not hard to avoid that. It saves energy and is safer - ie if one cell fails while left floating overnight - that could be bad. The cells are always safer kept separate. A car battery is better for that kind of usage.
```

---
## \#59 Posted by: Hummie Posted at: 2018-02-15T22:19:19.380Z Reads: 33

```
according to the link i put up it makes sense to cut the charge for a couple reasons: consumer wont wait forever for the green light saying fully charged as the last bit of a charge to 4.2 on CV will be very slow, also cells typically drop to around 4.15 as soon as pulled from a 4.2 supply and that is a bit safer voltage and will last longer as well, bu the voltage 4.2 is even arbitrarily decided...why not 4.19 or 4.21...and it depends on what trade-off of cycles vs capacity you want.  the danger of sitting on a 4.2 source would be the same as if the cell were overcharged at maybe 4.3 and then settled down.  the plating will be the same in either situation.  
in an instance of a bad cell that were self-discharging more than typical i think it would have to be practically a short to get enough discharged heat and in such a situation of having such a bad cell it would be the same situation off the cv supply with the paralleled cells beside it also feeding it current trying to bring it up to the higher voltage.  so i think but am just trying to figure it out based on what I read
```

---
## \#60 Posted by: PXSS Posted at: 2018-02-15T23:35:12.137Z Reads: 35

```
OH GOD! I feel bad for you. You have been sorely misguided. I have only read a few posts from this thread and @Hummie advice for you and can tell you that most of it is baseless. You should use a BMS, any self respecting engineer that deals with batteries for power delivery and storage uses a BMS. 

BMS are designed to protect battieries. There is a whole industry based on this technology. Hummie does not know better than the industry. 

Leaving batteries plugged in is bad. Batteries have self discharge. Leaving them plugged in is charging them. There is research into plating when batteries are left charging indefinitely. Research done by the big companies as well as government entities. If it was not an issue then manufacturers wouldn't specify a maximum charge time. 

Leaving batteries plugged in all the time with no BMS is how you end up with a board on fire. Just look at the hoverboard industry... They learned the hard way. 

I will read through your thread tonight and post my suggestions for any questions you've had and if you have more I will answer them to the best of my knowledge
```

---
## \#61 Posted by: dg798 Posted at: 2018-02-15T23:37:04.833Z Reads: 31

```
Please don’t say anything negative about @Hummie, he’s a great help.
@Hummie any ideas on what to test the 10s Charger with the module on besides for my batteries?
```

---
## \#62 Posted by: dg798 Posted at: 2018-02-15T23:45:21.224Z Reads: 28

```
@getyorma, is there some kind of module that could just shut off the drok automatically once it hits a certain current?
```

---
## \#63 Posted by: Hummie Posted at: 2018-02-16T02:05:28.729Z Reads: 29

```
wowzers.  too many drones maybe.  Its not just me trying to get to the reason why the big industry have the current cut off eventually even when it would just be a micro current when using just a CV.   if you read the last link I posted its with people who i would consider experts discussing it and I pull the info i gather mainly from there.  if you have a good reason why anyone does anything, instead of assuming its the best with no need for a reason, lets hear it.

and is a bms a safe haven?


it seems simply if youre above a high voltage of around 4.2 that's when significant plating is occurring, so if you want to sit all day and the next and next at 4.1 you tell me is that not safe?  if you have even a bum cell in parallel it is getting a constant microcurrent.  the constant low current doesn't seem an issue and its just the voltage.  sitting at 4.2 is going to destroy a battery more than it going to 4.2, than shutting off current till it self-discharges down to 4.1 or whatever, and then the charger kicks in and back to 4.2 repeatedly.  the difference seems the cell is not sitting at 4.2 where of course it takes more abuse and less cycles  but sit at 4.1 on a charger all day I'm open to hearing why not
```

---
## \#64 Posted by: dg798 Posted at: 2018-02-16T02:22:32.731Z Reads: 25

```
[quote="dg798, post:61, topic:43088"]
@Hummie any ideas on what to test the 10s Charger with the module on besides for my batteries?
[/quote]
i am home from school and ready to test but how would i know if the module overrides the charger?
```

---
## \#65 Posted by: PXSS Posted at: 2018-02-16T02:26:10.898Z Reads: 26

```
Alrighty! Your thread. GL
```

---
## \#66 Posted by: Hummie Posted at: 2018-02-16T02:26:30.228Z Reads: 27

```
you should get someone else to tell you and I don't have a drok.  ive already corrupted an innocent nubbie in some eyes with questions of whats safe.  i break stuff all the time and don't read instructions so what I would do is put the multimeter to the pcu and adjust the pcu till you get the voltage you want and then plug in the battery!  but id add a wattmeter in there in the future.  and check the cell voltages before you do it.  and watch them while doing it.
```

---
## \#67 Posted by: dg798 Posted at: 2018-02-16T02:27:15.917Z Reads: 28

```
how much is a basic watt meter that can cycle through all cells?
```

---
## \#68 Posted by: Hummie Posted at: 2018-02-16T02:30:06.058Z Reads: 28

```
a wattmeter will show what the voltage is coming from the pcu, (which will drop when you connect it to the pack and then they will come up to the initial voltage it was putting out without a load on it, almost).  it doesn't tell you about the individual cells.   to keep the cells balanced there are different ways done by bms or you could get a discharge balancer for 10$
```

---
## \#69 Posted by: dg798 Posted at: 2018-02-16T02:30:59.599Z Reads: 28

```
i just want to make sure i get to the right voltage. can i just use a multimeter?
```

---
## \#70 Posted by: dg798 Posted at: 2018-02-16T02:32:03.809Z Reads: 26

```
is there any place i can get a 12s brick power supply for 20 or under?
```

---
## \#71 Posted by: Hummie Posted at: 2018-02-16T02:33:16.648Z Reads: 26

```
if its good and proven accurate.  you could test it against your outlet in your house maybe.  ac.  or connect to cellphone battery at full charge, see if its at 4.15 maybe.  get two multimeters maybe or better yet get a wattmeter inline with the pcu and compare it to the multimeter.
```

---
## \#72 Posted by: dg798 Posted at: 2018-02-16T02:33:48.820Z Reads: 30

```
alrigh will take all into consideration.
```

---
## \#73 Posted by: Hummie Posted at: 2018-02-16T02:35:57.640Z Reads: 30

```
you can get one for 20$ somewhere for sure.  search for 48v power supply and get one that's "regulated".   but i forget the details on that.
```

---
## \#74 Posted by: dg798 Posted at: 2018-02-16T02:36:28.894Z Reads: 29

```
ok looking now
```

---
## \#75 Posted by: dg798 Posted at: 2018-02-16T02:38:50.045Z Reads: 29

```
like this?http://www.ebay.com/bhp/48v-power-supply
```

---
## \#76 Posted by: Hummie Posted at: 2018-02-16T02:42:48.889Z Reads: 30

```
https://jet.com/product/detail/b61d6b8b5b524af1a3693e5872f49ccb?jcmp=pla:bng:nj_gen_electronics:electronics_adaptors_cables_power_other:na:PLA_333105205_1222657059503198_pla-4580015686348761_c:na:na:na:2PLA15&pid=kenshoo_int&c=333105205&is_retargeting=true&clickid=2e9b538d-c2ac-4320-bf34-806cd0e960c6&msclkid=29a2563705951b5b968c0cb1466a1f20

cheap.  but i have a 500 watt one like this
https://www.aliexpress.com/item/48-volt-power-supply-110V-220V-AC-to-36V-DC-5A-240W-single-output-48v-Switching/32787481279.html?spm=2114.search0104.3.1.72d2dc34Zfe8QW&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10151_10065_10344_10068_10130_10324_10342_10547_10325_10343_10546_10340_10548_10341_10545_10084_10083_10618_10307_5722316_5711213_10313_10059_10534_100031_10629_10103_10626_10625_10624_10623_10622_10621_10620_10142,searchweb201603_25,ppcSwitch_2&algo_expid=5a417cbe-d779-4a2d-906d-cbee2521a299-0&algo_pvid=5a417cbe-d779-4a2d-906d-cbee2521a299&priceBeautifyAB=0

that i'll sell you for 30$ but it does 500 watts.  i have too many of these and opt for the lucky golden knob one with lcd i just got going that shows the voltage.  its 60$ and have one in the box extra.
```

---
## \#77 Posted by: dg798 Posted at: 2018-02-16T02:44:13.539Z Reads: 30

```
the one from ali express, how would i know when its done charging?
```

---
## \#78 Posted by: Hummie Posted at: 2018-02-16T02:47:19.522Z Reads: 27

```
haha it's never done.  put the multimeter up to it if you want.  but if you get a 48v supply it will only put the cells to a maximum of 4.0 a cell (assuming theyre all balanced) ...so you end up with maybe 80% of the full potential charge but get like 5x the cycles out of the cells and they are much safer at full charge or while charging.  

it will peter down to a very low current when it is at the "end" of charging.
```

---
## \#79 Posted by: dg798 Posted at: 2018-02-16T02:48:12.600Z Reads: 28

```
got it. im gonna go off and do some more research
```

---
## \#80 Posted by: dg798 Posted at: 2018-02-16T03:35:08.826Z Reads: 34

```
Would this work?  https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F122518141083
```

---
## \#81 Posted by: dg798 Posted at: 2018-02-16T03:36:35.673Z Reads: 35

```
Or this?
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F272666880424
```

---
## \#82 Posted by: ZackoryCramer Posted at: 2018-02-16T05:16:29.964Z Reads: 36

```
No. Those are power supplies with output of only 48v. To fully charge a 12s you need a 50.4v supply.
```

---
## \#83 Posted by: Hummie Posted at: 2018-02-16T06:17:25.084Z Reads: 36

```
yes it works and will put you at like 80% of full charge, and your cells will last like 4 times as many cycles, and you'll be safer with less worry about balancing while charging.  

there was a group buy here where they got the manufacturer to put it to 50v I think, but the standard 48 is good for getting enough juice in to get home maybe.  49.2v id like.
but go for more amps and spend more bucks.
```

---
## \#84 Posted by: dg798 Posted at: 2018-02-16T14:44:03.566Z Reads: 36

```
Alright i found a god one for cheap and it has protection features and led indicator for charging.
Look what I found on AliExpress
https://www.aliexpress.com/item/32836644573/32836644573.html
```

---
## \#85 Posted by: dg798 Posted at: 2018-02-16T14:45:53.306Z Reads: 34

```
Do you think it’s a scam?
```

---
## \#86 Posted by: Hummie Posted at: 2018-02-16T15:50:43.153Z Reads: 34

```
ive seen that one rebranded for sale.  don't think its a scam.
```

---
## \#87 Posted by: dg798 Posted at: 2018-02-16T17:13:14.185Z Reads: 32

```
Is it worth it?
```

---
## \#88 Posted by: Hummie Posted at: 2018-02-16T17:16:44.826Z Reads: 34

```
http://vruzend.com/product/48v-lithium-ion-battery-charger-3-amps/

here it is again I think

pretty cheap.  but id go for at least 5 amps or ...if you're being cheap get mine for 30$ and it does 8 amps!!
```

---
## \#89 Posted by: dg798 Posted at: 2018-02-16T17:36:27.183Z Reads: 34

```
is there a way to calculate how long it would take to charge at x amount of amps?
```

---
## \#90 Posted by: Hummie Posted at: 2018-02-16T19:17:47.291Z Reads: 34

```
lets say its a 5ah battery,  so 5 amp hours,  5 amps continuously for an hour is what it can put out if fully charged, so if its empty and you charge with a 5amp charger it will take an hour pretty much to go from what they consider empty to full.
```

---
## \#91 Posted by: dg798 Posted at: 2018-02-16T19:21:44.544Z Reads: 33

```
alright thanks!
10 charc
```

---

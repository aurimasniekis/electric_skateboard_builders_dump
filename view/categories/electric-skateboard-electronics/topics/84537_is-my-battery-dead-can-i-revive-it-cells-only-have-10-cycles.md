# Is my battery dead ? Can I revive it ? Cells only have 10 cycles

### Replies: 51 Views: 664

## \#1 Posted by: ElskerShadow Posted at: 2019-02-18T10:41:41.515Z Reads: 160

```
I thought I had done everything right ! 
I left the battery sit at 36 V for winter. 
When I go to check on the battery since sun came back
I was at only 2,35 volt..... 
Each cells are wether at 0 v or 0,35 v 

There's nothing I can do right ? Like all those brand new 30Q cells must go to trash ? 
![IMG_20190218_113543|666x500](upload://mkIYgsrvuUFS3wkyn76up3bK7vZ.jpeg)
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-02-18T11:01:43.442Z Reads: 154

```
Was it connected to voltage meter / vesc/ antispark? Mines been sitting in my closet just chilling for the last 5 months... Nothing has happened 🤔
```

---
## \#3 Posted by: TowerCrisis Posted at: 2019-02-18T11:35:06.594Z Reads: 152

```
Lithium based batteries do not get damaged solely from being over discharged.

What will kill a lithium cell is pulling reasonable amounts of power at low voltages. When this happens the electrolyte will "offgas" and build up pressure within the cell. This is what causes prismatic cells to puff. Internal resistance will increase as voltage drops, and any drawn power will cause electrolyte decomposition.

Luckily for you, these cells were not under load at such a low voltage. They simply discharged VERY slowly. This probably did not damage them.

Do NOT try to power anything with them, as this could cause instant permanent damage.

You can likely recover these cells. You'll need a non-standard charger like a bench power supply that can do CCCV.

Set the voltage to your max pack voltage, and limit the current to 0.25 - 0.5A. The lower you set this, the higher the likelyhood of recovery and the slower the pack will charge. You can do the math regarding how long it would take to charge (5Ah pack at 0.5A would take 10 hours, etc)


You also have the option of charging each P group individually by using the same current settings but setting your voltage to 4.2V. I would highly recommend this over charging the whole pack at once as your series groups are likely out of wack.

Did you say some are at 0V and some are at 2.35?

If they are actually at 0V then those P groups are toast. And you won't be able to replace them with new cells as the new cells wouldn't match well with the other recovered ones.

I'm hoping the 0V was just a measurement error. Could you give a detailed list of all the P group voltages?

If the cells are seriously that out of wack, then your BMS is probably what caused it and is toasted.
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-02-18T11:44:58.799Z Reads: 134

```
They just need a little nap :D 

![pfFhISq|480x384](upload://k8PW6gpf97DTUe7pmI0s5mLoER3.gif)
```

---
## \#5 Posted by: ElskerShadow Posted at: 2019-02-18T12:57:35.962Z Reads: 123

```
Thanks for the reply guys.

To clarify : the whole pack is at 2,40 v 
Each P group is between 0,34 and 0,45 V 

The only charger I have are regular ones, and a 4S lipo charger... 
What should I buy to restore this battery ? All the cells are brand new it would be a shame not to try to revive them. 

The battery was sitting with just an antispark plugged into it.. maybe that's the culprit
```

---
## \#6 Posted by: SeVeSeventyOne Posted at: 2019-02-18T14:06:20.999Z Reads: 114

```
What I would do is to try to charge each individual group separately with some power supply with limiting resistor in between. Take any 5V power supply (like USB power supply) and add a resistor in between say 50ohms will max pass 100milliAmps, Add a mutimeter to check the voltage that it will never exceed 4.2V in a cell. When you have reach say 3.7Volts, you can start charging the next group untill all groups are 3.7Volts. Then you can start charging the pack normally. Some chargers refuse to charge empty cells.
```

---
## \#7 Posted by: ElskerShadow Posted at: 2019-02-18T15:26:35.937Z Reads: 112

```
![IMG_20190218_154518|375x500](upload://6ERT21BoKrO1iwnJxByAlOny7qn.jpeg) 
I have tried with my lipo charger... No luck it says low voltage and won't charge
@TowerCrisis BMS is charge only 

Whole pack voltage : 3,30v at charge port and 4,14 v at output
P1 - : 00,28 v
P2: 00,28v
P3: 0,28v
P4: 00,44v
P5: 00,45v
P6:00,46v
P7:00,47v
P8:00,48v
P9:00,48v
P10 +: 00,48v
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-02-18T15:34:02.611Z Reads: 106

```
use nihm to boost up the voltage than use lipo mode to charge to full,
```

---
## \#9 Posted by: ElskerShadow Posted at: 2019-02-18T15:37:17.899Z Reads: 104

```
I have tried and I can charge with nihm charging at 0.1 V and voltage instantly raised at 1,23 v for P1
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-02-18T15:38:06.833Z Reads: 104

```
than use nicd and try again or increase the amps but dont do it for too long.

youve gotta be fast

as soon as the group hits 3v switch to lipo immedieatly
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-02-18T15:42:03.673Z Reads: 102

```
I dont mean to be rude Alan but are you sure you can give advice about this kind of thing? I dont want this to result in an even more broken pack
```

---
## \#12 Posted by: ElskerShadow Posted at: 2019-02-18T15:42:32.504Z Reads: 103

```
Yeah I have to be fast before the voltage drops again ? 
I am currently charging P1 at 0,2 amps to avoid any stress on the cells. 
P1 went from 0,28 to 1,79 v in a few minutes of charging
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-02-18T15:43:30.515Z Reads: 99

```
[quote="ElskerShadow, post:12, topic:84537"]
before the voltage drops again ?
[/quote]

yeah the voltage drops really fast, the nicd part is used to trick the charger.
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-02-18T15:44:50.915Z Reads: 103

```
[quote="Sn4pz, post:11, topic:84537"]
are you sure you can give advice about this kind of thing
[/quote]

yes defiantly, i trust myself, but i usually do it on my trusty icharger 1010b+

^revived a lot of dead laptop cells
```

---
## \#15 Posted by: Sn4pz Posted at: 2019-02-18T15:46:18.075Z Reads: 99

```
ah ok, lol

good luck esker :( seems like antisparks are becoming a winter parasite for esk8 :rofl:
```

---
## \#16 Posted by: ElskerShadow Posted at: 2019-02-18T15:47:49.763Z Reads: 100

```
Yeah I was so joyful at the idea of riding this board again ! I guess I have to stick with my other builds for now. 
I already see myself spend the week looking at this charger, hoping I won't have to build a new battery :/
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-02-18T15:47:50.314Z Reads: 101

```
Do you have a lab bench power supply? if so reviving can be much easier...
```

---
## \#18 Posted by: ElskerShadow Posted at: 2019-02-18T15:48:22.621Z Reads: 99

```
I wish I had, I want to buy one since months but never took the plunge. Now I regret hahah
```

---
## \#19 Posted by: ElskerShadow Posted at: 2019-02-18T15:49:13.533Z Reads: 99

```
BTW do you have a good one not too expensive to recommend ?
```

---
## \#20 Posted by: AlanZhou Posted at: 2019-02-18T15:49:38.326Z Reads: 93

```
cant recommend one, as my i charger does the trick most of the time.

you know you can charge at higher amps for shorter periods right (chances are that will boost the voltage up higher and faster)

^not recommend

and why not take the pack apart and do each cell individually? chances are one or two cells are damaged.
```

---
## \#21 Posted by: Sn4pz Posted at: 2019-02-18T15:53:27.147Z Reads: 89

```
This is certainly a @Namasaki question. good luck!
```

---
## \#22 Posted by: ElskerShadow Posted at: 2019-02-18T19:19:18.816Z Reads: 83

```
I better do each P and see afterwards I definitely don't want to unweld and spot weld everything again. I hope I have no dead cells on the pack. But from what I've seen none are dead. 
I already charged the first P to 3,7 volts without issue 
I LL keep doing that to each P tomorrow
```

---
## \#23 Posted by: Arek Posted at: 2019-02-18T19:30:38.781Z Reads: 82

```
If for nothing demanding, like just charging batteries, you can buy whatever bench power supply you find as long as it has 60V/5A output or two 30V outputs which can you connect in series and obviously full control of voltage and current.
Preferably switching one which won't be heavy like traditional linear one.

I'm currently using MCH-K305D and Agilent E3647A.
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-02-18T19:36:01.515Z Reads: 82

```
damaged cells dont show unless you test em, damaged cells could be one cell damaged draining the p group slowly.
```

---
## \#25 Posted by: KaramQ Posted at: 2019-02-18T19:40:06.764Z Reads: 84

```
Do you have a treadmill, if so attach it to some sort of build, run it on a treadmill for about half an hour, and you’ll be good to go
```

---
## \#26 Posted by: TowerCrisis Posted at: 2019-02-18T19:45:28.958Z Reads: 86

```
No no no no! So many bad ideas recommend in this thread.

The ONLY way you can do this safely and with control is with a bench power supply, charging each P group individually.

If you don't have one, get one. This is definitely not the last time you'll use it.
```

---
## \#27 Posted by: maxchilton Posted at: 2019-02-18T20:13:38.096Z Reads: 83

```
Yup. i've done this before, setting the charger to nimh/nicad, charging the lithium pack for a 5-10 seconds to get voltage just high enough for the charger to detect, once detected, switch to lithium mode and charge as normal.
```

---
## \#28 Posted by: ElskerShadow Posted at: 2019-02-18T22:26:38.018Z Reads: 79

```
I've reached 3,28v with this technique but I still get the low voltage error from the charger, weird
```

---
## \#29 Posted by: Namasaki Posted at: 2019-02-19T04:35:27.057Z Reads: 76

```
This would be a very good time to invest in a Lab Power supply.
And as @TowerCrisis suggested, it will come in very handy more than once.
I got one and it is all I use for maintenance, testing and even daily charging.
Once you've used a Lab supply, you'll never want to use a brick charger again except for portable charing.
If you don't want to go all out, you can save some money with a 60v 3a supply.
https://smile.amazon.com/KORAD-KA6003P-Programmable-Precision-Adjustable/dp/B00AXL7UJA/ref=sr_1_5?crid=2XZUETEPZWOCJ&keywords=korad+power+supply&qid=1550551051&s=gateway&sprefix=korad+%2Caps%2C184&sr=8-5
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-02-19T05:20:22.472Z Reads: 73

```

[quote="Namasaki, post:29, topic:84537"]
you’ll never want to use a brick charger again
[/quote]

Well except for lipos, cell balancing via the charger
```

---
## \#31 Posted by: Namasaki Posted at: 2019-02-19T06:29:07.168Z Reads: 70

```
[quote="AlanZhou, post:30, topic:84537"]
Well except for lipos, cell balancing via the charger
[/quote]

Let me clarify, I meant on any system with a bms.
```

---
## \#32 Posted by: sk8l8r Posted at: 2019-02-19T07:36:01.572Z Reads: 65

```
[quote="TowerCrisis, post:26, topic:84537"]
The ONLY way you can do this safely and with control is with a bench power supply, charging each P group individually.
[/quote]

You could use a single P usb powered charger, it's what I use a is really safe
```

---
## \#33 Posted by: ElskerShadow Posted at: 2019-02-19T07:47:30.728Z Reads: 62

```
Bought it, paid 50 $ in shipping but it'll be worth it !
```

---
## \#34 Posted by: TowerCrisis Posted at: 2019-02-19T07:51:44.807Z Reads: 61

```
It's possible but I would advise against it, as you have no control over the current.
```

---
## \#35 Posted by: mishrasubhransu Posted at: 2019-02-19T08:02:08.599Z Reads: 60

```
Yeah, I have revived slowly discharged cells too. Just connect them to hobby charger(with nimh mode) and charge at a low current like 100mA/cell, until a parallel group reaches 3.1V or so, then charge on a regular li-ion charge. 

I have a hobbyking charger that does the job
```

---
## \#36 Posted by: ElskerShadow Posted at: 2019-02-19T08:03:19.753Z Reads: 58

```
I have done exactly that but even after reaching 3.1 v I dunno why the lipo charger still says low voltage error. 
I will check again this morning
```

---
## \#37 Posted by: mishrasubhransu Posted at: 2019-02-19T08:04:32.258Z Reads: 57

```
Go higher then.
```

---
## \#38 Posted by: b264 Posted at: 2019-02-19T08:07:10.408Z Reads: 60

```
[quote="ElskerShadow, post:5, topic:84537"]
The battery was sitting with just an antispark plugged into it… maybe that’s the culprit
[/quote]

Which antispark?
```

---
## \#39 Posted by: sk8l8r Posted at: 2019-02-19T08:58:00.507Z Reads: 58

```
True, you can't control it - at least not found one yet you can.

But for someone who is lacking equipment it's really cheap and feels pretty safe if you monitor it closely
```

---
## \#40 Posted by: ElskerShadow Posted at: 2019-02-21T14:52:29.433Z Reads: 58

```
Push to start antispark from @Martinsp  couldn't even use the push to start function he sent me some faulty units still waiting for an answer from him since both I bought are useless
```

---
## \#41 Posted by: ElskerShadow Posted at: 2019-02-21T14:56:02.536Z Reads: 57

```
I have bought the recommended power supply 
I recieved it today and I did the silliest mistake, didn't switched the unit to 220v 
When turned On I heard a BUZZzzz inside the unit and since then it's a brick. 
I don't see any internal damage... Have I fried the thing ? I hate myself sometimes... Money thrown away 
![IMG_20190221_155059|666x500](upload://jX0AGjaSkjond39j23nU5a3DkDx.jpeg)
```

---
## \#42 Posted by: Hummie Posted at: 2019-02-21T15:34:02.824Z Reads: 55

```
The flipsky push to start ruined my lipos!
```

---
## \#43 Posted by: nuttyjeff Posted at: 2019-02-21T15:36:21.508Z Reads: 54

```
There should be a fuse at the back. Try replacing it.
```

---
## \#44 Posted by: ElskerShadow Posted at: 2019-02-21T15:50:24.329Z Reads: 50

```
Yeah I was looking for that ! 
But I can't find any fuse like there's on my spot welder for instance
```

---
## \#45 Posted by: deucesdown Posted at: 2019-02-21T16:21:12.459Z Reads: 50

```
Wow sorry to hear that! These are nice convenient supplies.

https://www.eevblog.com/forum/blog/eevblog-314-korad-ka3005p-psu-teardown/?action=dlattach;attach=36975;image

The power plug looks like the ones with integrated fuse holders, check it?
```

---
## \#46 Posted by: ElskerShadow Posted at: 2019-02-21T16:58:49.097Z Reads: 48

```
You were right, under the plug there was a little cavity with the said fuse ! 
Fortunately I had some spare from my sunkko spot welder so it's up and running 
I am charging the last P Group ! 
Almost there to revive this pack :) 
![15507681998697288840117398906408|375x500](upload://53jYlXj7VbgrgQ6qzzqdiVValf7.jpeg)
```

---
## \#47 Posted by: Namasaki Posted at: 2019-02-21T17:05:07.327Z Reads: 47

```
Sooooo glad to hear that there was a fuse to save the day!
```

---
## \#48 Posted by: TowerCrisis Posted at: 2019-02-22T10:55:26.650Z Reads: 43

```
So glad to see that it'll be up and running! Make sure to update us regarding cell balancing and what kinda range you're getting.

One last note, before you take it for a full ride please check if the cells are discharging evenly, take it for a few 100 meters then recheck the cell voltages. If there's a bad group you'll notice a voltage drop. Personally I would do this several times before trusting it.

Best of luck!
```

---
## \#49 Posted by: nuttyjeff Posted at: 2019-02-22T11:08:13.477Z Reads: 42

```
Perfect! Just wasted money for a fuse :stuck_out_tongue: Hope you get your battery working again.
```

---
## \#50 Posted by: ElskerShadow Posted at: 2019-02-22T13:38:46.710Z Reads: 37

```
I LL share the results when I am done . I have charged each group to 3.2 v at 0.3 Anow I am doing a second round and charging them to 3.7v at 0.5a

Thanks for the tip. I will do that a few times before trusting the pack again, if you had to take a guess will I lost a lot of capacity ? It's only a 10S3p so if I lose a lot of capacity I will really feel it, as long I don't sag i'm fine :p
```

---
## \#51 Posted by: deucesdown Posted at: 2019-02-22T14:32:31.888Z Reads: 32

```
The danger is the damage if any is unlikely to uniform across all the cells. I think your chances are really good though.
```

---

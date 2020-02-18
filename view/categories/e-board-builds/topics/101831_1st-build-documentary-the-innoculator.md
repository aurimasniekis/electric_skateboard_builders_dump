# 1st Build documentary. The Innoculator

### Replies: 37 Views: 1228

## \#1 Posted by: turbolovah Posted at: 2019-09-16T00:24:04.471Z Reads: 254

```
After much research and consideration I have finally decided to pull the trigger and buy parts for my DIY.
I will be documenting the entire build on this thread, with links to parts, and actual prices paid including shipping to help others who are considering their first build.

Backstory:
Have wanted to make a DIY from the beginning, but because of budget constraints at the time, I bought a Meepo V2 (late 2018 29mph version). I loved my Meepo, but after about a thousand miles my motor bearing shell has broken apart to an almost unusable state, and instead of replacing the motors I am using it as an excuse to start my DIY :blush:

Build:
This build is ongoing, and it is meant to be as cost effective as possible so parts will be recycled.
I am making this board almost entirely out of @dickyho parts, because they seems to be the most cost effective and are frequently used and tested by other members of the community. I am using my existing Meepo deck until I can find another one that I like enough.


Trucks, mounts, and pulleys: $134 shipped
I chose Dickyho's single motor kit drive kit with wheels as well as his motor mount kit for the 2nd motor
https://www.ebay.com/itm/DIY-single-motor-drive-kit-for-electric-skateboard-97MM-wheels-without-motor/302690518618?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

https://www.ebay.com/itm/DIY-electric-skateboard-parts-pulleys-and-motor-mount-kit-for-83-90-97MM-wheels/323277743059?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

Motors: $112 shipped
I chose to purchase 2 Dickyho 6374 motors at 200kv
https://www.ebay.com/itm/6354-6364-6374-6384-150-170-200-230-270KV-High-Efficiency-Brushless-motors/303074535503?ssPageName=STRK%3AMEBIDX%3AIT&var=602007163507&_trksid=p2060353.m2749.l2649

Deck: "Free"
Meepo V2 deck

ESC: $89 shipped
I purchased 2 Mini Flipsky VESC 4.2s from Aliexpress for $89 shipped (A freaking steal). They claim it is being shipped from the USA (where I am) so shipping is an estimated 4-7 days. I am weary of this as this seems like a too good to be true type situation, but as aliexpress does have buyer security, I figured I would take the gamble.
https://www.aliexpress.com/item/4000122043995.html?spm=a2g0o.cart.0.0.45d33c006irGVL&mp=1

Battery "Free" (so far)
This is the part I will get flamed about haha. I am recycling my 10s2p samsung 20r pack from my Meepo, and might buy my buddy's 10s2p samsung pack to make a 10s4p 20r pack. I know these are not ideal cells and will sag like hell, but it's what I got until I can make some money to buy some 30q or vtc4 cells.


Remote: I have no clue what remote to get yet, I am looking for the most budget friendly thumb roller option.

I will update this page as parts come in, super excited to start!!
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-09-16T00:28:53.919Z Reads: 220

```
For the esc you should have gotten the 4.12, the 4.2 has cutout issues.

https://www.aliexpress.com/item/4000110350979.html?spm=a2g0o.productlist.0.0.57cc264bBBl2mM&algo_pvid=dc456579-470f-4d12-aff6-e6e1a24efd56&algo_expid=dc456579-470f-4d12-aff6-e6e1a24efd56-0&btsid=ed51d442-f971-423c-8338-f9dbd6ecdd94&ws_ab_test=searchweb0_0,searchweb201602_10,searchweb201603_52
```

---
## \#3 Posted by: turbolovah Posted at: 2019-09-16T00:43:25.976Z Reads: 208

```
I was under the impression Flipsky fixed this in late March by changing the resistors they used.
```

---
## \#4 Posted by: BillGordon Posted at: 2019-09-16T03:22:04.228Z Reads: 197

```
They did, but no telling which batch these come from. @Gamer43 or @Schtekarsten might be able to shed some light.
```

---
## \#5 Posted by: Halbj613 Posted at: 2019-09-16T06:18:08.320Z Reads: 183

```
isnt there a problem with the batteries if they dont have the same mileage

wont there be a problem with putting them in parallel

also what would be really cool is to wire the charge port in parallel and then go and power each vesc seperately with one of the two packs
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-09-16T08:37:00.297Z Reads: 167

```
@Halbj613  you can use old and new cells, but each group should have same amount of old and new cells compared to other groups. for example, if you have used 12s4p and you want to upgrade to 12s6p, you will add in each 4p group 2 new cells, so each group will be made of 4 old and 2 new cells. and ofcourse before connecting old and new cells in parallel, they MUST be at same voltage. 

@turbolovah  if you have two assembled battery pack, each with its own bms, why not just connect them in parallel?  you won't have to disassemble anything. maybe I understood you wrong and you plan to connect them in parallel? however, if they don't have bms or you are not sure, just be careful that batteries are on same voltage before connecting them.
```

---
## \#7 Posted by: turbolovah Posted at: 2019-09-16T14:59:17.259Z Reads: 150

```
@Tinp123 hey thanks for the advice! His bms blew, so I am either recycling his cells for a new large pack, or installing a bms and running in parallel. Depends on if he is willing to sell it to me or not.
```

---
## \#8 Posted by: Schtekarsten Posted at: 2019-09-16T20:41:00.319Z Reads: 148

```
yeah they made the swap late mars, but it looks like there is a reseller selling the esc so who knows, it might have sat on a shelf for a while. only way to find out I guess is having a looksy. the new resistors (8 of them) should say 47 (47 ohms) and the old ones 4h7 (4.7 ohms). I guess you could ask the reseller to have them check the values. but good luck with that :joy:
either way I made a little video in my thread where I explain how you can swap them out yourself:
https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824
```

---
## \#9 Posted by: turbolovah Posted at: 2019-09-16T21:17:57.572Z Reads: 127

```
@Schtekarsten I read the whole thread and watched your video, GREAT stuff! I already bought the things so I won't bug the seller, I doubt they would understand me anyway 😂. I will definitely do the resistor swap if need be though, gives it a little more DIY magic in my book. It does make me wonder what kind of bulk these aliexpress sellers purchase in if they still have stock from 6 months ago though.
```

---
## \#10 Posted by: turbolovah Posted at: 2019-09-16T23:50:00.585Z Reads: 120

```
Question:

Does anyone know if I can reverse mount with these @dickyho mounts? Judging by the picture I believe these to be the long mount version, but suddenly i'm unsure.
```

---
## \#11 Posted by: Z408 Posted at: 2019-09-17T00:37:27.295Z Reads: 112

```
Just bought the same kit but the dual version, per @dickyho, he said it was possible.
```

---
## \#12 Posted by: turbolovah Posted at: 2019-09-17T00:39:14.284Z Reads: 113

```
Yea, I just saw some people do it over on this thread https://www.electric-skateboard.builders/t/new-designed-a-motor-mount-for-sale-looking-for-review/59212/635
```

---
## \#13 Posted by: turbolovah Posted at: 2019-09-19T18:00:55.215Z Reads: 116

```
So now I'm shopping for an antispark switch, I really want the push to power on function so I'm looking at flipsky's smart anti spark, but the description says that it has a max voltage of 10s, but then it states 13s for 4.12 vescs. Since the 4.2 is based on on the 4.12 will this work? Flipsky has informed me that they just got samples in and could ship me 1, but i dont want to buy it if its gonna blow up when I transition to 12s. (Which is looking like it will be pretty soon)
https://flipsky.net/collections/accessories/products/antispark-switch-smart-280a
```

---
## \#14 Posted by: wwohl602 Posted at: 2019-09-19T18:55:00.742Z Reads: 99

```
I was recently recommended this one: [Anti spark switch ](https://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/31847)
```

---
## \#15 Posted by: turbolovah Posted at: 2019-09-20T18:25:31.069Z Reads: 108

```
So I went ahead with the Flipsky smart antispark, looks like i am literally the first person to buy this switch. Wish me luck! If it fails i will go to loopkey.

I went a little crazy last night, and spent way too much money. This budget motor fix is getting expensive haha.
Here is the damage

48 LG HG2 cells $200 shipped

Flipsky smart antispark $50

Flipsky VX1 remote $50

4mm bullet connectors $6

Y type cable for battery to vesc $6

Canbus connector $2

Shipping from flipsky $30

Red carbon fiber vinyl wrap 24'x60' $8

12 guage copper wire $5

Red and black 1/4" sleeve $7

Griptape $8

I'm making a DIY spot welder out of a car battery so those parts are:

Motorcycle starter solenoid $10

2 guage wire $7

Momentary button $4

Still have to get some copper nails from home depot for the electrodes, and I'll 3d print an electrode holder to keep em stationary.

Thinking about migrating this post to the new forum. Any thoughts?
```

---
## \#16 Posted by: turbolovah Posted at: 2019-09-21T03:47:30.229Z Reads: 100

```
Update: I just purchased a 12s 20 amp smart bms $35 shipped. I got the 20A version because it was cheap and I am bypassing anyway. I purchased it from here
https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/

Any concerns I should have with this bms on my setup?

I also bought a 50.4V 4amp battery charger for $27 on ebay
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F283494884774
```

---
## \#17 Posted by: turbolovah Posted at: 2019-09-21T09:35:55.602Z Reads: 104

```
Oh boy, I did it again..... i bought another thing.....

$35 --- $44 shipped

I think it's a steal
https://www.skateshred.com/wholesale-blank-longboard-decks/40-x-10-drop-through-blank-deck.html?gclid=Cj0KCQjwlJfsBRDUARIsAIDHsWq0uRe5bs0nHeC6JcOB7Gozf6N-fwqYzXIZPvyKzrWDfwiYIAFCgfgaAiTXEALw_wcB
```

---
## \#18 Posted by: turbolovah Posted at: 2019-09-21T23:20:46.989Z Reads: 101

```
Update

The Meepo v2 motor is on its last leg 😭![20190919_093356|281x500](upload://7LGGH33HT2hGAdtGvdE7CmSFWwf.jpeg) 
![Screenshot_20190921-161501|281x500](upload://n7akoI63ohcre1JAjkzISO8EaNu.jpeg) 

My parts can't get here fast enough
```

---
## \#19 Posted by: Lockstah Posted at: 2019-09-23T02:12:52.812Z Reads: 87

```
I feel you brother been waiting 4 weeks on a motor mount to complete my 1st build ..
```

---
## \#20 Posted by: turbolovah Posted at: 2019-09-24T21:20:22.967Z Reads: 81

```
Wooo, the skateshred deck is here and it looks gorgeous, the concavity feels great under the feet.

![Snapchat-1471374932|281x500](upload://bIK2AmTXy51iYIQko4aqJfTxVSo.jpeg) 

The vinyl and griptape have also arrived so I know what I'm doing tonight!
All of the spot welder parts have arrived, and the HG2s are arriving today as well, so I'll be making my battery pack tomorrow.

Still waiting on my motors, mounts, pulleys, and vescs. I'm gonna decide what to do about an enclosure tomorrow.

Contemplating swapping my meepo hardware over to the new deck while I wait. I was able to epoxy parts of the meepo hub back together and I am currently riding the shit out of it still. Surprisingly smooth with an epoxied casing. No noise or balance issues

I bought a kayak handle for $7 and some really nice m6 enclosure bolts and washers for $10. I bought m6 inserts for $6 as well.

Im trying to be as through as possible documenting all of my spending, admittedly probably to keep track of it myself,  but hopefully it helps others to understand that all of the little things add up.
```

---
## \#21 Posted by: turbolovah Posted at: 2019-09-27T17:11:15.217Z Reads: 69

```
Ok, so I've done alot since the last post. 
Too tired for words, the pictures will explain....

![20190924_214443|281x500](upload://cNvArENo1gueXEworgaFZlR5Yl.jpeg) 

![20190924_222011|281x500](upload://acWhF8XapbjtTwNO3mh9igNMT4T.jpeg)

![20190924_231159|281x500](upload://7muGAh1tKs4GqoXIaBwSs7NtmUs.jpeg)

![Snapchat-797982429|281x500](upload://gO7dU75sbpKGxfds6RFvXEs84fQ.jpeg) 

![20190926_191307|281x500](upload://sx37zW2FyP29fo4FBUpphrHW5cz.jpeg) 

![Snapchat-929361331|281x500](upload://5OMKeUe0vZkrIRuYESuUS5JYlO5.jpeg) 

![Snapchat-1197405842|281x500](upload://zPu291RYgBwqajSMdfn1WPbZn7e.jpeg) 

Vescs finally came in,  now I'm just waiting on bms and charger. I'm president of the eskate club at the University of California Riverside, so ive been working on everyone's boards. Im going to start charging

![Snapchat-1842666593|281x500](upload://e6zGpJrlYlxjKkEEQWawhqROEN3.jpeg)
```

---
## \#22 Posted by: RyEnd Posted at: 2019-09-28T04:11:52.927Z Reads: 62

```
Really interested to see how you fit the battery. I've got that skateshred deck on a push board and it's all scraped up. I ride it real low, but I can drag the edges on the ground in a hard turn on flat.
```

---
## \#23 Posted by: turbolovah Posted at: 2019-09-28T05:57:59.468Z Reads: 57

```
I'm making a flat pack with a slimish psychotiller enclosure. I doubt I'll be able to keep it drop through, but I wanted to mount it that way preliminarily for shits n gigs.
```

---
## \#24 Posted by: Wilsonliang777 Posted at: 2019-09-28T06:25:20.416Z Reads: 60

```
So are the resisters on the esc 4.20 the new fixed version or the old version?  I am also looking to buy a pair .
```

---
## \#25 Posted by: turbolovah Posted at: 2019-09-28T17:56:26.080Z Reads: 63

```
![20190928_105202_001|281x500](upload://ildvnprmyK4ay1L8pNmwI4ZDi7O.jpeg) 

I can't tell with my naked eye, and i dont have a magnifying glass at the moment, but if my shitty camera isn't lying, i don't believe I see a decimal point on these resistors. Maybe @Schtekarsten can confirm, but I do believe they are the 47!
```

---
## \#26 Posted by: turbolovah Posted at: 2019-09-28T18:04:12.781Z Reads: 64

```
I went to psychotiller's amazing skateboard laboratory this week to get an enclosure. They let me ride some of their boards, I was blown away by the crazy power of their 4 motor setups.
![20190925_145913|690x388](upload://uSiRHN2X6UwkV6wQ9KZKx3Q7I8a.jpeg) 

![20190925_150107_014_01|281x500](upload://vIQPwHPcFg0FqUSn69Z84ddkJIq.jpeg) 

Picked up this beautiful enclosure $70

![15696937991251189039338|281x500](upload://snxDBv3VuRGnZTMtgozxIE7tkDr.jpeg)
```

---
## \#27 Posted by: Schtekarsten Posted at: 2019-09-28T19:39:57.431Z Reads: 62

```
yah that is 47 ohms resistors which is what you want for that esc (if it was 4.7 it would have been stated 4h7)
there are three categories /levels of mosfets on the 4.20 vesc though. (in other words how well the deal with heat)
1, that is the basic one with a single row of six "628 mosfets"
2, the very old dual 4.20 plus used six "612 mosfets" with is slightly better
3, the current version of dual 4.20 plus uses dual rows of six "628 mosfets" meaning you won't have temp issues on pretty much any street setup. you need to bypass the antispark by soldering a wire on the underside of the pcb on the current and previous "plus versions" and either use a loopy key or a reliable antispark.
```

---
## \#28 Posted by: turbolovah Posted at: 2019-09-29T18:35:02.920Z Reads: 54

```
Thanks for the verification, you are legit
```

---
## \#29 Posted by: turbolovah Posted at: 2019-09-29T18:44:30.090Z Reads: 57

```
Finished gripping the board, i straight copied @sayekim  but have nowhere near the skill or artistic capability,  and it came out horribly. 

![20190928_151340|281x500](upload://jZIP0sl7CUKJUakgqdyHXWn8n1s.jpeg) 

I decided to rip it off and go for simple black, i dont actually want as much attention drawn to me as that that color would have done. Also painted my blue @dickyho mounts black to match the all black scheme

![20190928_181921|281x500](upload://xHWDL2Yzh9FMb7wu4rLeQe5BUtg.jpeg) 

![Snapchat-1161929057|281x500](upload://36i6bEQTJW6FiSA8abWW9c4Miet.jpeg) 

My house is a wreck
![9804|690x388](upload://bWqNGx3XP2ExFwGujrjDXj5N0nZ.jpeg)
```

---
## \#30 Posted by: turbolovah Posted at: 2019-09-29T23:22:55.907Z Reads: 51

```
Built the spot welder. It works!!

![20190929_160614|281x500](upload://cd3IkbtUC8dQE023fsoFp6YEhul.jpeg)
```

---
## \#31 Posted by: sayekim Posted at: 2019-09-30T11:48:05.334Z Reads: 44

```
Thanks for the credit. From afar it doesn’t look very bad at all. 

Hell I notice some mistakes on mine too. 

Granted your deck does seem slightly more difficult to do with its curves.
```

---
## \#32 Posted by: turbolovah Posted at: 2019-10-04T06:59:33.617Z Reads: 36

```
So the innoculator is complete. Build pictures pending for tomorrow.
Now my question is this, i accidentally bought the wrong charger,  it is 54.6v my question is, can I use this until my replacement comes in a few days? I realize that it will over charge my battery left unattended, but can I use it if I check the voltage of my battery every 10 minutes and stop around a conservative 48v?
```

---
## \#33 Posted by: turbolovah Posted at: 2019-10-06T22:15:57.282Z Reads: 33

```
Finished, here are some pictures pre-wrapped battery.
![20190929_235351|281x500](upload://fGuuj1xDd2MnjYwZCZFvPwMDS35.jpeg) 

![20191002_235555|281x500](upload://4xuH6bfpcVTbIQgL9rqzYStgTM9.jpeg) 

![20191003_123447|281x500](upload://vLefRDhZhJtuhZFh8rLuLQsdjXu.jpeg) 

Gotta clean her before i take a finished picture, she hauls ass. These 200kv dickyho motors are super smooth and powerful.
```

---
## \#34 Posted by: turbolovah Posted at: 2019-10-07T00:03:01.497Z Reads: 29

```
Whelp, I just blew a vesc. Have no clue why or how. One moment it was working, and the next neither motor would run or brake and I was going down hill at around 30mph +, thank god I can footbrake. I was running them pretty hard, but my VESC current settings are well within the ratings.

What happened? What should I do? The VESC was $50 is it worth trying to get it repaired?

My motor current is set at 50A, my motor regen is -40A

Battery current is set at 40A, and regen set at -18A

I probably can't send it back to the aliexpress seller either... I did use it for about a week after all.

Battery is 12s4p HG2 cells
VESC is 4.2 with the updated 72ohm resistors
```

---
## \#35 Posted by: RyEnd Posted at: 2019-10-07T01:01:44.374Z Reads: 29

```
200kv @ fully charged 12s puts you above the ERPM limit, if I'm not mistaken. Also I believe the 4.2s are more reliable below 35A.
```

---
## \#36 Posted by: turbolovah Posted at: 2019-10-07T03:04:27.529Z Reads: 29

```
Ouch, yea, I was blasting full speed. To avoid this on my next vesc do I have to get a different model? Would this have happened on a flipsky 6.6 dual?

Are the Erpm limits different?
```

---
## \#37 Posted by: RyEnd Posted at: 2019-10-07T03:36:58.191Z Reads: 28

```
Yeah, the 6.6 hardware goes up to 150k
```

---

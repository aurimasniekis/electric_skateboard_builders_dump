# Will this build work?

### Replies: 19 Views: 1520

## \#1 Posted by: gdp-aggie Posted at: 2016-10-17T17:41:14.266Z Reads: 128

```
I'm new to making e-boards but for the past month i've been looking intensively into the mechanics and and electronics of them and was wondering if  with this parts list would this board work?
 
https://docs.google.com/spreadsheets/d/1T4gvcqBl18iSd3CvIxSFlb8PFTWhJ8g_zwnOccLcZgo/edit?usp=sharing

the motor mount is not on this list because i am having it custom fabricated but if anyone knows of some low price belts and pulleys it will be much appreciated.
```

---
## \#2 Posted by: SORRENTINO Posted at: 2016-10-17T17:56:22.715Z Reads: 106

```
Isnt the Turnigy AE 80 esc 6s max for lipo?
```

---
## \#3 Posted by: Quinlanbrown Posted at: 2016-10-17T18:01:01.343Z Reads: 102

```
You should use a vesc not a hobby one it will work a lot better also that switch won't work because its not thick enough wires it's make to be plugged into a board unless it works with the bms but Idk if you can do that also those batterys look like they would blow up or not put out enough juice bc that's a little cheep, for gears and pullys you should go to diy electric skateboard and get the one that bolts on so you don't have to cut the truck also it mite be easier to not get a drop through board because it's hard to get it so low, good luck tho
```

---
## \#4 Posted by: ajaynagra Posted at: 2016-10-17T18:04:49.208Z Reads: 92

```
If you are from europe i sell a pulley kit for 30 Euros and i also sell the remote that you need 

https://eu.electric-skateboard.market/store/polar/
```

---
## \#5 Posted by: thisrealhuman Posted at: 2016-10-17T18:11:26.737Z Reads: 90

```
I started with a Turnigy AE-100 and it is NOT SAFE. At 6s voltage it will accelerate if the signal is lost as a safety feature for planes so they don't just drop out of the sky. I couldn't find any way to turn it off, and the programing is way too time consuming.

The first one i had blew up while braking, the second one had me nervous about chasing my board too often. I'm using a turnigy K-force 120A now, but for the price you are better off with a VESC.
```

---
## \#6 Posted by: gdp-aggie Posted at: 2016-10-17T18:27:48.032Z Reads: 85

```
I was thinking the batteries were a little cheap so i was considering getting the panasonic 18650 battery instead. And as far as VESC goes do you have any suggestions? (I am on a college students bugdet fyi lol)
```

---
## \#7 Posted by: Quinlanbrown Posted at: 2016-10-17T18:41:00.222Z Reads: 81

```
I got mine from diy electronic skateboard but it's around $100 but I think it's worth the extra money bc you can program it and use a lot more batterys it also has a lot more safety features, if you build your own board that with save the difference also you can build a nice battery box for batterys you could use 2 zippy 5000 mah bc your already gona use a bms and that would cost around $45 but you can't always get 2 more and add on
```

---
## \#8 Posted by: lox897 Posted at: 2016-10-17T19:25:12.051Z Reads: 79

```
What config will you do your battery in?
```

---
## \#9 Posted by: gdp-aggie Posted at: 2016-10-18T00:19:19.591Z Reads: 70

```
I was thinking of using this config drawn up by another user and I'll either make it 12s or 10s. 
<img src="/uploads/db1493/original/3X/f/3/f3db181cfac38c61977240696d256f3c1d7b141e.png" width="690" height="490">
```

---
## \#10 Posted by: gdp-aggie Posted at: 2016-10-18T00:20:56.666Z Reads: 66

```
What do you mean by getting the drop through deck so low? Also do you have any suggestions for a power plug? My main goal for this is to not have to remove the entire battery pack from the board to charge it. I want to be able to plug it in where ever i go.
```

---
## \#11 Posted by: TarzanHBK Posted at: 2016-10-18T07:11:13.810Z Reads: 60

```
depending on which panasonic cells you want to use, but you have to pay attention on the discharge rate. 
Normally people build at least a 10s3p - so 30 cells, 10packs of 3 cells in series. The diagram you posted with only 10 cells in a 10s1p setup will only work with high drain batterys like the 26650 A123: https://eu.nkon.nl/rechargeable/26650/a123-systems-anr26650m1b-a-grade-3-3v-a-grade.html
```

---
## \#12 Posted by: Quinlanbrown Posted at: 2016-10-18T15:26:08.671Z Reads: 56

```
Well if you have a drop thru board the trucks the motor mite hit the board bc the boards mounted to the top but I didn't really look into the deck so idk, if you do use that bms you can charge with this 
http://www.ebay.com/itm/221909154788
http://www.ebay.com/itm/222180188366
```

---
## \#13 Posted by: gdp-aggie Posted at: 2016-10-18T17:44:55.319Z Reads: 44

```
Would a 10s 2p setup work ok?
```

---
## \#14 Posted by: thefer Posted at: 2016-10-18T18:43:20.686Z Reads: 44

```
theoretically it could work. But the thing is drawing more amps out of a battery increases heat. Heat is the enemy in these builds. I would do at least 3p on it. The max draw your motor supports is 65A so aiming closer to that would be ideal.
```

---
## \#15 Posted by: sl33py Posted at: 2016-10-18T18:59:07.941Z Reads: 42

```
[quote="gdp-aggie, post:13, topic:11303, full:true"]
Would a 10s 2p setup work ok?
[/quote]

Not very well, and you might/likely will shorten the pack life.

it's all about amp capacity - if your cells are "capable" of 20a output (constant) and 30a burst - if you run them at 20a (so in 2p - at 40a) a lot - they will not give you the full mAh capacity they have, plus generate a lot of heat and the pack will have a shorter life of recharge cycles.

here's a great example of the impact to overdrawing your cell:
[img]http://lygte-info.dk/pic/Batteries2012/Samsung%20INR18650-25R%202500mAh%20(Green)/Samsung%20INR18650-25R%202500mAh%20(Green)-Capacity.png[/img]
look at the voltage sag under heavy load - it immediately sags down to around 3.5v at 20a draw!  this equals a lot of heat - and the 2500mAh cell actually gives you 2100-2200mAh.

by adding more batteries in parallel they each provide less amps each - less sag - and more pack life.  Now i don't envision going to a 6/8p setup like @Chaka does, but on a normal 10 or 12s setup i want a minimum of 60a capacity.  This is the line in the sand i've chosen.  Or go to some of the 26650 and try 1p/2p...

my measured peak amps on a dual motor setup 8s was around 45-50a.  So i know this is my target, and given that peak was just for a few seconds i want to ensure i over-build and ensure long pack life able to provide ample amps.

HTH!
```

---
## \#16 Posted by: gdp-aggie Posted at: 2016-10-18T19:11:27.773Z Reads: 34

```
for the 26650 how many cells would you suggest?
```

---
## \#17 Posted by: sl33py Posted at: 2016-10-18T19:52:49.881Z Reads: 35

```
[quote="gdp-aggie, post:16, topic:11303, full:true"]
for the 26650 how many cells would you suggest?
[/quote]


It will depend on the batteries chosen.  And similarly to lipo packs - i take their claimed "70a constant!" claim with a large grain of salt.  Look for Mooch's review and testing that will show a similar actual discharge curve like above.

If you go with some of the Basen black 4500mAh 26650 which seem to have around 25-30a constant amps capability, i'd go with 2p to be safe.
```

---
## \#18 Posted by: gdp-aggie Posted at: 2016-10-18T21:45:19.720Z Reads: 35

```
so I combed the internet and unfortunately the battery type i would like is out of my price range right now so i guess i'm going to go with some zippy lipo's any suggestions that could still allow me to use a bms and charging port configuration? also i guess if i'm not using the 26650 or 186650 batteries would it be possible to use a ESC instead of a VESC?

(sorry i'm asking so many questions i'm still trying to get a firm grasp on batteries and how to configure them for long life and efficiency)
```

---
## \#19 Posted by: sl33py Posted at: 2016-10-18T22:06:34.522Z Reads: 33

```
No worries.

I am definitely a fan of inexpensive (relative - not the scary cheap ones i expect will spontaneously burst into flames (im kidding)) lipos.

I am almost always looking for the thinnest C dimension on HK.  So that i can have two in series (2 * 3s for 6s, or 3 * 3s for 9s... etc.), but keep them "low profile".  Better clearance, less visible and more stealth, and still *relatively* easy to charge vs one 6/8/9/12s battery.

Personally i'd skip the BMS for lipo and use the money towards Li Ion, or better/more lipo's!  add BMS later, or just pull them to charge normally w/ iMax B6ACv2 or similar charger.

a BMS is extra weight and complexity that gives you 0 additional miles.  that same $/weight in lipos/li-ion = more miles!

ESC vs VESC - i'd usually decide based on the voltage/#series batteries you want to run.  Most hobby RC ESC's will max at 6s.  Some will do 8s (usually pretty $), and a few will do 12s (usually more $ than VESC).  I like the ability to run 12s.  So either DIYes 12s ESC, or similar, or VESC would be my suggestion.

Fun scenario...  you have a 12s BEAST, and your buddy/friend/enemy ask to ride it.  Always want to spread the stoke...so of course you hand it over ... and it's promptly crashed w/ them on their ass...

or option B - take the board, flip it, pull 1 or 2 batteries to give them 6s power, and hand it back for them to try.  It's not a sofware "newbie mode" like i love on my Marbel, or on my buddies boosted, but as close as i can get today...

my .02
```

---

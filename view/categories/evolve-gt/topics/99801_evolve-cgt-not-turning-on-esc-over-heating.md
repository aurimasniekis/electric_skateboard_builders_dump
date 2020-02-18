# Evolve CGT not turning on_ Esc over heating

### Replies: 25 Views: 368

## \#1 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T12:55:47.773Z Reads: 61

```
Hi,
My friends went on my board, 2 of them at once, and as they accelerated to quickly, it shut down. I also know this is a preventative measure so as not to fry all the electronics but this is different.  Now if I was there I would have said not to do it so no point telling me it is my fault because i have read a lot on the forum and are aware of evolve's ''weird'' quality.
 
The board will not turn on, or at least the blue light on the power button does not flash.
I have taken the board apart and it smells like something is frying on the ESC. I don't think it is the BMS because when I try and charge it, the red light comes on the charger signifying it is charging.
the ESC also heats up (like untouchable hot) immediately when I turn the board on in one particular spot below the evolve logo on the ESC. it seems like it comes from a little black square below. pics below.
Also, when I took the cover off, the yellow lead from motor 1 was unsoldered. just above it, is where the heat is coming from. I have now re-soldered it back.
Any help is appreciated and if someone now the price for evolve to repair or is selling an Evolve ESC then please DM me.

Kind regards
Louis![20190806_132853|666x499](upload://kgLZ2xwMX2rKQPe0KfhWQRSMzhW.jpeg) ![20190806_132750|666x499](upload://vzRPNGdKER6fpneYetcsziAPMbp.jpeg) ![20190806_132934|666x499](upload://pN1GYvleFlXpwqhzCCzNIv7aBoc.jpeg) ![20190806_132922|666x499](upload://4QV0yQ0sK1VKOI9tyZ4VlnJZH0D.jpeg) ![20190806_132911|375x499](upload://sYnfRgFUrm1Ln7eIHVFCrs950UG.jpeg)
```

---
## \#2 Posted by: Crashmaster Posted at: 2019-08-06T14:25:14.689Z Reads: 54

```
I had mine recently shut down. And I found out that one of my capacitor leads had a broken solder joint. 
You can see in the pic. The lead closest in the pic was just barely touching.
Not saying this is your problem. Just inspect the board with a magnifying glass to see if anything looks suspicious. 
And inspect the pins if any are bent or missing.
![0729191214_Film1|666x500](upload://uDGZVLTzD7L26RrXandHblpuQco.jpeg)
```

---
## \#3 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T15:00:44.374Z Reads: 50

```

Thanks, @Crashmaster!
how did you remove the ''two'' ESC from each over. I tried forcing a little with 2 screwdrivers but didn't dare.
```

---
## \#4 Posted by: Crashmaster Posted at: 2019-08-06T15:05:15.190Z Reads: 49

```
Remove the 4 Phillips screws with the red insulating washers. 
Pull apart carefully. 
When putting it back together make sure the pins are lined up.
```

---
## \#5 Posted by: Halbj613 Posted at: 2019-08-06T16:59:02.479Z Reads: 47

```
if you are not able to fix it

Then you could replace it with a vesc
```

---
## \#6 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T17:09:01.460Z Reads: 46

```
Sure but do I have the money for a Unity and a BMS? 300 plus euros?
not sure lol. I have taken it apart and looked carefully I will post detailed photos of the whole thing and show where it is heating up. @Crashmaster if you can take a peep to see if you can spot anything :wink:
```

---
## \#7 Posted by: Halbj613 Posted at: 2019-08-06T17:25:44.498Z Reads: 41

```
Why do you need a new bms
```

---
## \#8 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T17:49:33.835Z Reads: 39

```
Evolve BMS won't work with Focbox Unity, will it?
```

---
## \#9 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T17:54:05.982Z Reads: 42

```
![20190806_191335|375x500](upload://jyu4lANiusrCLp3e0JqrTSYWUWQ.jpeg) ![20190806_191349|375x500](upload://leGSJlHLJYirezwpmvGzTwybeZS.jpeg) ![20190806_191235|375x500](upload://3MXkADjrJzASLG3GjTqbN8sEgh1.jpeg) ![Capture%20_2019-08-06-19-52-33|265x500](upload://vf3QsbhyW6brW2VxUSWBEUjg8ia.jpeg) ![20190806_191249|375x500](upload://bolSXovsQUMAGM0ukYnBo76EnWD.jpeg) ![Capture%20_2019-08-06-19-52-01|265x500](upload://mEqEhFgKfSTm9BsCvK9hqznOMMu.jpeg) ![20190806_191244|375x500](upload://Ai59dWC2cltj1gb8t4w9hc25gpW.jpeg)
```

---
## \#10 Posted by: Crashmaster Posted at: 2019-08-06T18:06:42.155Z Reads: 40

```
I don't see anything out of the ordinary. 
Except your positive lead insulation is torn.
```

---
## \#11 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T18:11:40.528Z Reads: 39

```
Yep. I dont know how though but i saw that too when i took the top off but it should not change anything.
How can i diagnose if it is the BMS?
```

---
## \#12 Posted by: Crashmaster Posted at: 2019-08-06T18:27:11.405Z Reads: 37

```
I assume your able to turn it on. 
I had to unplug my battery and plug it back in for it to turn on. 
When mine died it would not turn on at all.
```

---
## \#13 Posted by: PixelatedPolyeurthan Posted at: 2019-08-06T18:56:35.419Z Reads: 33

```
Negative. The blue light on the power botton does not flash when i press it. I pulled the esc apart and looked at it then put everything back and pluged in only SWITCH, UART and BATW, leaving the motors and hall sensors unplugged and got zero response from the board except as i said when i turn it on it immetiately heats up as i showed in the pics above with a yellow circle.
```

---
## \#14 Posted by: Crashmaster Posted at: 2019-08-06T20:24:59.424Z Reads: 30

```
The 2 black components that are circled are voltage regulators. The small one is a LDO and the large one is a linear. 
A linear regulator dissipates heat proportional to the amount of voltage it must drop, and the amount of current flowing through it.
Even if this was in front of me it would be difficult to trouble shoot assuming the 2 boards need to be together to work properly enabling to test with a meter. 
I'm no expert. And not a electrical engineer.
But I have done board repairs in the past on other equipment. 
Unfortunately it's starting to be a lost art due to it's easier to replace the board than try to trouble shoot a board without schematics.
I only know of a few people who do enjoy doing this type of work.
```

---
## \#15 Posted by: PixelatedPolyeurthan Posted at: 2019-08-07T09:20:27.391Z Reads: 28

```
Thanks for that :blush:

I am just going to have to get a new ESC I think.
I have contacted evolve France (because that is where I live) to see what they have to say.
They are really rude though and quite unhelpful so we will see.
```

---
## \#16 Posted by: PixelatedPolyeurthan Posted at: 2019-08-07T10:23:33.786Z Reads: 29

```
@Crashmaster So 179 euros for an ESC, 40euros/hour for repair, 40 euros total for shipping (return) and if it is the BMS it costs 39euros.
So a Min. of 259euros.
I say perso get a unity and sell evolve remote. What do you think?
With your knowledge do you agree that the chances of the problem being the battery/cells being fried is minimal? if something went wrong it is either BMS or ESC right?
```

---
## \#17 Posted by: sQuaff Posted at: 2019-08-07T11:19:07.930Z Reads: 27

```
I dont think is the bms because I had the same problem couple times and if smells like is frying looks like is the controller ( esc )  and You dont need to send your board just ask them for a replacement. No shipping and no labor. Also you could find on eBay for better price.
```

---
## \#18 Posted by: Crashmaster Posted at: 2019-08-07T19:15:52.896Z Reads: 25

```

It's a decision you need to make.
If you want to be stuck using the Evolve stuff and dealing with the high prices of replacement parts their service.
Or Go aftermarket were you have more options to choose from,
Eventually by the end of the year I'll be changing over to an aftermarket Bms and Esc's and controller to get out of being stuck with their stuff and not having a option for how I want my board to perform.
```

---
## \#19 Posted by: esk8jpn Posted at: 2019-08-08T01:01:41.227Z Reads: 20

```
Are there any Evolve riders in your neighborhood?
If so, I thought that I could temporarily replace it with a normal ESC to identify the failure.

The Evolve forum often sells second-hand goods. I have a V1 ESC(brakes are dangerous) and I want to help you, but unfortunately I live in Japan...
```

---
## \#20 Posted by: PixelatedPolyeurthan Posted at: 2019-08-08T05:40:22.689Z Reads: 18

```
Thank you @esk8jpn.
I live in France but no where near Paris. May be @okp can help me ?
```

---
## \#21 Posted by: PixelatedPolyeurthan Posted at: 2019-08-08T09:16:49.736Z Reads: 15

```
@esk8jpn?
 Does the stock Evolve battery just plug and play with the Focbox Unity? 

Does the BMS or the battery itself need to be changed?

EDIT

@Eboosted I just saw last year you had the same problem, were you able to tell what failed on the ESC? if you read my description above and look at the photos can you tell me if you spot anything suspicious?
https://www.electric-skateboard.builders/t/help-why-is-my-bms-balance-wire-melting-on-custom-evolve-gt-battery-build/47142/18?u=pixelatedpolyeurthan
```

---
## \#22 Posted by: PixelatedPolyeurthan Posted at: 2019-08-08T11:11:39.127Z Reads: 15

```
And my last problem is now i don't know what to do.
I beleive i have 3 options. I paid 950 euros for this board btw. It has only 50 Battery cycles used on it and the board is in great condidtion.

#1 Pay 250 odd euros to get it fixed then sell for around 1000 euros and make a custom evo falcon all terrain board.

#2 Buy the new hobbywing ESC for evolve for 175USD and sell like above.

#3 Redo the whole board into a focbox beast but i will end up being the same price as a new GTR or whatever and think that is stupid.
```

---
## \#23 Posted by: esk8jpn Posted at: 2019-08-08T11:52:33.787Z Reads: 13

```
The stock Evolve battery pack is a Deans connector, it cannot be plug and play with Unity.  You need to create an XT60 conversion cable.

Deans connector
![031004000001|334x200](upload://yHvLjejJvAbQVq4cCPwDY1Y8Dv7.jpeg) 

Don't need to replace the BMS.
```

---
## \#24 Posted by: Eboosted Posted at: 2019-08-08T15:17:55.175Z Reads: 13

```
You can't just unplug the battery and connect a Unity as the remote works with the original ESC.

If I were you I'd but a new 10S4P Li-Ion battery pack with bms, an unity and a remote and enjoy a completely better board in all ways
```

---
## \#25 Posted by: PixelatedPolyeurthan Posted at: 2019-08-08T17:14:56.639Z Reads: 12

```
@Eboosted if I change the battery then I will sell this board and go DIY.

**If I change the dean connector to xt60 and buy a new remote for unity will it work?**

remember I brought the gt 2nd hand on a budget. now if I start upgrading the battery, ..., etc then it will be just more expensive then building one DIY that would be richer both electronically and powerfully.
I think in any case I will sell it to a friend so I can ride with someone and then make my self a monster board **but I need to know what will and won't work with the unity, please.**

Thanks again Alan... if I go DIY I am sooo buying that Evo falcon enclosure :heart_eyes:
```

---

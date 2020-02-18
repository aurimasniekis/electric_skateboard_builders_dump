# Need help with charging

### Replies: 24 Views: 1155

## \#1 Posted by: Thatdudedominic Posted at: 2018-01-31T15:18:36.728Z Reads: 103

```
I have 4 3s 5000mah  I hate the fact that I have to take everything apart and charge each battery on a balance board I’m looking for a new method to charge my born without taking everything apart can I get some input I have an old charger already for 50 V charging at2amp I believe Where do I go from here![image|533x500](upload://t7cVBEwZkpkzEAMYqOuJSVQ3ePo.jpeg)
```

---
## \#2 Posted by: craj1031tx Posted at: 2018-01-31T15:36:28.108Z Reads: 94

```
You'll have to get a 12s BMS circuit and wire your charge port into it, and then the BMS into your battery array. Should be lots of info out there on the forum.

Two things you need to determine: what brand BMS to get (expect to pay about 60-70 shipped for a good 12s, or you could try your luck with an aliexpress $25 model), and if you want the BMS to sit in between both the discharge and charge circuit, or just the charge circuit. sitting in between both is the best approach but is more costly; many feel it's ok to have it solely on the charge circuit and bypass it for discharge.
```

---
## \#3 Posted by: pennyboard Posted at: 2018-01-31T15:39:43.378Z Reads: 90

```
You don’t necessarily need a bms. I’ve been charging a 12s lipo pack direct with the charger linked below for 6 months and it works great. 

https://m.ebay.com/itm/50-4V-2A-Power-Adapter-For-Self-Balanced-Vehicle12S-Li-ion-Battery-Charger-Plug-/291922334252
```

---
## \#4 Posted by: MysticalDork Posted at: 2018-01-31T15:41:25.659Z Reads: 79

```
Also, triple check that the "50v" charger you have is actually putting out the correct voltage (which should be 12*4.2=50.4v)

You'll also need some sort of port to plug the charger into. I used an XLR plug because I had them, and they're available with dust covers, but anything works as long as it's fairly robust.
```

---
## \#5 Posted by: craj1031tx Posted at: 2018-01-31T15:41:32.824Z Reads: 75

```
Interesting, i've heard of people charging large li-ions without a bms, but it is very rare to charge lipos without one, from what i understand. i think the vast majority of people would agree that having a bms on a lipo pack is mandatory.
```

---
## \#6 Posted by: MysticalDork Posted at: 2018-01-31T15:42:52.520Z Reads: 73

```
Definitely agree with the "you really do need a BMS" statement. The cells are never THAT well balanced, especially long term.
```

---
## \#7 Posted by: pennyboard Posted at: 2018-01-31T15:43:07.840Z Reads: 69

```
Yeah I mean it’s all up to you and what you feel comfortable doing.
```

---
## \#8 Posted by: b264 Posted at: 2018-01-31T17:40:34.418Z Reads: 65

```
[quote="pennyboard, post:3, topic:45159"]
You don’t necessarily need a bms. I’ve been charging a 12s lipo pack direct with the charger linked below for 6 months and it works great.
[/quote]

It works great, all the way up to the huge fire.  I mean, even right before that it will work great.  :roll_eyes:

You better check each cell voltage with a multimeter at a MINIMUM to verify it's working as good as you think it is...
```

---
## \#9 Posted by: Thatdudedominic Posted at: 2018-01-31T17:59:29.407Z Reads: 61

```
So my full charge is 50.4 and my cut off is at 44.4 volts I have two motors 6374 two vesc from  torque boards what’s is a bms how do I find it and wire it right
```

---
## \#10 Posted by: MysticalDork Posted at: 2018-01-31T18:55:52.248Z Reads: 57

```
http://lmgtfy.com/?q=What+is+a+bms second result.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-01-31T19:04:24.443Z Reads: 58

```
Read this thread:
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#12 Posted by: Namasaki Posted at: 2018-01-31T19:08:00.440Z Reads: 54

```
[quote="craj1031tx, post:5, topic:45159, full:true"]
Interesting, i’ve heard of people charging large li-ions without a bms, but it is very rare to charge lipos without one, from what i understand. i think the vast majority of people would agree that having a bms on a lipo pack is mandatory.
[/quote]


Lithium battery packs should always be balance charged. Both Lipos and Li-ions.
```

---
## \#13 Posted by: b264 Posted at: 2018-01-31T19:08:19.600Z Reads: 50

```
[quote="MysticalDork, post:10, topic:45159, full:true"]
http://lmgtfy.com/?q=What+is+a+bms second result.
[/quote]

If you want to say "second result" then you can't pick "google" as the search engine because Google gives each person different results.  ddg.gg will give the same results for the same query.
```

---
## \#14 Posted by: Acido Posted at: 2018-01-31T19:31:01.724Z Reads: 46

```
Bms for charge only is mandatory if you ask me on every type of battery
Unless you have a balance charger
```

---
## \#15 Posted by: MysticalDork Posted at: 2018-01-31T19:59:43.577Z Reads: 40

```
True, but I'd be willing to wager that Wikipedia is high on everyone's list.
```

---
## \#16 Posted by: pennyboard Posted at: 2018-01-31T20:32:18.666Z Reads: 36

```
I pull the enclosure once a month, and check the cells. Each time I do it, they are perfectly balanced. I think the danger of lipos has been blown out of proportion and with some common sense and care, they're perfectly safe
```

---
## \#17 Posted by: Thatdudedominic Posted at: 2018-01-31T20:55:15.719Z Reads: 36

```
So what’s hooks to the bms from the charger
```

---
## \#18 Posted by: Clonkex Posted at: 2018-01-31T21:32:18.127Z Reads: 36

```
That's perfectly fine until one of the cells goes bad. Without balancing, the first time you know about it will be when your house burns down.

It's like parachuting. You can be as careful as you like in packing your parachute (checking your cells), but eventually it's going to fail to open (a cell will go bad). Without a backup chute (BMS) the results are catastrophic.
```

---
## \#19 Posted by: pennyboard Posted at: 2018-02-01T01:20:10.366Z Reads: 31

```
Well I guess agree to disagree on battery design. Thanks for your opinion though :grinning:
```

---
## \#20 Posted by: louwii Posted at: 2018-02-01T01:58:13.837Z Reads: 30

```
Wait, what ?
Are you sure you understand the possible consequences of charging a Lipo or Li-ion battery without a balance charger or BMS ?
I mean, not caring is a thing. But you can't say that not using a BMS or balance charger is OK and safe.
```

---
## \#21 Posted by: pennyboard Posted at: 2018-02-01T01:59:11.992Z Reads: 28

```
I'm saying that I routinely check my cells and they have never strayed out of balance. That is the point of a BMS, to keep them in balance, and if my cells stay in balance without one, a BMS is unnecessary.
```

---
## \#22 Posted by: louwii Posted at: 2018-02-01T02:03:00.471Z Reads: 28

```
Sure, I agree. You should have indicated that in your first post, especially when a newbie is asking for help/advice :slight_smile: And battery are a serious subject due to how dangerous it can be. It's better to share the whole picture, I think too much information is always better than not enough information.

One thought: I believe cells get out of balance more easily with age and charge/discharge cycles.
```

---
## \#23 Posted by: pennyboard Posted at: 2018-02-01T02:06:10.627Z Reads: 28

```
Yeah, that's fair, I could definitely be more descriptive.

[quote="louwii, post:22, topic:45159"]
One thought: I believe cells get out of balance more easily with age and charge/discharge cycles.
[/quote]

Yeah this is true, I usually get new batteries about once a year. Costs me $100 to get high discharge lipos, when similar range and lower discharge lions would cost $350 to $400. So i figure the cost is about the same long-term (lions last about 3-4 years I believe)
```

---
## \#24 Posted by: louwii Posted at: 2018-02-01T02:07:56.166Z Reads: 22

```
Yeah, that's why I went for Lipos too for my first build.
It's also easier to swap, if you ever need to.
```

---

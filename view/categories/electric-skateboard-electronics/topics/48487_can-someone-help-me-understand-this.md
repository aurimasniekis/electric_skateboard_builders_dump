# Can someone help me understand this

### Replies: 50 Views: 1401

## \#1 Posted by: Thatdudedominic Posted at: 2018-03-08T12:57:02.211Z Reads: 230

```
So I want more range I’m running 4 3s 5000 mah battery’s and I want to add a another on in  parallel Which drawing is correct to achieve 44.4v 10,000 mah or am I just dreaming to Big thanks guys 

 ![image|375x500](upload://sjQSu8YGPiQWhOrS0AgmtTl1M8Z.jpeg)![image|375x500](upload://j9pAClEwIuFRF9DVFvWT3SYAh6u.jpeg)
```

---
## \#2 Posted by: TranxFu Posted at: 2018-03-08T13:00:47.959Z Reads: 207

```
For 12s 10mah it’ll be a „12s2p“ setup. Which means you’ll need another 3 packs of these.
```

---
## \#3 Posted by: Thatdudedominic Posted at: 2018-03-08T13:01:22.154Z Reads: 201

```
Can you show me a quick schematic of it how it will look
```

---
## \#4 Posted by: TranxFu Posted at: 2018-03-08T13:02:34.723Z Reads: 201

```
At work atm. But practically 2x 4 of these in series and then add those 2 packs in parallel.
```

---
## \#5 Posted by: wafflejock Posted at: 2018-03-08T13:03:26.810Z Reads: 195

```
You want parallel if you are trying to increase capacity mAh rather than voltage.  The first diagram you are effectively making one battery larger than the rest and then hooking them in series, don't think this will work because that one section where they are parallel will be able to run twice as long as the rest.  The second option also won't work because you're attaching a 3S to a 12S in parallel which will dump charge from the high voltage battery into the lower voltage one.

Basically you just need to double up on all the series batteries you have in the original setup then can have pairs in parallel and the rest in series (12S "2P", usually reserve P for 18650s) but hopefully makes sense.
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2018-03-08T13:34:58.239Z Reads: 175

```
![12s|690x388](upload://wwm2nvPsokarsa2Y1u7HVIzEqK8.png)

Hope that makes sense :D
```

---
## \#7 Posted by: wafflejock Posted at: 2018-03-08T13:57:42.128Z Reads: 162

```
Just to note the added parts could have lower mAh than the original if say you want to add 1Ah3S at each position (4Ah total), that'd be fine so long as the voltage is still the same.

You should also try to keep the internal resistance about the same so make sure to calculate max discharge if you do use different types of cells in parallel.
```

---
## \#8 Posted by: Thatdudedominic Posted at: 2018-03-08T14:37:35.613Z Reads: 152

```
So this mean I need to get 4more of the same battery’s 👍🏽
```

---
## \#9 Posted by: Thatdudedominic Posted at: 2018-03-08T14:39:30.195Z Reads: 152

```
I think I’m just going to invest in a battery pack 12s5p hope I can find one for a good price cause charging my board is a pain in the rear end 

 ![image|374x500](upload://ps1VNNoA7m9LfsRDQYcqiuDjRYX.jpeg)![image|375x500](upload://plFzc1JsjN956iWrtIxXX8XoEEx.jpeg)
```

---
## \#10 Posted by: butt_stallion Posted at: 2018-03-08T15:12:45.216Z Reads: 131

```
If you have the time your could build your own.  Lots of resources on the forums to help you with it.   I would invest in [This spot welder](http://www.electric-skateboard.builders/t/boss-level-custom-spot-welder/25980/595).  If you ever need to do maintanence on your battery you have the knowledge.  If it's too much of a hassle I'm sure someone would be happy to sell you one on here.
```

---
## \#11 Posted by: wafflejock Posted at: 2018-03-08T15:57:37.365Z Reads: 124

```
Yeah could definitely see that with that many separate packs... it does allow you to keep it relatively slim but charging becomes a minor nightmare.  Personally using 2x5S 5Ah batteries but it does end up being a pretty thick brick of cells (works out okay for my board since it's a short deck with a kicktail anyway)

[swappable batteries](https://photos.app.goo.gl/KzDYcYYeHPuD4u5e2)

Charging still involves hooking up both batteries separately (could charge in parallel but my charger wattage limits the rate anyway)
```

---
## \#12 Posted by: Thatdudedominic Posted at: 2018-03-09T01:08:07.959Z Reads: 106

```
So up date jus brought 60 18650 cell’s I there 5000 mah and I found these I do not wanna spot weld ![image|281x500](upload://pcnBi7Ag0BiWq8MDoo84V3X2Qcb.jpg)
```

---
## \#13 Posted by: Thatdudedominic Posted at: 2018-03-09T01:10:27.490Z Reads: 98

```
I want to make a flat pack
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-03-09T01:11:47.350Z Reads: 100

```
link the 18650’s please
```

---
## \#15 Posted by: Thatdudedominic Posted at: 2018-03-09T01:13:02.632Z Reads: 97

```
Are they bad 
https://www.ebay.com/itm/50Pcs-18650-3-7V-Rechargeable-Li-ion-Battery-Charger-For-Flashlight-Torches-S-/202242441208
```

---
## \#16 Posted by: GrecoMan Posted at: 2018-03-09T01:14:45.170Z Reads: 96

```
yes. cancel that immediately.

get some 30q’s from nkon.nl
```

---
## \#17 Posted by: Thatdudedominic Posted at: 2018-03-09T01:15:09.320Z Reads: 96

```
Okay cool thanks for the tip
```

---
## \#18 Posted by: Thatdudedominic Posted at: 2018-03-09T01:21:05.817Z Reads: 96

```
Okay now I have questions how do I know if they are brand new and do they have A expiration date or a build date
```

---
## \#19 Posted by: GrecoMan Posted at: 2018-03-09T01:24:14.488Z Reads: 92

```
everything on nkon is new.
18650’s don’t expire.
build whenever the hell you want.
```

---
## \#20 Posted by: RedEagle Posted at: 2018-03-09T01:37:44.162Z Reads: 91

```
You have NO idea how much you've ruined my day
```

---
## \#21 Posted by: butt_stallion Posted at: 2018-03-09T01:57:28.848Z Reads: 86

```
Has anyone used these before?  The battery bus bars are stainless steel, which I don't think is very conductive.  But I could be wrong.
```

---
## \#22 Posted by: wafflejock Posted at: 2018-03-09T02:57:09.337Z Reads: 83

```
How so?
10char
```

---
## \#23 Posted by: RedEagle Posted at: 2018-03-09T04:23:31.694Z Reads: 80

```
Let's just say I wanted to try something similar..
```

---
## \#24 Posted by: mmaner Posted at: 2018-03-09T04:49:38.901Z Reads: 75

```
Just ordered 65 30qs from ru.nkon.nl myself 😀
```

---
## \#25 Posted by: L3chef Posted at: 2018-03-09T05:41:47.722Z Reads: 73

```
Why from ru.nkon? Do you get them cheaper from there?
```

---
## \#26 Posted by: Nordle Posted at: 2018-03-09T06:33:13.394Z Reads: 72

```
Why not? Isn't cold war finished?
```

---
## \#27 Posted by: GrecoMan Posted at: 2018-03-09T11:05:01.621Z Reads: 71

```
ru.nkon.nl is for people outside the EU

nkon.nl is for EU
```

---
## \#28 Posted by: mmaner Posted at: 2018-03-09T13:02:26.552Z Reads: 65

```
$2.75 each.  That's the best price I've seen.
```

---
## \#29 Posted by: FredrikHems Posted at: 2018-03-09T14:08:42.428Z Reads: 63

```
When you guys say EU, do you mean  Europe or the European Union? Seems like many dont know the difference..
```

---
## \#30 Posted by: GrecoMan Posted at: 2018-03-09T14:08:57.578Z Reads: 63

```
i have no clue

all I know is that it won’t let you order from ru.nkon.nl if you’re in the “EU” (quote from many other posts about this)
```

---
## \#31 Posted by: wafflejock Posted at: 2018-03-09T15:58:01.198Z Reads: 61

```
No reason you can't do it as well (remix/upgrade)

https://cad.onshape.com/documents/15cd342c90ae1b0b6fd666bf/w/40780c7d8d67fd69a32fbf6e/e/fe1a99d1423c52e012228250

^^ my design is here, it works for 5S 5Ah packs (from turnigy) but you could modify the design or just use ideas from it if they are useful.  I'm not manufacturing them or anything it's a substantial amount of work to do that by hand and I don't see it being a big enough market of buyers to justify doing anything at larger than at home scale.  Happy to have it myself, but too time costly to make to offer for sale (for me anyway).
```

---
## \#32 Posted by: RedEagle Posted at: 2018-03-09T23:44:02.459Z Reads: 54

```
I wanted to do exactly what he did with 5 5s 5ah packs. 10s4p configuration. Two in series and the rest in parallel.
```

---
## \#33 Posted by: wafflejock Posted at: 2018-03-09T23:57:24.112Z Reads: 55

```
Ah I see sorry misunderstood.  To be fair I didn't really ruin anything in this case, you have to blame physics or nature for this one (don't shoot the messenger)
```

---
## \#34 Posted by: RedEagle Posted at: 2018-03-10T00:08:12.482Z Reads: 53

```
Yeah but you know what I meant. Not aimed specifically at you or anything.
```

---
## \#35 Posted by: L3chef Posted at: 2018-03-10T11:00:04.818Z Reads: 46

```
That's a sweet price.. 3.99€ fron nkon.nl :frowning:
```

---
## \#36 Posted by: GrecoMan Posted at: 2018-03-10T12:24:38.255Z Reads: 41

```
add it to the list of reasons to move to the US 🤣
```

---
## \#37 Posted by: Blitz Posted at: 2018-03-10T12:45:39.587Z Reads: 40

```
EU stands for European Union, I'm From Ireland and I got in Ukraine without visa "European Union" so company's shipping to any country part of the Union will not have to pay import fees etc.
```

---
## \#38 Posted by: FredrikHems Posted at: 2018-03-10T13:05:13.561Z Reads: 37

```
Yeah, i knew that, but there is alot of confusion around here about EU and Europe..
```

---
## \#39 Posted by: L3chef Posted at: 2018-03-10T13:05:17.814Z Reads: 37

```
And leave all this behind? Free education and medical help for cheaper batteries. Naah man :smirk:
```

---
## \#40 Posted by: GrecoMan Posted at: 2018-03-10T13:06:45.226Z Reads: 37

```
idk man... i’ve never paid a dime to go to public school 🤔

but medical help...

you can enjoy your $5 30q’s while i’ll be over enjoying my $2.75 30q’s 😉
```

---
## \#41 Posted by: L3chef Posted at: 2018-03-10T13:10:19.106Z Reads: 36

```
:joy:
Yeah I will sit here with my expensive cells in one hand, and a proper beer in the other :see_no_evil:
```

---
## \#42 Posted by: GrecoMan Posted at: 2018-03-10T13:38:45.639Z Reads: 33

```
hey now that was uncalled for 🤣
```

---
## \#43 Posted by: PXSS Posted at: 2018-03-10T13:45:20.682Z Reads: 35

```
[quote="GrecoMan, post:40, topic:48487"]
you can enjoy your $5 30q’s while i’ll be over enjoying my $2.75 30q’s :wink:
[/quote]
They never taught you that €1 ≠ $1. 

Man our public schools suck
```

---
## \#44 Posted by: GrecoMan Posted at: 2018-03-10T13:46:48.921Z Reads: 35

```
he said €3.99 per cell... so i said $5 🤔
```

---
## \#45 Posted by: PXSS Posted at: 2018-03-10T13:50:53.276Z Reads: 32

```
What about the €2.75? You forgot that that's not $2.75?

What did we learn in the other topic today? Confirm your sources! 😂😜

Mike said $2.75 but it's actually €.
```

---
## \#46 Posted by: GrecoMan Posted at: 2018-03-10T13:56:08.880Z Reads: 32

```
lol I was just going off what @mmaner said

sorry for throwing you uber the bus btw 🤣
```

---
## \#47 Posted by: PXSS Posted at: 2018-03-10T14:00:55.121Z Reads: 31

```
¯\\_(ツ)_/¯  .
```

---
## \#48 Posted by: mmaner Posted at: 2018-03-10T14:01:31.914Z Reads: 31

```
Yep, had a couple if bears and started drunk buying 😀
```

---
## \#49 Posted by: GrecoMan Posted at: 2018-03-10T14:02:13.177Z Reads: 32

```
that post makes me think you’re still hungover 🤣

you always seem to have a way with words, sometimes the correct spelling and grammar brings a tear to my eye. absolutely beautiful writing.
```

---
## \#50 Posted by: mmaner Posted at: 2018-03-10T14:05:18.316Z Reads: 32

```
Just woke up, not hungover just sleepy stupid.  I've got to find a solution to this phones auto correct, it's killing me.  My FBI agent must think I love ducks. 😀
```

---

# Charging 2 6s batteries in series

### Replies: 39 Views: 1127

## \#1 Posted by: dg798 Posted at: 2017-11-26T19:43:05.983Z Reads: 89

```
Is there some sort of 12s charger that can charge 2 6s batteries in series. Or a dual 6s charger that’s not extremely expensive.
```

---
## \#2 Posted by: ugothakd Posted at: 2017-11-26T20:03:13.913Z Reads: 86

```
You could always wire your 6s batteries in parallel, and do the same with the balance leads, and charge them with a 6s charger. It will probably be slow, doubling charge times. Your best bet is to get a battery management system
```

---
## \#3 Posted by: dg798 Posted at: 2017-11-26T20:04:32.496Z Reads: 84

```
i can't really afford a 12s bms right now and im not the best with wiring
```

---
## \#4 Posted by: ugothakd Posted at: 2017-11-26T20:10:50.766Z Reads: 81

```
Then charge them one at a time... It takes work to get something nice. There are some group buys for 12s bmss often. A BMS will be much cheaper than any 12s charger
```

---
## \#5 Posted by: dg798 Posted at: 2017-11-26T20:13:17.275Z Reads: 70

```
currently i am charging one at a time. it just takes too long to charge both of them seperately.
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-11-26T20:13:52.952Z Reads: 66

```
just get a parallel charging board
```

---
## \#7 Posted by: dg798 Posted at: 2017-11-26T20:14:57.197Z Reads: 68

```
i hear it doesnt balance charge each cell properly and that its dangerous.
```

---
## \#8 Posted by: FredrikHems Posted at: 2017-11-26T21:18:24.091Z Reads: 62

```
Then just buy 2 of the I max b6 copy chargers. Under 20$ each
```

---
## \#9 Posted by: dg798 Posted at: 2017-11-26T21:20:14.506Z Reads: 61

```
i have 2 right now but i cant seem to find a decent charger. it takes like 12 hours to charge one of them
```

---
## \#10 Posted by: FredrikHems Posted at: 2017-11-26T21:23:47.508Z Reads: 61

```
Do you have 2 imax`s? if your batteries aren't 30000 mAh each (Which they obviously aren't) it shouldt take 12 hours
```

---
## \#11 Posted by: dg798 Posted at: 2017-11-26T21:25:30.365Z Reads: 56

```
i have 2 imax but i am only using one for each battery.
i am using a 2 amp powers supply but it only lets me go max 1.2 amps.
```

---
## \#12 Posted by: FredrikHems Posted at: 2017-11-26T21:26:38.869Z Reads: 53

```
Then i understand.. You better just buy 2 more powerful supplies of eBay
```

---
## \#13 Posted by: dg798 Posted at: 2017-11-26T21:32:12.739Z Reads: 54

```
i guess thats what i will have to do
```

---
## \#14 Posted by: danielz Posted at: 2017-11-26T21:33:21.420Z Reads: 54

```
Ive done this. Vesc on the left, batteries right two. My connectors  are all antispark. My balance leads come out a little hole in my enclosure. 250w charger. You can either do them one at a time, or buy a fused parallel board. Oh ive also a temperature sensor connector, to stop charging if the temp exceeeds 30c.

<img src="/uploads/db1493/original/3X/f/b/fba549e73c886e972afc9c4d721f8acadc45127c.JPG" width="375" height="499">
```

---
## \#15 Posted by: gbutcher Posted at: 2017-11-26T21:37:00.451Z Reads: 52

```
A more powerful power supply is required as mentioned above.  Nothing wrong with parallel charging if you do it right.  I've been doing it for years and never had an issue.  

https://oscarliang.com/parallel-charging-multiple-lipo/
```

---
## \#16 Posted by: dg798 Posted at: 2017-11-26T21:43:08.329Z Reads: 51

```
i think im just going to buy a more powerful supply.
also can i charge a 5200 mah 6s 15C~30C battery at 5 amps?
```

---
## \#17 Posted by: danielz Posted at: 2017-11-26T21:45:27.827Z Reads: 51

```
All batteries are different. My 6s 30c ones are 2c (10amp) Ive seen much higher. 

Everyone recommends 1c. I charge 1.5c. My batteries only go 1-2 celcius over ambient temp.
```

---
## \#18 Posted by: E1Allen Posted at: 2017-11-26T21:46:42.002Z Reads: 49

```
Check out used chargers on rcgroups.com.  I picked up a 1000w charger and 750w power supply for $80shipped
```

---
## \#19 Posted by: dg798 Posted at: 2017-11-26T21:53:23.186Z Reads: 49

```
ok thanks for everyones input.
```

---
## \#20 Posted by: FredrikHems Posted at: 2017-11-26T22:04:19.869Z Reads: 49

```
Remember that you can only charge up to 2a on 6s/25.2v on the iMax b6
```

---
## \#21 Posted by: dg798 Posted at: 2017-11-26T22:29:13.006Z Reads: 44

```
it says i can go up to 5 amps
```

---
## \#22 Posted by: E1Allen Posted at: 2017-11-26T22:32:02.638Z Reads: 41

```
It can. Depending on battery voltage.

50w charger charging a 6s battery 25v.  50/25=2a
```

---
## \#23 Posted by: dg798 Posted at: 2017-11-26T22:33:56.872Z Reads: 41

```
what if i use more than a 50w charger
```

---
## \#24 Posted by: E1Allen Posted at: 2017-11-26T22:35:10.738Z Reads: 41

```
Then more amps. My 750w power supply can do up to 6s at 30a roughly. Which is more than enough for one battery.
```

---
## \#25 Posted by: dg798 Posted at: 2017-11-26T22:36:24.679Z Reads: 41

```
ah ok got it thanks
```

---
## \#26 Posted by: Jammeslu Posted at: 2017-11-26T22:37:35.435Z Reads: 41

```
Buy a 5 dollar bms an bypass discharge and you live happy
```

---
## \#27 Posted by: E1Allen Posted at: 2017-11-26T22:39:00.632Z Reads: 41

```
But with a larger charger and a parallel charge board you can charge your like batteries together and faster
```

---
## \#28 Posted by: dg798 Posted at: 2017-11-26T22:40:26.531Z Reads: 39

```
i cant find a cheap 12s bms anywhere
```

---
## \#29 Posted by: dg798 Posted at: 2017-11-26T22:46:48.358Z Reads: 39

```
can i run 4-5 amps off this one https://www.amazon.com/Selectec-12-Volt-Power-Supply/dp/B009ZZY28M/ref=sr_1_3?ie=UTF8&qid=1511736355&sr=8-3&keywords=6+amp+dc+power+supply
```

---
## \#30 Posted by: E1Allen Posted at: 2017-11-26T22:47:54.507Z Reads: 42

```
My charger.  <img src="/uploads/db1493/original/3X/2/7/270c41550bb2501539181b9954b05ed68d4f7e67.jpg" width="281" height="500">

Still limited to charging 6s max. Just connect in series on the board
```

---
## \#31 Posted by: dg798 Posted at: 2017-11-26T22:49:23.723Z Reads: 41

```
wow what are you using as a power supply
```

---
## \#32 Posted by: E1Allen Posted at: 2017-11-26T23:11:26.085Z Reads: 40

```
I believe it's from a computer server
```

---
## \#33 Posted by: dg798 Posted at: 2017-11-26T23:13:58.903Z Reads: 39

```
oh ok also anyone know of a cheap 12s bms
```

---
## \#34 Posted by: danielz Posted at: 2017-11-26T23:21:38.174Z Reads: 37

```
I use an cheap used 203 watt original xbox power supply off ebay with a Charsoon Antimatter 250W from banggood. Because the xbox power supply is only 12v this charger limits max wattage to arround 200w anyway.
```

---
## \#35 Posted by: ugothakd Posted at: 2017-11-29T13:22:39.251Z Reads: 32

```
Search these very forums. There are some for under $50
```

---
## \#36 Posted by: dg798 Posted at: 2017-11-29T14:01:47.527Z Reads: 32

```
Alright thanks
```

---
## \#37 Posted by: BpaoZedong Posted at: 2018-03-29T11:46:53.989Z Reads: 28

```
Is it possible to have two 6s in parallell and charge them seperately ? Do you have a soloution for that?
I have a schematic for my version, would appriceciate if you could take a look at them
.![Skjermbilde|690x347](upload://8fL7qPvYXwbFe5MLAU7VE0LA77K.JPG)
```

---
## \#38 Posted by: danielz Posted at: 2018-04-02T03:49:02.502Z Reads: 25

```
Just do what i did, but swap the series y adapter for a parallel y adapter?  the adapter acts as the loop key. Charge them with a single charger using a parallel charge board. 

Or are you try to use 4 batteries?
```

---
## \#39 Posted by: BpaoZedong Posted at: 2018-04-02T20:59:07.553Z Reads: 20

```
Im trying to use four batteries, where i want them in 6s2p. And i only have a 6s battery charger, and therefor i would like to charge them seperatly (charge 3s battery in series)  and not in parallell.
```

---

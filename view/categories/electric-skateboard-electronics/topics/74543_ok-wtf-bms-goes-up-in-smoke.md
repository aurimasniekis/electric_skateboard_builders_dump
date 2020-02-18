# Ok WTF? BMS goes up in smoke

### Replies: 26 Views: 487

## \#1 Posted by: Pete75 Posted at: 2018-11-13T09:37:17.776Z Reads: 142

```
So I purchased a cheap 10s bms of Ebay. My battery is a 10s2p samsung 30q.  I soldered up the red balance leads and found the BMS getting hot? And eventually 2 and components went up in smoke. Did I solder wrong items first ?![20181113_203023|281x500](upload://t0M4Dm5ccKlROFTmS7SYbAnUoJ1.jpeg) ![20181113_203036|690x388](upload://nwxDGAcjS9sdml6wEwYr9ZjMAdG.jpeg) ![20181113_203109|690x388](upload://D6VbjhuL0TN96mKF1Y5Zjkg5TB.jpeg) ![20181113_203114|690x388](upload://roHgnsIEGzN9eTlzjeQTdskgXXV.jpeg) 

Am I an Idiot, I cant see how just the balance leads can heat up the bms without the negative connected?
Any ideas appreciated.
```

---
## \#2 Posted by: linsus Posted at: 2018-11-13T09:43:22.932Z Reads: 136

```
most likly connected in the wrong order. Cant really tell from the pictures since i cant follow what wires goes where on the connector, or what wirescheme your BMS needs.

Also for the love of skatan cut some smoother corners on that nickel. Looks sketchy
```

---
## \#3 Posted by: linsus Posted at: 2018-11-13T09:48:00.345Z Reads: 133

```
![sketch|191x500](upload://v61k5xiuKWVi0QeMvTBrqUyJzpl.jpeg)

Only marked one picture,but you get the idea. Keep in mind balance wires dont want to sit next to something edgy as well, friction on a balance lead and you can count on some smoke. Hot glue is magic.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-11-13T09:51:48.211Z Reads: 121

```
do you have a wire diagram of your bms?
did you measure the voltage of the balance wires counting up from 1-10 in 3,6-4.2V steps ?
```

---
## \#5 Posted by: Pete75 Posted at: 2018-11-13T10:10:49.850Z Reads: 120

```
![20181113_210749|281x500](upload://a1GfmRMl4ArCrxCOir1v2MH1gz0.jpeg) ![20181113_210713|281x500](upload://od7ZEA27hrizmw6YzVn7q6xCHPq.jpeg) 
Closest to the black is cell one and it does go up in order.
```

---
## \#6 Posted by: Pete75 Posted at: 2018-11-13T10:13:23.293Z Reads: 115

```
![Screenshot_20181113-211259_eBay|281x500](upload://zqkgCcnGAs3uFQAMHlwaXBctxHL.jpeg)
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-11-13T10:15:20.655Z Reads: 114

```
Check the voltage of the pins in order, see if the voltage keeps increasing
```

---
## \#8 Posted by: Pete75 Posted at: 2018-11-13T10:16:38.259Z Reads: 111

```
Yes it does goes all the up to 34 haven't charged them fully yet. Voltage isn't dropping.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-11-13T10:21:10.325Z Reads: 108

```
did you connect + and - on your bms?
![20181113_203109|690x388](upload://lPOo33mrGXoERoT6e5tETy8pz8R.jpeg) 
or it just looks like this?
```

---
## \#10 Posted by: Pete75 Posted at: 2018-11-13T10:25:16.095Z Reads: 103

```
No all that I hooked up so far was the balance leads, the 10red and it felt warm so I thought might need the black on balance lead hooked up, then it really heated up.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-11-13T10:26:10.579Z Reads: 102

```
so no main leads connected to your bms?
i mean from the chargert to the bms
and from the bms to the battery?
```

---
## \#12 Posted by: Pete75 Posted at: 2018-11-13T10:26:56.118Z Reads: 100

```
No not even one, was that the issue?
```

---
## \#13 Posted by: Andy87 Posted at: 2018-11-13T10:28:20.007Z Reads: 100

```
could be yes.
as far as i know you need first connect the main leads, than the balance leads.
you already connected the charger, and if yes how much amps charger is it?
```

---
## \#14 Posted by: Pete75 Posted at: 2018-11-13T10:34:38.903Z Reads: 96

```
No charger connected , just building the battery pack. The reason I had the balance leads hooked up was to solder the leads to the correct length. After they were soldered I was going to solder up the charge leads. Just cant see why the bms would heat up just with the red balance leads connected?. Could be dodgy BMS.
```

---
## \#15 Posted by: Jumpman Posted at: 2018-11-13T10:49:24.231Z Reads: 95

```
Everything I’ve read about setting up a BMS suggests connecting B- first, then charge and discharge, then finally the balance connector.
```

---
## \#16 Posted by: Andy87 Posted at: 2018-11-13T11:01:46.655Z Reads: 96

```
So you soldered on the balance wires with plugged in jst plug on the bms?
If yes did you start with the black wire or with the red wires?
```

---
## \#17 Posted by: Pete75 Posted at: 2018-11-13T11:25:23.592Z Reads: 93

```
I started with the 10 red wires Andy..
```

---
## \#18 Posted by: Pete75 Posted at: 2018-11-13T20:36:24.598Z Reads: 78

```
I just noticed that the wire that is to go to p1 I have hooked up to the same cell the red discharge leads go onto.![20181113_210749|281x500](upload://a1GfmRMl4ArCrxCOir1v2MH1gz0.jpeg)  should this be p10 or does it not matter. As in p1 being closest to negative lead.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-11-13T20:53:58.472Z Reads: 66

```
First cell is where your black thick discharge wire is soldered on the negative terminal.
On this cell on the positiv side there need to be soldered the first red balance wire.
Thats than b1.
The next cell positive terminal is b2 and so on
```

---
## \#20 Posted by: accrobrandon Posted at: 2018-11-13T21:00:47.059Z Reads: 65

```
u probably did i t backwards...which i did twice.... but felt the bms get hot and unplugged before damage could occur... happens quite often during first builds... then kaput to bms!
```

---
## \#21 Posted by: longhairedboy Posted at: 2018-11-13T21:04:08.813Z Reads: 65

```
[quote="Pete75, post:10, topic:74543"]
I hooked up so far was the balance leads, the 10red and it felt warm so I thought might need the black on balance lead hooked up, then it really heated up.
[/quote]

you definitely got the balance leads in the wrong order. They will heat up quick when the logic gate for the balance column gets the wrong voltage for where it is. Then the second you complete the discharge circuit by connecting the negatives you're going to float resistors as the battery shorts itself through the BMS. 

[quote="Pete75, post:14, topic:74543"]
The reason I had the balance leads hooked up was to solder the leads to the correct length.
[/quote]

next time figure out where you need the connector to rest and just tape it down. don't ever wire balance leads in while plugged into the BMS. After you do that, the very next step should be to use a volt meter to probe each balance lead and make sure that they all count upwards in the correct order starting with 3.whatever volts, then 7.whatever, and so on up to the last pin which should be the highest. 

[quote="Jumpman, post:15, topic:74543, full:true"]
Everything I’ve read about setting up a BMS suggests connecting B- first, then charge and discharge, then finally the balance connector.
[/quote]

yes, the balance leads don't plug in until they've been checked twice or three times and the negative pack mains are connected to the cell pack side of the BMS.
```

---
## \#22 Posted by: Darkie02 Posted at: 2018-11-13T21:13:22.183Z Reads: 55

```
Well the up side you confirmed them bms balance even when not charging
```

---
## \#23 Posted by: Pete75 Posted at: 2018-11-13T21:17:14.174Z Reads: 57

```
Thank you very much for your help. I didnt think to make shore the balance leads were right, as I figured it would just do the voltage for each cell. Lesson learnt. I always thought the first cell would be the one closest to main+
```

---
## \#24 Posted by: longhairedboy Posted at: 2018-11-13T21:22:06.170Z Reads: 58

```
[quote="Darkie02, post:22, topic:74543, full:true"]
Well the up side you confirmed them bms balance even when not charging
[/quote]

... eh... ish. Balancing is a discharge process that usually happens only when the charger is present. In most BMSs. In my experience.
```

---
## \#25 Posted by: Pete75 Posted at: 2018-11-13T21:24:42.065Z Reads: 56

```
Thank you everyone for your help, it makes sense now. I appreciate the time you took to respond to my stuff up.
```

---
## \#26 Posted by: Ian-mountainboard Posted at: 2019-04-21T15:17:03.814Z Reads: 35

```
You cant connect the ballance leads to the bms until the b- is solderd to the bms. Tgen it is ok to plug in the balance leads. If this id done backwards it will burn up
```

---

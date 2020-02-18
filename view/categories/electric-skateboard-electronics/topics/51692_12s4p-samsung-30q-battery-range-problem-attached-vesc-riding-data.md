# 12s4p Samsung 30q battery range problem (attached vesc riding data)

### Replies: 27 Views: 1450

## \#1 Posted by: Mattmccrary8 Posted at: 2018-04-09T12:08:29.508Z Reads: 298

```
Ok so I have a 12s4p Tb battery and for some reason the range has drastically decreased. It continually cuts off and I can’t figure out what to do. 

Yesterday I went for a long ride and it cut off at 7-8 miles and wouldn’t turn back on till I charged it a little. I was watching the vesc app on my iPhone and the cells were around 3.6-3.5 volts coasting while the entire voltage was 44v when the board dropped. I’ll post my ride settings and have my battery cut off start at 33.00 and the cut off end at 30.00. I normally do 36-33 but lowered it to do a long ride.

![image|374x500](upload://ifp2ZCrz1py2SNftAena8rsvePK.jpeg)![image|374x500](upload://oCE8W82F5N7Pg1vtxcPaAACXgXi.jpeg)![image|374x500](upload://7tXsdaOT1TJPSwOemTigIyncPVZ.jpeg)![image|374x500](upload://n2YpQXn2g8BCOUERbBboQv9b3tz.jpeg)
```

---
## \#2 Posted by: Mattmccrary8 Posted at: 2018-04-09T12:17:37.843Z Reads: 272

```
At 5.8 miles the voltage sagged to 21 volts quickly. Does anyone know what could be causing this? Should I lower my cut off settings. 

I did update my vesc’s from 2.18 to 3.35 last night but haven’t riden yet. I’m nervous about the cut offs
```

---
## \#3 Posted by: pat.speed Posted at: 2018-04-09T12:23:39.706Z Reads: 263

```
Dead cell? Where did you get the battery and can you individually check each cell. Also make sure everything is plugged all the way in and not hanging half out
```

---
## \#4 Posted by: oyta Posted at: 2018-04-09T12:31:19.486Z Reads: 257

```
If you go down to 30V on 12s the cells are down to 2.5V. I would say that is too low for 30Q. At least you reduce the life time (number of charge cycles) a lot. I think you should stop between 36V and 39,6V - check the discharge curves of 30Q. Edit: typo
```

---
## \#5 Posted by: Mattmccrary8 Posted at: 2018-04-09T12:32:43.457Z Reads: 252

```
I got it from torqueboards and I have no battery experience so I didn’t want to open it up unless I absolutely had to.
```

---
## \#6 Posted by: Mattmccrary8 Posted at: 2018-04-09T12:34:49.950Z Reads: 247

```
Every time I read up on cut offs, people were advising around 36 and 33.6 for cut off end for 30q cells. I could be mistaken.

Is this what happens when you have a dead cell
```

---
## \#7 Posted by: pat.speed Posted at: 2018-04-09T12:39:40.312Z Reads: 241

```
33.6v IMO is the lowest you want to go with li-ion, 36v is also good as you will get lots more charge cycles.
```

---
## \#8 Posted by: oyta Posted at: 2018-04-09T12:43:48.287Z Reads: 235

```
33.6V is down to 2.8V per cell on 12S (33.6v/12s). It should be Ok, but generally speaking going lower on minimum voltage and higher on maximum voltage reduces the number of charge cycles a battery can handle. Going down to 30V equals 2.5V per cell on a 12s - that is way too low if you care about battery lifespan. I have not had dead or weak batteries (yet!) so I do not know how they perform.
```

---
## \#9 Posted by: Mattmccrary8 Posted at: 2018-04-09T12:55:12.310Z Reads: 220

```
@torqueboards got any ideas on what you think could be happening?
```

---
## \#10 Posted by: torqueboards Posted at: 2018-04-09T13:48:13.787Z Reads: 206

```
@Mattmccrary8 Not sure, but you can send us an email and send it out to us and we'll check on it for you.
```

---
## \#11 Posted by: Mattmccrary8 Posted at: 2018-04-09T13:56:24.353Z Reads: 196

```
Sounds good, just sent you a email with the ride data attached.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-04-09T14:15:04.739Z Reads: 190

```
[quote="Mattmccrary8, post:6, topic:51692"]
33.6
[/quote]

3.35per cell.. which is 40.2v... cutoff for a 12s..

But yes if you have a series pack out of balance/dropped, when you ask for the juice, the whole pack sags...
```

---
## \#13 Posted by: Mattmccrary8 Posted at: 2018-04-09T15:41:16.069Z Reads: 178

```
Ya I think the pack has to unbalanced or something. Was super tough to stay on when it hit those deep cut offs
```

---
## \#14 Posted by: Deckoz Posted at: 2018-04-09T15:50:33.691Z Reads: 174

```
If you have a hobby charger... I normally unplug the balance lead from the bms... And measure the individual cells... Find the low one. Then use a 2 pin header to charge the low cells as 1s to bring it back into viable range.

This method only works if the cell hasn't been abused... If you've done several charge cycles like this then likely the IR of that series pack is hgher and will likely no longer maintain balance due to the IR difference...
```

---
## \#15 Posted by: Mattmccrary8 Posted at: 2018-04-09T16:11:52.865Z Reads: 167

```
Ya I think I’m going to just send it in to Torqueboards once they send me a RMA. I’m just hoping it can be salvaged like you’re saying. Not trying to continually spend, just want to ride 😭
```

---
## \#16 Posted by: longhairedboy Posted at: 2018-04-09T16:29:55.260Z Reads: 163

```
bad welds/poor connections within the P groups can do this. Its not the only cause of course. I've seen bad BMSs (the charge/discharge type. not charge only) do this as well when components start to go bad.
```

---
## \#17 Posted by: Mattmccrary8 Posted at: 2018-04-09T20:24:51.842Z Reads: 144

```
Looks like there was a fault code. Mid ride it dropped to 21.3 volts. @Namasaki I saw you in a couple different forums discussing similar problems?  @Ackmaniac  

![image|374x500](upload://9vtqbkpr7n8Vl2NRiY3LBNR2hok.jpg)
```

---
## \#18 Posted by: Ackmaniac Posted at: 2018-04-09T22:00:27.505Z Reads: 128

```
Use the BMS only for charging. Kick it out of the Battery-VESC cycle.
If you don't have a BMS check your wires.
```

---
## \#19 Posted by: Mattmccrary8 Posted at: 2018-04-09T22:13:58.511Z Reads: 129

```
Is that I have to physically do to the bms or is that a setting I can change in my vesc’s. I’m running FW 3.35
```

---
## \#20 Posted by: Ackmaniac Posted at: 2018-04-09T22:16:58.111Z Reads: 131

```
Battery and VESC should have a direct connection. BMS should not be included in that cycle. And then you can have a additional cycle between the BMS and the Battery. this way the BMS is only there for charging.
```

---
## \#21 Posted by: Michael319 Posted at: 2018-04-09T22:48:32.467Z Reads: 119

```
My battery came with the bms fully wired, both for charging and discharge (12s2p 30Q). I'm having similar issues to this thread, would you still reccomend a direct connection? Seems worth trying.
```

---
## \#22 Posted by: Mattmccrary8 Posted at: 2018-04-09T23:02:14.693Z Reads: 113

```
Got it from Torqueboards? Or where did you get it at?
```

---
## \#23 Posted by: Ackmaniac Posted at: 2018-04-09T23:06:52.030Z Reads: 112

```
12S2P is a bit weak. But a BMS in the discharge cycle is always a bad idea if you ask me. Because it can cut power at any time. And it doesn't tell you anything about it's status. So it's better to only use it for charging and check the single cell voltage from time to time manually to see if the cells are roughly balanced.
Would be better if the BMS beeps when something is wrong instead of cutting power.
BTW i have no bms in any of my boards. I use a external charger or check the cells from time to time manually.
```

---
## \#24 Posted by: epss4 Posted at: 2019-01-05T20:36:01.343Z Reads: 71

```
Is it a torque board battery too??
```

---
## \#25 Posted by: Fearless562 Posted at: 2019-03-26T03:50:24.975Z Reads: 46

```
Hey man I wanted see what you ended up doing with your Battery? I have the same issues with my TB 12s4p. I took it off my board and noticed if I put a little pressure on the back with my hands it would shut off. Just trying to see if  you sent it back and what the issue was.  Thanks
```

---
## \#26 Posted by: torqueboards Posted at: 2019-03-26T04:02:12.265Z Reads: 44

```
@Fearless562 Your issue would most likely be that something is hitting the back of the LCD. There are some buttons on the back of the LCD and they are being pressed. The battery should still be on it's just the LCD that is turning off. You would have to open it up and move the components so they aren't hitting the LCD. They could of gotten shifted.
```

---
## \#27 Posted by: Fearless562 Posted at: 2019-03-26T04:31:04.914Z Reads: 40

```
Yeah it feels as though something shifterd slightly. Would that also cause the board to power on and off when riding? It seems like when I accelerate hard it kicks off and then regains power a few seconds later.
```

---

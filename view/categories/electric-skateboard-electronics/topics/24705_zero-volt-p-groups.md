# Zero volt P groups

### Replies: 28 Views: 1124

## \#1 Posted by: longhairedboy Posted at: 2017-06-06T13:23:28.082Z Reads: 138

```
this is so insane. 

ive been building my own batteries for about two years now and i thought i had seen almost everything peculiar about 18650 based packs. 

twice now the following has happened: 

i have a board that won't charge all the way. the BMS is cutting off the charger prematurely, say around 70% or thereabouts on the fuel guage. otherwise it runs fine, just doesn't charge all the way or ever act fully charged. so i figure it's orobably broken welds or maybe a bad solder on a balance lead or maybe a balance lead found a way to short, who knows. so i cut the pack open and find all good welds and solder joints. Then it's time for the volt meter. all the cells are reading 4 volts ish and seem properly balanced. 

except one p group. That one is reading 0.00v on all four cells. 

how the actual fuck does this happen? why didn't it vent or do whatever they do on over discharge? lipos would have puffed. these just sit there and play dead and affect nothing but performance. 

anyway thoughts and opinions are welcome because i'm very confused right now. Also greatful because if a cell group is going to fail, this is how i would prefer it to do so.
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-06-06T13:32:13.102Z Reads: 136

```
also its worth mentioning that simply replacing the p group works. the bms will take it back up to 100% and balance with no issue. at first i thought maybe its bad BMSs.
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-06T14:37:28.755Z Reads: 123

```
You could test the bms by using it with your new cell group and monitoring voltage as it approaches 4.2v. Perhaps the bms is overcharging the cell group to death. A severed balance lead could be causing the group to be unmonitored as well.

Is there any physical indication of damage on the cells?
```

---
## \#4 Posted by: TeleRando Posted at: 2017-06-06T16:18:16.194Z Reads: 113

```
Out of curiosity, what BMS are you using?
```

---
## \#5 Posted by: SeanHacker Posted at: 2017-06-06T16:24:54.882Z Reads: 112

```
I think I have the same problem dude. My pack only charges to 80%. Pretty sure its the BMS shitting out on me. Should have the replacement in a day or two. Hopefully it solves my problem. I'm using a SuPower BMS.
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-06-07T02:55:46.574Z Reads: 101

```
[quote="Jinra, post:3, topic:24705"]
Is there any physical indication of damage on the cells?
[/quote]

 Not that i could see. And I checked the insulation on all of the balance leads and checked the voltage at the pins in the connector for each p group. 

 [quote="TeleRando, post:4, topic:24705, full:true"]
Out of curiosity, what BMS are you using?
[/quote]

Its a Battery Supports 12S 60Amp BMS. They've been very faithful so far. Hopefully this isn't an issue with them. 

[quote="SeanHacker, post:5, topic:24705, full:true"]
I think I have the same problem dude. My pack only charges to 80%. Pretty sure its the BMS shitting out on me. Should have the replacement in a day or two. Hopefully it solves my problem. I'm using a SuPower BMS.
[/quote]

I would hate to see you waste the money but i also hope that's not the problem. Ugh. I've got 5 more sitting here that just arrived, i have to stay ahead of them because they take so long to get here. I hope they're all good.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-06-07T03:19:15.038Z Reads: 93

```
My question is why didn't the bms detect low voltage on the zero group and shut down in protection mode?

BTW, have you ever considered trying the Bestech bms on your builds?
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-06-07T03:32:59.993Z Reads: 92

```
That's the question i have too. I'm about to replace the BMS and see what happens. 

I have tried BesTech. The reason I'm using SuPower BMSs is because BesTech kind of burned me on an RMA involving three 12S BMSs. I'm not going to talk smack though, they do produce a quality product when its not DOA. I have a few 10S ones here.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-07T03:38:18.595Z Reads: 92

```
I have only ordered around 7 bms's from them and have been fortunate so far with no problems. Sorry to hear about the RMA issues.
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-06-07T03:45:40.305Z Reads: 90

```
I mean you just never know what you're going to get from who over there. They all have bad batches just like everyone else. That's why i'm so eager to get somebody in the US to start distributing something at a reasonable price. Preferably with some added features. 

I'm completely rethinking my pack structure after building all these flexy packs for bamboo mods. I want a flexy box now like evolve has and i want to go back to 7 ply decks. I have a split box scarlet on the wall now that was sick, you could bounce all over the place.
```

---
## \#11 Posted by: Pantologist Posted at: 2017-06-07T03:51:34.070Z Reads: 85

```
I had a Bestech BMS that had two of the balance resistors shorted together. That killed one parallel pack. It happened throughout use but i doubt it was a manufacturing issue. More like, should have been in a shock proof enclosure and properly cooled.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-06-07T03:57:28.654Z Reads: 82

```
was it exposed to any road dust or moisture?
```

---
## \#13 Posted by: Pantologist Posted at: 2017-06-07T04:08:36.897Z Reads: 82

```
It was a sealed ABS enclosure. I doubt any air was really getting in which was probably what led to the short.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-06-07T04:17:39.716Z Reads: 78

```
I run mine in sealed enclosures and they never overheat.  Wonder if yours just had a bad resistor that failed in service.
```

---
## \#15 Posted by: longhairedboy Posted at: 2017-06-07T19:15:21.358Z Reads: 63

```
i'm going to be replacing my BMS this afternoon. I suspect the BMS is at fault now for sure beause unlike the other time this happened, this time replacing the P group just made it shut down more. PAck voltages are stable, but it won't stay on. The BMS keeps killing it any time i put a load on it. 

So weird. We're either learning or dead, amirite?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-06-07T19:52:23.829Z Reads: 59

```
[quote="longhairedboy, post:15, topic:24705"]
So weird. We're either learning or dead, amirite?
[/quote]

That's for sure....
```

---
## \#17 Posted by: treenutter Posted at: 2017-06-07T20:46:40.525Z Reads: 57

```
@longhairedboy I had the same problem with a bestech BMS; one of the P groups completely drained to 0% while on the bench. All other P groups remained normal. The balance lead was soldered properly and I couldn't see evidence of any shorts. I replaced the BMS (and obviously the cells) and that fixed the problem for me. 

I was unlucky enough to have this happen on my first 10S build, I thought I had done something wrong!
```

---
## \#18 Posted by: Namasaki Posted at: 2017-06-07T20:49:00.326Z Reads: 58

```
Did you RMA the defective bms and if so, what was your experience with Bestech's customer service?
```

---
## \#19 Posted by: treenutter Posted at: 2017-06-08T00:12:41.195Z Reads: 53

```
@namaski I tried to RMA it. They asked me to do multiple rounds of testing w my multimeter. I did two "rounds" of this (touch various contact points with the multimeter, take pic showing result, send to their support team) Eventually I decided that neither the cost of shipping it back nor the additional tests were likely to lead to a replacement, so I stopped trying and bought another BMS. 

I think Bestech makes good stuff but if you get a DOA unit there's not an easy was to resolve it.
```

---
## \#20 Posted by: Jinra Posted at: 2017-06-08T00:20:49.812Z Reads: 51

```
Have you looked over the BMS for any burns or broken solder?
```

---
## \#21 Posted by: Namasaki Posted at: 2017-06-08T00:29:15.640Z Reads: 51

```
That sounds ridiculous.
I was under the impression that they test every board at the factory before shipping it out.
There shouldn't be any DOA unless someone on there team is wet stamping the inspection operation.

Unfortunately, there are not a lot of options for high power bms's.
```

---
## \#22 Posted by: longhairedboy Posted at: 2017-06-09T03:08:50.300Z Reads: 46

```
its totally clean, like brand new clean. 

So what i did was tear into the pack itself again and this time  i found a few things. it looks like the balance wires had intermittently started shorting and one of them cooked inside the insulation until it was no longer conductive. Ive actually seen that happen in front of me. The superworm type balance lead wire has insulation on it that can take those kinds of temps breifly, and breifly is all the wire can handle so the short cooks the balance leads copper like a fuse and leaves the insulation intact. When it happens it looks like a light is walking through the wire on the inside, then its gone.  Which is way better than that crap insulation on the balance leads that come with the BMSs, that stuff just melts instantly almost and would probably cause another short. Anyway between that and some other weirdness the whole pack is basically useless. I'll probably save the good P groups and cobble together a short lived beater battery out of them at some point. 

So i guess this wasn't exactly like the last time.
```

---
## \#23 Posted by: Namasaki Posted at: 2017-06-09T04:17:01.287Z Reads: 44

```
So nothing wrong with the bms then?
On one count of battery slaughter, we the jury find the  defendant mr. BMS, Not Guilty?
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-06-12T13:53:45.036Z Reads: 40

```
yeah apparently the BMS was fine. Just the cells were screwy. 

Its so weird.
```

---
## \#25 Posted by: Jinra Posted at: 2017-06-12T14:33:59.677Z Reads: 40

```
Perhaps it was a rogue cell that took out the whole parallel group.
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-06-13T18:09:42.787Z Reads: 36

```
Probably a foreign intelligence cell.
```

---
## \#27 Posted by: Jinra Posted at: 2017-06-13T18:12:51.964Z Reads: 36

```
Did you get your 18650s from Russia? :laughing:
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-06-13T18:35:33.925Z Reads: 35

```
Its possible the spy cells have infiltrated US distributors, we're going to have to assume the worst and go to DEFCON ZERO. EVERYONE IS BURNED. TORCH YOUR BOARDS AND PHONES. OBTAIN RUN BAGS AND MEET AT PRE-ENCODED RENDEZVOUS POINTS. THE PACK IS PUFFED. I REPEAT: THE PACK IS PUFFED
```

---

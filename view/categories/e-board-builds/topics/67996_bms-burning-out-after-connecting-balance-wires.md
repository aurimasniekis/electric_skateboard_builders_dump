# Bms burning out after connecting balance wires

### Replies: 23 Views: 614

## \#1 Posted by: Rions Posted at: 2018-09-14T08:44:22.403Z Reads: 116

```
I have a 60amp bms that i am connecting to a 10s 3p 36v battery pack.i have only a P- and B- plus balance wired with black negative and red positive on each end.

I require a break for charger (and also want to add  on/off switch).i have triple checked all soldering and followed diagrams from other builders on this forum however my bms smokes up once i plug in balance cables.any ideas where im going wrong or videos/images i can download.Usually working with bms that have 3 cables including the charge one.

 ![11|281x500](upload://bAxAb1k4Zq1yZentPJuqgImLJxr.jpg)![20180914_182818|281x500](upload://tfB0ejZN8Aada6Epnn3vvKAkr1R.jpg)
```

---
## \#2 Posted by: WARMAN Posted at: 2018-09-14T09:03:51.445Z Reads: 108

```
Plenty of info in this thread on wiring...
https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179?u=warman
```

---
## \#3 Posted by: rich Posted at: 2018-09-14T10:27:50.186Z Reads: 97

```
[quote="Rions, post:1, topic:67996"]
followed diagrams from other builders on this forum
[/quote]

The most important diagram is the one of your BMS, link?
In general it's better to fully understand how a BMS works before connecting.

It seems like all your connections are correct (if discharge/charge is same port). 
Did you measure the increasing voltage from cell 1 to 10 on balance plug to get sure if the order is right?

If you mixed up the order of balance wires the BMS would smoke but it can also be faulty.
```

---
## \#4 Posted by: Rions Posted at: 2018-09-14T22:51:27.308Z Reads: 66

```
Yes i did follow all balance wires and they all jumped up 4v till end 36v that is from  first red working down to the end black.......thanks for the reply mate just cant seem to pinpoint the issue
```

---
## \#5 Posted by: pat.speed Posted at: 2018-09-14T23:02:37.057Z Reads: 65

```
What did you plug in first, balance leads or main leads? Some bms modules can be killed from plugging in the balance leads first
```

---
## \#6 Posted by: Rions Posted at: 2018-09-14T23:17:09.668Z Reads: 63

```
Just now i tried plugging in balance first as i had plugged balance in last and still smoking up.these balance cables are definitely in correctly    getting frustrated
```

---
## \#7 Posted by: Rions Posted at: 2018-09-14T23:18:51.285Z Reads: 60

```
Thanks mate have checked these out
```

---
## \#8 Posted by: pat.speed Posted at: 2018-09-14T23:45:20.473Z Reads: 54

```
Is the first lead of the balance wires connected to the main negative battery lead or the positive one?

And some more photos might help
```

---
## \#9 Posted by: Rions Posted at: 2018-09-15T00:03:09.626Z Reads: 54

```
Black balance wire is connected to battery pack end negative and last red balance wire is connected to start positive red of battery pack.
In terms of correct position on actual bms the left has a -negative symbol and the right has the +positive symbol so one assumes this is correct![24|500x500](upload://jH0HzV19heX9gUpNdqVF1r47J9a.jpg)
```

---
## \#10 Posted by: Rions Posted at: 2018-09-15T00:08:38.015Z Reads: 51

```
![11|281x500](upload://rwONkGQZBW1TVBBTjlPJrBUgJSg.jpg)
```

---
## \#11 Posted by: pat.speed Posted at: 2018-09-15T00:57:20.726Z Reads: 49

```
Hmm...yes this is correct, I’m not sure what else could be wrong with the wiring. It seems it may actually be a problem with the bms, maybe an internal short
```

---
## \#12 Posted by: Rions Posted at: 2018-09-15T01:16:06.093Z Reads: 49

```
I have now tried 2 of the same bms and same result.......perhaps the rating is not correct however it is a 36v bms with 60amp
```

---
## \#13 Posted by: Rions Posted at: 2018-09-15T01:18:34.509Z Reads: 48

```
Thanks for your replys,i appreciate the help....might just have to minus the bms till i figure it out
```

---
## \#14 Posted by: TiMMaTTie Posted at: 2018-09-16T09:15:04.867Z Reads: 40

```
Do you have a link to the BMS you bought?
```

---
## \#15 Posted by: DeathByBacon Posted at: 2018-09-16T10:11:00.333Z Reads: 37

```
Isn't black supposed to be the first and a red at the end with the full voltage reading of your pack?
```

---
## \#16 Posted by: Benjamin899 Posted at: 2018-09-16T10:12:35.212Z Reads: 37

```
@Rions first black goes to the negative of the first cell group.
https://youtu.be/m4DGDkwFr54?t=61
![bms|690x313](upload://wPjvjFd3QWRpCrexfkEZzJYstDR.PNG)
```

---
## \#17 Posted by: Rions Posted at: 2018-09-16T11:24:20.490Z Reads: 32

```
It was off ebay will look at purchase history
```

---
## \#18 Posted by: Rions Posted at: 2018-09-16T11:28:38.964Z Reads: 32

```
Looking at your video link and diagram this is the same order as i have my wires in??? Sorry not sure if i understand what it is your refering to.any help is of course appreciated
```

---
## \#19 Posted by: Rions Posted at: 2018-09-16T11:33:28.260Z Reads: 31

```
Oh sorry think  getting you- iv started with positive to begin sequence whereas it should start with negative right?
```

---
## \#20 Posted by: pat.speed Posted at: 2018-09-16T11:43:25.206Z Reads: 32

```
Yes it starts with the negative, the black wire connects to the main negative lead of the battery and then each wire after that connects each series connection in sequence
```

---
## \#21 Posted by: gigoy Posted at: 2018-09-16T11:53:55.024Z Reads: 29

```
[quote="Rions, post:9, topic:67996"]
Black balance wire is connected to battery pack end negative and **_last_** red balance wire is connected to **_start positive red_** of battery pack.
[/quote]

Black balance wire to where black main negative is, **_last_** red balance wire to where the **_main positive is a.k.a last pack of the series_**.
```

---
## \#23 Posted by: Benjamin899 Posted at: 2018-09-16T12:02:33.177Z Reads: 30

```
@Rions you basicly wired your battery in the wrong order. that black balance lead goes to the battery negative and from there you start. That is your b1, but from that picture it looks more like you started your b1 at the postive end, that why it shorts.
```

---
## \#24 Posted by: Rions Posted at: 2018-09-16T19:16:49.602Z Reads: 24

```
Yes makes sense
```

---

# Space Cell 3 not charging anymore

### Replies: 13 Views: 601

## \#1 Posted by: TheLastEnting Posted at: 2017-09-13T13:21:04.664Z Reads: 86

```
So recently I have been having trouble charging my space cell 3, I've not really cycled it more than I'd say 15 times since buying it, but the other day when plugging in the charger the light stayed green, and didn't turn red to indicate it was charging, even though the battery level indicator was reading 17%.

I tried replacing the charger, and it didn't fix it, so that ruled out the charger. Then while running tests and measuring voltages I managed to short out the charge port and blow it up, so I have also since replaced that, but it hasn't solved the problems either which rules out the charge port as well.

I didn't particularly feel like completely tearing apart the battery to try and diagnose and fix the problem myself, so thought i would come here for some advice first. Thanks for any help in advance guys!
```

---
## \#2 Posted by: barajabali Posted at: 2017-09-15T20:38:45.223Z Reads: 71

```
Hit up Enertion to see if its in warranty. Either way if youre in the US I can fix it for you.  don't open it until Enertion gives you the OK because you will void your warranty
```

---
## \#3 Posted by: Mikenopolis Posted at: 2017-09-15T21:09:24.517Z Reads: 72

```
"out of office" my a$$! hahaha.
```

---
## \#4 Posted by: Dornacht Posted at: 2017-09-15T21:15:00.717Z Reads: 70

```
Enertion most likely won't if it's older than a year, they never did mine, I had a dead cell so the bms didn't charge the board, check the last 2 cells closest to the bms, sometimes they wouldn't cut the plastic barrier long enough to and the cells spark out, at least this was what happend to mine
```

---
## \#5 Posted by: barajabali Posted at: 2017-09-15T21:16:56.502Z Reads: 65

```
hahaha yea i am. The check out on my site is down. But i know this is a process so by the time im up and running we can make it work out.
```

---
## \#6 Posted by: TheLastEnting Posted at: 2018-01-22T20:30:46.153Z Reads: 56

```
Okay, so after a few months out of the shop I've finally managed to get some time in and got around to doing a bit more testing and reading etc. and I think I've narrowed down the problem now, but could definitely use someone with more knowledge on the topic's help.

So the same symptoms persist, battery will discharge (currently still holding 17% charge, 34.6V on a 10s pack), however when plugged in to charge, the charger will not indicate battery is charging and after leaving it for about an hour or so just to make sure it wasn't the charger, the battery definitely isn't charging.

So next port was to check all the connections, I tried replacing the charger and charge port anyway, but it didn't help things, still not charging, but I'm certain all of that's working now at least.

I started doing some reading, and found people with similar symptoms were finding unbalanced cells in their packs, so fearing the worst I took measurements over all of the cells in my pack, and all were within 0.1V of each other, and measuring the voltages over the balance leads I'm getting the same over those, as you'd expect to see for a working pack.

So given everything is still connected, everything still balanced, no immediate faults that I can find... Is it safe at this point to assume that my BMS is dead...?
```

---
## \#7 Posted by: myreala Posted at: 2018-01-22T22:02:34.310Z Reads: 46

```
Doesn't really leave much room for anything else. Most probably the BMS.
```

---
## \#8 Posted by: TheLastEnting Posted at: 2018-01-23T11:52:13.677Z Reads: 42

```
Then I need to try and find a good source for a UK BMS, any leads/advice?
```

---
## \#9 Posted by: longhairedboy Posted at: 2018-01-23T12:05:03.837Z Reads: 39

```
probably just leaked a few watt hours. plug the hole and pour some more in, you'll be fine.
```

---
## \#10 Posted by: TheLastEnting Posted at: 2018-01-23T13:07:05.756Z Reads: 36

```
I don't suppose you have a more detailed method to...

[quote="longhairedboy, post:9, topic:33041"]
plug the hole and pour some more in
[/quote]

Cheers
```

---
## \#11 Posted by: longhairedboy Posted at: 2018-01-23T13:45:20.997Z Reads: 33

```
[quote="TheLastEnting, post:6, topic:33041"]
I started doing some reading, and found people with similar symptoms were finding unbalanced cells in their packs, so fearing the worst I took measurements over all of the cells in my pack, and **all were within 0.1V of each other**, and **measuring the voltages over the balance leads I’m getting the same over those**, as you’d expect to see for a working pack.

So given everything is still connected, everything still balanced, no immediate faults that I can find… Is it safe at this point to **assume that my BMS is dead**…?
[/quote]

Correct. Something is wrong with the BMS. 

The best way to pour more watt hours back into your pack is to replace the BMS. There may be a spare one floating around on the forum somewhere.
```

---
## \#12 Posted by: TheLastEnting Posted at: 2018-01-23T14:36:59.427Z Reads: 29

```
Thanks for the confirmation, I was worried this might be the case.

I'm trying to keep this repair on the cheaper side for now, so considering wiring in a lower rated BMS into the battery for charging, and bypassing for discharge and setting the soft limits in the VESC. In your professional opinion, recommended for a fix or should I just wait and get a better BMS?

Thanks again!
```

---
## \#13 Posted by: longhairedboy Posted at: 2018-01-23T15:04:32.758Z Reads: 27

```
that would be ok as long as you don't run anything else on it that could potentially drain the pack over time beyond its lower limit. 

The LVC on the ESC only turns off the ESC. ITs not going to turn off the board or kill your under lights. That's one reason i prefer not to bypass discharge on customer boards, but in DIY its fine as long as you're mindful.
```

---

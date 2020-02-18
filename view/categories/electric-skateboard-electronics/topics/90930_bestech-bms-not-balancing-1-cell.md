# Bestech BMS not balancing 1 cell

### Replies: 20 Views: 294

## \#1 Posted by: Z4MSupreme Posted at: 2019-04-17T21:49:24.687Z Reads: 67

```
Hi,
Recently I had a problem with my battery pack (10s3p 30q pack with an 80A bestech BMS) with the BMS cutting out while accelerating. This was due to one of the cells being much lower than the others and cutting out. I thought that it was a dodgy group of cells and replaced them today. 

However after charging the battery pack all the cells were balanced except the first cell that was at 3.6V. before I wired the new batteries they were 3.6v meaning that the BMS did not charge them. 

I'm not sure if I have a problem with my BMS or my charging brick (cheap eBay charger). 

Any help would be much appreciated, thanks
```

---
## \#2 Posted by: Arzamenable Posted at: 2019-04-17T21:54:48.907Z Reads: 66

```
Take a look at the resistors inline w/ the corresponding P group on the bms. Sometimes those go bad, sometimes visibly so.
```

---
## \#3 Posted by: Z4MSupreme Posted at: 2019-04-17T21:58:34.137Z Reads: 66

```
Thanks. Could it also be due to the BMS not being able to balance groups that are to big of a different voltage?
```

---
## \#4 Posted by: Arzamenable Posted at: 2019-04-17T22:08:18.978Z Reads: 62

```
I had similar things happen, replacing p groups back to back. Blamed the bms. 

I don’t know your bms’ thresholds. You could try taking a voltmeter to the groups during charging.
```

---
## \#5 Posted by: Z4MSupreme Posted at: 2019-04-17T22:09:49.352Z Reads: 57

```
Why do I need to check voltages while charging? What am I looking for? Thanks
```

---
## \#6 Posted by: Arzamenable Posted at: 2019-04-17T22:12:02.734Z Reads: 55

```
Haha, I suppose there are better ways. Thinking out loud. 

Ive been using lipos lately and I frequently have a cell checker in balance leads.
```

---
## \#7 Posted by: Z4MSupreme Posted at: 2019-04-17T22:23:13.532Z Reads: 50

```
I've got a cell checker and a the cells are at 4.2v while just one is at 3.6V. I've been reading that a BMS cannot balance when there is such a big difference in voltages. Could i charge the individual cell with a lipo charger while it is wired in the pack so that it brings it closer to the others to be balanced?
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-18T03:04:53.665Z Reads: 42

```
You do know that the bam does not charge the cell right?

I don’t understand how that one cell stayed at 3.6v though, as even when you charge straight through the power leads every p group should still be charged up
```

---
## \#9 Posted by: b264 Posted at: 2019-04-18T03:07:33.748Z Reads: 43

```
[quote="Z4MSupreme, post:7, topic:90930"]
Could i charge the individual cell with a lipo charger while it is wired in the pack so that it brings it closer to the others to be balanced?
[/quote]

Yes.<blahblahblah>
```

---
## \#10 Posted by: goldrabe Posted at: 2019-04-18T03:20:24.355Z Reads: 39

```
You can charge individual cell groups through the  jst balance connector with a TP4056 USB  charging circuit like in the photo. ![20180722_083335|281x500](upload://177qhJCMGzBkck60A0B9y25byyb.jpeg)
```

---
## \#11 Posted by: b264 Posted at: 2019-04-18T03:44:58.619Z Reads: 35

```
Be extra careful not to short out the P-group doing this.
```

---
## \#12 Posted by: goldrabe Posted at: 2019-04-18T03:50:18.819Z Reads: 35

```
Yeah I guess if he has a balance charger on hand it's easier and faster. Took two days of charging to get the pack in to 0.05V accuracy. After that I figured that the cells where dead and threw this peace of Chinese fire hazard out.
```

---
## \#13 Posted by: RedBaron Posted at: 2019-04-18T04:01:24.415Z Reads: 34

```
You can test the resistors by setting a volt meter to test resistance. If memory serves me right bestech uses 30ohm resistors.
```

---
## \#14 Posted by: Andy87 Posted at: 2019-04-18T05:47:20.257Z Reads: 30

```
The bms should be disconnected in that case, I guess.

As min the balance adapter.
```

---
## \#15 Posted by: Eboosted Posted at: 2019-04-18T06:11:48.830Z Reads: 27

```
The BMS won't balance if the difference between pgroups voltage is too high.

Take off your battery and balance manually.

If you get cutouts during braking on fully charge battery your problem is not an unbalanced pgroup but a BMS protecting the battery from overcharge buy cutting all connection between ESCs and battery
```

---
## \#16 Posted by: Z4MSupreme Posted at: 2019-04-18T06:49:11.696Z Reads: 23

```
Great will give that a try😀. Thanks
```

---
## \#17 Posted by: Z4MSupreme Posted at: 2019-04-18T06:50:04.677Z Reads: 23

```
I've got a very similar liion module, might do it that way as I don't think my lipo charger has a Liion setting. Cheers 👍
```

---
## \#18 Posted by: Z4MSupreme Posted at: 2019-04-18T07:21:08.683Z Reads: 22

```
![IMG_20190418_081813|666x499](upload://zIKqEymrlMc8Z2QT6Ygd06RuiKs.jpeg) 

I've just put that cell on charge. does this looks ok to you?
```

---
## \#19 Posted by: goldrabe Posted at: 2019-04-18T07:39:35.377Z Reads: 19

```
I can not say for sure. Your module is different, I connected the two balance leads neighboring each other and worked my way up from the black minus lead.\
Did you located the low group? Sometimes this small modules charge cut off is not accurate, check the unbalanced group sorroughly for its charging status.
```

---
## \#20 Posted by: Z4MSupreme Posted at: 2019-04-18T07:52:15.371Z Reads: 18

```
Ok. Thanks. I located the lower cells as the first group. I'll keep checking on the voltage 👍
```

---

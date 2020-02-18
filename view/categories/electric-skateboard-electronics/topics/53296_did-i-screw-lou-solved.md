# Did I screw Lou? Solved

### Replies: 18 Views: 1271

## \#1 Posted by: Chase Posted at: 2018-04-24T01:47:47.466Z Reads: 324

```
Posted this earlier but I figured I’d give it its own topic to get the proper help.

So I decided to upgrade to 30q to combat voltage sag. I just switched the cells and re-wired the bms. When I first plugged the battery into the speed controller it came on and ran fine. Now this morning after charging the cells, when turning the board on , the esc beeps to show power then the whole board shuts off. The only thing different from when I tested last night is I crammed the battery case cover back on. The only thing I could think of happening was some sort of solder joint inside the battery broke when I stuck the case cover back on. The weird thing is my multimeter still shows 37 V so if the battery was messed up why is it still showing voltage? If the esc was messed up why would it start up then shut back off?

![image|666x500](upload://ghWt9UiEhcqFh3mqDQHvykKhjVN.jpeg)![image|666x500](upload://XKiYorZnIC7DRyMajHtWNgyM9d.jpeg)
```

---
## \#2 Posted by: Chase Posted at: 2018-04-24T19:46:30.646Z Reads: 251

```
If anyone cares I fixed this. When snapping the case back together, a plastic piece was pulling off one of my terminal connections. It’s strange that the multimeter was still reading voltage.
```

---
## \#3 Posted by: b264 Posted at: 2018-04-24T19:52:58.693Z Reads: 244

```
That the Lou board only came with a 10S1P of Panasonic PF cells is hilarious
```

---
## \#4 Posted by: mrquin Posted at: 2018-04-24T20:28:13.523Z Reads: 234

```
How does it feel with the new batteries?  More power?  More speed?
```

---
## \#5 Posted by: PredatorBoards Posted at: 2018-04-24T20:58:09.331Z Reads: 215

```
I imagine just less sag and more range. The bottleneck is the ESC
```

---
## \#6 Posted by: Chase Posted at: 2018-04-24T21:10:08.777Z Reads: 205

```
 It’s all about the sag. The old batteries would have significant loss after just a few seconds of going uphill. Now I can blast up but it will still suddenly slow after going full throttle uphill for about 30 sec. Havent tried the range yet. This is the dual hub version btw with a replaced esc to the dual sine sold by diyeboard.
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-04-24T21:21:15.485Z Reads: 196

```
The battery should not read 37 volts, once fully charged ut should read 42 volts
```

---
## \#8 Posted by: Chase Posted at: 2018-04-24T21:32:28.614Z Reads: 190

```
Yeah that’s what I meant to say. It does.
```

---
## \#9 Posted by: Chase Posted at: 2018-04-26T00:45:39.995Z Reads: 165

```
For some reason my brakes now start to studder/slip every so often. This just happened after switching to the 30Q cells. Any ideas why?
```

---
## \#10 Posted by: ARetardedPillow Posted at: 2018-04-26T00:53:52.593Z Reads: 158

```
Are you braking with the battery fully charged?
```

---
## \#11 Posted by: Chase Posted at: 2018-04-26T00:57:15.881Z Reads: 151

```
No. If I do that the board will cut off all together. This is different. It just slips when I do long brakes like going slow down a hill. This is at all battery levels.
```

---
## \#12 Posted by: Chase Posted at: 2018-04-26T18:39:42.366Z Reads: 143

```
Yeah so the battery rattled the connections loose again. It’s because I was trying to do all the soldering/ spot welding without taking the bms out of the case. The wires are cut to extend to the terminals and not a bit closer. Ideally I’d be able to find a small 8 pin bms wire to have more to work with when I put this back together again. May just have to get rid of the case because of the cramped space.
```

---
## \#13 Posted by: Chase Posted at: 2018-05-05T02:35:23.566Z Reads: 116

```
So maybe someone can tell me what is going wrong. Ever since I switched to the 30q cells the board will work fine then about 30 min in it just cuts off entirely. If I push it I can hear the esc beep to try to power back on but the battery won’t supply it with power. After a couple of hours it will start to work again. This all started after switching to the 30Q cells. I’m new to this. Is the stock batteries bms somehow responsible? Any other ideas would be greatly appreciated. All the solder spots are good. It seems to happen right after getting recharged all the way but that may just be a coincidence.
```

---
## \#14 Posted by: DeathCookies Posted at: 2018-05-05T21:52:25.389Z Reads: 90

```
Maybe the Esc is Low quality stuff and is not build for a good battery supply and overheats with the Extra current of the 30q?
```

---
## \#15 Posted by: Chase Posted at: 2018-05-05T22:57:53.940Z Reads: 87

```
I don’t think it’s the esc. I replaced the stock esc with the dual sine Belt esc from diyeboard. It’s supposed to be able to handle 60 amps I think.
```

---
## \#16 Posted by: Chase Posted at: 2018-05-08T01:21:51.026Z Reads: 70

```
So instead of a pin connector, the balance wires are glued onto the bms chip. I think the reason it was cutting out is because a couple of the wires were coming loose.
```

---
## \#17 Posted by: PDXroses Posted at: 2018-06-25T01:00:31.838Z Reads: 59

```
Can you change the ESC setting to combat sagging?
```

---
## \#18 Posted by: PredatorBoards Posted at: 2018-06-25T04:15:25.529Z Reads: 42

```
 Besides running in a slower speed mode that draws less current no. Your other option is to use cells win higher CDR. The higher the CDR,l (in relativity to the current being drawn by the board) the lower the voltage sag.
```

---

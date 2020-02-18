# Have I Killed my LIPO? like an idiot

### Replies: 12 Views: 1222

## \#1 Posted by: LukeL Posted at: 2016-11-19T03:33:33.492Z Reads: 136

```
I've had my board running for a month now just trying to make it a bit prettier (still using tupperware), I've spent past few hours trying to get my mad monkey GT2B mod to work (it's still not). I got it to bind with the receiver but the throttle does nothing so i thought i'd check the throttle display thing on the BLDC tool, with my wire harness I usually disconnect one of my 5S lipos and short out that connection so when programming the VESC i'm only using 5S instead of 10S.

It's late and I messed up by plugging my loop key into my spare lipo instead of the the interrupt, there was a spark, the metal connections in the xt90's are melted and the cell voltages are very unbalanced.

<img src="/uploads/db1493/original/3X/8/f/8f5f66028131accdcccb775cec6bec1b1eb603cb.jpg" width="690" height="471">

(Loop key on left, LIPO on right)

I guess well over 100A went through it to deform the metal like that

The cell voltages are 4V, 8V, 12.2V, 16.3V, 20.4V

Any advice on what i should do? I've put it in a lipo safe bag for now, is it safe to plug into an IMAX b6 if i put a new connector on it? if it did balance would it be safe to use? if not how am i supposed to get rid of it?
```

---
## \#2 Posted by: Pantologist Posted at: 2016-11-19T03:36:37.625Z Reads: 129

```
Once you short circuit the battery like that, it discharges super high current and unbalances the cells. The capacity of the cells drops a lot. That is what happened to me for one of my battery packs. Might be usable still. I wouldn't take the risk though. LiPos are scary when they cath fire :P
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-11-19T03:45:11.824Z Reads: 125

```
I overdischarged my lipos at one point, managed to get them fixed by following a tutorial similar to this one.

https://www.youtube.com/watch?v=bmOhUO6vbak

Hope it helps.
```

---
## \#4 Posted by: Hummie Posted at: 2016-11-19T03:50:17.810Z Reads: 114

```
Iwrite the voltage they're at now on them and balance and charge and keep going.  Watch it charging and see if it gets warm or puffy and the same when you discharge it hard.   It's probably good
```

---
## \#5 Posted by: barajabali Posted at: 2016-11-19T04:20:15.847Z Reads: 104

```
Your cells aren't that off balance.  You measured from the negative to each cell. If you measure each cell individually your highest vs lowest is only off by .2 v. A quick discharge and full balance recharge might fix it. Swap out your xt90 I think you're fine
```

---
## \#6 Posted by: LukeL Posted at: 2016-11-19T04:51:34.545Z Reads: 97

```
Ah I see that now, thanks, how I didn't realise that I don't know
I'm going to get some sleep and try it out tomorrow, is there anyway to tell if it's damaged them in any other way like reduced discharge rate? and will it effect me connecting it in series? I know people say to use batteries with similar usage
```

---
## \#7 Posted by: barajabali Posted at: 2016-11-19T04:55:56.491Z Reads: 92

```
you'll be fine. lipo's arent as bad as people claim them to be. if you want, you can oen it up and take a look at the solder tabs to make sure they're not fried.  Sometimes that happens to the middle most series connection acts as a fuse, it just explodes. But if it is you can just reconnect it and solder it. (99% chance it didnt happen to you) 

You can connect in series. discharge rate wont be affected.  
If you ask me, pretend like nothing even happened.  If you see puffing then start worrying but a little short isnt gonna kill your pack.
That connector is toast though lol worst one ive ever seen.
```

---
## \#8 Posted by: NNGG Posted at: 2016-11-19T06:49:01.524Z Reads: 70

```
. 
ALWAYS keep them in some sort of container that is metal of a lipo safe bag. I have heard too many horror stories that lipos spontaneously catch fire or melt down form poor quality control of ba chargers.  

I shorted a 3S lipos very quickly accidentally and It puffed up a little and a tab was un-soldered. But now its still running strong after ~50 cycles. Be careful man.
```

---
## \#9 Posted by: DilatedPupils Posted at: 2016-11-19T07:33:56.885Z Reads: 64

```
Might be better to use a different kind of connector to avoid this from happening again. Maybe use xt60 on your battery.
```

---
## \#10 Posted by: Hummie Posted at: 2016-11-19T08:48:19.131Z Reads: 59

```
the xt90s plugs I like and use but soldering them is dangerous as well as all those xt style plugs because you have to have both battery leads exposed close beside each other before you slide up the cover.  You can't heat shrink one side and then the other.  Easier to short
```

---
## \#11 Posted by: SORRENTINO Posted at: 2016-11-19T14:55:52.959Z Reads: 49

```
Measure the IR of the cells, only way to tell if they are good or not still!
```

---
## \#12 Posted by: LukeL Posted at: 2016-11-20T00:22:01.908Z Reads: 29

```
currently discharging it, seems fine there's no heat and the pack isn't puffy
```

---

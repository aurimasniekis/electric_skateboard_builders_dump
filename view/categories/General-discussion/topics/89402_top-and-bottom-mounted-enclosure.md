# Top and Bottom Mounted Enclosure?

### Replies: 20 Views: 274

## \#1 Posted by: DEEIF Posted at: 2019-04-05T00:36:15.009Z Reads: 100

```
Hi! I was wondering if anyone had built a board which had an enclosure in the bottom, for a small lightweight battery and esc, and had an “Extended Range” Battery mounted on top of the deck for long rides. I was thinking I could do this with a parralel connector so that when it wasn’t connected to the ER battery I could just put a “loop key” in. Then when it was going to be used the loop key would be replaced by a battery. Would this be possible and/or has anyone done this before?
```

---
## \#2 Posted by: b264 Posted at: 2019-04-05T00:40:46.033Z Reads: 97

```
It was discussed [in another thread](https://www.electric-skateboard.builders/t/range-extender-plugged-into-charge-port/64327).  You can't just connect lithium batteries together like that.  The best you could do is use one to charge the other one through a custom circuit you'd have to design yourself.
```

---
## \#3 Posted by: DEEIF Posted at: 2019-04-05T01:12:16.498Z Reads: 87

```
Ah ok! I think I’ll just go with a higher ah pack then!
```

---
## \#4 Posted by: b264 Posted at: 2019-04-05T01:13:36.044Z Reads: 82

```
To be clear, you can connect them together, but you can't connect and disconnect them without balancing them first.  Each disconnection requires you to rebalance the two packs before you can connect them together again.
```

---
## \#5 Posted by: DEEIF Posted at: 2019-04-05T01:15:47.977Z Reads: 75

```
Oh, so if I had a bms in both, and balanced them, say the night before, then they would be fine if connected in this way?
```

---
## \#6 Posted by: b264 Posted at: 2019-04-05T01:16:36.123Z Reads: 74

```
No.  They have to be balanced together with some sort of custom circuit that you'd have to make yourself.  Or charged to exactly the same voltage.

You could in theory charge both packs to exactly 42.0V for example and then connect them together.  But if they aren't matched when you connect them together, there might be fire.
```

---
## \#7 Posted by: DEEIF Posted at: 2019-04-05T01:17:14.356Z Reads: 73

```
So maybe having some sort of 2 way bms?
```

---
## \#8 Posted by: Esk8enginneer Posted at: 2019-04-05T01:32:02.694Z Reads: 75

```
Batteries in parallel share the amp load so it would be best practice to have two batteries that are the same capacity (mAh).  And yes the cell voltages need to be the same when you make the parallel connection.  This is done all the time in the rc hobby world.  The batteries in our boards have these connections that is why it is important to make sure all your cell are at the same voltage when you build your battery.
```

---
## \#9 Posted by: Pedrodemio Posted at: 2019-04-05T01:39:55.627Z Reads: 72

```
If you always remember to have them fully charged before connecting it’s all good, or the same voltage

The problems is the day you mess up and forget that they are unbalanced

What you can do (and it’s what I’m doing in my board) is connected the external pack on the charge port of a good quality BMS, like the one @SimosMCmuffin is making

If the current between both packs is too big the BMS will simply cut the connection, if the voltage of the external pack is lower than the main it will no be connected until the main pack drops

For how much current you should allow some math is needed, taking in account the maximum charger and discharge current of both packs and their respective internal resistance

For example, I calculated that when connecting my main 10S5P of 30Q cells in parallel to my 10S3P of NCR GA cells the maximum allowed voltage difference should be 2 V and 7,5A since one is dependent on another the BMS will do it for you, but if you would do it manually it would have to be lower than 2 V
```

---
## \#10 Posted by: DEEIF Posted at: 2019-04-05T01:45:18.767Z Reads: 64

```
@Pedrodemio
 Alright, so if I understand this correctly what your saying is that it will work if I say use a 12s4p pack of 30Q in my board and then have a 12s5p pack of 30Q as an external pack. If I charged both batteries to a true 100% with a bms so that both packs balanced. I then connect the 12s5p pack to the charge port of the 12s4p pack, this would work?
```

---
## \#11 Posted by: Pedrodemio Posted at: 2019-04-05T02:20:57.300Z Reads: 58

```
Only the charge port if you are using a BMS to limit the current

If you are doing it manually, use something like a XT60 connector, independent from the one you normally use to charge you board, and with a fuse between this connector and the battery

Connecting this way you allow the load to be distributed between both batteries, so the wiring and everything else must be capable of handling the load
```

---
## \#12 Posted by: DEEIF Posted at: 2019-04-05T02:35:09.980Z Reads: 52

```
Alright Thanks! So once both batteries are fully charged to 100% I just plug the 12s5p into the charging port of the 12s4p...
```

---
## \#13 Posted by: b264 Posted at: 2019-04-05T02:37:26.763Z Reads: 49

```
Problem is, if you rely on that strategy, then one day you will accidentally connect them when they aren't matched at 100% charge and something bad will happen.  Humans make mistakes.  But aside from that, yes everything @Pedrodemio  said is spot on, especially this part

[quote="Pedrodemio, post:9, topic:89402"]
The problems is the day you mess up and forget that they are unbalanced
[/quote]

So keeping them connected together is the best strategy.
```

---
## \#14 Posted by: DEEIF Posted at: 2019-04-05T02:39:51.890Z Reads: 44

```
Alright Thanks! I think I will try to design something that when the battery is not at a complete 100% it says “Do Not Plug In” although I’m not sure how to design this exactly...
```

---
## \#15 Posted by: b264 Posted at: 2019-04-05T02:41:09.264Z Reads: 43

```
That strategy will not work in the long-term.
```

---
## \#16 Posted by: ryansinatra Posted at: 2019-04-05T02:46:42.057Z Reads: 39

```
Every high end Gotway EUC I ride connects battery packs in series. Each pack has their own separate BMS. Never had an issue disconnecting and connecting them when doing maintenance. Maybe ive been lucky
```

---
## \#17 Posted by: b264 Posted at: 2019-04-05T02:57:12.662Z Reads: 38

```
He's talking about parallel and not series.
```

---
## \#18 Posted by: ryansinatra Posted at: 2019-04-05T03:05:29.317Z Reads: 38

```
Sorry I meant parallel my bad
```

---
## \#19 Posted by: b264 Posted at: 2019-04-05T03:10:06.409Z Reads: 37

```
If you connect them when they aren't the same voltage, they will balance and if that balance current exceeds the maximum charge current of the pack, bad things happen.  If you're using BMSs that helps a lot, too.
```

---
## \#20 Posted by: ryansinatra Posted at: 2019-04-05T03:12:28.057Z Reads: 36

```
I don't disagree at all. I'm just saying. Back when I didn't know anything about battery packs I did this all the time 😂
```

---

# Why can&rsquo;t I just use this as a switch?

### Replies: 13 Views: 577

## \#1 Posted by: Alex.Scheff Posted at: 2018-05-18T07:52:36.771Z Reads: 189

```
Hi I'm still searching for an switch option and I found [this](http://s.aliexpress.com/2qUzaUJb?).
It can handle enought Amps and Current and its also quite cheap.
Do you think I can use it?

Alex
```

---
## \#2 Posted by: Maxid Posted at: 2018-05-18T08:18:51.457Z Reads: 180

```
should work - only problem is that the spark due to inrush current will wear the contacts over time. After a couple hundred switches the relay might not work anymore.
```

---
## \#3 Posted by: SkaterBoy58 Posted at: 2018-05-18T08:23:04.757Z Reads: 172

```
its a solid state relay!
```

---
## \#4 Posted by: lrdesigns Posted at: 2018-05-18T08:29:27.979Z Reads: 163

```
Could work. Few downsides, you need a separate 4-32v supply to turn it on/off, where will you get that? Its a bit bulky. It may need a heat sink depending on how much amps your going to draw.
```

---
## \#5 Posted by: Maxid Posted at: 2018-05-18T08:32:16.479Z Reads: 157

```
sorry you are right - just read relay and was thinking of mechanical ones.
```

---
## \#6 Posted by: b264 Posted at: 2018-05-18T08:33:07.238Z Reads: 156

```
This might be a bipolar-based design which will burn off 3% of your power as heat.  That's a lot of cooling and wasted battery life.  And if it's FET-based then the inrush current will probably destroy it after a short number of cycles.
```

---
## \#7 Posted by: Alex.Scheff Posted at: 2018-05-18T09:37:22.006Z Reads: 136

```
Well I think I'll go with an mechanical switch instead, thanks to all :+1:
```

---
## \#8 Posted by: Quezacotl Posted at: 2018-05-18T10:18:00.507Z Reads: 129

```
Or you could go with a FET sparkswitch. Search the forum.
All mechanical switches wear out eventually. Not saying sparkswitch can't break, but it's better.
```

---
## \#9 Posted by: TehAtheist Posted at: 2018-05-18T11:46:18.170Z Reads: 119

```
You cannot use this switch. The purpose of a anti spark switch is not only to negate the spark, causing the contacts to wear. But also to prevent damaging you electronics. The capacitive load will draw a short but high amp current from the batteries, for a short time it'll appear as if your speed controller is a short circuit untill the capacitors are charged. This high current will (perhaps eventually) break your components. 

That's also why there is a resistor in the spark plugs, first the capacitors are charged through a resistor, lowering the current.
```

---
## \#10 Posted by: Maxid Posted at: 2018-05-18T14:53:36.589Z Reads: 88

```
@whitepony does not use an AS but connects his wires directly everytime. He did not report problems this way AFAIK. He had loop keys melt and AS fail though.
```

---
## \#11 Posted by: TehAtheist Posted at: 2018-05-18T14:59:49.822Z Reads: 83

```
How are his capacitors?
They aren't made for the big inrush of current I think.
```

---
## \#12 Posted by: Maxid Posted at: 2018-05-18T15:01:26.822Z Reads: 82

```
Well he is one of the most active riders on here who commutes to work every day. When he advocates not using AS keys but rather replacing bullet connectors from time to time( they degrade due to the spark) I take his word for it.

http://www.electric-skateboard.builders/t/re-building-loaded-vanguard-with-bamboo-fibreglass-carbon/10460/118?u=maxid
```

---
## \#13 Posted by: whitepony Posted at: 2018-05-18T18:40:27.111Z Reads: 63

```
hehe, Im still all sparks :smile: never had a vesc fail on me after the first day, had a few dead early birds, but mostly due to the foc bug back then i think
```

---

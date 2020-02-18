# Battery Wiring Question

### Replies: 13 Views: 683

## \#1 Posted by: butt_stallion Posted at: 2018-02-06T00:20:55.018Z Reads: 81

```
Can I just run one nickel strip from negative to postive cells, kind of like the bottom right cells in this picture?

![sketch-1517876316473|690x388](upload://cbCDTVJ4t3ttoEtinDRufRfDFED.jpg)
```

---
## \#2 Posted by: Genghis_Kuan Posted at: 2018-02-06T00:46:15.254Z Reads: 74

```
Short answer yes, just make sure you understand how much current that strip of nickel will be carrying and account for it
```

---
## \#3 Posted by: butt_stallion Posted at: 2018-02-06T00:53:28.920Z Reads: 71

```
So I might need to double it up is what you're saying?
```

---
## \#4 Posted by: b264 Posted at: 2018-02-06T00:54:35.265Z Reads: 75

```
To make it flexible it's better to not use nickel strips for that.  Use 10AWG stranded with silicone insulation.

You can if you know exactly what you're doing and it's a completely flex-free deck, like a carbon-fiber deck
```

---
## \#5 Posted by: b264 Posted at: 2018-02-06T00:55:52.371Z Reads: 77

```
Imagine picking up your board when it's all done and bashing it wheels-first into a concrete wall as hard as you can for 30 minutes.  Because that's exactly what happens when you ride it.  So the battery has to survive that without the nickel coming loose, which will cause a fire...
```

---
## \#6 Posted by: butt_stallion Posted at: 2018-02-06T01:09:53.916Z Reads: 71

```
Could 12AWG work? Because that's what I have on hand.  Also, are you saying to solder the copper wire directly to the battery?  I thought I wasnt supposed to do that
```

---
## \#7 Posted by: ShutterShock Posted at: 2018-02-06T01:31:06.884Z Reads: 61

```
12 AWG would probably work fine, 10 AWG just gives some extra current buffer.

And you are partially right, not a great idea to expose the batteries to an extreme amount of heat, but if you tin both sides beforehand and do it carefully, you can still get a good solder joint without applying a crazy amount of heat.  Most people do wires between cell groups on flexible decks.
```

---
## \#8 Posted by: butt_stallion Posted at: 2018-02-06T01:31:59.589Z Reads: 58

```
Okay, I will probably do that then.  It's not a super flexible deck but just to be safe.
```

---
## \#9 Posted by: ShutterShock Posted at: 2018-02-06T01:33:56.612Z Reads: 54

```
Yeah just be careful with the heat, I'd probably measure your voltage and resistance after each joint just to be sure nothing gets messed up. 

It is much easier to find an error when you measure periodically or after every cell, than finding out after the whole thing is put together that you have one bad cell
```

---
## \#10 Posted by: butt_stallion Posted at: 2018-02-06T01:35:01.207Z Reads: 53

```
I should probably invest in a cheap multi-meter then
```

---
## \#11 Posted by: ShutterShock Posted at: 2018-02-06T01:36:46.950Z Reads: 50

```
It's an essential tool in any build that involves electronics, IMO.  The one I have is great for the price, it's from Amazon: https://www.amazon.com/gp/product/B00KXX2OYY/ref=oh_aui_detailpage_o08_s00?ie=UTF8&psc=1
```

---
## \#12 Posted by: butt_stallion Posted at: 2018-02-06T01:37:32.294Z Reads: 46

```
I know it is.  Usually I have access to one.  But now that I'm off at college I don't have access to it anymore
```

---
## \#13 Posted by: b264 Posted at: 2018-02-06T01:42:18.641Z Reads: 49

```
[quote="butt_stallion, post:6, topic:45686"]
Could 12AWG work? Because that’s what I have on hand.  Also, are you saying to solder the copper wire directly to the battery?
[/quote]

Yes 12AWG will work if it's high-strand-count with silicone insulation; No, I meant solder to the nickel.  So the P-packs are welded together but the series packs are wired together for flexibility.  And don't heat it hotter or for longer than you need to to make a good connection.  Keep the cells as cool as you can.
```

---

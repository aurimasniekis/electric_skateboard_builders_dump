# Do I need any complicated electronic stuff?

### Replies: 12 Views: 1026

## \#1 Posted by: jbalint1122 Posted at: 2017-03-20T11:14:57.901Z Reads: 134

```
So I am building my first board, (penny style, sk3 6374 190kv, FVT 120A, 8S)

I often see these "Anti spark switches", and stuff here on several builds. Are these needed? Would I have any problem if I went without them?
Sorry if this is a frequently asked question. You can link some threads if thats good.
Thanks.
```

---
## \#2 Posted by: JLabs Posted at: 2017-03-20T11:19:50.260Z Reads: 132

```
An anti spark switch is required for the build or you could fry your electronics. You go with a conventional style switch from DIY (I think @barajabali has a few left over) or use an XT90S loop key. The loop key is the cheapest but not as pretty. Either will do the job perfectly.
```

---
## \#3 Posted by: jbalint1122 Posted at: 2017-03-20T14:01:53.084Z Reads: 109

```
Thanks! You just saved me. 
I think I will go with the loop thing.
Is there any additional stuff I possibly looked over?
```

---
## \#4 Posted by: Hummie Posted at: 2017-03-20T14:18:48.315Z Reads: 105

```
or just use the xt90s as it's usual used as a plug.  even simpler.  You can get away with just using a regular non-anti-spark plug too but it will make a big spark and snap and carbonize your connector each time adding resistance.  doable though and I'm pretty sure your electronics should be fine.   the anti spark is just to slow down the huge inrush of electricity that the capacitors on the esc ask for as soon as they're connected to the battery.  they get filled quickly
```

---
## \#5 Posted by: PXSS Posted at: 2017-03-20T14:24:12.312Z Reads: 98

```
What I've done is used an XT90S with a fuse strip on it. This way, I have an anti spark switch and a fuse in a small, cheap, replaceable and easy to access package
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-03-20T14:25:27.523Z Reads: 94

```
We're doing exactly that on one of our personal boards to see how long it will last before becoming useless. We made a cheap little one out of an XT60 actually. So far no effect on the electronics.
```

---
## \#7 Posted by: JLabs Posted at: 2017-03-20T14:30:59.203Z Reads: 87

```
It was about 3 months until I blew something with out an antispark. I think it's inevitable with sensitive electronics.
```

---
## \#8 Posted by: jbalint1122 Posted at: 2017-03-20T16:34:11.013Z Reads: 79

```
Thanks for the replies guys! This is getting more complicated than I thought it would...
I think I will have to do a bit of research to find out more.
If you could link some nice threads, that would be awesome.:slight_smile:
Thanks!
```

---
## \#9 Posted by: e-Octo Posted at: 2017-03-20T16:41:37.738Z Reads: 75

```
Definitely don't "need" complicated electronics.  Motor - ESC - Battery and Tx/Rx...  but some are nice to have.

Especially with 8s - you will get some spark and wear - but the FVT may have inrush proteciton already built into it's little on/off power switch.

I too am a fan of a simple loop key anti-spark, here's a good how-to:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

A lot to learn - good luck!
```

---
## \#10 Posted by: Hummie Posted at: 2017-03-20T19:00:08.722Z Reads: 60

```
I can't find info confirming but as I understand it the battery wires create inductance, storing energy in a magnetic field,  and the big caps where the wires first connect to the esc are there to smooth the current coming in and out of the battery. ( or
Maybe just there to deal with the voltage spike as the magnetic field colapses when current is turned off, and just an issue going one way...or maybe both ways and a high voltage spike is bad for th batteries too ) If the caps weren't there u will destroy the esc especially with long battery wires. The spark is a good thing in a way as it shows u the important caps are doing their job. With the caps doing there job the esc should be protected.  The spark, or not having a spark, is solely a possible connector deterioration issue.  The spark and the inrush of current it is showing is kept in check by the caps.  So chose your poison do u want the convenience of not having to replace connectors that get chard or know when ur caps have died.  The caps can also be losing their capacitance, decreasing with heat and use and as the electrolyte inside evaporates.  So u still could have a spark at connection and assume the caps are good but really they've deteriorated as don't have enough capacitance to deal with the inductance of the battery wires.
```

---
## \#11 Posted by: jbalint1122 Posted at: 2017-03-20T19:12:33.964Z Reads: 59

```
Thanks guys!
So much more to learn :grinning:
```

---
## \#12 Posted by: Hummie Posted at: 2017-03-20T19:22:14.641Z Reads: 52

```
What are the circuitry bits?  Inductors, capacitors, diodes, resistors, ...transistors.  I think those are all the circuitry bits in the world and are how elec is controlled.  Just knowing how those very generally work is a great foundation to making a board. The science of electricity is awesome..until they start getting into math equations and then it's awesomely complicated

someone here said they were using dielectric grease on their connections without an antispark and it worked well.  Maybe just have a dab at the end of your bullet plug and connect there first.
```

---

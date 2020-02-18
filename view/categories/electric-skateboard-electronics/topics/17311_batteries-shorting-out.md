# Batteries shorting out

### Replies: 6 Views: 604

## \#1 Posted by: brandon Posted at: 2017-02-06T22:11:29.852Z Reads: 79

```
So I'm running two 3s lipos in series. I charged both of them a few times individually, then I bought a 3s to 6s connector so I could charge them as a 6s battery. I charged them this way several times with no issue. The other day I plugged in the power leads to my charger, then while plugging the second balance connector into the 6s adapter, I got sparks and melted the shit out of the connector. Without any doubt I plugged it in the correct direction, and even backwards I don't think the key allows any contact between wires. I couldn't salvage the connector, so I cut the wires and soldered the 6s connector directly to the two batteries, charged no problem. When they were full I put them back on my board, plugged the power wires into my series adapter, more sparks and fire, also plugged in the correct direction. I cut the balance connector off, and now my board is running like its supposed to.

No idea wtf is going on. Internal short in one of the batteries maybe? I can't find anything wrong with my adapters, and they worked like they were supposed to for several months.
```

---
## \#2 Posted by: Hummie Posted at: 2017-02-06T22:18:54.998Z Reads: 75

```
maybe you put the two 3s packs on the charger in a different order than the main leads.  I've done that and melted the balance plug.
```

---
## \#3 Posted by: brandon Posted at: 2017-02-06T22:29:04.649Z Reads: 70

```
So I need to make sure the order of the balance series adapter and the main power series adapter match? I guess I could have gotten them reverse both on the charger and the board
```

---
## \#4 Posted by: Namasaki Posted at: 2017-02-06T23:42:59.573Z Reads: 59

```
You might already be aware of this but I'll mention it anyway. 
On each battery pack the black balance wire is connected directly to the black power wire and the red balance wire is connected directly to the red power wire.
```

---
## \#5 Posted by: jmasta Posted at: 2017-02-07T00:09:40.903Z Reads: 50

```
If you are connecting your main power leads in series, you should clip one of the wires on your 3S -> 6S balance lead adapter. Currently the positive wire from battery A is connected to the ground wire from B, which is the middle pin of the 6S balance port.  If you hookup the main leads in a different order than their adapter, it will short your battery

To prevent this, I recommend modifying the adapter by cutting the ground balance wire from the second battery (B0). Use a multimeter to confirm before cutting

**INPUT**
[ A0 | A1 | A2 | A3 ] +  [ B0 | B1 | B2 | B3 ] 

**OUTPUT  (Currently)**
[ A0 | A1 | A2 | A3=B0 | B1 | B2 | B3 ]

_Change to_
[ A0 | A1 | A2 | A3 | B1 | B2 | B3 ]  

_or_

[ A0 | A1 | A2 | B0 | B1 | B2 | B3 ]
```

---
## \#6 Posted by: PXSS Posted at: 2017-02-07T00:11:37.487Z Reads: 39

```
I feel like this is really one of those you just have to investigate with a multimeter to figure out where the short is.
```

---

# Snipping focbox white plugs

### Replies: 20 Views: 632

## \#1 Posted by: Hummie Posted at: 2018-02-04T20:14:19.491Z Reads: 142

```
If I were as steady as a surgeon and ground down the white pug beside the motor wires, I think it's for the sensor, and made sure to not get all the way down to the board or solder around it or let any of the pins mesh would that be doable?  I know it sounds ridiculous but trust me the way it is now, just sqeezing in 12s5p the plug will get blown off from the first ground hit.  even if I cut it down 3/4 would be solved.
```

---
## \#2 Posted by: Blasto Posted at: 2018-02-04T20:20:27.288Z Reads: 135

```
Sounds more like a butcher than a surgeon
```

---
## \#3 Posted by: Hummie Posted at: 2018-02-04T20:21:02.741Z Reads: 134

```
haha.  but tell me what you think.  if you had to remove a limb would it kill the animal.  or I could solder it off? @Blasto I think you know about these things
```

---
## \#4 Posted by: Blasto Posted at: 2018-02-04T20:22:58.412Z Reads: 129

```
Lol, solder it off. Those connectors are not easy to remove without having a proper technique

Ex 1: heat plastic shroud with a hair dryer until soft and remove. Then remove pin per pin with an iron.

Ex 2: remove with a shovel type iron or multiple iron’s
```

---
## \#5 Posted by: Hummie Posted at: 2018-02-04T20:24:48.699Z Reads: 113

```
great to hear.  any advice is hugely appreciated @Blasto or anyone else who knows the details on doing this.  Or maybe its obvious and I heat it then pull and make sure whats left isn't bridging?
```

---
## \#6 Posted by: Sebike Posted at: 2018-02-04T20:26:14.762Z Reads: 114

```
https://www.highlandwoodworking.com/ProductImages/handsaws/459001.jpg
```

---
## \#7 Posted by: ShutterShock Posted at: 2018-02-05T03:36:10.877Z Reads: 97

```
Basically @Blasto has the two main ways

1) use a dremel and literally just cut through it (with absolutely no power connected of course) and be sure the pins aren't touching after you're done.

2) Use a super wide iron and melt a bunch of extra solder onto the back of the trace and drop out the connector, then use a soldering pump or bulb and get rid of all the solder, leaving an empty socket for the plug.  This is a delicate process and you have to get it off quickly otherwise risk melting through a ground layer or something

3) Melt off the connector like blasto said and de-solder each pin of it (may be pretty hard)

Either way you are destroying the plug, so I am assuming you don't need to use it.
```

---
## \#8 Posted by: scepterr Posted at: 2018-02-05T03:50:17.346Z Reads: 84

```
I'm confused how it's in the way...
@Hummie can you take a pic?
```

---
## \#9 Posted by: ShutterShock Posted at: 2018-02-05T04:31:13.541Z Reads: 73

```
I think it is in his other post about the fets overheating?  It looks like it might collide with an enclosure but tbh I'm not sure either
```

---
## \#10 Posted by: Hummie Posted at: 2018-02-05T05:04:29.653Z Reads: 69

```
![image|375x500](upload://rPBULJP3Y3jUTPvXmREzPH2P6vh.jpeg)![image|666x500](upload://smTPFXmf9cY78Hs4tUpn5jXBXBf.jpeg)![image|375x500](upload://eTQeFrAY4HBwyYNwj0GGD5EXdOD.jpeg)![image|374x500](upload://yFgDxmRJ4T39taERxBjBPT4wHKc.jpeg)![image|374x500](upload://4SYlgMx1eWBYvTZG0XXm1BIWiWO.jpeg)

I’ve counted to 3 and made my up my mind.  Definitely will be making a strong cover for the gets n will add the little copper stick on heat sinks.
```

---
## \#11 Posted by: Blasto Posted at: 2018-02-05T05:39:34.299Z Reads: 52

```
Your cutout is clearly not intended for 60 cells... why dont you drop your cell count to 48 or 50 (dont know what is your config) You wont be wasting to much real estate and you’ll have space for your focbox’s (with heatsink)

Adding a copper heatsink to the focbox is not that easy, the fets need to be electrically isolated, so they must not have a direct contact with whatever heatsink you plan to use.
```

---
## \#12 Posted by: Hummie Posted at: 2018-02-05T05:51:55.280Z Reads: 48

```
i have lots of little copper heatsinks that stick on and isolated.  

true it doesn't look like it fits and it seems not ideal in a large way but with the white plugs out of the way and also taking the 3 pins out for the canbus and soldering wires there, then the boards are low and the caps will be as flush as the cells and I'm going to make a fiberglass cover that I can make much more robust at this end.   I can still get to the miniusb and that's all i use.
```

---
## \#13 Posted by: jrpwit Posted at: 2018-02-05T05:55:28.480Z Reads: 47

```
Why not keep the stock heatsinks on?

![0204182219|690x388](upload://n9pEPV645mCMs1h35JRRkdJ0JLI.jpg)

Practically the same height as an 18650
```

---
## \#14 Posted by: Blasto Posted at: 2018-02-05T05:55:31.660Z Reads: 45

```
[quote="Hummie, post:12, topic:45555"]
canbus and soldering wires there
[/quote]

Another friendly piece of advise, if the can bus is connected, always power on and off both modules together. 

If only one is powered then you plug the other, you will blow both CAN transceivers. 

Just something to keep in mind
```

---
## \#15 Posted by: Hummie Posted at: 2018-02-05T05:58:33.344Z Reads: 43

```
good to know blasto! jesus.  I wasn't setting it up that way but didn't know. so many ways to blow up
@jrpwit ...youre right maybe it can fit now it's upside down.  but it sticks out too much.

  but it's probably overkill for me and I have those cool looking stick on copper ones.  something will happen
```

---
## \#16 Posted by: jrpwit Posted at: 2018-02-05T05:59:05.882Z Reads: 44

```
I don't have much of a problem with hight in my build. Just add another few plys to get the height up.

I don't have much of a problem getting them in my build. The holes are a few mms taller than an 18650.

![0204182249a|690x388](upload://yeLA3dR907UKmCyg6kAXAYtND1y.jpg)
![0204182252a|690x388](upload://2Cg7sulPtpnRYr74jfUI7DC8qwC.jpg)
```

---
## \#17 Posted by: Hummie Posted at: 2018-02-05T06:00:15.965Z Reads: 43

```
wow cool deck, kinda what I'm doing but with way more cells at 60.  actually not that many more...that's a huge deck.  That looks like a surfboard for land
```

---
## \#18 Posted by: jrpwit Posted at: 2018-02-05T06:03:34.311Z Reads: 45

```
38 inches? Not that long imo. It was originally one of these.

https://www.muirskate.com/longboard/completes/38911/five-mile-war-horse-longboard-skateboard-custom-complete
```

---
## \#19 Posted by: Hummie Posted at: 2018-02-05T06:04:38.214Z Reads: 44

```
weird it just looks like you have so much more room for cells
```

---
## \#20 Posted by: jrpwit Posted at: 2018-02-05T06:13:55.694Z Reads: 40

```
Probably could go 12s4p but for strength I'm sticking with 3p. I am trying to make it pretty thin. The lid will probably be fiber glass.

12s5p would be crazy though. Best of luck trying to cram those focboxes in.
```

---

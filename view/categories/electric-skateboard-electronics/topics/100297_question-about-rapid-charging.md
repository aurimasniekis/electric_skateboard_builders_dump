# Question about rapid charging

### Replies: 26 Views: 423

## \#1 Posted by: Randy_bobandy Posted at: 2019-08-14T22:46:28.123Z Reads: 126

```
I wanted to get some input on charging speed for my battery.  I'm somewhat new to this stuff and want a second opinion.  I built a 12s5p battery and have a bestech bms with a max charge rate of 20amps. I want to get a second high speed charger for days I want to ride alot and long trips and such. I was on aliexpress and saw a yzpower charger for $93 and I have read that some people here ha ve had a good experience with that brand. Problem  is the only option for that charger are 12a,13a,14a,15a. I want a 10amp charger but I don't knkw about the other brands. I know the 30q cell is rated at 1c so a 5p pack should be able to charge at 15a. I would be using this charge rarely and I would use my 3a charger if I don't plan to ride anytime soon after the battery dies. What are your options on a 12a charger? Is that to many amps? How bad will it reduce my capacity charging at that current(not using it very often). If anyone knows of a better charger I would love some suggestions thanks!
```

---
## \#2 Posted by: wwohl602 Posted at: 2019-08-14T22:59:00.345Z Reads: 121

```
Interested to hear the results. What BMS are you running?
```

---
## \#3 Posted by: Randy_bobandy Posted at: 2019-08-14T23:04:12.741Z Reads: 121

```
![20190814_160333|653x500](upload://ltZWGbeQLdchrqoNL2LZIycBuZZ.jpeg)
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-08-14T23:36:40.440Z Reads: 111

```
The BMS can withstand that, but can the thin balance wires take 12/15/20a? 

Make sure to fuse your ports if you're going that high... I'm getting a 12s7p 30q soon and I'm staying below 8a charging because I'm terrified of hurting something

Then again I'm a wuss, so... 😂

E: I realize this isn't how it works.
```

---
## \#5 Posted by: Randy_bobandy Posted at: 2019-08-15T00:35:03.909Z Reads: 107

```
Well apparently they can. I dont know why they would rate the bms is the balance wires couldnt handle it. I don't know for sure but the balance wires don't take the full amperage and just a few milliamps(says 168mA). Then again I hope someone who knows more then me to tell me if it's ok
```

---
## \#6 Posted by: linsus Posted at: 2019-08-15T08:08:24.834Z Reads: 95

```
Balance wires has nothing to do with the max amp om the charger. The balance current is set by the BMS.
Read the datasheet for your battery cells to deterimine max charge amp. i.e if its 30Q cells the rated charge is around 4A max per cell.

That beeing said. The last 30-40% of the battery charge wont get that much faster. Thats the portion where the cells reach higher IR and current over the cells fall, also called the CV mode. At the end of this part the balancing occurs as well. Atleast for the cheaper china BMS's that does not use active balancing.
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-08-15T08:22:57.636Z Reads: 94

```
Most chargers in aluminum cases (likely including the YZPower one) have potentiometers on the board inside that can be adjusted to change the voltage and current limits of the charger - it should be totally possible to buy that 12A one and turn it down to 10. In fact, the ones that are available in multiple current options (4, 6, 8, etc) are usually all the same identical board inside, just set differently and sold for a different price.
```

---
## \#8 Posted by: UKRider Posted at: 2019-08-15T13:14:59.552Z Reads: 85

```
The 30Q can be charged at 4 amps max, as you have 5p that means the max you could charge the pack is at 20amps. The BMS can handle that as you have stated it's 20amps. I would be concerned about your actual charge port, can that handle that many amps? Some of the basic DC 2.5 mm jack's get very hot and can't handle much amps. I'm not sure how much they can handle but I have read somewhere that 8amps is max. Maybe somebody else can shed some light on this?

Also need to check the awg of the wires in the charge port.
```

---
## \#9 Posted by: ShutterShock Posted at: 2019-08-15T15:35:22.401Z Reads: 73

```
yeah some of the jacks only do 4A lol I wouldn't push them too hard.  I usually use xt-60 as my charge port
```

---
## \#10 Posted by: Randy_bobandy Posted at: 2019-08-15T16:13:58.187Z Reads: 69

```
I would be adding a different charge port for the fast charger. I think I was going to use a gx16 plug since that's one of the pre configured options on the charges. I would also be using thicker wire for the charging plug too.
```

---
## \#11 Posted by: Randy_bobandy Posted at: 2019-08-15T16:17:25.771Z Reads: 68

```
Thats good to know. Ill grab the 12amp one and open it up and drop the current. Thanks for.the info!
```

---
## \#12 Posted by: Randy_bobandy Posted at: 2019-08-15T16:21:06.525Z Reads: 65

```
Ya I didn't think the balancing wires mattered with charge current. I didn't realize the 30q did 4amps max I thought I read somewhere it was 3amps but if thats the case 12amps shouldn't be a problem with a 5p configuration.
```

---
## \#13 Posted by: linsus Posted at: 2019-08-15T16:22:32.586Z Reads: 62

```
General rule is to stay away from max ratings in electronics tho. If max is 4 then do 3. Lower current will prolong the life of your pack as well.
```

---
## \#14 Posted by: thisguyhere Posted at: 2019-08-15T18:20:23.744Z Reads: 62

```
[quote="Sn4pz, post:4, topic:100297"]
can the thin balance wires take 12/15/20a
[/quote]

balancing current is negligible:

![image|690x49](upload://sez2tmuM7baZxnW4rmCyPEetrUi.png) 

[quote="Randy_bobandy, post:1, topic:100297"]
the 30q cell is rated at 1c so a 5p pack should be able to charge at 15a
[/quote]

not 1c, but 4amp, so 5p you can max 20amp, but i wouldn't:

![image|619x500](upload://soVJeiahjcXe7cAR0naI7DerANg.png) 

if you use a higher amperage charger, just make sure to use lower gauge charge wires.  also, the common 2.1/5mm barrel plug is not suitable for anything more than 5A.
```

---
## \#15 Posted by: Sn4pz Posted at: 2019-08-15T18:47:48.425Z Reads: 60

```
[quote="thisguyhere, post:14, topic:100297"]
> can the thin balance wires take 12/15/20a

balancing current is negligible:

![image.png](https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/5/c5e25ca80d87e2efe89d66f43b4109b8fe0056c6.png)
[/quote]

Read my edit xP 

I edited it shortly after commenting... Wasn't thinking about it right
```

---
## \#16 Posted by: Randy_bobandy Posted at: 2019-08-16T00:20:02.503Z Reads: 52

```
What would be the highest you would go? I dont plan on charging it at this speed very often, only times I want to ride all day.
```

---
## \#17 Posted by: thisguyhere Posted at: 2019-08-16T03:59:45.998Z Reads: 48

```
Depends on the connectors you're using. 

Like i said before, if youre using barrel plugs, no more than 5A.
```

---
## \#18 Posted by: Randy_bobandy Posted at: 2019-08-16T06:25:37.994Z Reads: 44

```
I was planning on using a gx16 connector since thats one of the options with the charger.

Edit: I take that back that only does 5 amps as well. It looked to be a more capable port but I guess not.
```

---
## \#19 Posted by: MysticalDork Posted at: 2019-08-16T06:59:04.227Z Reads: 42

```
It's 5 amps **per pin**. If you use a connector with more pins, then you can gang them together to get more current handling.
```

---
## \#20 Posted by: thisguyhere Posted at: 2019-08-16T15:48:50.283Z Reads: 40

```
just make sure to use wire less than 20awg and you should be fine.

seems you should be able to push up to 10A through that connector, right?  not sure, haven't used one before.
```

---
## \#21 Posted by: Randy_bobandy Posted at: 2019-08-16T19:02:49.929Z Reads: 34

```
Ok cool so if I get a 4 pin I could do 10amps?
```

---
## \#22 Posted by: MysticalDork Posted at: 2019-08-17T05:05:03.145Z Reads: 33

```
Probably. If you need waterproof, there are also plastic connectors of similar type to the GX16 with o-rings and seals, I'm using those for my ebike project.
```

---
## \#23 Posted by: ThomasL Posted at: 2019-08-17T18:21:05.166Z Reads: 32

```
Actually I tried 5a charging on a 12s5p, the plastic started to melt inside the charging port.
I changed both battery and charger port to xt60, no issue anymore.
```

---
## \#24 Posted by: Sn4pz Posted at: 2019-08-18T14:53:32.030Z Reads: 27

```
Do you have any extra to sell, or a link for them? I can search for a bunch but I would like to make sure I get a good one. It's for a 10s3p battery, if that will matter 🤷
```

---
## \#25 Posted by: MysticalDork Posted at: 2019-08-18T19:52:41.948Z Reads: 24

```
I'd say use these: https://www.amazon.com/Waterproof-Connector-Socket-Electrical-Socket/dp/B07BDDLX7V/ There are a lot of different variations - panel mount, cable-end, male, female, different sizes (those are 13mm, but I've also seen 16, 20, and 29mm as well with up to 24 pins) and etc. Just search "IP68 connector" and you'll find dozens.

According to their rating system, the 2-pin version will handle 10A on its own (the low pin-count connectors have fatter pins.) 

Make sure to measure your charger's cable diameter and check that it will fit in the cable-grip on the connector - the 13mm ones might be a tight squeeze depending on how fat the cable is. If the 13mm size doesn't fit, then this one should: https://www.amazon.com/HangTon-Connector-Waterproof-Circular-Multipole/dp/B07DJ9BW9W/
```

---
## \#26 Posted by: Sn4pz Posted at: 2019-08-18T19:59:22.922Z Reads: 20

```
Thank you very much 👏
```

---

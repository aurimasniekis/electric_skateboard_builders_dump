# Rewiring space cell to fit inside the SPACE CELL PRO Enclosure

### Replies: 27 Views: 2548

## \#1 Posted by: michaelcpg Posted at: 2016-07-02T11:58:41.956Z Reads: 211

```
Hey guys,
Enertion's space cell enclosure arrived a few days ago and I'm about to start installing my space cell in it. I'm looking to pull the space cell apart, removing the plastic cell holders and nickel strips and then resolder the cells together with copper wire that I bought today but just wanted to see if you guys think this stuff should be thick enough?

<img src="/uploads/db1493/original/2X/2/2af606e719f116598a374fc6e73c23e87774de53.jpg" width="281" height="500">

It doesn't have a guage measurement on it but says it's rated for 25A so I was planning to solder two bits of wire between each cell to be safe/add strength to the connections.
Are there any issues I could have with the battery if I were to solder it together this way?

Cheers
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-02T12:13:44.386Z Reads: 199

```
Why do you want to take it apart? You will need at least a 100w soldering station/iron as well.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-07-02T12:19:05.924Z Reads: 196

```
Doesn't fit in the enclosure otherwise due to the fact that the plastic cell holders stop the cells from being able to sit between the ribs of the enclosure, connecting the batteries via wires rather than nickel strips should also make the battery more forgiving when it comes to small amounts of board flex
```

---
## \#4 Posted by: lox897 Posted at: 2016-07-02T12:22:14.095Z Reads: 191

```
Well it should work. Just make sure you use a decent iron otherwise you will heat up the cells too much.
```

---
## \#5 Posted by: mattdig Posted at: 2016-07-02T13:40:50.840Z Reads: 184

```
I'm a bit confused. Are you saying that the Enertion SPACE cell doesn't fit in their own enclosure? That doesn't sound right.
```

---
## \#6 Posted by: whitepony Posted at: 2016-07-02T15:19:02.475Z Reads: 176

```
I would use thicker wires - why waste energy on heating up small battery wires if you could use that energy for higher topspeed or longer range. everything depends on the length of the cable of course ... play around with DC voltage drop calculators! 
the total length of wire in a fully assembled battery is quite significant. in most 18650 setups you can roughly say, its about 4x the battery length (flat layouts used in most boards and used by the space cell). in my case probably around 2m including the cable ends and everything until the vesc is connected.

2m 10AWG cable: 1.8% loss -> http://www.calculator.net/voltage-drop-calculator.html?material=copper&wiresize=3.277&voltage=36&phase=dc&noofconductor=1&distance=2&distanceunit=meters&amperes=50&x=42&y=13

2m 16AWG cable (looks a bit like yours): 7.3% loss -> http://www.calculator.net/voltage-drop-calculator.html?material=copper&wiresize=13.17&voltage=36&phase=dc&noofconductor=1&distance=2&distanceunit=meters&amperes=50&x=60&y=15

thats the reason why I reinforce my batteries with copper wires ontop of the nickel strips. you have quite significant losses within your system BEFORE it actually enters the esc & motors!
```

---
## \#7 Posted by: michaelcpg Posted at: 2016-07-02T23:13:49.580Z Reads: 152

```
That seems to be the case, at least not without really squeezing it between the enclosure and the deck which I'm not comfortable with due the fact that it'll stress the battery with any amount of board flex. To some extent it makes sense though as the original space cell was designed to fit in the raptor where as the new space cells usually come preinstalled in the enclosures.
```

---
## \#8 Posted by: michaelcpg Posted at: 2016-07-02T23:17:35.161Z Reads: 151

```
I measured the diameter of the cable I bought and it's somewhere between 2 - 2.5mm which looks to put it somewhere between 12 and 10AWG so the voltage drop doesn't look too bad? Considering that I'm looking at soldering two wires between each cell as well, shouldn't the wire I have be thick enough?
```

---
## \#9 Posted by: mattdig Posted at: 2016-07-03T04:01:29.159Z Reads: 142

```
Before you go taking the battery apart I'd contact Enertion for some support. This seems like a lot of unnecessary work that might ruin an expensive battery.
```

---
## \#10 Posted by: onloop Posted at: 2016-07-03T04:14:01.617Z Reads: 146

```
[quote="mattdig, post:5, topic:5464"]
the Enertion SPACE cell doesn't fit in their own enclosure?
[/quote]

This was never my intention.... 

The SPACE Cell Pro is a new battery design all together. So the Case is not meant to be a case for the old version. I just offer it separately to anyone who needs a nice case....

However, someone did confirm via email that the Old SPACE Cell actually fit inside....
```

---
## \#11 Posted by: Karmannghiagirl Posted at: 2016-07-03T04:17:39.067Z Reads: 135

```
why not make it backwards compatible? or at least make it super obvious that it does not work with the older space cell batteries?
```

---
## \#12 Posted by: onloop Posted at: 2016-07-03T04:20:12.093Z Reads: 132

```
[quote="Karmannghiagirl, post:11, topic:5464"]
why not make it backwards compatible?
[/quote]

maybe i was thinking forward to much..... sometimes making everything backwards compatible makes innovation harder.

but like i said, someone has confirmed the old space cell fitted....
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-07-03T04:23:59.969Z Reads: 126

```
A warning about compatibility issues on your website's page for the separate enclosure may be a good idea.

Although it may just fit, I don't think I'd personally feel comfortable using the battery in the enclosure in this way due to there being essentially no excess room at all to allow for minor flexing of the board during riding without putting pressure on the battery. Just something to keep in mind.
```

---
## \#14 Posted by: mattdig Posted at: 2016-07-03T13:33:24.803Z Reads: 118

```
In which dimension is the case too small?
```

---
## \#15 Posted by: michaelcpg Posted at: 2016-07-03T21:16:18.498Z Reads: 113

```
Height. The plastic spacers on the cells mean that the cells can't fit into the ribs of the enclosure which means that the battery sits higher than it otherwise would
```

---
## \#16 Posted by: mattdig Posted at: 2016-07-04T03:09:07.817Z Reads: 109

```
In that case you might want to try removing material from the enclosure, or the deck, or add a spacer around the outside of the case to fill the gap to the deck. Im not using a space cell, but in order to get my battery to fit the case I bought, I had to carve about 3mm out of the deck, and I added a 3mm rubber spacer.
```

---
## \#17 Posted by: michaelcpg Posted at: 2016-07-04T03:27:01.205Z Reads: 108

```
Although it's a longer process, pulling my battery apart and rewiring it is really my only option because I also want to upgrade it to a 10S4P pack in the near future and the only way I can fit that many cells in the enclosure is removing the cells from the plastic spacers as the battery pack will be too long for the enclosure otherwise.
```

---
## \#18 Posted by: Luke Posted at: 2016-07-04T03:28:57.092Z Reads: 108

```
If you need a  router to make your deck a little bit thinner in the area where the battery sits, i can help :)
```

---
## \#19 Posted by: Blasto Posted at: 2016-07-04T04:16:05.710Z Reads: 112

```
So you will dismantle the space cell just to rebuild it while soldering the cells and hopefully nothing will go wrong?

Dude this sounds like a bad idea, mind as well buy some single cells and go from there. Use your space cell for another build or sell it.

Mind you another option would be to break off all the plastic holders and "fold" the nickel strip so the cells are closer together... Again this doesn't sound like an elegant solution neither
```

---
## \#20 Posted by: michaelcpg Posted at: 2016-07-04T04:35:40.286Z Reads: 112

```
It's definitely not the ideal solution but I had to basically build the space cell from scratch in the first place because that was the only way Jason could get it into the country (NZ). 

Selling it and buying new cells isn't really an ideal solution either as it'd likely mean I'd end up losing money overall and I'd probably have trouble finding a buyer anyway due to the e-board market in NZ being pretty small and shipping overseas would just be a hassle. Buying 18650's locally is also way too expensive and importing from most overseas sellers looks to take weeks or even a month for shipping which I'd rather not spend that long without a board as it's my primary way of commuting to work.

I was actually considering just breaking off the plastic spacers but that would likely end up being an even worse idea due to the fact that it'd probably actually be quite difficult to break them all off without damaging the cells due to how tightly they hold the cells and using pliers or a knife so close to the cells just seems like it probably wouldn't end well...

Ah the joys of being so secluded from the rest of the world....
```

---
## \#21 Posted by: Luke Posted at: 2016-07-04T04:42:29.088Z Reads: 99

```
[quote="mattdig, post:16, topic:5464"]
that case you might want to try removing material from the enclosure, or the deck,
[/quote]

Can someone comment on the viability of routing out 2 ply for Michael's board to fit everything better? I see it as the least destructive solution
```

---
## \#22 Posted by: michaelcpg Posted at: 2016-07-04T04:48:20.757Z Reads: 100

```
Unfortunately it's still not an ideal solution in this case because it'd mean I won't have enough room for an extra 10 cells to upgrade to a 10S4P pack at a later stage because of the fact that the gaps between the cells produced by the plastic spacers would add too much length to the battery.
```

---
## \#23 Posted by: Luke Posted at: 2016-07-04T04:51:22.407Z Reads: 102

```
So the issue is height at the moment and length and height if you want to upgrade to 4p eventually?
```

---
## \#24 Posted by: whitepony Posted at: 2016-07-04T04:52:58.896Z Reads: 103

```
I removed up to 5mm off my tesseract with a handheld router to sink in the battery a little - it worked out well, but added noticeable flex, so I covered it with a layer of carbon:

http://www.alternative-4.com/DIY/tesseract_rework_oncemore%20-%2016.jpg

in retrospect, Im not sure why I tried to route away the strong rocker of the board and making it completely flat instead of embracing the rocker. with foam and vacuum bagging, you can make bend enclosures easily. next time maybe ... :slight_smile:
```

---
## \#25 Posted by: michaelcpg Posted at: 2016-07-04T04:54:29.518Z Reads: 103

```
Essentially yea
```

---
## \#26 Posted by: Luke Posted at: 2016-07-04T05:02:54.553Z Reads: 101

```
Yeah its slightly noticeable, but that board is beautiful :cry:
```

---
## \#27 Posted by: onloop Posted at: 2016-07-04T05:29:11.134Z Reads: 101

```

I have done some measurments, the old space cell should fit inside. You will have approx 9mm of play, so be sure not to tighten the enclosure fully against the deck.

<img src="/uploads/db1493/original/2X/1/1e42fa0dfb8d33be2c0bb1247bb7bdef4081947b.png" width="690" height="225">
```

---

# Identifying that BAD 18650!

### Replies: 31 Views: 1042

## \#1 Posted by: Savace Posted at: 2018-10-02T22:27:16.825Z Reads: 207

```
Ill try to explain it briefly, basically i have a 12s10p 18650 set up, board keeps cutting at 44volts (should be 50V full charged and can hit around 38V before needing recharge), this is a self build, there are  **4**  of the packs (pictured below ) in the board, each with  **3**  rows of  **10**  batteries ( 4 x 3 = 12s / 10 = series)

when taking the voltage across all the packs this is what it looks like

1st pack | | | X 3.53 3.28 3.53 10.4
2nd pack | | X | 3.8 3.8 3.8 11.68
3rd pack | X | | 3.8 3.8 3.8 11.67
4th pack X | | | 3.8 3.8 3.8 11.67

clearly the 1st pack is the problem which is what is in the pic - the middle row has the lowest voltage across it at 3.28. I have guessed two of the cells and cut them out the series and tested them and they both show 3.28.
so my question is - how can identify the bad cell - do i need to cut them all out and test - i have a feeling they have balance charged since the board cut out so none will be “dead”

![IMG_2510|666x500](upload://pMsYQt2BBgedZTK0kNY7VCUgDRh.jpeg) 
![BatterySkateboard|251x500](upload://8O1CFPPWQHwSj1WomwGpHzwZMZy.png) 

 currently i think they are all now sitting at 3.29v individually in that "bank", guess i need to solder them back into the series and run the board dead again , then cut them out quickly before other good ones surrounding it in that bank it balance charge it and revive the bad cell /cells and see if i can see what one/s are dead unless anyone else knows a way to test them?
```

---
## \#2 Posted by: Newby Posted at: 2018-10-02T22:31:43.902Z Reads: 190

```
Are you using a bms?
```

---
## \#3 Posted by: strattos Posted at: 2018-10-02T22:33:38.944Z Reads: 191

```
Easiest way to test for a bad cell is internal resistance. There's plenty of chargers out there that do a quick easy test. Or you could fairly simply design your own.

Or you could attach a load thermal camera it and bad cells should be hotter.

Could also be an issue of pack design but I don't know what kind of currents your pushing nor what your connecting wire is made from. But that kind of design is asking for uneven current draw Imo.
```

---
## \#4 Posted by: Savace Posted at: 2018-10-02T22:33:53.504Z Reads: 186

```
Yes it has a BMS ![IMG_2512|666x500](upload://n7srWXG7PG3TWxsfPH9tNOnuo24.jpeg)
```

---
## \#5 Posted by: Newby Posted at: 2018-10-02T22:40:45.271Z Reads: 176

```
double check its working because it's unusual to take out 3 series groups, unless it's more than one bad cell
```

---
## \#6 Posted by: darkkevind Posted at: 2018-10-02T22:50:27.618Z Reads: 168

```
If you have one bad cell in a parallel pack, you now have X amount of bad cells in a parallel pack... All linked cells will be dead and need replacing.
```

---
## \#7 Posted by: Savace Posted at: 2018-10-02T22:55:48.356Z Reads: 168

```
How could i check if its working? I have looked up  all other series in all other groups are balanced fine, Would you agree that it could be the center row of that group as it its showing as 3.29 - the others are at 3.58 (the board has been sat there for 2-3 days since it cut out last so they could have ended up charging the bad series)

Debating if its easy just to swap out the entire row.
```

---
## \#8 Posted by: thisguyhere Posted at: 2018-10-02T23:04:52.937Z Reads: 165

```
it's no wonder you're having issues.

you've probably pumped A LOT of heat into your cells soldering it together.

just immediately you've got a cell isolated, no longer a part of a P group:

![image|672x500](upload://2zVNH8kkmkigFFEsVhyM2yyIY9W.jpeg) 

you've probably got a bunch of shorted out cells on the positive end of one or many of your cells.

frankly, this is one of the most frightening battery packs i've seen in a long time.

it's probably not realistic to start over but...i'd start over.
```

---
## \#9 Posted by: Newby Posted at: 2018-10-02T23:08:12.067Z Reads: 155

```
As @darkkevind said the row is shot now and needs replacing. But it's possible the whole group could need replacing aswell. Although oddly, (3.8+3.28)/2= 3.54. Could be a coincidence or maybe the bms found the middle ground
```

---
## \#10 Posted by: moon Posted at: 2018-10-02T23:09:36.182Z Reads: 154

```
![image|661x500](upload://l0y8tWXF6tt3yxnEDvK9U32baGe.jpeg)
```

---
## \#11 Posted by: mikenyc Posted at: 2018-10-02T23:10:09.559Z Reads: 148

```
wow .. this looks like a time bomb
```

---
## \#12 Posted by: Newby Posted at: 2018-10-02T23:10:21.706Z Reads: 148

```
I didn't even know where to start on the build quality so stayed quiet. I can feel my blood pressure rising the more I look
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-10-02T23:11:35.470Z Reads: 151

```
i have sweaty palms looking at this.
```

---
## \#14 Posted by: Lumaci Posted at: 2018-10-02T23:43:51.159Z Reads: 146

```
Im out of words, this looks dangerous. 

But the issue is most likely the one in the pics.
```

---
## \#15 Posted by: rojitor Posted at: 2018-10-03T02:29:36.719Z Reads: 136

```
![DoSvZd5XgAENY0W|418x409](upload://m7sWMTgGc0ySxse4S3cgvzw5hfQ.jpeg)
```

---
## \#16 Posted by: rojitor Posted at: 2018-10-03T02:32:39.276Z Reads: 135

```
On a second thought maybe my pic has been rude. Well... I am not a soldered packs fan. I think they are dangerous and easy to fail.
I hope you fix It.
```

---
## \#17 Posted by: Schulerbible Posted at: 2018-10-03T02:46:19.685Z Reads: 132

```
Quite a horror show :slight_smile:
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-10-03T04:27:49.771Z Reads: 131

```
Cold joint here in blue. It looks like the pack received some high G force and has changed shape a bit which has made some cells move and (possibly) break the connection. The hot glue has come off some of the cells. Or OP did that trying to disconnect the two cells. 

![image|690x470](upload://alsicXh4CfjILOkYMnyxk0K3Egc.jpeg)
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-10-03T04:32:59.280Z Reads: 131

```
[quote="Savace, post:1, topic:69912"]
I have guessed two of the cells and cut them out the series
[/quote]

Maybe we missed this guys, the two broken connections where cut as part of the diagnostic.
```

---
## \#20 Posted by: Eboosted Posted at: 2018-10-03T04:41:54.285Z Reads: 130

```
You should carefully disassemble the pack, clean the cells with solder wick, test them, discard tha bad ones, balance the rest of them, spot weld them, use fish paper between the cells and rings between the positive terminals.
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-10-03T04:46:14.769Z Reads: 130

```
Just under this melted white insulation is the negative contact. With time and vibration you could have a :fire: I bet many of the cells look like that under the copper bus bar from the heat of soldering. 
All the positive ends should have the fish paper circle insulations. I would at a minimum rebuild all the positive sides if you want the pack to be safe after solving the bad cell issue. Sorry to spam your thread. 
![image|690x297](upload://7VDanGSf9532rVTyEYtWAloE1xF.jpeg)
```

---
## \#22 Posted by: b264 Posted at: 2018-10-03T07:17:39.704Z Reads: 115

```
[quote="Eboosted, post:20, topic:69912"]
clean the cells with solder wick
[/quote]

This will just get them hot again.  Less heat is better.  IF that was to be done, only on the poisitive ends for sure
```

---
## \#23 Posted by: darkkevind Posted at: 2018-10-03T08:20:15.431Z Reads: 109

```
All that's separating these cells, insulating them from one P pack to the other on top of it, is about 0.2mm of heat shrink! No + ring protectors either! 😯

Honestly I'd either bin these cells and get a properly built pack or if you really have to, de-solder everything, disassemble them all and start over with proper insulation and silicon coated wire...
```

---
## \#24 Posted by: Newby Posted at: 2018-10-03T08:37:58.460Z Reads: 101

```
I bet there's friction scuffs already on the heatshrinks. 0.1 now. The balance wires look like they're rubbing and the BMS isn't even wrapped up. Parralel connections more built up than series?
```

---
## \#25 Posted by: Newby Posted at: 2018-10-03T08:41:39.121Z Reads: 101

```
If you have to take it apart use a Dremel or some wrenches to pull the copper out. The less soldering the better. When you build batteries you need to imagine if anything close or overlapping were to make a connection. Which usually ends in catastrophic failure unless it's a p group. For a 12s10p you need a lot of fishpaper
```

---
## \#26 Posted by: rich Posted at: 2018-10-03T10:19:23.273Z Reads: 90

```
That's a bomb!
Or at least the picture which @rojitor posted. 

Get rid of this battery, I know it's a lot of money but how much is your life or your family worth?

The hot glue has no contact, no isolation at all, mechanical stress on all solder joints only, no padding (on a MTB bro, that must shake well). How long did you use this battery?

I know there are not much fans of soldering Li-ion but it's possible. Soldered this pack with 80-100W iron, flux, flat copper wires (3mm²) and copper bar for serial connections (4mm²), works flawlessly.

![112038h|690x388](upload://lHX08SSnZ4gjXYsQOupsT33b6vl.jpeg) 
![221416h|690x388](upload://izMgdITEo8icUd03ncvO8hdgx0T.jpg) 
![220157e|690x197](upload://x7NjBbfiD8cuwflnZichEEaB4fb.jpg) 

Furthermore I put fishpaper on all battery poles after soldering and heat shrinked all paralell packs. Between the packs is 2mm neoprene rubber and also around. Everything inside enclosure is glued with flexible glue.

After my heavy crash where I destroyed the front truck and cracked the deck only 2-3 packs shifted a bit but everything is working also thanks to flexible wires and padding. If I had your battery it would look different.

Please rethink your battery design, it is very dangerous.
```

---
## \#27 Posted by: Savace Posted at: 2018-10-03T21:24:17.011Z Reads: 77

```
all- thanks for all the responses - a note on the board , this is my first eskate and I purchased it used about 3 weeks ago for 800 quid , I come from a quadcopter background so know what I’m doing when it comes to the electronics - never used a BMS on a quad so had to read up how it worked and did kind of think that the way this was wired looked dangerous! I have gone on it at least 10-15miles /charged it twice only as kept cutting at 44v, i had not opened the case as it was cable tied shut (i thought cabled tied to the board) so had not seen the state of the battery.

However I have taken your comments on-board (no pun) everyone's shock and horror at the pictures and rojitor's picture made me pull the trigger and I ordered 4x16000mAh 6s Lipos, will run them as 12s2p (2 for spare to take with me on long rides - the battery box can take all 4 with room to spare) , would I need a BMS with 2x lipo or could i just wire them in? If so could i use the one i already have? Either way I would remove the batteries and use a balance charger to recharge them everytime. And I agree it looks like a real mess ! Thanks for all your replies. Took me so long to reply as i had reached my post limit and had to wait 24hours!

I removed all the 18650's and thought you would enjoy the pictures, any one want to buy 120x18650 buy assumes all responsibility :D lol  :smiley:

![IMG_2521|666x500](upload://xlGtFOx3uCyvwjCyfWPMHA8BJlz.jpeg) ![IMG_2520|666x500](upload://8hRB2xwCTPwRs5ifj8SUwcjeBsi.jpeg)  
![IMG_2519|666x500](upload://7TRjo1HiuG8bMw6TE2cdaFQbxse.jpeg) 


And the board:
![A3D8D2F7-3AEA-46C1-90CE-592B396CF946%20(1)|690x388](upload://3sLZBOaAsXgLT7OFmkxSMqPwoI6.jpeg)
```

---
## \#28 Posted by: Acidfie Posted at: 2018-10-03T22:24:51.088Z Reads: 77

```
lol dude, how many different cells are those :smile:

no self-praising here, but thats a good soldering

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/2/d257ade9f169847f7e42518bf70ed5d201af8351.jpeg)
```

---
## \#29 Posted by: lrdesigns Posted at: 2018-10-04T00:50:25.462Z Reads: 71

```
I was wondering where you went. Haha. 

That battery may get the award for the worst one on this forum. :nauseated_face: :face_vomiting: :fire: There is nothing about the construction that could be considered even sub standard.

That BMS is ultra weird too and the size of bus. It must be recycled from something large. 

If you have a hobby charger you can just ballance on every charge cycle and not use a BMS. Just one tip though, hotglue all the ballance connectors wires just near the plug, both battery side and charger side. I found with constant use one pin can come loose and you could charge the pack minus one cell and not notice.
```

---
## \#30 Posted by: sk8l8r Posted at: 2018-10-04T07:55:04.779Z Reads: 61

```
OMG there are more of them LOL

I'm getting anxious just looking at the pics, get those somewhere fireproof ! :slight_smile:
```

---
## \#31 Posted by: Savace Posted at: 2018-10-09T20:17:38.411Z Reads: 43

```
Well everyone - Thank you all for your help, thought you may enjoy an image of the battery bay now :slight_smile: 

![IMG_2571|375x500](upload://emDRmZUkreiEJH0NZakucWho60z.jpeg)
```

---

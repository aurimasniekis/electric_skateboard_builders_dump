# Horská doska - Dougie&rsquo;s mountain board build

### Replies: 48 Views: 2159

## \#1 Posted by: DougM Posted at: 2018-06-13T01:45:36.916Z Reads: 306

```
So in the past I've been very bad about documenting any of my builds, so this time I thought I'd start with the documentation in the hopes that while I build it I won't have any excuse not to put down the details here while it is in progress.  

The board will be a dual motor mountain board.  In my inexplicable tradition of giving all my boards Slavic names I've chosen horská doska, roughly translated from Slovak as Mountain Board.

The budget is about $100 per month, plus the occasional splurge.  So it'll likely take me until next summer to get all the pieces.

The design I've been using in the past, extruded rail drop decks, has worked really well and this one will be the same.  I will spend some time rendering it in Solidworks so will post renderings here.

1) batteries will be 10S6P of the new 4kAh Sanyo 20700's.  While these will give me epic range, they are only 15A batteries so the 6P will give me 90 Amps, which seems to be a pretty good budget for a dual motor (45A per motor)
https://liionwholesale.com/pages/search-results-page?q=sanyoncr20700b
I spent this month's budget on the first 12 of these.

I thought about making a carbon fiber frame, but with such a ridiculously heavy pack and 2 motors there isn't really any point in trying to shave weight. 

Wheels will be 6" pneumatics.  I'm currently thinking about converting Evolve's conversion kit:
https://evolveskateboardsusa.com/collections/gt-carbon-parts/products/gt-series-all-terrain-conversion-kit#tab3

Probably, since I want this to be a super-reliable board, I'll steal the VESC6 out of the WidowMaker (which used to have a slavic name before it tried to kill me) and get another VESC6.  Or B) if the dual FOCBox comes out in time I might get one of those.

This opens up the possibility of turning Widowmaker into a dual 5065 using 2 VESC4.12's.

I really want to play with the flexboardz suspension, but I don't have sufficiently detailed drawings or models to reproduce one, so that would be a big experiment.  Failing that I'll just go with mountainboard trucks.

I've been looking for another Tacon Bigfoot 160 to use in this build, but you can't seem to get them anymore.  So I'll probably go with the 6355's that I put on my first dual motor build.
products/electric-skateboard-motor-6355-190kv
These are sensored, which is probably better anyway.

I'm also going to try for direct drive.  Years ago I made a gearcutter, so I guess I'll have to dust it off and try to remember how it works.

There are some great projects for remotes going right now, so by spring I expect there to be some great new products (or DIY's) available, so that'll be the last thing on my list.

More to come!
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-06-13T02:21:03.711Z Reads: 254

```
dont go evolve at kit, go w/ psychotiller wheels. i have the at kit its been a pain w/ the 6355 and cutting shafts ect..
```

---
## \#3 Posted by: Battosaii Posted at: 2018-06-13T04:44:35.183Z Reads: 250

```
I can vouch for the psychotiller wheels they are awesome. I'm riding my Raptor 2 right now and it feels sketchy I'm already used to Pnumatics lol
```

---
## \#4 Posted by: DougM Posted at: 2018-06-13T05:14:18.216Z Reads: 249

```
Thanks for the guidance - I was trying to save a bit of dosh, but I definitely don't want to muck around with having to re-machine the wheels.
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2018-06-13T05:18:40.613Z Reads: 243

```
Expensive but worth it for wheels. 6355 are great motors also just got me a new set same ones. I used liion for my cells I hear imr cheaper.
```

---
## \#6 Posted by: DougM Posted at: 2018-06-13T05:26:21.718Z Reads: 245

```
I cadded up the frame tonight - just so you can see what the thing will look like.

Trucks are off GrabCAD and are just temporary.  I need to fit the batteries next to determine the rail width.

![image|690x497](upload://lH6GkD12jnWMybtjvzZOv8eKTTS.png)

![image|690x121](upload://nDK1ubsFpdXy7J3coijEPia7kpo.png)
```

---
## \#7 Posted by: DougM Posted at: 2018-06-15T02:05:33.986Z Reads: 216

```
The first 12 20700's have arrived :-)

![IMG_20180614_190546|374x500](upload://yVPRDBRuAnwLUCmlDVzw66UBr5K.jpg)
```

---
## \#8 Posted by: DougM Posted at: 2018-06-17T00:03:23.632Z Reads: 215

```
I started working on the FlexBoardZ replica suspension but didn't get very far.  

![image|690x313](upload://166mHVlLFHvvRGypgRdEcv0CFTe.jpg)

Mostly because I got distracted by a taillight.

![image|690x327](upload://9cVyx1z38RHkqlqZof12Zs07AlY.jpg)

I have a trip coming up on a newly paved road called the Middle Fork Road.  It's long and windy and beautiful, but it has no painted lines and there is vehicular traffic on it.  So I decided a hi-vis vest and a really bright taillight was in order.

![image|690x434](upload://wvbZCTUwdJ6GwoU21k7TDUou42a.jpg)
_(proving once again that digital cameras and LEDs don't match - it's red)_

There's not much interesting about taillights (this one is 3D printed out of clear PLA) except that there are these incredibly bright LEDs called Luxeon Z's.  They are tiny and put out an incredible amount of light using a very small amount of electricity.  I'm pretty sure most cop lights use Luxeon Z's.

[Luxeon Z Digi-Key](https://www.digikey.com/product-detail/en/lumileds/LXZ1-PD01/1416-1053-1-ND/3961158)

I use 18 in series with an 80 ohm current limit resistor.  It's tied into the anti-spark switch, so gets the full 10s pack voltage.
```

---
## \#9 Posted by: DougM Posted at: 2018-06-17T02:52:28.557Z Reads: 207

```
Ok, based purely on looking at pictures of this type of suspension I found on the interwebs here's what I think it will go together like

![image|690x470](upload://nprJQ5AakXfG7lRFon6uCcCiRMV.jpg)

I'm still missing the lower links, but a beer and a burger are calling my name.
```

---
## \#10 Posted by: DougM Posted at: 2018-06-21T04:45:52.655Z Reads: 203

```
I 3D printed the mount block last night for test fit.  It looks really nice but I don't think I'm going to be able to use that design.  

![IMG_20180620_213035|666x500](upload://ocOXH7tprYWnQOPztHwvm2aBP2k.jpg)

I spent some time last night puzzling over how to attach it to my frame, and while I could attach it to the same mounts I usually attach the trucks to this seems like a hack.  I'm going to spend some time braining up a more integrated attachment.  I think I can integrate the lower links nicely into a slightly modified version of the drop plates I'm currently using.

Next up is ordering some aluminum extrusion to make the cross bar.  Ironically [OnlineMetals](http://www.onlinemetals.com/) is local to me.  I'm going to pick up [1 inch](http://www.onlinemetals.com/merchant.cfm?pid=14469&step=4&id=1270&top_cat=60) and [1 1/4 inch](http://www.onlinemetals.com/merchant.cfm?pid=18015&step=4&id=1270&top_cat=60)

I also need to find some ball joints for the lower links.  McMaster 2458K32 look good on first blush  

Also it seems prudent to get some UHMW sheet with adhesive on one side so I get nice smooth action between the parts.  Probably McMaster 1441T91
```

---
## \#11 Posted by: DougM Posted at: 2018-06-22T04:38:50.024Z Reads: 201

```
Made a little bit of progress on the trailing arms

![image|688x499](upload://q4mrhFb5lgYfgoVS5rKzQEb5I0k.jpg)

and mounting the thing to the frame

![image|690x350](upload://f73G8h3CUORD4gkpW6i3RXyoRfS.png)

Probably those plates don't need to be so long - that's kind of a relic of the previous design.  But then again it'd be nice to have someplace to put all the electronics.  I could see tucking a little box up in there with a couple of FOC's.
```

---
## \#12 Posted by: DougM Posted at: 2018-06-23T01:35:22.477Z Reads: 195

```
Metal has arrived :-)

![IMG_20180622_181431|666x500](upload://miw55KPt839bFiBYArFcBUBCjY6.jpg)
```

---
## \#13 Posted by: DougM Posted at: 2018-07-01T16:15:32.080Z Reads: 182

```
Got a small windfall from a computer job so I put in my order for Psychotiller pneumies.  Very likely they'll get tested out on Farkassem, (the dual motor board), before they go onto this one.  Unless the trucks aren't wide enough.

I tried to ride in Bend, Or, but the trail out of the park was cobblestone and then turned to gravel.  So I didn't get very far.  Sunriver has 26 miles (!) of curvy, hilly, smooth beautiful trails, but they don't allow skateboarding, wah wah.
```

---
## \#14 Posted by: DougM Posted at: 2018-07-05T00:09:07.386Z Reads: 183

```
The first trailing arm is complete(ish).  Clearly I forgot to think about wire routing but that's an easy fix.

  ![IMG_20180704_164801|666x500](upload://3K6DIB16xvhQLThR0ZMr9dx7Izn.jpg)

I really need the Psychotiller pneumies to come in so I can test-fit everything and figure out how long of an 8mm bolt I need to order.

In the meantime I'll work on the cross-brace.  But I need some 1.5" 6061 round stock which I don't have, so I'll have to wait for another order.  Which is ok, I only have today and the anti-spark switch on Widowmaker has failed on (which I guess is better than failing off) which makes me cranky.

_Update_:  the anti-spark switch problem turned out to be a loose wire.  Perhaps using screwterms in a high-vibration environment was another of my not-so-bright ideas :-)  In any event, screwed the wire back in and Widowmaker is back on the road.
```

---
## \#15 Posted by: Lionpuncher Posted at: 2018-07-05T00:35:56.941Z Reads: 169

```
This looks awesome man! Looking firward to watching the progress of this build. I'm using 20650's for my current build. Lg's, but for different reasons. They are legit 30 amp discharge so I'm using them for a smaller pack. Keep the awesomeness coming!
```

---
## \#16 Posted by: DougM Posted at: 2018-07-05T00:50:30.970Z Reads: 165

```
I just also put in an order for another 24 20700’s.  That gives me 6S in case I want to do some test riding before I can afford the rest of the batteries.
```

---
## \#17 Posted by: DougM Posted at: 2018-07-06T03:58:38.541Z Reads: 173

```
Mmmm, shiny things...

![IMG_20180705_185115|375x500](upload://gdu7gaE1tNtDM9HF3U6i0pLAijJ.jpg)
```

---
## \#18 Posted by: DougM Posted at: 2018-07-08T04:59:11.149Z Reads: 169

```
I know all y'all have been wanting to ask me, "but Doug, what happens if the material you designed to isn't the same as the material you ordered?"

Well, I'll tell you...

![IMG_20180707_203309|374x500](upload://bEQtxLmIsKzdbGKFhGupqGDBv17.jpg)

THE PARTS DON'T FIT! :slightly_frowning_face: 

Turns out this is kind of a fortuitous mistake, though, because the wider box channel means I don't have to mill out the other side of the cross-brace which will make it considerably stronger.
```

---
## \#19 Posted by: High-roller Posted at: 2018-07-08T06:20:05.192Z Reads: 164

```
I am so following this!!! Good to see more swing arm designs coming out! 
If this works will you consider posting the cad files so people can make their own?
```

---
## \#20 Posted by: DougM Posted at: 2018-07-08T15:33:21.359Z Reads: 161

```
@High-roller -  Absolutely.  I'd love to see people improve on the design.  I will post the files once I know that the thing actually works.  It's completely designed based on pictures I found on the Google.  There aren't any documented swing-arm builds out there that I could find.
```

---
## \#21 Posted by: DougM Posted at: 2018-07-08T15:35:48.611Z Reads: 141

```
@psychotiller - any chance you can look up order 9204255?  I really need those wheels to continue the build and they were ordered on the 28th and still haven't shipped.  Thanks.
```

---
## \#22 Posted by: High-roller Posted at: 2018-07-08T16:14:23.255Z Reads: 144

```
I'm trying one kind of like this:
https://www.electric-skateboard.builders/t/wtf-is-this-unknown-build/31121 sort of like this:
I'm planning on pairing a set of those trucks with a "29 jet Spud. I'm still trying to figure out how to attach them to the deck without drilling extra holes or putting unnecessary stress on the deck.
```

---
## \#23 Posted by: DougM Posted at: 2018-07-08T18:53:26.110Z Reads: 150

```
@High-roller  Looks pretty easy - you just need a big block of aluminum for the holes for the upper and lower control arms, then you can transition back to a regular skate truck pattern, like flexboardz did here:
![plateau%20dessous|666x500](upload://jg2Z7gqA5lYeLAK0vn7GEhFRIi.jpg)

Are you building the suspension from scratch or did you find one on eBay?
```

---
## \#24 Posted by: High-roller Posted at: 2018-07-08T20:32:55.478Z Reads: 151

```
I bought BMW streetcarver-style trucks from a guy here on the forum. I was thinking I'd 3d print the plate like you mentioned, instead of making it from aluminum, in order to save weight and cost. Since the original holes were spaced out wider I'm worried that using a plate to bolt it to the four standard holes will concentrate the steering forces on a smaller area, possibly causing more mechanical stress to the deck.
What do you think?
(Bty, my apologies, I didn't mean to hijack your thread)
```

---
## \#25 Posted by: DougM Posted at: 2018-07-08T21:36:52.428Z Reads: 147

```
I'd have to see pictures of what you bought to know exactly what to recommend, but If you are 3D printing what I think you are 3D printing then that will blow apart long before the deck does :slight_smile:

You  can sandwich the board between thin(ish) aluminum plates to distribute the forces.  Think of a standard skate truck riser but instead of being the same size as the truck it's maybe 3/4" larger on all sides.
```

---
## \#26 Posted by: DougM Posted at: 2018-07-09T02:13:06.151Z Reads: 148

```
So it's becoming a thing!

![IMG_20180708_184523|374x500](upload://od5WAdzEj5ziAraX3gjs7KWpoE0.jpg)![IMG_20180708_162054|375x500](upload://duDguDjVPVMqNXSsFBy6IsN9fDd.jpg)![IMG_20180708_165327|374x500](upload://fypuyL75VK1sUPTl8mZje10reH5.jpg)

I knew I was going to have to rework the trailing arms because if I want geared drive the motor needs to be closer to the wheel, but also in looking at the way it goes together the lower link needs to be horizontally in line with the suspension bushings or it will either twist or bind up.  So that has to be moved (or depending on how squishy I want the suspension to be I might add a drop plate to line them up.

In the meantime I can always belt-drive the wheel (I think the Psychotiller's come with belt cogs) just to get it on the road.  I am also going to put a standard truck on the front just so I can test the rear in the real world.  If I need to make changes I only want to make them on one end, then when I have it perfected (or approximated) I can reproduce for the front end.

But the real test is whether the thing turns at all or whether I'm making a huge pile of aluminum scrap.  With luck that question will be answered next weekend.
```

---
## \#27 Posted by: DougM Posted at: 2018-07-14T19:59:45.809Z Reads: 134

```
I went on a group ride on Thursday and there were 2 people there with mountain boards - In talking to them I'm pretty sure I under-spec'd the size of the tires, so I'm switching up from the 6" pneumies to 8" pneumies.

I'm going to try to get the gearcutter up and running this weekend - if I do I'll post a vid if I can, or piccies if I can't.
```

---
## \#28 Posted by: Okami Posted at: 2018-07-15T15:07:26.792Z Reads: 129

```
Do u think your system might allow some form of shock absorber to be installed?

 I imagine if tilting arm gets fixed in place with shock absorber it might absorb road vibration / irregularities as well
```

---
## \#29 Posted by: DougM Posted at: 2018-07-15T15:14:09.975Z Reads: 132

```
Yes you can put bushings on the lower link.  If you look at the FlexBoardZ suspension you can see the rubber bushings in the right side of this picture:

![image|690x220](upload://2OJgyoncYsciBwtSc7GqVLdfbJp.jpg)

I was planning on starting with various types of skate bushings and then go to springs if I need to.  Fortunately the way my design came together I have tons of space available in that area.
```

---
## \#30 Posted by: DougM Posted at: 2018-07-19T00:53:04.281Z Reads: 130

```
I know all y’all have been wanting to ask me, “but Doug, what happens if you accidentally go on Criagslist just to see what's there?

Well, I'll tell you what happens, you come home with this:![2841|375x500](upload://shlQv0C5zD7QTK3PvcaI8Yy2xZ0.jpg)
Mostly I just wanted the trucks, but actually it's a really nice board.  

In any event the wheels are 8" which is my target diameter.  So this represents an opportunity to get going on the spinning mechanicals at the same time I can keep working on the trailing link suspension.  

Now I just need to figure out how to mount motors to those trucks.  That's my goal for tonight and tomorrow night.
```

---
## \#31 Posted by: DougM Posted at: 2018-07-20T04:33:38.053Z Reads: 125

```
So I got the bracket figured out for putting the MBS Mountain Board trucks on the Doska.  It's 21 degrees, which seems to be what the MBS deck angle was.  (correct me if there is an official angle for these things that's other than 21)

It shouldn't be that difficult getting this up and driving around - I don't see any big blockers.  Probably, honestly, I'll play on it until fall and then switch it all out for the trailing arm suspension for a spring debut.

![image|690x328](upload://zipDYHJU8aXDw7cIG17oIt4zaZp.jpg)

I'll throw the MBS wheels up on Thingiverse but the truck is kind of an embarrassment since I didn't have time to model it up properly.

I ordered some Delrin to make the cogs.  The MBS drivetrain will be chain drive since they are temporary - I'll focus on the gear drives for the trailing arm version.  This is the cog to mate to the MBS wheels.

![image|597x500](upload://7zqrTvy3u3JJLc4Pa9NrePTv2l9.png)

I also got a basic motor mount worked up and 3D printed a test - it looks pretty good so I've got some aluminum on order to make those.  I don't want to make the final motor mount until I can actually bolt the cogged wheel onto the truck so I can do some chain length reality checks.
```

---
## \#32 Posted by: DougM Posted at: 2018-07-23T04:30:43.257Z Reads: 119

```
The weekend got away from me but I did manage to get the risers made.

![IMG_20180722_200434|666x500](upload://mxy3a1psGGgtDF08Y8oFx4gX188.jpg)

Unfortunately some of the metal I ordered is on backorder so I'm not sure when that will arrive, but the Delrin should be here tomorrow. BUT. . . that might not do me any good because my little tabletop CNC mill might not have enough Y-axis distance to make the cog.  It's 5.6" and the table range is 5.7" so we'll see if I can squeeze it in there without hitting the hard stop.

UPDATE:  I can do it!  I manually moved the Y axis all to the way to the end, backed it off a half a turn, then powered it up and test-ran the pattern and it didn't hit any of the hard limits.  Score 1 for the little Taig!
```

---
## \#33 Posted by: DougM Posted at: 2018-07-24T03:41:28.205Z Reads: 115

```
I know all y’all have been wanting to ask me, “but Doug, how the hell do you make chain sprockets anyway?  Well, I'll tell ya, it's kind of a hack.

So my chain is ANSI #25, which basically means it's about half the size of bike chain.  Getting the chain isn't too difficult, but it's kind of tricky to find a chain breaking tool, but they are out there.  I ended up making my own, but that's a much longer story.

So to start with you have to go to one of these cool esk8 calculator sites and decide on your gear ratio.  I gear all my boards, more or less, for 25mph.  This seems to be the sweet spot between enough power to climb hills and slow enough so I don't die instantly.

My current board has 4" tires, for the sake of this calculation I want to reproduce the exact same gear ratio only for the 6" Psychotillers (those of you who don't have a life and have actually read this whole thread will realize that this is a complete diversion from the 8" MTB wheels I just got.  This is because I really want pneumies on Widowmaker, I already ordered the Psychotiller wheels and all my aluminum and Delrin for the 
Horská doska build is on backorder.  So here we are.)

So it just so happens that you don't really need to do a lot of calculatin' to figure out that 6" is 150% of 4" so you just take the number of teeth on your current board and multiply by 1.5.  My current board is 11:34, so the new board is 11:51.

But let's say, like me, that math isn't your strong suit.  Then you can just go to this esk8 calculator website:

http://calc.esk8.it/

and enter a bunch of numbers.  Here are mine for Widowmaker:
![image|652x500](upload://7qg98IomVCOvXPr0uUbt6HVsIt9.jpg)

So my top speed is 26.4 mph.  Now change the wheel size from 4" (102mm) to 6" (153mm) and then just ditz with the Wheel Pulley Teeth until the number is about the same:
![image|651x500](upload://sHjya6nxq3KfxOrnSRRSPVbMVIu.jpg)

Ok, so now let's make the cog.  Go to this website:

http://www.idleamusements.com/?page_id=367

and super handily in the "Common Chain Sizes" table it tells you everything you need to enter except the number of teeth.  In our case ANSI 25 is 0.25 Pitch and 0.13 Roller Diameter.

Now just enter the number of teeth (51) and hit the "Submit" button.

What you get is a DXF output and a GCODE output.  Download the DXF output and load it into your favorite 3D manipulation software (mine is Solidworks because work bought me a license) and what you get is something like this:
![image|565x500](upload://mhVhMYefVFyzhHxTZitevDCgIHx.png)

The inside width of the chain is 0.125, so I extrude the gear out to about 0.120.  (it actually doesn't matter since I just turn it back into a 2D DXF when I put it in my CAM software).

I don't like the pointy teeth, so I remove an arbitrarily small amount from the edge:
![image|402x500](upload://zLLOMCAPeQoKSVYewHaEsNl3BG9.png)

The particluar Delrin I bought is 3/8" thick, so I add the thickness back in a little bit in from the teeth. 

Now add the holes to attach it to the Psychotiller hubs, which are a 6-bolt pattern about 1.895" apart.  They are either 10-32 or M4, so using a TAP and Drill chart (https://littlemachineshop.com/reference/tapdrill.php) make the holes 0.1960".  Also add an arbitrarily sized center hole.  Mine is 1.4" Dia.

All said and done it looks something like this:
![image|489x500](upload://yPCICsVGgKAC6PKuRY454yCoqxi.png)

Export the thing back out as a DXF:
![image|514x500](upload://2kdB0OTtt2cL459zGYVrv9HDkNn.png)

And you're ready to CAM.  That's another post.
```

---
## \#34 Posted by: DougM Posted at: 2018-07-27T05:39:48.672Z Reads: 103

```
Got the truck brackets made.  It required a bit of imaginative and foolhardy fixturing to cut the angles:

![IMG_20180724_192628|374x500](upload://zUUY0uUqsd3Y0yRQg82c7xG525n.jpg)
_Kids, don't try this at home!_

Got the brackets and trucks mounted on the frame but didn't have time to put the wheels on.  I still need to do something about a deck.  I'm seriously thinking of doing bigfood pads instead of a standard deck;  Something derivative of this:
![image|225x297](upload://rFva3PRTn8sjST2h1xKGXRrJA87.png)

I CNC'd the driven cogs:
![IMG_20180726_221244|374x500](upload://119rkDeCOVP1klEMcQ9iwMwEw4f.jpg)

But I still need to finish them out on the lathe.

I'll definitely have a rolling chassis by the weekend.  Maybe get some battery packs welded up but doubtful it'll run under its own power.  There's still a long ways to go especially since I'm waiting for the FOXBox Unity to ship.
```

---
## \#35 Posted by: xilw3r Posted at: 2018-07-27T10:30:10.278Z Reads: 95

```
I never completely understood how the flexboard works. Especially since it can carve so steep.

So basically the swing arms can... emm swing. And the actual steering happens in the main block that hold the swing arms and is bolted to the board. And then the underside has just reinforcements running on the sides ..for reasons. But the ammount this thing can tilt and the reinforcements dont fit in my head. And I really wonder how the main block is constructed.

Hope your project works out man.

https://www.youtube.com/watch?v=uQHykgcGW7Y
```

---
## \#36 Posted by: DougM Posted at: 2018-07-28T15:42:06.094Z Reads: 95

```
[quote="xilw3r, post:35, topic:58701"]
I never completely understood how the flexboard works.
[/quote]

Me neither actually :-)  Since everything I've done to date has been derived from photographs there's going to be a lot of tweaking even after it's built.  Then we can spend some time determining how changes in the various components affect ride.
```

---
## \#37 Posted by: DougM Posted at: 2018-07-29T02:24:42.546Z Reads: 91

```
As promised, rolling chassis by the weekend (barely).  If you look really closely you can see that the new Delrin cogs are installed on both rear wheels.

![IMG_20180728_104503|666x500](upload://370Tv0NLzJOwjMDiq5DwJxWlYwc.jpg)

I did get the deck CNC'd (I did the standard deck for now, not the bigfoot feet) and I spent some quality time trying to figure out how to make a motor mount that will fit around these trucks.  Right now it looks alarming like the Starship Enterprise.

![image|690x379](upload://bmr87CEjjNCtMQ5uwowlrqHukZt.png)
```

---
## \#38 Posted by: DougM Posted at: 2018-07-29T03:34:01.446Z Reads: 95

```
I know all y’all have been wanting to ask me, “but Doug, WTF, don't leave us hanging, how do you CAM the chain sprockets? Well, I’ll tell ya, it's all about feeds and speeds.

Actually it's not,  It's all about feed rate and depth of cut.  And the kind of end mill you get.  I haven't changed the speed of the spindle since I unboxed the mill.

So unfortunately I don't use an open source CAM package, use something called CAMBAM, which, at $150, is actually kind of a bargain.  It is only 2.5D, though, even though it says it's 3D.

Also. since we're in the disclaimer section, I use a Taig desktop mill (2019CR-ER).  It's a tiny thing that can be delivered by UPS and I can actually pick it up and carry it into the house.  Of course once I've carried it into the house I'm constrained from doing wet cutting and misting and those sorts of things.  So I dry mill.  This has a negative impact on the finish of the part, but otherwise it wasn't a big deal to adjust my cutting style to compensate.

A word about end mills.  You can't go wrong with a 2-flute cutter.  You can go totally wrong with a 4-flute cutter.  You can go halfway wrong with a 3-flute cutter.

In this case, since I'm milling teeth for a ANSI #25 chain the biggest cutter I can use is 0.125"  But generally you want a cutter that's slightly smaller than your smallest feature.  Unless you have a tool changer.  Which I don't.  

For aluminum 2 flutes is the max.  For plastics you can use 3-flutes, but you have to be careful about melting.  Especially if you're milling plexiglass.

So this is the point at which we talk about magic numbers.  I have a set of numbers for each material I machine.  Aluminum is different than Delrin, which is different than Starboard, which is different than Nylon.  But Nylon and Delrin are pretty much interchangeable.

For every material I've machined I have the following values:
Depth increment (DI): how deep the cutter goes on each pass. for aluminum this is 0.011".  For Delrin you can go 0.040".

Cutting Feedrate (CF):  This is how fast the table moves around.  For aluminum this is 9.  For Delrin it's 12.  I think this number is Inches per Minute.

Plunge Feedrate (PF):  This is how fast the cutter plunges down into the material.  Cutters don't like to drive straight down into material the way drill bits do, so I go pretty slow.  as a general rule I set my PF to be half of my CF.  Unless it's aluminum in which case the PF is 1.

Keep in mind that there's a tangential correlation between the size of your cutter and how aggressive you can mill.

BORING!  just show me pictures.

Ok, here's a picture of the cog as I modeled it last week and exported to DXF.  This is a purely 2D drawing.

![image|629x500](upload://xerMUBnsvvEzcJqUTT12zLFzF43.png)

Every single one of those teeth is comprised of about 5 polylines, so you want to join them all together to make one big polyline:

![image|509x500](upload://jLs3aMwfqs7U7r2oVK8iE4BMq6J.jpg)

So now all I have to deal with is 6 screw holes, 1 big hole in the center, and the teeth.  The rest I'll do on the lathe by hand.

Set Machining Origin:  This is where the mill will consider X=0; Y=0.  I always use the lower left corner.  In the image below the little red X is my machining origin.  When I put the material in the mill I just move the cutter to the lower left corner of the material and home all axis'  Z is a bit different but we'll get into that.
![image|387x454](upload://6odyk2GWga76dfO8PoTnluJwuMI.png)

Next, set your tool diameter.  
![image|299x115](upload://pWVESBRtrPfyFv2swwXyU9Jw7z3.png)

Next, I'm going to want the machine to separate the part from the surrounding material, so I need to add a cutout circle slightly larger than the teeth.

![image|512x500](upload://xKdMGKycPzlKT4vkPgHwTDOnsm9.jpg)

Ok, first drill some holes.  This little menu thingie here is all the milling operations I can do.  Number 5 is drill.

![image|223x74](upload://uOcjW1tOLRmxnXH18MYJKXkBaYg.png)

Basically now I just select the object I want to act on and apply the magic numbers we talked about above.

![image|350x261](upload://8IdFum6tfBkscJVrSOdVRFA0WIO.png)
_the green line is the circle we're working on, the blue line is the tool path.
_
![image|280x440](upload://lrbuCevCCoQjpdd8s4EOVSksWBl.png)

Note the target depth.  Remember that the Delrin I bought is 3/8" (0.375) so I add another little bit to make sure I cut all the way through the material.  I have a plastic sheet underneath so I don't cut into my milling table.

Repeat for all the rest of the holes:
![image|496x500](upload://nH6gLco23jB1JzR0YdSA072WP6F.png)

Now for the teeth I'm going to use a machining operation called a Profile (number 1 on the menu thingie).  But it's exactly the same as the drill, except that I'm not going all the way down since the teeth only have to be 0.120 wide I'm going to go to -0.200 and clean it up on the lathe.

![image|502x500](upload://5ko0h3axu4Z801l4pXODYqW6ntp.jpg)
_red is the teeth, green is the tool path

Now do exactly the same thing for the cutout, except go to full depth.  But wait!  On your cutout you need to add some holding tabs so the work won't try to run away.  
![image|508x500](upload://tce0rTlam8v32okXO6f6cf2kI1Q.jpg)
_this shows the whole thing - all tool paths, holding tabs, etc._

Installment 3 is where I actually cut the thing on the mill, which might happen tomorrow, but don't hold your breath.




_
```

---
## \#39 Posted by: Okami Posted at: 2018-07-29T07:17:51.908Z Reads: 84

```
Nice explanation.

 Havent had a chance to do such cnc work so far but im happy u have given an insight about some of the details related to it.

I touched the topic about flexboardz design a while ago but to make one happen, I guess a decent machine shop is needed. So im glad u are heading in this direction.
```

---
## \#40 Posted by: DougM Posted at: 2018-07-30T00:48:57.141Z Reads: 80

```
Aaaaaaaaaaaaaand we're motorized.

![IMG_20180729_173941|666x500](upload://p1teBrcUBoi1AoxxrKBZ6Qs5j4n.jpg)

left on the list:
[ ] mount deck
[ ] think about waterproofity
[ ] Mount VESC's (4.12's until the FOCBOX Unity is available)
[ ] get more batteries
[ ] weld up battery packs
[ ] wire everything together
[ ] add charge port
[ ] charge
[ ] ride

I'm a little lacking in torsional rigidity - need to give that some thought.
```

---
## \#41 Posted by: faithfulpuppy Posted at: 2018-07-30T02:33:05.597Z Reads: 73

```
awesome explanation dude! I didn't realize you could get CNC mills capable of cutting aluminum that small. What does one of those cost?
```

---
## \#42 Posted by: DougM Posted at: 2018-07-30T04:01:17.649Z Reads: 73

```
@faithfulpuppy about $1200 for the CNC ready version.  After that you have to provide your own stepper motors, drivers and software.  But I went this route because stepper motors and drivers are incredibly cheap now and I use LinuxCNC as the software, which is FOSS.

You can find them used on eBay if you're willing to take the risk.  

Taig just came out with the new 5 series which has ballscrews rather than the ACME the old one has.  Upgrading mine would cost $1,000 which I might do if I start see lash in the axes.  So far there is zero lash which is pretty amazing.
```

---
## \#43 Posted by: faithfulpuppy Posted at: 2018-07-30T04:09:35.269Z Reads: 66

```
oh shit, nevermind lol. I had assumed they cost around the same as similar size 3D printers
```

---
## \#44 Posted by: DougM Posted at: 2018-07-30T04:14:47.254Z Reads: 70

```
well, they do :-)  My Lulzbot mini was almost exactly the same price.  I will be the first to admit, however, that I bought the lulzbot because I wanted something that "just works" out of the box and on that count it did not fail.

Until I went to the latest software/firmware, then it was a flaming piece of crap.  Until I reverted to the software/firmware that it shipped with.  Now it's back to being reliable.
```

---
## \#45 Posted by: DougM Posted at: 2018-08-02T04:32:07.705Z Reads: 68

```
AAAIGH!  one Nickle shy of a complete battery pack!

![IMG_20180801_210122|374x500](upload://9O191XHRUAPDzTne0zvR0UtCKOy.jpg)
```

---
## \#46 Posted by: DougM Posted at: 2018-08-22T00:57:43.995Z Reads: 64

```
Well, I have news.  I've fallen in love.  With eFoils.  I know, and I'm sorry, but the lines, the grace, floating effortlessly over the water is the siren song I simply cannot resist.  Also, it hurts a lot less when you fall.

So instead of doing the trailing link suspension on this board this winter I'm going to wrap this up with the current suspension and mostly my traditional build methods; and bulid and eFoil.  I invite you to follow my build over here...

http://efoil.builders/

I haven't actually started my build log yet, but as soon as I wrap up this board I'll be learning about the complex, frustrating world of waterproofing things which, if you read my novel about my ride home in the hail, is probably something I need to learn :slight_smile:

TO THAT END, I'm actually putting the electronics in a box for the MTB build, so I needed to learn how to bend metal.  My idea is to build a box out of -6061 aluminum 0.060 thick by using a cheap Harbor Freight metal bender and then 3D print the end caps so I can route wires in and out.  I will be posting piccies of that here soon.

After that my Flipsky's have come in from @Hummie's group buy:

https://www.electric-skateboard.builders/t/flipsky-6-6-group-buy-its-on-115-w-2-day-shipping-and-tracking-usa/63725

My initial impression of them is pretty good - I had no problem connecting to them with VESC tool 0.95 (Note that 0.95 is brand new, if you're running 0.94 you won't have access to the 3.40 firmware that they come with)

I happened to have a 5065 on my desk, so I spun it up and configured it.  The target motors are of course the 2 6374-190's that are on the MTB, so once I get the Flipsky's mounted and wired I'll configure for those and with luck will have riding impressions up by the end of the weekend.

That means that the FOXBox Unity will end up on WidowMaker driving the 2 aforementioned 5065's leaving the genuine VESC6 to drive my eFoil!

Almost like I planned it.
```

---
## \#47 Posted by: DougM Posted at: 2018-08-23T02:53:06.262Z Reads: 60

```
So, let's talk about bending metal.  I started with a sheet of 0.060 6061 aluminum and I bought one of those amazingly cheapie Harbor Freight metal benders, which basically is 3 pieces of metal welded together with a handle, but amazingly it did the job...

![IMG_20180821_184327|374x500](upload://fwJSYNA6uVCAMKgYJmudAoSM77l.jpg)

The two things I learned are 1) make sure your bend is 90 degrees before you move on to the next bend because you won't be able to get it back into the machine; and 2) bending is an inexact science, so even though you are really careful to draw your lines in the right place there will be some variation, so account for it in your sizing.  In my case one of the wings was a bit longer than the other wing.

![IMG_20180821_184924|374x500](upload://yDz9YsUxbjDiqIgkKlmb03L2HSq.jpg)

The clever part, I mean I think it's clever, is that I can 3D print the ends, which means I can print all sorts of holes and connections and doodads in the end that would be much more complicated if I tried to make the end out of metal.

![IMG_20180821_214134|374x500](upload://356EkLpgCSi5mbxMML1vVfCsKrY.jpg)
Note this is an early prototype, the final ones will look like this:
![Box%20Motor%20End%20MTB%200v2|690x335](upload://iJbzjyCCwFPpKsv0Y9dHzHyP8Us.png)![Box%20Battery%20End%20MTB%200v2|690x365](upload://ysuJgma2mn4spmCCHknwhi3TxSo.png)

So this brings this capability within the skillset and budget of just about anyone.  The metal bender is dirt cheap, the aluminum is cheap, and everybody knows somebody with a 3D printer.

2 more quick notes - remember that aluminum and radio waves don't mix, so make sure your receiver is outside this box; and that aluminum and heat do mix, so mount your ESC's heat sink directly to the metal
```

---
## \#48 Posted by: DougM Posted at: 2019-01-28T02:10:50.817Z Reads: 42

```
Long overdue update.

I've still been working on this board a bit.  I made a cool Carbon Fiber battery cover for it, but the bad news is that I was running it with 2 flipsky 6.6's and one of them died.  Won't turn on anymore.  It's something in the anti-spark portion of the board, but I'm not sure I want to mess with it.

So I ordered another FocBox Unity.  I already have one of these and I'm pretty smitten with the fact that you can change settings from your phone!

So far all riding I've done with the Unity has not resulted in significant injury or Uber rides home, so I'm willing to take a chance on another one.

The only downside is I have no idea when I'll get it.  Hopefully by late spring.
```

---

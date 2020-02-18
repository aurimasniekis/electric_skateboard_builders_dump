# Question to battery builders: what&rsquo;s the best layout for this 10S3P

### Replies: 21 Views: 621

## \#1 Posted by: Maxid Posted at: 2018-10-01T08:37:23.472Z Reads: 167

```
I need to build a 10S3P battery for an E-Bike (the ESC is set to a max current of 15A which is why I went for Sanyo GA cells to get that edge in capacity). It has to fit inside a water bottle (SKS cage box) that I already bought and that other ebike builders have successfully used before. However to fit the battery inside is has to be in this configuration
![15383820610177732718146978894937|375x500](upload://95ZQ6CYW5EFwMiRCt3P7HqasK38.jpeg) 
So 10 cells per "layer" and then three of those layers stacked on top of each other.
(Please excuse the poor drawing - I am on vacation and don't have my CAD software with me :smile:) 

I know that this config is far from ideal and will be tricky - but I want to do it this way nonetheless. 
The question I am hoping to have answered by you guys is what the best layout would be.
I could do three p groups per layer and connect them in series OR I could connect three p groups vertically in series. The second option would have the benefit that you could simply fold the entire pack into its final shape and don't have to worry about strong insulation between the layers.
The last P group will also be a pita because I have to connect three stacked individual cells in parallel - but it should be doable with some creative wiring.

Another thing someone recently pointed out: is it really better to connect the cells in series first and only then do the parallel connection? So far I have always seen people do their p-groups and then connect them in series.

Well I am looking forward to your hints and ideas. Thanks a lot already.

@rojitor @Acido @TarzanHBK @mmaner @PXSS
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-01T12:47:33.581Z Reads: 137

```
I would suggest modeling this up so you can get accurate measurements, I cant even visualize this with any degree of accuracy.
```

---
## \#3 Posted by: Maxid Posted at: 2018-10-01T13:05:02.922Z Reads: 136

```
What measurements do you mean?
Width and height will not differ much between the two options and both will fit inside the bottle. It's more about what is safer and easier to spotweld.
```

---
## \#4 Posted by: mmaner Posted at: 2018-10-01T13:06:25.087Z Reads: 129

```
of the cells put together in various ways.
```

---
## \#5 Posted by: Maxid Posted at: 2018-10-01T13:07:52.620Z Reads: 124

```
The configuration has to be as shown above - my question is only about what way to connect the cells is the "better" one.
```

---
## \#6 Posted by: L3chef Posted at: 2018-10-01T13:11:32.133Z Reads: 118

```
Perhaps you could use nickel sheets instead of tabs. And some 12awg between 3 layers.
```

---
## \#7 Posted by: PXSS Posted at: 2018-10-01T13:25:51.957Z Reads: 123

```
Welcome to my job. Lol
There's two ways to do this (there are more but they all suck, trust me). The most important question is do you want pos/neg lead on the same end of the battery or do you not care. 
Its a little easier to make if leads are on opposite sides. 

Key here is that the battery has to fold into place. Tier one folds over tier 2 and tier 3 folds under tier 2. Kinda like folding a paper in three but you can't fold both sides up.  

Anyways, here is the first of the two possible layouts. I am in a rush so I'll do the second tonight. 

As you can see the positive wire doesn't come out the front face, so you'll have to use copper braid there to bring the wore out to the side of the pack. Use fishpaper sheets for insulation between tiers.

E: You can do nickel sheets cut out to shape or nickel tabs. I laid out the cells in a way that you get the widest path in the series connection. 

![image|690x412](upload://kAEXfDKmyIXt4PUlSZdhALbrVJv.jpeg)
```

---
## \#8 Posted by: Maxid Posted at: 2018-10-01T14:18:24.982Z Reads: 109

```
Wow that looks complex. Thank you for taking the time to draw this up. Having both ends on one side would be ideal however.
The one option I thought about would look like this in your drawing style:
![15384034460112620523859022917020|375x500](upload://sKA5p1RjKY9UeOVLWe7TWZky3I6.jpeg) 
With the last remaining p-group being stacked would look like this:
![15384034670975946117232113031980|375x500](upload://6WQ9fxtRBkWea9FFZdWlvKx9mCC.jpeg)
```

---
## \#9 Posted by: rojitor Posted at: 2018-10-01T14:24:36.918Z Reads: 102

```
![battery|375x500](upload://wNCRc7q6mxaPeh1vpDXNHBqzHlp.jpeg) 
i'd keep it as fast and simple as possible. 9 blocks of 3 cells parallel, then make bend series and make the last 1s3p as above. It's very simple but insulation and heat could lead to problems. the wires could also fit tight. I don't know how the bottle is. The best way is what @pxss said. He's a pro after all.
```

---
## \#10 Posted by: Maxid Posted at: 2018-10-01T14:28:20.922Z Reads: 94

```
I think your way is exactly what I pictured as well.
That at least tells me that I indeed thought of a valid way to do this - thanks a lot for the help. Will also have to try to visualize @pxss's recommendation a little better in my head to fully grasp how the cells are layed out there.
```

---
## \#11 Posted by: rojitor Posted at: 2018-10-01T14:33:31.851Z Reads: 93

```
his option is by far better. The 1s3p part could be tricky and the wires there could make it impossible to fit. Depends on the bottle. Also the insulation must be perfect. I'm lazy and he is a pro. Facts...
```

---
## \#12 Posted by: PXSS Posted at: 2018-10-01T18:44:12.677Z Reads: 93

```
The issue with both of your methods is that you cannot place the battery flat on a table to do all the welds and then fold it into shape. It is possible to make it by doing all the welds on the individual tiers and then merge them together by stacking them up while doing the welds but it's hard to handle. Its easy in terms of electrical connections but hard to manufacture. So a great design for a one of a kind battery but not if you have to make several of them which is why I didn't consider it. In my job I need to keep in mind mass manufacturing with my battery packs so that configuration didn't really cross my mind. It doesn't by any means make it a worse design!

The thing with the configuration I proposed is that you can lay down all the cells flat on a table, do all the welds on one side, stick fishpaper on, flip it over, do all the welds on the opposite side, place fishpaper on and then fold into shape. You make no welds while trying to hold things in the air and alignment is always near perfect.

Another thing about the design I did above is that the fold is along the wider and flatter side of the pack instead of on the "rounded" side. This leads to the fold being less affected by vibrations. This is also a single connection fold design. This means that there is only one electrical connection done on each fold. Doing more is possible but it gets tricky and harder to manage.

---
Another option is to make 3 individual 10S1P packs and then connect them in parallel with a wiring harness.
All three groups end up with main leads and balance connector. This is probably the easiest way to not mess up the welding since you would weld three of the same and then just connect them together. The issue with this is wiring.... You have to do a looooot of wiring. I'm talking about 30 balance leads and 6 main leads, plus you have to make the harness to connect them in parallel.

---

I'll go into details for the other configuration tonight after work.

---

Edit:
Flat layout of the design from earlier. Changed slightly to work better. 

![image|375x500](upload://tMwuhgVqfLJ1nS92mUaIM5cHsv2.jpeg) 

You do all the welds, attach some fishpaper and fold. Done
```

---
## \#13 Posted by: TarzanHBK Posted at: 2018-10-02T05:39:57.507Z Reads: 78

```
Sorry i'm late to the party.
You have to consider a few things when doing a layout.
The most important thing to me is insolation, because you dont want to short your pack because of a bad layout without the proper material in between.
Next thing is wiring. It's often easier to layout a series pack design, but the wiring to parallel is a mess and takes up a lot of space like @PXSS mentioned. 
Then there are a few layouts that looks good first, but are impossible to weld.
So in this case, i'd go for @PXSS layout. It's a bit harder to weld, but then easier to fold, good to isolate and not a wiring mess.
Just make sure it doesnt short at the aluminium bottle :metal:
```

---
## \#14 Posted by: Maxid Posted at: 2018-10-02T07:00:31.602Z Reads: 75

```
[quote="TarzanHBK, post:13, topic:69718, full:true"]
Just make sure it doesnt short at the aluminium bottle :metal:
[/quote]
It's a plastic bottle ;)
```

---
## \#15 Posted by: PXSS Posted at: 2018-10-02T10:31:00.934Z Reads: 68

```
If I were to do it your way, @Maxid and @rojitor
I would do it like this. Reason is that your fold is still along the widest side and you can still cover the entire surface with a single piece of fishpaper and then fold into place. The wires are kind of a nuisance but if you don't plan to take the pack apart, it works quite well. 

![image|666x500](upload://71Ei1dFHBmRDPwAV6I9pDACOhv8.jpeg)

E: actually. Turn that bottom middle cell back around the way you had it. There's really no reason to do it this way. I would still connect them with a wire though instead of a folded tab so you can take it apart easier.
```

---
## \#16 Posted by: PXSS Posted at: 2018-10-02T11:04:34.758Z Reads: 68

```
Last configuration. 
This one has positive and negative leads on the same side. All pads are kept quite wide. You have to run a few wires to merge some pads accross two tiers but in general a fairly good and easy to weld pack. 

Same design as before where you weld all of one side, attach fishpaper, flip, weld opposite side, attach fishpaper and fold. Wires are installed in folded position. 

![image|690x396](upload://5NHowYaUe2sy9XpIuq6RGcb9154.jpeg) 

The only real reason this pack is better than the second is the width of all series connections. In design 2 all series connections are 1 tab wide. In this design all series connections are at least 2 tabs wide. 

Don't forget solder tabs for balancing wires :slight_smile:

I'd say either of the three options is good. They all have their pros and cons but the general design idea of having a single fold along the widest and flattest area is maintained and the whole surface can be covered in fishpaper to isolate from the next group.
```

---
## \#17 Posted by: Maxid Posted at: 2018-10-05T20:06:00.370Z Reads: 54

```
To give a short heads up before I am going to do this battery on Sunday:
I am probably going to do three 10S1P packs and connect them in parallel via the main leads.

I tried all methods by connecting the cells as shown in your drawings with duct tape. The issues I found were:
1) I do not have nickel sheets but only strips - your configurations make a lot of sense but are hard to weld when only using strips. I would have to do multiple layers and criss cross the strips all the time. This does not seem ideal to me. Also this makes handling quite dangerous as once a nickel strip slips it comes into contact with other "stages" of the battery.
2) My folding pack with nine 3P packs would work but all the folds are right next to each other and the nickel will always stick out a little - this has the potential for lots of shorts as the cells need to be very close to each other in order to fit inside the bottle and I thus cannot use fish paper between them to properly insulate them.
3) I do have some space left in front and behind the widest (4 cells) part so  I should be able to hide the wires for a parallel harness there. It also sounds quite elegant when I think about it because I can check every individual cell from time to time via the parallel leads. I have some ribbon cable left that I will use as balance leads and will keep it short to not have too much wiring that needs to be stowed in the bottle.

PS: One thing I messed up already: I ordered heat shrink from nkon and chose the wrong size. I thought the dimension they give you is the diameter but they give you the width when flat - D'oh!
So I will have to use duct tape instead.
```

---
## \#18 Posted by: PXSS Posted at: 2018-10-06T10:10:50.728Z Reads: 50

```
[quote="Maxid, post:17, topic:69718"]
I would have to do multiple layers and criss cross the strips all the time.
[/quote]
Yep. There really is no way to get away from multiple strips crisscrossing. You can do it in 2 layers if you plan well. 

[quote="Maxid, post:17, topic:69718"]
Also this makes handling quite dangerous as once a nickel strip slips it comes into contact with other “stages” of the battery.
[/quote]
Magnets are your best friends for this. Small round magnets hold strips down to cells so that they dont move. After 2-3 welds the strip should go nowhere and is safe. Also fridge magnets or some kind of magnet sheet is extremely beneficial to cover up parts that you are not working on and prevent any potential short. I have also use fishpaper sheets with magnets on top if I dont have the right size magnet sheet. 

The nice thing about multiple strips is also multiple current paths but yes, it is very tedious.

---

[quote="Maxid, post:17, topic:69718"]
It also sounds quite elegant when I think about it because I can check every individual cell from time to time via the parallel leads.
[/quote]
It's not really all that useful, tbh. I've made packs like that in the past thinking that it was going to be useful to have the individual cell data and it always confimed that the parallel groups were at the same voltage. 

The real nice thing is being able to travel because the individual packs are less than 100Wh and being able to use several chargers to charge the individual packs faster. 

I like the idea of being able to add more packs in parallel to increase range without affecting the system or to be able to swap out pack if somehow one gets damaged. 

Good luck with the build!
```

---
## \#19 Posted by: Maxid Posted at: 2018-10-06T15:44:50.276Z Reads: 43

```
Do you think it would make sense to connect the balance wires of the three 10S1P packs in parallel as well (so that the cells can balance themselves) or is that unnecessary?
```

---
## \#20 Posted by: Maxid Posted at: 2018-10-08T09:53:51.014Z Reads: 38

```
![IMG-20181008-WA0001~2|436x336](upload://hPYWepWM1xG9MTjRC2DAQBfWVW2.jpeg) 
Indeed wiring was a mess - I soldered 10AWG cables to the tabs which was overkill and cost me nerves with my soldering iron.
I made them so tht pack is connected in parallel permanently as you can hardly get it out of the bottle again anyway. Thanks everyone for the help!

PS: I hope nobody saw me through the window of my workshop - this thing with red cells looks like a TNT bomb :D
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-10-09T00:46:24.810Z Reads: 27

```
Cool. Got any more pics of the construction? For SCIENCE?
```

---

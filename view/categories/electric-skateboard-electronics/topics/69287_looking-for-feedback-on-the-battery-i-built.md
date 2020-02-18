# Looking for feedback on the battery I built

### Replies: 111 Views: 1940

## \#1 Posted by: RHill051 Posted at: 2018-09-26T19:11:24.479Z Reads: 329

```
Hey, so I was a little overly anxious to get started on my build and after putting several miles on it now I'ce decided to come back and see what I can do to refine my build. I firstly wanted to get the communities thoughts on the battery I made. I'd also like feedback on the ideas I had for mounting the BMS and FOCBOX to the bottom of the board. 

First off the Battery. I didn't have a large enough shrink warp so I took two pieces and taped it together. It worked surprisingly well :smile: the second smaller wire goes to my battery meter which has an on off button so I can check the voltage without connecting the loop key. I tried to use fish paper to isolate the 2 rows of cells but realized after the fact that I have nothing between the cells in the other direction.. I've seen at least one person mention that the hot glue I used might not be sufficient at holding everything together since it can melt if the battery warms up enough I'm hoping that the balance wires will be ok in the configuration but want others opinion before all my hard work goes up in flames:
![Overview%20of%20battery|690x345](upload://jMbKw72nTwL9shw214f0SVJIuyw.jpeg) 
![Bottom%20view%20of%20battery|690x390](upload://jmUQwszAH0nVRLpeVuVBAIZs3JV.jpeg) 
![Negative%20lead|690x336](upload://racoBVv9Bp7gCkDlDkKbG4XWAiQ.jpeg) 
![Possative%20lead|690x294](upload://dCMymfWovpHOwQGhS0SobQMvDoW.jpeg) 
![Left%20side%20of%20battery|690x304](upload://9r15RC5ZrANglGploYxlHOpSbTs.jpeg) 
![Right%20side%20of%20battery|690x285](upload://eDU7gTWHqD38HRVdi7j9Z1G3zfq.jpeg) 

Here is the FOCBOX mount I designed and printed. I drew a lot of inspiration from what is available on buildkitboard.com as they offer a 3D printed mount for sale. I added space next to the FOCBOX so can use double sided tape to mount the receiver as well. I will use the rest of the empty space to mount the Bluetooth module I ordered to the plate as well most likely using more double sided tape.
![FOCBOX%20mounted%20to%20plate|402x500](upload://lC2fxcefmzkOmoJVuzNqP96EBRT.jpeg) 
![FOCBOX%20and%20plate|618x499](upload://obpmGzywFoV4MbhLEoeTRkIJgks.jpeg) 

Lastly I wanted to connect the BMS to the bottom of the board as well so I made a very simple mount specifically for the Bestech BMS. I had to swap the screws from the top of the BMS to the bottom since they were longer but I think it will work out nicely (P.S. this bms id dead because I accidentally put power through the e-switch wires :frowning:) 
![Top%20of%20BMS|631x500](upload://qh5TA5KgrhygZOyvSElhFOTVsUg.jpeg) 
![Bottom%20of%20BMS|690x448](upload://bCBNzGrHjq6avjkTrMP662FHLkJ.jpeg) 

Thanks in advance for all your input. This community has been awesome to be part of!
```

---
## \#2 Posted by: TowerCrisis Posted at: 2018-09-26T20:45:21.058Z Reads: 286

```
![Capturfdhgsgafgsfgfsgfdgfsgfsgsgfsdgfe|690x382](upload://1BpJbHSjbISfb4I1InZny5qaM31.png) 

Things like this are generally considered dangerous. If something pokes that corner and pushes either one under the insulation it has the potential to short out the P group.
```

---
## \#3 Posted by: RHill051 Posted at: 2018-09-26T21:11:49.248Z Reads: 277

```
I tried to keep an eye on that sort of thing on the possessive side of the battery, would you say its a better idea to have trimmed the corners so there is less of a chance of something like that happening?
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-09-26T21:14:37.808Z Reads: 271

```
Yes I believe the current consensus on the forums is that trimmed corners are preferable. I think that was how @deltazeta 's board went up in smoke?
```

---
## \#5 Posted by: kalebludlow Posted at: 2018-09-26T21:18:59.156Z Reads: 266

```
One thing is that the balance wires shouldn't cross over each other. Reduces the chance of them shorting each other out
```

---
## \#6 Posted by: RHill051 Posted at: 2018-09-26T21:49:40.335Z Reads: 265

```
Ok, I can remove the heat shrink and clean that up but what would be the advised way of doing so? should I just run it through channels between battery and then back up to the end via the gap between the two rows of cells?
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-09-26T22:35:02.194Z Reads: 261

```
![IMG_7676|375x500](upload://efyjs8wAQn7GechnUuI7l60m9S5.jpeg) Clean balance wires are key!
```

---
## \#8 Posted by: Sn4pz Posted at: 2018-09-26T22:37:19.365Z Reads: 254

```
looks great :O
```

---
## \#9 Posted by: RHill051 Posted at: 2018-09-26T22:45:02.444Z Reads: 249

```
oh damn... looks like I've got some work to do tonight :) lol fantastic battery!
```

---
## \#10 Posted by: luv2sk8te17 Posted at: 2018-09-27T02:04:56.931Z Reads: 247

```
What size pack is this? Do you mind sharing what it cost? I'm curious on the pricing of lipo vs li ion.
```

---
## \#11 Posted by: dareno Posted at: 2018-09-27T02:17:45.615Z Reads: 247

```
Great first build man.  One thing that is guaranteed is help with batteries on the forum.  I've probably done more research on battery  building than any other aspect and still haven't had the nerve to build from scratch.:sweat:
Have rewired a new bms though and used the gurus on here to do it right.  Still managed to cross over 2 p packs in my connector.  Bms started to heat up on its own and man theres nothing like that to make you change your undies.  It was easy to spot though because of the tidy routing and labelled packs.  I now do all my battery tinkering even just connectors etc outside on my deck with a fire extinguisher nearby.  Point is check and double check and then check again.  Mistakes are easy and there are no second chances with batteries.
```

---
## \#12 Posted by: RHill051 Posted at: 2018-09-27T03:12:51.525Z Reads: 235

```
This is a 10S3P using Samsung 30Q I bought from Nkon. I just put together this parts list and it turns out the battery cost more than I though it did lol.. but on the plus side I'm going to make back some of my money by helping a friend build their battery and he'll buy some of the parts from me. Looks like I was just under 300 but now I've got a spot welder and the knoledge and confidence to make another battery for friends :) (on a side note I went for a 4.3 mile ride the other day on my board and only used about 27% of the battery capacity!! 
![image|690x249](upload://nKhaV8O6XNXKNkfMyYbN5eJcIUm.png)

EDIT: I should mention that some of that I had to use for others parts of the build like the silicon wire and the xt90 plugs so they weren't 100% a battery expense
```

---
## \#13 Posted by: RHill051 Posted at: 2018-09-27T03:19:20.773Z Reads: 236

```
yeah, I accidently put power through the e-switch wires on my first BMS and fried it... felt like such an idiot... when I got the new one I sat down double/triple checked everything and then like an idiot totally over looked that the first balance lead was connected to the wrong spot... I was lucky that it only fried the e-switch and I am still able to use the BMS with a loop key. The fact that I'm helping a friend has made me reach out to see what I can do better for the next time and how I can improve on my first build. I just came back from pulling all the balance leads off the battery and trimming them but I'm still not happy with it.. I made the leads too short and the BMS is almost touching the battery on the one side.. I'd like another half inch of slack to allow some movement due to vibration and what-not. Either way this is what I ended up with after the first go at "improvements" I'll do it all again tomorrow and that time I think I'll take a different approach and see how it works out. 

Thanks everyone for the advice and suggestions so far!!

![15380185618811193071367796648681|666x500](upload://ycwDzkBhmTHvvlSORo1H39W9WKT.jpeg)

I trimmed a bunch of the excess wire from the leads but like I said I took too much off on some... I keep trying to use the fishpaper between the rows of cells but I feel like its a big part of why I'm having a hard time... I suspect is still probably advised that I use it unless someone has another idea. I think I'm just stuck in a rut and can only see the one solution... I like the example @ARetardedPillow shared but not entirely sure how I can replicate that. Its going to be my goal to morrow though.
```

---
## \#14 Posted by: b264 Posted at: 2018-09-27T03:31:03.576Z Reads: 217

```
[quote="ARetardedPillow, post:7, topic:69287"]
Clean balance wires are key!
[/quote]

Yes, except I wouldn't cross the balance wires over one another until after they exit the cell area, then cross them all over so they're in the correct order

Right where those cross each other will wear down due to vibration eventually making a place where a short could happen
```

---
## \#15 Posted by: b264 Posted at: 2018-09-27T03:33:13.891Z Reads: 213

```
And just to be safe I try to connect the balance wires to the negative terminals as opposed to the positive ones, because in general the positive side of the cell is more dangerous
```

---
## \#16 Posted by: RHill051 Posted at: 2018-09-27T03:44:25.765Z Reads: 208

```
Honestly that was my goal but, I failed miserably lol. Like I said I'll do better tomorrow :) I'll definitely make sure to avoid crossing any wires till i'm out of the battery
```

---
## \#17 Posted by: b264 Posted at: 2018-09-27T03:50:18.771Z Reads: 211

```
These aren't balance wires, but they were accidentally crossed for about 200 miles and they had already worn through the blue heat shrink that was against them and there was a big indent in the insulation right where they crossed.  Just because they were crossed.  It creates a pressure point.  Had I not caught this, it would have caused a failure (best case) or a fire (worst case)

![20180201_023937|690x345](upload://lM0UmugZnvLBi4zY7k1tDa2VE3i.jpeg)
```

---
## \#18 Posted by: dareno Posted at: 2018-09-27T04:22:20.132Z Reads: 209

```
[quote="b264, post:15, topic:69287"]
I try to connect the balance wires to the negative terminals
[/quote]

did not know that.  and like I said hours of research.  I probably saw it a hundred times and it didn't sink in lol
```

---
## \#19 Posted by: lrdesigns Posted at: 2018-09-27T05:00:40.349Z Reads: 210

```
This is the best ballance wire job I have seen. There still is some crossing, but can that be totally eliminated? I guess the crossing can be after the cells in the free air just before the balance plug. They are well insulated from the cells though.
![IMG-20180704-WA0018|690x388](upload://8zDUyyEHtBvXDqCPpx1J88pLijG.jpg)
```

---
## \#20 Posted by: b264 Posted at: 2018-09-27T05:04:11.161Z Reads: 213

```
That's really good-looking.  Who made that?

I would bring the wires out of the battery in the same order they happen to be in and not cross any, then cross them all in the circled area

![IMG-20180704-WA0018|690x388](upload://1YFVspXADHUskjQ5zarlSL4ahcs.jpeg)
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-09-27T05:10:49.241Z Reads: 205

```
@Eboosted, his is packs look pretty damn nice. Also @Kaly   makes nice packs but with a different approach. I keep a folder of images from the forum of nice safe packs for future reference.
```

---
## \#22 Posted by: lrdesigns Posted at: 2018-09-27T05:19:00.307Z Reads: 219

```
These scare the :poop: out of me. Its like 2mm and a small bump from :fire::fire_extinguisher::fire_engine: I hope you went in and at least fold them back at 45deg or trim them. 
![image|690x179](upload://1Z9L98LCcXb6TZ3H5E3cgIRETfU.jpeg)
```

---
## \#23 Posted by: Eboosted Posted at: 2018-09-27T06:01:49.606Z Reads: 222

```
[quote="b264, post:20, topic:69287"]
I would bring the wires out of the battery in the same order they happen to be in and not cross any
[/quote]

In this picture of the flexible batteries I make for Hs11 or Carver there is no crossing anymore :slight_smile: 

[img]https://i.imgur.com/KmCwUPY.jpg[/img]
```

---
## \#24 Posted by: baxtred Posted at: 2018-09-27T08:28:27.698Z Reads: 213

```
I'm also making a flexible battery with 30Qs. I used 3 layers of 10x0.2mm strip and bridged with 13awg wire in parallel. Designed everything to be handle 60 amps continuous without very much heat buildup. 

![20180927_022431|210x499](upload://fmmQUkXKhLAXMvnaH8Ovb2cubUV.jpeg)
```

---
## \#25 Posted by: sk8l8r Posted at: 2018-09-27T08:52:05.754Z Reads: 208

```
I have to say those battery's are looking pretty elegant :)
```

---
## \#26 Posted by: RHill051 Posted at: 2018-09-27T14:36:26.440Z Reads: 202

```
honestly I didn't even think to do anything about them yesterday but after work today I'll definitely try to just fold them back so they can't cause an issue in the future. Folding them didn't even cross my mind as an option but I greatly appreciate the idea!! Added it to the list for tonight.
```

---
## \#27 Posted by: RHill051 Posted at: 2018-09-27T14:42:57.346Z Reads: 201

```
I do have another question for others out there. As you can see with the mounts I have for the BMS and VESC I'm trying to attach everything I can to the bottom of the board. I'm a little stuck on how to do the same with the battery though. My first thought was to use some [footmen loops](https://www.amazon.com/gp/product/B07CK2Z8PL/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1) screwed to the deck that I can then loop Velcro through in order to hold the board against the bottom of the deck. I think I'll need to have a rigid support across the battery to keep it from wanting to fold but I'm wondering what others think of that approach?
```

---
## \#28 Posted by: mmaner Posted at: 2018-09-27T15:02:39.480Z Reads: 197

```
I typically use RTV or Hot Glue, in the past I have used velcro straps secured to the deck with panhead sheet metal screws then layer over that neoprene.
```

---
## \#29 Posted by: lrdesigns Posted at: 2018-09-27T15:08:21.415Z Reads: 202

```
[quote="Eboosted, post:23, topic:69287"]
In this picture of the flexible batteries I make for Hs11 or Carver there is no crossing anymore :slight_smile:
[/quote]

These balance wires are so BEAUTIFUL!! :heart_eyes:
```

---
## \#30 Posted by: luv2sk8te17 Posted at: 2018-09-27T16:23:25.463Z Reads: 200

```
Just for anyone looking for a cheaper alternative I built a 10s 5000mah lipo setup...$100...Pretty easy.They also have higher out put than li ion. Possibly lighter too since they don't have the cell casing. I will await for anyone to knock me on lipos lol...
![515ddaa630571bccacab39775957c63c668e061a_1_375x500|375x500](upload://w7BZmRrsxKWsfQijqhkW8NCezBy.jpeg) 
![90dd51f08899c10a6426057b239c4fcca3e37d61_1_666x500|666x500](upload://lvdjK3T4atd6IfrW3xvj5LJRVRK.jpeg)
don't mind the tape(temporary till i paint this thing)
```

---
## \#31 Posted by: RHill051 Posted at: 2018-09-27T17:34:25.818Z Reads: 191

```
I won't disagree that using Li-Po's would probably be easier but my battery is 9000mah and should have quite a few more charge cycles than the Li-Po equivalent. For me the added capacity and longevity of the battery were why I chose to go the rough of building my own. I like the duel motor setup you have though. I'm sure having Li-Po's works better with two motors drawing more amps.
```

---
## \#32 Posted by: luv2sk8te17 Posted at: 2018-09-27T17:40:10.848Z Reads: 185

```
Oh yeah with 9000mah you will be able to ride into the sunset....and back! Props to you for making one instead of buying premade.
```

---
## \#33 Posted by: lrdesigns Posted at: 2018-09-28T00:35:10.315Z Reads: 186

```
Hey @Eboosted a couple questions about the balance wire setup. 
1. So it does not matter the order of the cells as all the wires are positive? 
2. @b264 mentions hooking the balance wires to negative instead of positive side. Can any BMS do that? I never heard of that setup before. Seems like it could be safer with the ballance wires going over the cells.
```

---
## \#34 Posted by: b264 Posted at: 2018-09-28T00:59:19.909Z Reads: 185

```
[quote="lrdesigns, post:33, topic:69287"]
@b264 mentions hooking the balance wires to negative instead of positive side. Can any BMS do that?
[/quote]

The P groups have positive and negative connected together.  Since they're connected together, it doesn't matter where you put the balance wire -- except the first and last one

So I mean not like the grey one below, but like the three indigo ones

![wires|587x300](upload://pWmvqRqffIJXz3qawErRXBjQijt.png) 

So basically I'm saying only one balance wire ever needs to connect to the positive side of the P-pack

And since the risk of shorts is higher on the positive ends, you should not connect them there except the last one

To the BMS, there is no difference...
```

---
## \#35 Posted by: RHill051 Posted at: 2018-09-28T01:08:43.175Z Reads: 179

```
I get what you're saying but does it really matter... the wire will behave the exact same if you connect it to the positive (the purple wire in the middle) or the negative (the gray wire in the middle). What I'm really taking away from this it the idea of avoiding crossing wires.
```

---
## \#36 Posted by: b264 Posted at: 2018-09-28T01:10:56.225Z Reads: 172

```
I'm saying under heavy vibration and flexing it's better to have more stuff physically further away from the positive end of the cells.  If it's the same electrically, then there is no reason to put it on the positive end.  That's all I'm saying.  It's more risk with no extra reward.
```

---
## \#37 Posted by: Eboosted Posted at: 2018-09-28T01:30:25.211Z Reads: 167

```
The order of the BMS wires does matter, if you make a mistake you will cause a short as soon as the BMS is plugged
```

---
## \#38 Posted by: lrdesigns Posted at: 2018-09-28T01:35:31.404Z Reads: 174

```
So having non crossing ballance wires only works with that battery layout, and not the boosted board style double stack? I guess they can still cross AFTER the cells before the balance plug where there should be more free space.
```

---
## \#39 Posted by: RHill051 Posted at: 2018-09-28T03:11:18.663Z Reads: 180

```
Well I am very happy with the changes I made. I still have fish paper between the cells it wraps underneath and is trimmed to match the profile of the cells none of the balance wires crossed until after they exit the pack everything is it is taped in fixed in place I'm just going to go back now and trim the corners of those nickel strips on the positive leads and I think I should be golden unless there's any further suggestions.![IMG_20180927_221001|690x357](upload://AjQ02UGs21VrnDmgL6ImY9VdFlk.jpeg) ![IMG_20180927_221012|690x430](upload://h0on1tlzgJdHc9ZrqfyHxxm7KTe.jpeg)
```

---
## \#40 Posted by: RHill051 Posted at: 2018-09-28T03:35:00.088Z Reads: 173

```
I tried to curl those edges and not sure if it got better or worse at least it's not protruding over the edge.![IMG_20180927_223421|690x315](upload://sfOIUF1wlXhqKkuh8DeMhuhoxaD.jpeg)
```

---
## \#41 Posted by: b264 Posted at: 2018-09-28T03:35:49.956Z Reads: 171

```
[quote="Eboosted, post:37, topic:69287"]
The order of the BMS wires does matter
[/quote]

You're missing the entire point of what I'm saying, look at the image
```

---
## \#42 Posted by: Eboosted Posted at: 2018-09-28T05:05:31.471Z Reads: 169

```
@b264 I reread what you explained, I missed your point and understood @lrdesigns question incorrectly, sorry about that.

Positive and negative balance wire tapping is exactly the same, physically is much better to tap it on the negative as the wire won't flex or vibrate and addition inch and between the p-groups.
```

---
## \#43 Posted by: RHill051 Posted at: 2018-09-29T16:57:37.324Z Reads: 169

```
Well I was really proud of the "improvements" I made the last few days. And was going to show my brother the board... Rode it maybe 100 yards and it stopped... Upon inspection I found this... I thought I was safe b cause it was not running over the BMS but it seems it shorted out on either the screw holding the BMS to the board or the screw on the board itself... When I plug it in it doesn't show power on the FOCBOX anymore... Though the receiver has power... I am guessing I killed another BMS... What should I have done differently to avoid this for next time?![IMG_20180929_115311|666x500](upload://aGKcGj3zOTy1fX0DjlIxsSM1HpG.jpeg) ![IMG_20180929_115255|666x500](upload://ijyQET2QR9MYe7APSgCQp1emlbD.jpeg)
```

---
## \#44 Posted by: trancejunkiexxl Posted at: 2018-09-29T17:01:46.017Z Reads: 166

```
Looks great! 😁
```

---
## \#45 Posted by: RHill051 Posted at: 2018-09-29T17:22:07.272Z Reads: 160

```
You sure? I know there's got to be something I can do to prevent a short like I just had... Im thinking I might change the brackets I mad so they have a protective wall that goes over that screw on the top..
 That will prevent another short. I'm also thinking of making some sort of channel I can run the wires in so they don't rub on anything
```

---
## \#46 Posted by: RHill051 Posted at: 2018-09-29T18:20:15.301Z Reads: 158

```
@mmaner and @b264  what do you guys think?  I just hooked a multimeter to the BMS and that actually seems to be working fine, there's 41V at the FOCBOX and the receiver comes on but I got nothing. Any suggestions?
```

---
## \#47 Posted by: mmaner Posted at: 2018-09-29T18:56:46.667Z Reads: 155

```
What lights are on at the FocBox?
```

---
## \#48 Posted by: RHill051 Posted at: 2018-09-29T19:02:54.970Z Reads: 154

```
None... However the receiver lights up when I turn on the board using the loop key
```

---
## \#49 Posted by: Friskies Posted at: 2018-09-29T19:41:06.549Z Reads: 152

```
Check with a multimeter?
```

---
## \#50 Posted by: mmaner Posted at: 2018-09-29T19:49:49.397Z Reads: 156

```
Are you getting a connection in the software?
```

---
## \#51 Posted by: RHill051 Posted at: 2018-09-29T19:57:15.097Z Reads: 152

```
I'll have to probably wait till this evening to see if I get a connection in the software sine I'm at my brother's house. Unless he has a laptop I can use. But basically I was riding and it just stopped abruptly essentially power cut out came to stop took the cover off everything looked fine so I disconnected the loop key reconnected it and the motor worked again but as I was putting the cover back on I heard a spark which is when I found the where in the shrink wrap on the positive of the battery which I assumed shorted out on the screw that goes into the wood of the board since then I have not noticed any lights on the speed control aside from power to the receiver. I was really hoping someone else had experienced something similar and had an idea that wouldn't require a ton of troubleshooting. I'm just disappointed I can't show my brother the board after all the hard work I put into it.
```

---
## \#52 Posted by: RHill051 Posted at: 2018-09-29T20:05:24.959Z Reads: 147

```
I did check and there was 41v at the FOCBOX bit light still didn't come on
```

---
## \#53 Posted by: RHill051 Posted at: 2018-09-29T22:30:59.718Z Reads: 148

```
All right I connected the vasque to the computer but the computer does not recognize it. The receiver still turns on and shows the blue power light but no lights display on the vesc.![15382602206112995196384911631668|375x500](upload://lOjKBZkV7NqLGX6M0SvpJT6Ivpt.jpeg)
```

---
## \#54 Posted by: RHill051 Posted at: 2018-09-29T23:19:47.781Z Reads: 144

```
So to help provide as much info as possible I want to mention that when shortening the wire under the board I shorted the wires on both the FOCBOX and the motor since they were really long. I was told that wire length can have an impact on this scenario. Wondering if you guys would agree.
```

---
## \#55 Posted by: Sn4pz Posted at: 2018-09-29T23:23:23.242Z Reads: 140

```
[quote="RHill051, post:54, topic:69287"]
I shorted the wires on both the FOCBOX and the motor since they were really long
[/quote]

see any magic smoke come out?
```

---
## \#56 Posted by: RHill051 Posted at: 2018-09-29T23:26:33.238Z Reads: 138

```
No, no smoke, nothing when I get home I'll take the cover off the VESC not that I'll really know what I'm looking for. But if it helps get to the bottom of this
```

---
## \#57 Posted by: Sn4pz Posted at: 2018-09-29T23:28:09.523Z Reads: 140

```
some people here know what to look for here and are willing to help, so just upload it whenever and we can help ya :)
```

---
## \#58 Posted by: lrdesigns Posted at: 2018-09-30T01:06:47.865Z Reads: 142

```
[quote="RHill051, post:43, topic:69287"]
What should I have done differently to avoid this for next time?
[/quote]

Cover any exposed contact and any sharp edge of the BMS that could wear down an insulation with fish paper or some other abrasion resistant material.
```

---
## \#59 Posted by: RHill051 Posted at: 2018-09-30T02:59:33.776Z Reads: 144

```
okay, I've taken a few pictures of the fox box but nothing looks right to me... Anyone know where I could check voltages on the vest to see what actually went bad? I'm no electrical engineer but I'd be curious if it's possible to isolate the bad component and replace it.![IMG_20180929_214516|666x500](upload://tuJXTlWBJ6zyeJ8tqJy7JKiyFzg.jpeg) ![IMG_20180929_214745|666x500](upload://y4X9NYMHSP5JUHvQjRhVWrwyXaZ.jpeg)
```

---
## \#60 Posted by: RHill051 Posted at: 2018-09-30T19:54:51.542Z Reads: 138

```
Ok so I got a suggestion from @JohnnyMeduse to follow this [thread](https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/7) which I think has confirmed the u401 can bus is bad.. I've done a little research on replacing it but still have a few questions.

1. Are all vp232 can bus chips the same? or should I be looking for a specific one?
2. I saw someone say that the chip will fry if the wires touch when soldering. Do you agree that it would ruin the chip is the ends touch while soldering?
3. While looking at the board I noticed one of the caps are missing from the r6 spot on the board ( you can see it in the first picture above in the very bottom right corner next to the micro usb port) does this matter?

Thanks for all your help guys!! As frustrating as this is I feel like I'm still learning and getting better!!! I'm also considerably less frustrated at the moment since it seems I have the chance to possibly fix the board vs buying a whole new one
```

---
## \#61 Posted by: RHill051 Posted at: 2018-10-01T00:37:38.999Z Reads: 130

```
Correction its not the u401 component but the MCU or U1 component... considerably more difficult to replace lol but might still give it a try and see if I can fix it
```

---
## \#62 Posted by: lrdesigns Posted at: 2018-10-03T03:55:11.917Z Reads: 126

```
Visually there is no sign of :boom:. Are you 100% sure its the esc? Did you try to bypass the BMS and see if it works. Or trying a different esc with the BMS connected? 

If you don't have any extra esc's to test, maybe one of the other forum members could help you out if they live close. Share what city you live in to see if anyone is close by.
```

---
## \#63 Posted by: RHill051 Posted at: 2018-10-03T04:04:26.386Z Reads: 134

```
I did check to see if I'm getting the correct voltage after the BMS and that looked like it was good. Based on the fact that the positive lead of the battery shorted out on one of these two screws 
![Untitled|666x500](upload://vrnZ1G8Y6gOOLBQB69uQmFtqfRH.jpeg)  
@JohnnyMeduse (who was recommended to me by a few others on the forum as one of the most knowledgeable people when it comes to troubleshooting a VESC) said it was most likely the MCU on the VESC. I spent a lot of time today researching how to replace that chip as its pretty small and had a ton of pins on it. I've got a replacement coming tomorrow and the bad one is already been desoldered. 
![IMG_20181002_171442|375x500](upload://l7EaEEHJtVq2S7r5xfUXrVWG9FC.jpeg)
```

---
## \#64 Posted by: lrdesigns Posted at: 2018-10-03T04:08:23.867Z Reads: 132

```
Well good luck on the repair. I tried to replace a DRV once but just ended up desoldering a bunch of other components. lol. 

This area in blue also looks like a good way to cut the wire insulation.
![image|690x436](upload://zlUKIuepHy7Q0VzQm7qktQdJegf.jpeg) 

Maybe a 3D printed cover for the BMS would be a good idea. I do like your printed mounting brackets, very neat.
```

---
## \#65 Posted by: Eboosted Posted at: 2018-10-03T06:13:45.975Z Reads: 124

```
Get two focboxes so you don't have to wait weeks when they go bad, when the build is reliable sell the focboxes you still have in stock.

Please post your VESC current limits here, you might have killed the controller with wrong settings and might kill a second one if you keep the same settings
```

---
## \#66 Posted by: RHill051 Posted at: 2018-10-03T13:25:07.350Z Reads: 116

```
[quote="lrdesigns, post:64, topic:69287"]
This area in blue also looks like a good way to cut the wire insulation.
[/quote]

I agree :) if I've got time today I was going to try to design and print some cable management stuff. I'll be sure to share the end result :) If anyone is interested in the other parts I printed just let me know.

edit: Also regarding your attempt to desolder the chip, I ended up using the kapton tape to mask off the rest of the board and then took my high temp heat gun and a slowly warmed up the chip and solder. I used a temp gun to try to gauge when it was warm enough and not too hot. If you look closely you can see that 2 of the micro caps shifted a little but they are still making good contact so I should be good. now I'm just worried about the soldering part. hopefully with enough flux that will go well haha. Also I really melted the plastic plug on the back side of the vesc... luckily I have some extras getting delivered today. I'm under the impression I have to flash the new MCU chip so I plan to follow this thread: [VESC Boot Loader Installation Tutorial](https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103) to do that. If that is not the correct thing to do please let me know.
```

---
## \#67 Posted by: RHill051 Posted at: 2018-10-03T13:26:45.245Z Reads: 116

```
[quote="Eboosted, post:65, topic:69287"]
Please post your VESC current limits here, you might have killed the controller with wrong settings and might kill a second one if you keep the same settings
[/quote]

I don't think it was the current limits. I was working with @mmaner to get those right. I had the max motor and batter current set to 60A. Before I do anything though I'll be sure to share what I have in the tool so I don't accidently overlook something.
```

---
## \#68 Posted by: RHill051 Posted at: 2018-10-03T20:41:49.191Z Reads: 111

```
Quick question. Any of you have an extra 7 pin socket? I melted the one on my vesc by accident when removing the bad MCU. I've got some extra 6 pin sockets but not the 7 pin ☹️![15385992748816200624888862841552|375x500](upload://xvEhEO7lHeXXowf7d58QuyVxiUG.jpeg)
```

---
## \#69 Posted by: RHill051 Posted at: 2018-10-09T14:22:22.836Z Reads: 101

```
Hey guys, So I got a new MCU soldered onto the board, just now finally managed to get the correct firmware flashed to it and I think I'm ready to start inputting setting for the build. Last time I was running the board sensorless in BLDC mode. But I was hoping someone would be willing to help guide me through a hybrid setup where its FOC mode in low eRPM and BLDC in high eRPM. To help get the ball rolling here is my build.

BKB 6374 190KV 3200w motor
Bestech BMS
Enertion FOCBOX
10S3P Samsung 30Q Li-Ion battery

Any advice is greatly appreciated. I'm not sure exactly how to enable the "hybrid" mode I've heard about.
```

---
## \#70 Posted by: Sn4pz Posted at: 2018-10-09T15:24:01.395Z Reads: 91

```
not to shoot you out of the sky, but you should probably just set it up in BLDC first and see if the focbox responds well to it :man_shrugging:
```

---
## \#71 Posted by: RHill051 Posted at: 2018-10-09T15:25:17.820Z Reads: 90

```
thats a good idea :slight_smile: I'll do that now and let you know how it goes (not sure if it will stop raining today but if it does I'm dying to get out and ride again!)
```

---
## \#72 Posted by: Sn4pz Posted at: 2018-10-09T15:26:26.803Z Reads: 93

```
before you disconnect the focbox why not take some screenshots of the values that you have? Maybe thats what caused the initial issue? 4.xx hardware is pretty finicky... or so ive heard :laughing::sweat_smile:
```

---
## \#73 Posted by: RHill051 Posted at: 2018-10-09T15:27:57.771Z Reads: 91

```
I can do that, I was running 60A for the motor and battery max, -30A max break and -40A max recharge anyone think that would be a problem?
```

---
## \#74 Posted by: Sn4pz Posted at: 2018-10-09T15:30:11.141Z Reads: 95

```
well 60a is kinda high for even a focbox with no cooling solutions... So be careful of that on your ride. 

Whatever you do dont full throttle unloaded motors, thats a pretty common vesc killer

I mean if you need 60a, then you need 60a and I cant tell you to go lower... but maybe 50 is a nice compromise? Battery and Vesc wise
```

---
## \#75 Posted by: Sn4pz Posted at: 2018-10-09T15:31:56.478Z Reads: 95

```
wait 40a max recharge? this sounds funny to me ( at least for a 3p battery?) 


... I havnt opened bldc tool in months :sweat_smile:

![image|521x155](upload://epDZtx2Uv5rEl0qlida8OvaVJIe.png) 

like this?
```

---
## \#76 Posted by: RHill051 Posted at: 2018-10-09T15:48:18.432Z Reads: 92

```
well I'll try those settings. However when I get the the motor detect step I hit "Start Detection" but liturally nothing happens, no entries in the log, no messages about success or failure... is there something else wrong with the FOCBOX?
```

---
## \#77 Posted by: Sn4pz Posted at: 2018-10-09T15:55:56.737Z Reads: 90

```
weird.....


char
```

---
## \#78 Posted by: RHill051 Posted at: 2018-10-09T15:56:09.910Z Reads: 88

```
P.S. the battery voltage is 40.9V so no early cutoff interference.
```

---
## \#79 Posted by: RHill051 Posted at: 2018-10-09T16:22:00.275Z Reads: 86

```
Another odd thing is when trying to set up the remote, it doesn't look like the vesc is getting any feedback from the remote/receiver. The real time data doesn't change at all. Something else I'm noticing is the VESC will disconnect from the computer after a few minutes. Is there something else on the board that I should look at to try to see if there is another damaged component to replace?
```

---
## \#80 Posted by: Sn4pz Posted at: 2018-10-09T16:24:55.589Z Reads: 87

```
maybe add some pics of the mcu now that its back on?

I mean if its reasonably priced, might as well replace the drv yourself if you can too. Some DRVs fail without external damage

*not that this would impact your remote function at all
```

---
## \#81 Posted by: RHill051 Posted at: 2018-10-09T16:27:30.136Z Reads: 91

```
[quote="Sn4pz, post:80, topic:69287"]
maybe add some pics of the mcu now that its back on?
[/quote]

Sure thing :) here is the chip soldered back into place. I went through with my multimeter and verified there are no bridges between any of the pins.
![IMG_20181009_082347|375x500](upload://oQabxFmhHbmF3X3vPGB2hanMd0c.jpeg) 

In regards to the DRV, any chance you could point me in the direction of which chip that is on the FOCBOX? I've been trying to find some write up that explains which one it is so could do some more research on it but I'm totally stumped.
```

---
## \#82 Posted by: Sn4pz Posted at: 2018-10-09T16:28:31.985Z Reads: 92

```
absolutely! you must have been using the wrong keywords to search :) 

let me edit this with some topics
not in any order....: 
https://www.electric-skateboard.builders/t/focbox-drv8302-error/53288

https://www.electric-skateboard.builders/search?q=DRV%20focbox

![Inkedyarrrr_LI|666x500](upload://mQ070TVfCP4kO83gLLbnMOVxnZK.jpeg)
```

---
## \#83 Posted by: RHill051 Posted at: 2018-10-09T17:05:16.007Z Reads: 85

```
well it looks like I can get the chip for around 6-12 buck (depending on what they charge for shipping) but my I'm curious if its worth replacing more and more parts... at what point is it no longer worth trying to fix? I have a lot more confidence in my ability to replace the DRV chip after doing the MCU but will this fix my issues?
```

---
## \#84 Posted by: Sn4pz Posted at: 2018-10-09T17:08:55.121Z Reads: 84

```
Ive got no evidence to say that the drv is whats causing the focbox to act oddly

It could be that there was a short of something else as a result of the MCU going out, unfortunately thats where my knowledge stops.... so I summon the almighty wizard :laughing: @JohnnyMeduse
```

---
## \#85 Posted by: RHill051 Posted at: 2018-10-09T17:15:58.136Z Reads: 82

```
oh man, JohnnyMeduse probably hates me by now, I sent him like 10 messages late last night in our private chat while I was trying to figure out why I couldn't update the firmware. In reality I still can't update the firmware using the BLDC tool but I was able to flash the correct firmware onto the chip using the ST Link v2 so the BLDC tool stops bugging me about it. Whatever was preventing the firmware update is also likely causing the issues I'm currently having. I just don't know how to troubleshoot what might be the point of failure now. 

Sorry you're getting pulled into this again JohnnyMeduse... I was trying to give you a break but your reputation is obviously too powerful to keep your name from coming up haha
```

---
## \#86 Posted by: Sn4pz Posted at: 2018-10-09T17:32:31.842Z Reads: 82

```
@CarlCollins is also the man, AND a focbox master :) 

could probably ask him? :P 

sorry to throw names out everyone <3
```

---
## \#87 Posted by: Sn4pz Posted at: 2018-10-09T17:36:11.200Z Reads: 85

```
![image|666x500](upload://pRiUEFaMTihd7xNWHWBt2Nx3bX3.jpeg) 

is that chip in-between the caps still looking.... melted? on your focbox?
```

---
## \#88 Posted by: RHill051 Posted at: 2018-10-09T17:36:18.155Z Reads: 85

```
The only name I've heard is JonnyMeduse so its nice to learn of others who are more knowledgeable than I am. To anyone out there who has an idea of whats going on with my FOCBOX I am really appreciative of the assistance. All I want lately is to get this thing working again so i can go ride.. week and a half that I had to ride it was so addicting!! I just want more of it lol
```

---
## \#89 Posted by: RHill051 Posted at: 2018-10-09T17:38:49.657Z Reads: 82

```
[quote="Sn4pz, post:87, topic:69287, full:true"]
is that chip in-between the caps still looking… melted? on your focbox?
[/quote]

not sure which one you are talking about
```

---
## \#90 Posted by: Sn4pz Posted at: 2018-10-09T17:45:09.076Z Reads: 80

```
![yarrrr|666x500](upload://phryqJQBJ0Vk3YG73DlLHYoAuQ7.jpeg)

sorry for poor drawing :D
```

---
## \#91 Posted by: RHill051 Posted at: 2018-10-09T18:20:12.629Z Reads: 83

```
no, that was just some of the silicon used on the capacitors. I did however notice something off, but not sure if its enough to cause the issues I'm seeing.
![IMG_20181009_130107|666x500](upload://yDrJhmLnaT91P91ggyC0WvsQlcG.jpeg) ![IMG_20181009_131442|375x500](upload://AgGBfLwuE1xTtFAZGPhFKPCjEiH.jpeg) ![IMG_20181009_131500|375x500](upload://2S0GzvhiXPHvMHq5veU7UVRRZIJ.jpeg) ![IMG_20181009_131203|375x500](upload://uxp7WJZTMD2q7Qv1wppUD9VRX2X.jpeg)
```

---
## \#92 Posted by: Sn4pz Posted at: 2018-10-09T18:38:56.050Z Reads: 79

```
! looks like it could be a good piece to fix!
```

---
## \#93 Posted by: RHill051 Posted at: 2018-10-09T18:56:19.169Z Reads: 80

```
[quote="Sn4pz, post:92, topic:69287, full:true"]
! looks like it could be a good piece to fix!
[/quote]

ok that chip has been fixed, going to let the board cool down and then I'll try it again. (I'm really new to re-flowing so I want to share what I did in case I should have done it a different way) I don't have an SMB station so what I've been doing to re-flow or solder is to mask off parts of the board using kapton tap and then slowly heat up the chip using my heat gun. (I think that's how this one chip was moved.. as the solder melted the tape pulled it up) so that's all I just did was heat it up slowly till the chip settled back down and the let it cool off.. not sure if I should have added flux or not but I'm open to advice for more experienced and knowledgeable people.
```

---
## \#94 Posted by: RHill051 Posted at: 2018-10-09T19:05:42.262Z Reads: 81

```
Ok tried to run the motor detect and it still does nothing :frowning:... I'll keep scouring the forum but if anyone has an idea whats going on I'm starting to get desperate lol
```

---
## \#95 Posted by: CarlCollins Posted at: 2018-10-09T21:22:36.164Z Reads: 74

```
@RHill051
Can you let us know which firmware version you flashed to the FOCBOX using ST-Link?
```

---
## \#96 Posted by: RHill051 Posted at: 2018-10-09T21:47:49.408Z Reads: 76

```
[quote="CarlCollins, post:95, topic:69287"]
Can you let us know which firmware version you flashed to the FOCBOX using ST-Link?
[/quote]

Sure, I flashed the "VESC_default.bin" found here https://github.com/Ackmaniac/vesc_tool/tree/master/res/firmwares/410_o_411_o_412 after trying to figure out what firmware to the tool was trying to flash.  Here are my steps. It would be awesome if I just need to flash a different firmware with the ST Link :slight_smile:
![image|175x500](upload://ipWhQVzD5VpdEjCVuQtAfl5vETc.png)
```

---
## \#97 Posted by: CarlCollins Posted at: 2018-10-09T21:55:18.239Z Reads: 75

```
@RHill051
**Do the following**
Use ST-Link to downgrade the firmware to 2.18 (Default of FOCBOX)
**2.18 Firmware for Hardware Version 4.10, 4.11 & 4.12: https://we.tl/t-c5ypVXS4JG (Enertion one)**
and use this tool to program it: 
**MAC Version of Enertion's BLDC tool: https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-mac/**
**Windows Version of Enertion's BLDC tool: https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/**

Then switch back to the latest firmware using USB flashing.

_I have faced this issue several times and only problem is with the ACK version of Firmware when flashed via ST-Link_

Let us know if this works for you :slight_smile:

**I would also love to assist you via Team Viewer if you face any difficulties**
```

---
## \#98 Posted by: RHill051 Posted at: 2018-10-09T22:24:30.455Z Reads: 69

```
Ok so flashing with ST Link is done. Connected to BLDC Tool and was able to read firmware no problem. I'm not sure exactly how to update the firmware from here though. (sorry I don't have team viewer, I've used google hangouts to share desktop in the past)![image|690x282](upload://uLmmfAs92D15IclMXTViGo2AE84.png)
```

---
## \#99 Posted by: CarlCollins Posted at: 2018-10-09T22:31:40.938Z Reads: 70

```
@RHill051
Now you have 2 options
You can configure it using BLDC tool and give your setup a go 
Or you can connect it to VESC tool and flash it using normal USB flashing procedure
```

---
## \#100 Posted by: RHill051 Posted at: 2018-10-09T22:35:31.280Z Reads: 67

```
Are you saying to keep the FOCBOX on 2.18 and setup using BLDC tool? vs
connecting to Acmaniac tool and upgrading firmware by USB? It sounds like you are referring to a 3rd tool that I haven't heard or when you say VESC tool. Even on version 2.18 using BLDC the FOCBOX disconnected after a few minutes and needs to be power cycled in order to connect to the computer by USB again...
```

---
## \#101 Posted by: CarlCollins Posted at: 2018-10-09T22:39:53.134Z Reads: 69

```
@RHill051
Let me clarify 
By default, FOCBOX comes with 2.18 FW which works with BLDC Tool only. 
You flashed it to FW 3.1 to make it work with VESC tool Ackmaniac Version
You used this link: https://github.com/Ackmaniac/vesc_tool/tree/master/res/firmwares/410_o_411_o_412

So all I am saying is 
You can program your FOCBOX by staying at the stock firmware and using BLDC tool
Or you can flash that Achmaniac firmware again on it to make it work with VESC tool
The choice is yours.

For that disconnection, Let me know the length of your MicroUSB wire
```

---
## \#102 Posted by: RHill051 Posted at: 2018-10-09T22:44:02.719Z Reads: 68

```
So I decided to try to input some of the settings using BLDC just to see if I get some different results and it looks like when I click on "Start Detection" the motor actually spins up however it does not print any results to the adjacent window. Any advice on how to get the detect to work? btw **HUGE** thanks for helping out!! I honestly thought I was never going to see progress lol
```

---
## \#103 Posted by: CarlCollins Posted at: 2018-10-09T22:46:10.216Z Reads: 69

```
If you are on Windows or MAC, Please download team viewer on your PC/Machine (Don't worry it's free)
And Inbox me your ID and password.
I would love to check it myself :slight_smile:
```

---
## \#104 Posted by: RHill051 Posted at: 2018-10-09T22:47:19.523Z Reads: 65

```
ok I'm on it give me a min or two
```

---
## \#105 Posted by: CarlCollins Posted at: 2018-10-09T22:47:44.837Z Reads: 64

```
Take your time
```

---
## \#106 Posted by: CarlCollins Posted at: 2018-10-09T23:52:29.865Z Reads: 64

```
Problemo Solved :slight_smile:
```

---
## \#107 Posted by: lrdesigns Posted at: 2018-10-10T01:55:45.423Z Reads: 66

```
Cool! So what was the problem exactly and how to fix it? The FOCBOX is now in working order?
```

---
## \#108 Posted by: RHill051 Posted at: 2018-10-10T13:24:16.912Z Reads: 71

```
[quote="lrdesigns, post:107, topic:69287, full:true"]
Cool! So what was the problem exactly and how to fix it? The FOCBOX is now in working order?
[/quote]
Ok, So first I want to give a huge thanks to @CarlCollins!! The man is awesome!! He took the time to screen share with me and identify what the issues were. I know that a huge part of my problems were coming from the fact that I did not have the correct drivers on my computer to communicate with the FOCBOC and that was causing it to disconnect after a few minutes. I also speculate that it was part of the reason I was unable to write anything to the focbox over USB. Second we tried using a shorter cable. (or maybe just a different cable in general because the one that ended up working was probably 4 foot instead of 5 foot in length). Next I think following these steps also helped get things going in the right direction again. Without haveing tested just the USB scenario I don't know if I would have had to do this or not but these are the steps followed and it worked for Carl and I. 
[quote="CarlCollins, post:97, topic:69287"]
**Do the following**
Use ST-Link to downgrade the firmware to 2.18 (Default of FOCBOX)
**2.18 Firmware for Hardware Version 4.10, 4.11 &amp; 4.12: https://we.tl/t-c5ypVXS4JG (Enertion one)**
and use this tool to program it:
**MAC Version of Enertion’s BLDC tool: https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-mac/**
**Windows Version of Enertion’s BLDC tool: https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/**
[/quote]
I was having some issues with the motor detect process and Carl did something to get that to work but I totally missed it since he was working pretty fast. @CarlCollins could you elaborate on what you did to get the motor detect to work? 

P.S. In case someone else is having issues I would advice you to take caution when trying to flash numerous times using ST Link. According to Carl that can burn up the DRV chip if done several times in a short period of time. I think he said something like 15 times in a 10-20 min time period would be dangerous (lucky I didn't fry the chip 2 nights ago haha) I'd be happy to elaborate more on a specific area if it would help someone so please don't hesitat to ask. But for now remote is connected and the motor responds as you would expect.

I guess that means at some point soon I'll have to start figuring out how to set up the board for the "hybrid" configuration using FOC at low eRPM and DLBC at high eRPM like how @mmaner has mentioned he uses. But in the mean time I still haven't been able to go tide the board because of the rain we've been getting. I've never hated the weather as much as I have since I got my board working a couple weeks ago hahaha
```

---
## \#109 Posted by: CarlCollins Posted at: 2018-10-10T19:53:04.145Z Reads: 63

```
@RHill051
Thank you so much man! Glad to help
For the motor configuration part, I've done the following
I reduced Motor Max to 50A from 60A
Reduced Batt Max from 60A to 30A and Batt Min to -12 from -60

selected the motor type to BLDC and perform detection.
After that, I adjusted the Pulse of Remote as per the remote type>

I hope this helps
```

---
## \#110 Posted by: Sn4pz Posted at: 2018-10-13T00:34:38.591Z Reads: 55

```
i know you said the issue was solved, but if anyone else has this issue, heres another thread sort of like it?

https://www.electric-skateboard.builders/t/focbox-did-i-kill-both-in-1ms-help/41761
```

---
## \#111 Posted by: RHill051 Posted at: 2018-10-13T01:51:01.513Z Reads: 56

```
So technically the board works (sort of)¹ but I was trying to update the firmware using both the Ackmaniac tool and the VESC tool but it fails to flash... I created another thread https://www.electric-skateboard.builders/t/trouble-flashing-updated-firmware-on-focbox/71011 to try and get some more advice on how to get the firmware updated. 

¹ So I was riding the board this evening and all of a sudden the motor cut out... It didn't completely die, it was moving really slowly but then after a few seconds it came back to normal. Not sure what was going on. I'm afraid to try riding again lol
```

---

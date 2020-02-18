# Nickel Strip becoming work hardened by vibration, and breaking

### Replies: 43 Views: 1425

## \#1 Posted by: slade Posted at: 2019-01-27T00:04:02.633Z Reads: 249

```
So I finished my first build a few weeks ago, and up until now it was running like a dream! Unfortunately I begin to have connection issues, where the voltage would drop to basically nothing in certain orientations. I was expecting broken solder but when I opened it up I found broken nickel strips. 

I had some u shaped nickel strips to bridge the junctions of some of the batteries like this:
![20190126_155650|281x500](upload://35krgqckEoohFdmWoX1AAq94tTs.jpeg) 

While the solder joints connecting them to the strips on the batteries are fine, they are broke at the U bend, most likely from all the micro vibrations ever so slightly bending them, work hardening them, and making them brittle like a paperclip would if you bent it back and forth enough. I see signs of this same wear on a few others as well.

I'm not sure what the best way to fix this is, because if I just put a different U shaped strip in there I think there's a good chance it'll just happen again in a month or so. Any advice or ideas?

Cheers!
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-01-27T00:31:51.437Z Reads: 233

```
Lots of conductive materials will work harden (copper/nickel/aluminum...) after stress so the best thing is to use lots of thinner pieces like braided flat wire...if you're hurting for space then you can connect the batteries to plates and mount the plates at one point to the deck to prevent the batteries bending

What does the entire pack look like?
```

---
## \#3 Posted by: slade Posted at: 2019-01-27T00:50:07.363Z Reads: 230

```
Hmm.. That's an interesting idea with the flat braided wire!! You think if I jam some strips of that in there are fill it with solder, the capillary action will suck it all up and create a solid connection with the terminals/strips? 

Here's a shot of the entire pack:
![20181029_225155|690x388](upload://t87WUdZCPg8tHSpGnJg2KCM461V.jpeg)
Since taking this photo, I've swapped out the BMS on top with a thinner one that can handle more amperage (30A). Only using a 4A charger with this.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-01-27T00:58:18.601Z Reads: 220

```
hmm, only one layer of nickle?
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-01-27T01:04:12.147Z Reads: 216

```
I've been told soldering directly to the battery usually doesn't work, but you might be able to get copper braid to stick to nickel strip, if you tin the nickel and copper first it should work a bit better
```

---
## \#6 Posted by: slade Posted at: 2019-01-27T01:10:15.575Z Reads: 211

```
There are two U bridges of nickel between each of the junctions in the middle of the pack. Are you suggesting that I add another layer of strips across all junctions? My max amperage output currently is 60A, and unless I drastically change my setup, I don't see that ever increasing.
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-01-27T01:11:57.864Z Reads: 214

```
those are 0.15x 8mm strips right?, people usually do 2 on parlell (just to be safe) and 3 on series. each strip can handle around 8 amps i believe
```

---
## \#8 Posted by: b264 Posted at: 2019-01-27T01:41:15.906Z Reads: 209

```
Soldering directly to the cell most definitely does work, but it's not recommended because it's nigh impossible to do that without getting the cell too hot and degrading it.

Soldering to nickel that's right next to the cell is much better but you still need to beware of putting heat into the cells, and be quick about it.
```

---
## \#9 Posted by: ZachTetra Posted at: 2019-01-27T01:41:56.503Z Reads: 202

```
How do you connect to an 18650 w/o a spot welder?
```

---
## \#10 Posted by: b264 Posted at: 2019-01-27T02:27:37.650Z Reads: 196

```
Well you can solder directly to the cell, ***but it's not recommended at all*** and even if you did, you'd have to have solder skills

This cell is soldered

![20171227_031414%20(another%20copy)|690x345](upload://xthO8N98q91xTGY2oMGJaVGzEL6.jpeg)
```

---
## \#11 Posted by: b264 Posted at: 2019-01-27T02:36:07.521Z Reads: 196

```
Disclaimer: NOT RECOMMENDED to solder to the cells.  This was done with a super-hot high-quality iron, with 30 years of soldering experience, and I had a piece of aluminum handy so the cell had an iron on it for about 1 second, then a piece of cold aluminum pressed against it, sucking the heat off the endcap before it traveled into the cell.  Without shorting the cell out, of course.  And it probably still damaged the cell a little bit.
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-01-27T02:51:12.720Z Reads: 190

```
you know that spot welding the same spot 6 times in a row will cause the cell to heat up a lot too right? (not by a shit tone though)

52c on the same spot for spot welding
212c for soldering (unsafe)
```

---
## \#13 Posted by: taco Posted at: 2019-01-27T03:05:03.796Z Reads: 189

```
Spot welding doesn't generate as much heat, it works on a much smaller area than a soldering iron which is a big piece of metal and has tons of heat capacity.  I can touch the terminal immediately after a spot weld and its not scorching hot, it is after soldering.

OP: Rather than bending metal tabs to meet the other segment of your battery, just solder some lengths of an appropriate gauge wire to some nickel tab, then spot weld those nickel tabs onto the battery.  That will allow the wire to do the bending instead of your nickel tabs.  This is how a lot of large factory-made packs are done.  

Certain cell layouts are easier to wire without needing as many connections like this - a big long serpentine arrangement is really great if you only have 2-3 parallel, avoids having to turn corners or connect cells head-to-toe. (i realize that's not practical for a lot of eSkate builders as we need typically thinner packs that have more parallel cells.)

Be careful to insulate everything really well! if you have enough rattles to break those connections then think about how the cells might also rattle around in there, rubbing against each other or the case. The factory shrink wrap on most cells is not very durable.
```

---
## \#14 Posted by: Sender Posted at: 2019-01-27T03:21:11.521Z Reads: 179

```
[quote="b264, post:8, topic:82218"]
but it’s not recommended because it’s nigh impossible to do that without getting the cell too hot and degrading it.
[/quote]

I still think it is fine to solder on the batteries some times if you:

1.  Have a good soldering iron and appropriate tip.

2.  Are fast; in and out.

3. Know what you are doing.

4.  Aren't a moron.
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-01-27T03:23:12.945Z Reads: 175

```
What happens if I am:
1. using old kit
2. have a weak solder pull out game
3. am a dumbass
4. <see #3>
```

---
## \#16 Posted by: mmaner Posted at: 2019-01-27T03:30:38.173Z Reads: 174

```
Don't. &nbsp;
```

---
## \#17 Posted by: moon Posted at: 2019-01-27T03:36:11.285Z Reads: 172

```
[quote="Sender, post:14, topic:82218"]
Aren’t a moron
[/quote]

Unlucky guy
```

---
## \#18 Posted by: LEE Posted at: 2019-01-27T05:21:16.505Z Reads: 172

```
![image|431x500](upload://p629vldjT9lFdgMVfSh7MmOel1u.jpeg) ![image|611x500](upload://8hBr7SAS5c9UajX6ev2gCW4jJN9.jpeg) ![image|275x499](upload://lJuNpaA9u0tp664v4sRZNYg2obQ.jpeg) 

Friend owned inboard M1 nickel broke.
I am a little skeptical about the battery build that folds nickel.
Is there a good way to secure the series single stack securely?
I think the Chinese 10S2P double stack is robust.
```

---
## \#19 Posted by: pat.speed Posted at: 2019-01-27T09:46:37.610Z Reads: 158

```
Personally the pack design isn’t great, the series connections should ideally run down the length of the battery and then at one end have a bridging WIRE to connect either side of the lots of cells. This way no strips are bent and the two half’s can flex to the concave of the deck. Like this diagram from @mmaner 

 ![image|690x287](upload://caAhsEcD23SyV4AudnaU0eWKs6f.jpeg)

If you can redo the pack that is the best, but adding braided wire for the serial connections is another good way
```

---
## \#20 Posted by: MysticalDork Posted at: 2019-01-27T10:15:50.115Z Reads: 151

```
If you decide to go with nickel strip, one way to reduce the amount of bending that the nickel sees is to increase the radius of the bend. Space the cells farther apart, so there's more room for a less-sharp bend, and then put something stiff and slightly compliant (like a 1/4" thick strip of firm rubber) between the cells to keep them from smooshing back together. This can also be paired with using several thinner strips instead of one thick one.

If you go with copper braid or wire, use one that has lots of fine strands, and keep the radius large just like above. It does zero good if the whole thing is saturated with solder, that just makes it behave like a solid bar. You want solder on the ends, and none in the middle. When I was doing my packs, I always used a pair of hemostats clamped on the braid to suck the heat out and keep the solder from flowing up into the middle, which worked great.

Side note on soldering to cells: If you're at all uncomfortable with it, don't do it.

[spoiler]If you do do it, have a good temperature controlled iron with a clean fat tip.

Use an aggressive flux (not just the stuff in the solder wire), I use "ruby fluid" liquid flux, sold at my local hardware store for soldering copper pipes. It becomes active at a lower temperature than rosin flux, and that means it takes less time to tin the cell. Less time means less heat is transferred.

I add a small drop of flux to the cell, and with a blob of solder to the iron, I quickly tin the cell, then cool it back down to room temp. Then I tin the copper. Then I put the copper on the cell, and use the heat of the iron to melt and smoosh them together, using the absolute minimum amount of heat and time. Immediately cool the cell again.

I find that having the iron very hot (~400C) allows it to bring the joint up to temperature much faster, and thus the actual amount of heat transferred to the cell is less than if you tried to go with a low temperature.[/spoiler]
```

---
## \#21 Posted by: slade Posted at: 2019-01-28T06:37:42.851Z Reads: 133

```
Yeah, I wish I had seen something like that earlier on :confused:
It's only my first build so there are many other smallish things I'd go back in time and change too.
```

---
## \#22 Posted by: slade Posted at: 2019-01-28T06:39:17.283Z Reads: 137

```
Update: Today I bought some tinned, braided, copper wire and soldered the connections together as such:
![20190127_132146|281x500](upload://hqsPpC36IjJe0J2NiNhAUmqtx7u.jpeg) 

I reassembled everything in the enclosure and took it for a mile and a half loop. Everything seems fine so far, but only time will tell I think. I'll update here if it breaks again.
```

---
## \#23 Posted by: pjotr47 Posted at: 2019-01-28T13:54:18.308Z Reads: 130

```
May I be honest with you? Sorry but that pack looks like shit. I would not even trust it in my neighborhood. Please start fully over again. Take your nickel off your cells, dremel the top and button flat again. Buy some good, stiff, 10-12mm wide nickel weld them again on those cells.
```

---
## \#24 Posted by: Yecrtz Posted at: 2019-01-28T14:17:46.672Z Reads: 130

```
That looks like a safety hazard..
```

---
## \#25 Posted by: slade Posted at: 2019-01-28T18:21:54.614Z Reads: 124

```
Thank you for your opinion. I'll consider it if/when I remake my enclosure
```

---
## \#26 Posted by: taco Posted at: 2019-01-29T22:29:38.888Z Reads: 118

```
may be a little bit hazardous... but more than that it is likely to have additional failures and internal disconnections that disable your board. Why not spend the time to get it closer to perfect? Those braided lengths of wire are not long enough, presumably from your photo you once again are asking metal to stay intact after bending it 180 degrees and subjected to the same stress that broke the nickel tabs.

Focus on isolation of individual pack segments, longer lengths of braided wire with the sheath still intact. 

People will overstate the safety risks often IMO but they shouldn't be ignored completely,  People have lost their homes to bad battery assembly.  Like I said more likely it will be just disappointing or embarrassing if you don't take time to get it right.
```

---
## \#27 Posted by: slade Posted at: 2019-01-29T22:52:22.554Z Reads: 115

```
What are you using to prevent shorts between the top and bottom rows? Fish paper?

Also, one of the main reasons I didn't do this configuration in the beginning was that this has 10 junctions of this troublesome head-to-toe arrangement that I tried to use the U bends to resolve. What are you doing here for those joints that I can use to improve mine?
```

---
## \#28 Posted by: pat.speed Posted at: 2019-01-29T23:13:59.591Z Reads: 113

```
I will only be having one row as it single stack, but yes fish paper would be put between the rows. I will also be having fish paper separating each p group. 

In a single stack design I am going to lay a strip of copper on top of the cells at each end and then connect that to the nickel welded to each end of the cell with 14awg wire. This way I can just run 1 12awg wire between each series connection on top of the cells. 

You could also rotate the cells 90 degrees so that you can then do one long nickel/wire connecting the p groups
```

---
## \#29 Posted by: slade Posted at: 2019-01-31T06:15:32.022Z Reads: 102

```
Do you have links to examples, guides or general photos of how others are accomplishing this?
```

---
## \#30 Posted by: pat.speed Posted at: 2019-01-31T06:24:27.387Z Reads: 105

```
@thisguyhere sells pcb boards that make it much easier and tidier. If you also have a look through this thread you might get some ideas 


https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102
```

---
## \#31 Posted by: thisguyhere Posted at: 2019-01-31T06:37:50.011Z Reads: 101

```
some recent photos of batteries being built, see if you find any of it useful

   https://photos.app.goo.gl/PdFRx9yzJ9UqUtHg7
```

---
## \#32 Posted by: slade Posted at: 2019-01-31T06:38:00.891Z Reads: 105

```
Yeah, I remember looking back briefly at that thread you linked to early into my build and at the time remember seeing things like this: 
![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/a/fa523b70834b68e8657fb43c7303a4407c41e524.jpeg)
And thinking 'oh, the head-to-toe connections just look like some bend nickel, easy-peasy.

From the sounds of it, you're suggesting to redo the head-to-toe connections to be more like this?:
![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/a/8/a8c5834d45777d4553b7bdf8789f6d68783ba435.jpeg)
With the bend right angle nickel strips over the edge of the batteries, with fishpaper insulating behind it

Both of these photos are from that thread.
```

---
## \#33 Posted by: slade Posted at: 2019-01-31T06:40:21.655Z Reads: 101

```
So I really like the video in that album of the pack once there's two rows of batteries, but I just don't see how those two rows are connected in series. What are you using to connect it?
```

---
## \#34 Posted by: thisguyhere Posted at: 2019-01-31T06:45:51.398Z Reads: 104

```
see if this helps

   https://photos.app.goo.gl/cC64ujNoLHkNBhFK9
```

---
## \#35 Posted by: thisguyhere Posted at: 2019-01-31T06:48:05.175Z Reads: 104

```
but to answer your question, the two half are connect here using the same copper strand you see for the other series connections:

![image|690x216](upload://dPPvoW1xrT3nnE76NCJbuSSpWv6.jpeg)
```

---
## \#36 Posted by: slade Posted at: 2019-03-10T02:05:01.335Z Reads: 96

```
THIS IS NOT A FINAL SOLDER. Just an example of what I'm thinking about to give an example. I'm taking the communities advice and remaking my battery connections. I recently bought some better flat braid wire and more nickel strips. This photo's an example of the idea I'm seeing, with the only-right-angle bends and wire on top. 
![20190309_175803|281x500](upload://dqpiKQZjIxmtggUUNz0fckr7mK0.jpeg) 
Obviously this pic has some pretty cold joints but the concern I'm having is that the nickel strips are still going to break between the terminal and connection to braided cable. 
In addition, I'm noticing the braided cable is pretty stiff, since the solder gets so quickly sucked up along the fine threads through capillary action. 
Any advice on how to tackle these concerns? 
Thanks
```

---
## \#37 Posted by: TowerCrisis Posted at: 2019-03-10T03:04:49.323Z Reads: 92

```
Pre-tinning the nickel will help, the faster you solder the less it will wick.

You should also have a horizontal nickel strip going sideways across the P group, it will help keep the strip stable and prevent damage.
```

---
## \#38 Posted by: deucesdown Posted at: 2019-03-11T14:18:35.555Z Reads: 84

```
[quote="slade, post:36, topic:82218"]
braided cable is pretty stiff, since the solder gets so quickly sucked up along the fine threads through capillary action
[/quote]

Short lengths of copper wire will do that, I don't think you can prevent it.

Here's one method to deal with it

https://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411/81?u=deucesdown

And generally scroll through this thread and look at photos

https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102/42

examples like this https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102/13?u=deucesdown the long bent wires on the left, will help with wicking of solder.

Another example more similar to yours (my post) https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102/163?u=deucesdown

btw use fish paper not electrical tape. e-tape won't stand up to abrasion.
```

---
## \#39 Posted by: Fiori Posted at: 2019-03-11T14:39:10.963Z Reads: 76

```
In my opinion you just need to secure the battery better.  The battery shouldn't really be under that "accordion" style stress that caused those pieces to break, and making stronger connections isn't really the answer.  I'm not saying you don't need strong connections, I'm just saying that your connections shouldn't be the only thing holding the battery together.

I would just re-weld it just like you did(assuming these are spot welded?) and wrap the shrink wrap better/tighter this time and also add some support. You can use some strong tape as support for the battery before you shrink wrap it to give it more rigidity. Use clear shrink wrap. 

Then you need to make sure there is padding around the battery so these battery destroying vibrations don't ruin anything else.  Adhesive backed felt tape works really well.

Finally, I'm not sure how the battery is secured, but it needs to be supported better to reduce stress. Strong connections, structural support(not the connections), thick/thorough insulation, and sufficient padding are paramount to building a safe and reliable battery.
```

---
## \#40 Posted by: deucesdown Posted at: 2019-03-13T14:37:30.373Z Reads: 69

```
+1 I usually cut a sheet of abs slightly larger than the pack, tape it to the pack, then shrink. Even for a flex pack the abs is flexible, but will mostly keep things from moving around.
```

---
## \#41 Posted by: slade Posted at: 2019-03-14T05:53:29.373Z Reads: 65

```
Where are you able to find the ultra wide nickel strips? The only way I've found it is in giant reams of 50+ meters
```

---
## \#42 Posted by: slade Posted at: 2019-03-14T05:56:08.437Z Reads: 67

```
By adding strong tape, do you mean just SUPER tightly wrap the entire pack in something like packing tape before shrink wrapping it?
```

---
## \#43 Posted by: deucesdown Posted at: 2019-03-14T11:25:06.302Z Reads: 58

```
[quote="slade, post:41, topic:82218"]
ultra wide nickel strips
[/quote]

https://m.aliexpress.com/item/32832709611.html?trace=wwwdetail2mobilesitedetail&productId=32832709611

It's very tedious to find on aliexpress...

[quote="slade, post:42, topic:82218"]
strong tape,
[/quote]

Filament strapping tape

https://www.amazon.com/Scotch-Filament-Tape-Clear-Pack/dp/B00548R6AU

But really any way you can think of to stabilize.
```

---

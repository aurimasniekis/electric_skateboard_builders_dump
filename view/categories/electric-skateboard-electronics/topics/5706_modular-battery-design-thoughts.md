# Modular battery design. Thoughts?

### Replies: 23 Views: 3161

## \#1 Posted by: michaelcpg Posted at: 2016-07-07T10:26:59.639Z Reads: 300

```
Hey guys,
I'm about to look at building a 10S4P pack using LG HE4 cells. I'm wanting to be able to take my board on planes so I'm looking to build the battery in such a way that it can be pulled apart into 5 separate 2S4P packs to take in carry on, then easily be plugged back together via bullet connectors or similar.

I was originally looking to solder the cells together with nickel strips but the only place I seem to be able to find them is on Aliexpress where shipping takes close to a month to get to NZ without paying crazy amounts for shipping which isn't really ideal so instead I'm thinking about using 12 to 10AWG bare copper wire, preferably stuff that's made out of a few strands at most to increase rigidity. 

As I don't have room to use plastic spacers between the cells, I'm thinking about hot gluing them together into two parallel groups of 4 cells, possibly along with bamboo skewers running down the gaps between the cells to help strengthen the 2 groups. Each pack will then be covered in the same sort of heat shrink that's used on Enertion's space cells.

I may also look at adding a fuse between each of the 5 packs, possibly the same 40A blade fuses that the space cell uses?

<img src="/uploads/db1493/original/2X/c/c1e40fd4f3527cf7e36fb51eca3f2c0beb14b634.jpg" width="622" height="500">

Would be interested to hear what you guys think about this idea.
Cheers :)
```

---
## \#2 Posted by: Nordle Posted at: 2016-07-07T10:32:36.160Z Reads: 285

```
Your idea...
...it's a very good one i think:) recently did my first 18650 pack, and if i would make something different next time, would make it modular. As you said, it's better to take on a flight. You can change out broken parts or add booster.
```

---
## \#3 Posted by: PB1 Posted at: 2016-07-07T11:16:35.990Z Reads: 277

```
@michaelcpg I'm currently working on a very similar 18650 battery pack out of Samsung 25R. So I think this is a great idea! 

Total pack will be 10s4p, made out of two packs of 5s4p (so that I can fast charge them in parallel).
Each 5s4p pack will be made out of 1s4p packs. However I want to spot weld them in a way that they stay flexible. 
I've already hot glued the cells, no issues. 
Soldering the copper wire to the cells takes some care. 

Check http://ru.nkon.nl/ if they ship nickel strips to NZ. It's a very reputable Dutch company, the "russian" website is for non EU countries (no VAT).
```

---
## \#4 Posted by: Luke Posted at: 2016-07-07T12:12:56.692Z Reads: 269

```
Lol 30 euro shipping to get it all the way here, I call this geographic isolation tax.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-07-07T14:47:16.745Z Reads: 255

```
 Consider doing your pack with RTV silicone.
 It makes the pack a little more flexible and you can easily remove cells for replacement. 
<img src="/uploads/db1493/original/2X/1/18d7e40481b95392c33f5f8f999235653b67711b.jpeg" width="666" height="500">
```

---
## \#6 Posted by: DougM Posted at: 2016-07-07T15:09:30.778Z Reads: 235

```
I like the idea because then you could add/remove packs for range and weight considerations.

I guess each pack would have to have autonomous charge/management capability.
```

---
## \#7 Posted by: barajabali Posted at: 2016-07-07T16:33:50.073Z Reads: 230

```
I like the idea. Bullet connectors aren't a new idea to the battery world. People use them to make their terminal leads detachable from the battery and make their batteries break into two pieces for easy transport.

I've seen it done before but you can take it a step farther!
```

---
## \#8 Posted by: anorak234 Posted at: 2016-07-07T16:37:10.506Z Reads: 221

```
Sounds like an awesome idea! You could try using magnetic connectors like with a Mac for easy disconnect
```

---
## \#9 Posted by: mason Posted at: 2016-07-07T17:07:12.913Z Reads: 228

```
I'm in the middle of designing a quick-release lipo pack which will be very similar. If there is enough interest I will sell it.
```

---
## \#10 Posted by: Skitzor Posted at: 2016-07-08T09:44:52.838Z Reads: 217

```
It's a great idea. I recently was looking in to make a travel case for my raptor, but then I remembered the battery would probably be a hazard in checked or cabin luggage. And for 370 euro's you are not going to risk your space-cell getting confiscated... 

So I started looking into what the limits would be.
According to the FAA (Federal Aviation Administration):
<img src="/uploads/db1493/original/2X/f/f9b77ec63ac85645fd335dcdf833dd565e7513bc.PNG" width="690" height="154">

So max: 160 * 2 = 320 Wh , this is slightly less than a half 10s3p battery...
```

---
## \#11 Posted by: michaelcpg Posted at: 2016-07-12T08:50:58.952Z Reads: 200

```
<img src="/uploads/db1493/original/2X/a/a93fe70c54f1fddaa967c8e5a7536cc2a3daeae3.jpg" width="690" height="388">

Just a bit of an update. I've changed the design a little for several reasons. I'll still be building 2s4p packs but instead if just bare copper wire. The cells will each be connected to 10AWG wire via fuse wire that's rated at 20A. So far this design has made it much easier to solder them cells together and means I don't need to apply as much heat en soldering wire to each cell. Will post another photo once I've got one of the packs all wired up :)
```

---
## \#12 Posted by: Nordle Posted at: 2016-07-12T08:53:43.221Z Reads: 197

```
Tesla style!
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-07-12T09:52:33.173Z Reads: 207

```
<img src="/uploads/db1493/original/2X/1/1f4191fafdc1d88b786c7a155c31c955fd9fcbc5.jpg" width="690" height="388">

One pack wired up. Just need to add some strength to the connection between two groups of 4 and then cover the whole thing in heatshrink :)
```

---
## \#14 Posted by: michaelcpg Posted at: 2016-09-23T00:10:56.808Z Reads: 179

```
It's been a while since I've posted an update... I've been through a few design revisions since initially building the pack like this. The main issue I've had with this original design is that the vibrations from riding on rough roads would sometimes cause the glue holding the batteries together to become unstuck which would allow them to move around slightly which often resulted in fuse wires breaking.

Over the past week I've been rebuilding the battery using a more robust design. Wanna say thanks to @chaka for designing the awesome cell holders that I'm now using :)

<img src="/uploads/db1493/original/3X/8/1/81e23a1fd995e69e6ad58f6f953abdace25f3c77.jpg" width="690" height="388">

As you can see, I'm now using brass strips as bus bars instead of running wire above the batteries which makes the packs thinner :) 

<img src="/uploads/db1493/original/3X/6/f/6fabb1e428a25933b6bccdf8b48e46fb05e4a471.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/f/4/f408724a6a3e99ce78cf5c52aab325432c35b110.jpg" width="690" height="388">

I then soldered wires with spade connectors to the ends of the bus bars as a way of connecting the separate packs. I tried a few different ideas here before I was happy.

<img src="/uploads/db1493/original/3X/7/d/7da372b7d573bd750698d7c90bfb6f3d0f5c2486.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/e/1/e109581e44803ada9b59c99f53d88c3ac4686668.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/3/632b9be1ecd834973e0d8354d08b23e0e038827d.jpg" width="690" height="388">

Then it was just a matter of covering the ends of the cells in electrical tape and connecting them all up :)

<img src="/uploads/db1493/original/3X/a/d/ad2b4793cfdce63bcac0cf5beecb228afc86d28b.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/4/5/4563dcda03855cc788e00651d10217db15deabd4.jpg" width="690" height="388">

This is currently where I'm up to. Still need to cover the packs with heat shrink as well as a layer of felt for vibration dampening. 
The end result is that I have a 360Wh battery that I can break down into 4x 72Wh packs and 2x 36Wh packs, so fingers crossed I'll be able to take my board when I go flying :)
```

---
## \#15 Posted by: Pantologist Posted at: 2016-09-23T00:14:24.020Z Reads: 164

```
Sweet. That looks super clean. 

Just curious. What is the difference in specs between brass strips and nickel ones?
```

---
## \#16 Posted by: michaelcpg Posted at: 2016-09-23T00:26:58.711Z Reads: 159

```
Cheers. I believe brass has slightly better conductivity than nickel. These strips are significantly thicker than what people around here use for spot welding as well though

https://www.bluesea.com/resources/108/Electrical_Conductivity_of_Materials
```

---
## \#17 Posted by: chaka Posted at: 2016-09-23T00:36:22.294Z Reads: 160

```
Looks nice! How do they fit against the ridges or your enclosure?
```

---
## \#18 Posted by: michaelcpg Posted at: 2016-09-23T00:39:44.155Z Reads: 166

```
Thanks :) They fit, but not perfectly. I'm not concerned about it though, my next project will be to design a wood deck with internal space for the batteries similar to your FreeRide decks so this is just a temporary situation :)
```

---
## \#19 Posted by: boards Posted at: 2016-09-23T01:03:38.110Z Reads: 165

```
<img src="/uploads/db1493/original/3X/2/6/26d1f11844d2499b2dcbc01f71925393acfe50c5.jpg" width="375" height="500">

I'm also doing the legendary @chaka design. Waiting for an open source BMS to come along though, so currently will have to use imax as charger. (Shouldn't be bad since battery will split up into parts < 6s). I think this design will hopefully just allow me to use my 50w weller station to attach fuse wire to the cells, might have to buy a 100w though (Or even finish my spot welder build).

I think I'm also going to modify my wood deck with a router to make the board slimmer with batteries. (Currently has no flex, so hopefully it'll be fine)

Any tips if using a spot welder is worth it in this kind of battery build?
```

---
## \#20 Posted by: DougM Posted at: 2016-09-23T18:41:22.630Z Reads: 151

```
There is an open source BMS [here](http://raphaelchang.com/projects/bms/) that I'm going to start looking into since my attempts to deal with the chinese BMS vendors ended in frustration.

It looks like he's actively working on it - V3 of the hardware was last touched 28 days ago.

Bonus that it uses my favorite processor, the Teensy 3.2.
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-09-23T19:44:40.119Z Reads: 145

```
oh wow! i'm bookmarking that.
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-09-23T19:58:14.333Z Reads: 147

```
also yes! modular packs! i was thinking about that very thing the other night. Isolated P-groups with bullet connectors on the mains and a healthy length of balance lead that can be trimmed later to go back to the BMS.
```

---
## \#23 Posted by: Svenska Posted at: 2016-09-24T05:16:18.937Z Reads: 134

```
Is there a link for the cell holders?
```

---

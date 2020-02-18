# Polyurethane battery enclosure, bad idea?

### Replies: 17 Views: 3191

## \#1 Posted by: lock Posted at: 2017-06-03T13:12:07.375Z Reads: 468

```
Really just thinking out loud with this one... would appreciate any input.

I'm building up a Trampa street carver and looking over the various options for mounting stuff. There's the above board 'box' (not my preferred option) and the below board segmented enclosures ala Kaly and whitepony.

It was one of the guys at work that suggested why not just make the enclosure out of a flexible material. Polyurethane came to mind, and it seems [fairly readily available in quite a range of stiffnesses](http://www.barnes.com.au/polyurethane-53). By my rough maths it seems the material would need to stretch 3% or so, which seems reasonable for 50-60 shore A resin.

### Pros
- Flexible
- Should make for good watertight seal against board

### Cons
- Less structurally stiff than CF or ABS, batteries could be damaged by impact
- Doesn't like high temps (above 80 deg C)
  - so maybe BMS + VESCs get located to a separate enclosure made from a different material?
- Heavier than CF and ABS

Noticed @Hummie has [sealed their battery pack with it](https://www.electric-skateboard.builders/t/potting-the-vesc/3149/13), so there's some precedent. 

Am I missing anything?
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-03T13:36:17.734Z Reads: 441

```
I personally don't see any problems with it, but how would you mould it? 

Also if the BMS and VESC get to 80C you have bigger problems than a melting enclosure lol.. you should be fine making the entire thing out of Poly. 

I think it would be cool to try something new!
```

---
## \#3 Posted by: lock Posted at: 2017-06-03T14:34:35.039Z Reads: 429

```
[quote="JLabs, post:2, topic:24480"]
I personally don't see any problems with it, but how would you mould it?
[/quote]

Yeah, most silicon moulds are made from existing parts of which I obviously don't have. 

Was thinking about making a male plug using the board, and some high density insulation foam sealed and sanded with a primer. From that the female mould would be taken. A thin layer of modelling clay(?) would then be laid in the female mould to make up the part volume. The inside surface of this layer would be pretty average, but it's the inside of the enclosure so doesn't really matter. After application of mould release, the top half of the mould would then be poured over the female mould + modelling clay.

After the top and bottom moulds have been made it then becomes a conventional mould type process. Of course I've never moulded anything, so I'm certainly not 100% this will work.

Good to know about the VESC / BMS temps :thumbsup:
```

---
## \#4 Posted by: baxter Posted at: 2017-06-03T16:00:04.301Z Reads: 396

```
I think the Buffalo F1 had the right idea in terms of allowing flex under the board. If memory served they used moulded silicon with by solid supports around the parallel cell packs:

<img src="/uploads/db1493/original/3X/9/6/963bce7acb595fd433a3c79d9e95e7347ffc9602.png" width="680" height="301">

<img src="/uploads/db1493/original/3X/a/6/a68be60824526583a3662ee2d49401b2b5927672.gif" width="680" height="295">
```

---
## \#5 Posted by: Hummie Posted at: 2017-06-03T16:49:55.978Z Reads: 430

```
<img src="/uploads/db1493/original/3X/6/2/62884c11e87202c61fe95ebbc2db6d9f17206ed9.jpeg" width="666" height="500">Smooth-on has great stuff if you haven't seen it.  And jbjengineering or bjb. 
I think you could do it quickly with some structure on the board as the plug, then polish it with wax and lay wetted carbon or glass on top with hard polyurethane.  The onyx from smooth-on is awesome and hardness in like 3 minutes.  
Making a silicone mold I think it would need a mother mold too to give it structure and a lot more time and work than

Set it up for flex somehow as what I have now is just lipos glued down with 80duro pu an carbon glued to the top and the carbon is so stiff it's peeling the cells off the board
```

---
## \#6 Posted by: lock Posted at: 2017-09-05T23:59:45.661Z Reads: 400

```
Some success, some failure. TBH I never really expected this to work first try, fortunately polyurethane is reasonably cheap and I still have enough left over for at least one more attempt.

Plan was to always make a mould the 'old fashioned way'; carve out a male plug, and take a fibreglass female mould from it. However, I found a local company who specialised in CNC machining various types of foam. Quote wasn't too bad, just a little more than what it would have cost me to do it the 'old fashioned way', so thought why not.

Measured up the Trampa deck, and set about designing something I didn't mind the look of.
<img src="/uploads/db1493/original/3X/3/d/3df62e6917bf683254ade3d7b4d103e08441926f.png" width="690" height="469">

Month passed before I was able to pick up the machined mould. A little longer than expected, but I don't think they were really making any money out of this so really didn't want to be pushy.
<img src="/uploads/db1493/original/3X/2/1/21de0c1d2d47ad0a6624e1b15fab69fa9b0cd9c3.png" width="426" height="500">

It's a urethane foam, quite dense and somewhat heavier than expected when you first pick it up. I sealed it with about 5 coats of a water based polyurethane paint. While denser that polystyrene, I'd still expect it to soften if exposed to any sort of solvent.

<img src="/uploads/db1493/original/3X/a/3/a398a683574086c79d2341a08720af33964f389d.png" width="375" height="500">

Relieved to see the CAD geometry, and that of the actual board measured up ok.

<img src="/uploads/db1493/original/3X/3/f/3f9b2151d09ff6db5cd5950a681dc6d5f261af5c.png" width="375" height="500">

Modelling clay to build up the flange areas.

<img src="/uploads/db1493/original/3X/9/0/9092288e9064ce9b886c5368336a643ff30d0403.png" width="375" height="500">

Few coats of mould release wax were applied, followed by a single coat of PVA (blue stuff).

<img src="/uploads/db1493/original/3X/1/d/1dfbe0e638b79de6c1ef8c0e789ddab0e50b4ae2.png" width="375" height="500">

Finally the black stuff goes in. This is a 65a polyurethane, usually a yellowish colour, but I mixed in a black pigment. This particular type has a long'ish work time of 25 minutes. Initially I painted the mould, then added a thickener to the resin. Theory being the thickener would allow it to stick to the vertical surfaces.

Spent the next hour or so trying to smoosh the thickening polyurethane away from where it wanted to pool. . . with limited success. Left it sit in the mould for the next 48hrs just to be sure it dried.

It released really well from the mould which was nice as I'd like to use it again. However it was immediately obvious it was somewhat more flexible than I'd like and had expected. :joy:

<img src="/uploads/db1493/original/3X/0/7/07eb21c28058256949d3aeb5125eaab3e83aca79.png" width="375" height="500">

Main problem is that the vertical surfaces are really quite thin (no real surprise), as in less than 0.5mm thin :unamused: .

<img src="/uploads/db1493/original/3X/5/9/59c93175eb378eafd2a76789fb76997bccf391d3.png" width="375" height="500">

Still, there's some success in that I do actually quite like the way it turned out from an appearance perspective, and there's certainly no concerns about it stiffening up the board  :joy:.

Figure I have a few options, open to suggestions here...
- Give up and use CF / fibreglass in the mould.
- Manufacture a top half of the mould somehow. Could also include a few internal walls that run between the battery segments.
```

---
## \#7 Posted by: lock Posted at: 2017-11-20T01:29:39.401Z Reads: 393

```
Moving house kind of put this project on the bench for a while, back onto it now.

To make the other half of the mould I needed to create a void out of something, so lined the mould with modelling clay. Rolled in out to be about 4mm thick using a rolling pin and 2 strips (4mm thick) of masonite that were placed either side of the clay under the rolling pin (to ensure even thickness).

<img src="/uploads/db1493/original/3X/8/3/834627eaa9983aac8a56b924dfb0aba7137ec112.png" width="375" height="500">

Used some cardboard I had lying around to make ribs running across the board, first 4 rows are for the batteries, then BMS, cables, and finally the VESCs. Internal surface finish isn't great, but no one will see that... 
 To get an outline that matches the Trampa deck I placed the deck on top of the clay and simply ran a butter knife around the outside of it cutting off the excess clay, the edge of the enclosure lines up rather well with the deck.  Those squares around the edge are the locating pins for the top half.

<img src="/uploads/db1493/original/3X/8/9/89de1452fba83080734ede5664f640ec05cd6003.png" width="375" height="500">

Covered the mould and clay with PVA mould release and a few coats of wax (not shown). Then laid down a thick coat of a 'trowel on' hard (80 shore D) polyurethane mix. It's really rather thick, and quick setting, basically by the time I had sufficiently mixed it I was running out of work time.

<img src="/uploads/db1493/original/3X/c/8/c846c1b7ca2298ede00b4a9345b4c6dc0d06e6f6.png" width="375" height="500"> 

Left it a day and peeled the mould off. Took an hour or so to get it cleaned up to this extent 😒
<img src="/uploads/db1493/original/3X/0/4/04b545dee167df326030921b3dfcb851ddb0f058.png" width="375" height="500">

I don't have a particularly good plan for filling this mould. Ordinarily the two halves would be fixed together, and you'd fill it up via a hole from a low point making sure you had vent holes at all the locations bubbles could form. This wouldn't work here as the viscosity of the liquid polyurethane is too low to flow through the mould. Instead I mixed up a batch, poured it in the bottom half and just squeezed the two halves together. Could have worked, but I didn't mix up enough, hence there's a number of missing sections and large bubbles.
<img src="/uploads/db1493/original/3X/4/5/453a2f1862709a931deb9bd6b1b4132954252896.png" width="375" height="500">

Still it's an improvement from the last attempt. Wall thickness around the outside is much better, and the cross ribs (well the ones that worked out) add a lot to the stiffness.

3rd attempt is in the mould, should be ok to pull out later today🤞.
```

---
## \#8 Posted by: lock Posted at: 2017-11-20T23:25:24.740Z Reads: 369

```
Drilled a series of holes in the top half of the mould to hopefully allow air and excess polyurethane to escape. The downside is the excess squeezed out sets on top of the mould and required quite a bit of effort to cut off before even thinking about trying to open up the mould.
<img src="/uploads/db1493/original/3X/a/0/a03ee20b580de522abc031d8c214c5bb01b230ad.png" width="375" height="500">

It worked out pretty well this time around. Few bubbles, but nothing that'd stop me from trying to use it. Here it is straight out of the mould.
<img src="/uploads/db1493/original/3X/8/1/8182d94bd80f9c80759e9b9fcff717aff5dffe77.png" width="375" height="500">

And all cleaned up.
<img src="/uploads/db1493/original/3X/8/8/88579340ef22442fb21b4cf148446736df011610.png" width="640" height="204"><img src="/uploads/db1493/original/3X/6/7/6770751f88b6e6a85041d5bff346bd01197289a1.png" width="640" height="323"><img src="/uploads/db1493/original/3X/7/d/7da820fe53a1923d77f174ec74417538849a854f.png" width="640" height="429">

Now about that colour. Got sick of wasting pigment while sorted out production issues so left it out of this one. The polyurethane is a clear yellowish colour normally, but when mixed with the white thickening fibre you get left with this 'off white' colour that's really only reminiscent of one thing 😏. Transparent enclosure would be cool; maybe something for the future.
```

---
## \#9 Posted by: lock Posted at: 2017-11-27T23:56:10.731Z Reads: 353

```
Drilled a bunch of holes, and installed some thread inserts in the deck over the weekend. Was a little keen to see how the enclosure performs when mounted.

I drilled all the holes in the white enclosure, but wasn't happy with the results. While the drill bit worked though the polyurethane quite easily, it really just kind of teared its way through 😒.

<img src="/uploads/db1493/original/3X/c/a/cabdc8a2079cd9672a272cb7c861351b710617b6.png" width="601" height="500">

Picked up a 'leather punch', tool used to put extra holes in a belt, and the results are much better.
<img src="/uploads/db1493/original/3X/0/c/0c02a98cb2124d5f479e1964e6d9cc66d1cbdf9e.png" width="610" height="500">

Installed the battery, and screwed on the enclosure. Here's the obligatory Trampa flex test. Didn't notice any change in stiffness, but didn't expect too.
https://youtu.be/bXx9dK56j14

Seemed to hold up ok for the 5 minutes I bounced on it for; long term durability is still a concern.
```

---
## \#10 Posted by: lrdesigns Posted at: 2017-12-05T05:35:14.378Z Reads: 334

```
Wow, really amazing DIY effort. :astonished: and I like the design with the triangular de-bossed areas.
```

---
## \#11 Posted by: lock Posted at: 2017-12-05T06:04:26.737Z Reads: 327

```
Thanks! 

Figured if I was going to the effort of getting the mould CNC'ed I may as well put some detail in, even if it is for purely for aesthetic reasons. I'm happy with how it looks, especially in black.

<img src="/uploads/db1493/original/3X/c/9/c90e81252aa9a8875a2dc2dcc84998cffe01e717.png" width="690" height="363">
```

---
## \#12 Posted by: barajabali Posted at: 2017-12-12T00:45:46.312Z Reads: 314

```
You should sell this design to Trampa themselves.  

Bravo!
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-12-12T00:46:45.581Z Reads: 312

```
nah cause they’ll copyright “enclosure” and sell it for $6000
```

---
## \#14 Posted by: lock Posted at: 2017-12-12T02:33:37.910Z Reads: 303

```
Good point, always planned on releasing the CAD for all this stuff. Don't think the enclosure would be of much use, but the Trampa deck model may be.

Anyway [CAD (STL & STEP) can be found over in my github repo](https://github.com/lachlanhurst/locks-esk8/tree/master/cad/enclosure). I'd be happy for anyone to use the enclosure model under a Public Domain (do whatever) license. So yes Trampa, feel free to take the model, make it better and sell it back to me.
```

---
## \#15 Posted by: Juvaknin Posted at: 2018-03-23T17:18:53.200Z Reads: 221

```
Nice work! I need one.. if you can im ready to buy one.. can you sell one??...
```

---
## \#16 Posted by: banjaxxed Posted at: 2018-03-24T20:59:55.836Z Reads: 197

```
Those cads are great to have, anyone with a cheap cnc mill can use it to make their own male wood mold and form an accurate trampa enclosure with kydex etc, no need to leave diy...and hey if you prefer segmented, then change the cad and link-up as lock did

Occurred that without a CnC you could still get creative and 3d print the mold in abs which can survive the heat afaik...just print in sections

Might even be something to print straight out in flexible filiment
```

---
## \#17 Posted by: lock Posted at: 2018-03-25T05:22:37.869Z Reads: 183

```
Followed up with Juvaknin via PM. But general gist is I still have no plans to sell this. The enclosure seems to be holding up well, but it's only done 50km or so. It's also a PITA to make, and there's a fair amount of luck involved in the process. Maybe you'll get a massive air bubble, maybe you wont.

It's a pretty big model to 3D print, but using flexible filament sounds interesting. And wood, either for a male/female mould sounds good. This was carved out of a high density foam, but the foam they used is actually rather expensive.

The original plan was to use this mould for a CF vacuum formed enclosure. Flexibility would be introduced by cutting through it much like the Trampa battery tray. Would still like to give this a go one day, setup costs are a little high for me right now.
```

---

# 3D printing vs Street Vibration - TPU or ABS next?

### Replies: 12 Views: 700

## \#1 Posted by: accrobrandon Posted at: 2018-07-31T00:42:15.688Z Reads: 121

```
So I designed this light holder for my board cuz i really dig this specific light. My first try not knowing anything about 3d printing plastics was the cheap option PLA... it eventually cracked apart in no time. Some one recommended PETG next but the same thing happened in less time and looked exactly the same inside where it broke. So whats next and can with stand the forces of the street?

If i do ABS my expectation is a solid piece of plastic through and through (not knowing anything about how it is printed) and hoping that would hold... 

option B would be TPU which sounds kinda rubbery and 3d hubs says there are variable hardnesses from 60a to 95a... and I assume 95 would be more rigind...and perhaps this is what i need? Something rubbery hard that can absorb vibration??

no clue about either tho...thoughts??

![0613180938b_HDR|690x388](upload://8sM7K45e9Q69dFXIUT6RFykELk0.jpg)
![0617182106|690x451](upload://4TiUmRwEAAD1uUICVlpP2tFo0fg.jpg)
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-07-31T00:48:50.022Z Reads: 107

```
Nylon... 100%. Nylon is slightly flexible but super duper strong.

Also, more walls. Infill doesn't make a huge difference, but do 5 perimeter walls for sure and .2mm layer height.

A layer of TPU dampening on the bottom, maybe 1mm and TPU washers under metal washers to bolt it all down, nylon sandwiched in TPU... This will 100% serve you amazing.
```

---
## \#3 Posted by: DougM Posted at: 2018-07-31T00:49:19.546Z Reads: 105

```
So what you have to understand about 3D printing is it's just like wood grain - it has one weak direction and that's the direction parallel to the grain.  The other directions are super-strong.

In your case the layers in the Z axis are the weak point.  You need to design your part so that the forces on the device aren't in the Z axis.

I'd print the thing with the front of the light flat to the bed of the 3D printer.  Then once it's mounted if it cracks it'll crack along what is now the Y axis.   Unfortunately that's where the screw holes are.  So you'll need to reinforce that section with a very large washer.

I have even printed pieces at a 25 degree angle from the bed before to get the grain into a non-critical direction.
```

---
## \#4 Posted by: accrobrandon Posted at: 2018-07-31T00:53:31.333Z Reads: 99

```
will keep in mind...just for reference i dont own a printer..i just order online cuz my needs are minimal at this point. thx
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-07-31T00:57:25.140Z Reads: 98

```
This too, but certain materials and higher temperatures with materials like Nylon and PETG, printing without a fan with Nylon and PETG and Z strength becomes essentially a non issue... I have parts crack in the Z axis that shear across multiple layers, the crack looking solid diagonally where the material strength itself took precedence over Z layer strength due to such good layer bonding. 

So OP if you need to use a cooling fan on PETG or Nylon for some reason, or use other materials like PLA, 100% consider reorienting your part. Otherwise, you need more walls, higher temps, less cooling fan. If PETG at higher temps, no cooling fan, 5 or 6 walls and <50% infill still gives you trouble even with your part oriented with stress on the Z layers still gives you trouble, I'd be surprised.

Also, the spot your light mount cracks is where there is a straight 90 degree hard angle. Try adding a small fillet, these are great for adding strength.
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-07-31T00:59:43.691Z Reads: 91

```
Also, let me know if you are trying to order from 3D hubs, I might be able to do it for you cheaper since I've already got nylon loaded, and can print TPU dampers/washers for you as well. I can add the fillets to your part too if you like and make any other changes you need. I can do TPU in natural (off-white) and Nylon in clear/off-white or black. I've also got PETG in neon green/yellow.
```

---
## \#7 Posted by: DougM Posted at: 2018-07-31T02:35:05.488Z Reads: 86

```
Totally get @skatardude10 to print your parts since he has experience in nylon.  I'll probably do the same if he offers :slight_smile:

To give you an idea, I printed this clamp, using supports, at about a 15 degree angle so the grain was angular to the stress lines.  Ideally it should be more like 35 degrees but that's a lot of support material.

![image|645x500](upload://g3eplYRSI8mppVqu0GgfZVo3sNQ.jpg)
```

---
## \#8 Posted by: danile Posted at: 2018-07-31T02:37:35.015Z Reads: 82

```
Consider also redesigning your mount.
The transition between the base and the upper block is way too "square".
```

---
## \#9 Posted by: deucesdown Posted at: 2018-07-31T02:57:09.641Z Reads: 78

```
The flex I've printed is ridiculously strong. With high infill it's not very flexible, dare I say almost rigid? But not good for overhangs and things like that. I've had good luck with hobbyking flex, which is on the hard side.

https://hobbyking.com/en_us/flexible-3d-printer-filament-black.html

So many uses for flex filament for eskate.
```

---
## \#10 Posted by: AutoItKing Posted at: 2018-07-31T03:51:28.687Z Reads: 73

```
This. Square edges will always start cracks. It's super easy to add a chamfer or fillet to your parts in Inventor, Fusion, SolidWorks, etc. If you do anything do this.

As far as material, I'm using a 3D printed wheel pulley made of PETG. Printed it with 2mm walls and 90% infill. It's basically a solid chunk of plastic. It's holding up well so far! The best tip I can give is to makes sure to print it with no part cooling fan at all, quality won't be quite as nice but it'll be strong. I've never had an issue with layer adhesion using no fan.

Flexible filaments can be a bear to print but it would be stronger. Layer adhesion can be a problem with flexibles though.
```

---
## \#11 Posted by: accrobrandon Posted at: 2018-07-31T14:38:09.534Z Reads: 52

```
thanks for the info guys... @skatardude10 will drop you a PM about a nylon print now vs 3dhubs =)
```

---
## \#12 Posted by: wafflejock Posted at: 2018-07-31T15:22:38.387Z Reads: 49

```
Yah Nylon will not crack I've stress tested it pretty thoroughly and can pretty much guarantee if it is dried properly the part won't break.  I made a motor pulley out of nylon and was able to ride with it for a couple of months before the grub screw started to wear its way through the nylon but for a part that is just sitting on the board or holding something on nylon will be fine.

Other advice still stands though and moreso with rounding corners from the top down view of the part so it doesn't warp up off the bed while printing, sharp corners don't work well anyhow since the printer needs to stop moving in one direction and start moving 90 degrees from that which it just can't physically do completely accurately, smoother edges help with the motion of the head and help with reducing shrinking/warping.

If the part is too big you may want to still go TPU since nylon needs to be printed relatively slow and is difficult to fight warping and water absorption relative to TPU and TPU still has a rubbery quality that will stop it from cracking worst case scenario it 'delaminates' between the layers because of being too cool while printing.  Downside with TPU being it 'droops' while printing so can suffer if you have big overhangs.
```

---

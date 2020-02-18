# New to the community - Rate My Build!

### Replies: 25 Views: 1426

## \#1 Posted by: emstr Posted at: 2017-06-19T06:28:24.850Z Reads: 203

```
Hey guys, I'm doing my first electric skateboard build. I've selected a couple parts and I'd appreciate feedback on it, no matter how critical. I'd also love to know of any must-have connectors or cables I'll need since I live in NZ and it's expensive to ship things here.

<img src="/uploads/db1493/original/3X/e/d/edc946ab39b00e530ff211e287d2f65827a7c7ba.jpg" width="666" height="500">

The parts I've got are the Wheels and belts from DIY: diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/

The 190kv sensored motors from DIY: diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/

A VESC from DIY (should I get a VESC-X instead, and why?): diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

The controller from DIY: diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/

3x 8000mAh 11.1v 30C batteries from Hobbyking: https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html?___store=en_us

Does everything look good? Let me know if I'm forgetting anything important (I probably am) I've prebuilt a deck myself so no worries on that front. What connectors might I need from previous experience?

I'd also really like to know how you guys would reccomend charging this build, I really would like to have an easy and quick solution which doesn't require me taking the whole case off.

Thanks so much!
```

---
## \#2 Posted by: gee Posted at: 2017-06-19T06:42:01.244Z Reads: 188

```
DIY motor mount only fits caliber trucks. So you should make sure that's the right trucks. 
VESC is fine I think. 
The battery that you pick has the SAME 5.5mm connector as my compact battery. They can connect in series but not in parallel. I know you trying to connect it in series but keep in mind that the vesc from DIY connector is a XT-90 male. SO the 5.5 mm doesn't really hook up nicely from the XT-90 therefore you need this 
https://www.amazon.com/gp/product/B01MY484TH/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
This allows you to connect the battery to the vesc without soldering. I had to order this because 5.5mm doesn't really stay on the vesc's XT-90.
You will need a charger to charge your battery don't forget that. Right now I charge it battery to battery. I'm thinking of buying the parallel charging board but I'm going wayyyy over my budget. 
We have similar build so you can ask me and I'll help you out. I'm new here too.
EDIT: don't forget to order the male to male connector to connect the receiver to the vesc. It doesn't include in the vesc so you have to select it from DIY.
```

---
## \#3 Posted by: emstr Posted at: 2017-06-20T00:28:09.696Z Reads: 142

```
Cool, thanks for your feedback!

Ever thought of using a BMS? Was looking at doing that over a balance charger, but it seems complicated and hard to buy.

I'm going to order the parts now, thanks for your help!
```

---
## \#4 Posted by: gee Posted at: 2017-06-20T14:08:42.444Z Reads: 109

```
I heard about the BMS but it seems a little complicated for me as of right now. BTW get threadlocker since i'm 100% sure your screws and bolts will fall off regardless of how tight you tighten it.
```

---
## \#5 Posted by: memesupreme Posted at: 2017-06-21T08:20:10.512Z Reads: 92

```
A bms is great for making it easy to charge the board and keeps all the cells balanced, which will extend their total life span. Im not a LiPO expert but I'm pretty sure you'll have to connect the corresponding balance wires of all three in parallel, also you'll have to make a sort of enclosure for it too, you don't have to have one, it's just like a nice little piece of security. Main thing to thread lock is the motor mount, the motor onto the mount, and whatever enclosure you plan on using, unless you want it to be removable. I haven't skated NZ roads in years but just in case still use thread locker👍🏽
```

---
## \#6 Posted by: emstr Posted at: 2017-06-28T05:24:18.876Z Reads: 84

```
@gee @memesupreme @Namasaki 

I need to choose my batteries. Battery needs at least 250wh to get me at least 10km of range.

I could either do 5x 8ah 2s batteries. https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html?___store=en_us

3x Battery 3s 30C 8000mAh 11.1V series = 9s 8000mah 34V

34*8 = 

272wh $120

= $0.44/wh

169mm*207mm*27mm = 945cm^2

**OR 3x 3s batteries 8ah**

5x 2s 8ah 7.2V - https://hobbyking.com/en_us/zippy-flightmax-8000mah-2s1p-30c.html

5*8*7.2

= 288wh $165

= $0.57/wh

166*(69*5)*15mm = 859cm^2

These are a little bit more expensive, but they give 10s instead of 9s and a seemingly smaller footprint. Would I be correct or is there something I'm overlooking?

I'm going to use bestech BMS. Either 

@Namasaki can you think of any parts I might need for this build as I'd like to order everything in one go to avoid NZ shipping cost multiple times.

Also, I'd like to get the bullet connector @gee but I'm going to the states for 2 weeks in 10 days and that item ships from China - is there one on amazon or hobbyking that I could use? Sorry, I tried to find myself but couldn't find one.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-06-28T05:58:26.427Z Reads: 70

```
Five of these batteries would give you up to 20km
They are hard case so they are more protected and easier to mount
They are thicker than the flightmax 2s but otherwise they are more compact.
Their wires are better situated making them much easier to link together in series
They are higher C rating which is always better
Last of all they are a little lower in price.
https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html?wrh_pdp=3
```

---
## \#8 Posted by: emstr Posted at: 2017-06-28T06:01:04.807Z Reads: 67

```
I do live in quite a hilly area. Very tempting though. You have these batteries yeah? You've gotten 10km with some slightly hilly terrain? - That would be my only worry, I like the 60C though
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-28T06:03:22.970Z Reads: 67

```
I get 16 km easy with lots of hills and up to 20 km on flat
```

---
## \#10 Posted by: emstr Posted at: 2017-06-28T06:04:58.808Z Reads: 60

```
So what are your feelings on the 8ah packs?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-06-28T06:07:40.394Z Reads: 59

```
I've never used them so I can't say for sure. They do sound tempting, it's just that they have such a large footprint.
If you have room enough, the extra 3000mah is a real plus
If you only need 10 km range, you wont drain the 5000mah packs more than about 50%
```

---
## \#12 Posted by: emstr Posted at: 2017-06-28T06:14:26.890Z Reads: 59

```
They are slightly bigger yes - however when I'm adding it up on my deck design they seem pretty similar

<img src="/uploads/db1493/original/3X/4/3/43059467f6f2ca3d6aaf3558211423ea02ef16b9.png" width="403" height="500">

The 5ah ones are 25mm while the 8ah ones stacked together would be 30mm. It's cool to stack them right? That would be one thing haha.

Also for the bms - will I need any wires to connect to the BMS that you think I might currently be missing?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-06-28T06:15:58.705Z Reads: 51

```
ok, I didn't realize your where stacking them.
It's much better not to stack them cuz they can't dissipate heat as well stacked.
Plus the wiring will be more difficult
They are very long so you wont have much room for the wiring on the end of the packs
You need to allow room for the enclosure flange
```

---
## \#14 Posted by: emstr Posted at: 2017-06-28T06:20:16.601Z Reads: 52

```
Would it likely be a big issue? I haven't seen anyone do it previously. I'm making the enclosure from fiberglass so I'll be able to customise the size.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-06-28T06:26:11.117Z Reads: 61

```
the wires on the 8ah packs come out of the end of the batteries on the same side and they are 10ga wires so you will have a lot of bulky wiring on the side of your pack making the total width about 7" to 7.5" Then you will need another 2" total for the enclosure flanges. You would need at least a 10" wide deck.
the 5ah turnigy batteries have 12ga wires that fold neatly on top of the batteries and because the wires are on opposite sides of the same end of each pack, it's very easy to link them neatly

This is a 10" deck and as you can see, you don't have the whole 10" to work with unless you have no concave.

<img src="/uploads/db1493/original/3X/f/9/f9ec9611b06617bd78a7dc8b507cc24d4354f3b8.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/e/2/e2099006099577f970e90422828166fe2f0d623b.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/1/c10db52cb4e91b5d00c7714d2bc95998042cc7d1.jpg" width="666" height="500">
```

---
## \#16 Posted by: nmagz3 Posted at: 2017-06-28T06:49:13.035Z Reads: 52

```
So far so good!  I totally agree with you regarding shipping costs.  If there wa anything else that I'd do differently to save money would be to get my parts from one place.  However, although I lost out on saving some cash I did have a great lesson on who does what in the esk8 industry.  Good luck with your build!  Can't wait to see it :slight_smile:
```

---
## \#17 Posted by: emstr Posted at: 2017-06-28T07:09:23.975Z Reads: 53

```
I'm noticing you have two motors - If I used the 5ah batteries would I get better battery performance with my one singular motor?
```

---
## \#18 Posted by: emstr Posted at: 2017-06-28T07:11:41.988Z Reads: 56

```
Thank you! Especially here in New Zealand shipping is $40 USD :frowning: 

I'm loving the community - unless I'm mistaken you're the one who runs Big Kids youtube channel. If so, love the videos and keep up the awesome work!

If not, keep doing you! Thanks for commenting :slight_smile:
```

---
## \#19 Posted by: emstr Posted at: 2017-06-28T07:27:29.696Z Reads: 58

```
Also (sorry to be a nuisance) would this charger work for the 10s Bestech BMS? Spec says 42v, but one would assume it would be smart enough to accept higher volts and only take 42. Could I use the charger? If so, what type of charge port would I need to buy, does anyone know?

<img src="/uploads/db1493/original/3X/0/d/0dbd28f5944fbfaa99a3f9a2396b8a88b946dd2d.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/e/1/e1a5d004cd800e4d67248fe72263e072b5e8d415.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/7/57ed0f6b1f18d5600214a3bf4176d7dbd00b15d6.jpg" width="375" height="500">
```

---
## \#20 Posted by: Namasaki Posted at: 2017-06-28T07:33:20.418Z Reads: 54

```
[quote="emstr, post:17, topic:25661, full:true"]
I'm noticing you have two motors - If I used the 5ah batteries would I get better battery performance with my one singular motor?
[/quote]
A single motor will have to work twice as hard as dual motors. 
If running single I recommend using a 6374 motor and low gearing. Like 15/40
```

---
## \#21 Posted by: Namasaki Posted at: 2017-06-28T07:36:12.505Z Reads: 54

```
[quote="emstr, post:19, topic:25661"]
would this charger work for the 10s Bestech BMS? Spec says 42v
[/quote]
 
You can't use a 54.6v charger to charge 10s. 
You can't even use that charger on 12s
You will definitely need a 42v charger for 10s
```

---
## \#22 Posted by: emstr Posted at: 2017-06-28T07:38:12.509Z Reads: 52

```
Yup I got the 6374 & 16T HTd5 12mm gearing.

So that means the batteries will drain even more than usual? Looks like I might have to do 8ah if I want 20km range
```

---
## \#23 Posted by: emstr Posted at: 2017-06-28T07:40:51.049Z Reads: 54

```
Okay, good to know. Thanks so much. Would you reccomend: https://www.amazon.com/Masione-Adapter-Lithium-Battery-Charger/dp/B06XGGZW22/ref=sr_1_1?ie=UTF8&qid=1498635562&sr=8-1&keywords=42V+2.0ah+Scooter+Lithium+Battery+Charger

With this charge port? https://www.amazon.com/UUShop-Balancing-Electric-Charging-Replacement/dp/B06XSFQK71/ref=sr_1_fkmr0_1?ie=UTF8&qid=1498635621&sr=8-1-fkmr0&keywords=Smart+Balance+Wheel+Charging+Port+Power+Button+Repair+Parts+Hover
```

---
## \#24 Posted by: Namasaki Posted at: 2017-06-28T11:34:41.510Z Reads: 50

```
I have used that brand of charger and it works but the tend to get hot because they don't have a fan. 
I also like the 3-prong charge port.
```

---
## \#25 Posted by: nmagz3 Posted at: 2017-06-28T15:28:55.882Z Reads: 42

```
Thanks man!  Yup that's me.  I don't do anything special compared to the guys in this forum.  I just like creating media.  So I make videos answering questions that I already had from my first build.  Can't wait to see your final build.  It'll be your first but not your final.  Such a great hobby!
```

---

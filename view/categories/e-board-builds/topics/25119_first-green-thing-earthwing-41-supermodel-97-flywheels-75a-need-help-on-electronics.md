# \[First\] Green thing &#124; Earthwing 41&rdquo; Supermodel &#124; 97 Flywheels 75a &#124; Need help on electronics

### Replies: 28 Views: 1842

## \#1 Posted by: karosass1 Posted at: 2017-06-11T17:20:07.170Z Reads: 230

```
After lurking for too long, finally started building my own build. 

For starters I built regular longboard to learn how to ride. Current build is:
<img src="/uploads/db1493/original/3X/e/7/e70556543298a64a428113f62975f595a5243d95.jpg" width="375" height="500">

Earthwing 41" Supermodel Green Stain deck
Caliber I 50 degree trucks (green as well, not seen in picture)
Abec 11 97mm 75a flywheels
First Abec7 Green bearings I could find

Planned parts:

**Battery**: 
Initially was thinking about lipo, but recently changed my mind and will probably go with 18650 using battery holders like this:
http://www.ebay.com/itm/181775746575

For batteries themselves:
https://eu.nkon.nl/samsung-18650-inr18650-25r.html
And I will try making each pack <99Wh, just to have an option of air travel. As much as I calculated, it's 9.25Wh per battery, so 10 batteries per pack connected together? Not sure tho about what pack to go in general tho (10s3p, etc.). The goal is commuter board, dont really care about high speed nor huge hill climb.

**Motor:**
While I would like to have dual (for braking mostly, especially to have some brakes in case one motor fails), I don't have that kind of budget yet. So for now I'm thinking about 6374 192kV 3300W. Or should I go with smaller one and later add a second one? I'm 90kg person just to mention.

**VESC:**
esk8.de one, because of it being europe based, so no additional VAT tax.

**Controller**
Again something I'm not sure about, want something as small as possible and reliable. Nano?

**Questions summed up**

* What am I missing and especially what small things I could order now from chinese on ebay/aliexpress, since I'm starting my actual build at the end of the month, when I get my salary. So that they could actually arrive on time (god bless 1 month delivery time)
* What battery specifications I should go with if I don't really care about big speed/torque/hill climb, am 90 kg person
* Is 6374 too much? Can I go with some smaller motor to which later I could add second identical one to make it dual?

Thanks!
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-11T17:30:22.713Z Reads: 195

```
Don't get 25r - voltage sag is a pain with them. Get 30Q!
battery holders like these are also not well suited for the currents we use.
```

---
## \#3 Posted by: smurf Posted at: 2017-06-11T17:59:17.415Z Reads: 192

```
The 6364 should have enough power and it's possible to use a second one with torque boards extra wide trucks.

diy-electric-skateboard-kits-parts/torqueboards-218mm-trucks/
```

---
## \#4 Posted by: karosass1 Posted at: 2017-06-11T18:10:09.278Z Reads: 179

```
Is it because of the wires? Because I'm fine with resoldering them with stronger ones, or soldering those packs directly (If for example making single pack slim tower looking pack). I just don't want to solder batteries because my soldering iron isn't really powerful and I don't have proper soldering skills imo to solder battery pack without damaging it.

I'm fine with changing the batteries tho. Thanks!
```

---
## \#5 Posted by: karosass1 Posted at: 2017-06-11T18:12:40.468Z Reads: 165

```
They are 218mm, I have 10 inch Calibers, so 254mm, which means I should be ok?
```

---
## \#6 Posted by: Maxid Posted at: 2017-06-11T18:13:25.754Z Reads: 164

```
the springs are used to carry the current and are too thin. also vibrations will cause cells to slide out of their holders eventually if not secured properly.
```

---
## \#7 Posted by: Maxid Posted at: 2017-06-11T18:14:14.438Z Reads: 156

```
the 218 are NOT from end of axle to end of axle but the hanger width AFAIK.
```

---
## \#8 Posted by: karosass1 Posted at: 2017-06-11T18:17:54.883Z Reads: 155

```
Oh right, in torque's description they write that "The truck profile is similar to Caliber but slightly bigger by 1mm.". As much as i understand profile == width, so i still pretty much should be ok?

On other note:
Are there any other cheap battery holders that would be good enough for the this current, or should I just get proper soldering iron?
```

---
## \#9 Posted by: anorak234 Posted at: 2017-06-11T18:32:23.244Z Reads: 145

```
Get a spotwelder
```

---
## \#10 Posted by: karosass1 Posted at: 2017-06-11T18:49:48.799Z Reads: 140

```
Expensive one use item. I'd rather get a good powerful soldering iron
```

---
## \#11 Posted by: smurf Posted at: 2017-06-11T18:55:32.809Z Reads: 138

```
Someone said nkon.nl will weld up battery packs. I think having a battery professionally welded is money well spent.
```

---
## \#12 Posted by: karosass1 Posted at: 2017-06-11T19:55:56.458Z Reads: 131

```
This is something new, can't really find this info on their site, will try writing their support. Thanks
```

---
## \#13 Posted by: Stef Posted at: 2017-06-12T00:08:24.164Z Reads: 128

```
If youre going for a dual drive, now or later, 2x 6355 is a LOT of power at 10S. I have 2x 6355 at 10S and I literally cant go full throttle because the board just shoots away from under my feet. 

If you start with one 6355 then you'll probably be fine on small slopes but maybe not on steep hills.

I use VESCX (now 'FOCBOX') which I highly recommend, having the ability to do FOC without to much risk is great, The housing also makes it a bit more foolproof against accidental shorts.

Also, going sensored is definitely worthwhile imo.
```

---
## \#14 Posted by: karosass1 Posted at: 2017-06-12T09:30:35.523Z Reads: 120

```
While I would like enertion focbox, it's a bit out of my price range (200$ + 25% Vat tax + 20$ item check cost). I will probably go with Esk8.de VESC 4.12(150 eur) since it's Europe based. It supports foc as well, but they say it's experimental and still in development so 'use at your own risk' .
```

---
## \#15 Posted by: Jebe Posted at: 2017-06-12T10:19:37.722Z Reads: 110

```
why do you want to use foc?
BLDC is great
```

---
## \#16 Posted by: karosass1 Posted at: 2017-06-12T11:01:10.087Z Reads: 113

```
I don't, I just like having options. I mean FOC is as much as I understand is more efficient, but not as reliable yet? Anyways as mentioned I'm planning on esk8.de vesc, unless I find cheaper reliable option that is europe based.
```

---
## \#17 Posted by: Vaulter92 Posted at: 2017-06-12T14:01:43.843Z Reads: 116

```
If you do not want to spot weld the batteries check this recent post...
http://www.electric-skateboard.builders/t/battery-packs-no-spot-welder-or-solder-required/25135
```

---
## \#18 Posted by: karosass1 Posted at: 2017-06-12T21:07:00.568Z Reads: 105

```
For anyone else interested about nkon.nl pre-welding pack - I asked them about it and how much additionally would it cost to the battery price for pre-welding it (30 batteries), their response:

''Hi,

About 40 euro for the welding I estimate, depends on exact requirements.

Regards,
Arjan''
```

---
## \#19 Posted by: arussellsaw Posted at: 2017-06-12T21:54:28.289Z Reads: 99

```
i did the same thing today and had the same quote, i think i will probably end up doing this when i order my cells
```

---
## \#20 Posted by: karosass1 Posted at: 2017-06-30T07:51:35.298Z Reads: 90

```
Finally got mechanical kit from ebay, seemed fine, except for in motor mount the hole to put on the truck is round, while my truck is square. So I ended up doing terrible thing -> made my truck rounder. Looks horrible, but didnt want to order another mount, not sure even if I could find one that would fit. Anyways my truck costs almost as much as motor mount so in worst case I will just get a new truck.

It's a salary day as well, so I will finally start ordering main components. And once again I started to wonder again whether I should go with lipo or lion. ~140 EUR for a battery seems kind of a lot (lion 10s3p 30Q) while I could simply get 2 lipos like this https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html and get 10s. Of course there's the bursting in fire thing and less recharges.

I'm still thinking about solderless battery pack with 18650, I just received battery holders that I forgot I ordered, which look like these:
http://img.dxcdn.com/productimages/sku_292672_1.jpg

While they don't have springs, they say its for 3.2-7.4V, so 2S only? But what could go wrong, the contacts seem big enough, at least bigger than springs on the previously mentioned ones.

+ Are SK3 motors from HobbyKing sensored? Should I just get it there or get ~50% more expensive one in esk8 related eshop (esk8.de/aliensystems)?

Edit: I totally forgot about range.. ~10s1p lipo would have only about ~6 miles? While 10s3p lion would have ~16. So probably will end up with 18650s.
```

---
## \#21 Posted by: karosass1 Posted at: 2017-07-08T17:36:03.728Z Reads: 77

```
Lesson learned - before buying shady ebay mechanical kits, check if they will fit the truck and in general consider their lack of quality, here's how it went for me:
Received motor mount:

<img src="/uploads/db1493/original/3X/0/0/00dff6d950c198b2ec72549eb9aa2d916f05ec21.jpg" width="281" height="500">

Notice how the hole for a truck is round and not adjustable. And now take a look at my truck, notice the problem? :expressionless:
(The mount was specifically said to be designed for 63 motors)

<img src="/uploads/db1493/original/3X/6/8/683f3b7d6f67ecdc91a3a43b9e3d9ea50e93e63c.jpg" width="690" height="388">

I had 2 choices pretty much - either get other mount or... commit a sin..
<img src="/uploads/db1493/original/3X/f/8/f8af6dac2590c4ce92c32552f68fc28fb56ec050.jpg" width="281" height="499">

Yeah...

But that's not where the problems stop.Tried checking how all the 'transmission' will fit together:<img src="/uploads/db1493/original/3X/5/0/50dba14d96c19aa466e4327541be4d43cea249ee.jpg" width="281" height="499">

I stretched included belt as much as I could here and it still was quite far away from the holes to mount the motor on...

So I will have to go with even hackier way and make new holes to mount the motor.
And I don't like the fact that there's only 2 holes for mounting the motor, seems like not enough to confidently hold the motor.

Well on other hand I saved quite a bit of money (35$ for full mechanical kit with a belt)
```

---
## \#22 Posted by: JLabs Posted at: 2017-07-08T17:56:21.276Z Reads: 72

```
Or you could get a longer belt..
```

---
## \#23 Posted by: karosass1 Posted at: 2017-07-08T19:32:07.588Z Reads: 70

```
Doesn't change the part about not being comfortable mounting 1.4kg motor with 2 screws that are barely 3mm wide.

But the point is that this is a mechanical kit, not separate parts bought from different vendors, so it should fit, but I guess these chinese ebay sellers don't do any QA at all.
```

---
## \#24 Posted by: TranxFu Posted at: 2017-07-08T20:01:24.586Z Reads: 64

```
I think the one at fault here is you. I've seen that kit on AliExpress and ebay a couple of times. There were dimensions and different perspectives on the mount on each listing... If you have a caliber truck get a mount for a caliber truck. Anyone could've seen that it wouldn't fit without even measuring... As well as the design issues you mentioned. 

Point is: don't go cheap on parts and blame the seller afterwards...

EDIT to not make this a rant: If you've settled for that mount. Get some longer grub screws and drill into the truck and tap them. I have a colleague which is using that same mount and he never got them to sit tight and stable without doing that.
```

---
## \#25 Posted by: karosass1 Posted at: 2017-07-08T20:15:15.175Z Reads: 60

```
I'm not blaming seller on misfit for my truck part, in my first sentence I say that I learned a lesson to not order stuff without checking by which I mean it's my mistake. I'm blaming seller on belt having wrong length. But yeah, I will make this work. What I'm planning to do is to make 4 new holes on motor mount, use longer screws and probably nuts inside the motor so that vibration wouldn't shake screws out after a while.
```

---
## \#26 Posted by: lrdesigns Posted at: 2017-07-14T03:27:18.858Z Reads: 53

```
These mounts are notorious for working their way loose from the truck. Once you find the perfect alignment after a few test rides you need to epoxy around where it attaches to the truck. This prevents the torque of the motor wiggling the mount back and forth ever so slightly till it comes loose.  After you do this it can be a decent mount. They are made from a fairly hard stainless so drilling them might not be easy. 

Preferably use the grey colored type for metal like JB weld or similar. 
http://www.ebay.com/itm/J-B-Weld-Original-Cold-Weld-Formula-Steel-Reinforced-Two-Part-Epoxy-3960-psi-/302119967592?hash=item4657c0db68:g:xDIAAOSwImRYEXlk
```

---
## \#27 Posted by: karosass1 Posted at: 2017-07-14T06:46:56.726Z Reads: 51

```
Thanks! I noticed the part about drilling being hard, battery powered drill was miserable at it, thankfully friend has drill press at work and it managed to do it. And your post kind of confirmed my suspicion that couple of screws screwed into the truck won't be enough to hold mount in place long term.
```

---
## \#28 Posted by: karosass1 Posted at: 2017-07-14T13:41:01.190Z Reads: 50

```
Another minor problem
<img src="/uploads/db1493/original/3X/3/8/38d87e3259e7d7676e1e57f93174d892cc41e75a.jpg" width="690" height="388">
Left is female connector I had and intended to use as charging jack, right is male connector from my new 42V power brick. 
While they look similar, the hole inside male one is slightly too small to fit. 

So I guess I will solder xt90 on it instead and use that for charging. (I'm just assuming charger has only positive and negative wires, and nothing additional) 

Still waiting for battery, bms, VESC :)
```

---

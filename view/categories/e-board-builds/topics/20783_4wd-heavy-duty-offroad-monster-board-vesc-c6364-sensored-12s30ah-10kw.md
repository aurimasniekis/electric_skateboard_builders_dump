# 4WD Heavy Duty Offroad Monster Board - VESC, c6364 sensored, 12S30Ah, 10kW

### Replies: 62 Views: 13023

## \#1 Posted by: Duffman Posted at: 2017-04-11T09:12:28.188Z Reads: 949

```
Finally here is the buildlog of my 4WD heavy duty offroad monster board.

As always, all 3D-data is available at Thingiverse: http://www.thingiverse.com/thing:1900477

This is what I'm talking about:

<img src="/uploads/db1493/original/3X/7/7/77e383309dcd3957a0ef2e5723636cc766c2502e.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/1/c/1c8b6620dd9a75b2e53641d12aae740dafaaa888.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/5/e/5e26ae4eccf9ed33a0f6f74365770e68381af1a0.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/3/632d2cf608ce82fb348564c0dde2e9e9669df5f8.jpg" width="690" height="388">


The current setup is:

Next Redux Deck
MBS Matrix Trucks
MBS F5 Bindings + FX Pro II Heel Straps
4x Mefo Ice Slider 11x4,50-5 on 125mm Gokart rims
4x VESC 4.7 modified with heatsinks, 0,5mOhm shunts, extra TVS diodes and lots of caps
4x c6364 with internal hall sensors
2-stage 8:1 - ISO-04 chain reduction
32W LED headlight
12s30Ah lipo (10Ah+10Ah+10Ah packs)
3D-Printed NRF Hand Controller (http://www.electric-skateboard.builders/t/vesc-nrf-hand-controller/16212)

Just the right toy if you want to have fun when you want to go really offroad:

https://www.youtube.com/watch?v=7bQtSXBECRY&t=12s
https://www.youtube.com/watch?v=1zK5Ij2xajM&t=1s
https://www.youtube.com/watch?v=bsXjOlEDBRA
https://www.youtube.com/watch?v=5OL1wXB8DbY
https://www.youtube.com/watch?v=UxpQMWbrWwg&t=5s
https://www.youtube.com/watch?v=91NqHfn0nbw&t=2s
https://www.youtube.com/watch?v=jEyQMHNaoKc
https://www.youtube.com/watch?v=y6vFfcoDARQ
https://www.youtube.com/watch?v=nYPRy8Zqvp0&t=7s
https://www.youtube.com/watch?v=wYgjUt7ua_E&t=17s

But let's go back to 2015 when everything started:
```

---
## \#2 Posted by: lrdesigns Posted at: 2017-04-11T09:35:49.521Z Reads: 725

```
I imagine people on mars getting around on these things. Its funny how the board makes those motors look small.
```

---
## \#3 Posted by: Duffman Posted at: 2017-04-11T09:57:09.601Z Reads: 731

```
Infected by the eSk8-Virus I wanted to build my own unique board.

When I started this project, the first designs of the VESC were released but not commercially available.
So I had to order the PCBs somewhere in Hong Kong and a bunch of electronic parts from mouser and to assemble my VESCs by myself:

<img src="/uploads/db1493/original/3X/d/0/d0385d534a33e2cc84ae0cc86db3171ed82726b3.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/a/e/aef09bdb2361952109c67db516ad3248da1b1d6b.jpg" width="345" height="194">

I bought a cheap, used MBS Pro90 board of ebay and some MBS Matrix trucks. Unfortunately the board has only 20 degree tip angle so I had to use angled wedges to get good steering capabilities.

As my intend was to go really off road, the 'normal' mountainboard tires seemed too small and I decided to use 10" mini quad tires:

<img src="/uploads/db1493/original/3X/8/a/8acb20a91f50583f53418306b33be0fe10e1d9f7.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/8/6/86d490dbc6a4f52e26666e5c52950f25f09a99f6.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/c/0/c018913392d692a29ddc99cd93d9fe4237405e8b.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/5/2/52f0d8f799e5405a7731770b20b783117bbe756a.jpg" width="345" height="194">

Because I tried to build this beast as light as possible I started with quite small Hobbyking NTM-5060 motors. Of the box they have way too high 270kv so i had to reconnect them to WYE resulting in 155kv. To get the desired 40kmh with those big tires I needed a reduction of 8:1 which was easier to archive with a 2-stage chain reduction held together by laser cut aluminium sheets.

<img src="/uploads/db1493/original/3X/7/1/71d41cd2c0f7fbf361de1b8bbd4988c9f1dd1f7d.jpg" width="602" height="500">

<img src="/uploads/db1493/original/3X/e/2/e2d3b4b7b5958835e2586d876de218a1ed03afcc.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/2/c/2c9a696df727d3e10e324d1fc493cde9a32b2e52.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/2/f/2f09216fe0cf63f6548ac22f9e1ccfcc313173ad.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/a/8/a874e1ca94d3e2511601bb6f2734e3025a8cc03d.jpg" width="345" height="194">
```

---
## \#4 Posted by: Duffman Posted at: 2017-04-11T10:49:14.670Z Reads: 670

```
@lrdesigns: It has been called Lunar Rover before... http://www.elektro-skateboard.de/forum/showpost.php?p=34922&postcount=51

----------

To connect 6x 4s5Ah lipos to 12s10Ah I made a power distribution board with included lipo alarms and loop key:

 <img src="/uploads/db1493/original/3X/2/e/2e662e186522b0675a6dc44827523300297f3af9.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/6/3/639671acabd9f2e25ef45b1b070b44918e7c9734.jpg" width="345" height="194">

That is what you get if you let your friends ride...:joy:

<img src="/uploads/db1493/original/3X/e/b/ebdfa13d4f25b6668fc1c74d10d7739b1653989b.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/6/1/613b3cefe35eef03175dd68e97135593a6312715.jpg" width="345" height="194">

----------


This was the first rideable version in 2015:

<img src="/uploads/db1493/original/3X/2/7/2736de679d247a70e039a08e3f3c77229e7d260e.jpg" width="690" height="388">

Took it to the German eSK8 Championship https://www.esk8b-dtm.de/?language=en but even if the track looks like a desert and the board looks like escaped from Mad Max the smaller boards were better to handle on this course:

<img src="/uploads/db1493/original/3X/a/d/ad2db4c88037423c83586708710f17c977141f2c.jpg" width="690" height="460">
<img src="/uploads/db1493/original/3X/c/d/cd56f4b9bbd28878f65b2f3fcf8194bc1fc3d884.jpg" width="690" height="303"><img src="/uploads/db1493/original/3X/e/5/e5a959110584e9db2c84adb3e06bf1dc621cfb5a.jpg" width="667" height="500">


Always wear a helmet!!! (at least the guy behind the camera did...)
<img src="/uploads/db1493/original/3X/4/d/4d6e3a0374142aaa4b6e2cea45a14605556ec501.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/d/3/d3ff9e405bf9bf76baf158f53de6b6c739b76350.jpg" width="345" height="194">
```

---
## \#5 Posted by: Duffman Posted at: 2017-04-11T13:02:45.431Z Reads: 653

```
One of the first improvements was to get rid of those crappy voltage based battery meters. Instead I'm using this coulometer until now without any issues:

<img src="/uploads/db1493/original/3X/5/3/5368617ec2d876b6936fbb40dc4b2a7d33af9277.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/d/e/deabe0b4af08f8a28406db25c142ea37ed53e2af.jpg" width="345" height="194">

It can be programmed to any battery capacity and to different shunt resistors to match almost any setup. It sits together with a bicycle speedometer in a 3d printed case on top of the VESC enclosure:

<img src="/uploads/db1493/original/3X/c/8/c8612bd7cdb25390690df0f0bb4d9df3893cec30.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/c/1/c1b20a7a9528c8d8dd0806c70f18abef6a6f31ab.jpg" width="345" height="194">

<img src="/uploads/db1493/original/3X/2/a/2a2b2dee402df985f02763737d3067b320b89765.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/d/1/d1362b2f964d55c7588ea4027440ca997087ffae.jpg" width="345" height="194">


The next big improvement was to switch to sensored. Therefore I used 3d printed housings for the hall sensors:

<img src="/uploads/db1493/original/3X/3/4/349dd6e72d6a2641def69eafd77fbe0281e8ad88.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/f/5/f5d9ae6b89a93510da9b67aa9d0ef7c598bd0031.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/5/f/5fbb3b45f4046ef995de2b8616cd1793ead20cc4.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/a/1/a100e67d8cbd4e398e4cecc2c32a1f5a6906e48d.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/3/b/3b31aec0af753486ad7e40c67c1d3272d6d39a24.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/9/c/9c2904ffb4c1ad33881e60382309cf8179e78996.jpg" width="345" height="194">

The holders sit on the motor holding plate and can be adjusted to the optimal position:

<img src="/uploads/db1493/original/3X/a/7/a780518bbce2bbd8bcf0f8b3aae5d6bc6b97b0b9.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/0/d/0deca8a72586c4cd99426494eb457f6658ee3585.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/b/7/b7f63a83deda5fc100ae09ec5734575fb9c9b73b.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/c/a/cae2919059674d77e041888288923140703701d7.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/7/d/7d0ac25061d61723cbb535dec32c43ba1ec9587f.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/f/a/fa9766cbcc365d075fca8eab30a0706c2cc60cd9.jpg" width="345" height="194">
```

---
## \#6 Posted by: Duffman Posted at: 2017-04-12T08:19:53.978Z Reads: 616

```
After two sets of tires in maybe 5 months, I had to look for a new type of tires because those mini quad tires are really CRAP:

<img src="/uploads/db1493/original/3X/5/3/535f8b673af6b7e1e5f75264b2d2448abe393824.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/4/5/45c30996625e0464c5d70f43b4f258a788f2d24f.jpg" width="345" height="194">
<img src="/uploads/db1493/original/3X/e/b/eb78cde78619c3a9af3e7998b2e84d7483b2b5f8.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/1/9/19736154ed7f90002a9db84ad0096574309b283b.jpg" width="345" height="194">

I tried to find something in a similar size but had no success and had to go for the bigger and heavier Mefo 11-4.5-5  - gocart snow tire:

<img src="/uploads/db1493/original/3X/9/6/96cc6862ed3dd849e698fe17f38af26788a9169c.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/c/7/c79a42045acdeb9c4f2dc26e4cc228d03d368739.jpg" width="345" height="194">

<img src="/uploads/db1493/original/3X/5/b/5b47e6ebd9a338418d89d61d6de08407e1d4f1cc.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/7/e/7e19a20f6bb06928c24026567f4c5addb2e048e3.jpg" width="345" height="194">

To fit these tires on my Matrix trucks I had to machine some custom rim adapters out of aluminium:

<img src="/uploads/db1493/original/3X/b/1/b1a8c7ba92a1dd7158fba2d94523a83d087ae297.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/d/d/ddc9d02c392a90b990a5d924bdd53692f2b89d82.jpg" width="345" height="194">

<img src="/uploads/db1493/original/3X/d/3/d3f8ceba1e36888e823612fa8e3537a2aa5d928b.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/a/d/ad52e14e8268376f55450889130bec370bc02ec9.jpg" width="345" height="194">

After this mod the board started looking like a monster:

<img src="/uploads/db1493/original/3X/b/b/bba1ed4e657ec77cb23e7c9f7a5f579a600e3c63.jpg" width="690" height="388">
```

---
## \#7 Posted by: Okami Posted at: 2017-04-12T11:40:13.020Z Reads: 571

```
@Duffman  Wanted to comment ''Destroyer of tires'' .. but then I saw the picture with the crappy tire, so yeh, they were probably not of the highest quality.. too bad you had to remake the rims for the new tires to fit.
```

---
## \#8 Posted by: onloop Posted at: 2017-04-12T12:31:35.938Z Reads: 570

```

Congrats on the amazing build, You are seriously a fucking legend brother! this is an amazing build! Made my day :slight_smile:
```

---
## \#9 Posted by: Duffman Posted at: 2017-04-12T12:54:28.103Z Reads: 558

```
Thank you! But this was only the beginning. I have made a lot more optimizations which I will share as soon as I find the time...
```

---
## \#10 Posted by: onloop Posted at: 2017-04-12T12:56:01.973Z Reads: 553

```

its amazing what those little ntm 5060 prop drives can do :)
```

---
## \#11 Posted by: Duffman Posted at: 2017-04-12T13:45:34.190Z Reads: 546

```
Yes, the power output of 4 NTM5060 was already impressive, but if you were drawing high power for a longer time, like riding in snow or loose sand, they got veeery hot.

Later I switched to c6364 motors and beefed up my VESCs. This almost doubled the power output...
```

---
## \#12 Posted by: Trdolan03 Posted at: 2017-04-17T05:50:51.122Z Reads: 535

```
@Duffman
Is it possible to show some pictures of your vesc's after modification?
```

---
## \#13 Posted by: Duffman Posted at: 2017-04-19T13:59:19.153Z Reads: 537

```
Luckily (for you) I had to open my VESC enclosure yesterday, because I had some connection issues with one of my hall sensor plugs.

Cable tension relive:
<img src="/uploads/db1493/original/3X/0/a/0ab4ee8e3985c7c3107059febf0ee702e6da093b.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/3/0/307483acfe20b68c62b88a776101041a24f89005.jpg" width="345" height="194">

NRF Transceiver & BT Module and 14 ultra low ESR caps:
<img src="/uploads/db1493/original/3X/2/b/2ba8999bb4fbbe790c3006be8525592ecf28bded.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/5/2/525d5eb34a8aace13a2988acf31e559ed7d9e4f4.jpg" width="281" height="500">

6mm bullet connectors for the VESCs:
<img src="/uploads/db1493/original/3X/d/b/dbf9f42674e19ef0147066d1acd94c32a982092d.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/b/6/b67e980a5636dd4576597ecd8cdc5df0be460331.jpg" width="345" height="194">

Microswitches to add the possibility to disconnect every single VESC in case of a fault from the CAN bus:
<img src="/uploads/db1493/original/3X/c/a/caace137a975770196dae313bc53e78fff2b7f7d.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/9/5/951c8db2c3a8153c1f383f96ea184edc55b8f024.jpg" width="345" height="194">

20µF on GVDD, 0,0005 Ohm shunts for up to 240A current measuring ability, NRF extension and BT directly soldered to the PCB:
<img src="/uploads/db1493/original/3X/6/7/67526ab84aa46fb9adb324e56ae64b3f2d20027f.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/d/e/dec10549023c79e4d381d98de969571e82b46150.jpg" width="345" height="194">

VESC with heatspreader soldered to the common positive FET connections, 54V TVS diode on top of of the big ceramic cap. Hard to see under the heatspreader: 
<img src="/uploads/db1493/original/3X/4/b/4bc55dbb1817a8557cfd5eee6d6a05ac870ebf26.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/b/8/b84326b5baa98098692d9a6559e4f00ad7265d5e.jpg" width="281" height="500">
```

---
## \#14 Posted by: monkey32 Posted at: 2017-04-19T14:20:44.281Z Reads: 489

```
<img src="/uploads/db1493/original/3X/3/0/308503d62cf907b839774ddfb2cf5cb99c7c9408.jpg" width="504" height="354">
```

---
## \#15 Posted by: Trdolan03 Posted at: 2017-04-19T14:32:46.595Z Reads: 481

```
@Duffman Thanks for those. Your build is a beast.
```

---
## \#16 Posted by: Duffman Posted at: 2017-04-19T15:31:45.512Z Reads: 494

```
https://youtu.be/VUQ_XAvSJqc
```

---
## \#17 Posted by: Okami Posted at: 2017-04-19T15:36:04.622Z Reads: 486

```
@Duffman  You should estimate the value of your build.. im sure it would grab the first places and would be the king of emtb's ;) :D
 :crown:

Your capacitor ''booster pack'' also looks incredible..

So how many micro farads of caps do you have per one vesc?
```

---
## \#18 Posted by: michichopf Posted at: 2017-04-19T18:39:19.092Z Reads: 477

```
Jeesus, this beast is the stuff of dreams. I never thought I would want a mountain e-board. After riding one for 5 minutes and seeing your stuff my bank accaunt is going do die (after its alive in the first place :) )
```

---
## \#19 Posted by: Mobutusan Posted at: 2017-04-19T22:31:31.510Z Reads: 474

```
I'd like to officially cast my vote for @duffman for Build Overkill Of The Year (BOOTY award) in 2017, based on posting date, at least. I know this build is actually much older, but who cares? BEEFCAKE!!
```

---
## \#20 Posted by: Duffman Posted at: 2017-04-20T11:48:55.606Z Reads: 502

```
@Okami The total cost of this build was somewhere between 4-5k€. Hard to tell with this constant rebuilding and improving, don't really want to know exactly... :money_mouth:

I have a total of 28x 680µF caps. 7 per VESC, so 4760µF instead of 2040µF. But much more important is that each of them has less then the half esr than the stock caps, in common 5 times better. So hopefully less voltage spikes from switching at high currents.

@Mobutusan BOOTY sounds good ;-)

But back to the buildlog, I still have a lot of things to show you in detail:

The first testride with the new big tires was a lot of fun, but they were throwing so much dirt at me that I had to build fenders. Therefore I had the mounting plates cut from 4mm Alu and the fenders from 2mm Alu and bent to shape:

<img src="/uploads/db1493/original/3X/a/2/a27e8eb7d7cbe6eb30a089a493054ce05ec180e7.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/2/7/2729eb631643105fce950b559ea5e40129263226.jpg" width="345" height="194">

The two parts were riveted together and bolted to the gear housing:
<img src="/uploads/db1493/original/3X/7/8/786b31abce843c91ab360469c20e524632f6f3dc.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/7/d/7d60cb67638429ac56f0ed387b8d45fd35ffd0ed.jpg" width="345" height="194">

Spray painted and mounted:
<img src="/uploads/db1493/original/3X/f/d/fde18f331a6db1100bce7863f6c672099eb445cb.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/9/c/9c8a311d55c8a8b6b71cbe980bcb1e3bf3e9003c.jpg" width="345" height="194">

Additionally I finally printed the cover pieces for the gear housing:
<img src="/uploads/db1493/original/3X/c/2/c21e88fb216cf7493191ef5cc95e876ed80c0253.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/e/5/e5dcfe20a2069adfcb62bf9821eac25bbf31f802.jpg" width="345" height="194">

Completed:
<img src="/uploads/db1493/original/3X/2/a/2ab3a7e54dc0b2b3071403a41da082847ac97dcc.jpg" width="690" height="388">
```

---
## \#21 Posted by: Duffman Posted at: 2017-04-21T11:30:24.173Z Reads: 487

```
I rode around 500km offroad over the summer 2015, when fall came and the days got shorter and darker I had to build a proper headlight. Before I had done some experiments with flashlights but was never satisfied because there was always too much light directly in front of me and always to less light in the far field and in the corners. I found the perfect solution in a 32W (105 lm/W) high power LED strip in combination with a cylindrical lens. 

High Power LED Strip: http://www.leds.de/en/LED-strips-modules-oxid-oxid-oxid-oxid-oxid/High-power-LED-strips/SmartArray-L25-150W-25-LEDs-neutral-white.html

Datasheet: http://www.leds.de/out/media/Datenblatt_SmartArray_2014_V11_ENG(3).pdf

LED Strip Optics: http://www.carclo-optics.com/optic-12750-300mm?opticfamily=strip%20optic

This produces a oval shaped spot, wide in horizontal direction and narrow in vertical direction:
<img src="/uploads/db1493/original/3X/2/5/257fa0935c8b983763874c6e1057171a723d6aad.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/e/6/e60b4dd86a0e0b1abbc3165b0e61c99fefd2a4db.jpg" width="345" height="194">

The LED strip and the lens are held by a housing stacked out of laser cut aluminium sheets:
<img src="/uploads/db1493/original/3X/a/1/a1c0d28fde5a1d16423b9b15ed8ae40ff055e176.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/7/e/7e628ea64072ee1e4f16f16e365a5bf021ba4b82.jpg" width="281" height="500">

The two different parts in 1mm and 3mm thickness are alternating stacked to produce a housing with heatsink fins:
<img src="/uploads/db1493/original/3X/3/d/3d2970740c053f7334987667cea998904bb0b00f.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/d/3/d368043af4b25d632d17e5e91afd4cc5c5cd9906.jpg" width="345" height="194">

The stack is held together by M4 threaded rods and Locktite:
<img src="/uploads/db1493/original/3X/9/c/9c7d0db7b424f0d26e9e2e82104a7984c18974ac.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/c/b/cb845cba7d75074a8ee328ac0264d2fb9fac334a.jpg" width="281" height="500">

The LED strip is sitting in a milled slot:
<img src="/uploads/db1493/original/3X/4/a/4acbca56da5082338d2bf0b00154959dc50d4ebe.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/b/4/b4ad65a070cba88eca4b2ffb9670130453059c5b.jpg" width="345" height="194">

Completed housing with LED, lens and wires:
<img src="/uploads/db1493/original/3X/e/d/ed07ccc9dd6860ce37ebbbb18b29c217388fdf35.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/9/9/993a871fa9834094ea97c0f58a9f39b1b88551d0.jpg" width="281" height="500">

The spot has some chromatic aberrations but normally you don't see them, only when pointing on a wall:
<img src="/uploads/db1493/original/3X/4/1/41e4bcee43d843e4676e019a7a26c3e857c7e56d.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/9/9/991af8b29731e90bfadea42854a6101c12b38748.jpg" width="345" height="194">

The 32W LED puts out a huge amount of light. It is sold to replace a 150W halogen tube:
<img src="/uploads/db1493/original/3X/3/a/3a831ae9bfa4ba1609d2190cfcde4bb0d26e6d86.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/5/e/5e15e2ead96e92f313a925dec26375236781a2f9.jpg" width="345" height="194">

The LED housing is mounted on the12mm stabilization rods which connect the front motor holding plates:
<img src="/uploads/db1493/original/3X/4/1/4135ed8b9c91d0daf4da512df1562a6c0cead777.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/e/8/e8c12af5b15bce0caf4e6fc97726dba0b66b8e2c.jpg" width="345" height="194">

To power the LED I'm using a Meanwell LDD-1000HW - a current regulated 1000mA 56V step down regulator which is located in my 'cockpit' (black brick in the lower left corner of the last pic):
<img src="/uploads/db1493/original/3X/0/f/0f250f8a0b923c416ea19a35356ab8c42b06439a.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/9/f/9f69a74b5032f7bf4ccb2cc56023c2c08ab22a9e.jpg" width="345" height="194">
```

---
## \#22 Posted by: Okami Posted at: 2017-04-21T14:10:26.690Z Reads: 449

```
Insane light, man!

**@Duffman do you by any chance know how much lumens/watts Cree XM-L leds produce (commonly used now for flashlights)?**

Edit: <img src="/uploads/db1493/original/3X/c/d/cd0877bf6ae05be7832be09b9aad747d81f0e2de.png" width="690" height="218">

Ok, so at max it looks like they produce 10W of light, some of which probably gets eaten away by reflector or lens, if one is used.. so we would need at least 2-3 such Leds, to attain the same brightness level / power output as you got for your lights :)

----
They are now included in a lot of headlight lights but im not 100% sure at what power levels they are driven by the circuitry inside of these lights.

----
So far one of these lights (with 1x Xm-L cree led chip) have been good enough for me along with ''Zoom'' lens Im having for my headlight. 

But to be honest, now I think 2-3x of these chips at the power level I am getting, would give way better riding for trails/tracks in the dark!

The headlight can take up 2x 18650 but they are connected there in parallel and increases brightness only a little bit when 2x 18650's are inserted, instead of one.

I've also heard there is the XM-L2 led chip out but im not sure which lights offer it and which not.

----
If someone missed it, then my headlight has 1x XM-L chip, while there are models out there now which offer 2 or even 3x of these chips in one headlight. 

For off-road this is somewhat a quick solution as you dont have to install the light directly on the board, has seperate battery box and u get light in which direction you are looking at.

----
Though, im sure @Duffman has way more light for his big board than one or maybe even two of these XML chips can offer :) 

Also I apologize for sidetracking everything but Im just appreciating how much work @Duffman put into creating a housing/sink for these lights, too! :D 

So yeh for offroad and riding in darkness a good light is a must.. unless someone ones to hit a pothole, huge stick or something else while riding!
```

---
## \#23 Posted by: Mobutusan Posted at: 2017-04-21T15:30:05.472Z Reads: 398

```
Amazing work, yet again. This thing is like a 7 layer burrito of DIY goodness. Do you mind if I ask what you do for a living?
```

---
## \#24 Posted by: mmaner Posted at: 2017-04-21T15:31:48.302Z Reads: 408

```
[quote="Mobutusan, post:23, topic:20783"]
Do you mind if I ask what you do for a living?
[/quote]

Im gonna guess he is a professional lottery winner with degrees in physics, mechanical & electrical engineering and a red phone to Thor :slight_smile:
```

---
## \#25 Posted by: Duffman Posted at: 2017-04-24T06:48:08.688Z Reads: 410

```
@Okami I edited my post above with the links to the LED and optics.

According to the datasheet the strip produces 3283 Lumen at 32W power and 85°C temperature, which results in 103 lm/W. 
3 XM-L @10W each would produce almost the same, but usually they are driven at much lower power levels (3W) to get better efficiency.

@Mobutusan and @mmaner Unfortunately no lottery winner but mechanical engineer, doing CAD modeling of plastic injection moulds for 10 years and expensive hobbys like building drones, building cncs, building 3D printers and of course esk8ting ;-)
```

---
## \#26 Posted by: Jebe Posted at: 2017-04-24T06:58:29.197Z Reads: 406

```
Take ALL my money !
```

---
## \#27 Posted by: Duffman Posted at: 2017-04-24T13:17:54.596Z Reads: 448

```
Back to my 7 layer burrito ;-):

Because the new tires are gocart winter tires and can officially be equipped with spikes I simply had to try it and bought a 1000pcs set of 'screw in spikes':

<img src="/uploads/db1493/original/3X/0/0/008aa1a5cb579c7d5058f1c2782ebceff4336f5c.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/a/6/a61911b97bcea36cf3910003e42d6cd9e0de8f27.jpg" width="345" height="194">

Each tire can take 132 spikes, at 4 tires this means screwing in 528 spikes and takes about 2 hours:
<img src="/uploads/db1493/original/3X/0/1/0174b6e0d9358e2dad574daeca25c2724c47ee2c.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/0/e/0efbb6e24f7115839c86f1499cd11512ff577758.jpg" width="345" height="194">

Ready to ride:
<img src="/uploads/db1493/original/3X/c/9/c9b83742d29683adf3390a834b5e80f004f18457.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/e/8/e8a87670be1fe7f79cd5aaa8820044b931ae6d75.jpg" width="345" height="194">

After a short testride:
<img src="/uploads/db1493/original/3X/c/e/ce5a03d92d1044e4effa64e69933f7e9d151b3e0.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/6/7/67bf6d21e22a228dfd3e3faf89a924cafb8944a1.jpg" width="345" height="194">

<img src="/uploads/db1493/original/3X/c/2/c202a714bf5bb0d246c0e5243db32cdf373a0973.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/d/0/d0282bbaca103f22efcd9ba6cb44ebf71910491b.jpg" width="281" height="500">

After a real ride:
<img src="/uploads/db1493/original/3X/9/8/9887ceddb6d730fa86e6f9ea8e4ce6b2652f98f0.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/5/9/593667a88b758f27c2302c2dfa8d180e61b7f19f.jpg" width="345" height="194">

In 2015 we had 2 weeks of snow (and 2 weeks of fun!!!), afterwards I simply screwed the spikes out and was ready for spring again. Unfortunately we had no snow in winter 2016 so I couldn't use them again...:
<img src="/uploads/db1493/original/3X/4/8/480b545f31c2940ab356c33e527d424d116a731c.jpg" width="345" height="194"><img src="/uploads/db1493/original/3X/7/1/7162b8a39b55c30db024102d380fbc523e0903e5.jpg" width="345" height="194">

This was (for reference) a testride without spikes:
https://www.youtube.com/watch?v=wYgjUt7ua_E&t=17s

And this are some rides with spikes:
https://www.youtube.com/watch?v=nYPRy8Zqvp0&t=34s
```

---
## \#28 Posted by: DanSkates Posted at: 2017-04-24T13:49:38.111Z Reads: 406

```
Incredible!  Now that's REAL test right there!  Loving your work :wink:
```

---
## \#29 Posted by: ieatflys Posted at: 2017-04-27T23:10:17.829Z Reads: 417

```
@duffman i have a question or two for you if you dont mind..  im building a similar ish setup for street shredding that mite see offroad once or twice....    
  what made you decide to run such a large capacitor bank did you choose values for a specific reason or did you just fit what you could to avoid voltage sag so you wouldnt have issues with your vescs blowing up since there prone to it in foc mode due to voltage sag?

I see you have about 6 5000 ah lipos wired to 12s. Whats your actual functional capacity with the batteries wired to 12s?   I was having a hard time figuring your values judt out of curiocity..

How do you handle your voltage spark when hooking up power.  Do you have a resistor  setup to help keep that capacitor bank under control?   

Thanks for the replys.  Very sweet setup you have
```

---
## \#30 Posted by: Duffman Posted at: 2017-04-28T09:41:32.687Z Reads: 437

```
I wanted rearrange my VESC and cap wiring because I found out on my other builds that short connections and good ESR can keep your ESC cooler and improve your reliability. To keep wires short, I had to stack the PCBs and the caps and just filled the remaining space with more caps....

No matter how many caps you add, they won't help you with voltage sag, but can compensate for the inductance of long battery wires, which would induce high voltage spikes when switching at high currents.

This is the best and most detailed description of ESR I read in a long time: https://www.electric-skateboard.builders/t/vesc-faq-how-many-capacitors-what-uf/6125/48

I'm running 12s 10Ah (3x 4s5Ah x2) per 'layer' and can stack up to 3 layers for 12s30Ah. Everything at 20c constant / 30c burst.

To power everything up I simply use an XT90S antispark loop key with a little 100A ANL fuse. 

<img src="/uploads/db1493/original/3X/c/0/c0a8153f505584bc3c93c4f629afe824fbc51cd1.jpg" width="690" height="388">

This holds up very well against the 250A burst current I am pulling at maximum like in the beginning of this video:

https://www.youtube.com/watch?v=7bQtSXBECRY&t=12s
```

---
## \#31 Posted by: Nowind Posted at: 2017-04-28T11:15:36.854Z Reads: 412

```
Haha this board is the absolutely awesome Madmax Killer Vehicle.... watching the video and seeing myself strapped to the monster brings a big fat grin to my face... pulling this 11KW was incredible ... also whats amazing is the damping properties of this FAT tires, compared to my 8inch racer it feels so much comfortable even on super rough terrain :slight_smile:
```

---
## \#32 Posted by: ieatflys Posted at: 2017-04-28T23:06:28.647Z Reads: 401

```
Thanks for the reply  and very detailed responce.  Sweet approach you have taken... how much rsnge are you getting out of 30 ah?    Also did you choose tour capacitence baced on any math or just kind of as many as you could get to fit ?
```

---
## \#33 Posted by: ieatflys Posted at: 2017-05-02T07:03:14.161Z Reads: 394

```
@Duffman.  I am in the process of building my cap bsnk for my vesc....  what capacitors did you end up going with  could you maybe supply a link it sounds like youve found some good ones...  also when deciding how many to use and what uf  did you calculate in amperage or did  you run with the 220 uf per vesc oer 4 inch rule?
```

---
## \#34 Posted by: Duffman Posted at: 2017-05-02T18:35:32.731Z Reads: 415

```
These are the ones I used: http://m.ebay.com/itm/Elko-Panasonic-FR-680uF-63V-Kondensator-105-C-Low-ESR-same-as-FM-854466-/181757988566?hash=item2a519eced6%3Ag%3AINEAAOSweW5VZZHo&_trkparms=pageci%253A14fe1e30-2f65-11e7-91ba-74dbd1806b9b%257Cparentrq%253Aca6b5a4715b0ab1db5fb2259fffe9e50%257Ciid%253A2

For my other board which is also running VESCs on 120A with 50cm battery wires I just replaced the 2x3 stock caps. On this build I simply had the space  so I went with 4x7 caps.

Range depends highly on terrain. When driving and drifting on grass I should get around 20km with 12s30Ah. In loose sand or snow I can burn down the same battery on less than 10km.
```

---
## \#35 Posted by: Duffman Posted at: 2017-08-22T09:18:39.767Z Reads: 410

```
I always forgot to show you one little detail, which imo is a big improvement over the stock MBS spring truck system. 

Instead of using a spring and an egg shock (dampa), I'm using an elastomer compression spring to get better / softer steering capabilities and better dampening of speed wobbles.

I'm using E 1556/ 32 x 63 from Meusburger (https://ecom.meusburger.com/e/index.asp?id=2298&rnd=32287) original manufacturer seems to be Effbe (http://www.effbe.de/index.php?id=30&L=1).

In combination with some simple aluminium bolts it is a drop in replacement for MBS and Trampa spring trucks.

<img src="/uploads/db1493/original/3X/2/b/2b27872ff44b430b0ca79c026248151d22e4e4c6.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/6/8/68c809299278940383e8107421e149c8ec6ffda2.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/b/c/bcdedee87f09acf9965c1bf5d2183cb51cb92f9f.png" width="482" height="500">
<img src="/uploads/db1493/original/3X/8/b/8bea884b2f15cb5d06ed9df1679ebd6616fb7b0b.png" width="690" height="353">

This is a comparison of the usual spring/damper combination and elastomer springs:
https://www.youtube.com/watch?v=91LO9fK6-os

I'm running these in my Monster an in a Trampa/Next crossover board of a friend for more than a year and am totally satisfied with the feeling of the ride.

<img src="/uploads/db1493/original/3X/6/9/69db8c52394fd163bb6690ae9f632fb3349dffb1.jpg" width="690" height="388">
```

---
## \#36 Posted by: Nowind Posted at: 2017-08-22T09:59:10.584Z Reads: 376

```
Nice
Perfect documentation as always....
```

---
## \#37 Posted by: rich Posted at: 2017-08-22T12:06:46.784Z Reads: 371

```
What a 4WD monster build, wicked man!
Just a question according the elastomer spring. Are the thread inserts included and how's the feel compared to trampa springs with yellow dampas? Looks very interesting :yum:
```

---
## \#38 Posted by: Duffman Posted at: 2017-08-22T13:28:12.392Z Reads: 366

```
No, the thread inserts are selfmade, but you don't have to own a lathe to make some. Just cut a piece of metal to lenght, drill a hole and round the edge...

The hardest part would be to get the elastomer springs, as I don't know if they sell to private persons...
```

---
## \#39 Posted by: nw-esk8 Posted at: 2017-08-22T19:44:06.806Z Reads: 362

```
Now that is a beast of a board...
```

---
## \#40 Posted by: skslingo21 Posted at: 2017-09-03T06:02:27.094Z Reads: 367

```
All up weight? Drumroll pleaseeeeee

bababababababababababababababababababababab
(what drums sound like in my head)

Youve done a kickass job keeping things light with aluminum sheet!
```

---
## \#41 Posted by: Cobber Posted at: 2017-09-03T10:13:30.740Z Reads: 358

```
[quote="Duffman, post:35, topic:20783"]
I'm running these in my Monster an in a Trampa/Next crossover board of a friend for more than a year and am totally satisfied with the feeling of the ride.

https://www.electric-skateboard.builders/uploads/db1493/original/3X/6/9/69db8c52394fd163bb6690ae9f632fb3349dffb1.jpg
[/quote]

Each time this thread is commented on I re-look at this pic... :punch: :smiling_imp:
cool build, really tight, from the wiring around the batteries, the seamless integration of the front light, the tire tread, to size, the deck... very slick! 
less is more...
```

---
## \#42 Posted by: Duffman Posted at: 2017-09-03T11:37:54.207Z Reads: 343

```
This beast may be anything but not lightweight. I tried to build it as light as possible but it weights around 30kg naked and around 40kg with 3 stacks of batteries.

@Cobber:  This was just evolution. We started with a MBS Pro 90, a MBS Core 94 a Next Redux and a Trampa Deck, mixed everything up and got my Raceboard, my Monster and my friends Trampenstein (in the picture above)...
```

---
## \#43 Posted by: Cobber Posted at: 2017-09-03T11:59:40.822Z Reads: 344

```
ugly is beautiful...
you should try a bikini :wink:
```

---
## \#44 Posted by: skslingo21 Posted at: 2017-09-03T20:29:33.237Z Reads: 332

```
Im jealous of the big one :slight_smile:
Can you explain how you arranged and connected the cells in your pack?
Makes my vertical configuration with balance connectors look like childs play..:cry: :balloon:
```

---
## \#45 Posted by: Duffman Posted at: 2017-09-04T04:24:03.600Z Reads: 345

```
As I'm lazy, I'm just linking to my other buildthread:

http://www.electric-skateboard.builders/t/lightweight-mbs-pro-90-dual-vesc-sensored-c6364-belt-drive-nrf/17143/8?u=duffman

I have the same battery 'dock connector' on all of my builds which offers the possibility to simply switch batteries quick and easy from board to board or to stack them to the desired capacity.
```

---
## \#46 Posted by: skslingo21 Posted at: 2017-09-04T04:58:30.438Z Reads: 338

```
aha those stackable packs are nifty, I figured you had 18650s under the hood! no wonder the little one rips so much you got some serious amps your workn with
```

---
## \#47 Posted by: Tronik Posted at: 2017-10-28T02:23:57.813Z Reads: 327

```
damn dog that looks pretty dope, we should ride together sometime, hit me up. I got a 4x4 too.  skatemachines.com
```

---
## \#48 Posted by: Duffman Posted at: 2018-02-28T14:06:59.415Z Reads: 314

```
Finally some snow:

https://www.youtube.com/watch?v=vCzBo51sVNA
```

---
## \#49 Posted by: Der6FingerJo Posted at: 2018-02-28T14:17:17.231Z Reads: 318

```
Love it, you're doing the opposite of what most people here do when it snows :smiley:

Any special waterproofing added or the same setup as in the original posts?
```

---
## \#50 Posted by: macncheese Posted at: 2018-03-29T21:11:10.150Z Reads: 303

```
I love your idea on fenders. I was looking at 3D printing some. I may try a shot at bending aluminum like yours. I have similar size offroader.
```

---
## \#51 Posted by: Duffman Posted at: 2018-07-16T06:49:40.702Z Reads: 270

```
Offroad drone fun:
https://www.youtube.com/watch?v=vZ_kcUCrKCE&feature=youtu.be
```

---
## \#52 Posted by: Trdolan03 Posted at: 2018-08-08T21:31:13.991Z Reads: 246

```
What Lipos did you use on this (referring to brand)
```

---
## \#53 Posted by: Amonada Posted at: 2018-08-09T09:07:35.082Z Reads: 240

```
He posted a link in another Build thread:

https://www.electric-skateboard.builders/t/lightweight-mbs-pro-90-dual-vesc-sensored-c6364-belt-drive-nrf/17143/8?u=amonada
```

---
## \#55 Posted by: celica39 Posted at: 2019-03-10T20:04:28.538Z Reads: 146

```
Any update since ? Its my dream to ride in the Quebec winter but l don't find 200mm  tire with enough spike to use ice studs ,
```

---
## \#56 Posted by: Andy87 Posted at: 2019-03-10T20:14:57.605Z Reads: 145

```
With 8“ that’s gonna be hard. 
You can start with 9“ wheels from @MBS
 https://www.mbs.com/parts/13120-9-mbs-t2-tires-1
They definitely have enough meat for studs.
10“ would be even better, but than you need also hanger extension etc.
```

---
## \#57 Posted by: BigZwatt Posted at: 2019-03-10T20:22:22.907Z Reads: 141

```
Thats exactly what i was thinking.
```

---
## \#58 Posted by: celica39 Posted at: 2019-03-10T20:38:48.661Z Reads: 137

```
Yes l know they exist but the wheel (five stars )  for theses tire are not compatible with 12mm axle
```

---
## \#59 Posted by: Mobutusan Posted at: 2019-03-10T20:44:07.728Z Reads: 136

```
They are compatible if you use the 12mm ID bearings.
```

---
## \#60 Posted by: celica39 Posted at: 2019-03-10T22:30:57.674Z Reads: 127

```
Great but they don't sell them anymore and the 3 spoke are to much fragile for my taste
```

---
## \#61 Posted by: Andy87 Posted at: 2019-03-10T22:34:23.859Z Reads: 127

```
Thsn get the trampa 9“ megastar hubs.
```

---
## \#62 Posted by: Oculophilia Posted at: 2019-12-03T21:17:52.209Z Reads: 50

```
Wow. You put both the man and duff in duffman! At some point i think it becomes an ATV without a seat and you are about there. 

Definitely confirmed my belief as well that my destiny lies in mechanical/electrical engineering not the legal field.

Who needs to be pro at getting yourself out of trouble when there is tech like this and all the offroad dirt bikes that we can mod to help us get IN trouble?
```

---
## \#63 Posted by: Oculophilia Posted at: 2019-12-03T21:20:15.314Z Reads: 49

```
![1201192022|375x500](upload://ren26B7KBuezbXQfSS5TB9HAB8y.jpeg) 

Colorado winter checking in. 

Saw a video of someone studding their tires by removing, drilling, screwing ss screw, then sealing with contact cement. Working well so far and going to finish it up in the next few days.

You inspire duffman thank you for the detailed specs as well.
```

---

# Air Blade &#124; Enertion R-spec 6372 &#124; 10s5p &#124; TB single motor kit &#124; Never Summer El Jefe Board

### Replies: 64 Views: 7487

## \#1 Posted by: kyo Posted at: 2016-07-16T16:14:07.442Z Reads: 467

```
HI guys, finally i decided to build my very first eboard, after 3 months of lurking into this awesome community. Yeah. i did my homework, so many things to learn. Parts are on the way, well most of them. Here is the list

-Board: Never Summer El Jefe (inspired by @scrant ) (on the way)
-Mechanical: TB single motor kit: trucks, wheels, motor mount, belt … (on the way)
-Electronic: 

    1. VESC from Enertion.(ordered)
    2. Enertion R-spec big boy 6372 190kv.(ordered)
    3. Space cell pro 4 (10s4p)(initially).
    4. Controller: Nyko kama(maybe upgrade later due to some reported dropouts)

The battery is a tricky part. Due to aviation regulation, they don’t ship to where i live(Vietnam). So I am back to old school: DIY. I have 3 options and some questions in mind, PLEASE help me with this one.

    1. Li-on 12s4p Samsung 25R with BMS.
    2. Li-on 10s5p Samsung 25R with BMS.
    3. 2x6s 12000mah lipo to make 12s battery(or 2x5s makes 10s). Tear it down, make it slimmer.

Of course, the battery will have with a meter.
Questions:

1. With spec like that, should my board go with 10s or 12s? There are a lot of posts saying 12s is a bit too much for the VESC, that it will burn drv chip but there are also many boards use 12s with no problem ex: @longhairedboy , @lowGuido  …

2. Can lipo battery use BMS? I ask this because I saw noone here doing it. 
How can i charge the battery? I mean with what voltage? According to what i learnt : if 10s then 42v 2a, if 12s then 50.4 2a (4a for fast charger) Is this correct? Are there any cheaper alternative? 

3. How can I choose amp(current) for BMS ?

All help and suggestion are appreciated. 
Pic will coming soon.
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-16T21:16:23.955Z Reads: 409

```
1. 190kv with 12S is probably too much. Go with 10S. @chaka can confirm ERPM calculations.

2. Yes you can use a bms with lipo. Charge with the voltage that your batteries will be when fully charged. 4.2x10=42v for 10s.

3. Charge at 1C for quickest charge. So if you have a 12ah battery, charge at 12amps for quickest charge. Not many 12amp chargers so you could do .25c 3amps and that would take about 4 hours.
```

---
## \#3 Posted by: jrpwit Posted at: 2016-07-16T22:32:15.527Z Reads: 398

```
Yup to my understanding you can do 12s on a 190kv motor cause you are just below 60k erpm as long as the cells are at 3.7 volts. However if the cells are 4.2 volts you will have above 60k which my damage the drv chip. I had a similar problem designing my board cause I was planning to go 12s with a 245 kv motor. This would for sure damage the current version of the vesc cause that is far past 60k erpm even if the cells are at 3.7 volts (44.4*245*7=76146). For now I am going with 9s even though it will still exceed 60 erpm if the cells are at 4.2 volts. I should technique be going 8s but I plan to by easy on the throttle when my batteries are fully charged and also I will set the max erpm on the vesc to 5500 erpm just to be safe. 

For you 10s would be safest which is a reason enertion uses 10s. Maybe @chaka would shed some light cause he's the man.
```

---
## \#4 Posted by: kyo Posted at: 2016-07-17T14:37:14.501Z Reads: 348

```
thanks for your answers :smile:
```

---
## \#5 Posted by: ikjahaa Posted at: 2016-07-17T14:42:12.432Z Reads: 342

```
Waiting on @chaka too,
First time i heard of this e-rpm... sounds interessing.
```

---
## \#6 Posted by: jrpwit Posted at: 2016-07-17T17:03:04.926Z Reads: 334

```
Check or this thread about choosing the right kv for the current versions of the vesc. Chaka explains a lot of this in it but the erpm should be a problem anymore when the v6 vesc comes out :slight_smile:

Oops almost for got the link: http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#7 Posted by: jrpwit Posted at: 2016-07-17T17:08:24.344Z Reads: 350

```
Also you can check out this link to my build where chaka helped my out with my erpm. Btw he's the man. Just scroll down a bit to his posts.
http://www.electric-skateboard.builders/t/warhorse-five-mile-warhorse-83mm-flywheels-tacon-160-single-drive-3x-3s-zippy-5000mah-nunchuk-vesc/5899
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-07-18T17:02:40.334Z Reads: 322

```
All my boards are running 12S4Ps samsung cells with BMSs with VESC and dual Enertion R-SPEC 190KV 6355s. They get warm but they fly. No problems with them so far, but i use Ollin VESCs so maybe that's why. I have yet to run a single 6372 onthat though. I suspect plenty of warmth there too. 

you can use a BMS with any cell pack that has balance leads. You just have to make sure the BMS is specced for the right cell count and cell voltage/chemistry. I would choose the BMSs current based on the continuous rating of the cell pack, not the burst rating. For example my sammy packs have a continuous rating of 80amps so i use 80amp or less BMSs so that the cells never get uncomfortable.
```

---
## \#9 Posted by: kyo Posted at: 2016-07-29T15:58:24.476Z Reads: 333

```
Ok quick update 
Board came in last week 
<img src="/uploads/db1493/original/2X/7/79030ba3d177b150f8153f9be3330121e630e741.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/c/caea0106ee788548fb543632ca234239c968c974.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/6/628012940de96ae880134c45bde5a7c94e147798.jpeg" width="375" height="500">

And TB single motor kit came in yesterday @torqueboards 
<img src="/uploads/db1493/original/2X/4/4d7a3710cafbd5e0e65cae4e6d5c41c70ee5dc42.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/2X/2/2603c539767bff895a8eb641ab1214294a543330.jpeg" width="666" height="500">

And controller nyko karma
<img src="/uploads/db1493/original/2X/2/2daf1853b6204229ba41ab0863376c0520aa6659.jpeg" width="375" height="500">

Awe i just cannot wait ....
```

---
## \#10 Posted by: kyo Posted at: 2016-07-29T16:01:24.265Z Reads: 313

```
@torqueboards  what are these black plastic tube? Where do they go?

<img src="/uploads/db1493/original/2X/a/a2b75b240d17c34c0c00894b75b829690cf4379a.jpeg" width="375" height="500">
 
<img src="/uploads/db1493/original/2X/2/2ab7c526e97e4dbe07bd42efccad36346d4debc6.jpeg" width="375" height="500">
```

---
## \#11 Posted by: torqueboards Posted at: 2016-07-29T16:17:26.464Z Reads: 309

```
You probably only need one.

<img src="/uploads/db1493/original/2X/2/2673c2ae1f4e8cc1279322c00c761d75efd04e25.png" width="549" height="382">
```

---
## \#12 Posted by: kyo Posted at: 2016-07-30T04:48:03.957Z Reads: 301

```
@torqueboards
The bearings are sticky when i hold between my fingers. Then i spin it, it doesnt spin freely at all. I mean it turns but then quickly stop.
Is this a problem? They are supposed  to spin freely right?
```

---
## \#13 Posted by: torqueboards Posted at: 2016-07-30T04:50:04.660Z Reads: 292

```
Yeah, put them on the wheel and spin it. You can also try putting more bearing oil on it.
```

---
## \#14 Posted by: kyo Posted at: 2016-08-11T16:38:08.765Z Reads: 297

```
Look what i got in the mail today

That is my unbox knife 
<img src="/uploads/db1493/original/2X/3/3eee2ec36302d0c74cf2ae54199643aff6bf7945.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/6/63839bffd292f2a0ab8f787ce77e21d6f92278f5.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/9/99a812922b18071c9c765055841789fd7847d3c0.jpeg" width="666" height="500">

Isn't she beautiful?
<img src="/uploads/db1493/original/2X/0/0e50e44a2cf132afc78c19af2a62cafadc7bf8b4.jpeg" width="375" height="500">

@onloop : one of ur employees said that the VESC would come with xt90 , the one i got came with xt60. Not a big deal, i can replace it with xt90, the thing is that i was live chatting with him on the  enertion website, he went to the vesc and took a look came back, confirmed that it was xt90. Maybe this is from the old batch ???
<img src="/uploads/db1493/original/2X/5/5123c98ff3d25f81e25f1f6a02a0e1e0a747a51b.jpeg" width="375" height="500">

That is it for now, next is the bms and i'm good to go. So excited
```

---
## \#15 Posted by: kyo Posted at: 2016-08-12T02:24:33.608Z Reads: 279

```
@onloop, @EnertionSupport, I got my VESC, trying  to configure, and I don't want to burn it b/c i know nothing ab VESC setup, there are lot of burn VESC due to wrong configs.. My question: Do you have some kind of GOOD and SAFE vesc configuration for R-spec 6372 motor that i can follow. I want to ride it for some time before doing my own tweak.
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-08-12T09:09:24.255Z Reads: 281

```


http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980?u=michaelinvegas



Did you look here @kyo?
```

---
## \#17 Posted by: kyo Posted at: 2016-08-12T09:14:16.428Z Reads: 271

```
I am now. Thanks bruh.
```

---
## \#18 Posted by: Michaelinvegas Posted at: 2016-08-12T09:16:10.407Z Reads: 272

```
Just do a search on key words ....

I'm sure most of the answers are here for you...


A bunch of esk8 nerds here apparently 🤓 Lol
```

---
## \#19 Posted by: kyo Posted at: 2016-08-19T04:15:39.713Z Reads: 272

```
@chaka @lowGuido

Can i use a laptop-like charger to for the motor detection with the vesc? I mean to use it to power the vesc for motor detection. 

The charger is 19v 4a

Bc my bms is on the way.
```

---
## \#20 Posted by: lowGuido Posted at: 2016-08-19T05:30:03.151Z Reads: 271

```
Yes.  I do it with all of my VESC'S.
```

---
## \#21 Posted by: kyo Posted at: 2016-08-21T07:19:49.727Z Reads: 272

```
While waiting for bms and the battery itself, im gonna do the motor detection. After asking and reading around, finally have enough confidence to do it, but i ran to a post that the op has a quite serious incident while doing motor detection( broke his thumb nail) so i decide to make a motor stand 
<img src="/uploads/db1493/original/2X/f/f8ca4dd19cf5dadde3b95204f36d68bc89dfa405.jpeg" width="375" height="500">

I dont have a table saw so i improvised 
<img src="/uploads/db1493/original/2X/a/a3687d69fa60907a4548f7203dba5497c5082faa.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/5/5dc60c3d6164febd29cbf6b98188aa257e919089.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/a/a784c836b9c9f41c080ef9c00cc5c80bfc257736.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/3/3db055d94fa14cd98e45d4fa8144e0741fab7b9e.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/d/d629114c3b2740f082200a5eac3affb7744cf9a7.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/f/f03e7e606d21271ed925b2b8fa92af8d24e9015d.jpeg" width="666" height="500">

It turns out pretty good i think

<img src="/uploads/db1493/original/2X/0/007cd803b8c8dd693118b93de1124b3e063a85d6.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/e/e5dac62fd974beb08b283187aef6547bd7d6d7a0.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/a/ab91323afb44e755713d2ebfea7fa787559db346.jpeg" width="666" height="500">

And with my bad luck, my laptop has broken down when i need it the most. One of my friends always says "Well,  necessity is the mother of invention" . So i go and put together some old junks that i have kept for years to temporarily replace my laptop

<img src="/uploads/db1493/original/2X/8/839e07cf506ee89b293b44f7847617ab64276f5a.jpeg" width="666" height="500">

Oh god, hepl me. I have not touched ubuntu for years. Now i have to configure the vesc with it.

Then my brother helps with soldering the 5.5mm connector on the vesc

<img src="/uploads/db1493/original/2X/a/a7e14f85dd2b7b63b759ec49422875ae7b492142.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/1/1ab7bf1ba284d43c0362331a8dad9ca161e4997f.jpeg" width="375" height="500">

Well, it may not be a piece of art, but i think i will do the trick.
```

---
## \#22 Posted by: Michaelinvegas Posted at: 2016-08-21T08:02:46.690Z Reads: 253

```
How I solder bullet connectors....

I clip a piece of solder and stick it inside the bullet connector enough so that I can insert the wire then hit it a tiny blow torch and let melt then hit the outside with my regular soldering iron ... The silicone sheathing get toasted around the wire a little but some shrink and it's perfect 😉
```

---
## \#23 Posted by: kyo Posted at: 2016-08-21T08:09:46.467Z Reads: 243

```
@Michaelinvegas you mean like this

 https://youtu.be/-4foev6hjJk
```

---
## \#24 Posted by: Michaelinvegas Posted at: 2016-08-21T08:15:57.388Z Reads: 233

```
Yeah essentially 😉
```

---
## \#25 Posted by: kyo Posted at: 2016-08-21T08:18:30.771Z Reads: 232

```
Thanks bro.
```

---
## \#26 Posted by: Jebe Posted at: 2016-08-21T08:22:17.087Z Reads: 233

```
Nice board !
```

---
## \#27 Posted by: Michaelinvegas Posted at: 2016-08-21T08:23:52.994Z Reads: 236

```
Lol I hope the noobs aren't driving themselves crazy trying to do it the hard way
```

---
## \#28 Posted by: kyo Posted at: 2016-08-23T14:45:49.639Z Reads: 246

```
I believe everyone was noob once. Lol 
Hey today i made some space estimation for the electric stuff under my board
Which one do you think will give enough room for the motor?

<img src="/uploads/db1493/original/2X/c/c8db8129a0e99ff16c8d01b7cb0be9d79be7ba55.jpeg" width="666" height="500">

I think this one would, do you?
<img src="/uploads/db1493/original/2X/d/dc59f14b4b95d35d4455d081870e529f2db22db4.jpeg" width="666" height="500">
```

---
## \#29 Posted by: Michaelinvegas Posted at: 2016-08-23T17:12:38.848Z Reads: 234

```
Lol hey I never used paper to set up....

Good idea
```

---
## \#30 Posted by: Michaelinvegas Posted at: 2016-08-23T17:13:54.722Z Reads: 233

```
Top one 


------
```

---
## \#31 Posted by: kyo Posted at: 2016-08-25T01:28:57.494Z Reads: 243

```
Look what is in the mail today

<img src="/uploads/db1493/original/2X/1/1ff3d817bf249d426f46a7573b9bc4af0624bd68.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/b/b0b39cf544c713d85e9d0bc2c39127075fae5f04.jpeg" width="666" height="500">

This weekend is gonna be epic.
```

---
## \#32 Posted by: kyo Posted at: 2016-08-28T16:47:57.109Z Reads: 242

```
So i went the market this weekend. 

<img src="/uploads/db1493/original/2X/6/69b3b3ab91f4bca62ab53614313438451b04adc2.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/4/47dda392ed6dab9b28928c4e1c8e607ee95a2bc1.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/d/d9ab71156332ee432c4b2c758aeb8ffe0ba67044.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/c/cc0877f426d40b6324f3e3df6c9adf0beb941ff3.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/8/82d353b527ce3252af6967da3b095fe9ff007cb2.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/f/f5702990a5f09d9d09dfe63c4ad1793a52abd7e6.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/e/e359f0b68ec9fcb24018e879504e75fa1d448a89.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/e/e539921774249f8f0a046e9a82db3b86f1e4fe87.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/8/8325fa056101d32e7c8c0296d57708748a4aa5fc.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/6/63f96673e60eaf8632402670b71356da24f4bd13.jpg" width="666" height="500">

I bought everything that i needed for the board like, wire, connector, jst 2mmwhich later i decided not to use, instead i solder them directly on the vesc
```

---
## \#33 Posted by: kyo Posted at: 2016-08-28T16:54:12.303Z Reads: 237

```
Let's  get to work

<img src="/uploads/db1493/original/2X/3/35c67279e74d0d473acaf577bf3bdf7969b47c3f.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/b/b44203c02904db16372bc93d81d1c33ddae02e83.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/e/e672b699448a6e72c7b458880c842c3af33fff0b.jpeg" width="375" height="500">

I did the motor detection, the motor spins for some seconds, the stop but the bldc says bad detection result. 

I used laptop-like chager to do the detection, its 19v 3,42amps 

Can the charger be used in motor detection? Or i missed something.
```

---
## \#34 Posted by: anorak234 Posted at: 2016-08-28T16:56:53.176Z Reads: 228

```
That place is magical...
```

---
## \#35 Posted by: FlashNova Posted at: 2016-08-28T17:02:40.704Z Reads: 229

```
Dude, where do you stay at? That market looks like something I would see in Vietnam or Thailand.
```

---
## \#36 Posted by: kyo Posted at: 2016-08-29T05:20:22.865Z Reads: 226

```
@anorak234 ikr. Nowaday we usually do online shopping, but i prefer the traditional way :smile:

@FlashNova im Vietnamese, living in Ho Chi Minh city in the south of VN.
```

---
## \#37 Posted by: kyo Posted at: 2016-08-29T05:24:58.523Z Reads: 232

```
https://youtu.be/GVA8ySQNBjM

I did the motor detection but it was "bad detection result" what did i do wrong?

This is the first time detection, didnot write any configuration execpt for the nyko.

Im using laptoplike charger 19v 3,42amps is this the reason why it fails?
```

---
## \#38 Posted by: Blasto Posted at: 2016-08-29T15:32:04.609Z Reads: 220

```
Yes it could be your supply. I had the same results while trying with a 3S lipo, these motors need that extra juice. Worked fine when i used my 10S pack
```

---
## \#39 Posted by: kyo Posted at: 2016-08-29T15:49:58.141Z Reads: 215

```
Kool thanks man @Blasto 
I will try that this weekend
```

---
## \#40 Posted by: chris.hunt Posted at: 2016-08-29T16:10:05.685Z Reads: 232

```
OP also keep in mind if you charge with the fastest charging it will make the lifespan of you getting the full charge less over time. If you charge at a lower speed it is basically trickle charging which preserves your battery life.
```

---
## \#41 Posted by: kyo Posted at: 2016-09-19T12:00:16.398Z Reads: 226

```
So my drv is gone, while waiting for new drv chip and vesc to come, i make the case.

<img src="/uploads/db1493/original/3X/1/9/1937e4b249115b9d1d2e69c29bc3a9a5f6597a8a.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/f/ff11b3c247ae11fa0b63f107df882438085d7521.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/b/bb3f3ca3cbf1ab186a7eedd3c524a8cd7c06e8d2.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/e/ee3562dd2d55b9d0ee712d6e4b61f54da72e4f61.JPG" width="690" height="388">

<img src="/uploads/db1493/original/3X/1/5/1543f0a2013a61fa6b2a0e9f95fcf1bfe8069a4c.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/d/4/d4809d7cb933d1fdc1febc9d5aed20d8099ae650.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/c/f/cff8e0d726ac89ed31c9ee03bb19c34b387d5ef7.JPG" width="666" height="499">
```

---
## \#42 Posted by: kyo Posted at: 2016-09-24T08:50:39.041Z Reads: 195

```
Today i did a test_run with Fiberglass, bc this is the first time i worked with fiberglass. 

<img src="/uploads/db1493/original/3X/5/4/547f37aad56f023f22d89573cec72e38cfe476ac.JPG" width="666" height="500">

Oh men, this is hard as hell. Take a lot of work.
I could not smooth out the conners, edges. Any advices for me on this ? @longhairedboy @whitepony 

Is this the right kind if fiberglass ?

<img src="/uploads/db1493/original/3X/a/5/a56698ded4efb6a64802f2b027236bf456b201ff.JPG" width="666" height="500">

And some pic 

<img src="/uploads/db1493/original/3X/7/0/709e602a44da7dd032454bb43b8595476b723491.JPG" width="666" height="500">
```

---
## \#43 Posted by: kyo Posted at: 2016-09-24T08:54:20.474Z Reads: 191

```
When i pushed in like this 

<img src="/uploads/db1493/original/3X/2/c/2c03840ed7f437993bf1e377c32e5ce1054714b9.JPG" width="375" height="500">

It always creates some bubbles on top. I think this is bc the pattern of fiberglass. 

<img src="/uploads/db1493/original/3X/4/7/47f4557d0f2e6ae754d524339f359e1c724b9eef.JPG" width="375" height="500">
```

---
## \#44 Posted by: whitepony Posted at: 2016-09-24T11:53:57.571Z Reads: 180

```
yea, without vacuum its really hard to do a sharp edged enclosure. i tried once and failed too :confused:

you can use some wooden planks wrapped in cling film to press the fibers into the corners and make them stay there. basically some frame around your enclosure!
```

---
## \#45 Posted by: i2oadsweepei2 Posted at: 2016-09-24T12:16:42.137Z Reads: 188

```
I had a good outcome using fiberglass matt first then using the weave after. I let the matt get really tacky before I layed the weave on top. I also routed the corners of the wood mold to be round so there wouldn't be any bubbles. There is too much tension on sharp corners when you fold it over otherwise without using a vacuum like whitepony said. His way with the frame will work good too if you try again. 

Pics for reference.
<img src="/uploads/db1493/original/3X/f/4/f4831cdf8605d102f98ca5d2f6313d7e64b05f40.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/3/f/3f16d7873ef3e7fac0993568a4f023cd415fd9ab.jpeg" width="375" height="500">`
```

---
## \#46 Posted by: kyo Posted at: 2016-09-24T12:57:40.553Z Reads: 180

```
@whitepony @i2oadsweepei2

Thanks guys.  Appreciate it. I dont have a vaccum. So i will try to round up the edge and use the matt then weave.
```

---
## \#47 Posted by: kyo Posted at: 2016-10-08T09:27:44.080Z Reads: 185

```
Some update of last week and this week,

Last week is mu second attempt with fg, with different approach, i used double sides tap to stick the fiberglass to the plank wood, oh men i still failed,

<img src="/uploads/db1493/original/3X/6/6/662c1291662e0075a5c0673e120695a304faad0e.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/c/f/cfd3eccec0a0db4490a8187e143cf50b42243908.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/c/4/c4a0038ebac56c90c55d3495f559cc16142205cd.JPG" width="666" height="500">
```

---
## \#48 Posted by: kyo Posted at: 2016-10-08T14:20:39.730Z Reads: 178

```
It turned out pretty bad

Left is first attempt, right is second

<img src="/uploads/db1493/original/3X/a/7/a73daefd1dc8cbb8234422553a0ec173ad18043f.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/d/c/dc1388f0d31ae58b89912641e8e11fb048cc4042.JPG" width="666" height="500">
```

---
## \#49 Posted by: Tuomalar Posted at: 2016-10-08T16:44:45.219Z Reads: 165

```
I had problems with cornes too, but I splayed all 90 degree corners and result was much more better. Still not perfect, but better.
```

---
## \#50 Posted by: kyo Posted at: 2016-10-09T09:43:29.034Z Reads: 179

```
Alright, this weekend is third attempt. Things are getting better, just better not perfect. 

<img src="/uploads/db1493/original/3X/1/1/1123a4e7a8f12b7d051a09eef2fd9b370feb7539.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/c/e/ceabe5cc6287b566c25de3feac57fd2b31691c4a.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/2/f/2f40037e85831ae33df19c92fda62011d02dd859.JPG" width="666" height="500">

It turns out better than 2 previous attempts

<img src="/uploads/db1493/original/3X/7/6/764b6037172a4d084820fe6f007ad6adf7dc98b9.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/c/4c545066a2c4e16f0329c9d1a264cb1756985dda.JPG" width="666" height="499">

<img src="/uploads/db1493/original/3X/6/4/648fd2805a253acd057f7a6ba6c01c2ce42a9109.JPG" width="666" height="499">

<img src="/uploads/db1493/original/3X/0/8/08e1bd447259a60d7e48ae82524790d3f2777e2b.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/6/f/6f757a7fb78a0344127d745b7d99788b334f5777.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/8/8/882eaa4c268688d47a986d91dec38cf86e9868e1.JPG" width="666" height="500">

It is not what i expected but it is ok , useable. 
<img src="/uploads/db1493/original/3X/c/0/c097dee99fd9938300c6464944806f29f11091b2.JPG" width="666" height="500">
```

---
## \#51 Posted by: i2oadsweepei2 Posted at: 2016-10-09T11:00:03.300Z Reads: 158

```
That looks much better. The matt was a sticky hairy mess when I did it. Still worth it though. Good job!
```

---
## \#52 Posted by: kyo Posted at: 2016-10-09T11:25:34.543Z Reads: 161

```
Yeahh ikr, ok next week will the real deal. @i2oadsweepei2. Thanks for the tip. Next one would be beter looking for sure.
```

---
## \#53 Posted by: kyo Posted at: 2016-11-12T14:53:13.101Z Reads: 161

```
Some update: i finally the battery case that works,well in a way.
<img src="/uploads/db1493/original/3X/0/c/0cf0fbb846a0d0d79fa5a8599abf73938d4cf872.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/2/b/2be2b91a1d6c603279233fb59bef35738dc5ec94.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/6/f6dbdcbb4cbeb4fe6b99d8ec8740df8143d7d117.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/9/0930cace9f40d6bdb0fd8f3ce5874765064a34ea.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/9/a/9a3786efad816640607f154833ee4dfaffbe4b4b.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/8/b893ec026aeea6ecd81d7e7c2eac206e77039fda.JPG" width="666" height="500">
```

---
## \#54 Posted by: kyo Posted at: 2016-11-12T14:58:57.906Z Reads: 153

```
https://youtu.be/iu-UQMtN3sI
```

---
## \#55 Posted by: i2oadsweepei2 Posted at: 2016-11-14T23:48:32.532Z Reads: 141

```
Nice job on the fiberglass. Feels much better when we make things ourselves.
```

---
## \#56 Posted by: kyo Posted at: 2016-11-15T03:08:53.944Z Reads: 136

```
yeah, and i really enjoy the process of making things :wink: ,
```

---
## \#57 Posted by: kyo Posted at: 2016-11-27T02:27:18.642Z Reads: 122

```
Some updates: this week i did the wiring inside.

<img src="/uploads/db1493/original/3X/a/e/ae8209955c83b68ed9af9d34e0a405a808c5d23d.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/e/0e756d12b256a1c91123dd957139a3bd99bcf7f7.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/6/0/6030e8c9d1552bde6bda01689525f6c5b3c52c45.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/a/aa63d9c8009f328faaf2a172f1088e501adf6ac7.JPG" width="666" height="500">
```

---
## \#58 Posted by: kyo Posted at: 2016-11-27T02:29:49.204Z Reads: 120

```
After paint it black, the case looks really good. 

<img src="/uploads/db1493/original/3X/8/a/8a20f60cda0484abe2cfe60dca6109f4edff9235.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/7/a74427a1d003711b7b843408a576f0171f96526f.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/a/ea7077d78bd84e5592c220c6215fbfdbbffc2cc9.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/3/e/3efd31632baa4331e817ebcb1bf4c66825b4d669.JPG" width="666" height="500">
```

---
## \#59 Posted by: kyo Posted at: 2016-11-27T02:38:36.085Z Reads: 113

```
Why am i not able to change my first post in my thread? post 1 in this thread? i only am able to update the title.
```

---
## \#60 Posted by: lox897 Posted at: 2016-11-27T20:40:43.137Z Reads: 107

```
I believe they have a time limit, so if it is too old you can't change it.
```

---
## \#61 Posted by: kyo Posted at: 2016-12-10T13:53:50.289Z Reads: 98

```
Some update :  i finished my board, yay 

<img src="/uploads/db1493/original/3X/a/9/a9e2c5bb19e370d7e40e34b6ec72ee6193951566.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/6/f/6fa6642dc9a1215a93fa0fbec5b6c165cc3a6221.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/c/1/c1e5bd216e4e874b0c42079692314d674eaaf3f0.JPG" width="666" height="500">
```

---
## \#62 Posted by: kyo Posted at: 2016-12-10T13:55:03.289Z Reads: 97

```
Some cable management

<img src="/uploads/db1493/original/3X/e/1/e17341ce8459e82ee1da912607c22269dde15e48.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/3/0/30874dcf1f8c6ad00ae5e9548381f45fa8a63228.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/1/4/145ba6b5f9b6d29ba32c17a28c981ffbc52c1b13.JPG" width="666" height="500">
```

---
## \#63 Posted by: kyo Posted at: 2016-12-10T14:20:14.097Z Reads: 95

```
<img src="/uploads/db1493/original/3X/3/4/34af59f9b5a43d6c6041404734413e45d05a8748.JPG" width="666" height="500">

I use alumium foil( idealy lead foil, but couldnt find one) to grap around the phase wires to stop partly the electric magnetic field created by he wires. This field would jam the receiver signal.

<img src="/uploads/db1493/original/3X/e/8/e8ca8a97ba2141de6a450c89eac76871db735fa0.JPG" width="666" height="500">

After, no more dropout :wink:
```

---
## \#64 Posted by: kyo Posted at: 2016-12-11T03:02:06.631Z Reads: 85

```
https://youtu.be/29-4yuoB4pU
```

---

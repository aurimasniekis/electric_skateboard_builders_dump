# First build - Bustin Boombox 10s4p Samsung 30Q Dual OM5065 SixShooters AT

### Replies: 26 Views: 3599

## \#1 Posted by: Quiles Posted at: 2017-11-02T18:43:17.124Z Reads: 354

```
Hi all, thanks for all info on this forum....i've been reading this forum for the last 2 weeks!! It's insanely good!

I am starting my first build single motor (TB 6374 190KV). I need help on how to take de best torque out of it (as i live in a hilly area - 15% - i have 75kg/165lbs), and still want a good range of around 32km/20 miles. I don't really mind going much faster, as the asphalt in my neighboardhood is terrible (that's why i am going with 90mm wheels but down the road will change to 97mm, i think).

My parts list (ordered so far):
- <b>Deck Bustin Boombox (stiff) - 38''  - Battery + Eletronics space - 20''x6'' (i could push a little). </b>
<img src="/uploads/db1493/original/3X/c/2/c2a74a8f77410441d24932e08e2f847b531e6f07.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/7/2730c97c95ec8115353676da97440843eb8b779d.jpg" width="666" height="500">

- <b>TB 6374 190kv (Single Motor Build)</b>
collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv

- <b>TB Singlemechanical Kit - Trucks 180mm</b>
collections/single-motor-mechanical-kit/products/single-motor-mechanical-kit

- <b>TB 90mm Wheels (i think i will change to 97mm down the road)</b>
- <b>TB VESC</b>
collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller

- <b>TB Nano Remote</b>
collections/remote-controller/products/torqueboards-2-4ghz-nano-remote-controller

- <b>50units of Battery Panasonic NCR18650PF 2900mAh - 10A discharge rate</b>


To summarize the questions in my head:
- Initially i was thinking on 10s4p, but not sure what i am loosing not going to 12s4p. Just top-speed? Or also loosing some torque ?
- 60k erpm limit. I would be very close with 12s4p. Would i be safe?
- Need advise on BMS/Charging port connectors and on/off switch.
- Enclosures!!!! Need some help here. I was thinking on building one with Kydex....but not completelly sure.

Can't wait to receive the rest of the parts...still 30days away (i live in Brazil).

Thanks guys.
```

---
## \#2 Posted by: willpark16 Posted at: 2017-11-02T20:15:00.184Z Reads: 296

```
I wouldn't personally go 12s on that vesc it had mixed results
```

---
## \#3 Posted by: Guacamoleface Posted at: 2017-11-02T20:21:01.778Z Reads: 294

```
Personally, I think 10s4p is a nice place to be. Lots of power and enough top speed.
```

---
## \#4 Posted by: NickTheDude Posted at: 2017-11-02T20:26:50.599Z Reads: 290

```
[quote="Quiles, post:1, topic:37199"]
NCR18650PF
[/quote]

Why not use higher discharge cells so you can have a smaller pack? A 3P of 30Qs would be able to discharge more amps than a 5P of these.
```

---
## \#5 Posted by: Quiles Posted at: 2017-11-02T20:31:55.507Z Reads: 273

```
Unfortunatelly i already bought de batteries :pensive:
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-02T20:34:46.014Z Reads: 270

```
Lol don't be sad, I personally love those cells, just too pricey, they barely sag at full load for miles, I have a 7s3p I run at 28A
```

---
## \#7 Posted by: Quiles Posted at: 2017-11-02T20:38:04.439Z Reads: 257

```
yeah @willpark16, i know what you mean; as it's my first build, i want to stay on the safe side as much as possible.
```

---
## \#8 Posted by: Quiles Posted at: 2017-11-02T20:39:00.493Z Reads: 253

```
Thanks @scepterr! :slight_smile:
How many miles do you take out of your 7s3p?
```

---
## \#9 Posted by: scepterr Posted at: 2017-11-02T20:39:48.451Z Reads: 248

```
14ish with a 50mm 160kv motor
12ish with 6374 190kv
```

---
## \#10 Posted by: Quiles Posted at: 2017-11-02T20:45:10.430Z Reads: 246

```
cool, good info!
```

---
## \#11 Posted by: Quiles Posted at: 2017-11-02T20:47:35.905Z Reads: 255

```
On the [Cac.esk8](http://calc.esk8.today/advanced/) i am getting 23miles with 10s4p.....this configuration might get what i need. 
<img src="/uploads/db1493/original/3X/2/8/28eafd73a081600bfa260881e7a21e7a6d298824.png" width="690" height="466">
```

---
## \#12 Posted by: Quiles Posted at: 2017-11-02T21:05:31.380Z Reads: 237

```
@Guacamoleface I saw that you used hot iron solder on your board....how the batteries are holding on?..any issue so far?
```

---
## \#13 Posted by: Guacamoleface Posted at: 2017-11-03T06:03:10.824Z Reads: 228

```
I Just split the battery, and all solderspots seem fine. Used for one summer on rough pavement.
Getting a spotwelder early next week so building a new one with another structure. But battery held up nice.
Soldering was a hell of a job because you have to solder one parallell and let it rest and cool down before soldering it again. Took quite somw time just due to keeping heat distribution down
```

---
## \#14 Posted by: Quiles Posted at: 2017-11-03T15:44:34.031Z Reads: 220

```
good luck with the new battery pack...i still need to figure out where spot weld my pack, without having to buy one from aliexpress
```

---
## \#15 Posted by: RonnieFoxxx Posted at: 2017-12-12T06:45:12.160Z Reads: 210

```
Would you be more comfortable with a 12s on FOCBOX?
```

---
## \#16 Posted by: willpark16 Posted at: 2017-12-12T20:01:28.743Z Reads: 213

```
Yes Or Ollin vesc
```

---
## \#17 Posted by: Quiles Posted at: 2017-12-23T12:49:43.146Z Reads: 238

```
hi all, all my parts arrived. I decided to change couple of things.

Thanks to @NickTheDude  , i have change the batteries to Samsung 30Q. Still 10S4P.

I also changed de Motor mount to reversed to use the little tail Bustin deck has. Will post more pics.

I have to say that my first battery pack was a challenging one. Thanks to @darkkevind i was able to spot weld my pack using his car battery+solenoid welder! Not perfect Welds, but good enough. Thanks there!
<img src="/uploads/db1493/original/3X/6/e/6ed9f10c459dae532aa2d19a426ae0b9df858b80.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/e/fe5a8c2cb52683f5172261ad6c0a2cf7eab5d83e.jpg" width="666" height="500"> 

To build it, i have used the @whitepony schema below. On the edges (where the current flows) i used double nickel strips 0.15mm x 8mm.
<img src="/uploads/db1493/original/3X/9/a/9aa5e3aa229b9b830053f50a322ff19999ecf23b.jpg" width="690" height="175">
<img src="/uploads/db1493/original/3X/6/a/6ac2bc841225116594a4bba4cf24282be166867a.jpg" width="375" height="500">

On the edges, to link the 5 packs of 2S4P i have soldered 10wg wire to a nickel support, and then welded on the pack. I did not weld directly to the pack as i was afraid to transfer too much heat to the cells, as i am not an experienced welder. 
<img src="/uploads/db1493/original/3X/c/d/cd3ce5107f347fad997f3a6c5d7f5857b24ef9c7.jpg" width="666" height="500">

I still need to connect BMS cables. This is how the pack is looking so far.

<img src="/uploads/db1493/original/3X/1/0/10fccd5f8d93eb50fc50803b80630aeca0648e11.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/f/cf252290c820d45665f05cb4d1ddd4eaa7ff3173.jpg" width="666" height="500">
```

---
## \#18 Posted by: darkkevind Posted at: 2017-12-24T01:27:34.213Z Reads: 232

```
Hey man, glad I could be of some assistance.

Yeah those welds take some practice to get right with that welder, but once you get it... oh boy! :slight_smile:

Good work :thumbsup:
```

---
## \#19 Posted by: Quiles Posted at: 2017-12-24T23:37:18.549Z Reads: 246

```
:slight_smile: Yeah, in the end i was kinda getting used to. Thanks for detailed video!! Saved my build. Happy xmas!!
```

---
## \#20 Posted by: Quiles Posted at: 2017-12-31T19:28:50.293Z Reads: 245

```
**Part list UPDATED**. Will post more pics soon.

- Deck Bustin Boombox (stiff) - 38''
http://www.bustinboards.com/boombox-longboard-details

- TB 6374 190kv (Single Motor Build)
collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv1

- TB Singlemechanical Kit - Trucks 180mm
collections/single-motor-mechanical-kit/products/single-motor-mechanical-kit4

- Reverse TB Motor Mount with 320mm HTD5 Belt
products/reverse-motor-mount-only

- Anti-spark and ON/OFF switch - 29usd
https://lunacycle.com/remote-on-off-solid-state-switch/

- TB 90mm Wheels
collections/longboard-wheels/products/90mm-epower-flywheels-black

- TB VESC
collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller3

- Battery - 10s4p Samsung 30Q
https://www.imrbatteries.com/samsung-30q-18650-3000mah-15a-flat-top-battery/

- Battery 18650 Insulators
https://www.imrbatteries.com/18650-flat-top-battery-terminal-insulators-20pcs-matte-red/

- BMS 40A (just for charging)
https://vruzend.com/product/36v-10s-battery-management-system-bms/

- Nickel Strips
https://vruzend.com/product/100-pure-nickel-strip-for-battery-building/

- PVC Heat Shrink for Battery
https://vruzend.com/product/large-diameter-battery-heat-shrink-1ft/ 

- Kapton tape
https://vruzend.com/product/polyimide-kapton-heat-resistant-tape/

- 36V Battery charger with cooling fan (3 Amps)
https://vruzend.com/product/36v-lithium-ion-battery-charger-3-amps/

- DROK Blue Back-light LCD Battery Capacity Monitor
https://www.amazon.com/gp/product/B01LQ7MT4K/ref=oh_aui_detailpage_o09_s03?ie=UTF8&psc=1

- Charging port - 5.5 x 2.1 MM DC Power with Dustproof
https://www.amazon.com/gp/product/B076P97Z2G/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1

- XT90 connector - 5 pairs
products/nylon-xt90-connector-5-pairs

- 10 AWG Silicon wire
https://www.amazon.com/gp/product/B017TGYW3S/ref=oh_aui_detailpage_o09_s00?ie=UTF8&psc=1

- NEOPRENE RUBBER SPONGE -Self Adhesive Strip : 1" wide x 1/8" thick x 33 feet long
https://www.amazon.com/gp/product/B0089FMXN0/ref=oh_aui_detailpage_o09_s02?ie=UTF8&psc=1

- Heat Shrink tubes (many)
https://www.amazon.com/gp/product/B06ZXRLPTZ/ref=oh_aui_detailpage_o09_s03?ie=UTF8&psc=1

- Enclosure 3D Printed on 3DHubs.com - ABS 200 μm (with 3 middle part)
https://www.thingiverse.com/thing:2105446

That's all i recall now - will post more pics soon after i receive the 3d printed enclosure (should be here by next week).
```

---
## \#21 Posted by: Maralc Posted at: 2018-01-02T09:14:03.764Z Reads: 195

```
Nice build. What is the budget so far? Are you based in the US?
```

---
## \#22 Posted by: Quiles Posted at: 2018-01-02T22:13:25.946Z Reads: 189

```
Hi @Maralc, so far the build is 1,090 usd. I am based in Brazil (São Paulo) :slight_smile:
```

---
## \#23 Posted by: Quiles Posted at: 2018-01-06T15:10:46.393Z Reads: 195

```
Ok - i am one more luck guy that received DRV error. I was playing with firmware 2.54 changing controle mode to current and etc, and with no reason TB VESC stoped, i went to the terminal type "fault", none showed. After i type "faults", a bunch of DRV appeared. Is VESC really dead? 

Fault            : FAULT_CODE_DRV8302
Current          : 1.9
Current filtered : -0.4
Voltage          : 40.97
Duty             : 0.03
RPM              : 1.1
Tacho            : 122
Cycles running   : 4
TIM duty         : 1160
TIM val samp     : 609
TIM current samp : 21453
TIM top          : 41687
Comm step        : 5
Temperature      : 33.24
```

---
## \#24 Posted by: Quiles Posted at: 2018-05-29T03:23:24.263Z Reads: 147

```
Ok - after after couple of months, lot's of reading and waiting for the new parts do arrive....and after the "DRV" of death, the build changed a litle bit....to be honest, changes were huge: 

- Bought new motors - Dual OM5065 from @chaka 
- Decided to go AT - bought @psychotiller sixshooters
- Dual Focbox - @longhairedboy 
- Enclosure....have to say that the 3d printed enclosure was not good enought (very weak) - so i bought psychos 405.
- New Mounts from @marcmt88
- TB218 Trucks @torqueboards 
- Controller Enertion NanoX
- Gear ratio 14/60

Going back on the build log:

- Changed battery heat shrink wrap to add more flex (i was worried about deck flex) and organized the bms-lead cables:
![20180324_162321|375x500](upload://1AvsRyaDAU8mGYc5vxqwQO0ra2m.jpg)
![20180324_163933|666x500](upload://zAItimNuwz3l8rwVkYCYJWKfOSY.jpg)

- Put the 6'' AT and wheel bite came to hunt me....yeah...had to extend wheel base as much as i could:
![20180405_123217|666x500](upload://dPzqzqtvYRUvdpwoaeQiblwgseL.jpg)

- My cat was not happy with the mess on her area...LOL
![20180407_194549|666x500](upload://yEFdEVXyU7dF7BarXX2wQhjoUEm.jpg)

- Deck wrapping on Carbon vinyl using wrap-cut...pretty easy...
![20180421_103100|666x500](upload://onDKT1m5f8gi0nW2H4OA6bmpbGY.jpg)
![20180421_123649|375x500](upload://hdwTsYs6SVn6CZwrt92re9BdbhE.jpg)

- All parts ready to come together :slight_smile: 
![20180421_161053|375x500](upload://4lbRTDkAwj4VEFpBJMlsDTayh6e.jpg)

- Installing LCD / eswitch and charging port
![20180429_095959|375x500](upload://d1isGHx7ydGZxmAU6lDfMDoIQ2K.jpg)
![20180429_095952|375x500](upload://8CshY3sUQkabveMgmvEXiB1NAlE.jpg)

- Putting everything together with good rubber seal around the enclosure:
![20180429_093135|666x500](upload://iNU7aD7RNxJu6IQ9LxiljifOJLT.jpg)

- That's all folks:
![20180501_220118|666x500](upload://qNUstCroYXBtMyF2PMkyLstGCgr.jpg)
![20180501_220142|666x500](upload://nWkZLIei55jsWwnSanO0m5kYSUn.jpg)![20180501_220136|666x500](upload://pQu8mFop3UKfJnkIJ6NP9ZeFFz0.jpg)

My last throughs:
- After i extended the wheel base, deck became more flexy, pressing hard batteries in the enclosure.
- It's a bit high from the ground for me....i think a drop through would be a better choice
.....right now i am working to get this build on a new deck....a Landyachtz DropSpeed...let's see how it goes...

These things never ends...lol...the only constant is change...
```

---
## \#25 Posted by: billstr Posted at: 2018-09-12T17:13:17.324Z Reads: 86

```
Rad build! It's like a home made LaCroix. What was the total cost? Certainly less than the $2.3k LaCroix is asking...
```

---
## \#26 Posted by: Quiles Posted at: 2018-09-12T17:37:47.306Z Reads: 82

```
Thanks! This build was around 1.1k usd.....lot less than LaCroix (but have to say they have bigger batteries , carbon fiber enclosure and a flexy sexy deck :slight_smile: )
```

---

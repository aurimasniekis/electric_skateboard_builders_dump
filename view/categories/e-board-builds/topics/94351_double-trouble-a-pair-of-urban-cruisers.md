# DOUBLE TROUBLE - A pair of Urban Cruiser&rsquo;s

### Replies: 26 Views: 770

## \#1 Posted by: ducktaperules Posted at: 2019-05-19T20:16:57.385Z Reads: 233

```
I completed my first build "[BIG TORQUE](https://www.electric-skateboard.builders/t/big-torque-reliable-board-for-the-larger-rider-diy-cnc-tab-welder/43075)" over a year ago and feel like many lessons have been learnt during that process. I was planning some upgrades but small things i wanted to change resulted in needing to change a lot of hardware. 

A friend with a boosted board also decided that he wanted to go the DIY route so we decided it might be worth it to just start again from scratch and build a pair of boards together.

Following on from BIG TORQUE the goal here is a powerful board for a big rider however this time i want more range, more reliability and more comfort. lots of failures last year due to water ingress and mechanical breakages limited my riding time so this build im going to spare no expense in making things robust and reliable.

I plan to use this page as a detailed log and post regular updates on the build however i have a bit of a backlog so expect quite a few posts at once.
```

---
## \#2 Posted by: ducktaperules Posted at: 2019-05-19T21:02:13.381Z Reads: 220

```
First up PARTS LIST:

[12s4p SAMSUNG 30q](https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html)

After spending a long time last year re purposing batteries we decided now was the time to start building our own packs so we split the cost of a tab welder and committed. We chose 30q because they seem to offer good range but also long life. 12s4p should be 12Ah or about 520Wh which is double the capacity of my old pack. for both boards that 100 cells :slight_smile: 
![IMG_20190403_224534|666x500](upload://b9kUtVRDPiULLTa07dQ4OgEFLFF.jpeg) 

[KALY ENCLOSURES](https://www.kaly.nyc/product-page/battery-enclosure)

DIY enclosures are hard . . . very hard. After building a few now i have mad respect for those on the forum that make awesome enclosures. I have learnt that if you want something reliable then just buy one of theirs cause it will save you a shit ton of time and cost down the line. We went with the @Kaly enclosures cause it looks great and was very well priced.
![IMG_20190429_231318|690x402](upload://zhY68RaZRHHv4rhKtqdEEItWRYk.jpeg) 

[FATBOY SS GEAR DRIVE](https://shop.3dservisas.eu/collections/drivetrain/products/fatboy-ss-drive-hd)

As a large guy i found that belts needed to be fairley tight to avoid skipping witch means that they didn't last that long. After having a few snap whilst breaking I have been eyeing up some gear drives. Decided to go with @3DServisas Gear drives with the 5:1 reduction. The finish on these is great.
![IMG_20190515_083034|666x500](upload://fkgeMCTFLz15JyXLylUhChuTTew.jpeg) 
 
[TRAMPA ATB](https://www.trampaboards.com/trampa-mountainboard-with-12mm-solid-axle-infinity-trucks-ratchet-bindings--custom-wheels-p-26832.html)

My old Trampa board is built like a tank but the street carve deck doesent fit the enclosure well and the mini spring trucks wont fit most gear drives so i decided to move to a full size ATB. I also decided to switch up from skate wheels to urban treads and also get bindings as i have eaten asphalt more than once due to cracks and bumps on local country roads. I went for the 6.5" urban treads to keep the top speed below 35mph and also to allow running at very high PSI when i need the range.
![IMG_20190515_172516|690x474](upload://zvpmyD7jKeqNB0HduNrhy9riHty.jpeg) 

[MAYTECH 6880 "TOUGH" MOTORS](https://ranglebox.com/shop/product/maytech-6880-190kv-sensored-brushless-motor-x2/)

One of my old motors got knocked at some point and now resonates as certain frequencies. the Maytech motors having heavier than most however should be far more robust due to having sported motor bell at both ends. Might have to cut those long shafts down tho :frowning: 
![IMG_20190515_083131|666x500](upload://lA97LmDiSc3VNcDzfkcsxcy9dBV.jpeg) 

[LLT POWER Smart BMS](https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/)

Last time I had a faulty battery i couldn't work out why by board kept cutting out. i had no way of checking on the battery and no way of fault finding. This time a Bluetooth smart BMS will allow me to view the status of all cells in the battery. I also got a good case of face-pavement once because i hit the power and my BMS over-current decided to cut the power, after that i will only run BMS in bypass for discharge. This means i can get away with a smaller (20A) charge only BMS.

[FOCBOX UNITY](https://www.enertionboards.com/FOCBOX-foc-motor-speed-controller.html)

Since im bypassing the BMS for discharge i need a way to switch the board on and off. Decided to use the Unity as it has claimed higher output power than the old FOCBOX and also has integrated anti-spark power switch.
```

---
## \#3 Posted by: ducktaperules Posted at: 2019-05-19T21:14:31.105Z Reads: 193

```
GLUING PARALLEL GROUPS

First job was to assemble the Samsung 30q cells into 4p groups. I glued the cells together with hot glue. To ensure good alignment the cells were placed in some makeshift cell holders.

![IMG_20190406_104130|666x500](upload://7qVK7rBhvO34JLWMoGsxvR5Rekl.jpeg) 

Excess glue was "squeegeed" out with the corner of a credit card to ensure a clean join with plenty of surface area.

![IMG_20190406_111021|666x500](upload://4dzgexd5SUAkamWuTsbpwe5uJwg.jpeg) 

Cell positives were then fish papered to avoid any shorts.

![IMG_20190406_112018|666x500](upload://k8Rvg25JLCCUYgrqTtj6Jvg3ONW.jpeg) 

Looking good :slight_smile: 

![IMG_20190417_225728|690x230](upload://bl2OPJO2vMQRJ8m45VaYHc2k8PN.jpeg)
```

---
## \#4 Posted by: Vykku Posted at: 2019-05-19T21:22:36.326Z Reads: 175

```
[quote="ducktaperules, post:3, topic:94351"]
makeshift cell holders
[/quote]

Those look much better than what most people here are using.
```

---
## \#5 Posted by: ducktaperules Posted at: 2019-05-19T21:33:25.802Z Reads: 182

```
WELDING PARALLEL GROUPS

I am using @Kaly  [CELL Fuse pcb kit](https://www.kaly.nyc/product-page/cell-fuse-pcb-kit) to join cells in parallel and make it easier to join them into a pack. Additionally this kit means that every cell is individually fused adding another layer of protection in case of failure.

Nickel strips were soldered onto the pcb's using a jig that held the strips in place, this means very uniform strip positions. large tabs are for battery negatives and thinner "fuse" strips are for positives.

![IMG_20190509_222930|666x500](upload://vYp3a6GgxQ99wTNYO9lWg4B4cC6.jpeg) 

PCB and cells then fit into an alignment JIG ready for tab welding.

![IMG_20190427_232545%20(1)|632x500](upload://moogKzUlE8WOCBZPnXji7gKllkv.jpeg) 

At this point you could easily weld the cells by hand . . . but when there is this many cells to weld why do it manually?

https://imgur.com/gallery/4ilZ5p5

After finishing enough cells for one board.

![IMG_20190509_230334|558x500](upload://gtBOOYSVM6gyTLDE3E4L7uRuqsG.jpeg) 

Second board done.

![IMG_20190512_091436|666x500](upload://mFCHvgehGzcctLS323UjwbQdD5D.jpeg)
```

---
## \#6 Posted by: ducktaperules Posted at: 2019-05-19T21:34:29.593Z Reads: 170

```
[quote="Vykku, post:4, topic:94351"]
Those look much better than what most people here are using.
[/quote]

Thanks, thats what im aiming for :slight_smile:
```

---
## \#7 Posted by: Grozniy Posted at: 2019-05-19T21:39:55.028Z Reads: 169

```
Noice build
```

---
## \#8 Posted by: ducktaperules Posted at: 2019-05-19T21:57:00.623Z Reads: 178

```
MOUNTING CELLS IN ENCLOSURES

Cell groups have had large clear heat shrink tube applied over them to give another layer of insulation and protect them whilst being handled and moved around. clear heat shrink was then carefully cut off of the terminals in preparation for soldering once the pack has been glued.

![IMG_20190514_201506|597x500](upload://ApHjOE1PT21detFKD506yFJwq3r.jpeg) 

The packs are very solid at the point, not really concerned about damage from vibration or flex.

We cut some wooden spacers to go between the cells to ensure that there was no rubbing between parallel groups and that everything fit snugly.

![IMG_20190514_201518|666x500](upload://lkvd62yZEw1vx2pqDI7c7tOAXVf.jpeg) 

After some recommendations from work colleges we decided to use PURAFLEX 40, a "high modulus polyurethane sealant and adhesive" to glue the packs into place. We started by making sure the dividers were in securely.

![IMG_20190514_203229|666x500](upload://xwV27au5h2coi6yx8jVQDoFSamK.jpeg) 

Next we placed glue under the cell packs to ensure they stay in place. 

![IMG_20190514_204005|666x500](upload://vFLqm0RnzdSIgmURSaunaXV4mCv.jpeg) 

The X shape is so that as you press the pack down all the air is pushed out and you don't get left with bubbles underneath.

![IMG_20190514_204151|690x264](upload://8hlse8eLTfx2yxC2u13ui5Mjyuf.jpeg) 

A final bead was then laid around the edge to make sure that cells stayed secure and help to stop any ingress that might occur.

![IMG_20190514_210826|666x500](upload://ylK4NiRw6Nvaapik8Ok1WKGiBUI.jpeg) 

2 glued up batteries ready for soldering.

![IMG_20190514_211234%20(1)|690x419](upload://6mlLVrLi3U2Ho0uhtVmRl4d9FKS.jpeg) 

I had my doubts about the PURAFLEX but it has actually worked our very well. After 48h to fully dry these packs are solid. I can hold one of these upside-down above my head and shake it vigorously without worrying that any damage will be done. 

It also lasted much longer than we thought it would, we brought 3 tubes thinking we would need lots but we finished both boards and only used about half a tube.
```

---
## \#9 Posted by: ducktaperules Posted at: 2019-05-19T22:01:00.618Z Reads: 169

```
LAST OF THE BIG PARTS ARRIVED

![IMG_20190515_172956|690x408](upload://5MP1m8pttJglHrgiktB8bHA6ZsD.jpeg) 

![IMG_20190515_173005|666x500](upload://m9aD4DzfwvAwtCTXBRAJpRoqBA2.jpeg) 

![IMG_20190515_173014|633x500](upload://d04F0qpVG5AxqEfigxb4ziySIdm.jpeg)
```

---
## \#10 Posted by: ducktaperules Posted at: 2019-05-19T22:16:42.327Z Reads: 164

```
ENCLOSURE MOUNTING HARDWARE

Next job was to sort out the enclosure mounting hardware. The Kaly enclosures came with threaded inserts which needed to be drilled and tapped into the deck. Unfortunately i needed the pillar drill for this so had to do it at work (meaning no work in progress pictures).

![IMG_20190516_231549|690x456](upload://homghXxiWJKnD7wLnk2aduB5fBC.jpeg) 

In order to correctly position the Inserts we first clamped the enclosure to the deck in the correct position, making sure that no bolt holes overlapped the binding bolt positions. Due to variation in the binding positions on the 2 decks this means that enclosure position is slightly different on each board. Also worth double checking where the front of the enclosure is because they are not the same at both ends, make sure the binding bolts are in he correct positions before starting drilling.

We drilled through the enclosure mounting holes and into the deck with a pilot hole then removed the enclosure and drilled to the full width for the insert. The depth stop in the pillar drill was used to avoid drilling through the top surface of the deck.

![IMG_20190516_231610|690x231](upload://b3pT6KDU9lP0CDKqLACl1KVu6uy.jpeg) 

Inserts were then wound in slowly with a hand drill whilst applying lots of downward pressure. This can be slow and frustrating but ensures that you don't damage or strip any threads.

Finally both board have all mounting hardware fitted (and we were very itchy from all the fibres).

![IMG_20190517_181315|375x500](upload://eljZLHbL1Llp5nWszoucSqef2ih.jpeg)
```

---
## \#11 Posted by: ducktaperules Posted at: 2019-05-19T22:32:40.429Z Reads: 149

```
JOINING CELL GROUPS TOGETHER

We decided to use[copper braided cable](https://www.copperbraid.co.uk/product/flat-tinned-copper-braid-6-mm2-10-mm-wide-x-1-mm-thick-63-amps/) to join the parallel groups together. The braid is 10mm wide and 1mm thick allowing it to have a lot of flex. It has 6mm2 cross section of copper and is rated to 63A. we decided to use 2 pieces of this smaller braid instead of 1 larger braid as after doing some tests we found that the thinner braid was easier to solder and remained more flexible for the same current rating.

![IMG_20190517_185404|690x354](upload://fHku7rdgLtCRTUWT25Cl0i4kTHL.jpeg) 

The trick to getting the braid to remain flexible over short lengths is that you need to heat it quickly enough that you get a good joint but without allowing the heat to spread causing the braid to "wick" up the solder. This required us to source i larger soldering iron than i would usually use. luckily someone lent us an 80W iron without temperature control which would easily reach the required temperatures.

![IMG_20190517_181004|375x500](upload://eoNpPBMDsvGhrE4vBl65IAABpDt.jpeg) 

We also added an XT60 on the output ready for the Unity to connect to.

![IMG_20190517_202333|666x500](upload://jzpufck8jrTkx6kSrDPPf2D5C4P.jpeg)
```

---
## \#12 Posted by: Skunk Posted at: 2019-05-19T22:38:41.164Z Reads: 142

```
Damn... clean building going on. That 5p spot welder is dope. You should sell 5p packs so people can assemble their own battery from there. You could really pump them out with that setup.
```

---
## \#13 Posted by: ducktaperules Posted at: 2019-05-19T22:57:15.307Z Reads: 143

```
@Skunk thanks. I had considered selling them but i don't know if i want to be liable for other peoples safety. If my board cuts out or catches fire it will suck but whatever, if someone else had a problem because of one of my batteries then that would be hard to live with.

Also even if its automated its still surprising time consuming. I don't now how much money you could actually make from reselling cells that are joined together but i dont think it would be worth the effort. I think that most who are already buying pre-welded cells would also want them to be built into a pack and bms protected so there is no risk to them.

IMO a better idea would be to sell an enclosure with an integrated and protected pack that you can just add your own electronics to. This could make diy builds super easy and low risk for the amateur DIY builder.
```

---
## \#14 Posted by: Skunk Posted at: 2019-05-19T23:07:23.950Z Reads: 138

```
Oh i know more than a few guys that bought pre made p groups for building their batterys.
```

---
## \#15 Posted by: ducktaperules Posted at: 2019-05-19T23:11:41.507Z Reads: 146

```
ADDING BMS

Balance cables and an XT30 have been added to the Battery. The balance cables are routed to the LLT smart BMS and the XT30 is to allow separate charging of the cells. This charge path will probably have an inline fuse added at some point.

![IMG_20190519_181029|690x230](upload://9Y4pzhcI6YMIG7YSeXc7Ag8Yn7u.jpeg) 

Kapton tape is used to insulate all bare conductors on the battery and also keep balance cables from moving around.

As we have been building a board each they are slightly different but we are trying to keep the layouts as similar as possible.

![IMG_20190519_182814|375x500](upload://bSetoOP6dqs9IfEbINlOUvY9xJe.jpeg) 

Were still waiting on a Unity but everything seems to fit well. 

BMS is up and running but initially seemed to be having troubles getting correct cell reading for the first 3 cells. eventually we found that this was because you must have the B- port connected in order to get correct reading for the first few cells. Now it looks good, all cells seem to be at a healthy storage charge :slight_smile: 

![Screenshot_20190519-205414_2|509x500](upload://1UlH4JZUiUeb9Jm5xydyFv0cmUc.png)
```

---
## \#16 Posted by: Jaydawg56 Posted at: 2019-05-19T23:27:42.516Z Reads: 134

```
Dope build!  Two questions:

1) DieBMS?

2) what mm width does kaly use for his positive strips?

Thanks!
```

---
## \#17 Posted by: rusins Posted at: 2019-05-19T23:40:30.250Z Reads: 133

```
Do you even need cell level fusing if all your parallel groups are so well insulated from each other? (I know that's just what the Kaly kit comes with, but asking in general)
```

---
## \#18 Posted by: ducktaperules Posted at: 2019-05-19T23:56:27.863Z Reads: 139

```
@Jaydawg56 I would love a DieBMS and all the vesc metar integration it comes with. unfortunately it's also huge and designed to switch lots of current which I don't need with unity. If there was a smaller charge only version it would be an easy choice but for this build it's not worth the cost and inconvenience.

Not sure on the width but I can check next time I have the calipers out.

@rusins most common battery fault is that the positive nickel strip breaks through the heat shrink and contacts the negative cell casing. With these strips they will just burn at before any damage is done to surrounding cells (causing a chain reaction). Whilst I don't think it's very likely to happen on a pack this well insulated, it costs almost nothing to have the added protection.
```

---
## \#19 Posted by: ducktaperules Posted at: 2019-05-20T22:21:41.809Z Reads: 108

```
MOUNTING ELECTRONICS

As we needed a way to secure the Unity and BMS in place we decided to make a thin aluminium panel which they would both screw into. 

![IMG_20190519_204846|666x500](upload://kb4s1j9oM0MVRPSPEyFltYnUbDG.jpeg) 

We used aluminium as it should help sync some of the heat from the Unity during riding and the BMS during charging. Hopefully the large surface area will help some of the heat escape through the bottom of the enclosure easier.

![IMG_20190519_204900|666x500](upload://iSFy6zuGtfMjvs7iJUeOsWKNAE1.jpeg) 

Its not that fancy but it does the job. If i had access to a CNC that could cut aluminium i might have made something fancy but some times a hand made thing will do just fine.

![IMG_20190519_205213|666x500](upload://fk0wAJFaqCAchgytHE8XzbkHzia.jpeg) 

This was the first time powering the unity off the battery but everything seems to be working so far :smile:
```

---
## \#20 Posted by: ducktaperules Posted at: 2019-06-16T21:24:25.313Z Reads: 69

```
BUILDING GEARBOX'S

Next task was building the geardrives. First job is to mount the plate gears to the wheels. then mount the motor mount plates to the trucks. We can then check that the plates are parallel to the motor gears and lock tight them on.

Motors are then mounted and adjusted to ensure correct gear meshing.

![IMG_20190522_084728|690x366](upload://g3BLwUeasRwaaENZjFYi3gZNlKI.jpeg) 

Drive gear is unbolted from the wheel and placed into the drive. We filled them up with loads of grease, not sure how much you need but fuck it.

 ![IMG_20190528_180219%20(1)|666x500](upload://fZCtErsdr0lWm4hk9lXSxZN7bJd.jpeg) 

Outer case and steel plate are bolted on and the o-ring seal is fitted to keep all the grease in.

![IMG_20190522_212122|666x500](upload://mOh3qhHkiojp9tlDaHZxnrZ65z1.jpeg) 

Wheels fitted back onto both sides (and also front truck)

![IMG_20190522_220045|690x475](upload://7JufT4IwelIksOcwgu6UlHIFMZ9.jpeg) 

Finally test fit them on the board :smile: 

![IMG_20190522_222151|690x293](upload://o8Bf1WI9TyOr7kzGNDmtUUcBC4J.jpeg) 

Rinse and repeat . . .

![IMG_20190528_182330|690x382](upload://h7jiIHsHpEQDIJKXYFFhxodgD7g.jpeg)

![IMG_20190528_182524|690x339](upload://c7tdOHUudXRqUj4dFAnZDogjlsL.jpeg)
```

---
## \#21 Posted by: ducktaperules Posted at: 2019-06-16T21:46:12.743Z Reads: 67

```
TIDY MOTOR WIRES

![IMG_20190528_182753|616x500](upload://5l4mSLoa6jyCXqIhnOA0PWls33R.jpeg) 

With both builds at the same point (-1 unity) attention turned to working out a solution to keep the motor cables tidy.

After having to do a lot of maintenance on my old build i knew that it would be usefull to be able to unplug the motors from the enclosure for servicing. But after spending some time looking for compact waterproof sensor connectors we weren't able to find much that was suitable. We decided that a better solution would be to use the factory fitted connectors but try and protect these as much as possible. 

I made a custom cable rise on my last board to keep things tidy and so designed a new riser that would house and protect both the motor connectors and sensor connectors.

![17203d93bc319d8b94033c13062459ec36b273bf|690x330](upload://3iA3wwJcfec2pojCFUpaBhEjlGT.jpeg) 

The idea here being that this part fits on top of the trucks and all motor cables route through it. if protects the connectors and prevents accidental unplugging during riding.this is then sandwiched shut by the board when the truck is mounted.

![IMG_20190530_071217|609x500](upload://at3W0W7LdkxJRqTR0xOqpjGSit6.jpeg) 

The part was printed from PLA at 50% infill and seems very rigid.

![IMG_20190530_071141|563x500](upload://qZ0ifa8OuARGisqccOSvakF8XJb.jpeg) 

Connectors fit snugly into the recessed areas to avoid any damage that might be caused by vibration.

![IMG_20190530_071136|690x353](upload://nQYO85DhfKA4MSbd1KGnR4pVdID.jpeg)

The plan here is that if additional waterproofing is needed this could also also be filled with some type of grease to form a grease box and prevent water ingress. i do have concerns that if water was to get to the sensor cables it could wick down the inside if the cable and get into the enclosures.
```

---
## \#22 Posted by: ducktaperules Posted at: 2019-06-16T22:13:01.659Z Reads: 59

```
WATERPROOF ENCLOSURE SEALS

Next problem with the motor wires is finding a way to get them in and out of the enclosures in a watertight way.

We found that many cable glands avalable for <5mm cables (like 14AWG motor cables) were not designed to go through the thickness of the enclosure walls. additionally the sensor wire would likely be different thickness to the motor wires so it was difficult to find anything that matched in both sizes.

Eventually i decided it might be better to just design a custom cable gland that had the exact holes i need.

![cableEntry%20v1|690x322](upload://syGbqobGzejTskAaJBXa9FegnVk.jpeg)

The plan is that motor phase wires are on the outside and sensor wires are in the middle. 

![IMG_20190530_210632|690x336](upload://AeyZh9piEWH5K5pHeUDbCJrkfEF.jpeg) 

The outer part applies pressure to keep a silicone sheet sealed against the outside face of the enclosure. There are 4 bolts along the length which should mean that pressure is applied evenly and that there is a good seal down the whole length. The silicone seal has holes which are smaller than the cables ensuring a tight seal around each cable, even if the cable is slightly smaller than the enclosure hole. there is then a part that sits inside the enclosure which holds the mounting nuts and also ensure there is no sharp edges for the cables to rub on.


![IMG_20190530_221811|375x500](upload://euFsnfbpXcqqbGYiQJsP2mXhRC2.jpeg) 

It was relativity easy to mount into the enclosure as i was able to use the outer part as a drilling guide for all the holes. First i drilled the outer 2 holes then fitted the nuts to hold it in place. I could then drill the rest of the holes without the guide moving allowing them to all be clean and accurate.

I then unbolted the outer plate, debured all the holes then reassembled the entire seal with the cables in place.

![IMG_20190530_224547|629x500](upload://wfgCOCESnLQJlSoAp2mtDzHneP5.jpeg) 

The end result is a professional looking part that should very waterproof. I purposefully chose a non-black silicone so that you can see the seal and to make this part more of a visual feature.

![IMG_20190530_224939|666x500](upload://w4ngimXIlNmVKXM8LlOVdw2Usdq.jpeg)

The custom seal and cable riser look great when fitted together. These motor wires should be the only visible external cables and should keep the board looking clean and professional.
```

---
## \#23 Posted by: ducktaperules Posted at: 2019-06-16T22:31:46.305Z Reads: 57

```
FINISHING THE ELECTRONICS

Last job with the enclosure was to mount the the Unity switch and waterproof charge port. These were drilled into the side of the enclosure with the Unity switch in the middle of the rear segment and the charge port just behind. We had to drill these in quite a few size steps as the enclosure plastic seems to start to tear if you jump straight to a large drill size. Unfortunately there is no pictures of this process :frowning:

BMS and UNITY both got a good helping of thermal compound before being bolted down the their mounting plate, locktighting everything as I go. Mounting plate is then double sided into enclosure.

Cells are connected to unity and to BMS. Charge path from port to BMS then to cells is wired up. 

15A fuse is also added to the charge circuit close to the battery in case of internal shorts or charger/BMS faults.

Motor phase cables and sensor cables are connected. Multiple Bluetooth dongles and remote receiver are installed and secured in place. system is power up and tested to check that everything is working :grin: 

![IMG_20190531_191843|690x490](upload://wRTNOFYkjrXEJxAiMPrHe30Voxs.jpeg) 

Enclosure is then taped around the perimeter ready for sealing.

![IMG_20190531_191840|690x225](upload://ktf98jn2Zt616dlMKUBvi8e2zo5.jpeg) 

Enclosure was then sealed, excess plastic was cut from the sealing sheet after mounting to ensure a good clean cut all the way round. Mounting holes were drilled in the sealing sheet to ensure that holes  matched up with the holes in the enclosure.

FINALLY  . . . everything was mounted to the deck :smile:
```

---
## \#24 Posted by: ducktaperules Posted at: 2019-06-16T22:49:04.746Z Reads: 54

```
WHAT A DAY

By chance I somehow managed to complete both my board and my house on the same day.

![IMG_20190602_102815|666x500](upload://qaAywR1ruJgVJwOHPRUXUctLyeT.jpeg) 

The kaly mounting hardware for the enclosure went on easily and looks sweet.

![IMG_20190531_203756|690x292](upload://zQGjr8cNxLmKQf5tksKtGHQ0jyJ.jpeg) 

Everything is shiny and nice . . . Although im sure that wont last long.

![IMG_20190531_203816|666x500](upload://wtHyOc92m5Lwpy4DcATdmtDy4JO.jpeg) 

Ground clearance is a little low, might have to change up to the larger wheel size if this becomes a problem. I guess for now i will just see how it goes.

![IMG_20190531_203736|690x190](upload://pOQyR45Yx4LQdu1xNYTSODhFPnS.jpeg) 

The board looks awesome along side my friends boosted boards, they look like toys in comparison.

![IMG_20190531_204339|652x500](upload://veAM2AvN6DeEV41wZriRjHRZrti.jpeg) 

Cant wait to take it out for its first real test ride.
```

---
## \#25 Posted by: slick Posted at: 2019-06-17T19:33:19.800Z Reads: 42

```
[quote="ducktaperules, post:11, topic:94351"]
The trick to getting the braid to remain flexible over short lengths is that you need to heat it quickly enough that you get a good joint but without allowing the heat to spread causing the braid to “wick” up the solder.
[/quote]

Just an idea - would a damp piece of paper towel or tissue help if you wrapped it around the copper braid to help to keep it cool?

PS damn clean build - kudos!
```

---
## \#26 Posted by: ducktaperules Posted at: 2019-06-17T21:01:30.995Z Reads: 40

```
Something damp may help, i also tried using a big piece of copper that i had laying around but i found that a big iron and moving quickly seemed to give the best result.

[quote="slick, post:25, topic:94351"]
PS damn clean build - kudos!
[/quote]

Thanks :slight_smile:
```

---

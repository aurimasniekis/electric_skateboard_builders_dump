# Battery Management System + Zippys?

### Replies: 104 Views: 9822

## \#1 Posted by: mmaner Posted at: 2016-10-07T14:05:35.444Z Reads: 491

```
Is it possible to use a BMS with x2 Zippy Flight Max battery packs?  I ask because it would be easier to charge tat with a balance charger. and I wouldn't have to pull the batteries every time I wanted to charge.  thans
```

---
## \#2 Posted by: Plumb77 Posted at: 2016-10-07T14:09:07.130Z Reads: 472

```
Bump i have the same question.
```

---
## \#3 Posted by: barajabali Posted at: 2016-10-07T14:16:13.007Z Reads: 472

```
Yea it is possible.
```

---
## \#4 Posted by: mmaner Posted at: 2016-10-07T14:16:56.771Z Reads: 463

```
Can we get a wee bit more info mate :)
```

---
## \#5 Posted by: barajabali Posted at: 2016-10-07T14:21:56.504Z Reads: 460

```
Hahah yea sure. 

So let's assume you are using 2x 6s batteries. 

You need to first hard wire those packs together 
To do that, you need to run one of the pos leads to one of the neg leads which will effectivly series them. 

Then remove all of jst plugs but keep track of their order.

You will have a few extra balance leads which you don't need. At that point just follow the instructions that your bms needs to set it up. 

I offer this as a service for pretty cheap if anyone needs
```

---
## \#6 Posted by: mmaner Posted at: 2016-10-07T14:23:45.497Z Reads: 450

```
Cool, sounds easy enough.  If I can find the balance lead layout Ill see if I can draw up a schematic.
```

---
## \#7 Posted by: barajabali Posted at: 2016-10-07T14:25:15.970Z Reads: 444

```
Well you don't really need a layout. I would just dive into it. It will all make sense once you tear apart a couple lipos lol
```

---
## \#8 Posted by: mmaner Posted at: 2016-10-07T14:42:46.315Z Reads: 438

```
I ordered a 6S  60A  Li-ion / LiPO BMS [[link](http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html)].  I currently have only 3s Zippys, so I guess I'll order some 6s next week.  

Does anyone know how the balance leads specific connection points?
```

---
## \#9 Posted by: gaetjen Posted at: 2016-10-07T14:58:30.626Z Reads: 433

```
Hey,
I build one with a BMS and a 8s Lipo. I got two 4s Batteries and connected them in series. 
Here is a link to my build
http://www.electric-skateboard.builders/t/apollo-longboard-8s-lipo-bms-sk3-6364-245kv-enertion-wheels-and-motor-mount-vesc/7833
```

---
## \#10 Posted by: mmaner Posted at: 2016-10-07T15:08:27.553Z Reads: 414

```
Very nice build.  I like the enclosures a lot, looks beefy :).  Do you happen to have a drawing or pics of how you connected the balance leads?
```

---
## \#11 Posted by: rpn314 Posted at: 2016-10-07T15:16:13.286Z Reads: 399

```
You could also build some type of simple balance lead board so you can just connect the leads from the LiPo to it, and then have it output the 6s balance lead. That would be a non-invasive (to the LiPos) method. I imagine there may already be a product that does that as well.
```

---
## \#12 Posted by: mmaner Posted at: 2016-10-07T15:22:27.491Z Reads: 380

```
Great idea, I just need to find the pin-outs for the 3s and/or 6s balance leads.
```

---
## \#13 Posted by: rpn314 Posted at: 2016-10-07T15:39:39.586Z Reads: 380

```
Ask and ye shall receive: http://www.tjinguytech.com/charging-how-tos/balance-connectors
```

---
## \#14 Posted by: mmaner Posted at: 2016-10-07T15:53:05.849Z Reads: 388

```
you rock out loud sir :)
```

---
## \#15 Posted by: Namasaki Posted at: 2016-10-07T17:32:07.228Z Reads: 403

```
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#16 Posted by: mmaner Posted at: 2016-10-07T17:43:44.584Z Reads: 390

```
Very nice.  The wiring is confusing me but I hope it comes out as well as yours did.
```

---
## \#17 Posted by: VladPomogaev Posted at: 2016-10-07T18:14:20.706Z Reads: 379

```
I have a pretty good tutorial on that here: :) 

https://www.youtube.com/watch?v=jxHQjlHv1y4
```

---
## \#18 Posted by: mmaner Posted at: 2016-10-07T18:23:50.526Z Reads: 362

```
I saw that, very good video.  The issue I am having is find the exact connections for the balance wires for 2 battery packs, the connections for the battery POS & NEG & the ESC POS & NEG.  I see how to do it in theory, but in practice its fairly complicated.
```

---
## \#19 Posted by: mmaner Posted at: 2016-10-07T18:56:49.065Z Reads: 365

```
This is what I have drawn up.  The yellow boxes with a question mark are the questions I need to answer.  I think the Battery NEG goes to B- and the Battery POS goes to P-.  I don't know where the ESC and the balance wires would connect to the BMS.  Any help would be appreciated.

<img src="/uploads/db1493/original/3X/a/7/a7ecb64490ad4f37ff64ddb61ef1cea77ed0f33f.jpg" width="360" height="500">

The balance plugs are what is really throwing me.  As the 1st & 2nd wires apparently goes to cell 1 and then the 2nd & 3rd wire go to cell 2 and so forth I cant figure out how the 4th wire bridges into the second battery at cell 1.  

I am really hoping someone can tell me which wires go were.  I'll then update the drawing and post it for everones future reference.

Thanks
```

---
## \#20 Posted by: rpn314 Posted at: 2016-10-07T19:48:47.468Z Reads: 355

```
You're making great progress! I'll try and address those questions marks.

Let's start with those on the balance wires. Here's kind of a general overview of those balance wires. Skip this paragraph if you already understand it. Each battery has 3 cells, so you have 4 balance wires coming out of each one. The first is the negative of cell 1, which is also the negative of the whole pack (so the main black wire coming out of the pack and balance wire wire, most likely black, are connect to the same end of the same cell). The next wire is the spot where the positive end of cell 1 connects to the negative end of cell 2. This wire allows you to measure the voltage across just cell 1, to ensure it is not out of balance (thus "balance" wires). The next wire connects at the spot where the positive end of cell 2 connects to the negative end of cell 3, and serves the same purpose. The last balance wire connects to the positive end of cell 3 (most likely the red wire), which is also the positive end of your pack (big red wire coming out).

So you've set up the packs connected correctly to get a 6s pack. The way you did that is to connect the positive end of one pack to the negative end of the other pack. Literally do the same thing with the balance wires. Connected the corresponding ones in the middle. From your schematic, I think that would mean the #4 lead on the left balance plug is connected to the #1 of the right's. That means you now have a total of 7 leads, labeled like this 1--2--3--4/1--2--3--4, with the double dash being a single battery cell.

Now, as for bigger wires, assuming your BMS is also serving as over current protection, you have 3 wires going through the BMS. The negative of the combination battery (the two 3s cells together), the negative of the charging port, and the negative of the ESC. I think B- is the negative of the pack, P- is the negative of the ESC (the discharge), and Ch- is the negative of the charge port. I can't quite read what's on your picture, but I think it may be something similar to that. The positives are all connected together.

Edit: Removed "As a note, a 6s BMS should have a 7-port balance jack." ...total brain fart, it should be 6, as is pictured.
```

---
## \#21 Posted by: mmaner Posted at: 2016-10-07T22:43:11.867Z Reads: 328

```
Im gonna go back and read this a couple of times, just to make sure I understand.  I really appreciate all the help.
```

---
## \#22 Posted by: laurnts Posted at: 2016-10-07T22:49:58.194Z Reads: 327

```
Just becareful when connecting lipos together. Ensure using multimeter to know there are no shortings.
```

---
## \#23 Posted by: VladPomogaev Posted at: 2016-10-08T02:43:41.868Z Reads: 335

```
Here ya go! I went off [this](http://www.batterysupports.com/22v-24v-6s-30a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-475.html) following page for the wiring of everything involved. The ESC is directly connected to the battery because it overrides the current limit of the BMS.

Just to confirm my messy paint skills, the battery on the left is NOT connected to the BMS via the balance lead, and two of the pins between the two batteries are connected.

Please be careful while setting this up, while I am pretty sure what my diagram is correct, I have had a lot of people screw up because they thought polarity didn't matter/I might have made a simple mistake.

<img src="/uploads/db1493/original/3X/d/4/d4475d470b4bd30e8fb15b5782f77dfa3191a6eb.jpg" width="360" height="500">
```

---
## \#24 Posted by: mmaner Posted at: 2016-10-08T14:59:16.595Z Reads: 312

```
That is AWESOME!  I will update the drawing when I get back to work Monday and upload it for everyones use.  It will likely be a month or so before the BMS arrives, but at that point Ill test and post the results.  This could be a really cheap way to get very simple battery management fir our boards.  Thanks to everyone for the help.
```

---
## \#25 Posted by: XIII Posted at: 2016-10-08T18:58:36.211Z Reads: 308

```
I have never setup a BMS,

but this seems really strange because you bypass the bms completely when running your board. 
Is this a special way of wiring? Thought you had to have the BMS inside your "main" loop. 
This way your bms won't be able to cut off + the fact it's rated for 60A is not being used, the amps the esc is pulling is not going through the bms. 

Or am i wrong?
```

---
## \#26 Posted by: VladPomogaev Posted at: 2016-10-08T21:18:43.991Z Reads: 295

```
Like I said, I bypassed the current limit of the BMS in that wiring diagram. The BMS is rated for 30 amps and an eboard can draw quite a bit more than that.
```

---
## \#27 Posted by: XIII Posted at: 2016-10-08T21:29:55.333Z Reads: 289

```
I'm stupid, didn't read what you wrote ! My bad !
```

---
## \#28 Posted by: rpn314 Posted at: 2016-10-09T03:42:08.463Z Reads: 295

```
Not stupid, just learning. We've all been there!

Just for reference, I (200 lbs) draw about 40 amps, going 15-20mph uphill on my dual setup. So you may actually be okay with 30, but I would probably follow the wise advice of @VladPomogaev, 30 is a little low. I may add to that, if you are going to bypass it, then I'd see if you can save a few bucks and get the same one but just with as low of a discharge current as possible, since you're not going to use it anyways. I did that on my board. I've got a 10A BMS, but since I bypass it going to the ESC it doesn't create an issue.
```

---
## \#29 Posted by: chaka Posted at: 2016-10-09T04:53:15.501Z Reads: 279

```
I don't want to step on anyone's toes but you really want a more stable chemistry when using a BMS. Stick with cells that have an internal fail-safe like a123's or 18650's if you want something you can just plug in and walk away.
```

---
## \#30 Posted by: Namasaki Posted at: 2016-10-09T05:09:07.340Z Reads: 270

```
@mmaner 
Your balance lead wiring is incorrect for this bms.
You don't use the black balance wire from either pack. You only use the 3 positive wires from each pack.
Each positive wire represents 1 cell.
Starting with the pack that provides neg lead to the Esc. First cell in that pack is cell 1
The pack providing pos lead to Esc is the last pack and the last cell in that pack is cell 6
The red wire is always the last cell in a pack. In your case the red wires are cells 3 and 6.
You'll have to test the other 2 color wires with volt meter to determine which is cell 1,2,4 and 5
The black wires are ground wires and are not needed with this type of bms.
```

---
## \#31 Posted by: VladPomogaev Posted at: 2016-10-09T05:25:46.692Z Reads: 264

```
I'm not sure exactly what you are saying, but I think you are referring to the numbers which are on the pins of the balance connectors, right? In that case yup, they are wrong. I was going off the colors and the order of the wires.
```

---
## \#32 Posted by: Namasaki Posted at: 2016-10-09T05:28:10.111Z Reads: 268

```
@mmaner 
i'm not referring to the the numbers of pins. I'm talking about the balance wires from the batteries.
You have the ground balance wire from one pack connected to the red balance wire from the other pack and both of them connected to the bms balance plug. That is completely wrong and might short out the bms
You connect the main power leads in series but not the balance leads
When you connect a Lipo battery to a bms, you omit the black ground wires and only use the color positive wires.
The purpose of the ground balance wire is for use with a balance charger.
```

---
## \#33 Posted by: VladPomogaev Posted at: 2016-10-09T05:37:29.813Z Reads: 273

```
> You have the ground balance wire from one pack connected to the red balance wire from the other pack and both of them connected to the bms balance plug. That is completely wrong and might short out the bms
> You connect the main power leads in series but not the balance leads

No it's not. That part of my configuration is correct. Here's a 3s to 6s balance lead converter. You can clearly see how the positive and negative leads are connected together.  

<img src="/uploads/db1493/original/3X/9/d/9dfaea79a91fa5558f4e5aa3d7ca983a5ce82426.jpg" width="400" height="400">

> When you connect a Lipo battery to a bms, you omit the black ground wires and only use the color positive wires.

Yes. If you refer back to my diagram you can see that the negative of the left battery is disconnected. This is because it is  the ground of the entire battery pack. Since this is two 3S batteries in series, you still have to connect the center cells together, which do not count as the ground since they are in the "center" cells.
```

---
## \#34 Posted by: Namasaki Posted at: 2016-10-09T05:42:00.373Z Reads: 261

```
@mmaner 
It is wrong. Those 3s to 6s adapters are for Balance Charger balance ports. The Bms is different.
The Bms does not use ground wires from the battery balance harness.
That is why the Bms balance port has only 6 pins not 7.
A Balance charger port has 7 pins.
Trust me, I have actually wired Lipo batteries to a bms. A 10s bms wired to five 2s lipo batteries in series.
I know what I'm talking about.
I you wired a bms according to that diagram, I think you will blow up the bms.
```

---
## \#35 Posted by: VladPomogaev Posted at: 2016-10-09T05:43:49.368Z Reads: 256

```
Well the ground of the entire pack is **not** connected to the BMS balance port. I don't see the problem here.
```

---
## \#36 Posted by: Namasaki Posted at: 2016-10-09T05:44:46.182Z Reads: 255

```
@mmaner 
The ground wire from the balance harness is connected to the main ground wire of the pack
```

---
## \#37 Posted by: VladPomogaev Posted at: 2016-10-09T05:47:27.787Z Reads: 259

```
No it's not. Show me the problem wire. In the meantime @mmaner use at your own risk lol. 

<img src="/uploads/db1493/original/3X/b/6/b6261f51093edfa864a8734f37bb1fe33692a429.jpg" width="253" height="343">
```

---
## \#38 Posted by: Namasaki Posted at: 2016-10-09T05:48:46.073Z Reads: 254

```
@mmaner 
The problem is the red balance wire from this pack connected with the black balance wire from the other pack
```

---
## \#39 Posted by: VladPomogaev Posted at: 2016-10-09T05:50:10.241Z Reads: 252

```
Yeah, that's how you wire two packs in series. Black to minus. 

<img src="/uploads/db1493/original/3X/a/0/a05207814a088a8c53a06c5234a2fd6583552d6a.png" width="682" height="299">
```

---
## \#41 Posted by: VladPomogaev Posted at: 2016-10-09T05:53:20.823Z Reads: 248

```
They carry out the same function. Fine, if you think I'm wrong, so be it.
```

---
## \#42 Posted by: Namasaki Posted at: 2016-10-09T05:53:42.850Z Reads: 248

```
Take a closer look at the bms wiring diagram. There is no pin for a ground wire on the bms balance connector.
```

---
## \#43 Posted by: VladPomogaev Posted at: 2016-10-09T05:54:25.606Z Reads: 246

```
Yeah I did. The battery location/cells are flipped. I followed the diagram.
```

---
## \#44 Posted by: Namasaki Posted at: 2016-10-09T05:54:41.629Z Reads: 244

```
[quote="VladPomogaev, post:41, topic:10772, full:true"]
They carry out the same function. Fine, if you think I'm wrong, so be it.
[/quote]


Not really, because they are designed for a balance charger not a bms
```

---
## \#45 Posted by: VladPomogaev Posted at: 2016-10-09T05:55:18.463Z Reads: 241

```
Why though? What's the actual difference?
```

---
## \#46 Posted by: Namasaki Posted at: 2016-10-09T05:57:42.210Z Reads: 240

```
First of all, this is not about proving you wrong. Its about preventing a disaster.
The battery supports bms like the Bestech bms do not have a ground pin on there balance ports. They use the main ground wire for that.

A balance charger is made differently and has a ground connection on its balance port.
```

---
## \#47 Posted by: Namasaki Posted at: 2016-10-09T06:00:09.457Z Reads: 233

```
Lipo batteries are not really designed to be used with a Bms.
They are designed to be charged with a balance charger. That is why they are wired that way.
To use Lipos with a Bms, you have to modify their wiring by omitting the ground wire on every pack.
```

---
## \#48 Posted by: VladPomogaev Posted at: 2016-10-09T06:00:57.020Z Reads: 237

```
I understand what you are saying, but if you look at the diagram and the way that the batteries are connected, the ground balance pin is NOT connected to the BMS. The "main ground wire" is! 

> A balance charger is made differently and has a ground connection on its balance port.

**That's why one of the batteries does not have a connection to the balance port from it's balance plug!**
```

---
## \#49 Posted by: Namasaki Posted at: 2016-10-09T06:02:35.774Z Reads: 236

```
one of the battery's balance ground wires is not connected but the other battery's is.
And neither should be.
<img src="/uploads/db1493/original/3X/8/8/887b8ac65e6c5908334fdfd962b5a295fbc1562f.png" width="248" height="126">
```

---
## \#50 Posted by: VladPomogaev Posted at: 2016-10-09T06:06:42.718Z Reads: 241

```
That's simply not true. The two wires are already connected together due to the two batteries being connected in series through the larger plug. And, these two wires need to be connected to the BMS according to the diagram which I highlighted here:

<img src="/uploads/db1493/original/3X/2/6/2672ea3ebb3e2addbd8a431d59b7732320143010.jpg" width="690" height="406">
```

---
## \#51 Posted by: Namasaki Posted at: 2016-10-09T06:07:46.388Z Reads: 231

```
You are misinterpreting the diagram
```

---
## \#52 Posted by: VladPomogaev Posted at: 2016-10-09T06:08:02.148Z Reads: 234

```
No you are.
```

---
## \#53 Posted by: Namasaki Posted at: 2016-10-09T06:08:42.452Z Reads: 233

```
I've wired Li-ions and Lipos to Bms's 
Have you ever actually wired a bms?
```

---
## \#54 Posted by: VladPomogaev Posted at: 2016-10-09T06:09:08.793Z Reads: 237

```
I have a tutorial on it:
https://www.youtube.com/watch?v=jxHQjlHv1y4
```

---
## \#55 Posted by: Namasaki Posted at: 2016-10-09T06:13:22.752Z Reads: 234

```
What brand of bms is that?
There are some bms that use a ground wire on the balance port 
but battery supports or Supower, do not.
In the diagram for battery supports, it shows only 6 pins for 6s battery
a wire goes from the positive side of each cell to one of the 6 pins on the balance port. That is what the diagram shows.
```

---
## \#56 Posted by: Namasaki Posted at: 2016-10-09T06:15:36.363Z Reads: 224

```
Though all the cells and in both packs are connected in series through the main power leads.
The balance wires isolate each cell so that the bms can monitor each cell separately.
```

---
## \#57 Posted by: VladPomogaev Posted at: 2016-10-09T06:19:08.535Z Reads: 226

```
It's a Chinese brand, but my BMS is also a 6S, and it does not use a ground wire on the balance port.

@mmaner 's BMS also balances each cell, just like mine does.  I don't think you are correct in any of your claims. The plus and minus of the two batteries are supposed to be connected together, and to the balance port; the negative lead of the entire pack from the balance port is NOT connected; this system should work.
```

---
## \#58 Posted by: Namasaki Posted at: 2016-10-09T06:24:55.168Z Reads: 232

```
@mmaner 
The main power leads are connected in series but the balance wires are not suppose to be connected in series.
They are suppose to be isolated.
That is why there are 6 pins on the bms balance port. One pin for eace positive side of each cell. In a Lipo pack, that means the colored balance wires only.
The black balance wire is connected to the main ground lead of each pack. and has to be omitted when connecting to a Bms balance port.
```

---
## \#59 Posted by: Namasaki Posted at: 2016-10-09T06:34:33.567Z Reads: 235

```
Here is my Lipo with bms build
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#60 Posted by: Namasaki Posted at: 2016-10-09T07:01:48.466Z Reads: 236

```
Ok, after reconsidering this I realize that connecting the ground wire from the 2nd pack as shown in the diagram should not cause any problem.
However, it is  unnecessary.

<img src="/uploads/db1493/original/3X/5/8/588d0ef4dbf4e559508b0adb23acf24e2a98a5fc.png" width="248" height="126">
```

---
## \#61 Posted by: rodriguejoe1 Posted at: 2016-10-09T14:10:05.262Z Reads: 220

```
Thank God. I was running out of popcorn!
```

---
## \#62 Posted by: SageTX Posted at: 2016-10-10T00:01:02.242Z Reads: 213

```
Wow. Thoroughly entertaining! And informative.  Tune in next week!
```

---
## \#63 Posted by: rodriguejoe1 Posted at: 2016-10-10T00:09:22.545Z Reads: 219

```
Oh yeah..Think this was entertaining? Try wrapping your head around this discussion! You're going to need a lot of popcorn!

http://www.electric-skateboard.builders/t/hummie-vs-devin-volts-conversion-to-amps/6910
```

---
## \#64 Posted by: mmaner Posted at: 2016-10-10T03:22:53.894Z Reads: 228

```
I corrected the balance wires in the drawing, they now appear in the correct order.

The BMS I bought is a 60 AMP, I guess I posted the wrong link earlier in the thread.  The BMS I am using is [here](http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html).

Using the interface definition on the product page I used the following instructions, defined as (bms1) through (bms5), to make the POSITIVE & NEGATIVE connections as I understood them.

1. (bms1) The Positive output on Battery Pack (22V + ) could connecting to charger positive pole (charger +)
2. (bms2) Battery Pack (22V -) connecting with B- on board
3. (bms3) Chip board P- connecting to Charger Negative Pole (charger -)
4. (bms4) Chip board P- could be Negative output for charger, motor, controller
5. (bms5) Battery B+ could be Positive output for charger, motor, controller

I used a mulimeter to check the cells of a Zippy 5000mAh 3s 30c LIPO Pack.  With the negative probe on the BLACK wire and the positive probe on the WHITE wire I got 4.03v.  Leaving the negative probe on the BLACK wire I then used the positive probe on the YELLOW wire and got 8.09v.  Lastly Leaving the negative probe on the BLACK wire and moving the positive probe to the RED wire I got 12.13v.  If I understand correctly, the results mean that WHITE is Cell 1, YELLOW is Cell 2 & RED is Cell 3.

I am not clear which is battery 1 (Cells 1, 2 & 3) and which is battery 2 (Cells 4, 5 & 6).  Assuming the battery order is unimportant, though I dont see how it can be, I made the battery closest to the charging port Battery 1.  I then made the balance connections Using the Balance Connector illustration on the linked product page.

I would assume if pin 4 on battery 1 and pin 1 on battery 2 were bridged, that would define the cell order.  As there are only 6 balance connections on the BMS I am pretty much out of ideas.  I hope someone can help me understand this.

Otherwise I think the diagram is accurate.  Let me know if I missed something.  Thanks again for all the help.

<img src="/uploads/db1493/original/3X/d/e/dece96af46f22d0a56015e00e8e0fa540e413e20.jpg" width="292" height="500">

[[here's a google drive link in case the view is too small]](https://drive.google.com/file/d/0B3W3iSVbFDmeSnlLZXM5NlU5aG8/view?usp=sharing)
```

---
## \#66 Posted by: Namasaki Posted at: 2016-10-10T06:05:23.270Z Reads: 192

```
Your getting close, you have the balance wires correct but the main supply wires are not.
The negative supply wire should come from pack 1
The positive supply wire should come from pack 2
```

---
## \#67 Posted by: mmaner Posted at: 2016-10-10T14:28:30.607Z Reads: 198

```
Like this?  I have no idea why, can you explain?  I am really trying to understand this, but the idea of multi cell power source has me pretty confused when it comes to the charging requirements :).  Also, since it s a 60A BMS, do we need to bypass it while running?  Is there a benefit to including the BMS while running assuming the ESC does its job and cuts off at 3.2V?

<img src="/uploads/db1493/original/3X/e/3/e3796b0f060e303194ee50955916020ecb61ab9c.jpg" width="294" height="500">

[Google Drive link](https://drive.google.com/file/d/0B3W3iSVbFDmeSnlLZXM5NlU5aG8/view?usp=sharing)
```

---
## \#68 Posted by: Namasaki Posted at: 2016-10-10T15:15:47.252Z Reads: 178

```
All the wiring looks good now, assuming that the white balance wire is the first cell in each pack and the yellow wire is the second cell in each pack. 
As a precaution, you should check the voltage of each. The wire with the lowest voltage is cell one of each pack. 
The red balance wire is usually the last cell in the pack but it wouldn't hurt to check that one as well. 

Since you have a 60a Bms, You could discharge through it. Just set the Vesc max batt amps at 60 or less. 
I have measured current from the battery feeding dual motors going uphill and at 6s full throttle I was pulling less than 40a
```

---
## \#69 Posted by: mmaner Posted at: 2016-10-10T15:20:26.552Z Reads: 180

```
I checked the cells with a multi-meter...
With the negative probe on the BLACK wire and the positive probe on the WHITE wire I got 4.03v. Leaving the negative probe on the BLACK wire I then used the positive probe on the YELLOW wire and got 8.09v. Lastly Leaving the negative probe on the BLACK wire and moving the positive probe to the RED wire I got 12.13v. If I understand correctly, the results mean that WHITE is Cell 1, YELLOW is Cell 2 & RED is Cell 3.

Which of the POS/NEG wires do I move to discharge through the BMS?
```

---
## \#70 Posted by: Namasaki Posted at: 2016-10-10T15:44:53.195Z Reads: 171

```
You are correct with the balance wires
Wht 1
Yel  2
Red 3
Your most recent diagram is also wired correctly to discharge through the BMS. 
Another advantage of not bypassing the BMS is that when you have regen braking the charge back to the batteries goes through the BMS. 
So you shouldn't have to worry about over voltage when using brakes on a full battery.
```

---
## \#71 Posted by: mmaner Posted at: 2016-10-10T17:02:03.621Z Reads: 169

```
awesome, I really appreciate all the help on this.
```

---
## \#72 Posted by: Namasaki Posted at: 2016-10-10T20:05:05.303Z Reads: 172

```
Your very welcome
```

---
## \#73 Posted by: mmaner Posted at: 2016-10-10T20:43:04.991Z Reads: 173

```
Im still a couple of weeks away from my BMS card getting here, but as soon as it does I am going to build this and post the results, with build pics and diagram, in a tutorial format.  Thanks [rpn314](http://www.electric-skateboard.builders/users/rpn314/activity), [Namasaki](http://www.electric-skateboard.builders/users/Namasaki/activity) & [VladPomogaev](http://www.electric-skateboard.builders/users/VladPomogaev/activity) for educationg a n00b :).
```

---
## \#74 Posted by: jackw Posted at: 2016-10-10T20:56:10.226Z Reads: 175

```
For reference this is how I wired my 3x 4S Zippys up to my BMS (With help from @mccloed) and it's been working perfectly.
 
http://www.electric-skateboard.builders/t/help-with-charge-only-bms-wiring/5626/42?u=jackw
```

---
## \#75 Posted by: ajaynagra Posted at: 2016-10-10T22:44:50.333Z Reads: 169

```
Do you have any pictures :D
```

---
## \#76 Posted by: SageTX Posted at: 2016-10-10T23:16:13.667Z Reads: 173

```
[quote="rodriguejoe1, post:63, topic:10772"]
Oh yeah..Think this was entertaining? Try wrapping your head around this discussion! You're going to need a lot of popcorn!
[/quote]

Phew! Man physics is a bitch!
```

---
## \#77 Posted by: rpn314 Posted at: 2016-10-11T00:49:14.310Z Reads: 162

```
Hope I was able to actually be of help! Building up the community is what I'm here for, we all started as noobs at some point :)
```

---
## \#78 Posted by: Kaden56 Posted at: 2016-10-11T06:57:30.629Z Reads: 164

```
How do you develope this advanced whit 😂😂😂 couldn't have said it better.
```

---
## \#79 Posted by: tueboard Posted at: 2016-10-11T12:19:54.954Z Reads: 166

```
thanks for posting this thread i want to do the same :slight_smile:

which charging port do you will use? someone can provide any ebay link to buy it?

please share photos of the process, thank you
```

---
## \#80 Posted by: mmaner Posted at: 2016-10-11T13:09:54.174Z Reads: 166

```
I am planning on using the Razor charging port and charger.  
[36 Volt 1.5A Battery Charger](http://www.ebay.com/itm/New-36-Volt-1-5A-Battery-Charger-Electric-Scooter-Bike-36V-Mini-Pocket-Razor-/271959816018)
[3 Pin Charging Port](http://www.ebay.com/itm/3-PIN-CONNECTOR-JACK-SOCKET-FOR-BATTERY-CHARGER-RAZOR-IZIP-E-SCOOTER-STAR-II-USA-/162092268756?hash=item25bd73bcd4:g:-M4AAOSw9NxTwvQ0)
It's $21 shipped for both, looks fairly rugged and idiot proof.

That being said, I may salvage a charging port from an old notebook PC and use that and the charger that came with it.  I'll know more when I receive the BMS.

I'll post pics and diagrams of the entire build process when I have the components.
```

---
## \#81 Posted by: mmaner Posted at: 2016-10-11T13:10:42.838Z Reads: 155

```
You gave me some great info that I didn't have before, so I say +1 for rpn314 :).
```

---
## \#82 Posted by: mmaner Posted at: 2016-11-08T17:39:33.114Z Reads: 146

```
Finally got all of the pieces in.  I am planning on building the Zippy + BMS system tonight.  Wish me luck and Ill let you know how it goes, assuming I don't blow up :).
```

---
## \#83 Posted by: mmaner Posted at: 2016-11-08T22:42:14.117Z Reads: 141

```
Ive got everything wired up, per the diagram [here](https://www.dropbox.com/s/7kwz5lv8h9rd3xi/x2%20zippy%203s%205000mAh%20%26%20BMS%20100716.jpg?dl=0). ESC and motor seem to operate as normal.  There is one thing that is confusing me.  I have a [HobbyKing 105W 15V/7A Switching DC Power Supply](https://www.hobbyking.com/en_us/hobbyking-105w-15v-7a-switching-dc-power-supply.html).  When I connect it to the power port, but NOT to the wall outlet, it comes on.  You can hear the fan and see the light.  Is that symptomatic of something?

Here's a copy of the [x2 zippy 3s 5000mAh & BMS 100716](https://www.dropbox.com/s/y0bgsq2puxxwrkt/x2%20zippy%203s%205000mAh%20%26%20BMS%20100716.vsdx?dl=0) Visio doc if anyone wants it.
```

---
## \#84 Posted by: chinzw Posted at: 2016-11-08T23:44:12.600Z Reads: 149

```
Well, its getting powered by the battery. Once you plug it to the wall the power supply will provide the current and charge the battery instead.
```

---
## \#85 Posted by: mmaner Posted at: 2016-11-08T23:56:40.342Z Reads: 159

```
Cool, just wanted to make sure I hadn't missed anything.
```

---
## \#86 Posted by: mmaner Posted at: 2016-11-09T21:50:20.586Z Reads: 163

```
Here it is finished..  I labeled all of the wires.  It seems to be working well, but doesnt charge as fast as iMax B6.  It usually takes me about an hour fully depleted (19.2v) to fully charged  (25.2v).  It takes about 2 hours now.

<img src="/uploads/db1493/original/3X/d/2/d22ae93b8bb1736c33e86beb990830afb3ae1c93.jpg" width="332" height="500">

This is the BMS I used.
[24v 6s 60a 3.6v Li-Ion Li-Po Battery BMS](http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html)

This is the charging port I used.
[Waterproof 5.5 x2.1mm DC Socket Power Jack](http://www.ebay.com/itm/391532615616?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT)

Here's the wiring diagram.
[x2 zippy 3s 5000mAh & BMS 100716 Visio document](https://www.dropbox.com/s/y0bgsq2puxxwrkt/x2%20zippy%203s%205000mAh%20%26%20BMS%20100716.vsdx?dl=0)

If you have any questions, please feel free.
```

---
## \#87 Posted by: chinzw Posted at: 2016-11-09T22:25:50.834Z Reads: 154

```
Its taking more time because the HVC for this BMS i 4.25v per cell, and you're probably using a 2A brick.
```

---
## \#88 Posted by: mmaner Posted at: 2016-11-14T20:09:38.768Z Reads: 150

```
FYI, I think the BMS was defective.  It is not only NOT handling the charge of cells correctly, its not handling the discharge correctly either.  I now have a bad cell, a bad pack.  Any advice would be appreciated.
```

---
## \#89 Posted by: chinzw Posted at: 2016-11-14T22:22:26.491Z Reads: 144

```
What charging adapter are you using? Is it a 25.2v 2A?
The BMS will cut charging once a cell hits 4.25v. And it will start draining a cell as soon as it goes over 4.2v.
```

---
## \#90 Posted by: mmaner Posted at: 2016-11-14T22:44:59.512Z Reads: 144

```
the adapter is 15v 7a.  the BMS was handling the charge fine at first.  but on my first run it pulled only from the 1st cell on the 1st pack.  now im scared to charge it as the cell is at 0.7v.
```

---
## \#91 Posted by: chinzw Posted at: 2016-11-14T23:10:35.881Z Reads: 141

```
15v? No wonder why you fried your cells. You should not be charging with that brick, you should use a 25.2v to charge 6S.
```

---
## \#92 Posted by: chinzw Posted at: 2016-11-14T23:11:49.825Z Reads: 138

```
[quote="mmaner, post:90, topic:10772"]
but on my first run it pulled only from the 1st cell on the 1st pack.
[/quote]

The bms doesnt discharge individual cells on discharge... you discharge through the main leads.
```

---
## \#93 Posted by: mmaner Posted at: 2016-11-14T23:37:19.656Z Reads: 136

```
well damn, thought I had all this worked out...
```

---
## \#94 Posted by: chinzw Posted at: 2016-11-14T23:39:32.614Z Reads: 139

```
Basically, you have been running your battery down, and never charging it. You need 25.2v or higher for it to charge.
```

---
## \#95 Posted by: mmaner Posted at: 2016-11-14T23:41:44.268Z Reads: 137

```
cool, ill get another BMS and another adapter.  So, did I understand that the BMS doesn't control the discharge of individual cells?  What keeps the cells discharging evenly?
```

---
## \#96 Posted by: chinzw Posted at: 2016-11-15T00:43:54.714Z Reads: 134

```
Your bms is probably fine, just get 25.2v 2A charger.
The BMS protects the battery in a few ways:
Over-charge: If any cell hits 4.25v it will shut off the charging mosfets.
Over-discharge: If any cell hits 2.9v
Over-current: If you go over 60A

Since you discharge from the main leads, there's nothing that prevent the cells from becoming unbalanced. Manufacturers of lipos match the cells so that this doesn't happen.
```

---
## \#97 Posted by: mmaner Posted at: 2016-11-15T01:28:59.568Z Reads: 133

```
That makes more sense. I've some more notebook adaptors at work, I'll find one tomorrow. Thanks for the info.
```

---
## \#98 Posted by: chinzw Posted at: 2016-11-15T01:36:52.764Z Reads: 134

```
Be **VERY** careful with that 0.7v cell! If i were you id throw those batteries away and get new ones
```

---
## \#99 Posted by: mmaner Posted at: 2016-11-15T01:59:46.562Z Reads: 138

```
I already have thrown it away. I've got an extra I can out in the pack.
```

---
## \#100 Posted by: JdogAwesome Posted at: 2016-11-15T21:25:26.424Z Reads: 138

```
Hey @mmaner I'm using pretty much the exact same setup as you except im using 4x Zippy 3S 5Ah LiPo's for a 6S2P config. I'm pretty much following word for word @VladPomogaev tutorial on how to setup a charging system for my LiPo's. I ordered this 24V PSU from AliExpress to charge my LiPo's and its a great deal and with it I should be able to charge my board in just a little under an hour at about 9A for a safety margin. Also why did you buy such an expensive BMS if your just bypassing the over current protection anyways lol? 

24V 10A PSU
http://s.aliexpress.com/RRF3URVb 


6S 12A 25.2V BMS
 http://s.aliexpress.com/UFFzEv2Q
```

---
## \#101 Posted by: mmaner Posted at: 2016-11-15T21:55:04.412Z Reads: 139

```
I didnt intend to bypass any protection, I wanted to use the BMS for charge & discharge control.  I dint understand that the BMS doesn't control the discharge, only the cutoff.  Ill be getting another power supply, and Ill try this again, but its going to be a bit as I have a couple of work projects taking up a lot of time right now.  IN the meantime Im gonna use one of the [MEB Simple Charging Port Adapters](http://miamielectricboards.com/shop-1/ez).
```

---
## \#102 Posted by: chinzw Posted at: 2016-11-15T22:30:44.882Z Reads: 141

```
You didn't bypass any protection. You just thought the bms would control each cell independently for everything, but that's not the case.
```

---
## \#103 Posted by: catalin.dragosh Posted at: 2017-04-19T16:04:09.295Z Reads: 115

```
why do you need a 2A charger for the BMS? can't you use a charger with a higher amp value?
```

---
## \#104 Posted by: mmaner Posted at: 2017-04-19T16:05:56.419Z Reads: 110

```
of course you can, but a 2A charger is the minimum and it extends the life of the battery.
```

---
## \#105 Posted by: catalin.dragosh Posted at: 2017-05-02T23:34:45.851Z Reads: 97

```
HI,
I have bought this 6S BMS [here](http://www.ebay.com/itm/321790634514) but it has only 5 wires for balancing?!
Do you know how is the wiring done in this case?
Can this even be used for balance charging 2 x 3S batteries?
```

---
## \#106 Posted by: EvoHub Posted at: 2017-11-07T11:25:45.929Z Reads: 61

```
Hello everyone, do you think you guys could help me figure out how I'm suppose to connect the balance cables on to this BMS balance charger, it's for TWO 4s LiPo batteries = 8s<img src="/uploads/db1493/original/3X/d/f/df409a9bc0a6d9c0e499ba45aed79884acd95515.jpg" width="382" height="500">
```

---

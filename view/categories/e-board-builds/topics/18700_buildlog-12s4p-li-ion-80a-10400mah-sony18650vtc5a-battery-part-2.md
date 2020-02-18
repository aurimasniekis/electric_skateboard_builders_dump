# BUILDLOG: 12s4p Li-Ion 80A 10400mAh (Sony18650VTC5A) battery. Part 2

### Replies: 31 Views: 5036

## \#1 Posted by: 3sly Posted at: 2017-03-07T16:04:19.693Z Reads: 430

```
Hello everyone!

*The construction of the battery is almost complete, unfortunately I had to make a new topic as I can no longer edit the old one (which is only 3 months old)*

I'm back, and I'm tired of running my Multistar LiPo's to the point of failure. (3*4S 10000mAh 10C)
After convincing myself to justify the costs, I ended up pulling the trigger to make myself a sweet 12s4p battery pack. I'll also be making and installing a sparkswitch.

Here are the parts thus far:

* 48 x €5,05: US18650VTC5A Sony Cells (35A/2600mAh) (nkon.nl)
* 13 x €2,8 : 10mmx0.15mm Pure nickel strip (nkon.nl)
* €4,60: [50 pcs of battery holders](https://nl.aliexpress.com/item/Consumer-Electronics-Shop-Free-shipping-1-SET-50x-18650-Battery-Spacer-Radiating-Shell-EV-Pack-Plastic/32601474267.html?spm=2114.13010308.0.0.ifv4hD). I'll probably have to file down the tabs to accomodate the 10mm nickel strips. I didn't end up using them, maybe for another project.
* €80: [BMS 12S 80A](http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html). When charging I'll supply it with a (4,1*12)V power supply to extend the life of the cells.
* 10€: 3 Antispark chaka/vedder 1.4 boards.
* 15,5€: PVC Heatshrink aliexpress.
* ~€20: Parts for 3 antispark boards from Farnell + miscellaneous.
* €63: [CLG-150-48A](https://www.elpro.org/gb/150-w-ip65/35114-clg-150-48a.html): is normally 48V but I found out it can be adjusted up to 56V.
* €10: Voltage/capacity display.

I'll be spotwelding batteries to save the cells from getting to hot. For that I purchased a car battery and a DIY spotwelder of which I'm very satisfied.

I'm excited! Hopefully this will help others as well
Dries

<img src="/uploads/db1493/original/3X/4/6/4672d534658f899587ae2465077af991687d0d64.jpg" width="666" height="499">

This is the spotwelder and battery that I'll be using to assemble the cells:

<img src="/uploads/db1493/original/3X/e/8/e8518cc1be62698706e9fb50d5e11a3e2b22643a.jpg" width="690" height="388">
```

---
## \#2 Posted by: 3sly Posted at: 2017-03-07T16:04:33.399Z Reads: 407

```
Progress;

So a couple of days ago I finally got an adequate car battery to run the spotwelder. I had to return the first one because it arrived with a broken cell and got stuck on 10.58V (it got beaten up during transport). The battery I'm using is a VARTA B18 which is nice and compact but delivers alot (440A) of current.

I first charged all the cells to about 4.08V to see if they are all good and hold a charge. No problems there.

As I'm building a 12s4p and each battery can deliver 20A (They're rated for 30A according to sony, but alot of reviews said that 20A is a more accurate limit), I went with a 80A BMS. Why 80A and 4p? Well, I wanted to make this battery upgrade-proof, so that I can one day step up to a dual hub setup if I want to. According to the Carvon guy (my dream hubs), 80A was plenty for a dual hub setup. 

By doing some research I found out that the 10mm*0.15mm pure nickel strips can safely carry about 10A. That's why I decided to reinforce the outer serial connections with 2 copper wires of 1.5mm². The inner serial connections are made with a double layer of nickel strips, for a total of 8 nickel connections, as you'll see in the pictures.

I did the pretinning before the spotwelding, this saves the cells of being exposed to alot of heat. I also placed the solder blobs in between the cells, for the same reason.

<img src="/uploads/db1493/original/3X/d/b/db7351912867e9b33f3b816dc1394bdff2dfa039.jpg" width="690" height="388">

The inner serial and parallell connections. The battery will be folded open at the end of the process.

<img src="/uploads/db1493/original/3X/3/1/31caf0667b26772a980676f41665c09f2d06fc10.jpg" width="690" height="388">

The outer serial connections:

<img src="/uploads/db1493/original/3X/b/e/be71eaf03383f212377487457bd80b27c26fb56f.jpg" width="690" height="388">

The inner serial connections (4*2 strips) and the parallell connections (1 nickel strip should be plenty as there won't be going alot of current from one battery into the other). The balance leads were also soldered into place at this stage. Please, don't forget to tape of the ends of the balance leads, even though you think you'll be carefull enough :stuck_out_tongue: , trust me haha.

<img src="/uploads/db1493/original/3X/0/d/0d5dbf7b331937aee350e549239a4e622cc77e7b.jpg" width="690" height="388">

Soldering the copper wire to reinforce the serial connections on the outside and to allow enough current to pass through.

<img src="/uploads/db1493/original/3X/1/a/1a075a739d84ff6be4d09a93e9bcc0e34207e8da.jpg" width="690" height="388">

Now comes the fun part, folding open the battery. It's easier if you decide to hotglue the cells to each other before doing this:

<img src="/uploads/db1493/original/3X/5/1/51baab9d30c8421d0706754a552d41702de9ddeb.jpg" width="690" height="388">

Alot of hotglue. This doesn't really damage the cells, low temperatures and quick cooldown. I also made sure to alternate between cells to make sure I don't heat up individual cells too long.

<img src="/uploads/db1493/original/3X/f/f/ffd289dfea334059f3d71fe961e3a2b8e9f74e95.jpg" width="690" height="388">

At the top and bottom I placed a piece of 4mm corrugated soft plastic/foam. This'll protect the cells a bit against scratches.

<img src="/uploads/db1493/original/3X/9/c/9c23767f06b2a46292539589fb39920b2ec9411c.jpg" width="690" height="388">

I decided not to install the BMS before shrinkwrapping it. That way I can always access the essentials if I want to check the connections and make any future troubleshooting alot easier.

<img src="/uploads/db1493/original/3X/e/f/ef6eab5a98e9cfa6f914856a419024ff0e52105a.jpg" width="690" height="388">

I was amazed to see that the 12s4p was alot smaller then I anticipated.

<img src="/uploads/db1493/original/3X/f/4/f4e7d5c61c051bb7556ad671805842fd51be0795.jpg" width="690" height="388">
```

---
## \#3 Posted by: 3sly Posted at: 2017-03-07T16:04:41.384Z Reads: 378

```
Reserved for final updates: assembly of the sparkswitch; mounting of the sparkswitch/chargingport/display
```

---
## \#4 Posted by: Fiori Posted at: 2017-03-07T18:10:39.600Z Reads: 363

```
Awesome build man. I really like the homemade spot welder. Any links to the kit you bought? Or did you make it?
```

---
## \#5 Posted by: 3sly Posted at: 2017-03-07T18:13:01.849Z Reads: 364

```
Didn't make it myself, it's a kit that's gaining popularity on endlesssphere. But I see the price went up after the second batch. It's a very complete kit though. I also see that he now charges extra for the welding leads etc...

I made the suggestion to him to add a schotkky diode. A suggestion I read over at endlessphere to limit the avalanche currents. He now seems to offer this as an option as well. Personally I didn't use them (and had no problems), but if you tend to improve the reliability even further then feel free to add that.

https://www.tindie.com/products/KaeptnBalu/diy-arduino-battery-spot-welder-prebuilt-kit/
```

---
## \#6 Posted by: Smorto Posted at: 2017-03-08T02:26:54.307Z Reads: 329

```
Can I ask how exactly you completed this kit with the foot pedal? I am thinking of buying this kit as well but I want as much info as possible. Any other info about what settings you use and anything else would be great as well.
```

---
## \#7 Posted by: 3sly Posted at: 2017-03-08T17:40:22.656Z Reads: 305

```
I did exactly as the tindie link said. He provides a pdf that contains all the different steps. I think there's even a video on how he uses it. You just need a battery and footswitch. The footswitch is just a contact that temporarily closes. 

The settings themselves, I set it up to about 10ms, that was plenty for proper welds.
```

---
## \#8 Posted by: Smorto Posted at: 2017-03-08T23:09:18.210Z Reads: 275

```
So I need to solder a 12v (3s) battery to the 12v and GND places on the board? Where exactly does the foot switch connect? Which footswitch do you use and what is your exact setup? Really sorry for these stupid questions. Also I couldn't find the PDF download. I looked but one place said I needed to have a 'premium' membership to download.
```

---
## \#9 Posted by: 3sly Posted at: 2017-03-09T01:41:38.656Z Reads: 279

```
No problem. Yes you'll need an extra 12V psu (like a spare router psu) to power the arduino, you can do this also by battery.

The datasheet is on the tindie page, it's at the bottom right: 'datasheet'.

There is a jst-2pin header already in place to connect to the footswitch. You'll also get the female header that you have to solder to the footswitch you bought.

Just a 2dollar footswitch from aliexpress.
```

---
## \#10 Posted by: Smorto Posted at: 2017-03-09T02:01:37.155Z Reads: 277

```
http://www.ebay.com/itm/TEMCo-Aluminum-Foot-Switch-10A-SPDT-NO-NC-Electric-Power-Pedal-Momentary-New-CNC-/281070321451?hash=item417118bf2b:g:NHcAAMXQslhRjWim 

So I would just solder the included female wire to the plus and minus of this foot switch then connect it? And how exactly do you change the milliseconds? Just push the stick button? One last thing, the welder turns on when you connect the 3s battery correct?
```

---
## \#11 Posted by: sl33py Posted at: 2017-03-09T02:11:59.985Z Reads: 277

```
i built mine from scratch and got components from Mouser.  I actually used Kaeptnbalu's code vs the original from github since he had some improvements.

I'm curious which mosfets he uses.  There are the original ones recommended on ES, and a slightly more $ option that was supposed to be more durable.  I got the later ones.  IIRC it was about $60 in parts... so he either got a better deal from quantity discount, or maybe the cheaper mosfets?  the 1324 FETs were the upgraded ones i got.  

Recommend the "Diode Set" he sells as kit for 7$ - it will prevent the 100'ish millisecond avalanche current from damaging your FETs.  Good $ to prevent having to replace all the FETs when one fails (you replace all at the same time even if only one fails).

Read up on the Endless-Sphere thread - tons of good info!

HTH - GL!
```

---
## \#12 Posted by: sl33py Posted at: 2017-03-09T02:13:39.612Z Reads: 264

```
[quote="Smorto, post:10, topic:18700"]
the welder turns on when you connect the 3s battery correct?
[/quote]


I know some folks have had luck w/ super high output Lipo's - but the original is intended to be powered by a car / lead-acid battery not lipo.  I'd stick to what works as it makes a big difference from what i recall.

Re-read what you wrote - i think you are simply asking about powering the arduino to control it - i just pulled the power from the car battery as well, but you could use a separate 3s lipo (i think it takes 7-12v).
```

---
## \#13 Posted by: 3sly Posted at: 2017-03-09T02:17:35.396Z Reads: 246

```
@sl33py But the arduino needs to be powered by another 12V source (which is what he was talking about). You can connect the arduino to the car battery as well, but as the voltage drops when the weld is made, I'm not sure if that will affect the arduino. That's why I suggest running the arduino from a 12V(3s) lipo or a wallpsu.

@Smorto Yes, that's correct. I used this one, even cheaper: https://nl.aliexpress.com/item/THGS-SPDT-Nonslip-Metal-Momentary-Electric-Power-Foot-Pedal-Switch/32719602425.html?spm=2114.13010608.0.0.s0oQBG

I really suggest that you please read that datasheet and watch his video, it explains most of your questions. He explains how you just increase the timing by adjusting a potentiometer, the timing is displayed on a display. The welder turns on if you power the arduino with the external 12V source. The welder welds if you press the pedal and have a car battery connected. Can't go wrong.
```

---
## \#14 Posted by: Smorto Posted at: 2017-03-09T02:39:41.131Z Reads: 230

```
Awesome thanks a ton for the help. I will have to go out and buy the 3s battery as well, any specific Mah or C rating necessary? If it takes almost no power would a simple 9v battery work (almost certainly not but its worth a shot). Either way it's still cheaper than buying a 200+ dollar spot welder from china.
```

---
## \#15 Posted by: phizzle Posted at: 2017-03-10T06:39:19.578Z Reads: 224

```
Great post, I'm gearing up to make one and you've made it much easier for me with something to follow. Cheers!
```

---
## \#16 Posted by: 3sly Posted at: 2017-03-20T13:53:43.467Z Reads: 229

```
No problem!

Yeah maybe a 9V battery might work, maybe you can find some info on that. It's just to run the arduino and display, so it'll probably just use a few mA (so any battery wof the right voltage will be plenty).
```

---
## \#17 Posted by: Smorto Posted at: 2017-03-20T16:53:18.327Z Reads: 222

```
A 9v has around 500 mah, do you think that would work?
```

---
## \#18 Posted by: 3sly Posted at: 2017-03-21T11:46:54.073Z Reads: 214

```
Not sure, depends if an arduino can run of a 9V battery. Worth a shot. The mAh isn't really that important, because the arduino uses negligible currents.
```

---
## \#19 Posted by: sl33py Posted at: 2017-03-21T22:17:09.991Z Reads: 204

```
I have a 9v rechargeable i can test w/ my spotwelder - simple enough.  let me check tonight and i'll let you know.
```

---
## \#20 Posted by: aras_96 Posted at: 2017-03-21T22:28:46.954Z Reads: 211

```
Hello, this is my first post, so please be patient with me.

I have an initial idea of what my longboard build will be. Atm i have already purchased the following: 
- Longboard Deck, 
- Caliber II Longboard Trucks, 50 Degrees.
- Orangatang Kegel 80mm Wheels.
- 30 Teeth HDT 5mm Pitch 11mm wide wheel pulley
- 20 Teeth HDT 5mm Pitch 11mm wide motor pulley.
The pulleys have already been drilled and connected to the wheels.

I'd like to create a 10s4p Samsung 30Q battery pack. But im unsure about what type of bms i should buy, if you have any recommendations please provide them, or if you can teach me about how to pick a bms, that would be greatly appreciated.

I would like to get dual Turnigy Aerodrive SK3 - 6354-260kv, and dual vesc.

What are your thoughts and comments will be appreciated
```

---
## \#21 Posted by: Smorto Posted at: 2017-03-21T22:35:54.877Z Reads: 191

```
Awesome! That will be great to know.
```

---
## \#22 Posted by: Smorto Posted at: 2017-03-21T22:40:52.807Z Reads: 189

```
First off, this post should be in its own thread or at least not this one IMO since it is slightly off topic. However, it is your first post so I'll let it slide :slight_smile:. I think that you should read a little more on your gear ratios because 30t is a little low for your wheel (but doable) and 20t is much too high for your motor (not doable). Also 11mm wide belts will be hard to find but I bet someone makes them :slight_smile:. Also 260kv and 10s is too high for the VESC and you run the risk of blowing it. The 260kv motor combined with the high gear ratio will leave you very little torque. I would recommend dual 6354 or 6355 190kv sensored motors for the best mix of torque, speed, and smooth acceleration. Also do you have anything for a motor mount? Didn't see anything listed. Sorry for the long response :slight_smile:.
```

---
## \#23 Posted by: aras_96 Posted at: 2017-03-21T22:47:29.682Z Reads: 183

```
Thank you very much sir, haha, soz i'll make a new post, but i cant find the new post button.

I'll be making the motor mount myself, something similar to thoses on the market, im a student so i dont have the money to buy straight from them. 

ive seen people using 36teeth to 16 teeth, so i assumed it would be alright to go slightly lower as it showed on the online calculator that i would gain higher speeds, but weaker torque.

if i kept these pulleys, and purchased a 190kv motor at 10s or 12s would i be able to reach 30+ mph?
what if i purchased the 260kv and used 8s instead, i read that it would be better, and workable with the vesc. but im trying to go high speeds.
what do u think?
```

---
## \#24 Posted by: Smorto Posted at: 2017-03-21T23:16:49.804Z Reads: 180

```
If you go with that gearing ratio and motor you will have to kick push from a standstill (not a huge deal) but you will have very little torque for hills.... 

As for 30+...yes, definitely http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":20,"wheel-pulley-teeth":30,"wheel-size":90}|

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":260,"system-efficiency":80,"motor-pulley-teeth":20,"wheel-pulley-teeth":30,"wheel-size":90}|

However, the torque really won't be there and I think that the loss in torque will make for not as fun ride but that is 100% up to you, and who knows? Maybe you will enjoy it :slight_smile:.
```

---
## \#25 Posted by: aras_96 Posted at: 2017-03-21T23:21:39.767Z Reads: 165

```
I see, so if i went with the 190kv and those pulleys, do u recon it could go up a 15 degree hill at a decent speed.
what pulleys do u recommend 
and thanks for the reply and help

Love aras.
```

---
## \#26 Posted by: Smorto Posted at: 2017-03-21T23:32:02.577Z Reads: 168

```
Honestly I'm not sure, maybe some more experienced people can comment but I am not sure, maybe @JuniorPotato93? I know he has done a lot with pulleys. I would recommend DIYes pulleys (16/36) because they are quality products, and affordable.
```

---
## \#27 Posted by: Smorto Posted at: 2017-03-23T01:47:59.025Z Reads: 160

```
Did this ever happen? Just curious, not any pressure or anything :slight_smile:.
```

---
## \#28 Posted by: JuniorPotato93 Posted at: 2017-03-23T03:04:04.932Z Reads: 167

```
Honestly, the pulley you require is going to be based more on your riding set up as well as the rider. If you want to do 15 degree hills and you're light as a feather then by all means go for a smaller ratio if you also want speed but if you're built more like me and are 200+ and have your backpack or gym bag and that's another 20 lbs then youll have to go for aarger pulley regardless. You'll need to know your motor torque value and the desired gearing ratio and your weight and desired speed to know what gear you should be using really but then you should also make sure that is within the power requirements of your set up too so you don't blow the whole thing.
```

---
## \#29 Posted by: sl33py Posted at: 2017-03-23T17:46:26.951Z Reads: 160

```
Not yet.  I'll try to get it done this weekend.  Been a bit hectic and slipped my mind.
```

---
## \#30 Posted by: Smorto Posted at: 2017-03-23T21:21:10.982Z Reads: 157

```
Awesome, let me know if you do it :slight_smile:.
```

---
## \#31 Posted by: tonystark Posted at: 2017-05-09T14:24:07.073Z Reads: 123

```
I really like your built. Looks like you know what are you doing. Yeah, this welding kit is preaty expensive: 67€. Plus a car battery will cost atleast 60 if not a 100$. I think i will just buy spot welder on aliexpress if i cant make my own out of microwave transformer. Thanks
```

---

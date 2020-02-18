# Evolve Carbon (Gen2, non GT) FOCBOX Upgrade

### Replies: 70 Views: 2942

## \#1 Posted by: AlexBE Posted at: 2018-09-08T23:22:31.776Z Reads: 268

```
The battery on my old Evolve Carbon, not sure if it would be called Gen1 or Gen2, but it't the non-GT version with the single large rear motor, is dying. The fundamental problem is that the BMS cuts power to the board as the battery voltage gets too low. It's very annoying that Evolve designed this thing to not limit current to prevent the BMS cutout.

I pulled out the old ESC/Control system and replaced it with a FOCBOX and Nano-X controller. The increase in power/torque is mind blowing. Of course part of the reason for the torque increase is that no doubt I am running a much higher motor current than the original controller does. Does anyone know the approximate settings for the stock ESC? My new settings are 40A motor and 20A battery, the back wheel (pneumatic) can spin at low speed and the acceleration to top speed is probably twice as fast.

I am considering further increasing the motor/battery current because I don't really mind if I break this motor. At the moment it is barely getting warm and previously it got hot. Maybe this is a function of FOC and better control algorithms wasting less power even though the board output is much higher.

Seriously considering building a dual motor setup for this thing now, new lease on life!

The other huge advantages

* The BMS now never shuts down to protect the battery because the FOCBOX current limits and prevents the battery voltage getting low enough for that to happen.
* Much better braking (to a complete stop)
* FOC seems much quieter (faster, more efficient?)
* Controller has longer throw, better feel.
* Bluetooth monitoring of all ESC parameters like temperature, power etc.
```

---
## \#2 Posted by: Eboostin Posted at: 2018-09-09T00:32:27.215Z Reads: 239

```
That’s awesome! I always wanted to through a VESC in one. The motor is one of the quietest so can only imagine how quiet it is in FOC

Post up some pics if you can
```

---
## \#3 Posted by: natch Posted at: 2018-10-27T20:19:04.922Z Reads: 207

```
Hi, I'm very interested in this. I have an Evolve bamboo gen2 and I have the same SAG problems. Can you explain to me how you have replaced is ESC by the focbox? I would really appreciate it if you send me the photos and explain the process. Thank you!
```

---
## \#4 Posted by: Arzamenable Posted at: 2018-10-27T20:43:07.161Z Reads: 208

```
I would just titrate motor amps off heat. 

For reference:
“To find out what current the motor uses I plugged a Watts Up meter (also with T plugs) in between and it ended up being a whopping 24A! and a constant load of about 12-15A to hold a speed of about 28Kmh. (it is a 350w motor after all)”

https://secondlifestorage.com/t-Evolve-Skateboards-Range-Extender-Battery-upgrade
```

---
## \#6 Posted by: Arzamenable Posted at: 2018-10-27T20:53:55.570Z Reads: 193

```
This project basically means getting a new BMS, motor controllers, on/off switch, remote and receiver. At least for the evolve carbon GT, the battery bms, remote, and stock motor controllers are proprietary and don’t tolerate any tinkering. You can only change the motors or the battery (requiring a bms transplant). 

I might be wrong about the gen 2, but the gen 3 boards don’t like to be tinkered with unless you change everything. @psychotiller and @longhairedboy do battery swaps with bms exchanges if you are state side.

Not to self promote, but here is the unreliable shitshow that ensued after bumbling my own evolve battery exchange. 

 https://www.electric-skateboard.builders/t/diyvolve-quad-evolve-carbon-gt-evolve-supercarve-surfrodz-tpk-psychotiller-6369-200kv-x-4-unikboards-63mm-evolve-mounts-12s7p-30q-diebiems-focbox-x-2-fesc-6-6-x-2/71424?u=arzamenable
```

---
## \#7 Posted by: natch Posted at: 2018-10-27T21:57:57.813Z Reads: 172

```
Thanks! 

Unfortunately I live far away, in Spain. Then as I bought a 1 x Nano-X & Focbox Bundle I would need a bms and a power switch. Any recommendation? Is it easy to replace the bms of the original battery? many thanks!
```

---
## \#8 Posted by: AlexBE Posted at: 2018-10-28T00:37:01.429Z Reads: 165

```
Ignore what @Arzamenable said about the BMS, he has the GT and he is wrong about the Gen2.

To upgrade the Gen2, you only need to remove the ESC and remote receiver and replace those with a focbox and nano-x receiver. You do nothing with the BMS. The main feature you lose is the on/off switch. I have used an XT-60 connector and a loop-key. I did plan on adding an antispark switch but will be going dual motor with the Unity and so an additional switch is not required.

I will try to take the board apart later today and post some photos.
```

---
## \#9 Posted by: AlexBE Posted at: 2018-10-28T00:39:33.422Z Reads: 160

```
I'm not 100% sure what you are showing here, is this the difference in width between Gen2/GT trucks, and a modified Evolve (gen2?) truck adding a second motor mount?
```

---
## \#10 Posted by: AlexBE Posted at: 2018-10-28T00:42:19.996Z Reads: 150

```
This is essentially what I did, just kept ramping up the motor current based on temperature. I am currently running it at 50 motor amps and it stays cooler than it used to stock.
```

---
## \#11 Posted by: Arzamenable Posted at: 2018-10-28T01:55:27.315Z Reads: 153

```
Two gen 2 AT trucks mashed into 1 for a dual setup sometime. 

I sold my gen 2 bustin evolve awhile back. I assumed the bms situation was the same. Thanks for clearing up bump scoop. 👍
```

---
## \#12 Posted by: natch Posted at: 2018-10-28T05:43:40.026Z Reads: 155

```
Thank you very much you two. I will then keep the bms. I would be very grateful if at some point you can send me pictures of the assembly, the connections and how you fixed the focbox to the case. I'm new to this, I'm reading a lot here, but I have not started yet. Would it also be possible for you to export the focbox configuration and send me a file or something?👍👍👍
```

---
## \#13 Posted by: natch Posted at: 2018-10-28T10:33:30.689Z Reads: 146

```
Which on/off switch do you recommend?

This one looks very good https://lunacycle.com/remote-on-off-solid-state-switch/, 
but with the shipping is $60 ...

I just found this one, what do you thing?
https://eskating.eu/product/anti-spark-power-switch/
```

---
## \#14 Posted by: natch Posted at: 2018-10-29T10:37:51.646Z Reads: 131

```
I think that im going to order this one

https://eskating.eu/product/anti-spark-power-switch/

for the original bamboo battery gen2 and the focbox bundle, shallI order it with xt60 connectors on both ends? What fuse do i need?

Thanks!
```

---
## \#15 Posted by: Superflim Posted at: 2018-10-29T13:04:13.716Z Reads: 126

```
Electricboardsolutions has also anti spark
```

---
## \#16 Posted by: natch Posted at: 2018-10-30T17:21:03.321Z Reads: 124

```
Hello @AlexBE can I ask you how you have connected the hallsensor of the Evolve engine to the entrance of the focbox?

The output of the sensors is through a 5-pin XH connector and the focbox input is a 6-pin JST PH 2mm.

Thanks!
```

---
## \#17 Posted by: b264 Posted at: 2018-10-30T20:02:15.755Z Reads: 126

```
[quote="natch, post:13, topic:67458"]
I just found this one, what do you thing?
[/quote]

The customer service there is really, really bad
```

---
## \#18 Posted by: AlexBE Posted at: 2018-10-31T01:30:54.050Z Reads: 128

```
Hey, I actually just directly soldered the wires to the pins, not sure if the pinout even similar. I would use proper connectors but given this setup is temporary (until my Unity arrives), soldering was the fastest. I would suggest buying and crimping new connectors for a more permanent setup.
```

---
## \#19 Posted by: AlexBE Posted at: 2018-10-31T07:19:06.291Z Reads: 128

```
Oh, beware the pinout label on the FOCBOX is not correct. On mine at least.
```

---
## \#20 Posted by: natch Posted at: 2018-10-31T07:33:54.880Z Reads: 138

```
Thanks, Is this the right one?

https://enertionboards.zendesk.com/hc/en-us/articles/115000952453-Pin-map-on-motor-sensor-on-the-PCB-does-not-match-the-sticker

the engine has only 5 wires, I suppose they are 5v, GND, H1, h2 and h3, right?
```

---
## \#21 Posted by: AlexBE Posted at: 2018-10-31T08:14:02.158Z Reads: 139

```
Yes. Normally Red, black, and three colours for the hall sensors.
```

---
## \#22 Posted by: natch Posted at: 2018-11-01T07:46:58.902Z Reads: 137

```
Another question, how did you mount the focbox on to the heatsink, do you have one of these?

https://www.electric-skateboard.builders/t/evolve-heatsink-for-dual-focboxs/59619
```

---
## \#23 Posted by: AlexBE Posted at: 2018-11-02T00:17:30.338Z Reads: 123

```
I actually have mine just stuffed into the enclosure with some foam. I had planned on mounting it to the stock heatsink with screws by drilling the matching hole pattern. However I have found that it barely gets warm (via bluetooth telemetry) and so haven't bothered doing that yet.
```

---
## \#24 Posted by: natch Posted at: 2018-11-09T14:54:12.551Z Reads: 116

```
Hi again, I have another question. How did you manage to put the focbox inside the enclousore? It does not close because it's too high with the original case and without it i'm afraid It could get overheated since the mosfets would not be in contact with the heatsink.
```

---
## \#25 Posted by: AlexBE Posted at: 2018-11-11T00:34:09.425Z Reads: 115

```
Im not sure what you mean, the board's enclosure has loads of room for the focbox, i had to stuff it with foam to stop everything from rattling around...
```

---
## \#26 Posted by: natch Posted at: 2018-11-11T12:04:01.266Z Reads: 107

```
Ummm, in my enclusure the focbox doesnt fit because of the height. My focbox is the one with the black case. Maybe you have the one with the blue case and is lower..
```

---
## \#27 Posted by: natch Posted at: 2018-11-16T10:57:09.777Z Reads: 119

```
In the end I managed to make it work. Thank you very much for your help. Next steps, make an upgrade of the engine and the battery. Step by Step!
```

---
## \#28 Posted by: AlexBE Posted at: 2018-12-17T06:21:06.339Z Reads: 117

```
Update:![IMG_20181217_141405|375x500](upload://qbMj9CfVllMLjmyO48Ke2Qm1Mnn.jpeg)

* Replaced battery with 30Q 10s5p from @Marsen. Had to 3D-print a 6mm spacer to fit the battery in.
* Replaced original motor with SK8 6354-140KV, cut out a basic 6mm aluminium bracket.
* Added idler pulley to see if that changes anything.

Next steps
* Wait for my damn Unity controller.
* Weld 2nd motor bracket onto trucks and mount second motor.
```

---
## \#29 Posted by: AlexBE Posted at: 2018-12-17T07:40:03.756Z Reads: 115

```
![IMG_20181217_153338|666x500](upload://1NqYePEUXXuqlakMRUUpOmQjzsW.jpeg)
```

---
## \#30 Posted by: ricardo Posted at: 2018-12-17T08:18:37.100Z Reads: 113

```
Nice build!

I too have a Evolve Carbon Gen II which I modified with 2x maytech motors with GT trucks and Unik mounts; 2x FOCboxes, 10s7p battery and the Photon remote.

Let me know if you want a detailed parts list! ;-)
```

---
## \#31 Posted by: AlexBE Posted at: 2018-12-17T08:21:24.985Z Reads: 109

```
Oh WOW! I would love to see photos. 7p! you are nuts. I don't want to use the GT trucks because of the large decrease in width, I like the wheel base of the Gen2.

What kind of range do you get out of that thing? Pnumatics?
```

---
## \#32 Posted by: ricardo Posted at: 2018-12-17T08:30:25.553Z Reads: 108

```
Will try to find some photos tonight!

I haven't yet tested how much range I have now, basically because I haven't been on the board long enough (either through being tired or by doing all my errands and ride routes) One day I'll try to do a serious range test! ahah!

The decrease of width of the trucks, combined with using the Trampa urban threads on Superstar hubs, makes the board equally stable but more responsive and "pointy". This means you can still carve and coast along as much as you want, but also be sharper and faster on bends.

\o/
```

---
## \#33 Posted by: AlexBE Posted at: 2018-12-17T08:36:28.496Z Reads: 108

```
I suppose you can get an estimate of range by streaming telemetry to your phone, then checking how many Wh/Km you are using. I think that probably overestimates my range though.
```

---
## \#34 Posted by: AlexBE Posted at: 2019-01-04T08:41:44.297Z Reads: 112

```
![IMG_20190104_164003|666x500](upload://oErZOnIS20oNPFXf1JFQlstP20u.jpeg) ![IMG_20190104_164012|666x500](upload://eP6s71Zy4SE0f7aCAfGAJxiRSFR.jpeg)

Completed the upgrade to add the second motor. Torque!
```

---
## \#35 Posted by: b264 Posted at: 2019-01-04T09:08:21.873Z Reads: 109

```
[quote="ricardo, post:30, topic:67458"]
10s7p battery
[/quote]

You fit a 10S7P battery in there?  I modified one as well but it has a 10S6P
```

---
## \#36 Posted by: ricardo Posted at: 2019-01-04T09:20:51.818Z Reads: 110

```
Very *VERY* tight squeeze. Was supposed to be a 10s6p, but my supplier COFCOF @darkkevind COFCOF thought I had asked for 7p. :-D

I only noticed when we were assembling the whole damn thing, but don't regret it one single bit. I have yet to run  the board for long enough to have a feel for the range of the beast.

Need to post up some photos...!
```

---
## \#37 Posted by: okp Posted at: 2019-01-04T09:24:54.998Z Reads: 106

```
great job man.
```

---
## \#38 Posted by: b264 Posted at: 2019-01-04T09:25:21.571Z Reads: 108

```
Where did you put the BMS?
```

---
## \#39 Posted by: Arzamenable Posted at: 2019-01-04T09:26:40.028Z Reads: 109

```
Nice! I didn’t realize you were talking about a 2nd Gen Carbon. (I know the title clearly says so). Randomly, I just bought a busted 2nd gen carbon on eBay today with plans to do something like this later. 🤙
```

---
## \#40 Posted by: ricardo Posted at: 2019-01-04T10:25:15.636Z Reads: 108

```
The BMS is not that big, so it's stuffed on top of the Focboxes. I used a 6mm gasket to add space for the batteries and electronics.
```

---
## \#41 Posted by: AlexBE Posted at: 2019-01-05T06:45:59.490Z Reads: 108

```
Yep, 6mm required to clean 18650s.kind of annoying as you lose the extremely thin original look.

I just went for my first decent ride after adding the second motor, I have too much torque. :slight_smile:
```

---
## \#42 Posted by: NYCDiesel Posted at: 2019-03-12T03:51:32.755Z Reads: 104

```
Damn I'm so happy I found this thread, I have a  Carbon Gen 2 AT w/ a recently installed 10s6p 30Q pack that I installed in it last week. .I want to upgrade the motors ( BTW AlexBE your board is fucking SICK ) at some point but after reading this I want to uprade to the focbox for the increased amperage as well as being able to use the nano remote. I ordered a gen 2 POS replacement remote and it was 90 fucking  dollars ! WTF?

So my plan is to install the focbox but I see that they havea unity controller but is that only for dual motors rigt ? Could I use it to increase te amperage on mysingle motor then when it dies add on dual motors ? 

For some reason I can't private message so AlexBE if you could email me at jzsupramecy@aol.com, I have a couple question  for you if you don't mind, thanks a lot guys.
```

---
## \#43 Posted by: AlexBE Posted at: 2019-03-12T04:30:16.669Z Reads: 105

```
Might as well just ask any questions in this thread so everyone can see and search the information. Not sure why you can't PM me. My upgrade sequence went
* Add FOCBOX and Nano remote. Main benefit is increased motor current and soft current limiting to avoid the Evolve BMS suddenly cutting power to the system. No idea why the Evolve motor controller allows the BMS to be constantly activated. With this upgrade the board can be ridden safely because there is no unexpected loss of power. Also the FOC doesn't seem to bother dogs.
* A few months later. Upgrade battery to 10S5P 30Q. This mostly just increases range and power.
* Then change the motor to a 6354 SK8. I only did this because I knew I was going to change to dual motor when my Unity arrived. In reality I don't believe this is a performance increase. The stock motor is much larger and being an inrunner I think has better thermal transfer between the windings and the case/environment.
* Unity arrived and went straight in. No performance increase over a single focbox but to answer your question, yes you can run a single motor with a Unity.
* Figured out how to weld aluminium and then added the second motor bracket when I got a spare weekend. Massive performance increase. No more torque steer or torque in braking. Way too much torque for me to hold because of the low gearing. Definitely easier to just buy a Gen 3 axle assembly, but less fun and you lose the Gen2 width.

Main thing I need to add now is a BMS for charging. I have been charging to 41V to be slightly safer, but I opened the thing up after 50 charges and the battery is balanced to 2mV.
```

---
## \#44 Posted by: NYCDiesel Posted at: 2019-03-12T10:16:44.126Z Reads: 103

```
I think it may be because I just joined the forum, really not sure.

Much thanks for the in depth reply, I didn't know how frequently you checked the forums/thread but totally works for me. I have an upgraded BMS in my pack as well, I'm awaiting the battery builders (Pelicanbayinnovations) answer to exactly which one, he said was that it was "beefier" then stock.

So the 6354 itself wasn't an upgrade until you went dual huh. I live in a small apartment so I can't do anything to crazy like welding ( on a side note would you be willing to weld a motor mount for $?) so for now I was thinking about upgrading the motor to a SK8 6374 192kv for now. Do you think this will provide a more noticeable power increase ? 

My main goal , eventually, is to have a dual motor config with the stock trucks (not sure how exactly yet) but for now I don't mind the single motor setup. I am a big guy and the board  gets me up some gnarly hills but then again it is my first board and like every other hobby of mine (snowboards, motorcycles, drones etc.) I do always end up upgrading to something bigger and better eventually.... 


I hear what yoursaying about the GT trucks but I love the stance of the gen 2, especially since I wear sz 13 shoes.  The AT setup trucks through even the most gnarly of NYC streets... Is their any other way to install a secondary motor plate? Since I have a 10s6p already do you think I would gain anything from a Unity ? I REALLLYYYYY want to get rid of this POS remote, I had to order  a replacement for a ridiculous 90$! The thing sucks huge gorilla nuts too, it has no telemetry, no charge LED, nothing that makes it worth that much money. So I was thinking about the focbox and the nano remote, unless you guys can recommend some other system ? 

Sorry for rambling, I'm just excited to find people I can talk to about this  shit. on Evolves boards it was crickets chirping haha, thhanks for any help guys. And BTW AlexBE, your setup is too got damn sexy looking ha, I'll trade you a kawasaki zx10 for your board dead serious lol
```

---
## \#45 Posted by: AlexBE Posted at: 2019-03-13T02:33:46.790Z Reads: 93

```
I suggest not using a discharge BMS, I would use charge only. If you are using a FOCBOX or Unity, rely on that to not over discharge your battery. A discharge BMS failing would be very very bad if you were going fast.

The 6354 was possibly an upgrade, but wasn't huge. I probably could have pushed it a lot harder, but it was very hot outside at that time and I am conservative with motor temperature. I would guess it was a torque upgrade, but got a lot hotter than stock. 6374 will be a monstrous improvement. Single 6374 is similar power to 2 x 6354.

If you run single motor, just get a focbox, they are a lot cheaper than Unity (I think). I can't help you with second motor plate as it looks like you are in NYC and I am in Western Australia. I bet you can find someone locally though, it doesn't have to look pretty.
```

---
## \#46 Posted by: NYCDiesel Posted at: 2019-03-14T11:24:19.008Z Reads: 109

```
The builder of my battery pack says that the BMS was spare one that he just had and he says it is "stronger" but aren't BMS just to charge and balance the individual cells ? I build and fly FPV drones and it's funny but a lot  of the electronics are similar.  Motors range in size from 2205 - 2305 with KV from 1500-3000kv+ depending on  size and voltage. Batteries are from 3-6s and generally from 1000-2000 mah so I do know about lithium batteries and the importance of balancing cells, so this statement from the maker of my battery pack that it is generic and "stronger" is a bit unnerving. I will press for more info, I could always tear the heatshrink and take a look.

Alex its funny you mention cutouts because yesterday, for the first time ever, I had numerous cutouts when riding.The motors would spin for a few seconds then just stop, eventually after turning the board and remote off a few times it worked, but I felt like it was lacking power and torque. I was using a new remote that arrived yesterday, however, and today I opened and repaired the original remote and will test ride it today to see if the cutting out persists.

I really would love a dual motor setup but if a single 6374 motor will provide comparable power, I may have to just go for that. Can you bolt a 6374 straight onto the stock motor plate ? I love the look and torque of dual motors but I never have ridden offroad, so I think a single motor/single wheel setup will be ok for my city riding because it was working well for me when I first installed the 60 cell pack, enoug power to go up any hill and minimal torque steer, if any. And honestly,  I want to just get this setup going with minimal investment because I just found out about lacroix boards   :star_struck:  They look so sweet but I know if I get one ASAP then my poor Carbon will no longer be loved so I have to give her a decent fighting chance. What is the general consensus on the lacroix boards ?
```

---
## \#47 Posted by: topcloud Posted at: 2019-03-15T17:36:59.541Z Reads: 106

```

LaCroix is terrific, and our take on it with Surf Rodz and 13s is in finals, right now:

![52574056_2055527254562813_4628935259923152896_n|373x280](upload://76BuCgX7lqs1WJNwMndXUnUP0y6.jpeg) ![52540420_2180604775329691_8569642945995603968_n|280x383](upload://48onjHN0XkbUebxcbMJYk97YBHr.jpeg) 

I will still keep this, however:

![fullsizeoutput_2124|349x500](upload://ztrxDWAzHfxjyjFdkHCQpXiaU1D.jpeg) ![qQ69Q25bQpSlTKT0CYz7KQ|666x500](upload://lYzSN7kRFIgud1diOlLBeWqRrPR.jpeg) 

@BillGordon and @DAddYE are the pioneers on the eLofty drive (I bought the Metasurf that BAESK8 destroyed :slight_smile:) - and the eLofty drive is an axial drive that's mounted on DKP trucks:

https://www.ebay.com/itm/Electric-Skateboard-Accessories-Direct-Drive-Motor-Double-Trucks/153411663276?hash=item23b80c35ac:g:haUAAOSwVbhchndB

which work with these new wheels: 
![TORQUEBOARDS_110MM_WHEELS_2_2048x2048|690x460](upload://AnbAOkNmfeZKti8ntXchiTZTgSJ.jpeg) 
https:///collections/pre-order/products/110mm-really-big-wheels-tb110

I just ordered the eLofty drivetrain and TB 110 wheels for my Gen2 Carbon, and I have a feeling that it will be the first and last "Evolve" I ever actually like - even with the world's fastest LaCroix right next to it.

The eLofty on the 110 mm should, by all accounts, deliver a perfectly quiet, zero-maintenance Gen2 with heavy thane that will stay put when turning at the bottom of a hill, and not shake loose on pavement-to-plate transitions.  

We'll see in a couple of weeks :) good hunting
```

---
## \#48 Posted by: topcloud Posted at: 2019-03-15T22:27:53.758Z Reads: 96

```
@AlexBE would you happen to have the file needed to print this spacer for the enclosure?  I've tried search and have struck out.  Thanks my brother 

![image|666x500](upload://uXsDE9l8KC6ia8oRzw118HdsAyP.jpeg)
```

---
## \#49 Posted by: b264 Posted at: 2019-03-15T22:49:15.722Z Reads: 96

```
@topcloud I could badly use that spacer also :smiley:
```

---
## \#50 Posted by: topcloud Posted at: 2019-03-15T23:43:30.075Z Reads: 92

```
right on brother 

ok, anyone wants to print & sell me a few of these for the gang, ready to buy just LMK :)
```

---
## \#51 Posted by: AlexBE Posted at: 2019-03-15T23:44:20.830Z Reads: 93

```
Hey, I race drones also! BMS can do some subset of a bunch of things. Over voltage, under voltage, balancing etc. You probably have to make your own motor plate. It's fairly easy, even with basic tools because aluminium is so soft. If you have a drill and a file you can do it with a piece of 6-10mm aluminium plate.
```

---
## \#52 Posted by: AlexBE Posted at: 2019-03-15T23:53:08.541Z Reads: 101

```
[quote="topcloud, post:48, topic:67458"]
would you happen to have the file needed to print this spacer for the enclosure? I’ve tried search and have struck out. Thanks my brother
[/quote]

[quote="b264, post:49, topic:67458"]
I could badly use that spacer also
[/quote]

The spacer is really simple, the idea being that you can print it in parts. Hopefully the boards are similar enough that this will fit, I had to do a fair amount of tweaking to get it snug. The parts have a little channel in the top to put some neoprene/rubber in for a watertight seal.

https://www.thingiverse.com/thing:3494699
```

---
## \#53 Posted by: NYCDiesel Posted at: 2019-03-16T14:48:53.646Z Reads: 105

```
Sweet thanks for that file dude, I may be able to have a friend print it and be able to make a few copies so as i know I will let u guys know. 

Topcloud, that lacroix looks beautiful man. What did you guys do to it ? I know a local guy who has one who says he will let me try his before I place my order, just to be sure. I think 40mph is plenty for me as it is haha. Thanks for the links as well, those direct drive trucks look pretty interesting. I know hub sucks, belt is good and is direct drive best ? It would seem like it, no drivetrain loss and ease of  maintenance. That price is kind of steep ttough for such a low  KV motor, do you know if their are any oter options ? 

Alex thats so funny you fly drones too lol. I started FPV first then  came to esk8, they are both more addictive then crack lol. First of all would a 6374 motor just bolt up to the stock motor mount ?? And how did you actuallly get the mount onto the truck ? Thanks for all the help so far my dudes
```

---
## \#54 Posted by: topcloud Posted at: 2019-03-16T17:16:17.884Z Reads: 109

```
thanks bud, hope you make it out sometime to roll with us

@Sender is the first to put Surf Rodz on the LaCroix, and our build is credited to him.  Check out his posts for 'build of the year' and you'll see why we voted his LaCroix Best in Show.

@psychotiller is our friend, one of the best indie builders in America and builder of my LaCroix 13.  We're sticking with Psychotiller motors, fat belts and Six Shooters, as pictured.

Brother Sender has since evolved his LaCroix to include a @3DServisas gearbox on their custom 240 mm Surf Rodz hangers, reverse-mount motors, OnStar 24/7 roadside assistance, etc.:  https://www.electric-skateboard.builders/t/group-buy-fatboy-mini-urethane-gear-drive-fatboy-solid-cnc-hanger/73191/89?u=topcloud

@DerelictRobot's LaCroix is the way to go if you want Trampa-style, fluid carving with the consistency that only springs can deliver  https://www.electric-skateboard.builders/t/cascadia-carver-lacroix-prototipo-deck-trampa-ultimate-trucks-7-ss-kaly-nyc-4-1-gear-2x-flipsky-6-6-maytech-170kv-6374-sealed-hoyt-st-puck-10s6p-samsung-30q-pack/73770 

LaCroix Factory is ok.  Replace the plastic MBS base plates with MBS' new metal base plates; there's an entire thread here, on that topic.  Hoyt Controller is always suggested.  For wheels and tires, call me biased :) yet there's nothing that looks as good as Trampa CNC Superstars with Urban Tredz tires:

![st80GErlQSKWkv19ncB29A|666x500](upload://dYiAJo9qeJJMp8HkIZnX294VkVo.jpeg) 

Absolutely, 100% recommend CNC wheels over the plastic factory MBS Rockstar 2 wheels - don't get me wrong, MBS makes fine plastic wheels and they're great for the trail, I own 5 sets of their wheels - yet CNC makes a meaningful difference on pavement by delivering always-consistent performance.

If I had to upgrade one thing only: easy, the plastic base plates.  The plastic ones have broken on a few of us.  Maybe write LaCroix and ask them to install them on yours, they're good people.

Good hunting!
```

---
## \#55 Posted by: AlexBE Posted at: 2019-03-18T01:02:02.745Z Reads: 96

```
[quote="NYCDiesel, post:53, topic:67458"]
First of all would a 6374 motor just bolt up to the stock motor mount ?? And how did you actuallly get the mount onto the truck ?
[/quote]

No I don't think so. The mounting hole spacing is different. You will need to make (or buy) another mount. I just used 6mm aluminium plate. no doubt something off the shelf could be adapted to the evolve 3 hole pattern.
```

---
## \#56 Posted by: NYCDiesel Posted at: 2019-03-24T04:27:30.239Z Reads: 95

```
Yea that is a good idea. What I was wondering was how did you get the second motor mount onto the truck ? 

Lacroix does look pretty friggin sweet.... How do you think it compares to the trampa Kaly board ? They seem very similar.
```

---
## \#57 Posted by: topcloud Posted at: 2019-03-24T08:21:58.224Z Reads: 94

```
https://www.facebook.com/nyceboarding/

Every question you have about LaCroix vs Kaly can be answered by the members of NYC - and you can see the boards for yourself, first-hand.

They’re not comparable, in my opinion. The ride is completely different. Good hunting.
```

---
## \#58 Posted by: NYCDiesel Posted at: 2019-03-24T14:13:29.798Z Reads: 88

```
Hey thanks for that group link man, will definitely make me find some locals.

I have seen the Kaly board in person but it seemed a little narrow and I have pretty big feet so I am leaning more towards the lacroix.
```

---
## \#59 Posted by: hornet90 Posted at: 2019-03-31T15:14:45.662Z Reads: 79

```
What size feet do you have
```

---
## \#60 Posted by: NYCDiesel Posted at: 2019-04-05T07:00:07.573Z Reads: 79

```
13 Wide 

If you got some thoughts on the subject please share
```

---
## \#61 Posted by: NYCDiesel Posted at: 2019-04-05T10:55:44.621Z Reads: 82

```
I'm going to put a deposit later on the Kaly xl 2.0, with the upgraded wings I think it should be perfect.... will update after I test ride.
```

---
## \#62 Posted by: hornet90 Posted at: 2019-04-07T05:55:42.382Z Reads: 75

```
I have a kaly xl its a beast. If i tought i would be out more over the next 2 years i would order the 2.0
```

---
## \#63 Posted by: Anton77 Posted at: 2019-04-11T15:36:47.935Z Reads: 71

```
@ricardo I’m modifying a Gen2 Evolve Carbon skate board to make a dual motor setup. Could you send me some pics of your setup? Also is it possible to fit 6374 motors in the GT Truck with Unik motor plate mounts?
```

---
## \#64 Posted by: ricardo Posted at: 2019-04-11T18:34:22.620Z Reads: 72

```
yeah, it's possible... but frankly there's no need for it.

all the pics I have of the build are in my thread, unfortunately didn't take any more... :-/

https://www.electric-skateboard.builders/t/evolvenstein-carbon-gen2-enertion-focboxes-maytech-motors-unik-mounts-trampa-wheels-photon-remote/79866
```

---
## \#65 Posted by: RufioBangarang Posted at: 2019-05-06T10:13:48.370Z Reads: 59

```
When you installed the original focbox did you have to modify the stock BMS in any way on the Gen 2?
```

---
## \#66 Posted by: AlexBE Posted at: 2019-05-06T11:16:16.839Z Reads: 59

```
No. The gen2 BMS is dumb, it just kills power if the voltage gets too low, but the FOCBOX prevents that.
```

---
## \#67 Posted by: RufioBangarang Posted at: 2019-05-06T11:58:24.628Z Reads: 60

```
Cheers Alex .. did you end up ever getting photos of what you did? So what your telling me is if I get any old ESC I can put it in the gen 2 with everything else stock with no issues? I emailed Evolve regarding this as my remote is stuffed and they basically said it'd need new EVERYTHING.
```

---
## \#68 Posted by: AlexBE Posted at: 2019-05-07T01:49:15.872Z Reads: 56

```
Well, not any old ESC, a FOCBOX. Then you will need a remote to control that, like a nano. Yes that will work.
```

---
## \#69 Posted by: RufioBangarang Posted at: 2019-05-07T02:18:07.564Z Reads: 54

```
What about something a little cheaper than the focbox like a flipsky 4.2?
```

---
## \#70 Posted by: Djarden Posted at: 2019-08-09T16:59:47.644Z Reads: 32

```
do you have pics or videos showing how do add the FOCBOX to a gen2 board? thanks
```

---
## \#71 Posted by: AlexBE Posted at: 2019-08-10T01:49:06.568Z Reads: 27

```
No sorry, but there is nothing specific. You just install it exactly the same way you would any generic FOCBOX build.
```

---

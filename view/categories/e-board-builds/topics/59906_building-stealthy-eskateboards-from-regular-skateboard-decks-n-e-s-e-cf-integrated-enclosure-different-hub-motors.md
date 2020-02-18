# Building stealthy eSkateboards from regular skateboard decks &#124; N.E.S.E &#124; CF integrated enclosure &#124; different hub motors

### Replies: 85 Views: 5043

## \#1 Posted by: visnu777 Posted at: 2018-06-24T12:12:20.882Z Reads: 733

```
Hi there,
this spring a friend of mine I haven't seen for a while told me that he is driving around over there with an electric skateboard going 45 kph with a range of 35km.:open_mouth: I immediately got hook up on the idea of driving around and getting more independent from bus schedules. I don't have a car but use public transport a lot so it had to be small enough to carry around. I wanted to use my old Element Jeremy Wray deck which I recently transformed into a cruiser board with 3d printed TPU riserpads and longboard wheels. It should be able to be used like a unmotorized skateboard in case police gets suspicious or power runs out. I did a quick search and ended up ordering a cheap 70mm hub motor kit on ebay, sold by a absolutely clueless seller :D. 

![signal-2018-04-02-173840|316x500](upload://s5J3oZ5ZBjru3DwqS8pU7Nsjt5d.jpeg)

In the picture I already installed a 3d printed PU (from TPU). I ordered a custom 10S4P Battery made of Samsung 25R cells from someone building these professionally (including BMS) and when it arrived I could not wait to try it out and taped everything together for a test run. During this test run I encountered strange behaviour: In slow mode, everything was fine, but seriously, who wants to use that apart from getting used to driving? In medium mode there was random stuttering in between but it was mostly usable but in fast mode I had stuttering, immediate full throttle and stuff like that so something was obviously wrong. During that time I started doing research over here btw, which helped me pin down the problem. It had to be the ESC so I ordered one from diyeboard which worked perfectly. I taped everything together and already had a lot of fun
when after one bigger trip with my girlfriend one motor started scrubbing at the magnets. I'll never buy cheap stuff from ebay again :D Now I was already hooked up 100% so I had to get replacement hubs. I ordered the 70mm hub kit from diyeboard but when It arrived it revealed a bit of a problem: They are longboard style trucks but everything I already planned was based on regular trucks. (The ebay hubs were Maytech style so I cut my trucks the way the hubs fit with their rectangular shaft) The new trucks made turning way too sensitive so I had to move them one hole-distance each apart.

![signal-2018-05-04-203818|316x500](upload://88iftE3ChE3t2bMHcBYzcEjFJLk.jpeg)

Now I was in love with this hobby: The new motors were so quiet and powerful, speed was a little lower (25kph compared to 28kph with the previous ones) but it felt so much better, perfect :slightly_smiling_face:
Time for the casing... At work I had the opportunity to get the deck laserscanned with high precision:

![image|654x500](upload://mj1DId1OdChQK0In9GQxyGAR2ot.png)

I designed a case perfectly aligned to match the board shape for 3d-printing:

![image2|443x500](upload://3KPsoyjLtLivXDm6lrDhpteKndd.png)

but my printer is way too small so I had to depend on others... I hate it :D the printers at work were all not operable so I had to think of alternatives. I almost bought a CR-10 5S with 50cm build space. With that one I could print it in one piece but it would have been a waste of money since I mostly print smaller parts which can be done better with the fab mini. This forum finally gave me the solution: Kydex. I read a bit and after that I ordered a 30x60cm piece. The delivery gods were angry at me so I waited 3 weeks for it after which the seller did some research after which it was back on track. In the meantime I ordered another one to get the case started but with this there was some delay too :anger: Like there was a grudge on my whole project :D
While waiting I worked on the lights:

![signal-2018-05-11-192252|316x500](upload://kubeprIkaqoo1ZwZ3kd17Q0Aj9q.jpeg)
![signal-2018-05-11-192320|316x500](upload://46SdYLltyepcsvEzBcRp61RA7b8.jpeg)
![signal-2018-05-15-211613|316x500](upload://4Kjr7neBOcoo3i93uCrZFUkbAxu.jpeg)

They are driven by the main battery, I found a LED driver with up to 56V input and 350mA output.
They're still a work in progress (right now I don't have them assembled to the deck at all, I have to redo them first)

After working on the lights I started modelling a bed for the batteries since the board has strong concave that needs to be corrected so the batteries won't stretch. I printed it in 8 pieces on my fab mini with TPU and puzzled them back together.

![image_batterybed|690x281](upload://eRrXxyyNQ0arOyluNf7bt9IeGGU.png)

When the kydex arrived I already had a wooden body prepared for it:

![signal-2018-05-11-112644|316x500](upload://8Nj4Xyl9vL4yYUIBEH4XtdBmgyd.jpeg)

![signal-2018-05-18-140105|666x500](upload://ahScrA9ChcfdvgYS82pqfMYxykO.jpeg)

So i could start immediately when the delivery guy came by :D I placed a thermotransfer pad between ESC and the aluminium heatsink plus I added a real heatsink on top of it. The plan was to cut a hole in the case for the real heatsink and make the surrounding area waterproof.

![signal-2018-05-16-202017|316x500](upload://ocYUSNB7RpmtcskdtgVlnp5jbJm.jpeg)

![signal-2018-05-19-210416|316x500](upload://aXhCpBpoQ04AQtIbNSy3zTrfa8C.jpeg)

This V1 build worked like a charm until the board broke. It looked like swiss cheese all over so when I accidentally hit a really evil edge it cracked :( RIP my old friend :D
After that I instantly ordered a new deck (Sale, glas fiber coated) and tried to transfer everything to it but I wasn't aware of the non standardized truck distance. I was in a hurry and did a really dirty job to get it running at all costs so after that one I ordered a new deck to do it once again right :slight_smile:

![SAM_2216|690x227](upload://2z8xTdgDIko2HLs99qoApcNLSv0.JPG)
![SAM_2219|690x211](upload://7Z7AvMtRVECxxFH6PhrzBEz3t18.JPG)
![SAM_2211|690x490](upload://mhjiTH0RAimytjxlU0WulGZ7LVg.JPG)
![SAM_2212|690x403](upload://yUdYBMx9uAe53dMv0LstHONFHN.JPG)
![SAM_2213|690x257](upload://y6hVubS6mG5Oo5XfUkHUBTlcN1d.JPG)

The green deck is for my upcoming project, its still a regular deck but slightly larger (33.5x8.5 inch). I'll countersink(?) a battery and electronics bed and cover the whole thing with carbon. The shape will also be changed slightly depending on the new 90mm hub motor trucks (this time with replaceable pus).

Thanks for watching,
Michael
```

---
## \#2 Posted by: DAddYE Posted at: 2018-06-24T13:23:50.535Z Reads: 572

```
How tick is your kydex? Did you use a heat gun?
```

---
## \#3 Posted by: chrisongtj Posted at: 2018-06-24T13:50:59.896Z Reads: 566

```
Looks like a really decent job on the Kydex. Im also curious to know how thick it is?
```

---
## \#4 Posted by: visnu777 Posted at: 2018-06-25T07:46:11.855Z Reads: 542

```
Thanks :) It is 2mm Kydex, I put it in the oven at 150°C for some minutes until it was elastic and then I tried to put it on the wooden model for the case, after which I immediately put some foam on top and started pressing everything down. This resulted in a raw form that was perfected afterwards with a heat gun (Heatgun, foam, press and repeat*n). You might have noticed the texture difference between the two parts, the battery part went much smother since I let it in the oven for a shorter time than the electronics case which had obviously too much.
```

---
## \#5 Posted by: lowGuido Posted at: 2018-06-25T08:06:25.711Z Reads: 511

```
I threw this together one friday night cause I wanted to skate on the weekend.
![20180413_200446|281x500](upload://g5G5DkPQf97nfLgvOZrzRJk3Eme.jpg)
```

---
## \#6 Posted by: Alex.Scheff Posted at: 2018-06-25T08:15:42.702Z Reads: 456

```
What type of esc is this?
```

---
## \#7 Posted by: visnu777 Posted at: 2018-06-28T12:32:13.597Z Reads: 442

```
Not bad for quick and dirty, nice :) 
I got my new 90mm hub drive with replaceable pu and took it for a testride :) looked a bit ridiculous (eDragster :smiley:) The additional power and diameter work out as expected, they have better speed and torque at the cost of size and weight. Lets hope I'll still be able to carry it around like the previous one, otherwise I'll get the new 75mm hub motor from diye and build another version with the smaller deck (also with carbon fiber this time)
@Alex.Scheff I'm pretty sure you asked Guido but just in case you meant me: Its a diyeboard esc V1.1 with an additional heatsink to have it stand out of the case for cooling but sealed off properly.
```

---
## \#8 Posted by: Vanarian Posted at: 2018-06-28T13:48:29.729Z Reads: 426

```
This is something we should see more often, nice job ! Which width are your truck, standard 180mm ? Did you put risers to counter wheelbite with the RKP trucks ?
```

---
## \#9 Posted by: visnu777 Posted at: 2018-06-28T15:04:27.993Z Reads: 413

```
Again, not sure if you adress me but nonetheless: The trucks on the pictures are 6 inch, since I moved them outwards I had to print a PETG riser leveling out the contour (using the laser scanned model) plus a TPU shockpad for vibrations (and some height) :)
```

---
## \#10 Posted by: visnu777 Posted at: 2018-07-14T19:27:23.688Z Reads: 424

```
A little update on my chaotic planning and constructing:

I have to start with the plan changer: My DIYeboard ESC is half dead. I drove quite steep roads and at some point torque was gone. I stopped and checked everything and saw that one motor didnt work any more. I tried to fix it / find the problem but no chance, I carried it home. Maybe I've stressed it too much but It should have survived it. One motor channel is dead. I almost ordered another one when I said to myself: No, you will buy two VESCs now, at least you can do lots more with them (interfaces etc. I plan to build brake lights first). I ordered two Flipsky FS ESCs.

I recently bought 30 VTC 6 cells, 10 N.E.S.E. packs for 3P and build another battery. 

![newBattery|690x279](upload://4rrAYe00WBAQNfN1h3eRJOBdYv0.jpeg)

I sold my 3 month old 10s4p pack to a friend. The new pack will have no BMS (at least for now, I ordered one in China but I'm not sure if I will use one this time. The VTC6 should be stable according my research on the web. With this cells I'll have almost the same capacity as with my old 10s4p with Samsung 25R but save some weight. I enjoyed the 90mm hub drive a lot so far so I want to use only it exclusively and build the one eboard for me. As I told you before I'll use a 33.5x8.5 inch regular skate deck (Minilogo). I'll move the trucks further apart so the wheels will have enough space. I already tested this without electronics and it feels really good, like on railroad tracks :) . Yesterday I cut too much from the deck on the previous pictures and had to order another one. They're quite cheap but its a waste  :( Next time I'll be more careful. 

![construction_site|375x500](upload://a2EqkbGeHDh8Jg4R7IDHrflGMqH.jpeg)

Btw, I got 195mm Paris trucks for the front :)
```

---
## \#11 Posted by: visnu777 Posted at: 2018-07-18T19:03:49.314Z Reads: 400

```
Under construction:
![SAM_2224|690x460](upload://tN3hSDNRlDOALdA3zyXhCzWwEnF.JPG)
![SAM_2225|690x460](upload://4blMM1MMvQn6koeq2DvCyA39I91.JPG)
![SAM_2227|690x460](upload://w9xsJjj9ikQbzAgUhtsdc1gwRdq.JPG)
![SAM_2226|690x460](upload://qcUWvolOFB3InFRbj4CXJhjMTzS.JPG)
![SAM_2222|690x460](upload://qqPZ3MqayZdGL8juugugpsdxmKh.JPG)
![SAM_2223|690x460](upload://tX5V4BNzOdqHGmdgZb9OlyI5HEP.JPG)

Still a long way to go but you can see where its going :smiley: 
Its getting quite crowded in the electronics cabinet, I'll have to be creative :slightly_smiling_face:
I have 2 Flipsky FSESCs  (VESC 4.12), a Receiver for the remote, a Bluetooth module, an ESP32 MCU, a gyroscope, a led driver and a step down converter for 4x USB power.
```

---
## \#12 Posted by: sunnyD Posted at: 2018-07-18T19:05:09.322Z Reads: 366

```
Teamgee better be taking some notes!
```

---
## \#13 Posted by: visnu777 Posted at: 2018-07-19T20:11:48.901Z Reads: 383

```
Some more dremeling, filled up the gaps, sanded it down, cleaned with acetone.

![SAM_2229|690x460](upload://l2pytoyghEWZAfxx8juO0nrwjaT.JPG)![SAM_2228|690x460](upload://9KyTZMm5xL0FxavjacqJsnFruAl.JPG)

the lower part will be covered with carbon fiber two times, first I'll start at the top and fold it to the bottom and then I do the second layer only covering the bottom. I have no experience with CF so far but watched a lot of tutorials and I'm feeling pretty confident that it will work out, both the laminating process and the final board stiffness. If it doesn't I'll try something like the guys with the Spud CF decks, using the router to create a flat area for the batteries and electronics and then put a case on top of it. But I want this one to work out, making everything accessible from the top is way cooler than the usual bottom mounting of cases :) Since I'll make two lids I'll lock the battery with screws and the smaller electronics compartment gets a quicker locking mechanism so I can easily access the stuff inside. Since I don't want anything to be visible on the outside I'll hide it there ;)
```

---
## \#14 Posted by: visnu777 Posted at: 2018-07-22T19:47:10.618Z Reads: 372

```
so far so good :D Its far from perfect but somehow I made it. The first carbon fiber layer is attached to the top side of the deck and in a vacuum bag. (I hope It will not stick to the bag too much tomorrow.) I will add one more cf layer on this side but only covering the flat outer areas (mostly for decoration). ![SAM_2230|690x460](upload://oi70xbTFOLX88Z8rXEevW1UiX0s.JPG) The lower side will have one layer covering all and then at least two layers in the middle around 10cm wide for further stability.
```

---
## \#15 Posted by: visnu777 Posted at: 2018-07-24T14:10:12.866Z Reads: 373

```
My mess: :blush:

![SAM_2231|690x460](upload://89TDsT5NN7HonkG7NdGpYB4mdz1.JPG)

I can't wait to tidy up again, the project totally blocked my VR-area :D
```

---
## \#16 Posted by: visnu777 Posted at: 2018-07-26T06:32:48.951Z Reads: 371

```
![SAM_2232|333x500](upload://oiltJqDQtFe2dU3OGK1eUJbuZO5.JPG)

Time for a test drive when I come back from work. I have to sand it down once more and do a final epoxy coating after that test to seal the truck holes. I'm not sure about the clear coat yet, I have it here but it takes forever to dry and the epoxy is quite shiny all by itself. Is there any benefit out of it besides UV protection?
```

---
## \#17 Posted by: pat.speed Posted at: 2018-07-26T06:45:49.168Z Reads: 352

```
Looks great, I’m thinking of a similar shortboard build. The clear coat will help with protection from scratches and rocks, and it’ll make it even more glossy
```

---
## \#18 Posted by: visnu777 Posted at: 2018-07-26T06:48:20.055Z Reads: 351

```
Thanks :) I'll do it when its rainy outside :D
```

---
## \#19 Posted by: visnu777 Posted at: 2018-07-26T19:38:48.826Z Reads: 336

```
I just did a test run as planned and WOW, HOLY SHIT! I have to make the VESCs much smoother, right now its a beast :D My CF-Wood construction seems to hold up perfectly as far as i can tell right now (hurray :D)
```

---
## \#20 Posted by: visnu777 Posted at: 2018-07-27T21:08:10.990Z Reads: 332

```
My frist "real" testrun was successful and I was happy but when I returned home I wanted to check the remaining capacity. When I plugged in the antispark the electronics compartment started to smoke. After disconnecting the antispark I saw that the USB-Port had contact with the carbon case and melted. When I checked both vescs seperately both were unable to connect to the vesc tool :( so I must have destroyed them. The cause was a worn down shrink tube at the connection between the two 5s3p halfs, it made contact with the hull resulting in 17V on the USB...
```

---
## \#21 Posted by: Sn4pz Posted at: 2018-07-27T21:25:21.812Z Reads: 312

```
do you have another battery to at least test your stuff out on??

that sucks super hard dude :(
```

---
## \#22 Posted by: visnu777 Posted at: 2018-07-27T21:31:18.110Z Reads: 329

```
Yeah it sucks :( The battery is still in good condition but both VESCs are fried i'm afraid. Tried to connect to both of them via vesc tool but nothing happens. There are no lights on the VESCs too.
It could have been worse, I just returned home from work by train ;)
```

---
## \#23 Posted by: visnu777 Posted at: 2018-07-27T21:34:10.480Z Reads: 340

```
Here are some pictures of the almost finished board. Since the ESCs fried I have plenty of time to really finish it.![bottom|316x500](upload://5bpa5Z9zPOIFHfQNhL3zGMlPe3m.jpeg)![top|316x500](upload://8tJUJm3PnLuH7zefC8j2gAdmQgK.jpeg)![side|316x500](upload://xrBZ7uHJ3LJl85YMFsNSobue1CY.jpeg)
```

---
## \#24 Posted by: visnu777 Posted at: 2018-08-02T19:19:21.951Z Reads: 316

```
Almost ready for the last epoxy layer:

![SAM_2234|690x460](upload://rss0W3fSH32aCTKMIEzYJVATVET.JPG)

I removed all carbon on the inside so something like that can never happen again :) Call me paranoid but I feel better now :smiley:

... and yes, it was a very long and loud procedure (used up a lot of sanding deltas) but it had to be.
```

---
## \#25 Posted by: visnu777 Posted at: 2018-08-04T12:06:07.770Z Reads: 308

```
Making progress: 

![1|690x459](upload://nqeNqyT2MrI1bCwmpd3wIRcOvvQ.JPG)

the clear coat ruined the shiny epoxy look, but for now its ok. If I'm in the mood for sanding again I'll make it nicer. As you can see I tried transparent grip so you could see the carbon structure but its not working. For now I leave it as it is but in the future I#ll remove it and replace it with regular black grip (and maybe some red accents) Today my new Flipsky VESCs arrived (way faster than I expected) so I drive a bit around later/tomorrow (*hooray*).

These belong to my future (winter) project:
![2|690x459](upload://kJDeF6OHQFbv4lR6JqbO3LpfV6z.JPG)
I want to build a BLE/BT remote with display, analogue stick and (for now) two buttons with this nice ESP32 board, lets see how that works out :slight_smile: As you can see the board already has a 18650 holder on the back, a power switch, charging circuits (USB) and an oled display for useful information.
Wanted features: Throttle and brake, holding left / right triggers the direction lights, one button triggers an acoustic signal for others

Greetings from ultrahot Germany,
Michael
```

---
## \#26 Posted by: pat.speed Posted at: 2018-08-04T13:16:54.009Z Reads: 296

```
Wow, I’m surprised the clear coat made it less shiny, whenever I’ve used it it’s made it more glossy. Sorry for the bad advice that was just my experience, the boards coming along nicely though
```

---
## \#27 Posted by: visnu777 Posted at: 2018-08-04T14:09:05.697Z Reads: 291

```
Don't worry, maybe I did it wrong :D it doesnt matter that much, I did the Carbon Fiber stuff for stability not for decoration :D
```

---
## \#28 Posted by: visnu777 Posted at: 2018-08-07T06:59:33.498Z Reads: 296

```
Travelling:

![IMG_20180807_085358|375x500](upload://4p06OFdsXyZbbA0zuy33axScsC8.jpg)
```

---
## \#29 Posted by: visnu777 Posted at: 2018-08-10T17:46:43.692Z Reads: 289

```
Metr recording (values make more or less no sense, it was 4 km max)

https://metr.at/r/jQrTx
```

---
## \#30 Posted by: visnu777 Posted at: 2018-08-10T19:17:16.519Z Reads: 274

```
hmmm, I just disassembled my battery pack to measure every single cell but everything is in perfect balance. All cells were equal, only 3 cells of one 3p pack were 0.01V off. The Metr App constantly showed low voltage warnings so I wanted to find out if one of them was faulty resulting in voltage sag but everything is fine...
```

---
## \#31 Posted by: visnu777 Posted at: 2018-08-30T17:32:20.587Z Reads: 278

```
Update on the battery: After more irregularities with the Balance I decided to get a single cell charger with internal resistance measurement capabilities. I got the XTAR Dragon and used it to charge each cell seperately and checked the ir. I found suspicious cells and replaced them with new ones and now my pack is perfectly balanced and has no more heavy voltage sag :) I can climb steep roads and everything so i'm happy. 
Here are some pics of the final thing, i call it Red Star :smiley: 
![redstar2|690x319](upload://1Iax9gWnSVUIMb5zzO4AWuv8aPc.JPG)![redstar1|333x500](upload://1z4ryiQiiexNWTAW4YTAT91ZdTc.JPG)![redstar3|333x500](upload://zjSm1GoBXacd8jdJTWVpqaw7IHM.JPG)

Thanks to @rey8801 I will soon have brand new mad hubs with 74KV replacing these. I thought about getting the 130KV version but came to the conclusion that for me 36-38km/h are fast enough and I prefer torque over speed. I mostly went for the mad hubs because of the looks. I don't like the look of the DIYeboard hubs, they're too bulky for my likings, especially compared to my 195mm Paris V2 front truck. Now I'll get another 150mm V2 for the hubs and everything will hopefully look more balanced and more stealth since the hubs look more like regular wheels. I'm curious :smiley:
```

---
## \#32 Posted by: rey8801 Posted at: 2018-08-30T17:34:55.184Z Reads: 260

```
Didn't see it before. Nice I like the look!
```

---
## \#33 Posted by: rey8801 Posted at: 2018-08-31T13:48:07.045Z Reads: 260

```
I went through the all build log...a lot of work man. Respect! You should start to scan all the decks you can find :laughing:. For instance in my case I would love to have the Jet Spud scanned. You can buy and send back afterwords all the decks most used in ESk8 ahhahhaahahha
```

---
## \#34 Posted by: visnu777 Posted at: 2018-08-31T14:14:39.602Z Reads: 255

```
:) Thanks :) I would if it was my scanner :D
```

---
## \#35 Posted by: rey8801 Posted at: 2018-09-12T12:22:17.895Z Reads: 254

```
hey man I am rebuilding my battery pack and I want to test capacity and internal resistance of single cells. I can decide between these charger https://eu.nkon.nl/charger/charger-suitable-for-battery-type/lithium.html. Maybe you know which one to pick it up. In case you have a link for a good price of one that you know that works please share it...Thx :wink:
```

---
## \#36 Posted by: visnu777 Posted at: 2018-09-12T15:29:55.301Z Reads: 253

```
https://eu.nkon.nl/charger/xtar-vp4-plus-dragon-charger.html this one :) it has electrodes Like a Voltmeter and works AS such plus showin IR
```

---
## \#37 Posted by: visnu777 Posted at: 2018-09-12T16:13:29.920Z Reads: 260

```
Btw: Travelling again :wink: :sunny:

![IMG_20180912_181118|375x500](upload://tdPtYiS8coXmkU3r3okFCS7wxvy.jpg)
```

---
## \#38 Posted by: JamesNothing Posted at: 2018-09-12T18:29:43.239Z Reads: 259

```
need a scan of the spud? I happen to own both a spud29 and a fancy Artec 3d scanner I use at my 3d printing business, I could try to scan it :slight_smile: 


@visnu777 nice work, man!  that's a nice commuter you have there!
```

---
## \#39 Posted by: rey8801 Posted at: 2018-09-12T18:31:47.216Z Reads: 250

```
Please yes! I know other people that would love it to have it. I will share it with them too
```

---
## \#40 Posted by: rey8801 Posted at: 2018-09-12T22:30:26.171Z Reads: 241

```
Perfect it was the one in my cart already! Thx for the advice

It is out of stocks, damn :sweat_smile: Where did you get yours?
```

---
## \#41 Posted by: nuttyjeff Posted at: 2018-09-12T23:27:53.962Z Reads: 232

```
Oh wow id love to have this file.
```

---
## \#42 Posted by: JamesNothing Posted at: 2018-09-13T12:52:59.536Z Reads: 229

```
working on it, me or @rey8801 will let you know
```

---
## \#43 Posted by: visnu777 Posted at: 2018-09-14T12:40:38.897Z Reads: 228

```
On eBay ;) I found some German shops that have it in stock though.
```

---
## \#44 Posted by: rey8801 Posted at: 2018-09-14T12:42:22.401Z Reads: 225

```
Thx! at the end I found a good deal from Hobbyking. Is not the same model but the reviews online were all positive so I went for it :wink:
```

---
## \#45 Posted by: Okami Posted at: 2018-09-15T07:49:00.570Z Reads: 231

```
How much did u travel with that backpack and eboars together?

 Been thinking about doing hitchhiking with eboard just not sure for how long with heavy backpack it is possible to travel.

A seperate trailer for bag would help but would make riding and carrying a lot more bulkky, so not sure if this is an option..

Maybe a bag with wheels included would work?
```

---
## \#46 Posted by: visnu777 Posted at: 2018-09-15T11:02:11.208Z Reads: 223

```
Most of it was by train i'm not sure if I actually want to hike with all the stuff. My eboard is more than 9 Kilos. I'll try skatehiking though where I just have the empty backpack frame and my board and I just carry when the road is impossible to ride. Today I went for a 2x6km ride to buy 17,5 kg cat litter but it wasn't a very pleasant thing, you feel the road much stronger than usual which made my back foot ankle hurt a bit. It was no problem for my carbon fiber construction so I can now say that it will hold under any condition :D
The bag with wheels should have good bearings which they usually don't have.
```

---
## \#47 Posted by: Okami Posted at: 2018-09-15T18:47:58.784Z Reads: 216

```
Yeh ive ridden with heavier backpack also.. drastically pulls u down to ground more.

On a side note, if there is a frame for the bag, i guess it should be possible to fabricate wheel mounts for it and attach normal wheels for it. Next step wouls be to make it stable and turny enough..

Will keep this idea in mind. I guess thanks for helping figure it out one step further mentally :)
```

---
## \#48 Posted by: visnu777 Posted at: 2018-09-15T21:49:22.670Z Reads: 219

```
You're welcome :D
```

---
## \#49 Posted by: visnu777 Posted at: 2018-09-17T17:44:48.666Z Reads: 223

```
I have a new plan for my board: Since I will soon have one set of 75 KV "Mad" hub motors I ordered MBS AT wheels for the front. I'll scan them and create a sleeve for the hubs matching the front wheels. I will 3d print the model, use it as a protoype for a mold which I use to create a PU version of it. Additionally to this I'll create a 12s1p (2x6s) Lipo Box which can be mounted instead of the cover for the electronics, similar to the MTB boxes sitting on top of the board (but way smaller), extending range and give more power for (light) offroad experiences.
stay tuned :smiley:
```

---
## \#50 Posted by: sk8l8r Posted at: 2018-09-18T08:29:13.873Z Reads: 211

```
[quote="visnu777, post:49, topic:59906"]
I’ll scan them and create a sleeve for the hubs matching the front wheels
[/quote]

I've wanted someone to try this for a while now, very cool!
```

---
## \#51 Posted by: visnu777 Posted at: 2018-09-19T09:09:59.405Z Reads: 199

```
I've never done this or similar stuff but i'm pretty optimistic (thanks to youtube :D) They won't be perfect but will hopefully do for light offroad :) Hummie wrote a lot about different PU types he tried for his hubs but I just hope it works...
```

---
## \#52 Posted by: rey8801 Posted at: 2018-09-19T09:41:59.917Z Reads: 199

```
Super cool idea...if you don't mind I would like to have the scanned file of the wheels. Do you think you can also get a precise core dimension ecc...
```

---
## \#53 Posted by: visnu777 Posted at: 2018-09-19T09:46:07.012Z Reads: 196

```
Of course, I actually think I can upload it for the public since it is only a scan. I'll try to get the core scanned as well :)
```

---
## \#54 Posted by: rey8801 Posted at: 2018-09-19T12:35:00.862Z Reads: 194

```
Perfect! That would be super usefull for a project I am making.
```

---
## \#55 Posted by: Vanarian Posted at: 2018-09-24T22:38:35.332Z Reads: 193

```
Ha funny this is your thread! Now I know where the drive comes from :+1: 

Which width is your current trucks with the Diyeboard hubs? BTW From what Rey posted, you'd end up with 195mm total width when you mount MADs on 150mm Paris.
```

---
## \#56 Posted by: visnu777 Posted at: 2018-09-25T16:51:42.183Z Reads: 206

```
hehe, I actually have two different sized front trucks for this just in case :D I'm happy that i've found someone to whom it might be useful :) I gave up hoarding stuff a long time ago, since then I try to give things away so others may use them :)
```

---
## \#57 Posted by: visnu777 Posted at: 2018-11-09T18:32:09.480Z Reads: 208

```
My current setup: 

![SAM_2354|690x460](upload://sUyGqLJUXAgtTRjyQ5A4PmOee4j.jpeg) ![SAM_2357|690x460](upload://dhjuDPuuTC3FCxJGDPSuVo5CvAU.jpeg) ![SAM_2358|690x460](upload://wxNMh6kUCwuI5JHTmkF3pntQZoo.jpeg) 

I managed to install the lights, after the daylight saving toggle I have to drive when its dark and without light its dangerous :) My drive is upgraded to a dual Landwheel hub motor setup running at 50A/-60A motor and 45A/-10A battery for which I recently casted MBS AT style wheels on top of the sleeves (see diy casting thread) to fit the front truck with the real MBS AT wheels :)
```

---
## \#58 Posted by: City-Blade-101 Posted at: 2018-11-11T22:09:25.917Z Reads: 195

```
Guten Abend,
that build and the idea to work it out like this is a good option.
 I could imagine future skaters will flip something like this on a handrail, to smith, 360 flip off hahahahaha....
The only bad thing is the angle of the trucks!
I bet this board curves not very well, so you have to install wedges underneath, to bring the trucks in line. Maybe next time you can install the wedges underneath the carbon fibre, that would be awesome...cant wait for the next build!
peace
```

---
## \#59 Posted by: visnu777 Posted at: 2018-11-12T21:43:13.173Z Reads: 186

```
It works surprisingly well :). A friend of mine who owns a skateshop for a long time and has a lot of knowledge with longboarding can't understand why it works :D I can carve and still its stable at high speeds (my top speed was 62 km/h with a 2s Boosterpack (12s) and it still felt safe.) But nobody will bring this on a handrail, its 10 kilos :D and I would probably kill that person ;)
```

---
## \#60 Posted by: City-Blade-101 Posted at: 2018-11-12T22:37:41.898Z Reads: 183

```
hahahaha...that handrail-talk was mostly meant as a joke so i was just kidding:joy:...I could imagine that setup with a much smaller battery pack, so it could be possible to flip it hahahahaha...
...that sounds unusual to me, that the trucks are easy to handle with this angle, but hey, if it works for you its all more than good:wink:
...the fact that its stable at high speeds sounds real, because if you cannot carve or turn ( my opinion) there is no more place for something like speed wobbles hahahahahaha
```

---
## \#61 Posted by: visnu777 Posted at: 2018-11-12T22:50:23.713Z Reads: 167

```
I'll post a video soon where you can see how carvy it is. For me its perfect, it allows for really fast changing the lanes :)
```

---
## \#62 Posted by: City-Blade-101 Posted at: 2018-11-12T22:53:35.647Z Reads: 171

```
Yeah cool...like i said: if it works for you then itz all good :slightly_smiling_face:
i will watch your vid when itz online, because i have to see this thing turning hahaha...a good and interesting build anyways
```

---
## \#63 Posted by: visnu777 Posted at: 2018-11-28T11:44:38.551Z Reads: 167

```
I'm currently doing a overhaul of the board, this time with lots more patience so it will be more perfect than ever :) I'll reinforce the structure, make one big lid instead of the two (since it turned out I had to open both of them all the time :D), improve water proofing, include two Focboxes (not that the FSESCs didnt work, its just for the form factor and the fact that they were almost cheap and I had some money to spend) and integrate the Photon remote (when it will arrive) since I damaged my FS Winning remote due to a small accident (the USB Port got loose, now I have to use my Hobby charger to charge it).
Maybe I'll never really finish it and always keep improving :D
```

---
## \#64 Posted by: City-Blade-101 Posted at: 2018-11-28T22:07:59.687Z Reads: 165

```
Yeah! Sounds good. Seems like your first build was kind of a big learning field for you, so now you're able to avoid some mistakes and reinvent and precice your own style.I think with hub motors its not that difficult to build a board you can ride in the rain :wink:
Im still assembling parts for my very first build. I got two brand-new Onan x2 Hubs,a deck(never summer-superfreak(au mann das ist so geil), trucks(etliche), but was struggling with motor controllers. After months of reading and hopefully learning I will use this one: http://www.hellray.de/esk8-controller/
I will not run in foc, because I have a 4 wheel drive which is in foc, what is great, but i miss the motor sound hahahaha it feels strange and weird in foc hahahaha my beloved small everyday board runs (glaube ich)  bldc and that feels fine hahahah
And Yeah, the Photon Remote is a good choice in my opinion, even i can not tell about it if it works fine or not. But anyways, nice Remote, build with lots of brain, it will work! :grinning:
```

---
## \#65 Posted by: evoheyax Posted at: 2018-11-29T05:14:44.221Z Reads: 157

```
The flipsky escs have known issues so I would be careful with them. I would not consider them reliable. The 4.12 vesc in general had some design issues. It’s usually ok if you run it in bldc at 10s, but it has issues in foc and 12s, unless it’s an upgraded one like chakas 4.12.
```

---
## \#66 Posted by: visnu777 Posted at: 2018-12-08T14:35:26.569Z Reads: 158

```
Some pics of my new head/tail lights:

![ruecklicht|690x460](upload://7hzrz5OKytzG6HVQuXIhM5hHuFi.jpeg) ![r%C3%BCcklicht2|690x460](upload://uR16pv4ZdznhSAJ1A9CkloPw7wX.jpeg) 
![SAM_2386|688x500](upload://ajBReMEF4zhPXMkW1sm1CjSfZ5k.jpeg) ![SAM_2382|507x499](upload://3lYBNzKGFvfazmCfdLdDdChqaXH.jpeg) 
![SAM_2388|690x430](upload://9E7oHgJSkAlR8Z2pkrxszSOBVVt.jpeg) 

I aim for the best stealth/useable factor possible. Tail light is already done and covered in several layers of epoxy. My head light is a Cree MKR (max 1000 lumens@1280mA) which will be driven by a 1000mA pwmable current supply feeding on the main battery. It is so small that I will also thermoglue it to the front baseplate :)
```

---
## \#67 Posted by: visnu777 Posted at: 2018-12-09T19:57:48.810Z Reads: 143

```
ahhh, finally the last epoxy coating is curing, tomorrow I'll finish the deck once again :D Its a pity that the Focboxes seem to be hold in customs though, I'll have to use the FSESCs till I get them... With the Focboxes I will have enough space for 2 led current supplies, the Metr Pro, remote transceiver and battery display :)
```

---
## \#68 Posted by: visnu777 Posted at: 2018-12-10T14:12:14.668Z Reads: 145

```
Some more pics :)
Sanded:
![SAM_2391|690x460](upload://wBFaaAATaQkt9pfmrNRjXy5yYQn.jpeg) 
Epoxy coating:
![SAM_2393|333x500](upload://sfNr8KL67gcHUgVRlpSmUlvAlX9.jpeg) 

Stress testing :D
![SAM_2394|333x500](upload://y5cghJ799wX8UIvVmZ72jFbP36b.jpeg) ![SAM_2395|333x500](upload://zFGVbwnatfdr7Ba3NKJ2OeWSPab.jpeg)
![SAM_2396|690x460](upload://q9YynibRicR7thhU7S3LLdIntBs.jpeg) 
![SAM_2397|690x460](upload://pRMSlk2LTw3GposkDWiGr9vrlhp.jpeg)

This first test was not bad but some water leaked inside. Now its drying and waiting for a second run (after some modifiactions of course :D
```

---
## \#69 Posted by: visnu777 Posted at: 2018-12-14T19:44:05.593Z Reads: 138

```
![IMG_20181214_174859_BURST001_COVER|375x500](upload://eZT7kv92inljVUOr6vr3yYPKtZa.jpeg)
![IMG_20181214_180129|375x500](upload://wQ34qjQoOqWw8YDE5NxnLQMNEZR.jpeg) 
![IMG_20181214_204122|666x500](upload://ows5k2JTcqMN7OTha0o0qnpLUz4.jpeg)
```

---
## \#70 Posted by: visnu777 Posted at: 2018-12-25T12:58:51.438Z Reads: 121

```
![SAM_2405-01|333x500](upload://1q3NI2kPLqtu4sw0fQabFwQbZkH.jpeg) ![SAM_2408-01|333x500](upload://otIIU60FoHCIdXrIsbsfzG2Pfcw.jpeg) ![SAM_2406-01|333x500](upload://zfGcbFtA3q1QqDW1vNM5hZmtku4.jpeg)
Sadly I shredded the motors approximately 1 hour after the picture was taken :frowning: but I'll rewind them :)
```

---
## \#71 Posted by: Friskies Posted at: 2018-12-25T13:38:34.536Z Reads: 117

```
If you are riding at night I would get a bike light and mount kt to your helmet for the front. The rear is awesome as you only need to others to see you are slowing down etc. At the front at that height, all it does is light up cracks that are too close to the board to do anything about. 
I hope this helps a bit and saves you a fall or two :slight_smile:
```

---
## \#72 Posted by: visnu777 Posted at: 2018-12-25T13:43:01.670Z Reads: 115

```
Since yesterdays news of a legalization of plev in Germany stealth is not my highest priority any more so the headlights can be more visible :)
```

---
## \#73 Posted by: Friskies Posted at: 2018-12-25T13:44:45.161Z Reads: 113

```
I hope that Australia will follow soon. We exist in the grey here :stuck_out_tongue:
```

---
## \#74 Posted by: visnu777 Posted at: 2018-12-25T13:46:32.386Z Reads: 115

```
Atm it totally depends on the individual cop, they could fine you lots of money if they really want to.
```

---
## \#75 Posted by: visnu777 Posted at: 2019-03-27T18:06:17.868Z Reads: 88

```
@City-Blade-101 I still owed you a video of the cruising capabilities, here it is:

https://youtu.be/yiiGX7bFi8Q

 I'm not used to take movies with my phone. sorry for the quality but maybe its good enough to see how it works. I can change lanes really quick and carve :)
I'm driving around 40km/h ;)
```

---
## \#76 Posted by: City-Blade-101 Posted at: 2019-03-27T21:17:02.409Z Reads: 77

```
Oh, hahaha yes that is a nice one, and thanx for sharing. I think we must have different riding styles because i cannot see sharp turrns like I like to do, but everything is perfect if you like it and feel good on your board. Today I got something on my mind, a vision, and my first thought was to share this idea with you and Alessio. I know you re doing diy wheels for hubs and i got another idea that could work very good(maybe better) to finally get some really solid urethanes...
```

---
## \#77 Posted by: City-Blade-101 Posted at: 2019-03-27T21:19:18.168Z Reads: 71

```
the idea is to use a good branded Wheel like Abec11 for ex. and cut out the core with cnc to fit on a hub motor
```

---
## \#78 Posted by: rey8801 Posted at: 2019-03-27T22:11:03.476Z Reads: 66

```
Maybe try with a clone wheels first. Is difficult thst you will get a perfect core vmwithout vibrarion like that. Plus a CNC that cuts for 65mm wheels width is not that easy to find it.
```

---
## \#79 Posted by: City-Blade-101 Posted at: 2019-03-27T22:16:14.410Z Reads: 63

```
yeah, surely trying on cheap wheels first, may a lathe is the right choice of tool for something like this
```

---
## \#80 Posted by: rey8801 Posted at: 2019-03-27T22:30:48.464Z Reads: 60

```
No a lathe doesn't mill eccentric. It can but you need a really big lathe with 4 Jaws chuck. Maybe a powerfull laser is better.
```

---
## \#81 Posted by: City-Blade-101 Posted at: 2019-03-27T22:33:05.747Z Reads: 63

```
are you serious about the laser? I think a lathe you descriped is easier to find hahahaha
```

---
## \#82 Posted by: rey8801 Posted at: 2019-03-28T01:50:19.692Z Reads: 59

```
Not really because you will need to find a tool to cut tm in that way. I  work on lathe, also a big one one and what you ask is rather not possible. Moreover because the PU is soft and won't keep the shape once clamp it in the lathe.
The laser whatever metal cutting company have it. Will they be willing to help you... Probably no, but same will be for the lathe. Your best best, friend or publish workshop
Anyhow this is not the place to discuss of that. Make a thread if you want more advices from people :wink:
```

---
## \#83 Posted by: City-Blade-101 Posted at: 2019-03-28T12:14:12.017Z Reads: 52

```
Thank you Alessio, but I do not want to try out for myself, I just had this idea i wanted to share specially with you(knowing you re working on a lathe) and visnu777(knowing he is working on urethanes for hubs).
My thought was, when there are people in here who could do it, you or visnu777 where there right guys. Don't get me wrong, but i am not that kind of maker like you guys are and that is the reason for sharing stupid thoughts like this :joy::joy::joy:
I will not start a threat because your attention and explanation is more than enough for me to realize i was wrong again, but I will not stop thinking about innovation and you can be sure I will waste your time again if there are some stupid new thoughts on my mind. 
Peace my friend
```

---
## \#84 Posted by: rey8801 Posted at: 2019-03-28T12:17:16.849Z Reads: 51

```
Never stop thining of new things. Everything is possible, you only have to decide if it is worth it. To me for custom PU sleeves for hub motors, what Micheal did is a great solution.
```

---
## \#85 Posted by: City-Blade-101 Posted at: 2019-03-28T12:19:29.715Z Reads: 50

```
yes...maybe Michael has still the best solution.
```

---

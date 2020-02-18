# WTS: PCB based Firefly Remotes

### Replies: 73 Views: 3458

## \#1 Posted by: Zyb Posted at: 2018-08-28T14:54:03.472Z Reads: 513

```
![IMG_0084|666x500](upload://nuAND2JwuKNLBffn4RoCiFueIxz.jpeg) 

**Order form : https://goo.gl/forms/1e5Z04BQb3fVFsgP2**

Hey guys I would like to offer my version of firefly to you. Thanks to solidgeek for giving me permission to sell these remotes and for each remote sold donation goes to his paypal account. If you have intention to buy a remote please be patient and read the whole post as i provide some key/important things about it.

 After using it myself for 2 months everyday without a single problem I think it’s reliable enough to offer other people. Those of you who followed solidgeeks and ervinelins remote threads know that there has been numerous issues as well as quality updates. I tried to gather them and apply to my version. First of all wanted to eliminate most of the cables from the build so I went with a pcb design.
 Made some modifications to the case design so i could fit my pcb in the case and secure it with . I liked ervinelins code because I could switch between pages in the screen with a button instead of automatically switching between them. In order to use his code I added a button to the back of the remote and it’s completely optional you can use solidgeeks code aswell. If you are competent in programming I guess you can use that button for other purposes so it’s there as an option. 

Since installing different firmwares might be a thing in this remote I made it programmable from its usb socket without opening up the case. Changed 5v booster and charger modules with a single module and changed its resistor value so you can use your 2A phone charger to charge your remote. 

I had many issues with crappy seramic antenna nrf24 module so I’m using quality nrf24s instead. All nrf24 modules are behind 100uf tantal,10uf tantal, 100nf seramic caps for better power regulation. On receiver side there’s a 1000uf cap on 5v line for brownouts and 200uf tantalum cap on transmitter side.
Needing to reset on every boot was quite an issue thanks to arduino forums found this mcp130 chip and applied to 5v lines on both receiver and transmitter and there’s not a single issue using these since 2 months. 
2 switches, battery and an oled screen are connected with a jst connectors in case if you need to swap those components easily or to remove the pcb from the case.

**To summarize some differences from original design and some key notes;**
•	Receiver and transmitter are both pcb based and fixed to the shell of the remote with m2 bolts
•	Nrf24 power filter consists of 100uf tantalum, 10uf tantalum , 100nf ceramic cap (on both transmitter and receiver)
•	220uf tantalum cap on 5v(remote), 1000uf cap (receiver)
•	Programmable from usb socket fixed with 4 legs
•	Better nrf24 modules
•	5v booster and charging modules are replaced with a single module 
•	Mcp130 chip to solve power issues
•	Removable/replaceable switches, battery, oled using jst connectors
•	ABS printed parts in closed container
•	Mode button at the back of the remote
•	Tapped m3 bolts for the transmmiter
•	Clear heat shrink for the receiver


in my experience integrated antennas are not bad but not good enough. having at least one nrf module with external antenna either on remote or receiver side has a big impact on signal strenght(both with external antenna the better) so im including one nrf with external antenna and one with integrated. thats my setup aswell with carbon fiber battery enclosure + bamboo deck. didnt have a single dropout to this date.

**Finisihing and Colors**

Im printing with bright yellow ABS and its good as it is. Sanding only the burrs and edges for a smoother touch and applying clear coat gloss or matte paint. 
![IMG_0039|374x499](upload://9yD4cK4QgW4wwB3Bio4sVAqUWUs.jpeg)
I know some of you might like to have a different color or combination of colors for each part and much smoother surface. What i can offer as an option is sanding every part with 3 different grit sandpaper, apply 2 coats of filler sand again, 3 coats of paint of your choice, 2-3 coats of clear coat matte or gloss to finish the part. result is very nice and silky smooth, wouldnt say perfect but another level than 3d printed parts.
![IMG_0035|375x500](upload://koRpjJFg3aQ63nu11VD8bVs8olR.jpeg)
![IMG_0036|374x499](upload://qPAbET1WxQDsV67DAyuzD7oEF1g.jpeg)
![IMG_0042|666x500](upload://osfqZQnFoxGxTfgzSNbkvhRhfxU.jpeg)
![IMG_0038|666x500](upload://4N5i0HuC8Wh2Gc0ZwEWv0b0NSro.jpeg)

**NRF upgrades**

as i mentioned above im including quality Nrfs and one end will be with external antenna thats how i run my board too but if you want to have both ends to be with external antenna thats doable as an option.

**Free customization**
i will modify the receiver according to your VESC. Depending on your end i can include male/female/2.54mm pin or just bare cables. i have cables for both female and male options, so you need to note which one of the four options you need. For the uart connection i use 4p jst ph and it just works you need only 2 pins anyway. i will include what i have at hand but i see some uart ports has different positioning with tx/rx pins i need to see it so i can make a correct cable for your vesc. if its a focbox you dont have to tell me anything else because thats what i use too. 

**Shipping**

Theres a slight problem with shipping. My countrys national post does not allow any sort of liion battery doesnt matter if its removable or not you cant even send your cell phone thru the post unless you can remove its battery. If you would like have a remote from me and if you want me to ship it with national post you have to be able to source your own battery, remove 5 screws, twist or solder red to red black to black cables with supplied jst connector, insulate, put the screws back on. its an easy 10mins process due to pcb is held with screws and every cable is jst connector based. I will post an instructional video about the process. Another option is if you are in EU i can use a private company which has more expensive prices than the national post but better than UPS or DHL price wise.

**Pricing**
due to not having enough parts i cant provide kits at the moment. depending on the demand i will order the parts so i canbuild more.

Assembled remotes with receiver(without battery) **100$** + tracked shipping to anywhere around the world
for those of you who are in EU and want it with battery contact me for pricing about the shipping because the price is highly dependent on the country you are living.

**Extras**
paint job with a choice of your color(s) **15$**
nrf with antenna upgrade(includes antenna and nrf24) **7$**
i have 3-4 available semi assembled which would take couple of days to finish and test them, rest will be depending on the supply of the parts. 

Some more pictures:
![IMG_0059|315x420](upload://ybkhbwsj2cj8XHroPegglJTGDFr.jpeg)

![IMG_0093|288x500](upload://ynAMFEEtiOQWMxXDQBh7ygCgLkP.jpeg)

![IMG_0060|315x420](upload://1FViiu5qb6y4Pj0Fh3w83A31ZF1.jpeg)

![IMG_0096|666x500](upload://l9yl31rKioIq6DSgIulFls9TuNK.jpeg)

![IMG_0095|374x499](upload://9nXB3kbaRJ2l3Qn6IU58vUOghk5.jpeg)

![IMG_0094|374x499](upload://4GEzIUZuMlgu7DsSMk2vjNi15A6.jpeg)

![IMG_0100|374x499](upload://5JmcpgqqdEDk3BlycH882Nw5mdL.jpeg)

![IMG_0097|374x499](upload://g4SAhPuuaJjfAXaipf8e48Y6WOp.jpeg)
```

---
## \#2 Posted by: Jc06505n Posted at: 2018-08-28T15:07:24.980Z Reads: 435

```
First dibs, didn’t read it yet though 😂

Edit: Finished Reading Nice man , Super Clean! 

Danm if that Button was Connected to Switch I would've used it as a Momentary switch.
```

---
## \#3 Posted by: Zyb Posted at: 2018-08-28T15:12:11.458Z Reads: 429

```
Lol I suggest you read it thru tho 😂
```

---
## \#4 Posted by: Zyb Posted at: 2018-08-28T15:24:11.144Z Reads: 413

```
If I can’t reply to your private messages it’s due to my day work I ll get back to you as soon as I’m available
```

---
## \#5 Posted by: Moros Posted at: 2018-08-28T15:27:51.179Z Reads: 408

```
I'm interested in one but could you explain the NRF add on a little more?
In the post your say you've upgraded the remotes to a better NRF and an extra antenna is an option but in the add ons section you say its 7$ and includes antenna and NRF. So is it just an antenna added on and if I needed it could I just add my own antenna later on? I have a few extra for the metr module I have.
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-08-28T15:31:04.043Z Reads: 384

```
Question when you say 

[quote="Zyb, post:1, topic:66349"]
twist or solder red to red black to black cables with supplied jst connector, insulate, put the screws back on.
[/quote]

Does that still apply when you get a battery that already has a JST connector , this looks plug and play to me:

https://www.amazon.com/uxcell-Rechargeable-Lithium-Polymer-Battery/dp/B0798BZNDV
```

---
## \#7 Posted by: Zyb Posted at: 2018-08-28T15:37:54.132Z Reads: 361

```
@Moros
 [quote="Zyb, post:1, topic:66349"]
one end will be with external antenna thats how i run my board too
[/quote]
By one end I mean either transmitter or receiver and it works great that way. That’s included in the 100 price. Option is available if you want second end to be with external antenna aswell.
```

---
## \#8 Posted by: Zyb Posted at: 2018-08-28T15:39:49.879Z Reads: 345

```
Can you check if they are micro jst 1.25mm? I will include that crimped jst cable anyway but if that is 1.25mm it really is gonna be plug and play
```

---
## \#9 Posted by: evopanop Posted at: 2018-08-28T16:05:55.332Z Reads: 331

```
@Zyb Sent you a PM :slight_smile:
```

---
## \#10 Posted by: Battosaii Posted at: 2018-08-28T16:17:14.799Z Reads: 329

```
Looks great.
```

---
## \#11 Posted by: Jc06505n Posted at: 2018-08-28T16:22:14.530Z Reads: 321

```
Everything i found is 2mm the lowest being 1.5 :cry:
```

---
## \#12 Posted by: mmaner Posted at: 2018-08-28T16:23:39.068Z Reads: 315

```
Connector Type: 2P 1.5mm Pitch; Cable Length: 5cm / 2"
```

---
## \#13 Posted by: Jc06505n Posted at: 2018-08-28T16:28:59.972Z Reads: 311

```
The lowest I found, I'm going to order 10 through [Alibaba](https://www.alibaba.com/product-detail/3-7V-400Mah-Li-Ion-052535_60640478284.html?spm=a2700.7724857.normalList.21.1b9bae68LRgdSH) 

@zyb, The positive has to be on the left while the negative on the right , correct?
```

---
## \#14 Posted by: Scoo_B_SK8 Posted at: 2018-08-28T16:54:57.955Z Reads: 301

```
@Zyb 

Nice work!  PCB only way to go IMO.
```

---
## \#15 Posted by: Arzamenable Posted at: 2018-08-28T17:19:20.105Z Reads: 297

```
Nice! I have been using a trigger style remote based of the solidgeek remote. It is solid. I need more for other boards! PM sent.
```

---
## \#17 Posted by: Mich21050 Posted at: 2018-08-28T18:50:09.257Z Reads: 295

```
@Zyb You have a pm :smiley:
```

---
## \#18 Posted by: Zyb Posted at: 2018-08-28T21:00:39.155Z Reads: 288

```
Just came home ffrom work soon gonna answer your pms and questions also need to create an order form so I can know what you are after :) as there are couple of customization options regarding the receiver.
```

---
## \#19 Posted by: Zyb Posted at: 2018-08-28T22:33:03.758Z Reads: 317

```
[quote="Jc06505n, post:6, topic:66349"]
Question when you say

![|20x20](https://www.electric-skateboard.builders/user_avatar/www.electric-skateboard.builders/zyb/40/68913_1.png) Zyb:

> twist or solder red to red black to black cables with supplied jst connector, insulate, put the screws back on.

Does that still apply when you get a battery that already has a JST connector , this looks plug and play to me:

[amazon.com ](https://www.amazon.com/uxcell-Rechargeable-Lithium-Polymer-Battery/dp/B0798BZNDV)

![](https://images-na.ssl-images-amazon.com/images/I/41AI--WnoBL._AC_SY400_.jpg)

### [Amazon.com: uxcell Power Supply DC 3.7V 450mAh 502535 Li-ion Rechargeable Lithium Polymer Li-Po Battery: Home Audio &amp; Theater](https://www.amazon.com/uxcell-Rechargeable-Lithium-Polymer-Battery/dp/B0798BZNDV)

Description: This battery is really the latest state of the art technology in rechargeable. It is extremely thin, light weight and super thin compared to any rechargeable chemistry.Low weight, small s ...
[/quote]

i think thats jst zh and i may purchase some angled 1.5mm connectors and try to fit them in my pcb(1.25mm) or next iteration of pcbs will be with 1.5 connectors so it can be a plug and play.

[quote="Jc06505n, post:13, topic:66349"]
@zyb, The positive has to be on the left while the negative on the right , correct?
[/quote]
yes exactly!

everyone wants their remote sooner and i understand that i just wanna be fair to everyone. its kinda my mistake for not having enough parts. i will order more tonight but before that i will create an order form within an hour with every detail i need from you regarding the remote and first 3 + 1 without the battery will get their remote sooner than the others. so its gonna be first come first served. 

also will shoot a video tomorrow demostrating how easy it is to hook up the battery, then you can decide to go with or without it.
```

---
## \#20 Posted by: pjotr47 Posted at: 2018-08-28T23:19:24.412Z Reads: 287

```
Looks very good! Is there a way to buy only the PCB? Or is there a discount on bulk orders?
```

---
## \#21 Posted by: Zyb Posted at: 2018-08-28T23:25:20.787Z Reads: 275

```
Kits and individual parts are sadly not possible as i cant even supply the demand at the moment. only thing i can offer is the 3d prints for the remotes for around 10$ but i think there are alot of sources for that. Bulk order and a discount is possible but i need finish with invidiual orders first :/
```

---
## \#22 Posted by: Zyb Posted at: 2018-08-29T00:37:16.711Z Reads: 273

```
Form is up guys i hope i didnt miss anything i will check back tomorrow. first come first served according to the order completion date and time :) 
https://goo.gl/forms/1e5Z04BQb3fVFsgP2
```

---
## \#23 Posted by: uigiroux Posted at: 2018-09-05T04:03:53.979Z Reads: 261

```
I just got a kit from @SeeTheBridges for the Firefly remote and am wondering how yours differs from his..?  It seems like your design with the PCB's and nrf and separate or external antennas is more reliable.  Love the finished quality of your 3d prints :heart_eyes:  Also, you mention just EU shipping, so would it be possible to get this in the US (without battery I imagine)?
```

---
## \#24 Posted by: Zyb Posted at: 2018-09-05T09:00:51.209Z Reads: 265

```
You can still use his version it’s totally ok I just made some more mods upgraded some components etc to suit my needs. It is possible to send it to US I mentioned it in shipping section tho there’s an update..
I see most of the people want it without a battery. Currently you have to remove the top cover, remove the pcb from the shell, prepare the battery with supplied jst 1.25 cable, put everything back and done.
I switched places of most of the components so arduino and nrf is under the pcb and battery/5v boost is on top now. Also battery connector is jst ph 2.0 now because I noticed most of the batteries comes with that connector. Installing a battery will be a matter of removing the top cover plug in the battery connector and done. Putting arduino under the pcb increased the clearance and blocked the trigger motion so I had to make a cutout for it too. Also added pre drilled holes for fixing the pcb down instead of drilling them manually. There’s another version I did with tp4056 and 5v booster and external lm1117 3.3v chip see how they will turn out. Pcbs already ordered so I ll have to delay your remotes sorry for the inconvenience but I’m trying to make it better in some areas :) also ordered more parts waiting on them aswell.
```

---
## \#25 Posted by: pjotr47 Posted at: 2018-09-17T21:13:02.129Z Reads: 238

```
Is it possible to only buy the pcb?
```

---
## \#26 Posted by: boramiNYC Posted at: 2018-09-17T21:26:42.030Z Reads: 252

```
After using firefly remote for two weeks of commuting, there's a weakness that haven't been discussed. The cylinders (bar) that hold the spring tensioner and trigger both broke on mine from seethebridges version. I think it needs to be a lot stronger. I'm gonna try to put metal pins, rods there. If you want to improve the quality of your remote, pls consider this.
```

---
## \#27 Posted by: StefanMe Posted at: 2018-09-17T21:41:54.124Z Reads: 264

```
I have done the remote on an complete Version with bearings... i also replaced that weak part with an steel screw hole.
![image|374x500](upload://nshXnznv3WgOIPVJhHc4Q1LHYdq.jpg)
![image|374x500](upload://wy0OGXF18cJptqCnaTRJMSS9bLe.jpg)
```

---
## \#28 Posted by: Zyb Posted at: 2018-09-17T22:24:24.170Z Reads: 248

```
could be from the quality of the print also he was using pla to print his versions. abs is much stronger and tolerant to bending never had an issue with mine. tho before i started to print them myself i was using print services to get couple of samples and pieces were literally falling off of the remote. obviously they had some layer adhesion problems that may cause it too. 
@pjotr47
as long as theres no order to fulfill of course its possible to get the pcbs tho im still waiting for the new version. could be other iterations too as im thinking to add some other functionalities but that for another time :D

edit: btw if you can print the bottom part its very easy to implement those metal pins and it will indeed be very strong. you just need to hollow places where those bars are gonna go in and some 4mm diameter pins. let me know if you need help with modifying the stl file.
```

---
## \#29 Posted by: hoeksame1 Posted at: 2018-09-21T07:04:41.255Z Reads: 234

```
Pm send   .

Gr sam
```

---
## \#30 Posted by: KranzeKake Posted at: 2018-09-24T13:44:40.691Z Reads: 236

```
Hi, Im trying to order the remote, but I have some questions. I will be using two of these. collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller . When ordering, what option should I choose when it comes to the UART and PPM page?
```

---
## \#31 Posted by: Zyb Posted at: 2018-09-25T14:30:56.474Z Reads: 231

```
Hey, had a minor accident couldn’t reply earlier. So you need to select male ppm cable and jst ph 4 pin for uart.
```

---
## \#32 Posted by: KranzeKake Posted at: 2018-09-25T14:43:23.620Z Reads: 230

```
Thank you, hope everything is okey with you, cant wait for the remote :)
```

---
## \#33 Posted by: uigiroux Posted at: 2018-09-25T14:46:15.137Z Reads: 224

```
You ok bro?   Pics looked pretty gnarly, lol.
```

---
## \#34 Posted by: Zyb Posted at: 2018-09-25T14:46:20.636Z Reads: 229

```
Yea near miss 😅 going to have a functional hand in couple of days I hope waiting for the new pcbs anyway can’t progress without them
```

---
## \#35 Posted by: Zyb Posted at: 2018-09-25T14:49:15.203Z Reads: 228

```
Yea thanks I’m fine tho I learned a lot from that fall 😅 could have been a lot worse
```

---
## \#36 Posted by: mtuan293 Posted at: 2018-09-25T15:44:14.009Z Reads: 225

```
Are you still making it? Can I order it now?
```

---
## \#37 Posted by: Zyb Posted at: 2018-09-25T16:52:12.371Z Reads: 227

```
Planning to but the thing is I designed it from scratch for the second time and it all depends if the new pcb is functional which I’m expecting them this week.. hopefully 😁 got 2 versions with different component combinations. I ll have to test them all
```

---
## \#38 Posted by: mtuan293 Posted at: 2018-09-25T16:59:18.605Z Reads: 221

```
Oh that’s awesome! Keep us posted :grin:
```

---
## \#39 Posted by: Zyb Posted at: 2018-09-25T17:00:25.099Z Reads: 219

```
And there are some key mechanical durability improvements coming on I ll have more info when parts arrive.
```

---
## \#40 Posted by: ElectricCoast Posted at: 2018-09-26T12:51:31.612Z Reads: 222

```
I need 2 to 3 of these remotes.  What's the lead time to make and ship to the USA.  I can source the battery stateside.  I'll need some remotes in 2 to 3 weeks.  Thanks in advance for answering my questions.
```

---
## \#41 Posted by: Kit Posted at: 2018-09-26T13:54:20.804Z Reads: 223

```
Order submitted! I don't mind waiting for a bit while parts are tested, everything looks fantastic & it can only get better :stuck_out_tongue_closed_eyes:; will you be able to notify the payee via email before beginning work on their order?
```

---
## \#42 Posted by: ElectricCoast Posted at: 2018-09-26T14:29:14.123Z Reads: 217

```
I feel like a simpleton but which receiver is this designed to pair with?
```

---
## \#43 Posted by: Surfer Posted at: 2018-09-26T14:43:11.249Z Reads: 217

```
I filled the form!! Just to mention there is no option for ppm Vesc6.4 which is JST.
```

---
## \#44 Posted by: Zyb Posted at: 2018-09-28T08:32:01.558Z Reads: 210

```
at this point i cant give you an info about lead time i dont want to promise false time frame shipping is not under my control and because of that im still waiting for the pcbs which they must have arrived this week. receivers are there between the pictures in the first post.
@Kit
yea when i start building i will contact you for the confirmation of selections etc and send you invoice only when its ready and tested. 
@Surfer
oh ok i didnt know i ll make sure to add that do you know the pitch of that jst type?
```

---
## \#45 Posted by: ElectricCoast Posted at: 2018-09-30T10:30:13.807Z Reads: 202

```
If memory serves me correctly I can use this remote on multiple boards as long as I have the receivers to pair it to is that correct?  If so I'll need to order 2 remotes and 3 receivers.  I'll need a remote and then my son will need a remote plus I have another board I'll need to use my remote with.  I filled out the form but it doesn't give a selection for multiple remotes and receivers.  I know you can't guarantee lead times on shipping but do you know if the remotes will take 1 week, 2  weeks etc.. to make?  Thank you so much for making these for us.
```

---
## \#46 Posted by: Zyb Posted at: 2018-10-02T14:43:16.145Z Reads: 195

```
Yes of course as long as you have the same pipe on receivers and the remote you can use your remote with many boards.
Problem is those pcbs took very long time to arrive. Shipping company despatched it to overseas on 11/9 and it is yet to arrive. In the meantime I had another battery pcb order on 29/09 and it just arrived today. I guess it’s lost or something. I ve got no patience god knows when they gonna arrive so I’m gonna make another order with DHL delivery at least they say it’s 3-4 days delivery.
```

---
## \#47 Posted by: ElectricCoast Posted at: 2018-10-02T14:45:07.885Z Reads: 192

```
OK well count me in for 2 remotes and 3 receivers.  The order form doesn't clarify if I would need multiple items.  Thanks for everything.
```

---
## \#48 Posted by: uigiroux Posted at: 2018-10-02T16:04:36.159Z Reads: 197

```
Would you be able to tell me around where I am on the ordering list?
```

---
## \#49 Posted by: KranzeKake Posted at: 2018-10-10T16:32:41.099Z Reads: 189

```
Any updates? Really looking forward to getting my remote!
```

---
## \#50 Posted by: jimmymagix Posted at: 2018-10-14T20:14:28.822Z Reads: 191

```
Sorry to bug you but I would also like to know where I am on the list. I just ordered it and I'm completing my build over winter so it would be good for my planning to figure out when I'm roughly going to have all the bits together and ready. I'm really happy I found this thread though, this remote is precisely what I've been looking for!
```

---
## \#51 Posted by: uigiroux Posted at: 2018-10-14T20:24:55.912Z Reads: 200

```
This design he's doing is so much more well designed internally.  I had a kit for this remote, and when I saw all the work I'd have to do, and the crazy amount of wires that had to be routed everywhere I said fuck it and I sold that right as this design came out.  Perfect timing I must say!
```

---
## \#52 Posted by: ElectricCoast Posted at: 2018-10-15T04:38:57.507Z Reads: 200

```
I'm curious as well
```

---
## \#53 Posted by: Zyb Posted at: 2018-10-15T08:37:10.142Z Reads: 201

```
![image|395x500](upload://gwi7eZDPspzrHaMsP47znjajlKh.jpeg) 
This is the current build guys. I know it’s moving slowly but god damn design evolves literally everyday :) there are things I added which are not even present in the picture but mostly internal design will be like this with battery on top. It’s connector is jst ph 2.0
```

---
## \#54 Posted by: AreaKruzer Posted at: 2018-10-15T10:27:18.792Z Reads: 196

```
Looking clean and tidy.
```

---
## \#55 Posted by: Surfer Posted at: 2018-10-15T12:09:30.182Z Reads: 189

```
Hi Zyb, just  an idea to reach more tastes, I did used this remote and really miss a short throw option on the thumb wheel.
Some people love the long travel response and some other like me prefer a short travel. Maybe can you provide another thumb wheel with holes for the magnets more close to each other?
Btw that's already sooo sick!!
```

---
## \#56 Posted by: walleywalker Posted at: 2018-10-16T22:28:24.573Z Reads: 182

```
Can't wait. This is damn clean looking.
```

---
## \#57 Posted by: brenternet Posted at: 2018-10-16T22:34:52.547Z Reads: 182

```
Hi @Zyb, Just wanted to confirm I am on the list please?
```

---
## \#58 Posted by: ElectricCoast Posted at: 2018-10-25T23:51:04.719Z Reads: 164

```
How's the parts acquisition coming along?
```

---
## \#59 Posted by: Earlbond Posted at: 2018-11-19T05:07:30.291Z Reads: 153

```
Hi I'm new here so I was wondering if your version of the Firefly remote is compatible with the new focbox unity
```

---
## \#60 Posted by: uigiroux Posted at: 2018-11-19T09:03:18.922Z Reads: 154

```
It would be fine with the Unity.  You just hook up the receiver and pair them I believe.
```

---
## \#61 Posted by: jimmymagix Posted at: 2018-11-24T06:44:50.494Z Reads: 160

```
When do you think you'll be in place to sell these again? I'm doing a build over winter just now and I'm getting close to needing a remote for it. I've already submitted an order a while ago but I see that everything is on hold - just looking for a rough idea when things will be moving.

The work you've done is fantastic by the way.
```

---
## \#62 Posted by: StefanMe Posted at: 2018-11-25T19:19:31.607Z Reads: 147

```
Firefly Nano Remote by DroidSector...
Feather Remote StefanMe (Me 😬)...
Trigger style Remote by ervinelin...
There are plenty other builds of remotes at the moment. Why u don’t choose another more improved version?
```

---
## \#63 Posted by: sodniwe Posted at: 2018-11-26T20:15:37.204Z Reads: 150

```
I've been following this build and it seems that this will be a high quality improved version (which is why it's taking longer to finish).  I haven't tried all the remotes so can really say which one is better but props to @Zyb for taking his time and focusing on making a quality product.
```

---
## \#64 Posted by: Zyb Posted at: 2018-12-08T14:51:36.297Z Reads: 154

```
Speaking of updates, ditched every single external board like booster charger module even arduino. Only external pcb is the nrf24. Going well uploaded a sketch and it is working good so far. Made a charging led to see the status which turns off when it is fully charged. Going to test it further with the nrfs tonight and btw installed adafruit feather bootloader tho I influenced highly from sparkfun board I might try their bootloader too.
![image|375x500](upload://bP1PbnXKepO2xIgQJP9eNydeniN.jpeg) ![image|375x500](upload://utjWgUdleTolh7ViP0QK9RqaJ5K.jpeg) ![image|402x500](upload://mwVpd3mirouEDrwqdI1CsLHrmFu.jpeg) ![image|375x500](upload://msycFryiKA0fQmkNm84lqjOrsZT.jpeg)
```

---
## \#65 Posted by: Zyb Posted at: 2018-12-09T15:04:52.521Z Reads: 144

```
receiver is done aswell time for testing :) 
https://www.youtube.com/watch?v=IWQuSWRRCyw&feature=youtu.be
```

---
## \#66 Posted by: nuttyjeff Posted at: 2018-12-09T15:10:00.691Z Reads: 146

```
Damn i love that vid haha. Great work.
```

---
## \#67 Posted by: Zyb Posted at: 2018-12-09T15:11:08.130Z Reads: 147

```
Thanks 🙂 taking no shortcuts. More updates are on the way
```

---
## \#68 Posted by: uigiroux Posted at: 2019-02-06T13:42:10.577Z Reads: 116

```
Any updates??? 😁
```

---
## \#69 Posted by: Zyb Posted at: 2019-02-17T12:42:56.740Z Reads: 117

```
Damn I don’t get notifications to my mail I didn’t see your message :/ anyway there are good news. I finally succeeded with casting and I would say they turned out better than I expected. There was so many problems along the way sadly it’s not easy like 3D printing, one mistake costs you bunch of materials and a lot of time compared to 3D printing only filament. But it’s all good now phew 😅 
There was couple of challenging points I wanted to add to the design which is metal inserts. In my previous experience I tried to press fit them with heat like they are intended to use. At first they work but if you apply abit more force they come out of their socket somewhat easily. That was a big let down here is the example, it looks good but very very weak ![image|547x500](upload://QCuCRP19lVtQT17Xoj2jJLcvTK.jpeg) 
So my goal was with casting to embed these inside instead of putting them with heat after the remote is done. I finally figured out a way to do it and buried them in the remote so they are not even visible from the outside but they are in there. It became so strong that casing will break into pieces before these fail on you there’s no way to force them out. I cut up a piece from failed cast to demonstrate it, here it is
![image|375x500](upload://2IC1FS0JY6CHuiQMp4A8YrYXjWH.jpeg)
There were couple types of polyurethanes that didn’t work and gave me a hard time and without degassing the mixture with a vacuum chamber it’s not a decent product. So all of the parts going on thru the vacuum chamber prior to casting. 
My main reason to contact you is to give you choices and show you what I have. Let me know what you choose and I will start on the electronics in couple of days if all goes well you will have it soon.
Ok to the matter,
So I also bought couple of powders and dyes which I’m mixing them during casting. Whiteish one is a raw casting without any additives ![image|375x500](upload://slDYIWWilNInqUCTiwaQhd2TFSb.jpeg) ![image|375x500](upload://38Z0ISpoxZeb8wKW8JPxuRUj4uw.jpeg) ![image|666x500](upload://asUwkJh4hkrvKsrWbDNqcVsW3Em.jpeg) 
Then I have these with plain black pigment
![image|375x500](upload://lM0dQJdjwLKd41XrLwKjOUCiJLZ.jpeg) 

With graphite powder, it has a very faint sparkle to it kinda cool
![image|375x500](upload://w91KgniO0RJQgdaIkjQ2uDuQkTe.jpeg) ![image|666x500](upload://sihg8uWvDy6I0ayDlJwIxRtZVSE.jpeg) ![image|666x500](upload://1GuZ9aEoFzMfdoqoh4fsrK89XVn.jpeg) 
With lower mixed ratio of graphite powder
![image|375x500](upload://a3Y9O37BjsMzscGy6c4LtgsEdxX.jpeg) 
And I made this one with aluminium powders and gave it a worn out look. It has around %50 of real aluminium powder mixed into it. It is abit more heavier and harder
![image|375x500](upload://cqkiGEe66VgywIM4dbTCttlF6bH.jpeg) ![image|375x500](upload://4F3D2JkJS5PbHPMX1rqvixYcg01.jpeg) 
And then there this one like brushed aluminium effect again it has the same ratio of aluminium powders mixed into it that where this shine comes from. Tho there’s still no protection layer on this one. I might add gloss or matte coat and that’s going to effect the look as well all previous ones already have protection clear layer on them.
![image|375x500](upload://7lr4a6VW1mHBw2xOoZb53LmkQIs.jpeg) ![image|375x500](upload://unCtVvAaDYavmJxewJlhHpzhvI9.jpeg) ![image|375x500](upload://2txeRq3wouIPWRmS75Ghpc6s8KK.jpeg) 
That’s all about it and of course I can still make your original choice of colors I have those cans of paints. It’s a matter of spraying it on that whiteish version. So you have many choices let me know which one you want and I ll keep on working on it. Oh and by the way even the buttons and wheels are casted not a single piece is 3 printed 😂 here’s bunch of them 
![image|666x500](upload://qf931sN6MWuTXEk6vz53Yc9t2yI.jpeg)
```

---
## \#70 Posted by: Zyb Posted at: 2019-02-17T12:53:37.874Z Reads: 111

```
Oh and probably I should open a new thread this last version has nothing to do with pervious one.
```

---
## \#71 Posted by: X09 Posted at: 2019-02-17T20:48:52.222Z Reads: 103

```
Please do!
I am highly interested in your remote!
```

---
## \#72 Posted by: Gerrycorrado Posted at: 2019-02-17T21:33:13.800Z Reads: 100

```
Aluminium please! (worn or brushed, whatever looks best in real life)
```

---
## \#73 Posted by: Zyb Posted at: 2019-02-17T21:58:58.077Z Reads: 99

```
![image|281x500](upload://fWRb4FCRO2GZbMEVTCuwzphnFQP.jpeg) This is the screen I’m going with. I really liked multi Color screen when I had the remote of the evolve bamboo gt. So want to have a space on it with different Color to grab your attention for certain information. This is not the final layout but I guess it’s going to be similar.
```

---
## \#74 Posted by: KranzeKake Posted at: 2019-08-18T21:06:23.383Z Reads: 34

```
Any news? Really dont want this project to die....
```

---

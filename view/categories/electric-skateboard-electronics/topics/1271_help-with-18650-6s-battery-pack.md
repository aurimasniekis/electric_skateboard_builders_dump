# Help with 18650 6s battery pack

### Replies: 45 Views: 7961

## \#1 Posted by: delta_19 Posted at: 2016-02-08T01:58:38.036Z Reads: 289

```
so i want to make my own 18650 pack and have some questions.

first do i need a bms? cant i just have a balance lead for each cell group and charge it like a normal lipo in a sense?

second how much amperage should a good pack be able to give out? i was thinking 4p so i could get 80-100 amps constant, is that to much would 60-75 be ok?

last is it really worth it? is it really worth it over the standard zippy lipos everyone uses? lets say money and time are not an object are 18650 packs worth it?
```

---
## \#2 Posted by: paragon Posted at: 2016-02-08T03:11:02.177Z Reads: 283

```
Generally, they are safer and last for more cycles. If you have a good bms, you can charge them with a "dumb" charger. They are much more expensive than my 10c multistar lipos though.
```

---
## \#3 Posted by: laurnts Posted at: 2016-02-08T03:11:39.352Z Reads: 276

```
Personally I believe that people are using BMS simply because of ease of use. They want the single plug and charge solution, instead of plugging 2 cords and going through balance charging. It's also safer in terms of protecting the batteries from shorts and low voltage. Hence I don't think you really really need one.

100A continuous is way too much. VESC only draws peak 60A. Tested with multimeter, motor 200KV'ish only draw about 5 - 15A peaking at 20A tops on relatively flat ground (I weight 65kg). You will drain your battery super fast if you ever draw 100A and currently not much shady cheap chinese ESC that can handle 100A constant while pulling dead weight over kilometers of distance.

The reason i switch to li ion because of less risk in getting my entire build burned down due to bad lipo. Lipo has really descent -to- short charge cycle even though they have higher energy density per pack. I believe big lipo packs are also rejected by air ports and air carriers because of safety reasons.

---

If you're not in a rush, wait for that graphene lipo packs are abit cheaper. If you have the money then try get one :D Since I believe not getting a BMS is because it's too hard to install or getting SPACE cel are too expensive, then it's better to just stay with lipo and get new one if it's shows bad symptoms.
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-02-08T20:25:34.936Z Reads: 252

```
pretty much what @laurnts said. You can get a decent BMS on Ebay though for not a lot of cash, and if you can squeeze it in there, its a much better solution than an outboard programmable charger if you don't have a whole stack of lipos to charge as well. 

but i'm all about integration. I'm also about keeping my packs balanced, and a BMS can do that and extend the life of your pack in doing so.
```

---
## \#5 Posted by: barajabali Posted at: 2016-02-08T20:30:22.883Z Reads: 239

```
i dont use a BMS. i just attach balance leads on to it and use my lipo charger! lol i charge at low amps. and i monitor it constantly.
```

---
## \#6 Posted by: delta_19 Posted at: 2016-02-08T21:20:18.671Z Reads: 230

```
ok well then my next question is would this be a [ good bms][1] and if so how would i go about charging it with this [laptop charger?][2]


  [1]: http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html
  [2]: http://www.batterysupports.com/liion-lipo-252v-222v-2a-6s-wall-socket-battery-charger-ac-dc-p-135.html
```

---
## \#7 Posted by: laurnts Posted at: 2016-02-08T23:26:42.461Z Reads: 223

```
BMS is determined most likely from the voltage and amps it could discharge. The one you have with your link seems to be good for 6S with a nice discharge capability. To be honest, I have not much experience with good or bad BMS. I have experience with a fake chinese product that uses bms and it appears to be fine.

The charger appears to be in good selection as well. 2A charging current is the safest route for long life cycle. I personally looking for 5A'ish power supply since I have 10000mah, charging 2A is really slow.
```

---
## \#8 Posted by: delta_19 Posted at: 2016-02-11T12:48:48.413Z Reads: 216

```
So I ordered 48 Samsung icr18650 25r5 cells but have a question about charging.

If I use one of the following BMS boards where the charge and discharge leads are the same how should I change?

Option 1: one set of leads with a dean plug and use my old lipo charger.

Option 2: run 2 leads from both pads one for charging one for discharge with a 100A switch to close of the discharge leads when charging or not in use.

http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html

http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html
```

---
## \#9 Posted by: lowGuido Posted at: 2016-02-12T12:22:01.739Z Reads: 209

```
there is 3 pads, one is for the battery negative one is for the battery positive and one is for the charge negative. 
you don't need to use a lipo charger because the BMS will control charging.
```

---
## \#10 Posted by: delta_19 Posted at: 2016-02-12T13:15:08.291Z Reads: 199

```
I was gonna use the lipos to supply the power not to balance. also there is no pad for positive on this bms and the negative pad is for both charge and discharge.
```

---
## \#11 Posted by: lowGuido Posted at: 2016-02-12T13:26:15.603Z Reads: 194

```
ah sorry my bad, I misread the description. so in that case you just have B- to your battery -ve and P- to your charge port and ESC -ve
```

---
## \#12 Posted by: delta_19 Posted at: 2016-02-12T14:09:23.828Z Reads: 187

```
So as long as I have cut-off switch between the esc and battery I can throw a charger on the battery aswell to have a spacecell like set up?
```

---
## \#13 Posted by: lowGuido Posted at: 2016-02-12T14:40:29.541Z Reads: 180

```
thats right. thats exactly how the space cell works
```

---
## \#14 Posted by: delta_19 Posted at: 2016-02-12T15:49:57.794Z Reads: 179

```
Well then when my spot welder and batteries show up that's what I'm doing
```

---
## \#15 Posted by: delta_19 Posted at: 2016-02-29T03:11:26.534Z Reads: 166

```
well got the batteries and tested the crap out of them. they are legit and so sexy.... no im  not aroused by batteries stop asking. 
heres a link to the ones i bought. http://vitaltech.en.alibaba.com/product/60383730345-801914430/Wholesale_Authentic_Samsung_25R_18650_samsung_INR18650_25R_2500mah_samsung_sdi_18650_2500mah_battery_cell.html

if you want any ask to do the transaction via paypal.
```

---
## \#16 Posted by: Hummie Posted at: 2016-02-29T04:02:57.039Z Reads: 164

```
How do u know they're legit?  How much was it for shipping and can they sell less?  24? That looks like a great deal 
  I think li-ion has more energy density and less power density.  Don't know if that's by weight or size compared to lipo.  

I plan to wire two sets of 12 in series and two rows in parallel, (50 volts and 5amphour) and glue/pot them to my board with 70duro clear rubber without balancing wires but instead balance them individually with...a big light bulb or something. It will be very manual.  And charge them with a 50 volt bulk meanwell charger I have. 

Per mile li-ion maybe are cheaper.  Safer. Thinner..my lipos skim the ground.
```

---
## \#17 Posted by: delta_19 Posted at: 2016-02-29T04:10:45.184Z Reads: 159

```
The smallest amount they sell is 30 for 3.6 a cell. Shipping was 65. I know they are legit because I spent the last 30 hours running charge and discharge test to get the capacity of the cells and compared the discharge curve to what Samsung has published. Also they have all the little hidden markings that you find on Samsung 25r batteries.
```

---
## \#18 Posted by: Hummie Posted at: 2016-02-29T05:28:46.903Z Reads: 157

```
❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️💔
```

---
## \#19 Posted by: Mathieu Posted at: 2016-02-29T08:34:25.217Z Reads: 156

```
Not an expert but i think You can really save On BMS and get a lower amp rating and Just use it for Charing. Then for discharge you rely on the esc cutoff
```

---
## \#20 Posted by: delta_19 Posted at: 2016-02-29T22:18:27.328Z Reads: 156

```
what do you mean just use it for charging?  also lower amp rating? if anything i want a higher one but cant find a good 80A bms for around the same price.
```

---
## \#21 Posted by: Mathieu Posted at: 2016-02-29T23:18:43.502Z Reads: 141

```
You only connect to the bms for charging.. For discharging you connect it straight to the battery itself. That way you only need a bms that supports your charging current, like 5-10 amps or so. And for discharging you protect the battery with the low voltage cutoff from your esc. That way you don't need a high current bms sinecure you don't discharge trough the bms but straight from the battery to the esc. I'm not 100% sure but i think it would work. Get it?
```

---
## \#22 Posted by: delta_19 Posted at: 2016-02-29T23:26:34.219Z Reads: 133

```
oh thats what you mean, yeah that would work but having a bms on all the time is a much better option.
```

---
## \#23 Posted by: Mathieu Posted at: 2016-03-02T00:38:07.713Z Reads: 133

```
Would it matter that much? As long as the esc cuts of at the right voltage, what would the bms do more during discharge?
```

---
## \#24 Posted by: Hummie Posted at: 2016-03-02T02:01:50.739Z Reads: 134

```
The bms would monitor each cell and tell you when ...you're just about to explode. It's that one second extra where you have just enough time to launch your board as far away as possible from small children. Shoot for the elderly.
```

---
## \#25 Posted by: delta_19 Posted at: 2016-03-02T02:21:14.521Z Reads: 130

```
i like old people lets kill some little bastards
```

---
## \#26 Posted by: lowGuido Posted at: 2016-03-02T14:35:45.202Z Reads: 133

```
meh.. I like to live dangerously. No BMS for me.
```

---
## \#27 Posted by: delta_19 Posted at: 2016-03-02T14:58:15.549Z Reads: 133

```
I'm really trying to figure that out myself. I save $50 going BMS-less but I like the idea of a no worry plug and go battery.
```

---
## \#28 Posted by: lowGuido Posted at: 2016-03-02T15:01:22.361Z Reads: 130

```
if you want the easy plug in a simple charger and not worry, then BMS is the way to go.
if you are happy to have complicated charging cables and specialised chargers, and know what you are doing, its ok to go BMS-less
```

---
## \#29 Posted by: delta_19 Posted at: 2016-03-02T15:03:20.992Z Reads: 131

```
Well if I went BMS-less I was just gonna use the 6s lipo charger I have now
```

---
## \#30 Posted by: lowGuido Posted at: 2016-03-02T15:07:41.902Z Reads: 130

```
yeah that will work.
```

---
## \#31 Posted by: delta_19 Posted at: 2016-03-02T23:54:49.438Z Reads: 124

```
anyone here know how long it takes besttech to reply to an email?
```

---
## \#32 Posted by: lox897 Posted at: 2016-03-03T05:29:10.620Z Reads: 125

```
I skyped them 6 months back for a BMS question and still no response.
```

---
## \#33 Posted by: delta_19 Posted at: 2016-03-03T12:30:29.301Z Reads: 129

```
I emailed yesterday and got a response just now
```

---
## \#34 Posted by: longhairedboy Posted at: 2016-03-03T15:12:49.277Z Reads: 124

```
i usually just set my board on fire before i even start riding.
```

---
## \#35 Posted by: delta_19 Posted at: 2016-03-03T15:37:51.256Z Reads: 127

```
....... not sure who's expenses that joke is at. I burnt down my room once already.
```

---
## \#36 Posted by: longhairedboy Posted at: 2016-03-03T15:59:42.208Z Reads: 126

```
Not all jokes are at some individual's expense. It was a stab at lithium chemistries in general.
```

---
## \#37 Posted by: Hummie Posted at: 2016-03-03T16:17:40.919Z Reads: 128

```
We're talking li-ion at least.  Did u burn ur room with lipo or ion?  How'd it happen?

Been fantasizing about riding with my batteries on fire.  I'll want to keep rolling to keep the fire falling behind the escs and motors
```

---
## \#38 Posted by: lowGuido Posted at: 2016-03-03T16:42:29.734Z Reads: 128

```
my mate burned down his whole house, so I know these batteries are not to be fucked with.
but if you are careful and keep everything within its tolerances it should be ok.
```

---
## \#39 Posted by: torqueboards Posted at: 2016-03-03T17:01:08.655Z Reads: 134

```
Yeah, we just need more knowledge + care for these type of things. In a sense, we are dealing with a specific power tool or technology which needs to be handled as such.

It's not any different from a match, lighter or power tool.

Specific tools need to be handled with specific care.

A lighter can burn your house down.. but do you get mad at the lighter company for offering/selling it?

LiPo or 18650 cells can all catch on fire even LiFePo4. Education is our best solution.

<img src="/uploads/db1493/original/2X/a/ab3e7edf4885a8cedd6668a23df5169cdf2007f1.png" width="347" height="500">
```

---
## \#40 Posted by: delta_19 Posted at: 2016-03-03T17:05:27.115Z Reads: 129

```
lipo, it was some hobby stores brand of lipo and their brand of charger, one or the other was a cheap POS and it ended up exploding. lucky for me the shacks are made out of asbestos and crushed dreams so only my board burnt down.

also thinking of going with 6 of [these][1] and just beefing up the wires to 10awg then getting a 4 cell charger and a second set of 18650's so i can have one off and one on. 


  [1]: https://www.fasttech.com/products/1009/10002233/1290003
```

---
## \#41 Posted by: Hummie Posted at: 2016-03-03T19:23:10.733Z Reads: 121

```
I hear of them blowing up while charging more often than not.  Maybe we rely on the Chargers too much.  They're complicated.  I'm feeling safer with a bulk charger and balancing manually
```

---
## \#42 Posted by: delta_19 Posted at: 2016-03-04T00:41:14.559Z Reads: 121

```
so looking in to that holder might be to weak so gonna get 12 of [these][1] seeing as how they are made for high current draw high heat builds. heat wont be a big problem though when im rocking at 22km. 


  [1]: http://www.brimstonevapeco.com/product-p/slim-dual-18650.htm
```

---
## \#43 Posted by: Hummie Posted at: 2016-03-04T01:21:50.088Z Reads: 121

```
What happens at 22km?

Are u planning on soldering them into the "sled" or were u thinking of having them be removable?  I never hear of them being removable unless they're in a compression of some sort
```

---
## \#44 Posted by: delta_19 Posted at: 2016-03-04T01:25:17.839Z Reads: 120

```
22km is my max speed so max airflow over the sled.

and this is just a beefy AAA/AA/C/D holder like you would see in a TV remote so it holds it in via compression plus im gonna have lid on them to help hold stuff in place.
```

---
## \#45 Posted by: delta_19 Posted at: 2016-03-06T04:20:00.179Z Reads: 113

```
holy crap there are some useless people on endless sphere.... 

just want to know if the sleds i want to use will work at my amperages theres no need to go off topic on every other post or call me lazy for seeking a second opinion.
```

---

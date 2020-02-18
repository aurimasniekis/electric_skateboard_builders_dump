# VESC6 new spec?

### Replies: 46 Views: 2935

## \#1 Posted by: uigiroux Posted at: 2018-03-27T14:26:01.008Z Reads: 406

```
Hey so is Trampa now making a dual VESC 6 that can handle higher amount of power?

New
![Screenshot_20180327-091837|666x500](upload://mZtuGmlSqCeTgQkOJaKXws3fHRI.jpg)
Old
![Screenshot_20180327-091810|585x500](upload://2Xww506RMWXPlUS2s22O4yM0OV5.jpg)
```

---
## \#2 Posted by: sayekim Posted at: 2018-03-27T16:37:32.901Z Reads: 377

```
Yeah saw that too wasn’t sure. Must be one of their original patented designs. Guess we’ll see what this will cost
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-03-27T16:47:32.802Z Reads: 373

```
That's not dual and that's not trampas
```

---
## \#4 Posted by: uigiroux Posted at: 2018-03-27T17:23:43.378Z Reads: 363

```
I don't know how that isn't dual... It's got two power in cables on one side and then two sets of the three phase wire cables on the other side.  It's exactly like one of your dual FOCBOX enclosures with the cables, functionality wise, obviously not exactly the same.  If it isn't a dual VESC 6, why does it need two inputs for power?

![Screenshot_20180327-121001|690x371](upload://yqPg9qcqR6CIOSZfTcjMKOqDIBe.jpg)

I don't really understand what you mean when you say those aren't Trampas.  They're licensed to manufacture and sell them under the Trampa brand, and it's printed on the front of the VESC...  

![Screenshot_20180327-122040|494x500](upload://voTPou4TcqW3pPe1eZKNAwPlVvO.jpg)

Regardless, I'm not trying to debate semantics or split hairs so to speak, I'm just curious about this apparent looking dual VESC 6 which appears to be able to run at a higher power level then others.
```

---
## \#5 Posted by: uigiroux Posted at: 2018-03-27T17:43:58.052Z Reads: 345

```
Lol, no you're right I didn't notice it was three of each, I thought I just saw two power in cables and I guess my mind tricked me into thinking the other side was how it should be... Weird, huh?  What the hell are they doing.... Haha I guess the three powered VESC is the next innovating in Esk8! :slight_smile:
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-03-27T18:05:55.647Z Reads: 325

```
That's single vesc with higher current I guess 300A which will require at least 3 x XT90 inputs, and 3 x 3 phase wires so it would be bit more flexible compared to 00AWG wire...
```

---
## \#7 Posted by: b264 Posted at: 2018-03-27T18:18:33.632Z Reads: 324

```
[quote="Kug3lis, post:6, topic:50345, full:true"]
That’s single vesc with higher current I guess 300A which will require at least 3 x XT90 inputs, and 3 x 3 phase wires so it would be bit more flexible compared to 00AWG wire…
[/quote]

Yes, it is a single but no way you will get 300A over those wires, so they triple them up.
```

---
## \#8 Posted by: uigiroux Posted at: 2018-03-27T18:19:06.364Z Reads: 315

```
Wow that's crazy!
```

---
## \#9 Posted by: Orin635 Posted at: 2018-03-27T18:22:37.085Z Reads: 311

```
Probalby a really stupid question. but does this mean its 1 vesc for 2 motors
```

---
## \#10 Posted by: b264 Posted at: 2018-03-27T18:23:02.677Z Reads: 305

```
[quote="uigiroux, post:8, topic:50345, full:true"]
Wow that’s crazy!
[/quote]

Innovation isn't crazy.  Patent trolling is crazy.  I welcome the innovation, if it's actually Trampa doing it.

The innovation was probably *caused* by competition
```

---
## \#11 Posted by: b264 Posted at: 2018-03-27T18:23:45.118Z Reads: 301

```
[quote="Orin635, post:9, topic:50345, full:true"]
Probalby a really stupid question. but does this mean its 1 vesc for 2 motors
[/quote]

No, not yet
```

---
## \#12 Posted by: Orin635 Posted at: 2018-03-27T18:24:25.350Z Reads: 297

```
Awh that would be really good if it was. what does dual vesc mean then
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-03-27T18:59:12.791Z Reads: 290

```
two VESC in one case ;)
```

---
## \#14 Posted by: sayekim Posted at: 2018-03-27T19:13:43.667Z Reads: 280

```
I don’t get this thing. What would you use it for and how?
```

---
## \#15 Posted by: Acido Posted at: 2018-03-27T19:17:25.417Z Reads: 280

```
shouldn't dual vesc be one controller for 2 motors? like the Chinese ones
```

---
## \#16 Posted by: Der6FingerJo Posted at: 2018-03-27T19:18:31.830Z Reads: 277

```
Electric Motorcycle or Bike for example, a VESC on those would be really nice. Though personally i'd like to run a higher voltage in this case. If you really want to push 300A the Cables will be huge.
```

---
## \#17 Posted by: sayekim Posted at: 2018-03-27T19:21:46.590Z Reads: 270

```
Obviously I’ve never looked at how motors are connected on those but why does it have 6 phase wires? Hi
```

---
## \#18 Posted by: Der6FingerJo Posted at: 2018-03-27T19:22:33.986Z Reads: 273

```
There are multiple wires per phase. It's a regular 3 Phase output, just 2 Wires for each individual phase to handle all the current.
```

---
## \#19 Posted by: scepterr Posted at: 2018-03-27T19:22:52.744Z Reads: 275

```
Could do 16S on it, very likely for a bike
```

---
## \#20 Posted by: trampa Posted at: 2018-03-27T19:55:46.878Z Reads: 275

```
It is a magnetic flux compensator prototype. At this stage it is driving multiple reving resistors (up to three simultaneously, shown two) on up to 9 phase wires from up to three individual power sources.
If you drop those motors into 2L of water, the water temperature reaches 75°C in just under 300 Seconds, hence 75/300. We use it to boil Easter eggs, which are then hidden in the source code, so everyone can enjoy an eggciting Easter weekend browsing through GitHub.

![VESC HP Proto|666x500](upload://w0gtCPulEENHGoaSKVjAx8dUDv.jpg)

For Skateboards this thing is a bit overkill. We want drop two of those into a 19**75** Mini Cooper.
We are aiming at **300**KM range. Project 75/300. Since we could not get enough batteries into the car, we will drop them onto the car. Has some similarities to our Mountainboards with strapped on Battery Box.
Unfortunately we had to strip out the 140 HP 1340CC turbo charged engine and the 5 speed straight cut racing gear box. Hopefully we will find a new cooper chassis for the motor soon.

![75_300 - Kopie|520x342](upload://uR36j2rEWhaphGYevwoyJxeidfz.jpg)
```

---
## \#21 Posted by: Sebike Posted at: 2018-03-27T20:07:41.810Z Reads: 266

```
So this could actually be used as a Trampa Sous Vide?
```

---
## \#22 Posted by: trampa Posted at: 2018-03-27T20:11:45.610Z Reads: 263

```
Maybe we should publish a book called cooking in FOC.
```

---
## \#23 Posted by: Sebike Posted at: 2018-03-27T20:21:34.039Z Reads: 258

```
as long as you don't trademark "cooking", that's fine :wink:
```

---
## \#24 Posted by: squishy654 Posted at: 2018-03-27T20:28:15.534Z Reads: 258

```
Maytech was teasing those, I wonder if they working together.
```

---
## \#25 Posted by: trampa Posted at: 2018-03-27T20:34:11.885Z Reads: 256

```
Definitely not.
```

---
## \#26 Posted by: FredrikHems Posted at: 2018-03-27T22:06:35.759Z Reads: 245

```
TrampTech :sunglasses:
```

---
## \#27 Posted by: linsus Posted at: 2018-03-27T23:11:53.308Z Reads: 244

```
haha, sorry for the teaser pic. and sorry if you had to answer unwanted dms @trampa :wink: 

Without saying too much;

Yes its at 75 volt/300A. 

No its not a multi esc. its one. If you'd consider the cable girth for 300A for a second you might add up why theres so many wires. 

The boiling motor part is true tho. (stress heat test)

I'm sure Ben will share some info about this when right time comes.
```

---
## \#28 Posted by: banjaxxed Posted at: 2018-03-28T08:10:04.227Z Reads: 226

```
On the roof? Novel but won't make it handle better! Needless to say I want one
```

---
## \#29 Posted by: ElskerShadow Posted at: 2018-03-28T08:37:48.767Z Reads: 226

```
An EV ran With 2 VESC ??? Is this forul will become electric vehicle builders in the future ?
Actualy this sound amazing.
```

---
## \#30 Posted by: Eboosted Posted at: 2018-03-28T20:32:05.614Z Reads: 215

```
I'm building a Volvo P1800 atm, let me know if this thing is available, I could be your rat lab if these VESCs are available.
```

---
## \#31 Posted by: banjaxxed Posted at: 2018-03-28T20:35:22.463Z Reads: 214

```
More space here!
![IMG_8705|640x480](upload://9vZ0kffgsSdnCNvVaQVsH9Uv2Zr.JPG)
```

---
## \#32 Posted by: b264 Posted at: 2018-03-28T20:38:23.467Z Reads: 207

```
[quote="ElskerShadow, post:29, topic:50345"]
An EV ran With 2 VESC ???
[/quote]

[Electric cars](https://gem.polaris.com/en-us/e6/specs/) drive around here and they have the power equivalent of two 6374s (3200W x 2)
```

---
## \#33 Posted by: trampa Posted at: 2018-03-29T18:53:02.032Z Reads: 192

```
Our sparky has one of those. Gray, no windows in the back. More space for batteries...

I think the Mini is a great car for e-conversions. Light, small and it comes with a gearbox that can be easily coupled with a 30KW BLDC motor. 

As soon as the 300A version is stable, we will try to organize a pre-order sale for a small batch. 

Frank
```

---
## \#34 Posted by: chuttney1 Posted at: 2018-03-29T18:58:20.264Z Reads: 186

```
I can already tell there are dedicated mosfet gate drivers per phase and not the ones coming off the DRV chip. This is not a secret because of power requirements to drive loads as high as an EV.
```

---
## \#35 Posted by: SORRENTINO Posted at: 2018-03-29T19:02:23.312Z Reads: 184

```
What anti spark switch are you using with that. Seem like its the only thing that cant be made reliable lol
```

---
## \#36 Posted by: PXSS Posted at: 2018-03-29T19:04:55.650Z Reads: 186

```
If anyone needs something this powerful, look up 300A vesc. It's made by user TechAUmNu in the fightingrobots forums and it costs just a bit more than a regular vesc 6. He's already had the first batch of preorders filled but I'm sure he'll be making more
```

---
## \#37 Posted by: Kug3lis Posted at: 2018-03-29T19:08:25.274Z Reads: 183

```
DRV has voltage limit of 60V, it's 75V version so it's bit no brainer that it will have to use separate gate drivers, plus it also has 12V rail which indicates gate drivers :P
```

---
## \#38 Posted by: Nordle Posted at: 2018-03-29T20:02:47.117Z Reads: 178

```
A relay...
```

---
## \#39 Posted by: uigiroux Posted at: 2018-03-29T20:10:33.015Z Reads: 180

```
I've been messaging him about his product.  It's the A200S 16s 200A I believe.  I think they're €400, maybe a bit more, but right around there.  They look very high quality.  I asked about dual enclosures and using them in Esk8, he said he's doing to start making dual enclosures, so that would be perfect for running something like 80100 motors at 16s, I think you can actually run up to 18s with a few mods...  Anyways,  a build using these and the motors to match would be unbeatable!
```

---
## \#40 Posted by: squishy654 Posted at: 2018-03-29T20:27:48.438Z Reads: 182

```
So instead of simply making low cost vesc's that don't fry or blow up from normal use, you decided to make something I would never need? How about just a nice cheap vesc that is robust? or how about a simple 100amp version that is bombproof?
```

---
## \#41 Posted by: Der6FingerJo Posted at: 2018-03-29T20:34:04.327Z Reads: 177

```
Just because you dont need this doesn't mean that it's unnecessary. Higher powered VESC would be awesome for a lot of people, no need to restrict VESC development to eskates anymore. I think high powered VESCs are amazing, gives you alle the telemetry features and configuration abilities for a lot of cool vehicles.

Also if you compare our VESCs to different motor control units, a FOCBox or ESCape isn't as bad price wise.
```

---
## \#42 Posted by: squishy654 Posted at: 2018-03-29T20:37:31.762Z Reads: 176

```
oh for others things sure, but I'm in the skateboard builder forums right now...and we seem to be hurting for a robust vesc solution...
```

---
## \#43 Posted by: trampa Posted at: 2018-03-30T10:28:16.285Z Reads: 165

```
25KW is overkill for skateboards, we know that. But we need to move forward and 300A @ 75V is quite nice for many other applications. This thing can be scaled up if needed. On the other hand side, 300A is already demanding quite a battery pack. 

So far test results are promising and hopefully we can start a beta-batch within the next months.
```

---
## \#44 Posted by: trampa Posted at: 2018-03-30T10:53:06.852Z Reads: 164

```
[quote="Der6FingerJo, post:41, topic:50345"]
Also if you compare our VESCs to different motor control units, a FOCBox or ESCape isn’t as bad price wise.
[/quote]

That is quite true. We had a customer who spent 3K for one motor controller, to figure out that it didn't work at all for his application. The VESC six was performing way better and cost was only a fraction. 
Price is sometimes a matter of perspective.
```

---
## \#45 Posted by: Nordle Posted at: 2018-03-30T11:00:24.963Z Reads: 166

```
My perspective is that an item should be priced on the cost of materials and the work involved. Now it‘s up to you to decide how much is your work worth. It may be worth less than what you expected to others, and the sales will be small, or it can be vice versa.
```

---
## \#46 Posted by: trampa Posted at: 2018-03-30T19:56:33.081Z Reads: 151

```
Unfortunately a business has a lot more costs to carry than your work and product cost. 

-Tax >>import tax, company tax
-cashflow and interest rates
-labour/staff, health insurances, pensions
-your own labour (taxed again)
-rent for warehouse
-website and web service
-packaging
-shipping
-product returns
-insurance
-legal advice
-accountant
-computers/IT/Software
-R&D
-advertising
-traveling/flights
-Car, fuel, insurance, repairs
-furniture
-tools and moulds, machines
-carrying stock (cash you can't use to do something else with it)
-RISK. Eg a hole batch can go wrong over a silly detail.
- customer support and service
- cost for shipping of replacements (customer usually sits in New Zealand)
- etc. etc.

In the end of the year you need to have a positive balance or you don't have a profitable business. 
Most business starters forget the majority of the real costs involved running a business. Especially in the beginning you need to grow your business and without profits you can't. Without profits you can't hire someone, nor rent an office or travel to see your suppliers or simply buy stock, so that you can supply your customers in a timely manner. You can't invest into new products everyone wants you to put into production and in consequence you can't sustain what you have started. 

Product prices should reflect the entire costs you have, running and growing your business. 
The gap between product cost and sales price highly depends on the branch and annual turnover. In the e-skate industrie no one turns over millions of the same product. It's not a high volume, low profit market like consumer electronics and other consumer level products that are sold by the millions. People easily forget that when they compare prices.

Most profits you make selling a product don't end in your own pocket at the end of the year, especially not if you are a small or medium sized company offering a customer service, warranty and product support.
```

---

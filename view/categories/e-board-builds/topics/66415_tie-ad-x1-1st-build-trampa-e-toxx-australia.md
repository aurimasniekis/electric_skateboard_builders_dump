# TIE/ad x1 &#124; 1st Build Trampa E-toxx (Australia)

### Replies: 209 Views: 4176

## \#1 Posted by: malJohann Posted at: 2018-08-28T22:50:42.511Z Reads: 393

```
Hi All, stoked to be here. I started my esk8 journey on an Evolve BGT, but soon realised that I wanted more.

Sold the BGT to fund this here build, so I’ll be bipedal for a while. On to greater things!

Current build list, (street use):
Trampa 35* HolyPro 16 ply deck
12mm Vertigo hollow axle trucks
Superstar wheels with 6.5” Urban Treads
Ratchet bindings (possibly with heel straps)
E-toxx Mini Dual Direct Drive (straight cut gears)
E-toxx bumper x 2
Alien APS 6384S 170KV motor x 2
HobbyWing Ezrun Max6 ESC x 2
Turnigy Nanotech 5,000mah 6S 45~90C
No BMS, using balance charger (recommendations?)
FlySky GT2B Transmitter with Mad Munky mod
10ga wiring to put it all together, probably Nomex sleeved

I’m planning to have the ESCs and battery at the front to compensate somewhat for drivetrain weight at the back.

Any thoughts and recommendations are welcome, especially around my No BMS plans. I’d like to keep this build as light and clean as possible.
```

---
## \#2 Posted by: malJohann Posted at: 2018-09-01T13:06:36.467Z Reads: 339

```
Ordered the Trampa with Vertigos, E-toxx parts, plus an extra Trampa Infinity shipped to @Nowind for machining, as well as the Max6 ESCs, GT2B and wiring I think I need.

Decided to go for 2x Turnigy Graphene 6,000mAh 4S 65~130C batteries instead, which left me wondering which balance charger to get? A Turnigy Reaktor? Which one? Something else?
```

---
## \#3 Posted by: Andy87 Posted at: 2018-09-01T13:25:28.119Z Reads: 338

```
There are a lot of chargers outside.
Depends on how much money you want to spend, how fast you want to charge and if you want to charge more than one pack at the same time. Don’t forget that for the hk Reaktor you need a separate power supply unit too. Just that add some money on top too.
If you look for a cheap and easy but good charger than go with the I charger b6. They about 30-35€. There a AC version which has a power supply inside, or the version with external laptop brick. You can balance charge up to 6s and max 5a.
```

---
## \#4 Posted by: malJohann Posted at: 2018-09-01T13:57:36.173Z Reads: 318

```
Would this be overkill? What’s mid-range?

https://www.icharger.co.nz/icharger-308-duo
```

---
## \#5 Posted by: Nowind Posted at: 2018-09-01T15:01:58.001Z Reads: 293

```
I have a Junsi 4010DUO, using it since years.... choosed the 10S one because i got many 10S Bricks from the E-Drift-Trikes... the junsi is pricey but you get 1A hardware IMO.
Dont forget that you need also a good power adapter, for full performance 24V output.
I love my junsi but they are also many cheaper options ....
```

---
## \#6 Posted by: Spatt Posted at: 2018-09-01T15:44:17.837Z Reads: 294

```
so you are going to assemble a 12s2p lipo battery with 10000 mah and 50.4 volts right?so x4 lipo 6s or just 2 lipo so 12s 5000 mah? mmmmh if you don't have a lipo charger maybe it should be cheaper and more reliable to use a bms charge only, there are a tons of charger and with something like 60/80 dollars maybe less you will buy a good quality 12s bms and a good quality charger... a bms charge only is like 40/50 grams maybe. Also if you save money on charger for lipo you can invest in a vesc 6/escape/focbox unity/focbox cooled or something that can handle a lot of amps if you like the power!! but on the street so much power maybe it's an overkill. and also another thing, if you have foot straps you will mount your battery case in the middle of the board or under like a urban carver... and escs must be rear positioned since you can't make motor cables too long this is important!
```

---
## \#7 Posted by: malJohann Posted at: 2018-09-01T18:24:03.405Z Reads: 274

```
I’m still brand new at this, but thinking 8S1P actually. Already bought 2x Max6 ESCs.
```

---
## \#8 Posted by: Spatt Posted at: 2018-09-01T19:08:56.368Z Reads: 287

```
Welcome :smile:  You should make a research on kv of the motors and how combine the kv to the voltage of the battery, and the erpm limit.
If you choose a 8s with a 170 kv motor you will have a very high torque but a very low maximum  speed, so it depends on what you want! Make a check with esk8calc...
IMO The battery you choose it’s not correct.
 graphene are really expensive because of their performance but for your first build maybe you need not so much amps, and very low capacity, it means less time of fun! 
That battery is rated for 65 C, 65x6= 390 amps constant ahhaha it’s way exagerate for a dual drive! And it’s a sacrifice of capacity 
I don’,t know very well the esc you choose but someone on the forum is using that...
```

---
## \#9 Posted by: Andy87 Posted at: 2018-09-01T19:50:31.739Z Reads: 291

```
Actually it’s not totally right...😬
The C-rating is not a standard and the formula c*capasity= const current is what people say but in real live situation more or less only half of what would be the calculation. There is a device with which you can measure the real constant amps your battery can handle, it’s this device
https://hobbyking.com/en_us/wayne-giles-designed-universal-esr-meter-for-100-10000mah-1-6-cell-lipo.html

In my opinion it’s never bad to investigate in good batteries. @malJohann The graphen lipos shown to be reliable and stable also after many charging cycles. The higher C the less voltage sag you get. This results in better performance and longer range in the end. Less stress for the battery means your lipos will last longer.
For a MTB I wouldn’t go under 60c 5ah, especially if you go low voltage like 6-8s as with it you usually need more amps out of your pack to get the same performance like you would get with a 10-12s.
```

---
## \#10 Posted by: davewood1982 Posted at: 2018-09-01T22:06:58.557Z Reads: 270

```
i run a  mtb 8S1P setup using 2x 4s graphenes with Max6 ESCs. There brilliant batteries, zero voltage sag and i get 6/8 miles range  on 8inch AT wheels
```

---
## \#11 Posted by: malJohann Posted at: 2018-09-01T22:11:35.175Z Reads: 262

```
That’s what I thought I’d do. 2x 4S Graphene batteries. I’m not a range junkie either.
```

---
## \#12 Posted by: davewood1982 Posted at: 2018-09-01T22:36:27.237Z Reads: 255

```
could always get another 2 if you wanted more range aswell..  performance wise though their excellent and the Max6 ESCs are bulletproof! As for a charger? i just use 2 imax b6ac chargers (around £20each),  1 charger charging  each battery for a faster charge, takes around 2hrs at max charge rate.
```

---
## \#13 Posted by: malJohann Posted at: 2018-09-01T23:28:00.146Z Reads: 253

```
Do the b6ac chargers need a power source?
```

---
## \#14 Posted by: davewood1982 Posted at: 2018-09-02T00:57:08.587Z Reads: 239

```
no, Its  already built in on the b6ac model.
```

---
## \#15 Posted by: malJohann Posted at: 2018-09-02T04:15:56.137Z Reads: 237

```
@Nowind would I be able to run 200kV motors to their full performance on 8S 65~130C batteries?
```

---
## \#16 Posted by: malJohann Posted at: 2018-09-02T22:33:53.881Z Reads: 235

```
Also, what connectors and wires do I need to buy between XT90 battery and Max6 ESC, and between Max6 ESC and APS 6384 motors?
```

---
## \#17 Posted by: malJohann Posted at: 2018-09-03T07:41:32.616Z Reads: 239

```
Bought 2x B6AC chargers today, a BatSafe charging box, Freebord S2 bindings, and a @MasterCho ChoZen GT2B mod.

Need to buy motors next, that and maybe some electrical connectors are the only things outstanding (boy that escalated quickly).

If anyone can answer the questions above, that would be much appreciated.
```

---
## \#18 Posted by: Andy87 Posted at: 2018-09-03T07:51:58.581Z Reads: 248

```
I don´t own a Max6 esc but this is what I found on the first google search result
•Steckersystem Akku: T-Stecker / Dean
•Buchsensystem Motor: 6,5mm Goldkontakt

Yes it´s German ;) But I guess you get it.
The input wires I just would cut the plug and solder a xt90 anti spark on it. Most easy way as your batteries have xt90 too.
The APS motors coming with a 5.5mm bullet connector.
So I guess you need some 6.5mm male bullet connectors and change them on your APS motors (or make an adapter 6.6 to 5.5)
```

---
## \#19 Posted by: malJohann Posted at: 2018-09-03T08:11:17.859Z Reads: 241

```
It’s the APS and the Max6 input end I couldn’t find. Thanks mate!
```

---
## \#20 Posted by: Andy87 Posted at: 2018-09-03T08:11:54.636Z Reads: 240

```
Welcome and good luck! 👍
```

---
## \#21 Posted by: Nowind Posted at: 2018-09-03T15:39:43.250Z Reads: 237

```
[quote="malJohann, post:15, topic:66415"]
would I be able to run 200kV motors to their full performance on 8S 65~130C batteries?
[/quote]


200kv works good with max6, 170kv is an option too!

[quote="malJohann, post:19, topic:66415"]
It’s the APS and the Max6 input end I couldn’t find.
[/quote]


Max6 is 6.5mm
https://www.ebay.de/itm/Goldkontakt-Verbinder-Heavy-Duty-Stecker-Buchse-6-5-mm-10-Paar-partCore-100223/141573500081?epid=1837720720&hash=item20f6702cb1:g:vVYAAOSwEwZbPxYG

Castle Creations also have them for a bit more dollars
```

---
## \#22 Posted by: malJohann Posted at: 2018-09-04T04:41:50.868Z Reads: 230

```
Ordered an E-toxx Max6 CF mounting bracket and an Osprey Kamber 22 earlier today, got back to my desk after a meeting to find this!

![image|375x500](upload://hx5VoQHqGwhB8hHnz9nM1D0BOQj.jpeg)
```

---
## \#23 Posted by: davewood1982 Posted at: 2018-09-04T13:05:28.747Z Reads: 215

```
dont forget to get a programming card with them Max6's so you can adjust settings
```

---
## \#24 Posted by: malJohann Posted at: 2018-09-04T21:16:36.188Z Reads: 214

```
Was thinking of this last night, so I ordered the HW WiFi Express card and downloaded the iOS app. Also, this morning after confirming stock, I placed the order for the APS6384 200kV motors.
```

---
## \#25 Posted by: malJohann Posted at: 2018-09-05T00:15:10.744Z Reads: 223

```
Chargers have arrived. Pretty much going to feel like my birthday for the next two weeks or so.

![image|375x500](upload://tOqOarlSrwXq11cKtMlUAB8TrUx.jpeg)
```

---
## \#26 Posted by: malJohann Posted at: 2018-09-06T09:49:19.141Z Reads: 213

```
So today was big delivery day, three packages arrived all at once. I now have most of the electrical stuff, just need a couple more connectors, and some soldering consumables. Also, motors, let’s not forget those!

![image|375x500](upload://wphDBuAJewVWeV0V2TN5iAoHczw.jpeg)
```

---
## \#27 Posted by: malJohann Posted at: 2018-09-06T09:51:05.733Z Reads: 205

```
Plus, I have tracking numbers for the Trampa and E-toxx stuff.
```

---
## \#28 Posted by: Andy87 Posted at: 2018-09-06T09:51:58.218Z Reads: 196

```
looks like soon you will be quite busy ;)
```

---
## \#29 Posted by: malJohann Posted at: 2018-09-06T10:28:01.896Z Reads: 194

```
Can’t wait! How much W fuse should I get for this?
```

---
## \#30 Posted by: Andy87 Posted at: 2018-09-06T10:41:42.798Z Reads: 203

```
you will run 12s right?
Take a 58V fuse
Something like this
https://www.amazon.de/Leistungssicherung-Streifensicherung-Sicherung-Midi-weiss/dp/B00EBNRXRK/ref=sr_1_fkmr0_2?ie=UTF8&qid=1536230433&sr=8-2-fkmr0&keywords=58V+fuse

depending on how hard you wanna go, between 60-100A should be fine
```

---
## \#31 Posted by: malJohann Posted at: 2018-09-06T11:15:27.175Z Reads: 196

```
8S actually.
```

---
## \#32 Posted by: Andy87 Posted at: 2018-09-06T11:17:42.694Z Reads: 188

```
ah ok, sorry.
Than you can go with a normal 36V car fuse too.
the amps I would stay the same like with 58V
```

---
## \#33 Posted by: davewood1982 Posted at: 2018-09-06T11:45:39.726Z Reads: 185

```
he doesn't need any fuse or anti spark because the max6 esc already have them built in.
```

---
## \#34 Posted by: Andy87 Posted at: 2018-09-06T12:16:15.522Z Reads: 186

```
Didn´t know about it as I don´t own a max6.
That´s good. Which fuse is build inside?
```

---
## \#35 Posted by: malJohann Posted at: 2018-09-06T12:42:26.848Z Reads: 192

```
That’s awesome! Didn’t know.
```

---
## \#36 Posted by: davewood1982 Posted at: 2018-09-06T13:03:21.660Z Reads: 201

```
No idea about which fuse! but i pulled this from the hobbywing website itself , iv been using them without any  fuses or anti spark systems  for over a year now with zero problems.

![capture-20180906-135508|690x364](upload://3Yle7aP0nRNDOsiQ1dBDz1vpf7C.jpg)
```

---
## \#37 Posted by: Andy87 Posted at: 2018-09-06T13:07:45.163Z Reads: 195

```
But it’s only anti spark, nothing written about a fuse. As min not in the picture you posted.
Fuse should save you from short the battery or the esc. The antispark just kills the spark which can appear while connecting a battery to the esc.
```

---
## \#38 Posted by: davewood1982 Posted at: 2018-09-06T13:35:16.964Z Reads: 192

```
the system as stated protects both battery and esc, you literally can't have a functional ' anti spark system' without  some kind of fuse component or something that does a similar job of a fuse, as iv said, iv literally been using these escs as standard without any problems for over a year.
```

---
## \#39 Posted by: Andy87 Posted at: 2018-09-06T14:27:33.066Z Reads: 190

```
I thought there is just a precharge resistor inside🤔
I once shorted my battery with a anti spark loop key, so can you explain me why there the fuse inside the antispark plug didn’t triggered?
I‘m not a electrotechnical expert, so I just want to understand this.
```

---
## \#40 Posted by: davewood1982 Posted at: 2018-09-06T15:48:50.989Z Reads: 187

```
The switches ( similar to what the max6 uses) are obviously a lot more advanced than a loop key hence why the Vedder Anti-Spark switches are very expensive. Im sure theres a thread about the differences between the 2.
```

---
## \#41 Posted by: Andy87 Posted at: 2018-09-06T16:07:59.520Z Reads: 194

```
The vedder switch based on mosfets.
All this anti spark e-switched have a fuse in line or as min a holder for it. The vedder anti spark don’t replace a fuse. 
https://www.electric-skateboard.builders/t/vedder-anti-spark-switch-v1-3-kit-currently-out-of-stock/9949?u=andy87

If the mosfet blow than usually there gates stay open and your board always switched on. 
Still don’t get the argument why not to use a fuse?

A fuse should save your components from getting broke by burn before your esc or battery burn.
Did you burn one of that fuses in your max6?
And if yes how you can replace it?
If you can’t replace it than your max6 is fucked non the less, so a external fuse would solve that problem.

If i‘m wrong please put me in the right direction!
```

---
## \#43 Posted by: malJohann Posted at: 2018-09-07T01:24:51.839Z Reads: 185

```
Trampa board arrived early!

![image|375x500](upload://iir8qm4oes9R1F5uF8svKG9eCBM.jpeg)
```

---
## \#44 Posted by: malJohann Posted at: 2018-09-07T03:30:01.783Z Reads: 175

```
@DanSkates any input you may have would be welcome too, since you built a board very similar to this.
```

---
## \#45 Posted by: malJohann Posted at: 2018-09-07T04:30:57.215Z Reads: 173

```
Also need advice on soldering 10 ga wire.
```

---
## \#46 Posted by: Andy87 Posted at: 2018-09-07T04:44:14.740Z Reads: 178

```
What you want to know about it?
Just first dip the 10awg in solder than fill up the xt plug with solder, heat up everything together again and put things together.

If you think you have a problem that the 10awg will splice up, you can use a small thin copper wire or one braid of a spare awg peace. Than twist it around the end to tighten up all braids of your 10awg than proceed like described before.

I soldered 8awg easy to a xt90 like this.
Hope you understood my explanation 😅 it’s easy but with my English not so easy to explain...
```

---
## \#47 Posted by: malJohann Posted at: 2018-09-07T04:54:12.119Z Reads: 180

```
I’ve got a 30W soldering iron with temperature control. Is that enough power? Guessing not.

Which would be a good, but not priced over the top soldering iron/station if the above is true?

What kind of solder do I use? Is rosin based flux paste good? It’s what I have.
```

---
## \#48 Posted by: Andy87 Posted at: 2018-09-07T05:03:53.723Z Reads: 186

```
Get something like this with 60-100w
https://www.amazon.com/Choice-CH-IRON-100W-soldering/dp/B00XK5RXKC

it’s massive but for wires or nickel it does a very good job.
Use a 60/40 solder (more easy if it’s not lead free). Eboosted recommended 63/37 for nickel, but I never tried so far.

About flux, just look what’s written on what you already have, doesn’t matter if it’s paste or liquid. I just asked in my local electric shop about the right flux for connecting copper.
```

---
## \#49 Posted by: baxter Posted at: 2018-09-07T05:49:02.726Z Reads: 190

```
Not sure if you already have something like this but “Helping Hands” come in really handy holding wires an connectors steady for soldering.

https://hobbyking.com/en_us/hands-free-small-item-holder.html
```

---
## \#50 Posted by: malJohann Posted at: 2018-09-07T11:03:46.644Z Reads: 192

```
Took my Trampa out of the box, and everything is tops, except for this one gash in the front on top. @trampa like someone was negligent with a drill or something. Also shipped minus 8 M5 washers.

![image|375x500](upload://zRPXyhOJhlheoYV3YErUM46VBc8.jpeg)
```

---
## \#51 Posted by: Andy87 Posted at: 2018-09-07T12:02:27.331Z Reads: 191

```
Good place to drill a hole and mount a voltmeter 😉
```

---
## \#52 Posted by: malJohann Posted at: 2018-09-07T12:52:29.114Z Reads: 192

```
Positive take on it for sure, I’m a little disappointed, but it’s not the end of the world. More pissed that I couldn’t finish assembling tonight because none of my M5 washers for the trucks were in the package. Have to source those locally now, and not sure they’ll be “marine grade”.
```

---
## \#53 Posted by: Kug3lis Posted at: 2018-09-07T13:01:45.382Z Reads: 187

```
Be careful with APS 6384 200kV both of them got loose magnets within a 2 weeks... Now riding with my own glued magnets...
```

---
## \#54 Posted by: Kug3lis Posted at: 2018-09-07T13:04:43.415Z Reads: 185

```
[quote="malJohann, post:52, topic:66415"]
and not sure they’ll be “marine grade”
[/quote]

Haha, I bought some simple a2 stainless steel (not A4) washers and they didn't bent like trampa ones when tightening :D
```

---
## \#55 Posted by: trampa Posted at: 2018-09-07T13:14:43.398Z Reads: 179

```
Looks like it has been damaged during transportation. Was there something else in the Box, how did the Box look like? Technically that is no issue, its just an optical damage. Do you plan to mount something on the Tip?
Frank
```

---
## \#56 Posted by: malJohann Posted at: 2018-09-07T20:08:07.780Z Reads: 183

```
Should I take them apart and do preventative upgrades before using them?
```

---
## \#57 Posted by: malJohann Posted at: 2018-09-07T20:11:56.949Z Reads: 191

```
It was a complete MTB so many other things in the box, but as mentioned it’s okay.
```

---
## \#58 Posted by: malJohann Posted at: 2018-09-08T00:46:00.950Z Reads: 194

```
Marine grade hardware and compact tool problem solved!

![image|666x500](upload://9d8LBAUWpg7UWrum0aBfC6muBLx.jpeg)
```

---
## \#59 Posted by: malJohann Posted at: 2018-09-08T04:32:44.501Z Reads: 197

```
![image|666x500](upload://cxCqUWnlVFEGFvOPVtGmrlpO1zO.jpeg)
![image|666x500](upload://ezKAm7RfFFHJYZbudeUXvbN3Mba.jpeg)
```

---
## \#60 Posted by: malJohann Posted at: 2018-09-08T11:23:22.721Z Reads: 194

```
@trampa what are the four orings in the kit for?
```

---
## \#61 Posted by: FredrikHems Posted at: 2018-09-08T11:48:49.572Z Reads: 194

```
They are meant to go between the outer bearing in the hub and the metal spacer. This way you can tighten the axle nut down hard, without the bearings getting jammed :wink:
```

---
## \#62 Posted by: malJohann Posted at: 2018-09-08T12:17:34.513Z Reads: 182

```
Interesting. Mine came without assembly instructions, so kinda had to figure it out with outdated schematics on the internet.
```

---
## \#63 Posted by: malJohann Posted at: 2018-09-08T22:21:04.985Z Reads: 180

```
How much Amps will my system draw Const/Max? Essentially I want to know if I can use 45A Anderson Connectors instead of XT90.
```

---
## \#64 Posted by: malJohann Posted at: 2018-09-10T01:41:20.123Z Reads: 172

```
Anyone? I need advice, I’m no electrician. @rojitor maybe you can tell me about the Anderson Power Pole connectors?
```

---
## \#65 Posted by: Sourcecode Posted at: 2018-09-10T02:05:12.827Z Reads: 168

```
My trampa goes well over 45amps especially up hill
```

---
## \#66 Posted by: Andy87 Posted at: 2018-09-10T06:00:34.567Z Reads: 170

```
you could use them as connector on the VESCs but as battery connector, better stay with the xt90s.

45A is easy to reach offroad or on a hill
```

---
## \#67 Posted by: malJohann Posted at: 2018-09-10T06:23:39.250Z Reads: 177

```
Celebrate every arrival LOL! 😂

![image|666x500](upload://2EI3rX4v0YZsUPjw7bksSOmEs5S.jpeg)
```

---
## \#68 Posted by: Trdolan03 Posted at: 2018-09-10T06:29:20.964Z Reads: 177

```
Does anyone use xt60 for mtb?
```

---
## \#69 Posted by: malJohann Posted at: 2018-09-10T06:39:58.055Z Reads: 170

```
Now that I’ve done a bit more research I wouldn’t think so, can only handle 60A constant draw.
```

---
## \#70 Posted by: Trdolan03 Posted at: 2018-09-10T06:41:31.895Z Reads: 166

```
But we don’t draw anywhere near that constantly
```

---
## \#71 Posted by: malJohann Posted at: 2018-09-10T06:47:03.482Z Reads: 166

```
Depends how hilly your area is? There must be a reason my 65~130C batteries came with XT90 out of the box.
```

---
## \#72 Posted by: Andy87 Posted at: 2018-09-10T07:13:37.391Z Reads: 164

```
there is no xt60 anti spark plug.
one more reason.
With wires and connectors you can never by too big.
if you have the space for xt90 than use it.
probably it would work too, but it´s not so nice to solder 10awg wires on a xt60 too.
```

---
## \#73 Posted by: Kug3lis Posted at: 2018-09-10T08:02:25.096Z Reads: 166

```
Well I am running 90A mot/batt and using MT60 for phase connectors, after some hard pushing those connectors don't even come warm so I guess they are more than enough for esk8 loads :)
```

---
## \#74 Posted by: malJohann Posted at: 2018-09-10T08:55:34.744Z Reads: 165

```
Is there any reason that I can’t put my batteries and ESCs at the front truck? I’d like to balance my build weight wise and visually.
```

---
## \#75 Posted by: Andy87 Posted at: 2018-09-10T09:00:46.517Z Reads: 164

```
I like my xt90 connectors...they easy to solder as well...8AWG or twice 10AWG no problem... why to make the life more complicated ;)
```

---
## \#76 Posted by: Kug3lis Posted at: 2018-09-10T09:37:47.412Z Reads: 166

```
I meant I use xt90 for power too, just motor instead of bullets I use MT60 not XT60
```

---
## \#77 Posted by: Andy87 Posted at: 2018-09-10T09:55:56.023Z Reads: 166

```
how you got the motor wires in the right order by the first time?
just luck, or there is a easy way to test it out. Like that MT60 design, but don´t like that you can´t swap the phase wires if they wrong
```

---
## \#78 Posted by: Kug3lis Posted at: 2018-09-10T09:59:42.808Z Reads: 158

```
Well motor wire phases order doesn't matter ESC will pick it up. Worst case scenario you will need to change direction under general tab
```

---
## \#79 Posted by: Cobber Posted at: 2018-09-10T10:15:57.040Z Reads: 163

```
[quote="malJohann, post:74, topic:66415"]
Is there any reason that I can’t put my batteries and ESCs at the front truck?
[/quote]

The longer your battery-esc wires the more (bigger) induction induced spikes your esc will be exposed to.
```

---
## \#80 Posted by: rich Posted at: 2018-09-10T10:16:30.034Z Reads: 169

```
[quote="malJohann, post:74, topic:66415, full:true"]
Is there any reason that I can’t put my batteries and ESCs at the front truck? I’d like to balance my build weight wise and visually.
[/quote]

Do you mean on the front top of the deck?
That would mean endless phase wires, I had 85cm with ESC's in the middle, that worked.

I like the idea of placing the ESC's next to the battery so you don't need extra caps but I recommend mounting everything in the middle of the board, especially when you use bindings.

The whole weight of your drivetrain and motors are on the rear truck and not on the rear of the deck.  If you put weight on the tip of your deck the riding experience will be strange IMO. Middle position on the the deck is best for riding but carrying is a different thing :wink:
```

---
## \#82 Posted by: davewood1982 Posted at: 2018-09-10T10:25:13.615Z Reads: 161

```
Motor direction isn’t a big deal, even if you connected it up and the motors spun the wrong way there’s a setting on the max6 where you can change which direction they spin (either clockwise or anti clockwise). And as others have advised its not recommended to have too long phase wires so ideally you wanna keep the Escs on the back.
```

---
## \#83 Posted by: rojitor Posted at: 2018-09-10T15:36:28.602Z Reads: 169

```
I do not recommend you Anderson pp45 for that. They can deal with more than 45 amps but they can move slightly due to vibrations.
If one of them gets out a couple mm they will arc and burn unless you put them together firmly.
I usually shrink them
Powerpole 75 will not move at all and they resist way beyond 100 amps. They are rather Big though. I'd stick to xt90's for esk8.
![f44sj6|640x480](upload://rO1lSosZvFbUcHqo2xdJBsDul8x.jpg)
Here you can see 45 and 75. The size difference is noticeable
```

---
## \#84 Posted by: malJohann Posted at: 2018-09-11T10:51:32.904Z Reads: 161

```
Decided to go with Turnigy SK3 6374 192kV motors instead of the APS units.
```

---
## \#85 Posted by: Andy87 Posted at: 2018-09-11T10:56:58.169Z Reads: 160

```
make sure that your pulleys also fit to it.
APS has 10mm shaft, SK3 has 8mm shaft
```

---
## \#86 Posted by: malJohann Posted at: 2018-09-11T11:37:33.677Z Reads: 159

```
Already let Jens know I’ll be ordering 8mm motorspurs from him too.
```

---
## \#87 Posted by: malJohann Posted at: 2018-09-11T21:55:29.273Z Reads: 170

```
Feels like I’ve been chozen. :scream: @MasterCho 

![image|375x500](upload://2hy3qQ02aIoDVOU2ppvZSSiVbsX.jpeg)
```

---
## \#88 Posted by: malJohann Posted at: 2018-09-11T22:27:45.772Z Reads: 164

```
What size heat shrink tubing and wire mesh wrap should I get for the battery side and motor side of the ESC? Also, do I need a heat gun to shrink the tubing?
```

---
## \#89 Posted by: malJohann Posted at: 2018-09-12T22:15:51.199Z Reads: 161

```
Ordered the SK3 6374 192kV motors, MT60 connectors, and other consumables. Did quite a bit of research on soldering, and ordered a Miniware TS100 with an additional bigger tip, and Turnigy Graphene 1,500mAh 6S 65~130C battery for soldering. This is going to be my only soldering solution for now, bench and mobile if needed.
```

---
## \#90 Posted by: Andy87 Posted at: 2018-09-13T12:53:49.776Z Reads: 161

```
Yes sure you need to heat up the head shrink 😅
But you can use everything which makes things hot. Hair dryer or a light or the tip of your solder iron (don’t touch just hold close) should work fine.
About the wire mesh... it depends if you want to cover them all single or all in one tube.

Edit: I used 10mm for one motor wire. But I think you can get there two or even 3 motor wires inside. (3 would be tight thou)
```

---
## \#91 Posted by: malJohann Posted at: 2018-09-13T13:55:11.154Z Reads: 156

```
Thanks for the tips mate.
```

---
## \#92 Posted by: malJohann Posted at: 2018-09-14T00:44:08.768Z Reads: 167

```
Costs are mounting, it’s all the little consumables and tools you don’t have when starting your first build that pushes it above expected.

Looks like it’ll be around $3,700AUD / $2,660USD for the eATB only, and about $4,520AUD / $3,250USD with all the extras included.
```

---
## \#93 Posted by: malJohann Posted at: 2018-09-17T04:58:43.973Z Reads: 169

```
Soldering iron and supplies, and the same backpack LaCroix Boards use, the Osprey Kamber 22, has arrived.

![image|375x500](upload://olUef7yYrPpgUXXrFc1vQw3CLv8.jpeg)![image|375x500](upload://necJGA85NhAdeCTzxo5ltJarYZH.jpeg)
```

---
## \#94 Posted by: malJohann Posted at: 2018-09-17T05:06:20.511Z Reads: 154

```
I’m also seriously thinking of building and coding a PWM Controller for use with the Max6 ESC.
```

---
## \#95 Posted by: Andy87 Posted at: 2018-09-17T05:14:42.438Z Reads: 154

```
Yeah that’s sadly the hidden costs that nobody calculate 😅
```

---
## \#96 Posted by: malJohann Posted at: 2018-09-17T06:02:50.095Z Reads: 162

```
Seems the delivery day wasn’t over yet. 😂

![image|375x500](upload://mPVR9NpvZFKsPdUA4ze3g1i0UTz.jpeg)
```

---
## \#97 Posted by: malJohann Posted at: 2018-09-18T23:23:27.584Z Reads: 163

```
Decided to name my build “TIE/ad x1”, which is the TIE fighter model that Darth Vader flew. Why a TIE fighter? Well, I’ll be commuting on it, and flying in between the tie clad masses. 😂

/edit also helped that TIE stands for Twin Ion Engine, and this is a twin engine build.
```

---
## \#98 Posted by: malJohann Posted at: 2018-09-19T01:56:36.534Z Reads: 167

```
Big package day! This is what happens when you take one day leave. Deliveries!

Now I’m just waiting on the 8mm motorspurs from @Nowind and then I should have everything! I’ll start building though.

![image|375x500](upload://bUb7wre13DZwAtzxxRynm8ZcCQP.jpeg)
```

---
## \#99 Posted by: malJohann Posted at: 2018-09-19T10:16:14.726Z Reads: 167

```
Yes kids, I got it in raw finish.

![image|666x500](upload://aBzcz3pK9ijHjCHxbV83QilzXw4.jpeg)
```

---
## \#100 Posted by: Andy87 Posted at: 2018-09-19T10:19:02.414Z Reads: 163

```
sent it directly to me...I know you don´t need it... :joy::joy::joy:
looks good!
interested how it will look all mounted
```

---
## \#101 Posted by: malJohann Posted at: 2018-09-20T05:55:53.446Z Reads: 162

```
You beauty! 8mm motorspurs arrived today, only one day after the big e-toxx shipment!

![image|375x500](upload://jEkm1LmUGIVJGgQpuKH89enkcls.jpeg)
```

---
## \#102 Posted by: malJohann Posted at: 2018-09-20T12:47:04.544Z Reads: 167

```
Test fit without motors, since I need to figure this out first, and then get 3mm keyways cut into the shafts. Basically replaced the front red Dampas with green ones, and built the machined Infinity hanger onto the Vertigo baseplate with DD attached.

![image|375x500](upload://yovp1edSRl7FtmQlK5b1t7TiFi8.jpeg)
![image|375x500](upload://2Y4mWOjlDIMoToFCgnjfuETKMQm.jpeg)
![image|375x500](upload://ArDgPYYPyEpTgjtgZ36pl2lnn9u.jpeg)
![image|375x500](upload://l3IDdNSmrUcHeTBtt96erhqHK0T.jpeg)
![image|375x500](upload://wo9DNbWLHowDMuQUGhSEfk39REK.jpeg) 
![image|375x500](upload://gaU7HVpVlbdnErARLPwnhjccbuj.jpeg)
```

---
## \#103 Posted by: ArnhemAnt Posted at: 2018-09-21T03:54:49.480Z Reads: 162

```
Make sure you remember to use LocTite on all those screws on the DD and also get some SuGru to fill in the void, just like on the video that @Nowind posted on his website. 
I woke with a fright last night as I remembered about the SuGru - I had forgotten to use it. Stripped it down today and added it. Luckily, there wasn't a great deal of crap in the housing. I'm also using a "Berulub" grease on the gears and so far, it looks to be working very well. Still a little noisy, but nowhere near as loud as some of the others I have heard.
```

---
## \#104 Posted by: malJohann Posted at: 2018-09-21T04:00:57.449Z Reads: 156

```
Thanks mate, I have sugru, but Jens also sent me some. Also have various grades of loctite. Still need to get lube though.
```

---
## \#105 Posted by: malJohann Posted at: 2018-09-21T13:40:25.164Z Reads: 164

```
What do you get when you have 32 screws for the gear boxes only, and you add a perfectionist? Two hours, that’s what you get.

![image|375x500](upload://opK1BVjiyB8Jhh29VYmd41v7jSF.jpeg)
```

---
## \#106 Posted by: ArnhemAnt Posted at: 2018-09-21T21:14:59.246Z Reads: 161

```
Lookin' good man. Nice and shiny.
```

---
## \#107 Posted by: malJohann Posted at: 2018-09-23T23:53:43.262Z Reads: 162

```
Only two more things I’m waiting on, a waterproof RX box, and a JR Y-connector. I’m building in the meantime though, mounted the CF ESC/RX plate last night. Also got these when I got in the office today, now I can strip and do a final assembly on the gearboxes.

![image|375x500](upload://2bnE6k3m5YEpPBd2xyNjSVmSIas.jpeg)
```

---
## \#108 Posted by: malJohann Posted at: 2018-09-24T03:48:48.653Z Reads: 162

```
#lazytosoldersmallconnectors

![image|375x500](upload://iyomVIn2OP4BAEmdff5N62Tq8Xc.jpeg)
```

---
## \#109 Posted by: mmaner Posted at: 2018-09-24T03:53:29.234Z Reads: 154

```
I feel ya.  I spent 3 hours today soldering connectors for volt meters, poer switch, charge ports, receivers, etc. Tedious mess 😀
```

---
## \#110 Posted by: malJohann Posted at: 2018-09-24T04:29:12.666Z Reads: 151

```
This way I have only 16 joints to solder, all either 10awg or 12awg (also bought pre-made XT90 series and parralel connectors for between battery and ESCs), since it’ll only be the ESC power wires, and the motor and ESC balance wires to solder.
```

---
## \#111 Posted by: Andy87 Posted at: 2018-09-24T04:48:38.991Z Reads: 151

```
Lazy always good 😜
But don’t forget to cut the 5V wire on one side 😉
```

---
## \#112 Posted by: malJohann Posted at: 2018-09-24T05:01:41.506Z Reads: 149

```
This I know, been getting advice from @Nowind on the side too.
```

---
## \#113 Posted by: malJohann Posted at: 2018-09-24T05:02:57.956Z Reads: 154

```
If I can rebuild the drivetrain tonight and the soldering done tomorrow, no reason why I can’t be riding by Wednesday morning, even drilled the M3 set-screw holes on the motor shafts this weekend.
```

---
## \#114 Posted by: malJohann Posted at: 2018-09-25T02:27:00.755Z Reads: 149

```
Did the motorspur loctite job last night, took about an hour to disassemble/do/pack up, dunno if I’m just slow. That’s also about all the time I can spend per day max, so thinking my Wednesday morning estimate might be slightly optimistic.
```

---
## \#115 Posted by: ArnhemAnt Posted at: 2018-09-25T20:45:54.760Z Reads: 142

```
LOL. I've been building my board for the last 9 months. Finally got it all together and working, only to find I have a cell in my pack that has failed. Back to the waiting game again.....
```

---
## \#116 Posted by: ArnhemAnt Posted at: 2018-09-25T20:47:21.703Z Reads: 149

```
[quote="Andy87, post:111, topic:66415"]
But don’t forget to cut the 5V wire on one side
[/quote]


What/where are you referring to? I'm not sure I had to do anything like that.
```

---
## \#117 Posted by: malJohann Posted at: 2018-09-25T21:24:12.161Z Reads: 154

```
I believe he’s referring to the middle/red/positive wire from one of the ESCs, because the BEC can only handle one voltage being reported? IDK much about RC TBH, only what I’m learning on the fly.

Anyway, got everything Loctited (if that’s a word) in the back last night, shafts and motorspurs with 638, bolts with 243, plus I added sugru around the motor mounting bolts to cover the air gaps, oh and I added the bumpers and test fit the ESC/RX mounting plate.

![image|666x500](upload://f8VRKD0hrdLmBL0uAALrF04Hp5g.jpeg)
![image|666x500](upload://2iQlNNN4imcLqZsvkSIaA44dZzB.jpeg)
```

---
## \#118 Posted by: ArnhemAnt Posted at: 2018-09-25T22:28:10.344Z Reads: 149

```
[quote="malJohann, post:117, topic:66415"]
I believe he’s referring to the middle/red/positive wire from one of the ESCs, because the BEC can only handle one voltage being reported?
[/quote]


Got any pics of this? I don't think I did that to my setup.

Bumpers looks good man. I'd like to get some one day.
```

---
## \#119 Posted by: malJohann Posted at: 2018-09-25T23:04:06.734Z Reads: 153

```
Different ESCs and RX, but same concept as bottom right on this pic.

https://gr33nonline.files.wordpress.com/2016/03/dualescbec_wiring_diagram.png
```

---
## \#120 Posted by: malJohann Posted at: 2018-09-25T23:07:28.805Z Reads: 147

```
Source: https://gr33nonline.wordpress.com/2016/03/10/becs-and-escs/
```

---
## \#121 Posted by: malJohann Posted at: 2018-09-25T23:31:35.472Z Reads: 144

```
Looking at that article though, the BEC is in the ESC and is used to power things like the RX, so you connect only one to avoid frying your RX is what I’m guessing.
```

---
## \#122 Posted by: ArnhemAnt Posted at: 2018-09-26T02:51:44.009Z Reads: 144

```
Yep, cool. So you are using a 'Y' spitter cable over PPM? I am connecting my two ESC's via CanBus so that is why I was unaware of what you were talking about.
```

---
## \#123 Posted by: Andy87 Posted at: 2018-09-26T03:31:26.345Z Reads: 142

```
If you have a Y-split cable for your receiver, you want the 5V only from one vesc.
That’s why you need to cut the 5V wire on one site.
If you run via CAN and use a normal cable for your receiver you don’t have to do anything
```

---
## \#124 Posted by: malJohann Posted at: 2018-09-26T11:17:43.435Z Reads: 151

```
Traxxas waterproof RX box.

![image|375x500](upload://824B5qeTQqdclUp2Ql5JFwkDxCZ.jpeg)
```

---
## \#125 Posted by: malJohann Posted at: 2018-09-30T08:55:37.849Z Reads: 149

```
ESCs, RX and waterproof box mounted. Now to sort the wire spaghetti and do some soldering.

![image|375x500](upload://hYxt5VtJ5WP7fnrtTTfsZhAofGz.jpeg)
![image|375x500](upload://f2uZK5JSLMP8WAa8SwmEGw0jT75.jpeg)
![image|375x500](upload://4XUH9cl64jjmuZNE60cqfwOd3qx.jpeg)
```

---
## \#126 Posted by: malJohann Posted at: 2018-09-30T09:06:37.266Z Reads: 144

```
I’ll say one thing, when my Kinchrome hex key gave up and went round, the Wera replacement rounded some of the screws and not a scratch on the key. That’s another thing I had to buy though.
```

---
## \#127 Posted by: malJohann Posted at: 2018-09-30T12:49:37.677Z Reads: 148

```
Tidied up and mounted, plus a neat solution for my motor wires direct mounted to the e-toxx drives with 12mm hex cap bolts, some heat shrink and plastic ties.

![image|375x500](upload://w3h0tUDIiwv6IHueDgo1N9sSL18.jpeg)
![image|375x500](upload://3hzIBW512uiHdzN6fsUhnt5Y2EI.jpeg)
```

---
## \#128 Posted by: malJohann Posted at: 2018-09-30T12:53:25.951Z Reads: 144

```
Also, LOVE these tools.

![image|666x500](upload://useUrjDWaoIuGQ48ZhYoEP5x94D.jpeg)
```

---
## \#129 Posted by: Andy87 Posted at: 2018-10-01T09:52:14.234Z Reads: 144

```
best investigation :+1:
```

---
## \#130 Posted by: malJohann Posted at: 2018-10-01T21:19:49.094Z Reads: 151

```
Need to buy solder wick today for a less than desirable job last night. I couldn’t close the connector tail over the joints the way it was designed to.

Also, holy cable management batman! How do I make it look a little less like a science experiment?

![image|375x500](upload://ePPf9lZNkOIE5gGQNceRlK9sBO8.jpeg)
![image|375x500](upload://6EbAwhiYP8DYpe4TJSQCYKnC8cU.jpeg)
```

---
## \#131 Posted by: Andy87 Posted at: 2018-10-02T06:58:00.691Z Reads: 144

```
i like the look of the esc with the cables coming out in the back to the top... :sunglasses:
why you fixed the cables from the motors on the gear drive and not only root them up to the esc? 
just add some cable protection and it will look a bit less like science :joy::sweat_smile:
```

---
## \#132 Posted by: malJohann Posted at: 2018-10-02T07:29:20.817Z Reads: 146

```
The wires from the motor are solid copper and inflexible, they’re attached to the drive to prevent breakage in the motor can where they connect to the internals.

The silicone encased wires attached after the MT60 connector are flexible and will allow for movement without breaking.
```

---
## \#133 Posted by: malJohann Posted at: 2018-10-02T14:05:27.661Z Reads: 149

```
This soldering stuff is hard work! Not going to be the cleanest build to start off with, but it’ll work.

![image|375x500](upload://ujaNMpqrMvb2lAEXOQD894VuTwj.jpeg)
```

---
## \#134 Posted by: Andy87 Posted at: 2018-10-02T16:19:55.778Z Reads: 141

```
Are those Graphen lipos? 
How you plan to mount them?
```

---
## \#135 Posted by: malJohann Posted at: 2018-10-02T20:04:35.630Z Reads: 142

```
Yes, 2x Turnigy 6,000mAh 4S Graphene LiPos mounted to make 8S1P (might go 8S2P later).

I plan to Velcro them sideways to the top middle of the deck as they are, unless I have to seal them first.
```

---
## \#136 Posted by: malJohann Posted at: 2018-10-05T23:48:53.489Z Reads: 145

```
It powers up! I also added the TPU drive guards, after getting the M4x8mm bolts I was after.

Now to make the wiring look acceptably neat, build the remote into its smaller casing, and do the anti-puncture and balancing of the wheels.

![image|375x500](upload://s00STNmtQMPnidLuAP7P6wuvWoG.jpeg)
![image|375x500](upload://c8ndBt07CoRUyAhkpvFWNka5f8P.jpeg)
```

---
## \#137 Posted by: malJohann Posted at: 2018-10-06T13:31:52.810Z Reads: 144

```
Remote built. Took me about an hour, including pack out and pack up. I don’t have a workbench. Yet.

![image|375x500](upload://8C639jNnnsJoB2qaRmdyRQM4eCS.jpeg)
![image|375x500](upload://iXhNOxiTHyTruchOhmCz0Ou7fGB.jpeg)
![image|375x500](upload://Ar68IEpbEAkFE32yCit8icWTeSx.jpeg)
```

---
## \#138 Posted by: malJohann Posted at: 2018-10-07T00:28:46.426Z Reads: 141

```
Note to self: When binding and calibrating remote connection, wait for wheels to stop before setting it down.

DON’T DO BURNOUTS ON THE DINNER TABLE! #likelytocausetroublewiththewife

![image|375x500](upload://boePAaf0UCxma0uT9LwqzG6MRh5.jpeg)
![image|375x500](upload://2jhkP59ZfovUBbhtxXSt2Td2naB.jpeg)
```

---
## \#139 Posted by: malJohann Posted at: 2018-10-07T07:47:31.324Z Reads: 141

```
FUUUWOW! It’s alive! Thought I’d ease into it at punch level 1 and 50% brake, plus careful trigger use, but it still kicks ass!

No smoke either, which is always a bonus on your first build. Need to do something about tidying up that wiring some.

![image|666x500](upload://8q5kWp0Q5WoFKhzlitJTkmxZrEP.jpeg)
![image|375x500](upload://vGWlixDM9LAJeNydm8UvVlsNb7R.jpeg)
```

---
## \#140 Posted by: malJohann Posted at: 2018-10-07T20:18:41.073Z Reads: 139

```
Did my first morning commute to the train station. Sounds like I’m from the future with these ESCs! High speed stability suffered a little with the green dampas, but turning radius still sucks. I see some @Nowind elastomere replacements in my near future.

Acceleration is truly brutal, be respectful of technology level brutal. I’m going to be learning better trigger control, but can already see that I’ll be creating a PWM controller soon. I can at least code (17 years experience), so maybe it’ll be a holiday project.

Brakes are good except at low speed, doesn’t come to a full stop, wonder if the drag brake setting can sort this out. I had a little bump with a pole due to this and the poor turning radius, lucky it was only like 3km/h and I have the e-toxx bumper.

This is what I should have done from the start, NO comparison to the Evolve BGT. For one, I can fly up a hill, so much better than sagging up a hill. I have a 26% gradient hill just before I’m home, so it’s important.

Question, does the Max6 ESC convert braking into noise and heat? Because I had full brakes on a full charge, so assuming its not regenerative.
```

---
## \#141 Posted by: malJohann Posted at: 2018-10-09T05:04:24.089Z Reads: 139

```
This remote though, can’t shake the mental image.

![image|449x500](upload://3GbodaeX5PTi30iX9kaBPSSvBgc.jpeg) ![image|375x500](upload://Ar68IEpbEAkFE32yCit8icWTeSx.jpeg)
```

---
## \#142 Posted by: malJohann Posted at: 2018-10-09T20:28:56.261Z Reads: 134

```
If the board is braking at neutral throttle, brake setting 100% drag 0%, then calibration is off correct? I should be able to coast?
```

---
## \#143 Posted by: ArnhemAnt Posted at: 2018-10-09T20:48:30.816Z Reads: 134

```
[quote="malJohann, post:142, topic:66415"]
I should be able to coast?
[/quote]


Yes, you should be able to coast. I don't have any experience with those ESC's, but my setup, with the same drive unit, and dual ESCapes allows me to coast and braking is not an issue.
```

---
## \#144 Posted by: malJohann Posted at: 2018-10-10T10:54:43.728Z Reads: 132

```
So, my ESC cut power on me today, low voltage cutoff setting on Auto(High). I got off immediately and switched the board off.

Now some say that even that setting is not good enough with Max6 ESCs, but my two packs were 14.05V and 14.58V when I plugged them into the B6AC chargers.

So for 4S that means all cells are above 3.5V, which means it is safe? Should I still get a voltage monitor? If so, which one?
```

---
## \#145 Posted by: Andy87 Posted at: 2018-10-10T11:02:28.245Z Reads: 136

```
I have this ones connected when I´m for a ride
https://hobbyking.com/de_de/hobbykingtm-lipo-voltage-checker-2s-8s.html
The voltage monitoring is +-0.04V off from the real value, but for the go it´s enough precise for me. 
You can easy programm the Voltage when it should start peeping and it´s cheap too.
```

---
## \#146 Posted by: davewood1982 Posted at: 2018-10-10T11:58:35.415Z Reads: 133

```
Plus dont necessarily trust the readings you get from your charger certainly at the beginning of a charge since  the balancing mostly takes place towards the end of the charge! if your batteries were 14.05V and 14.58V according to the charger its likely in reality they were probably a bit lower!
```

---
## \#147 Posted by: Pedrodemio Posted at: 2018-10-10T12:07:52.116Z Reads: 128

```
The raw finish of these gear drive together with the shiny sk3 is simply gorgeous, now I want something like it
```

---
## \#148 Posted by: malJohann Posted at: 2018-10-10T19:23:07.604Z Reads: 124

```
Thanks mate, appreciate the compliment! :slight_smile:
```

---
## \#149 Posted by: malJohann Posted at: 2018-10-12T02:40:00.357Z Reads: 130

```
Having a calibration issue with my TX / RX / ESC. Having followed the Max6 calibration procedure correctly, my brakes engage when throttle is only lightly reversed. The trigger feels overly sensitive and dangerous.

About 25% travel to the braking side gives full brakes and a green light. Further than that ESC lights turn red and I sometimes get reverse, while full travel sees light go off. Applying full throttle get’s green.

@Nowind you have a lot of experience with these, could it be remote throttle trim? Why would the lights on my ESCs go off at full brake position?
```

---
## \#150 Posted by: Nowind Posted at: 2018-10-13T03:24:04.834Z Reads: 127

```
Which Remote?

Are you using reverse?
I would not advice, forward/brake best.
Do a calibration again.
```

---
## \#151 Posted by: malJohann Posted at: 2018-10-13T03:48:26.720Z Reads: 130

```
HK-GT2B. How do I switch reverse off? The lowest setting on the Max6 ESC is 25%.
```

---
## \#152 Posted by: Nowind Posted at: 2018-10-13T03:59:28.812Z Reads: 137

```
With the Prog Card.
Choose Forward/Brake

Remote is good.
Re Calibrate again without the Reverse
```

---
## \#153 Posted by: malJohann Posted at: 2018-10-14T00:37:01.790Z Reads: 134

```
Done. Calibration sorted. Thanks!

As an aside, I thought I’d weigh the complete setup.

![image|666x500](upload://sF7M5ZXit1j3AvPMC39Vi9m8yrQ.jpeg)
```

---
## \#154 Posted by: Riako Posted at: 2018-10-14T14:58:30.862Z Reads: 130

```
That is really realy awesome mate !! For a mtb its a really good light weight :+1: Well done & Enjoy !!!
```

---
## \#155 Posted by: malJohann Posted at: 2018-10-14T20:14:18.969Z Reads: 135

```
Didn’t know it was such a big deal honestly, just posted it because it’s about 2.5kg more than the Evolve Bamboo GT with AT wheels I had before.

Here’s the first pic of my board in the wild, waiting for a train to go 50km to the CBD. Having e-toxx bumpers on both sides is so good.

The front already spared my hanger some light damage, and the rear is so handy for tail standing and obviously protecting the motors.

![image|374x500](upload://pVIHrN0AxmgXpZJr01P12HPxJWu.jpeg)
```

---
## \#156 Posted by: malJohann Posted at: 2018-10-17T11:55:01.124Z Reads: 135

```
I’m a somewhat simple man. I do what works best with the least effort.

![image|666x500](upload://6AWR1rE4Oz6VyNzBMQc0qRofmYT.jpeg)
![image|666x500](upload://nD4OsPzprqcwjaASRFgvY7Cq45b.jpeg)
![image|666x500](upload://y7OksFZLqPEPPVzMEbNDTfXOq5k.jpeg)
```

---
## \#157 Posted by: malJohann Posted at: 2018-10-18T12:24:55.008Z Reads: 128

```
Anyone here that have experience with the standard Trampa inner tube valve cores being crap?

All my wheels let themselves down within a week, and I now have damage on one of my rims.

Didn’t notice until it was too late, and because I didn’t expect it TBH.
```

---
## \#158 Posted by: Andy87 Posted at: 2018-10-18T12:30:13.945Z Reads: 128

```
I once had a problem that the inner tube was damaged by the rims. the tube got inbetween of the two parts of the rim and caused a cut in the tube.
Have a look if not the tube has small cut´s or holes.
```

---
## \#159 Posted by: malJohann Posted at: 2018-10-18T12:48:02.066Z Reads: 126

```
Deflates too slowly for a damaged inner tube.
```

---
## \#160 Posted by: malJohann Posted at: 2018-10-18T23:53:13.053Z Reads: 134

```
Anyway, inflated the tyres yesterday, didn’t lose much pressure overnight. Rode it in today, but will keep an eye on it.

![image|666x500](upload://ivFNLvV4CTiBYw12YvcdBn9NaNf.jpeg)

A pic of the visible damage, could clearly only have happened with a deflated tyre to deflect that much at the bead.

![image|375x500](upload://lGIybpRhO9k9SnAPls3vdKgyT88.jpeg)

Also got reminded this morning when carrying it by the front foot binding up some stairs, that griptape can bite.

![image|375x500](upload://Al9k1rV1goiDNIVc9P5g0N4W1yg.jpeg)

Might just end up re-coreing the tyre valves this weekend.
```

---
## \#161 Posted by: Blacksheep Posted at: 2018-10-19T00:24:16.486Z Reads: 129

```
Where did you buy the battery ?
```

---
## \#162 Posted by: malJohann Posted at: 2018-10-19T00:25:12.188Z Reads: 129

```
Two Turnigy Graphene batteries from Hobbyking.
```

---
## \#163 Posted by: Blacksheep Posted at: 2018-10-19T00:26:23.801Z Reads: 130

```
The one from the control hehe
```

---
## \#164 Posted by: malJohann Posted at: 2018-10-19T01:12:46.445Z Reads: 129

```
The rechargeable battery for the HK-GT2B came with the controller.
```

---
## \#165 Posted by: malJohann Posted at: 2018-10-25T06:08:15.583Z Reads: 125

```
So bought my next step in the evolution of this build, and with a view to possibly create a commercial product out of this.

Waiting for my gray M5Stack to arrive, had to have something to tinker with while on holiday in December.

Note that this is a development platform, and the final product will likely be custom.

![image|500x500](upload://tkGReCqhu6JvEeE3VXUb7hDwOPM.jpeg)
```

---
## \#166 Posted by: Andy87 Posted at: 2018-10-25T06:23:52.490Z Reads: 121

```
Sorry for the noob question, but what is it?
```

---
## \#167 Posted by: malJohann Posted at: 2018-10-25T09:14:14.002Z Reads: 114

```
Its an electronic product development platform with a 32 bit dual core microprocessor, colour screen, 9 axis accelerometer and various forms of input and output (including BLE and WiFi) that can run Arduino or Micropython natively, and control peripherals like LEDs, servos, brushless motors, various sensors and a lot more.

I’m envisioning a throttle management unit with mode switching initially, and later down the road possibly wheely control, traction control, and electronic diff for dual or quad builds.
```

---
## \#168 Posted by: Andy87 Posted at: 2018-10-25T09:19:39.592Z Reads: 111

```
Sounds promising 👌
```

---
## \#169 Posted by: mourges Posted at: 2018-10-26T22:33:07.771Z Reads: 105

```
This is so close to what I am thinking of building - although I'm not planning on doing direct drive.  The batteries are cool - what's the range been so far?
```

---
## \#170 Posted by: malJohann Posted at: 2018-10-26T22:47:40.518Z Reads: 114

```
7km to empty last time I checked, but then the next day I noticed my tyres were flat. So I guess more under normal conditions.

Also take into consideration I go almost flat out all the time, with a commuting weight of nearly 100kg, and have to climb two hills with some slight upward slopes in between.

The climb including the slopes is about 700m, of which 100m is at 26% gradient.
```

---
## \#171 Posted by: mourges Posted at: 2018-10-26T23:39:26.750Z Reads: 108

```
I travel quite a bit for work so was considering 4 of these batteries which would give me the range I want, and according to qantas, I could fly with them as carryon with my board in oversize luggage.  Winning!
```

---
## \#172 Posted by: davewood1982 Posted at: 2018-10-27T00:01:15.085Z Reads: 112

```
i had same esc and battery configuration, i got 6 miles from mine , i  just recently added 2 more *Graphene* packs (in parallel) so now i get 12 miles
```

---
## \#173 Posted by: ArnhemAnt Posted at: 2018-11-02T22:02:38.674Z Reads: 103

```
[quote="malJohann, post:170, topic:66415"]
The climb including the slopes is about 700m, of which 100m is at 26% gradient.
[/quote]


Do you mind sharing your settings for motor (min and max) and battery (min and max)? I'm interested to see what you are using.
```

---
## \#174 Posted by: malJohann Posted at: 2018-11-02T22:59:51.628Z Reads: 109

```
I’ll have to connect my WiFi programmer to check, but from memory I only changed mode to Fwd+Brake, battery cutoff to Auto(High), and the direction of one of the motors.

Not many settings on these ESCs, unlike the VESC based ones. Plenty of power and torque throughput though. Very basic beasts these.

What do I do to protect my batteries from over discharge? Go only 4km instead of the 7km it runs to cutoff, so I’m not running them right down.

What did I do to protect the batteries from too high rate of discharge? Spec them to provide more thsn the peak 160A discharge per ESC.
```

---
## \#175 Posted by: malJohann Posted at: 2018-11-02T23:02:13.649Z Reads: 104

```
What do you do for charging? I want to add two more packs, but don’t want to add two more hours to charging. I have two B6AC chargers, so can’t charge 8S. Can I charge 4S2P, or do I have to charge individual packs only?
```

---
## \#176 Posted by: Andy87 Posted at: 2018-11-02T23:13:28.595Z Reads: 103

```
Maybe you can just add a lipo alarm and set it to 3.5v. With it you could get some more kilometers without over discharge your packs. 4km seems a bit less.
```

---
## \#177 Posted by: Andy87 Posted at: 2018-11-02T23:15:45.517Z Reads: 99

```
You can charge parallel but the packs need to have the same initial voltage.
The charging time will non the less double as you have more capacity to charge and your charger is limited to 60watt i think.
```

---
## \#178 Posted by: malJohann Posted at: 2018-11-02T23:23:08.301Z Reads: 97

```
[quote="Andy87, post:176, topic:66415"]
4km seems a bit less.
[/quote]

Fit for purpose at the moment, I only go 4km per day, which is my commute distance.

[quote="Andy87, post:177, topic:66415"]
You can charge parallel but the packs need to have the same initial voltage.
[/quote]

Why? I have balance chargers, which should be able to handle voltage mismatch?
```

---
## \#179 Posted by: Andy87 Posted at: 2018-11-02T23:32:21.910Z Reads: 101

```
Yes but if in pack 1 cell 1 is 3.5v and in pack 2 cell 1 is 3.7v I doubt the balance charger can bring them on one level.
It’s like with LiIon packs. If you have a 10s4p for example, you have one balance lead for 4cells. Means the bms balance the packs not the individual cells. If one cell in the 4p pack is bad your balance charger can’t handle that.
If to come back to the case I wrote before your balance charger will probably see the average voltage which is 3.6 and balance that up till reaching 4.2v. The thing is that then one cell is 4.1 and the other 4.3 when fully charged.
Idk how much the cells in parallel can balance each other, so maybe there will be a bit less difference but in general I understood it like that.
```

---
## \#180 Posted by: MotorJunkie Posted at: 2018-11-02T23:39:14.721Z Reads: 99

```
Nice building buddy! I'm the same weight as you maybe 5 lbs lighter. If most of your commute was flatter terrain, what motors would you have opted for?

Also, I'm a noob. I have to ask why you decided on Maxx instead of Vesc6?

Cheers!
```

---
## \#181 Posted by: malJohann Posted at: 2018-11-03T00:03:03.384Z Reads: 101

```
Thanks mate. Most of my commute is flat terrain, two thirds actually. I could have gone smaller motors, nobody really NEEDS 8kW+. Dual 6355 would have been more than enough.

I went Max6 and dual 6374 because I drew inspiration from @Nowind doing power wheelies on YouTube LOL! Instant torque and 160A output each FTW! Also Max6 is waterproof.
```

---
## \#182 Posted by: davewood1982 Posted at: 2018-11-03T02:53:05.079Z Reads: 104

```
i bought  a parallel charging board to do all 4 batteries at once, i 1st tryed charging all 4 on my B6AC charger but it look over 6hrs to charge on a parallel board, so i bought a more powerful charger and it now i can charge all 4 up in 2hrs using a parallel charging board! 

if you can't afford a a new a charger then you could just buy two parallel boards and use 1 for each B6AC charger so your charging 2 batteries on each charger,
```

---
## \#183 Posted by: davewood1982 Posted at: 2018-11-03T03:12:14.879Z Reads: 108

```
this is really good video and it explains how parallel charging works really well. 

https://www.youtube.com/watch?v=mRlsaD5tf_8&t=577s
```

---
## \#184 Posted by: malJohann Posted at: 2018-11-05T04:05:27.349Z Reads: 117

```
My holiday project has arrived. Now to code the initial ride modes.

![image|375x500](upload://4W2XPgHSRuCBl7s2b0tV3gtwYrg.jpeg)
![image|375x500](upload://bWD4CQ2hUiaMlAmFM0UuCENIhsY.jpeg)
![image|375x500](upload://7JXRE7cacZnz649BaELvN6FLaeU.jpeg)
![image|375x500](upload://3cAB5qnznAFHT6gGMK5MLOZ9tNu.jpeg)
```

---
## \#185 Posted by: mourges Posted at: 2018-11-05T21:50:13.252Z Reads: 109

```
I haven't seen the M5Stack before - looks quite promising and expandable.  Have you used them before?
```

---
## \#186 Posted by: malJohann Posted at: 2018-11-05T23:14:31.385Z Reads: 114

```
Nope, but up until less than 2 years ago, my day job for the 17 years before that was analyst programmer, so I won’t be completely useless. ;)

I’m going to re-flash this one to run Micropython on baremetal though, so won’t be using the pre-installed Arduino platform.

Check out these pics, looks very promising and capable. Dual core too.

![image|375x500](upload://P90m73y2a7nOoVynbJSAyfIU9a.jpeg)
![image|375x500](upload://7P3pCNCC00edPvQAw2y2CegMuk8.jpeg)
![image|375x500](upload://pLa83kO9hjxJutMeSv3MSiYsLlx.jpeg)
```

---
## \#187 Posted by: davewood1982 Posted at: 2018-11-06T01:32:47.881Z Reads: 100

```
Presumably its for the esc? what exactly is it and whats for?
```

---
## \#188 Posted by: malJohann Posted at: 2018-11-06T04:24:26.755Z Reads: 103

```
Its a modular microprocessor with WiFi, BT, 9-axis accelerometer, buttons and a screen with I/O ports to control hardware peripherals.

Initially I’ll use it between RX and ESC to control PWM, enabling different throttle/braking curves and modes. Then more capabilities later.
```

---
## \#189 Posted by: ArnhemAnt Posted at: 2018-11-06T05:26:29.852Z Reads: 103

```
[quote="malJohann, post:188, topic:66415"]
enabling different throttle/braking curves
[/quote]


Does this mean that you can alter the amount of current that goes back into the battery, when braking, depending on the stage of your on-board battery?
```

---
## \#190 Posted by: malJohann Posted at: 2018-11-06T05:53:28.094Z Reads: 103

```
No, it wouldn’t replace the capability of the BMS, rather add some to the RX, and then some of its own via other sensors. It’ll only be used to change the signal to the ESCs, later with input from optical and accelerometer sensors.
```

---
## \#191 Posted by: pixelsilva Posted at: 2018-11-06T08:00:46.572Z Reads: 110

```
> @Kug3lis
> 
> Be careful with **APS** 6384 200kV both of them got loose magnets within a 2 weeks 

You mean, those spensive chinese motors 'manufactured' in England by a renown british electric motor company! :roll_eyes:
```

---
## \#192 Posted by: mourges Posted at: 2018-11-10T05:15:46.540Z Reads: 101

```
Launch control, boost when heading up hills, etc
```

---
## \#193 Posted by: malJohann Posted at: 2018-11-10T08:49:20.057Z Reads: 101

```
Mostly limits and controls, boost can be done by the user, not sure I’d want to make the decision on when to boost, much more comfortable with limiting too much power though.
```

---
## \#194 Posted by: malJohann Posted at: 2019-01-09T04:18:01.728Z Reads: 89

```
Objectives for this year:
1. Finish ECU project to a working prototype, initially with only different engine response modes. Not sure where I’m going to find the time though.
2. Increase range with more LiPos, while making it as easy to charge as a laptop. Need a BMS that can handle anything from 1S2P to 4S2P charge. Need to find a charger that can balance charge the same, or the BMS should be able to handle 65C constant 130C burst discharge.

Any help or guidance with number 2 would be greatly appreciated.
```

---
## \#195 Posted by: Andy87 Posted at: 2019-01-09T04:56:11.596Z Reads: 87

```
I would go with a charge only bms.
If you have the space you could go with a smart bms so you could set your balance values and other things how you want and also display the individual cell voltage via pc or Android app
```

---
## \#196 Posted by: malJohann Posted at: 2019-01-29T10:39:58.053Z Reads: 85

```
Anyway, as covered in another thread, I stuffed my batteries over the holiday break by not giving them a storage charge.

I then bought 4x new Graphene 4S 5,000mAh batteries at 35% discount (combination sale and voucher) from Hobbyking.

So wired up it’s 8S 10,000mAh instead of the 6,000mAh I had before at only $40 more than the original cost.

Couldn’t get a BMS though, since they didn’t have stock. Any recommendations?
```

---
## \#197 Posted by: Andy87 Posted at: 2019-01-29T12:19:55.330Z Reads: 83

```
You looking for a charge only bms or charge/discharge bms?
If discharge, how much amps you want to have as max limit on the bms?
```

---
## \#198 Posted by: malJohann Posted at: 2019-01-29T12:37:47.952Z Reads: 86

```
I need to be able to dump 2x 160A at up to 33.6V under full load, so thinking of charge only, but it should be able to balance cells up to 8S5P which could be up to where I scale, although currently it would only be for 8S2P.
```

---
## \#199 Posted by: Andy87 Posted at: 2019-01-29T12:43:47.421Z Reads: 85

```
http://www.bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/BMS-D170V1%20with%20Relay.html
😅😅😅
Ok i will look for something else
```

---
## \#200 Posted by: Andy87 Posted at: 2019-01-29T12:48:18.726Z Reads: 84

```
If 15a charge and 84mA balance current is enough for you than I think the d140 from bestech would still work fine.
http://www.bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/BMS-D140.html

Edit: or as suggested before you could get one of this smart bms 
https://s.click.aliexpress.com/e/cGAybLgm
Just make sure that they sent you the bms set up for lipo not lifepo4 as it says in the description.
I just sent a message to the shop and I got one with the confit for lipos.
```

---
## \#201 Posted by: Andy87 Posted at: 2019-01-29T12:50:05.845Z Reads: 78

```
 [quote="malJohann, post:198, topic:66415"]
dump 2x 160A at up to 33.6V
[/quote]

... with this you made me curious 😅
What’s your plans for this year to hit that current?
Sounds definitely interesting 😅👌
```

---
## \#202 Posted by: malJohann Posted at: 2019-01-29T19:58:38.637Z Reads: 79

```
That’s my setup today. 33.6V because individual cells CAN get up to 4.2V each although not recommended, and my ESCs put out 160A each which is why I get over 8kW with two motors on 8S configuration.
```

---
## \#203 Posted by: Andy87 Posted at: 2019-01-29T21:22:10.061Z Reads: 76

```
But your motors rated only to 80a.
What about that?
```

---
## \#204 Posted by: malJohann Posted at: 2019-01-30T05:56:51.294Z Reads: 82

```
Oh, didn’t see that. You mean that I could achieve the same performance with one ESC and for phase I do y-wires, or doesn’t it work like that?

So at 80A and 29.6V per motor I’m only pushing 4.7kW combined? Man! Now I wonder what 8kW+ feels like!
```

---
## \#205 Posted by: Andy87 Posted at: 2019-01-30T06:15:21.315Z Reads: 86

```
No you need 1 esc for each motor.
But even if your esc can handle 160A it doesn’t mean that you actually draw that current all the time. I think your esc work the same like a vesc when it comes to current regulation.
If you drive on a flat road you push probably less than 30a through your esc, what means also your current drawn from the battery is somewhere around that and not 160a.
I don’t know in how far you can program your esc, but for example if you have a vesc and your motor is rated to 80a (most 6374 motors rated between 60-80a) you set your motor max current to 80a.
```

---
## \#206 Posted by: malJohann Posted at: 2019-02-08T11:37:54.166Z Reads: 81

```
![image|375x500](upload://wXwT0puWzf1obyzw2Mpywlx2E3s.jpeg)
```

---
## \#207 Posted by: malJohann Posted at: 2019-02-08T22:36:57.077Z Reads: 78

```
Now for a BMS. I’ll start riding it before I have one, but I’ve got a bit of an under-mounted transformation in mind. My current use doesn’t come close to using the deck flex, even so when under-mounting I’ll custom make an enclosure.
```

---
## \#208 Posted by: danepoostain Posted at: 2019-03-27T18:33:50.913Z Reads: 66

```
Awesome build! Can you explain the beads in the wheels? Is it for speed wobbles? Also what type of lubrication are you using on the internal gear of your drive system?
```

---
## \#209 Posted by: malJohann Posted at: 2019-03-28T04:10:31.198Z Reads: 62

```
Thanks mate! The beads are for balancing, although I haven’t put them in. Been so very busy the last two months, my new batteries aren’t even fitted yet.
```

---
## \#210 Posted by: malJohann Posted at: 2019-07-03T17:42:58.165Z Reads: 42

```
Thinking of selling the LiPos and going LiFePO4. Is the 8S limitation on my ESCs due to voltage? If so, can I go 9S LiFePO4 to make up for some of the voltage drop?
```

---
## \#211 Posted by: malJohann Posted at: 2019-09-30T10:19:42.851Z Reads: 21

```
This thread moved: e&ZeroWidthSpace;sk&ZeroWidthSpace;8&period;n&ZeroWidthSpace;ews
```

---
